---
description: "AWBusiness Surcharges Discounts Doc EN"
---



title: "EN_AWBusiness_Master_Data_9_4-2"
source: "EN_AWBusiness_Master_Data_9_4-2.pdf"
tags: ["surcharges", "discounts", "pricing", "A+W Business Master Data", "product management", "customer management", "price calculation", "software tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical guide from the A+W Business Master Data tutorial series, focusing on the configuration and application of surcharges and discounts within the system. It covers automatic and manual surcharges, product and partner master data settings, and various discount types and hierarchies."
long_description: "This document is a comprehensive tutorial on managing surcharges and discounts in the A+W Business software. The \"Surcharges\" section details how to define, allocate, and apply automatic surcharges for products and partners. It includes step-by-step instructions for setting up customer-specific surcharges, with examples for edge stripping, energy costs, and special discounts. A complex exercise walks the user through creating multi-dimensional price tables (cubes) and miscellaneous surcharges for specific conditions like edge overlength. The \"Discounts\" section explains the function and hierarchy of discounts, covering standard, graduated, and exchange discounts. It details how discounts are applied based on customer, product, product group, and price lists, and how they interact with surcharges. The document provides visual guides through software screenshots and explains the logic behind rate diversions and the discount search hierarchy, ensuring users can accurately customize pricing for specific customers or scenarios."
---

## Surcharges

*Fig. B-199 Automatic Surcharges*
*   **A**: Product master data
*   **B**: Partner master data

The selection of surcharges/special discounts in partner product management (A) is limited. In partner management (B), all general discounts/surcharges are available. Customised discounts/surcharges will be shown for the customers in question.

## Product Surcharge Allocation

Automatic surcharges are entered in dialog *Product surcharge allocation*.

*Fig. B-200 Product surcharge allocation*
*   **A**: Name of the surcharge
*   **B**: Number and name of the allocated product
*   **C**: Position in which the surcharge is added in the document

This example shows a couple generally applicable automatic surcharges. Each of these surcharges is based on a separate product (B), e.g. the product *Inside pattern* or *Edge stripping*.

The date 31.12.2099 indicates that this surcharge is valid indefinitely. Surcharges valid for a certain time only have an end date which appears in column *Valid until*. After the defined date, they will no longer be added or offered for selection.

By entering the item number (C) you can define the point at which the surcharge/discount shall appear in the document. Among other things, this item number determines the surcharge/discount calculation. 0 means that this surcharge shall be applied to an order item. The surcharge therefore has to be enabled in product management.

> **Example**
> If a surcharge/discount is entered with an item number of 900, it will appear at the end of the document. A surcharge/discount with item number 901 will be added as the next item.
>
> If an energy surcharge is to be applied in general, it is enabled in product definition. As a surcharge, its item number is over 900, e. g. 970; it will be added as the last order item when the order is saved.

Through its position in the document and based on the *Surcharge type* chosen in product definition, a surcharge/discount can be applied to another surcharge/discount. This means that a special discount can be applied to the entire order, including the automatic toll surcharge.

*⇨ "Surcharge Types" on page B-309*

## Available Surcharges/Special Discounts

The following discounts/surcharges have been defined and can be edited:

*Tab. B-15 List of automatic surcharges (Section 1 of 2)*
| Surcharge/discount | Description |
| :--- | :--- |
| **Delivery fee** | This surcharge is calculated for delivery. It can be enabled in partner management. |
| **Down payment** | The down payment is entered as a down payment invoice, and is deducted from the order total. For further information, please refer to section Sales. <br> *⇨ Sales, "Down Payments" on page C-273* |
| **Rush surcharge** | This surcharge will be applied if an order must be delivered sooner than is usual. It can be enabled in partner management. |
| **Energy surcharge** | The energy surcharge refers to the weight of the shipment. It can be enabled in product and partner management. In company data, it can be restricted to the glass weight. <br> *⇨ Software Reference, "Company Data > Price Calculation" on page B-944* |
| **Rack 1, Rack 2** | Rack surcharges are applied in connection with rack management. It can be enabled in product and partner management. <br> *⇨ Software Reference, "Company Data – Shipment" on page B-990* |

*Tab. B-15 List of automatic surcharges (Section 2 of 2)*
| Surcharge/discount | Description |
| :--- | :--- |
| **Max. surface, Max. aspect ratio** | These surcharges are applied if the maximum surface and/or maximum aspect ratio is exceeded. They can be enabled in partner management. The values are checked against the sizes entered in product management. <br> *⇨ Software Reference, "Price Parameters" on page B-602* |
| **Shortfall** | This surcharge refers to the minimum quantity defined in product management. It can be enabled in partner management. <br> *⇨ Software Reference, "Price Parameters" on page B-602* |
| **Edge stripping** | This surcharge is automatically applied for edge stripping of coated lites. It always refers to an item. It can be enabled in partner management. |
| **Invoicing** | This surcharge is applied when the invoice is issued. It can be enabled in partner management. |
| **IG recycling** | This surcharge applied for the disposal of IG. It can be enabled in partner management. |
| **Special discount 1 - 10** | Special discounts can be defined individually. With a positive sign, they are applied as a surcharge and with a negative sign, as a discount. They can be enabled in product and partner management. |
| **Pattern inside** | This surcharge will be calculated for the fitting of a patterned lite with the patterned side facing inwards if, usually, this side is facing outwards. It can be enabled in partner management. |
| **IG transport** | This surcharge is calculated for the transport insurance of IG units. It can be enabled in partner management. |

All other surcharges which are not automatically applied based on product and partner master data, have to be entered by hand in the document.

### Defining an automatic surcharge

An automatic surcharge is defined in the following sequence:

*   Enter a product in product management (surcharge product):
    *   Go to tab *Product* and choose the entry *Services/surcharges* as *Product type* and *Product group*.
    *   On tab *Production*, enter the quantity unit and whether the discount/surcharge shall be printed on the BOM.
    *   On tab *Price/surcharge*, enter the corresponding Surcharge type, e.g. *Basic item*.
    These steps are described in detail in chapter Product.
    *⇨ "Product Definition" on page B-182*
*   Enter a unit price for this product in price management.
    A negative entry for the automatic surcharge will result in a reduction of the price. It is applied as a discount.
    *⇨ "Input of Unit Prices" on page B-236*
*   In dialog *Product surcharge allocation* allocate the product to the corresponding automatic surcharge.
*   In customer master data, go to tab *Order*, section *Apply surcharges/discounts* and tick the checkbox for surcharges which shall always be applied to this customer.
    *⇨ Software Reference, "Surcharges/discounts" on page B-767*
*   In product master data, go to tab *Price/surcharges*, section *Apply surcharges/discounts* and tick the checkbox for the surcharges which shall always be applied to this product.
    *⇨ Software Reference, "Apply Surcharges/Discounts" on page B-601*

The following guideline shows how to enter a special discounts for a customer. The product *Special discount training* and the corresponding price table have been created for this purpose.

### How to define an automatic surcharge for a customer

1.  Go to menu *Master data > Company > Product surcharge allocation*.
    Dialog *Product surcharge allocation* appears.
2.  Go to the menu *Start > New* to switch to the input mode.

*Fig. B-201 Fields for automatic surcharge are accessible*
*   **A**: Customer
*   **B**: Choose the surcharge
*   **C**: Product for the surcharge
*   **D**: Item

The fields are preset with the data of the surcharge selected from the list.
3.  Choose the option *Customer* (A) and the customer for which this surcharge/discount shall be entered.
4.  Select the automatic surcharge/discount (B) you want to define, e. g. the entry *Special discount 3*.
5.  Select the product (C) to be allocated to the surcharge, e. g. the product *Special discount training*.
    Product *Special discount training* has already been assigned a price (proportional surcharge).
6.  Choose a long period of time in field *Valid to*, e. g. 2099 if the surcharge/discount shall be applied always.
    In this example, the validity is limited to the 31.12. of the current year.
7.  Enter the Item in the document (D):
    *   **0** for an item-related surcharge/discount, e. g. for a surcharge for exceeding the maximum surface. It will be calculated for every item to which it applies.
    *   **900 - 999** for surcharges/discounts which shall be applied to all previous items or parts of the previous items.

*Fig. B-202 Customised special discount*

In this example, the item number 999 is entered. This means that the special discount will be applied at the end of the order items, and will be calculated for the total.

8.  Select in the menu *Start > Save* to save the data.
    The data will be saved.

To make sure that the surcharge/discount is applied, enable it in the customer's master data. If there is an additional, general special discount, only the customised special discount will be calculated for this customer.

### Exercises

*   Enter a special discount of 3 % for your customer, to be automatically added as the last order item.

Please obey the sequence in which product, price, and allocation have to be defined.

In one of the following exercises you will check whether the special discount is applied as intended.

**Additional information**
*   ⇨ "Editing the Customer's Financial Data" on page B-100
*   ⇨ "Product Definition" on page B-182
*   ⇨ "Input of Unit Prices" on page B-236
*   ⇨ Software Reference, "Product Management" on page B-590
*   ⇨ Software Reference, "Price Management" on page B-710
*   ⇨ Software Reference, "Partner Management" on page B-757
*   ⇨ Software Reference, "Surcharge Product Assignment" on page B-1024

## Complex Exercise

By means of an example, input of prices for a product is explained in detail in this exercise.

### Tasks

Let us start with an example of prices for a product used in standard price lists:

*Tab. B-16 Product prices*

| Prices/sqm x mm laminated lite | 4 mm | 5 mm | 5 mm | 6 mm | 6 mm |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Surface sqm** | **up to max. 1410 x 2400 mm** | **up to 1600 x 3000 mm** | **> 1600 x 3000 to 2450 x 3000 mm** | **up to 1600 x 3000 mm** | **> 1600 x 3000 to 2550 x 4500 mm** |
| **A1** | | | | | |
| > 0.50 qm | 196.00 € | 202.00 € | 276.00 € | 208.00 € | 282.00 € |
| 0.16 - 0.50 qm | 253.00 € | 263.00 € | - | 271.00 € | - |
| 0.10 - 0.15 qm | 311.00 € | 323.00 € | - | 333.00 € | - |
| **A2** | | | | | |
| > 0.50 qm | 215.00 € | 224.00 € | 299.00 € | 230.00 € | 305.00 € |
| 0.16 - 0.50 qm | 281.00 € | 291.00 € | - | 299.00 € | - |
| 0.10 - 0.15 qm | 345.00 € | 358.00 € | - | 368.00 € | - |

The following calculation factors can also be applied for example:

*   If the edge is longer than 3750 mm a surcharge of 30% shall be added
*   The minimum production size is 200 x 300 mm
*   The minimum calculation length per edge is 300 mm

For the examples from the table first define the number of limit types (sizes) to be considered:

*   The surface limit (0.10 – 0.15 sqm; 0.16 – 0.50 sqm; over 0.50 sqm).
*   The width:
    For LG 5 mm there are two size limits (0<B1<1600 mm and 1600<B2<2450 mm) and for LG 6 mm one (2550<B2<4500 mm).
*   Height:
    For LG 6 mm there are two size limits, below and over 3000 mm.

This makes it a total of four limit types. The cube can take into account maximally three of them. The fourth size can be handled by a surcharge.

For every IG unit A1 and A2 and laminated lite thickness, six IG products are entered.
*   A1:
    *   IG A1 with LG 4 mm
    *   IG A1 with LG 5 mm
    *   IG A1 with LG 6 mm
*   A2:
    *   IG A2 with LG 4 mm
    *   IG A2 with LG 5 mm
    *   IG A2 with LG 6 mm

Now create a price table for each of the six IG products (= three price tables for every IG unit):
*   For IG products with a 4 mm LG lite, vector price tables with one limit type: the surface.
*   For IG products with LG 5 and 6 mm, cubic price tables with three limit types: surface, width, and height.

The fourth size is included as a surcharge for edge overlength from 3750 mm.

### Solution: Enter the Product and its Price

The example product is an IG unit. We are going to explain in detail how to proceed. At the same time, we are going to describe the cube (three-dimensional pricing). This will give you a good idea of how pricing works.

There are the following instructions on this subject.

*   "How to enter the price as a cube" on page B-334
*   "How to enter the miscellaneous surcharge" on page B-338
*   "How to enter the IG product" on page B-339

#### Price tables with three limits

First check which price list and price key (rate) is used by default to determine the sales price for the IG unit.

#### How to enter the price as a cube

1.  Go to menu *Master data > Products > Prices > Price list*.
    Dialog *Price list* appears.
    The checkboxes show the price lists active for standard calculation of the IG sales price.

    *Fig. B-203 Price list*

    The column *Stn. IG SP* is important in this example. The price list used for IG sales is *EURO Price 07* in this case.
2.  Close the dialog and go to menu *Master data > Prices > Rates*.

    *Fig. B-204 Rate: Year + key*

    As you see, several price keys can be allocated to the same price list. There are therefore various price list/key combinations that can be used for IG pricing. In this case, *EURO Price 07* and *Works VEGLA 97*. This shows where the new price list has to be saved to make sure that the price will be used automatically.
3.  Go to *Master data > Products > Articles > Articles*.
    Go to dialog *Product management* and check in which number area your IG products have been entered. Since price table and product should have the same number you should make a note of the free number.
4.  Select menu *Master data > Prices > Prices*.
    Dialog *Prices* appears.
5.  Go to the menu *Start > New* to switch to the input mode.

    *Fig. B-205 Enter price*

6.  Enter the number of the price table and select the price list and the price key.
7.  Go to tab *Cube*.
    The solution for this exercise is:
    *   Width => Limit type 1:
        *   For LG 5 mm, 2 size limits 0<W1<1600 mm and 1600<W2<2450 mm, and
        *   For LG 6 mm, 2550<W2<4500 mm
    *   Height => limit type 2
        *   For LG 6 mm split into two surfaces, below and above 3000 mm)
    *   Surface limit = limit type 3
        *   (0.10-0,15 sqm; 0.16 – 0.50 sqm; over 0.50 sqm)

    *Fig. B-206 Enter price*

    For the third dimension of the cube, set up a tab for every size limit of *Limit type 3*. To view the prices for 0.15 – 0.50 sqm please switch to the corresponding tab. Tab 0.15 includes prices from 0 – 0.15 sqm. Tab 9999.99 applies to a surface between 0.50 and 9999.99 sqm (these figures are inclusive values).
