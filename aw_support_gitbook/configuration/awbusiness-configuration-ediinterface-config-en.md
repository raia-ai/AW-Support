---
description: "EN-CONFIG-AW_Business-8"
---


---
### Fig. 113: Product stock dimensions

**Produkt-Lagermasse (BA_LAGMA)**

| Artikel | Abmessung | Durchschnittspreis ermitteln | abw. Preis-Schlüssel |
| :--- | :--- | :--- | :--- |
| 1004 | 3210 x 6000 | JA | Lagermaße |
| 1004 | 3210 x 3000 | NEIN | <k.A.> |
| 1004 | 3210 x 2000 | NEIN | Lagermaße |

### Fig. 114: Inventory management

**Lagerverwaltung (LG_LAGERORTE)**

| Artikel | Abmessung | Bestand | Teilnahme an gesamt Durchschnittspreisermittlung | Durchschnitts-Preis |
| :--- | :--- | :--- | :--- | :--- |
| 1004 | 3210 x 6000 | 100 Stk | JA | 1,25 EUR/qm |
| 1004 | 2000 x 2000 | 40 Stk | JA | 1,84 EUR/qm |
| 1004 | 1500 x 3000 | 45 Stk | NEIN | 1,99 EUR/qm |

Gew. Durchschnittspreis für Artikel 1004:
`(3210*6000*100*1,25 + 2000*2000*40*1,84) / (3210*6000*100 + 2000*2000*40*1,84) = 1,30 EUR/qm`

### Fig. 115: Price management

**Preise laut Tarifzuordnung in Preisverwaltung (PR_PREIS)**

| Preisschlüssel | Preis |
| :--- | :--- |
| Standard | 1,50 EUR/qm |
| Lagermaße | 1,00 EUR/qm |

### Fig. 116: Example order

**Beispiel-Auftrag mit den ermittelten EK's:**

| Pos. | Artikel | Abmessung | Preis-Schlüsselvorgabe | EK |
| :--- | :--- | :--- | :--- | :--- |
| 1 | 1004 | 3210 x 6000 | nein | 1,25 EUR/qm |
| 2 | 1004 | 2000 x 2000 | nein | 1,44 EUR/qm |
| 3 | 1004 | 3210 x 3000 | nein | 1,50 EUR/qm |
| 4 | 1004 | 3210 x 2000 | nein | 1,00 EUR/qm |
| 5 | 1004 | 1250 x 1433 | nein | 1,30 EUR/qm |
| 6 | 1004 | 3210 x 6000 | ja (Lagermaße) | 1,00 EUR/qm |

## 5.7. Imputed freight costs

The program Imputed Freight Costs offers two functions. These functions serve to determine the imputed freight costs for orders and print them in the shape of lists, and also split forwarding costs to orders.

**Description of the functions:**

1.  **Calculation and printing of imputed freight costs**

    The first function serves to determine and print the imputed freight costs for a certain number of orders. The number of orders is selected by delivery date, customer, and route. Please note that the imputed freight costs will be revised for every printout.

2.  **Splitting of forwarding costs:**

    The second function permits to split forwarding costs to a certain number of orders. The number of orders is selected based on delivery date and route.

**Notes:**

**Enabling the determination of imputed freight costs:**

The decision as to whether or not imputed freight costs shall be determined for an order, is based on the route selected for the order. Decisive is the entry in column €/km in route master data. If the entry in column €/km is over 0, imputed freight costs will be determined for the order. Otherwise, there will be no calculation.

**Order entry**

Imputed freight costs are determined at order entry for the first time. When an order is entered, the imputed freight costs will be determined for the present order and the associated orders of this customer for the same delivery date and route. Order entry offers a new menu item, `Functions -> Imputed freight costs`. This entry can be used to open a list of imputed freight costs.

**Determining the imputed freight costs:**

Imputed freight costs are calculated radial. The distance between the site and every single customer will be taken into account. Example: If the distance from a customer is 50km and a value of € 1.5/km has been defined for this route in route management, the imputed freight cost for this order would be € 75. If the customer has placed more than one order for the same delivery date, these € 75 would be split onto the individual orders, based on the glass surface of the orders.

**Splitting of forwarding costs:**

The forwarding costs will be split onto the individual orders, in relation to the distance to the customer and the glass surface to be delivered.

## 5.8. Down payments

### 5.8.1. Operation

Deposits are created by means of the module "Copy documents". A new document is created in which the items of the original order are listed. The deposit amount is a separate item.
Numbers for deposit invoices are taken from the partial invoice number area.

A new status has to be defined, and allocated to status point 89 The status must lie below the invoicing status.

The deposit product must be defined as „service“, product group „deposit“. No discount should be possible.

It has to be entered in product allocation ‚surcharges' as down payment.

Use system text 50 and 51 to enter invoice data for the item.

> 50 Invoice <ar> dated <ard> for deposit dated <ad>
> 51 deposit of for order <aa> of <aad>
>
> <ar> = deposit invoice number
> <ard> = deposit invoice date
> <ard> = deposit invoice date
> <aa> = deposit order number
> <aad> = deposit order date

Correct printout requires some changes in the form. Example: Rechn.qrp in the details block. Essential is the print condition in the old item line.

**New variables:**

| Variable | Type |
| :--- | :--- |
| DEPOSIT_HEADER | integer |
| DEPOSIT_ITEM | integer |
| ZW_BETR_NETTO | integer |
| ZW_BETR_MWST1 | integer |
| ZW_BETR_BRUTTO | integer |
| DEP_BETR_NETTO | integer |
| DEP_BETR_MWST1 | integer |
| DEP_BETR_BRUTTO | integer |

These variables are printed on the original invoice, as subtotals of the original items.

On the new deposit invoice, the original items will be printed (controllable via Options in Copy Documents) and the new deposit item.

## 5.9. Shape edge surcharges

### 5.9.1. Introduction and the problem

Many of our customers have a pricing method for edgework with which the shapes with slanted and round edges have a different price than those with rectangular or parallel edges. The reason for this is that this edgework has to be performed on special machines, which results in higher costs (CNC or one-side grinding machine instead of the efficient two-sided grinding machine).

Up to now, this problem has been solved in a manner so that the customer has several edgeworks (straight shape edge, curved shape edge and rectangular edge). This results in a very complex process for the customer. The staff that enters data have this under control, but with the Web Configurator, we are addressing the end customer, who is not aware of this technical issue, which would inevitably lead to wrong entry with incorrect prices. There is therefore no other way than to simplify entry, i.e. to return to the essential information of which edges do I want to process how. The software must do everything else.

### 5.9.2. Setting up shape edge price surcharges

The shape segment surcharges are set up in the shape edge surcharges. This is done per shape and price table and rate.

*(Fig. 117: Shape edge surcharges - Screenshot of UI)*

### 5.9.3. Creation of shape edge qualities

During transfer to production, the individual processing has to be split into several processing. Only this way can the production software determine the different size allowances and machines.

*(Fig. 118: Shape edge qualities - Screenshot of UI)*

Only the deviating edge qualities have to be entered in the shape edge qualities. All other edges can stay set to "<n.e.>" and inherit the quality of the edgework from product management.

If deviating edge qualities are set up for edgework, they will also affect the SNLive sketch and SN file creation, i.e. the deviating edge qualities are also transferred to the A=W CAD Desginer (Shapes).

### 5.9.4. Order entry pricing

Price calculation takes place by determining the single edge length and checking it against the minimum edge length or the minimum processing length. Please note that if we have a minimum length, the length of the edges are totaled that have the same surcharge. This is not the case with the minimum edge length.

**Exact calculation**

Base price 9.20 pro lm, shape edge surcharge edge 3 100% and 30 measurement rounding

Length \* Price/lm \* same edge surcharge = individual price

| Calculation | Result |
| :--- | :--- |
| 1.02+1.02+0.51=2.55 lm \* 9.20€ \* 1.0(0%) | = 23.46 €/pc. |
| 1.14 lm \* 9.20€ \* 2.0(100%) | = 20.976 €/pc |
| **Total** | **= 44.436 =>44.44 €/pc** |

*(Fig. 119: Example of the exact calculation of shape edge surcharges - Screenshot of UI)*

**Non-exact calculation**

Base price 9.20 pro lm, shape edge surcharge edge 3 100% and 30 measurement rounding

3 x the length of 1.02 lm is calculated + 1 x 1.02 lm \* 2.0(100%)

The user can determine how often the shape edge surcharge is applied to the width and/or height. The system supports the user to the greatest extent possible of edge 3 is removed, the shape edge surcharge is also dropped.

Length \* Price/Im \* same edge surcharge = individual price

| Calculation | Result |
| :--- | :--- |
| 1.02+1.02+1.02=3,06 lm \* 9.20€ \* 1.0(0%) | = 28.152 €/pc |
| 1.02 lm \* 9.20€ \* 2.0(100%) | = 18.768 €/pc |
| **Total** | **= 46.92 =>44.44 €/pc** |

*(Fig. 120: Example of the non-exact calculation of shape edge surcharges - Screenshot of UI)*

**Calculating minimum lengths**

The calculation for the option Calculate minimum length is completed. Each edge is checked for the minimum length in accordance with the measurement rounding and, if necessary, it is increased and a surcharge is applied.

When calculating total minimum length however a problem occurs in the case of different shape edge surcharges. How should the minimum length and the surcharge be calculated, how is it to be distributed?

Solution: For all identical edge surcharges, the lengths are added and are checked against the minimum length, which corresponds exactly to the process used when single processings are entered.

Base price 9.20 pro lm, shape edge surcharge edge 3 100% and 30 measurement rounding with minimum length 1 lm (not per edge!!!)

Length \* Price/Im \* same edge surcharge = individual price

| Calculation | Result |
| :--- | :--- |
| 1.02+1.02+1.02=3,06 lm \* 9.20€ \* 1.0(0%) | = 28.152 €/pc |
| 1.02 lm \* 9.20€ \* 2.0(100%) | = 18.768 €/pc |
| **Total** | **= 46.92 =>44.44 €/pc** |

### 5.9.5. Effects on production transfer

Shape edge qualities cause the processing records to be split per edge quality in production transfer. Plus the decoration is now transferred for edgework with the quality OtherEdgeWork.

There are two different cases hereby, depending on whether the A+W capacity planning is active or not.

*   Without capacity planning, the processing record is checked for deviating edge qualities. If they are available, the processing record is split into various processing records (one per edge quality). Then the processing plans are recalculated and the processing texts are created, as changes may have resulted from the splitting.
*   With capacity planning, the processing is split on the basis of the scheduling data. Splitting takes place into as many work processes as assigned by capacity planning. Also the new edge lengths come from this data. In this case, the processing text is newly created for each processing.

**Configuration in A+W Production**

Up to now, the SN edge quality had always been read from the A+W Production master data of the processing and checked to see whether this edge quality also exists on the SN drawing. If there are several edgeworks with the same SN edge quality in the BOM, everything will work if the size allowance (irrespective of the assigned machine) is the same for every edgework.

Now we have the case that the same processing article has different edge allowances in the SN file and perhaps differing grinding surcharges are calculated. If such an item is imported, this will stop at scheduling with an error: "Contradictory grinding allowance for the same edgework in the drawing". [2507]“

Set the switch `[ALCIM_SHAPE / SNUSEORDERDECOFORAWTYPE1090]` to prevent this from happening:

*   **0:** The SN edge quality is read from the article master data (BEARBEIT_EXTRA1).
*   **1:** The SN edge quality is taken from the order, if the field `<decoration>` is filled in the transfer file and edge processing has been assigned to the A+W processing type 1090 (other edge processing).

*(Fig. 121: Configuration special edge in A+W Production - Screenshot of UI)*

**Example of an extract from an OrderXML file:**

```xml
<awProcessing typeID="Polishing" id="1010" category="Edgework" quantity="10.25" quantityUnit="MTR">
    <Polishing>
        <EdgeWork n="2" />
        <EdgeWork n="4" />
    </Polishing>
</awProcessing>
<awProcessing typeID="OtherEdgework" id="1090" category="Edgework" quantity="3.75" quantityUnit="MTR">
    <OtherEdgework decoration="12">
        <EdgeWork n="1" />
    </OtherEdgework>
</awProcessing>
```

**SN edge quality on laminated glass parts**

If edgework is performed on a laminated glass part, a different DECO number is attached to the SN drawing. This number is the respective number for laminated glass edgework. This happens when the SN drawing is directly generated by A+W Business or when scheduling in A+W Production. When determining the grinding surcharges in A+W Production, the surcharges are checks with both DECOS.

List of SN edge qualities and the implementation on laminated glass parts (Number in A+W Business and A+W Production always +1):

*   Special edges 11-16 → laminated glass 84-89
*   Special edges 18-27 → laminated glass 90-99
*   Special edges 100-131 → laminated glass 132-163

### 5.9.6. Setting up Business Capacity Planning

In the special allocations 2, different work types can be created for a processing and shape for different shape edges.

*(Fig. 122: Configuration special allocation 2 - Screenshot of UI)*

If A+W Business Time Management is being used, the distribution of the work processes in special allocation 2 must correspond to the different shape edge qualities. If one of the work processes has edges with different edge qualities, a message is output during transfer to production and no OrderXML file is generated.

*(Fig. 123: Message during transfer to production for faulty special allocation 2 - Screenshot of UI)*

## 5.10. Wastage rates for price calculation

In A+W Business Pro is it now possible to use the wastage rates detected by the production manager for the price calculation of quotations and subsequent orders. The scripts 20160509a.sql, 20160510a.sql, 20160511a.sql and 20160508aa.sql must be initialized in order to use the functions.