8.  Enter the prices in all tabs.
    An additional calculation factor is the minimum calculation size of 300 x 300 mm. You will find that for the width and height, 300 mm has been defined as the lowest limit although the minimum production size is 200 x 300 mm. Pricing will only consider the limit sizes for calculation but not the production limits.
9.  Select in the menu *Start > Save* to save the data.

### Miscellaneous surcharge

A surcharge of 30% shall be applied if an edge is longer than 3750 mm.

#### How to enter the miscellaneous surcharge

1.  Go to menu *Master data > Products > Prices > Misc. surcharges*

    *Fig. B-207 Other surcharge*

    Edge surcharges are entered in *Misc. surcharges*. In this example, the edge surcharge is found in in surcharge table 10.
    The first line defines that from 0 to 2400 mm, a surcharge of 0% shall be applied, i.e. no surcharge at all. Acc. to the second line, a 35.00% surcharge will be applied from 2400,01 to 3000 mm and 45.00% from 3000,01 mm upwards.
    This includes all special rules.
    Table number 10 for *Misc. surcharges* can be entered at two points:
    *   **Product:**
        If the table number is entered in the product in tab *Price/surcharge*, the edge surcharge will be applied always, even if another price table is used, e.g. for purchase orders.
    *   **Price table:**
        If the edge surcharge shall not be applied generally, enter the table number only in the corresponding price table. This makes sense for example if you want to create a special quote or if this surcharge shall not be valid for a certain customer.