If a quotation is optimized with the Production Manager, the detected waste rates per glass type (= product number) in the table are now entered in the table BW\_ANGEB\_OPTI. The records of the selected optimization are given the value SELECTED = 1 and are therefore considered by the price calculation. The values of the other implemented optimizations with SELECTED = 0 are alternatives that can be used to compare the prices.

The determined rates therefore override the values entered in the product master data. If no (selected) values are available in the table for the document, the wastage rate from the master data still applies.

### 5.10.1. Management dialog

After the quotation has been optimized by the production manager, the wastage rate to be used for the price calculation can be subsequently determined in A+W Business. This allows the various prices to be easily compared and the selected price is directly transferred into the document. The dialog can opened from the document entry via `Functions > Wastage rates`.

In the dialog it is also subsequently possible to calculate the costs with a manual wastage value. For this, the required wastage factor must simply be recorded in the detail table under the entry "manual entry" and then selected. This can also be done if the quotation has not been optimized yet. It is also possible to use the value from the master data again by not selecting a record for the glass type.

The dialog implements a price calculation with each change so that the user does not have to do anything else than select the required wastage rates per glass type and confirm the dialog with OK. The purchase prices are also totaled per glass type and shown in the table for a better overview. This means the difference from the original price can be identified at a glance.

### 5.10.2. Document archiving and copying

The determined wastage rates are included in the archive when archiving documents and are also copied back when copying back from the archive. This ensures that the price is not changed when copying a document.

Copying a quotation to an order is an exception. Only the selected records are copied for the price calculation. Subsequent calculation with other previously determined wastage rates is no longer possible in the order.

## 5.11. Energy Surcharge

As from 1st November 2004, glassworks will charge an energy surcharge on glass. This surcharge will be applied per kilogram. The ALFAK2000 module, `Energy surcharge` allows to pass this surcharge on to the customers.

It allows the automatic creation of surcharge item 991. The surcharge can either be applied to glass, or to the weight of glass items. The surcharge will be calculated at order entry.

Should the amount of the energy surcharge change between input and delivery, the orders have to be corrected by means of program, `Recalculate documents`. This program offers a new option for this purpose, `Recalculate special discounts/surcharges`.

The surcharge can be defined for customers and suppliers, and can be enabled or disabled at document entry and in customer/supplier data.

No other automatic surcharges or discounts will be applied to the energy surcharge.

### 5.11.1. Rounding Parameters

As the surcharge is calculated with three digits after the decimal point, the rounding (digits after decimal point) of the price per price unit needs to be changed. If not already existing, a rounding rule with three digits after the decimal point has to be defined (illustr. 1) This will be entered in company roundings for rounding 1 (fig.2).

*(Fig. 124: Define rounding point - Screenshot of UI)*
*(Fig. 125: Rounding allocation - Screenshot of UI)*

### 5.11.2. Defining an Energy Surcharge Article

The energy surcharge article is defined as a service, the quantity unit is ‚pc.'. You have to allocate a product group that is not ‚000'. Splitting onto glass items in financial accounting/statistics is impossible.

*(Fig. 126: Product management - energy surcharge article - Screenshot of UI)*

The price has to be entered as price per kilogram.

*(Fig. 127: Energy surcharge - Price - Screenshot of UI)*

### 5.11.3. Entering the Energy Surcharge Article in Company Parameters

The energy surcharge article must be entered in tab Surcharges in Company Parameters.

*(Fig. 128: Energy surcharge - company data - Screenshot of UI)*

The surcharge calculation type, `only on glass weight` or, `on weight of glass/IG items` is set in tab 4 Documents.

*(Fig. 129: Energy surcharge - company data 1 - Screenshot of UI)*

### 5.11.4. Activating the Surcharge in Customer/Supplier Data

The energy surcharge has to be activated for every customer/supplier. This setting will be loaded at order entry, and can be changed there.

*(Fig. 130: Enable energy surcharge - Screenshot of UI)*

### 5.11.5. Order entry

The surcharge will be calculated and inserted when you leave item entry. To change the price, open item entry once more and change the price per price unit. The surcharge basis (the weight) is shown in item text 5, and can be printed after the form has been amended.

*(Fig. 131: Calculation after item entry - Screenshot of UI)*
*(Fig. 132: Surcharge basis - Screenshot of UI)*

### 5.11.6. Recalculation after a Change of Price

Orders entered prior to the price change, but have not been shipped so far, have to be transferred to a number manager. Now start program „Recalculate documents" with the option, `Calculate special discounts/surcharges`. All special discounts will be recalculated, including the energy surcharge. The item prices will not be changed.

*(Fig. 133: Recalculation of documents - Screenshot of UI)*

### 5.11.7. Changes in Version 4.1

Version 4.1 introduces some changes with regard to the energy surcharge. The surcharge is handled by the automatic special discount/surcharge logic introduced in 4.1. The advantages are:

*   Item number specification
*   The effects of the surcharges on another can be defined
*   Individual products can be excluded from the surcharge

The conversion of the old surcharge code in the customer master data is done automatically via update script. The energy surcharge has to be allocated manually, however. The energy surcharge code is set for the product type (1,2,3,50) for all orders and products. The energy surcharge product has to be entered in ‚product allocation surcharges'. Calculation is the same as in the previous version.

*(Fig. 134: Product surcharge allocation - Screenshot of UI)*

## 5.12. Tax calculation by Avalara Tax Service

In the United States, the calculation of the taxes depends on the locations of the seller and purchaser. It is still decisive in which region, in which country, and in which city the locations are located.

For this complex task, the activation of the Avalara Tax Service is described in the following. This service is a for-fee RESTful service from Avalara Inc. A_W Business transfers all relevant information for the document to this service and receives back the tax rates, tax basis amounts, and the tax calculated. The basis for the correct tax calculation is the so-called tax codes that must be entered in A+W Business for each product group. During the transfer, the tax code for each item is determined using the combi product group of the main product and transferred to Avalara.

**Product code management with the tax code for the transport**

Since the tax code is a new column, the script 20191029a.sql is absolutely necessary. The call of the Avalara service is done via a customizing for the tax calculation. For this, a formula in the customizing management, must be assigned the program point 52-Tax calculation. Starting from this moment, the tax calculation is no longer handled by A+W Business and must be done completely in the formula. An example can be found in the A+W Business formula folder with the name Tax\_Avalara.txt.

```
Set m nUdv [1] = 1;
! Check if the first m nKO STEUERFLAG is enabled. If not, start the regular tax calculation;
If NOT (m NKO STEUERFLAG & 1);
    Set m nUdv [1] = 0;
EndIf;

! Check if ShipTo address is inside the US. If not, start the regular tax calculation;;
If (m sAL LAND != 'US' AND m_SAL_LAND != 'US' );
    Set m nUdv [1] = 0;
EndIf;
If (m sAH LAND != 'US' AND m_SAH_LAND != 'US' );
    Set m nUdv [1] = 0;
EndIf;

If m nUdv [1];
    ! Only for testing, setting sandbox to true;
    Set m nUdv [0] = TRUE;
    udf AvalaraTax ( this, '255 S. King Street', 'Seattle', 'WA', 'US', '98104', m nUdv (0));
EndIf;

! Show errors that might have happened during transfer;
udf ShowResults ( MESSAGETYPE ERROR );

If NOT m nUdv [1];
    ! Standard tax caluclation instead of Avalara;
    udf_CalcStandardTax ( );
EndIf;
```

In this example, it is first checked whether the checkbox for the first tax rate in the document is activated and whether the goods are sent within the USA. If both are true, the function `udf AvalaraTax` is called. The transfer parameters to the function are the document itself (this) and the sending address. As last parameter it is specified whether the transfer is done to a test access of Avalara (true) or to the productive service (false). The function `udf ShowResults` is used to output any possible error messages that occur.

If one of the two criteria (sending within the USA or tax flag active) does not apply, the standard tax calculation will be performed by A\_W Business with the function `udf CalcStandardTax`.

The access data for the Avalara Tax Service will be entered in the company master data on tab 2. Taxes. Here, it is possible to authenticate either via user/password or via account number/license key.

The tax flag will always be taken over from the customer master data into the order and should be activated for all customers.

Important is also that the workplace has access to the Internet with the port 80 so that the Avalara service is accessible.

If everything is set up accordingly, the tax calculation in the order entry is now done via the Avalara service as soon as the items were recorded. Furthermore, when saving, there is always a recalculation of the taxes as soon as the customer address or the delivery address changes. As soon as the invoice printing is done, there is another tax calculation by the Avalara service. This guarantees that the applicable tax at the time of invoicing is calculated.

**The functions used:**

`bRet = udf_AvalaraTax ( fktDoc, sShipFromStreet, sShipFromCity, sShipFromRegion, sShipFromCountry, sShipFromZip, bSandbox)`

Tax calculation by Avalara Tax Service

**Parameter:**

| Parameter | Description |
| :--- | :--- |
| fktDoc | cfktAuf: document for which the tax should be calculated |
| sShipFromStreet | String: sender's street |
| sShipFromCity | String: sender's city |
| sShipFromRegion | String: sender's region |
| sShipFromCountry | String: sender's country |
| sShipFromZip | String: sender's postal code |
| bSandbox | Boolean: TRUE = use Avalara text access, FALSE = productive environment |

**Returns:**
TRUE = no error

---

`bRet = udf_ShowResults (nMessageType)`

Output of the messages

**Parameter:**

| Parameter | Description |
| :--- | :--- |
| nMessageType | Number: message type that should be displayed. This is a vector that can be connected to the operand (`|`). (e.g. `MESSAGETYPE_ERROR | MESSAGETYPE_INFO`) |

**Returns:**
TRUE = no error

---

`bRet = udf_CalcStandardTax ()`

Calculates the taxes according to the normal standard.

**Parameter:**
None

**Returns:**
TRUE = no error

## 5.13. IG construction prices

Over time, ever more IG prices (end product) are negotiated with the end customer. Due to competition or to gain a market.

Today, the only possibility for managing this in AWB is to create a new IG product and define its final price (primarily as sqm net price)

The number of fixed IG products for price design is growing constantly and thus, the maintenance effort keeps increasing and the search keeps getting more difficult.

In the order entry, it is becoming more complicated to select the right IG product.

The most difficult point is the EDI import; several existing end customer references could refer to this new fixed IG composition, and it involves additional effort to correct all of them according to the new price negotiation.

All of this is simplified greatly with the new IG construction prices feature.

For set-up, the scripts 20210225a.sql, 20210225m.sql, and 20210226a.sql have to be executed.

In IG base product, the "IG construction price" check box has to be checked.

In the management program, a price table has to be assigned for each glass construction. This price table contains the valid price for this construction. Different price codes or individual prices can also be used. Whether the price is also valid for the mirrored construction is determined by the "reversible" check box.

Each change of the price assignment is valid immediately in the order entry; this is true even on different computers.

**Search sequence:**

The access sequence is defined as follows

1.  **Fully qualified**
    This means that all existing components glass, spacer, and gas participate in the search.

2.  **Without spacer**
    The spacer with 0=all is found

3.  **Without gas**
    The gas with 0=all is found

4.  **Without spacer and gas**
    The record with spacer and gas 0=all is found

If no assignment is found after these 4 levels, the default price table from the product data applies. With triple IG, it is not permissible to assign a spacer or gas 0=all. This is already locked in the administration program. The storage can only be done for all spacers and/or all gases with 0=all.

The spacer and the gas are no longer price-relevant if the definition for this product was made explicit in the IG price assignment; for then it is assumed that this price is considered in the price table. If you are working with 0=all, then the element remains price-relevant and there is a search for a surcharge!

## 5.14. Limit quantities for parameterized macros

Parameterized macros are becoming more popular in order to be able to handle complex processings. These can be applied very flexibly thanks to parameterization. The size can thus be adjusted to the customer requirement and the number of processing articles kept small. But these parameters frequently also have effects on the price design; thus, e.g. a small cut-out is cheaper than a large one, or the parameterized drilling diameter defines the scaling of the price.

For this, the limit types "Macro <x> (dimension)" and "Macro <x>" are used for the 1st to 10th parameters of the macro. Here, it has to be noted that according to the type of the parameter, dimension or numeric value (e.g. angle), the appropriate limit quantity has to be selected. For a dimension parameter, the limit type "Macro <x> (dimension)" has to be used; the <x> is a placeholder for the parameter number. The prices can be scaled in the price management according to these new limit quantities.

This is possible for vectors, matrices, and cube prices.

Depending on the macro parameter, the price is drawn from the master data.

The limit quantity has to be set depending on the parameter. The limit quantity has to be assigned using the parameter index (1 - 10).

# 6. Purchase

## 6.1. Transfer to purchasing

### 6.1.1. Executing the P.O. transfer

After acquiring an order, purchase orders can be generated for the included purchase parts. To ensure that this can be performed, the order must be in the valid status range of the status allocation 30 "Transfer into the purchase pool".

### 6.1.2. Repeated P.O. transfer after item changes

If an item was transferred to one or more purchase orders, then it is blocked for changes in the item entry of the order. The function "Change blocked item" can be used to make changes nevertheless. To ensure that this is possible, the purchase order must be in the valid status range of the status allocation 660 and the order in the valid status range of the status allocation 650. If one or two of the above is not the case, then the order item cannot be unblocked and edited.

If the item is saved after a change, then the associated purchase order items will be deleted and the repeated P.O. transfer is triggered when closing the item entry. For this purpose, the purchase order numbers and the purchase order items will be suggested again for the items that were already in a purchase order. If the dialog is closed but the P.O. transfer has not been performed, then a new P.O. transfer must be performed. In this case new purchase orders will be generated.

### 6.1.3. Status points overview