2.  Select in the menu *Start > Save* to save the data.

### Defining a product

When all price-relevant data of an IG unit have been defined, the IG unit can be entered as a product.

This example shows the IG product 151000 which already exists. You will be able to see what you have to do to enter a similar product.

#### How to enter the IG product

1.  Go to menu *Master data > Products > Articles > Articles*.
    Dialog *Product management* appears.
2.  Go to the menu *Start > New* to switch to the input mode.

    *Fig. B-208 Product management IG*

3.  Enter the product number and a name.
4.  Go to tab *Price/surcharge* and enter - among other things - the numbers of the price tables and - in field *Misc. surcharge* - the table for the edge length surcharge.
5.  Enter the control code for the product.
6.  Go to tab *BOM* to enter the structure of the IG unit.

    *Fig. B-209 Product management IG BOM*

7.  Select the element after which a new element shall be added.
8.  Open the context menu and select the corresponding entry:
    *   **Enter element (before/after):**
        This serves to add an element on the same level, e.g. float to the main product.
    *   **Add element:**
        This serves to add an element on a lower level, e.g. a spacer to the glass.
    You can enter more elements in the same way.
9.  Select in the menu *Start > Save* to save the data.
    The data will be saved. The product has been entered. Other program parts can access this now and display and calculate the corresponding price, e.g. at order entry.