| Status point | Designation | Description |
| :--- | :--- | :--- |
| 30 | Transfer into the purchase pool | This status point is used if orders must be transferred to purchase orders or the purchase pool through the menu item P.O. transfer |
| 650 | Order status changed | This status point is used to check whether the order is in the valid status range for a repeated P.O. transfer |
| 660 | Repeated P.O. transfer | This status point is used to check whether the purchase order is in the valid status range for a repeated P.O. transfer |
| 670 | Purchase order created | Status point order for history entry and status change after transfer to a new purchase order |
| 675 | Inquiry generated | Status point order for history input and status change after transfer to a new purchase inquiry |
| 680 | Purchase order changed | Status point order for history input and status change after transfer to an existing purchase order |
| 685 | Inquiry changed | Status point order for history input and status change after transfer to an existing purchase order inquiry |

The status points 675 and 685 were added using the database script 20160620a.sql. If the script has not been run, then the status points 670 and 680 are also used for purchase order inquiries.

### 6.1.4. Purchase order for Georgian bars

If ordering Georgian bars, then the spacer can either also be ordered or the spacer will be transferred into the purchase order, but it will be processed there as "do not order". This behavior can be controlled with the company option "Order spacer together with the Georgian bars".

*   If the option is set, then the spacer will always be ordered during the P.O. transfer even is it is not entered as a purchase order in the parts list of the order.
*   If the option is not set, then the spacer will be transferred into the purchase order during the P.O. transfer, but it will be covered there with the acquisition type "do not order".

## 6.2. EDI Interface

### 6.2.1. Preparations and settings

Using the EDI interface requires some settings in program “References”. First, we describe the entries necessary to export purchase orders from A+W Business. This is followed by the settings that are necessary to import external orders.

During import, interface files are imported in the A+W Standard format (see the separate interface description) and imported for orders/quotations into A+W Business. For this, the system monitors the folders that are configured on the dialog for the B2B customer management. If in the interface file product numbers are used that are not present in the individual system, then mappings must be created in the article references in order to refer from the external article numbers to your own article numbers.

### 6.2.2. Customers

In the B2B customer management, the customer is configured who sends via EDI interface files. For this, at least the version of the interface file and the paths for the files must be entered. As soon as an interface version has been configured for a customer, the import checks whether an appropriate file is available in the specified source path. The command script is executed during import before reading in of the interface file and during export, the script is executed after creation of the file. Furthermore, the sequential number for the export is entered there and a different partner for the article references if necessary.

Here is an overview of the parameters in particular:

| Parameter | Options & Description |
| :--- | :--- |
| **Compulsory referencing** | ☐ An article reference must be created for all products.<br>☑ First there is a search for reference articles; if no reference is found there, the article number is searched for directly in your own inventory without mapping. |
| **Locking active** | ☑ For the duration of the import, a lock file is created that prevents simultaneous processing<br>☐ No lock file is created |
| **Maximum lock time** | Maximum validity duration of the lock file |
| **Definition of the document number permitted** | ☑ The document number from the interface file is used<br>☐ The document number of the number range is used |
| **Take over BOM completely from the interface file** | ☑ The product's BOM is completely composed from the interface file. Own BOM definitions from the article master data or the article references are thus overridden<br>☐ The BOM is composed from the interface file, the article references, and the article master data. BOMs in the file will be imported as exchanged elements and if necessary, surcharges will be applied. |
| **Dimension system and dimension precision** | Here, a dimension system deviating from your own settings and the dimension precision of the partner are specified. The import converts this to your own dimension system. |
| **Do not generate document in case of error** | ☑ If errors occur during import, the document will not be generated. The document number used at the time of import is saved and reused for the import after error correction<br>☐ The document is generated, any items with errors will not be imported |
| **Restriction exceeded rejects item** | ☑ |
| **Exchange for restriction violation** | ☐ |
| **Allow free complaint** | ☑ |
| **Basic product change with 2x exchange** | ☑ |
| **Delete inferior edge processing on glass** | ☑ |
| **Check processing parameters** | ☑ Check active (see chapter `Bearbeitungsparameterprüfung`)<br>☐ Check inactive<br>(Mandatory starting with version 2.2.028, checkbox is then inactive) |
| **Import of market partner-specific texts** | ☑ |
| **No shape recognition** | ☑ |
| **Expanded DXF import** | ☐ |

### 6.2.3. Selection of external documents

The selection of the individual documents for import is done directly in the table with the normal Windows standards. That is, via mouse-click and if necessary <Shift> or <Ctrl> and mouse-click. Furthermore, the three buttons above the table can be used to select all or no documents. The third button starts a selection dialog on which particular criteria for selection can be entered.

### 6.2.4. Multi-user operation

As soon as another user has selected a document for import, it is marked in the own view with an icon and it can no longer be selected. This prevents a document from being imported in several places and thus duplicated. The name of the employee who is currently editing a document and has selected it is displayed in the table.

### 6.2.5. Checking the reference article

As soon as the user has selected a document for import, the tab "2.Missing references" is activated. As soon as the user confirms the selection with <Enter> or by clicking the "OK" button or by selecting the tab directly, you change to the tab. The program checks whether for the selected documents all articles were created in the B2B article references. If all references are present and created correctly, the tab "3.Create documents" becomes active automatically. If at least one reference is missing, this is displayed in the table. With a double-click, the program changes to the management dialog of the article references, starts its new mode, and pre-populates the known data fields. The user must add and save the missing data. As soon as the dialog is closed and the user changes back to the import dialog, there is another check of the references.

### 6.2.6. Creating the documents

If all reference articles are present and the user changes to the "3.Documents" tab by clicking "OK" or pressing <Enter>, a display of the currently selected number manager appears with the documents it contains. The user can now select the number manager into which the documents should be imported or generate a new number manager by entering a new name. Furthermore, the client and the scheduling area are specified. The import is started by clicking "OK" or pressing the <Enter> key. Insofar as no specification of the document number was defined, the number range of the specified client and scheduling area is used.

After successful import, the imported documents appear in the overview of the number manager.

### 6.2.7. Customizing function for scheduling the files

As already mentioned, the program either schedules the external documents in the buffer tables on start of the import dialog or when pressing the "Import files" button. This functionality can also be executed via a workflow with customizing. The customizing function "udf\_EDIImportToDatabase" exists for this. The call in a workflow task causes a search of their directories for new interface files for all customers with activated EDI import and if necessary these are transferred to the buffer tables. If in the import dialog the automatic update is switched on, the documents stored this way appear automatically in the overview directly after successful scheduling. Error messages can, as for all workflow tasks, be viewed in the Workflow Monitor.

**Example:**

`udf_EDIImportToDatabase ();`

The function has no parameters.

### 6.2.8. DXF shape recognition

Prerequisite for using this new function is Shaping&Nesting from Version 2007. The DXF files have to be entered in the EDI file in field SN Name of the shape record (M1). The DXF files themselves have to be saved in the same directory as the EDI files. After successful import, the DXF files are moved to the backup directory. If shape recognition detects a free shape (shape 99) instead of a standard shape, the system will create a SN file with the converted shape data in the SN path.

### 6.2.9. Progress indicator/options

All events that occur are displayed as progress in the lower half of the dialog in a table. Via the Options menu, the message types (info, warning, and error) of the progress can be selected individually. Also whether the files can be transferred into the buffer tables on start can be set here. If this is deactivated, the transfer can be started with the "Import files" button. Via the checkbox for automatic updating, the table with the documents is updated at the specified second intervals. The lower limit of the interval for this is 5 seconds.

With a double-click on a document, a new dialog is displayed on which all data of the selected document can be edited. With a right-click on a document, a context menu appears via which, in addition to the display of the document, a lock that may no longer be valid can be lifted. For the lifting of this lock, a sub-right of the import dialog is required. If no rights are created, any user can lift the lock.

On the Options menu, you can set whether or not the log is displayed via the import on the dialog. If the progress is hidden, it is displayed automatically on the start of an action. With the "Hide progress" button, it can be hidden again.

### 6.2.10. Import in background

For the automatic processing of EDI files, it is now possible to create a workflow task for the Exchange Service. For this a formula is created in the formula management, which calls the function `udf_EDIImport`. An example of such a formula, including the sending of the processing status, is found in the installation folder under the general formulas (Workflow\_EDIImport.txt).

### 6.2.11. Processing parameter check

For the EDI import (Documents>Order>Import) effective immediately, the processing parameters in the processing record can be checked. The check can be enabled in the third party interface management (Master Data>B2B>Customer>Customer>2.Parameters tab>Check processing parameters) (en). Starting with the interface version Standard Version 2.2.028, the check is enabled by default and can no longer be switched off. For Edge processings, for example, the number of marked edges is checked, that is, if there is no shape, logically a maximum of 4 edges can be processed. If during the check of corner/edge assignments parameters are not set or values are impermissible, these are corrected automatically. Both this correction as well as errors during the check are logged on the progress/report window of the EDI import. For Miters, among other things the angle is checked for a correct value (> 1 and < 89). Insofar as for a Hole drilling a coordinate is not set, it is pointed out that at least one parameter of the processing <Drillings> was not entered. The next message shows in detail which parameter is missing or impermissible.

### 6.2.12. KLAES – XML / Internorm EDI interface version

The interface types (versions) Klaes and Internorm, which correspond with the EDI interface version 2.2.025, can now be defined in external interface management. Both cases deal with editing XML files, but with different structures. For the processing of the files, these must be copied into the EDI source directory. When starting the EDI import, the XML files are converted into the A+W EDI format using a filter program. If conversion is successful, the files have been created in EDI format in the same directory, which can then be automatically read into A+W Business. If errors have occurred in conversion, these are documented in the protocol file defined in external interface management. The source file (XML) is then moved into the backup directory.

Furthermore, the B2B customer (see screenshot) and the product references must be defined in the external interface management.

**Klaes example – Product = Contents from junctions in XML structure**

*   a) Insulating glass (main product) = `<glassproduct>`
*   b) Glasses = `<key>` or `<sys_key>` under `<pane_structure\pane>`
*   c) SZRs = `<key>` or `<sys_key>` under `<pane_structure\szr>`
*   d) Spacer = `<key>` or `<sys_syskey>` under `<edge_seal\spacer>`
*   e) Sash bars = `<sprkey>` or `<XItemId>` under `<glass_sashbar\sashbardata>`

### 6.2.13. Internorm interface

With the help of this interface, XML files are transformed into the A+W EDI format. During processing, logging is done in a file. There is writing to the log file in the following cases:

*   Syntax error in the input parameters
*   Conversion error (XML is not formatted correctly)
*   No customer number was written in the XML file
*   No width or height or quantity or product number
*   DUMMY - item
*   DUMMY - Georgian bars

So that everything works correctly, the following adjustments are required:

#### 6.2.13.1. Adjustment of the VB script Auftraege\_Import.vbs

The script serves to read all XML files out of the import directory. As a result, all paths must be adjusted.

*   Path of the source file ex.: `"\\xxx\xxx\Import\"`
*   Path of the target file ex.: `"\\xxx\xxx\Source\"`
*   Path of the log file ex.: `“\\xxx\xxx\Prot\import_prot“`
*   Path of the exe file ex.: `"C:\xxx\Albwir.Edi.Order.Transform.exe"`

#### 6.2.13.2. New path entries in the partner external interface management

*   Source path ex.: `“\\xxx\xxx\Source\"`
*   Source file ex.: `“*.asc”`
*   Log path ex.: `“\\xxx\xxx\Prot\"`
*   Back-up path ex.: `“\\xxx\xxx\Save\"`
*   Command script ex.: `WSCRIPT.EXE "C:\xxx\Auftraege_Import.VBS"`

#### 6.2.13.3. Adjustment of the EDI import

*   New screen button for opening the log file with the help of customizing
*   New screen button for deleting the log file with the help of customizing

#### 6.2.13.4. Adjustments of the customizing formulas

*   In the formulas, the path of the log file must be adjusted.
*   Formula for opening the log file. It is attached to the first button.
*   Formula for deleting the log file. It is attached to the second button.
*   Expansion of the formula EDI, which is called after the import of an order.
*   Formula for the two buttons.

### 6.2.14. EDI import of payments/complaints

Effective immediately, the EDI import (e.g. Documents>Order>Import) can process the record type A1 for payments on the header level. The following structure was defined for this:

**Table: Header record-down payments**

| No | Designation | Method | Type | Position | Length | Contents |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | Record type | M | A | 1 | 2 | A1 |
| 2 | Payment date | K | D | 3 | 8 | YYYYMMDD |
| 3 | Payment mode | M | A | 11 | 10 | 1) |
| 4 | Payment number | K | N | 21 | 3 | |
| 5 | Payment procedure | K | A | 24 | 10 | |
| 6 | Payment direction | K | N | 34 | 2 | 1=Payment credit note<br>-1=Payment cancelled |
| 7 | Currency | K | A | 36 | 3 | |
| 8 | Amount | K | A | 39 | 12 | |
| 9 | Payment reference - Order | K | A | 51 | 30 | |
| 10 | Exchange rate Currency | K | A | 81 | 12 | Example: 000000000100 if currency = EUR and the document is entered in EUR |
| 11 | Filler | K | A | 93 | 420 | |

1) The field may contain the external key of payment method. If no data record is found for external key, it is assumed that the correct AWB payment method is contained.

The record type is only imported and is not intended for the export of EDI documents. If you import an EDI file and such an A1 record is included in the file, then the data is written to the new intermediate table FS\_DOWNPAYMENT. After that, the imported data is evaluated and processed further if necessary. Now e.g. in case of an order, the payment data record is transferred to the table BW\_AUFTR\_ANZAHLUNG. The user then has the opportunity to view the data in the management program for payments (e.g. Documents>Order>Order>Totals tab>Payment Total button) and change it.