## Discounts

Discounts are another means of amending the price for every single customer without having to change the price lists.

This subject area will introduce the discounts and their functions.

## Hierarchy of Discounts

### Objectives

*   Introducing the discount functions.
*   Graduation of discounts.
*   Defining a customer discount.

### Benefit

*   Discounts reduce the list price of products when items are calculated in a document and are therefore an important tool for pricing.
*   As discounts can be allocated quite specifically, pricing can be customised to a very high degree.

> **Note**
>
> **Discount management**
> Discounts can be defined for customer or supplier groups or for single customers or suppliers. The discount management logic is the same for customers and suppliers.
>
> **Discount value**
> Discounts can be graduated by means of a limit type. The defined value will always be interpreted as a percentage.
>
> **Discounts in the rate system**
> Discounts always refer to a price list, a price key, and a product or product group.
>
> **Discount code**
> Discounts will be applied only if the code has been set in product master data.
>
> **Manual discount**
> Discounts can be entered manually in the order. Manual discounts will overrule the discounts defined for the customer.
>
> **Hierarchy of discounts**
> Price calculation in the document first checks the item settings. The program will stop searching for a discount if valid agreements are found in the item or in partner discounts.

## The Function of Discounts

Discounts reduce the list price of products when items are calculated in a document. Discounts are defined for single customers or customer groups and refer to a product or a product group.

This discount is automatically applied to the order when the product is entered. If no discount has been defined you can enter a percentage in the order. This manual discount can either be entered in the order header for the whole order, or at item entry for an item or a BOM element.

You can enter different discounts:

*   Standard discounts for a price list and a price key (rate)
*   Graduated discounts with a quantity limit
*   Exchange discounts

*Fig. B-210 Discounts for customer and customer group*

This example shows the discounts for a customer. The colors of the entries have the following meanings:

*   **Blue**: Product groups
*   **Red**: Product
*   **Green**: Product group and project

Since discounts are applied only if the product or BOM element is marked 'discountable', they can be specifically allocated to individual BOM elements or to complete products.

*Fig. B-211 Product management – Price/surcharge*

*Fig. B-212 Discount allocation options*

These examples show an IG product consisting of a float glass lite, the spacer, and a toughened glass lite. Discounts can be applied to all of those products. Whether the discount is applied in the order depends on the discount agreements made with the corresponding customer.

*   Customer A gets discounts on float glass and on toughened glass.
*   Customer B gets a discount on IG.
*   Customer C gets discounts on IG, float glass, and the spacer.

You can also see that the discounts are adding up, i. e. that a discount is granted for the IG unit as well as for the BOM elements.

In this example, discounts are granted for whole product groups (PGR). Discount agreements can of course also refer to individual products.

> **i Special discount**
> Automatic surcharges can also be used for defining general (generally applicable) discounts, e. g. for special promotions. These special discounts are never shown on the list of discounts.
> Special discounts must not be mixed up with the partner discounts described in this chapter.

## Discount Search

The following hierarchy applies to all calculations in orders:

*   Entries made in the order (top priority)
*   Agreements made in partner discounts

In this sequence, the next step will be performed only if the search produces no results. The following discount hierarchy is used for pricing:

*Fig. B-213 Pricing hierarchy*
> Product - 1004 customer
>> Product - 1004 customer group
>>> PGR-110 customer
>>>> PGR-110 customer group
>>>>> PSG-11* customer
>>>>>> PSG-11* customer group
>>>>>>> MPG-1** customer
>>>>>>>> MPG-1** customer group

Pricing in the document is also controlled by the settings made in company data system-wide. The individual settings are described in the Software Reference.

*⇨ Software Reference, "Company Data > Price Calculation" on page B-944*

## Definition of Discounts

### Objectives

*   Introducing standard-, exchange-, and graduated discounts.
*   Definition of discounts.
*   Defining a discount diversion.

### Benefit

*   Discounts are means of pricing which can be used to adjust the price of an order specifically for a customer or a customer group.
*   Based on supplier discounts, purchase prices can be calculated so accurately that the margins, e. g. for favourable offers, can be met.

> **Note**
>
> **Customer Discount**
> Customer discounts are analysed at the pricing of orders.
>
> **Supplier Discount**
> Supplier discounts are analysed when determining the purchase price.
>
> **Standard discount**
> Several discounts can be defined for a product group or a product, referring to different price lists and price keys each. One of the discounts has to be allocated as the default (standard) discount.
>
> **Exchange discount**
> Exchange discounts are granted for elements which are used in a BOM instead of the original element.
>
> **Grad. discount**
> Discounts can be graduated by means of a limit type.
>
> **Discount diversion**
> In discount management, diversions to other rates, rounding, minimum quantities, and surcharges can be set. This way, the standard settings can be overruled for every customer.