Furthermore, complaints can now be imported via EDI. The document to be imported must be marked in header record K5 field 9 with Document type as Complaint. Here, the user has the choice whether "Complaint" is directly in the field or a so-called mapping value for the foreign key (@REKLA@) or the internal sequential number (#2#) should be used to determine the document type. The same logic applies for the newly-added fields 18 and 19 in the item record P2, Complaint reason and -Location.

Another functionality has been developed for the import of complaints, which checks the fields 2 and 3 of the item record P3 to see whether a reference number (and reference item) is entered there. If there are several P3 item records with different references to a header record K1, the same number of complaints must be generated since the restriction in AWB is as follows: you can only assign one complaint to an original order (assignment of the original via database column AH\_HAUPT\_AUFTR in the complaint).

## 6.3. Export of purchase orders

First of all, enter the customer number you have at your supplier's, on the second tab in field External number.

*(Fig. 135: Export of purchase orders - Screenshot of UI)*

Now, define the export parameters in program „References". This menu is accessed via the buttons "Supplier" / "Supplier".

In field plant number, enter the company number of the target system (supplier). The multi-line field „Batch file for interface" allows to enter batch commands to be executed after the export in order to start an EDI terminal program for instance, or to copy the exported files to another computer. Set the interface version in combo box „EDI type". In the patch fields, enter the source and target path, log path, and backup path for the interface file. Checkbox „Compulsory reference" will make the export program enter an error message in the log book if there is no reference, and ignore the item with the non-existent external product. If this field is switched off, the original product number from product master data will be written in the interface file. This is useful for instance if the sending and receiving systems are using the same product master data. Checkbox „Locking active" in connection with the data field „max. lock time“ switches on a mechanism for a certain time; this shall prevent that two programs can access the same interface file simultaneously.

*(Fig. 136: External interface - supplier - Screenshot of UI)*

Now the article references must be created, insofar as the own article numbers from which those of the supplier differ. Switch to the product reference dialog.

Define a product for the required supplier. Shapes, Georgian bars and processing steps can be allocated in the same way as you do this at order entry. Also, specify the validity for every product. This is necessary for example if a supplier plans to change his product data (partially or completely) at a certain date. These changes can be entered in advance, but will be used for export purposes only after they become valid. The old product definitions will become invalid.

*(Fig. 137: Product reference dialog - Screenshot of UI)*

To start the actual export, switch to the document area, click in the menu on `P.O > Export` and start the export program.

*(Fig. 138: Export program - Screenshot of UI)*

A table appears containing the POs defined for the selected number manager. Click on OK to start the process. The status of the successfully exported purchase orders will be raised to prevent that a purchase order is exported over and over again. Should there be an error during export, you can check this in the system log, and print if required.

## 6.4. PO export via the Dorma Web Service

It is possible to transfer POs for the hardware manufacturer Dorma directly to its Web service. The configuration required for this will be described below. Essentially, this works so that on the A+W Business dialog for the EDI export, a table is filled with the Dorma POs. The table is read in at intervals of 5 minutes by AWSOA Commercial 6 Exchange Service and all POs found there are transferred to the Dorma Web Service. No workflow is required for this, the export is executed in the same thread of the openTRANS export. In the company master data, on the tab "10.System", the check box "Activate Exchange Service for workflows" must be switched on. Directly below it, the thread is entered in which the openTRANS export and also the Dorma export should be executed. If there is a zero there, the export is deactivated.

Then comes the definition for the access to the Dorma Web service. This is also taken care of in the company master data on the tab "7.Stock/PU/EDI".

Now it must be specified which number the supplier "Dorma" should have in the respective installation. For this, in the program "Master data > B2B > Supplier > Supplier" the interface type "Dorma" is assigned for the supplier.

Now it is necessary to create the product references for the Dorma article. This can either be done manually in the program "Master data > B2B > Supplier > Products" or by import of the Dorma article (see Chapter 1.8 Article import).

Error messages for the transmission to the Dorma WebService can be viewed on the Customizing Monitor under the "openTrans" workflow.

## 6.5. Additional functions

### 6.5.1. Copy external products:

*(Fig. 139: Copy external products - Screenshot of UI)*

This dialog serves to copy external product definitions from one customer/supplier to another. This dialog is accessed via the product reference program, entry „Functions/Copy product“.

### 6.5.2. Edge reduction for Georgian bars in customer data as from Version 3.3

So far, the parameter GEORGIAN BAR EDGE REDUCTION was only managed in customer master data, and did not influence order entry.

From version 3.3, the edge reduction for Georgian bars is analysed in connection with the calculation of cutbacks, and has priority over a purchase price calculation pattern.

When you update to 3.3 please check whether field Georgian bar edge reduction (tab Production) in customer master data contains information that might cause errors when you calculate the cutback.

## 6.6. Electronic document exchange

### 6.6.1. Order confirmation and invoice

**General**

As from Version ALFAK2008, order confirmations and invoices can be exported and imported again. The format used is the document exchange format openTRANS which has been adapted to ALFAK. It is also possible to import documents without this amendment, i.e. in standard format.

**Document export**

The export is configured individually for every customer. You can therefore defined whether and which documents shall be exported for the customer in question. External interface management offers a new menu for this purpose, Document export. This dialog also serves to define the export mode. There are two versions at present:

*   Automatic email dispatch
*   Saved in a defined directory (on the server)

Prerequisite for using the automatic email dispatch is that an email server is available in the network. The email address defined in customer master data is used as the standard address for sending documents to the customer. If an alternative address shall be used, it can be entered in dialog Document export.

Prerequisite for exporting documents successfully is that up-to-date archives exist and that a purchase reference has been entered [DokNo u. ItmNo] for the order item, tab „More details" and the Interface Service has to run with enabled B 2 B handle function!

When order confirmations and invoices are printed, the program will automatically check whether there are documents for which document export is active. If so, there will be a query as to whether document export shall be started. If this is confirmed, the corresponding documents will be marked for export. For every order there is an entry in order history, showing the corresponding status point (830 for invoice export or 840 for order confirmation export). If these status points have been allocated, the order will be set to the allocated status. The minimum or lock status is not checked because export is always directly linked with the print job.

A service is installed on the server (in new versions, AIS) which searches in regular intervals for documents marked for export. After that, the service runs the actual export automatically in the background. All exported documents will be saved in archives. To check this, the print program offers the tab Document export which shows the status of all documents currently marked for the export.

Please note: Roto invoice export has been integrated in the new process. Processing will be started together with the printout, not upon transfer to financial accounting as before.

Export will create special files:

*   RESPONSExxxx.awotres files are openTRANS-based order confirmations with Albat+Wirsam-specific amendments
*   INVOICExxxx.awotinv - files are openTRANS-based invoices, also with Albat+Wirsam-specific amendments

**Document import**

If a supplier sends in one of the two above-mentioned files, these can be imported by double-clicking on them. This even works from an email client. The above-mentioned file suffixes were linked with the program Albat+Wirsam openTRANS ImportTool for this purpose.
If the files are saved on the hard disk, a generic view of the document is available by means of a right click and the option View.

The import tool only supports openTRANS files 1.0, Version 2.1 is not supported.

Apart from the links to the above file suffixes, files with the suffix .xml can be imported as well. These files cannot be started directly from the email client however. A right click on the file and use of the options `Import as openTRANS document` or `Show as openTRANS document` will start the corresponding action.

After the document has been imported successfully, it is available in dialog `Electr. price check` or `Electr. invoice check` which have been added in section Purchasing, Order confirmation and Invoice. The dialogs are only slightly different, which is why this description applies to both.

**Electronical price check and Electronical invoice check**

**General**

The locking behavior in connection with the price and invoice check has been changed by another patch for ALFAK 2007. When a purchase order is accessed during an invoice check, it will be locked now. This means that a purchase order cannot be opened for a price or invoice check and P.O. entry at the same time. The new function 'Open P.O. entry' can be used to amend the P.O. during a price or invoice check. This function opens a limited P.O. entry, only for the purchase orders which are currently being checked with regard to prices or invoices.

**List of documents and filter settings**

When you access the dialog, the document view at the top shows all imported documents of the type in question. Various filter settings can be made for the view:
The combo box below the table defines whether only open (i.e. still unprocessed) documents, only rejected documents, or all documents shall be shown.

The button next to it offers additional filter options. These settings will be saved by user. In the top section you can search for the user who has entered the P.O. that belongs to the document:

*   *All* means that there are no restrictions
*   *Only one's own* means that only documents entered by the current user will be shown
*   *Defined* means that only documents will be displayed the purchase orders for which were entered by the defined user

The items "Only one's own" and "Defined by" can combined. This could be used for holiday replacements for example when a user will have to handle not only his own documents but also those entered by his colleague who is on holiday.

In the bottom section you can search for suppliers. The document view shows only documents from suppliers defined in the filter settings.

**P.O. list and document status**

When a document is selected from the document list, all related purchase orders will be loaded and linked with the document. The result of this link is shown in the sections 'P.O. list' and 'Document status'.

The P.O. list shows all related purchase orders. If there is one or more partial shipment(s) for a purchase order, this/these will be shown in blue letters. An icon in front of each P.O. defines whether the link between P.O. and document is complete. If this is not the case, column 'Notes' will tell you why this is so.

The 'Document status' view shows whether the document could be completely linked with all the related purchase orders. Like the document status, the individual criteria will be shown in color. The criteria are:

*   **Purchase orders completely referenced**
    Tells you whether the document refers to all purchase orders. This cannot be the case e.g. if the present document refers to a partial shipment. If the purchase orders are not fully referenced but the document is otherwise complete, a partial shipment can be issued automatically (see booking modes)

*   **Article items missing from purchase orders**
    Tells you whether the order confirmation or the invoice shows more items than listed in the P.O.

*   **Overall surcharges/discounts missing from purchase orders**
    Overall surcharges/discounts will not be ordered as a rule but still appear on the order confirmation and on the invoice. These items have to exist in the purchase orders in order to run an invoice check.

*   **Price difference**
    The purchase orders and the present document show different prices. The fields next to this show the difference as an amount and as a percentage.

*   **Difference in quantity**
    The purchase orders and the present document show different quantities.

*   **Document view**
    This button serves to display the newly imported document in generic form.

**Booking modes**

The document status tells you which booking modes are valid for the newly imported document. If the document status is green, the document can be booked. Above the document view, the program automatically changes the booking mode to 'accept'. The booking modes are:

*   **Reject:** The document will be rejected. There will be no price check or invoice check; the document gets the status 'rejected'. All related purchase orders will be set to the status allocated to status point 61 (for order confirmations) or status point 64 (for invoices).
*   **Accept:** The document will be accepted. The prices shown in the document will be applied to the purchase orders. The order confirmation number of invoices number plus all other document data will be saved. The status of the purchase orders is also set to 'Order confirmation check' or 'Invoice check'.
*   **Issue partial shipment:** A partial shipment will be issued. The imported document does not include all items of the related purchase order. Based on the document items, a new partial shipment will be issued which will be booked as described for 'Accepted'. The remaining items are kept in the original purchase order. The status of this P.O. will not be amended.

**Item overview**

You can switch to the item list to see which items cannot be allocated. This is where all items of this document are listed. If a purchased item could be found relating to an item of the document, it will be displayed in the same line.

The P.O. items that could not be allocated to a document so far are shown at the end of the table.

Like in the P.O. list, icons in front of each line mark the status of the individual items.

Overall surcharges/discounts are special. It may happen that the supplier sends just one invoice for two purchase orders, and that an overall surcharge appears just once in the invoice. Still, the overall surcharge applies to both purchase orders in this case. To handle this, all related P.O. items will be shown in the lines in front of the document item. The blue downward arrow shows that these P.O. items belong to the document item.

A detailed view for all lines of the item list is available at the bottom of the dialog. It shows details on the document items and on the P.O. items. If a P.O. item has been allocated to a document item, the details can be directly compared in this area.

**openTRANS functions and options**

The menu offers a new main item, `openTRANS`. It includes various functions and options for the processing of openTRANS documents. Separated by a line, the functions appear in the top section and the options at the bottom.

**The functions are:**

*   **Manual allocation of items**
    If the P.O. references are incorrect or missing from an openTRANS document, the system cannot automatically link document and P.O. items. Linking can be done by hand in this case.
    Selecting this function will open a new dialog consisting of two tables. The table on the left lists all document items that could not be allocated while the table on the right shows all P.O. items still to be allocated. Allocation is made by selecting one document item and one P.O. item each, and pressing OK. The now allocated items will be removed from the corresponding tables.

*   **Special case: overall surcharges/discounts:**
    As already explained in connection with the item list, it may happen that an overall surcharge shown in an invoice has to be allocated to several purchase orders. This is done by keeping the CTRL key pressed while selecting the P.O. items from the table.

*   **Another speciality of the overall surcharges/discounts** is the option of using the product number to define the future, automatic allocation to a certain supplier. The supplier's product number is saved along with one's own product number for this purpose. The two checkboxes at the bottom of the dialog can be used for this purpose. If both checkboxes are active, the overall surcharges in future documents from this supplier will be automatically linked with the currently selected product number.

*   **Another special case: ALFAK - collective invoices:**
    If collective invoices are issued by ALFAK, the overall surcharges/discounts will be listed as separate items for every order. Since the direct, manual allocation is not always easy, several document items can be combined and allocated to the P.O. items in this case. Subsequently, only the collected document item will be listed in the item overview. This method is always used for the automatic allocation of overall surcharges/discounts.

*   **Distribute footer surcharges/discounts to P.O.s.**