> **i Customer and supplier discounts**
> Customer and supplier discounts are entered in the same way and used for the calculation of documents. This chapter will just mention customer discounts to make the explanations easier to understand.

## Discount Management Dialog

Dialog *Discount management* can either be opened for customers or for suppliers. The different is limited to the selection of the partner or of the partner group. Otherwise, the tabs and fields are the same.

*Fig. B-214 Discount management - example: customer discounts*
*   **A** Tab with details
*   **B** Discount for partner or group
*   **C** Discount for product or PGR
*   **D** Discount rate and validity
*   **E** Code for default discount
*   **F** Discount rate
*   **G** Price list
*   **H** Price key
*   **I** Validity

Discounts always refer to a price list (G), a price key (H), and a product or product group (C).

### Time limit

You can define a time limit (D) for discounts if you enter several discount rates for a customer and a product or a product group. The discounts will only applied within the defined period in this case. This can be used e. g. to prepare special promotions.

### Standard discount

You can enter different discount rates for the same product group by referring to two different price lists and price keys (rates). Just one discount rate can be marked as the default (E) rate however. This will be automatically suggested in the order and can be changed if required.

### Project-related discounts

A discount can be restricted to a certain project. In this case, it will be used for pricing only if the order refers to this project. Since a validity can be defined for the project itself, project-related discounts do not have to have a time limit.

### Graduated discounts

Graduated discounts can refer to all limit types valid for the price lists and for surcharges. The discount can only be graduated by means of one limit type however.

### Exchange discounts

For exchange discounts, the discount granted for the lite to replace the original lite can differ from the discount granted for the IG unit. The exchange discount can be granted in addition to the discount for the IG unit if the settings in product master data are made accordingly.

> **Example**
>
> A 5% discount is granted on the surcharge for the exchanged glass.
> 10% discount will be granted for IG.
>
> Adopt from main item: 10% discount for IG will be granted.
> No adoption: 5% discount from the exchange discount will be granted.

The settings for adopting prices are described in detail in the Software Reference.

*⇨ Software Reference, "Adopt main item" on page B-602*

If a surcharge is applied when a lite of an IG unit is exchanged, the resulting exchange price may be reduced by the exchange discount.

> **Example**
>
> | Product | Price | Discount | Total |
> | :--- | :--- | :---: | :--- |
> | IG unit 2x4 mm float, 1sqm, 1000x1000 mm | 60.00 € | 50% | 30.00 € |
> | Replaced by TG | 75.00 € | 30% | 52.50 € |
> | **Total** | | | **82.50 €** |
> | Replaced by a toughened lite with a customised net price * | 75.00 € | 0% | 75.00 € |
> | **Total** | | | **105.00 €** |
>
> * In this example, a customised price is calculated for the lite to be changed in which is why the discount is omitted.

If company data only permit an individual price, A+W Business first checks if an individual price has been entered. After that, the defined discount will be applied. The combination of rates defined for the individual price overrules the combination defined in Discounts.

## Other agreements

By means of partner-related discounts you can enter different agreements, e. g. different minimum quantities, rounding, rates (rate diversion).

### Rate diversions

Diversions can refer to other rates if for the customer in question, other surcharges that those in the standard price lists shall be valid.

*Fig. B-215 Diversion of rates*

*   **Price group-related surcharges:**
    If no price group-related surcharge is defined, the price list and the key (rate) of the main item will be automatically used for surcharge calculation. These surcharges can also be loaded from another price list and/or key. The system will check in this case whether appropriate price groups have bee defined for the price list, the price key, and the product.
    If so, the program will search for entries in group surcharges. If there are no entries, a message will be issued at order entry saying that no surcharges were found.
*   **Price group-independent surcharges (exchange surcharges):**
    Exchange surcharges follow the same principle as price group-independent surcharges. The setting has to be edited only if the price list and/or key for the surcharge differs from that for the main item.
*   **Miscellaneous surcharges:**
    If another surcharge shall be used for this customer or customer group, an appropriate diversion can be defined, e. g. miscellaneous surcharges for overlong edges.

