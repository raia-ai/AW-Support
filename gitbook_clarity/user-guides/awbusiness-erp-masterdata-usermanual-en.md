---
description: "EN-UM-AWBusiness_5"
---


# Tutorial 1

---
## Surcharges

- **0** for an item-related surcharge/discount, e.g. for a surcharge for exceeding the maximum surface. It will be calculated for every item to which it applies.
- **900-999** for surcharges/discounts which shall be applied to all previous items or parts of the previous items.

*Fig. B-207 Customised special discount*

In this example, the item number 999 is entered. This means that the special discount will be applied at the end of the order items, and will be calculated for the total.

8. Select in the menu Start > Save to save the data.

The data will be saved.
To make sure that the surcharge/discount is applied, enable it in the customer's master data. If there is an additional, general special discount, only the customised special discount will be calculated for this customer.

---
*A+W Business Master data, B-401*

## Surcharges

### Fixing automatic surcharges

> Please obey the sequence in which product, price, and allocation have to be defined. In one of the following exercises you will check whether the special discount is applied as intended. The calculation of the surcharge value based on the changed surcharge base amount is still to happen. This guarantees that due to a dimension change, e.g. of the energy surcharge (reference basis is the weight), there is a recalculation, but the price per price unit is no longer updated. This prevents a constantly changing energy surcharge affecting documents for which the customer has already received an order confirmation. The fixing can be defined per footer surcharge in the surcharge management and also the status, starting with which it is fixed. By deleting the manual specifications (<Ctrl + Shift + V>), the recalculation can be forced in the item entry.
> ⇨ Sales: Software Reference, "Recalculate fixed special discounts/surcharges" on page C-1771

### Copy documents

When copying documents, there is a query whether the fixing of the surcharges should be eliminated. However, this counts only until the next transfer, then they are in dependence to the status active.

---
*A+W Business Master data, B-402*

## Surcharges

### Exercises

- Enter a special discount of 3% for your customer, to be automatically added as the last order item.
- Please obey the sequence in which product, price, and allocation have to be defined.
- In one of the following exercises you will check whether the special discount is applied as intended.

**Additional information**
⇨ "Editing the Customer's Financial Data" on page B-162
⇨ "Product Definition" on page B-245
⇨ "Input of Unit Prices" on page B-301
⇨ Software Reference, "Product Management" on page B-667
⇨ Software Reference, "Price Management" on page B-768
⇨ Software Reference, "Partner Management" on page B-808
⇨ Software Reference, "Surcharge Product Assignment" on page B-1049

---
*A+W Business Master data, B-403*

## Surcharges

### Complex Exercise

By means of an example, input of prices for a product is explained in detail in this exercise.

### Tasks

Let us start with an example of prices for a product used in standard price lists:

**Tab. B-16: Product prices**

**Prices/sqm x mm laminated lite**

| Surface sqm | 4 mm | 5 mm | 6 mm |
| :--- | :--- | :--- | :--- |
| | up to max. 1410 x 2400 mm | up to 1600 x 3000 mm | > 1600 x 3000 to 2450 x 3000 mm | up to 1600 x 3000 mm | > 1600 x 3000 to 2550 x 4500 mm |
| > 0.50 qm | 196.00 € | 202.00 € | 276.00 € | 208.00 € | 282.00 € |
| **A1** | | | | | |
| 0.16 – 0.50 qm | 253.00 € | 263.00 € | - | 271.00 € | - |
| 0.10 – 0.15 qm | 311.00 € | 323.00 € | - | 333.00 € | - |
| **A2** | | | | | |
| > 0.50 qm | 215.00 € | 224.00 € | 299.00 € | 230.00 € | 305.00 € |
| 0.16 – 0.50 qm | 281.00 € | 291.00 € | - | 299.00 € | - |
| 0.10 – 0.15 qm | 345.00 € | 358.00 € | - | 368.00 € | - |

The following calculation factors can also be applied for example:
- If the edge is longer than 3750 mm a surcharge of 30% shall be added
- The minimum production size is 200 x 300 mm
- The minimum calculation length per edge is 300 mm

For the examples from the table first define the number of limit types (sizes) to be considered:
- The surface limit (0.10 – 0.15 sqm; 0.16 – 0.50 sqm; over 0.50 sqm).
- The width:
  - For LG 5 mm there are two size limits (0<B1<1600 mm and 1600<B2<2450 mm) and for LG 6 mm one (2550<B2<4500 mm).
- Height:
  - For LG 6 mm there are two size limits, below and over 3000 mm.

This makes it a total of four limit types. The cube can take into account maximally three of them. The fourth size can be handled by a surcharge.

For every IG unit A1 and A2 and laminated lite thickness, six IG products are entered.
- **A1:**
  - IG A1 with LG 4 mm
  - IG A1 with LG 5 mm
  - IG A1 with LG 6 mm
- **A2:**

---
*A+W Business Master data, B-404*

- IG A2 with LG 4 mm
- IG A2 with LG 5 mm
- IG A2 with LG 6 mm

Now create a price table for each of the six IG products (= three price tables for every IG unit):
- For IG products with a 4 mm LG lite, vector price tables with one limit type: the surface.
- For IG products with LG 5 and 6 mm, cubic price tables with three limit types: surface, width, and height.

The fourth size is included as a surcharge for edge overlength from 3750 mm.

### Solution: Enter the Product and its Price

The example product is an IG unit. We are going to explain in detail how to proceed. At the same time, we are going to describe the cube (three-dimensional pricing). This will give you a good idea of how pricing works.

There are the following instructions on this subject.
- "How to enter the price as a cube" on page B-405
- "How to enter the miscellaneous surcharge" on page B-409
- "How to enter the IG product" on page B-410

#### Price tables with three limits

First check which price list and price key (rate) is used by default to determine the sales price for the IG unit.

**How to enter the price as a cube**
1. Go to menu Master data > Products > Prices > Price list.
   Dialog Price list appears.
   The checkboxes show the price lists active for standard calculation of the IG sales price.

---
*A+W Business Master data, B-405*

*Fig. B-208 Price list*

The column Stn. IG SP is important in this example. The price list used for IG sales is EURO Price 07 in this case.
2. Close the dialog and go to menu Master data > Prices > Rates.

*Fig. B-209 Rate: Year + key*

---
*A+W Business Master data, B-406*

As you see, several price keys can be allocated to the same price list. There are therefore various price list/key combinations that can be used for IG pricing. In this case, EURO Price 07 and Works VEGLA 97. This shows where the new price list has to be saved to make sure that the price will be used automatically.

3. Go to Master data > Products > Articles > Articles.
   Go to dialog Product management and check in which number area your IG products have been entered. Since price table and product should have the same number you should make a note of the free number.
4. Select menu Master data > Prices > Prices.
   Dialog Prices appears.
5. Go to the menu Start > New to switch to the input mode.

*Fig. B-210 Enter price*

6. Enter the number of the price table and select the price list and the price key.
7. Go to tab Cube.
   The solution for this exercise is:
   - **Width => Limit type 1:**
     - For LG 5 mm, 2 size limits 0<W1<1600 mm and 1600<W2<2450 mm, and

---
*A+W Business Master data, B-407*

- For LG 6 mm, 2550<W2<4500 mm
- **Height => limit type 2**
- For LG 6 mm split into two surfaces, below and above 3000 mm)
- **Surface limit = limit type 3**
  - (0.10 - 0.15 sqm; 0.16 – 0.50 sqm; over 0.50 sqm)

*Fig. B-211 Enter price*

For the third dimension of the cube, set up a tab for every size limit of Limit type 3. To view the prices for 0.15 – 0.50 sqm please switch to the corresponding tab. For the third dimension of the cube, set up a tab for every size limit of Limit type 3. To view the prices for 0.15 - 0.50 sqm please switch to the corresponding tab. Tab 0.15 includes prices from 0 - 0.15 sqm. Tab 9999.99 applies to a surface between 0.50 and 9999.99 sqm (these figures are inclusive values).

8. Enter the prices in all tabs.
   An additional calculation factor is the minimum calculation size of 300 x 300 mm. You will find that for the width and height, 300 mm has been defined as the lowest limit although the minimum production size is 200 x 300 mm. Pricing will only consider the limit sizes for calculation but not the production limits.
9. Select in the menu Start > Save to save the data.

---
*A+W Business Master data, B-408*

### Miscellaneous surcharge

A surcharge of 30% shall be applied if an edge is longer than 3750 mm.

#### How to enter the miscellaneous surcharge

1. Go to menu Master data > Products > Prices > Misc. surcharges

*Fig. B-212 Other surcharge*

Edge surcharges are entered in Misc. surcharges. In this example, the edge surcharge is found in surcharge table 10.
The first line defines that from 0 to 2400 mm, a surcharge of 0% shall be applied, i.e. no surcharge at all. Acc. to the second line, a 35.00% surcharge will be applied from 2400.01 to 3000 mm and 45.00% from 3000.01 mm upwards.
This includes all special rules.
Table number 10 for Misc. surcharges can be entered at two points:
- **Product:**
  If the table number is entered in the product in tab Price/surcharge, the edge surcharge will be applied always, even if another price table is used, e.g. for purchase orders.
- **Price table:**
  If the edge surcharge shall not be applied generally, enter the table number only in the corresponding price table. This makes sense for example if you want to create a special quote or if this surcharge shall not be valid for a certain customer.

2. Select in the menu Start > Save to save the data.

---
*A+W Business Master data, B-409*

When all price-relevant data of an IG unit have been defined, the IG unit can be entered as a product.

### Defining a product

This example shows the IG product 151000 which already exists. You will be able to see what you have to do to enter a similar product.

#### How to enter the IG product

1. Go to menu Master data > Products > Articles > Articles.
   Dialog Product management appears.
2. Go to the menu Start > New to switch to the input mode.

*Fig. B-213 Product management IG*

3. Enter the product number and a name.
4. Go to tab Price/surcharge and enter - among other things - the numbers of the price tables and - in field Misc. surcharge - the table for the edge length surcharge.
5. Enter the control code for the product.
6. Go to tab BOM to enter the structure of the IG unit.

---
*A+W Business Master data, B-410*

*Fig. B-214 Product management IG BOM*

7. Select the element after which a new element shall be added.
8. Open the context menu and select the corresponding entry:
   - **Enter element (before/after):**
     This serves to add an element on the same level, e.g. float to the main product.
   - **Add element:**
     This serves to add an element on a lower level, e.g. a spacer to the glass.
   You can enter more elements in the same way.
9. Select in the menu Start > Save to save the data.
   The data will be saved. The product has been entered. Other program parts can access this now and display and calculate the corresponding price, e.g. at order entry.

---
*A+W Business Master data, B-411*

## Discounts

Discounts are another means of amending the price for every single customer without having to change the price lists.

This subject area will introduce the discounts and their functions.

This includes the following training sessions:
- "Rabatthierarchie" auf Seite B-451
- "Rabattdefinition" auf Seite B-455

---
*A+W Business Master data, B-412*

## Hierarchy of Discounts

### Objectives
- Introducing the discount functions.
- Graduation of discounts.
- Defining a customer discount.

### Benefit
- Discounts reduce the list price of products when items are calculated in a document and are therefore an important tool for pricing.
- As discounts can be allocated quite specifically, pricing can be customised to a very high degree.

### Note

| Topic | Description |
| :--- | :--- |
| **Discount management** | Discounts can be defined for customer or supplier groups or for single customers or suppliers. The discount management logic is the same for customers and suppliers. |
| **Discount value** | Discounts can be graduated by means of a limit type. The defined value will always be interpreted as a percentage. |
| **Discounts in the rate system** | Discounts always refer to a price list, a price key, and a product or product group. |
| **Discount code** | Discounts will be applied only if the code has been set in product master data. |
| **Manual discount** | Discounts can be entered manually in the order. Manual discounts will overrule the discounts defined for the customer. |
| **Hierarchy of discounts** | Price calculation in the document first checks the item settings. The program will stop searching for a discount if valid agreements are found in the item or in partner discounts. |

---
*A+W Business Master data, B-413*

## The Function of Discounts

Discounts reduce the list price of products when items are calculated in a document. Discounts are defined for single customers or customer groups and refer to a product or a product group.

This discount is automatically applied to the order when the product is entered. If no discount has been defined you can enter a percentage in the order. This manual discount can either be entered in the order header for the whole order, or at item entry for an item or a BOM element.

You can enter different discounts:
- Standard discounts for a price list and a price key (rate)
- Graduated discounts with a quantity limit
- Exchange discounts

*Fig. B-215 Discounts for customer and customer group*

This example shows the discounts for a customer. The colors of the entries have the following meanings:
- **Blue**: Product groups
- **Red**: Product
- **Green**: Product group and project

Since discounts are applied only if the product or BOM element is marked 'discountable', they can be specifically allocated to individual BOM elements or to complete products.

*Fig. B-216 Product management - Price/surcharge*

---
*A+W Business Master data, B-414*

*Fig. B-217 Discount allocation options*

| Master data | Discountable | Customer A | Customer B | Customer C |
| :--- | :--- | :--- | :--- | :--- |
| Product IG 15000 | ☑ | **Discount on:** PGR Float, PGR Safe | **Discount on:** PGR IG | **Discount on:** PGR Float, PGR Spacer, PGR IG |
| Float 4 mm | ☑ | | | |
| Spacer | ☑ | | | |
| TG Safe | ☑ | | | |
| **Order** | **Calculation** | **IG price** - Discount Float - Discount Safe | **IG price** - Discount IG | **IG price** - Discount IG - Discount Float - Discount |

These examples show an IG product consisting of a float glass lite, the spacer, and a tempered glass lite. Discounts can be applied to all of those products. Whether the discount is applied in the order depends on the discount agreements made with the corresponding customer.

- Customer A gets discounts on float glass and on tempered glass.
- Customer B gets a discount on IG.
- Customer C gets discounts on IG, float glass, and the spacer.

You can also see that the discounts are adding up, i. e. that a discount is granted for the IG unit as well as for the BOM elements.

In this example, discounts are granted for whole product groups (PGR). Discount agreements can of course also refer to individual products.

> **Special discount**
> Automatic surcharges can also be used for defining general (generally applicable) discounts, e. g. for special promotions. These special discounts are never shown on the list of discounts.
> Special discounts must not be mixed up with the partner discounts described in this chapter.
> ⇨ "Automatic Surcharges" on page B-394

---
*A+W Business Master data, B-415*

## Discount Search

The following hierarchy applies to all calculations in orders:
- Entries made in the order (top priority)
- Agreements made in partner discounts

In this sequence, the next step will be performed only if the search produces no results. The following discount hierarchy is used for pricing:

*Fig. B-218 Pricing hierarchy*
1.  Product - 1004 **customer**
2.  Product - 1004 **customer group**
3.  PGR - 110 **customer**
4.  PGR - 110 **customer group**
5.  PSG - 11* **customer**
6.  PSG - 11* **customer group**
7.  MPG - 1** **customer**
8.  MPG - 1** **customer group**

Pricing in the document is also controlled by the settings made in company data system-wide. The individual settings are described in the Software Reference.
⇨ Software Reference, "Company Data > Price Calculation" on page B-970

---
*A+W Business Master data, B-416*

## Definition of Discounts

### Objectives
- Introducing standard-, exchange-, and graduated discounts.
- Definition of discounts.
- Defining a discount diversion.

### Benefit
- Discounts are means of pricing which can be used to adjust the price of an order specifically for a customer or a customer group.
- Based on supplier discounts, purchase prices can be calculated so accurately that the margins, e. g. for favourable offers, can be met.

### Note

| Topic | Description |
| :--- | :--- |
| **Customer Discount** | Customer discounts are analysed at the pricing of orders. |
| **Supplier Discount** | Supplier discounts are analysed when determining the purchase price. |
| **Standard discount** | Several discounts can be defined for a product group or a product, referring to different price lists and price keys each. One of the discounts has to be allocated as the default (standard) discount. |
| **Exchange discount** | Exchange discounts are granted for elements which are used in a BOM instead of the original element. |
| **Grad. discount** | Discounts can be graduated by means of a limit type. |
| **Discount diversion** | In discount management, diversions to other rates, rounding, minimum quantities, and surcharges can be set. This way, the standard settings can be overruled for every customer. |

> **Customer and supplier discounts**
> Customer and supplier discounts are entered in the same way and used for the calculation of documents. This chapter will just mention customer discounts to make the explanations easier to understand.

---
*A+W Business Master data, B-417*

### Discount Management Dialog

Dialog Discount management can either be opened for customers or for suppliers. The difference is limited to the selection of the partner or of the partner group. Otherwise, the tabs and fields are the same.

*Fig. B-219 Discount management - example: customer discounts*

- **A** Tab with details
- **B** Discount for partner or group
- **C** Discount for product or PGR
- **D** Discount rate and validity
- **E** Code for default discount
- **F** Discount rate
- **G** Price list
- **H** Price key
- **I** Validity

Discounts always refer to a price list (G), a price key (H), and a product or product group (C).

#### Time limit

You can define a time limit (D) for discounts if you enter several discount rates for a customer and a product or a product group. The discounts will only applied within the defined period in this case. This can be used e.g. to prepare special promotions.

#### Standard discount

You can enter different discount rates for the same product group by referring to two different price lists and price keys (rates). Just one discount rate can be marked as the default (E) rate however. This will be automatically suggested in the order and can be changed if required.

---
*A+W Business Master data, B-418*

### Project-related discounts

A discount can be restricted to a certain project. In this case, it will be used for pricing only if the order refers to this project. Since a validity can be defined for the project itself, project-related discounts do not have to have a time limit.

### Graduated discounts

Graduated discounts can refer to all limit types valid for the price lists and for surcharges. The discount can only be graduated by means of one limit type however.

### Exchange discounts

For exchange discounts, the discount granted for the lite to replace the original lite can differ from the discount granted for the IG unit. The exchange discount can be granted in addition to the discount for the IG unit if the settings in product master data are made accordingly.

**Example**
A 5% discount is granted on the surcharge for the exchanged glass.
10% discount will be granted for IG.

- Adopt from main item: 10% discount for IG will be granted.
- No adoption: 5% discount from the exchange discount will be granted.

The settings for adopting prices are described in detail in the Software Reference.
⇨ Software Reference, "Adopt main item" on page B-678

If a surcharge is applied when a lite of an IG unit is exchanged, the resulting exchange price may be reduced by the exchange discount.

**Example**

| Product | Price | Discount | Total |
| :--- | :--- | :--- | :--- |
| IG unit 2x4 mm float, 1 sqm, 1000x1000 mm | 60.00 € | 50% | 30.00 € |
| Replaced by TG | 75.00 € | 30% | 52.50 € |
| **Total** | | | **82.50 €** |
| Replaced by a toughened lite with a customised net price * | 75.00 € | 0% | 75.00 € |
| **Total** | | | **105.00 €** |

\* In this example, a customised price is calculated for the lite to be changed in which is why the discount is omitted.

If company data only permit an individual price, A+W Business first checks if an individual price has been entered. After that, the defined discount will be

---
*A+W Business Master data, B-419*

applied. The combination of rates defined for the individual price overrules the combination defined in Discounts.
⇨ Software Reference, "Several individual prices permitted" on page B-970

### Other agreements

By means of partner-related discounts you can enter different agreements, e. g. different minimum quantities, rounding, rates (rate diversion).

### Rate diversions

Diversions can refer to other rates if for the customer in question, other surcharges than those in the standard price lists shall be valid.

*Fig. B-220 Diversion of rates*

- **Price group-related surcharges:**
  If no price group-related surcharge is defined, the price list and the key (rate) of the main item will be automatically used for surcharge calculation. These surcharges can also be loaded from another price list and/or key. The system will check in this case whether appropriate price groups have been defined for the price list, the price key, and the product.

---
*A+W Business Master data, B-420*

- If so, the program will search for entries in group surcharges. If there are no entries, a message will be issued at order entry saying that no surcharges were found.
- **Price group-independent surcharges (exchange surcharges):**
  Exchange surcharges follow the same principle as price group-independent surcharges. The setting has to be edited only if the price list and/or key for the surcharge differs from that for the main item.
- **Miscellaneous surcharges:**
  If another surcharge shall be used for this customer or customer group, an appropriate diversion can be defined, e. g. miscellaneous surcharges for overlong edges.

---
*A+W Business Master data, B-421*

### The copy function

You can copy discounts while making the following changes:
- Transfer discounts to another price list or price key.
- Transfer discounts to another partner or group.
- Raise or reduce discounts in general by a percentage or by a fixed amount.
- Transfer or change discounts for a product or a PGR.

The copy function also allows changing all discounts at once without copying them to another rate. There are different options:
- Increase by a percentage or an absolute value.
- Reduction by a percentage or an absolute value.
- Increase or reduction to a fixed amount.
- Change rounding.

*Fig. B-221 Copy function for discounts*

---
*A+W Business Master data, B-422*

### Settings for Discount Calculation (Company Data)

Standard discount calculation can be modified in company data.

*Fig. B-222 Company data > Pricing*

**A** Settings for discount calculation

This tab is used for defining the options for the documents. Any changes on this tab will overrule the standard calculation in A+W Business.

For a detailed description of the checkboxes please refer to the Software Reference.
⇨ Software Reference, "Company Data > Price Calculation" on page B-970

---
*A+W Business Master data, B-423*

### Defining a discount

Discounts are defined for customers or suppliers or for customer or supplier groups. In the following example, dialog Discount management is opened for customers. The procedure is the same for Suppliers.

> **Copy discounts**
> If discounts have been entered already, you can copy and edit them for new customers or suppliers. In these new discounts, individual values can be changed or can be generally reduced or increased by a certain amount or percentage. This way, new discounts are easy to define. Please note that price year, price key, and rate for the target discount have to be entered before.

#### How to define a discount

1. Go to menu Master data > Partners > Customers > Customer discounts.
   Dialog Discount management pops up.
   ⇨ Software Reference, “Discount Management (Customers, Suppliers)" on page B-847
2. Go to the menu Start > New to switch to the input mode.

*Fig. B-223 Fields for the new discount accessible*

- **A** Customer for whom the discount is valid
- **B** Rate
- **C** Product for which the discount is valid
- **D** Default discount (standard discount)
- **E** Amount of discount

Tabs Discount list and Table will be released only after the new discount has been saved.

---
*A+W Business Master data, B-424*

3. Choose the option Customer (A) and select the customer for whom the discount shall be entered.
4. Select the price list and the price key (B).
5. Select the option Product (C) and the product for which the discount shall be granted.
   The appropriate fields are accessible now.
6. Go to field Discount and enter the value (E).
   The value will always be interpreted as a percentage.
7. Check the checkbox Default discount (D) if this discount shall be granted by default.
   You have filled in the mandatory fields now. All additional entries can be made later.

*Fig. B-224 New discount*

8. Select in the menu Start > Save to save the data.
   The data will be saved. The new discount appears on tab Discount list. You can add further data now, e. g. a graduation.

---
*A+W Business Master data, B-425*

### Defining a Graduated Discount

Every discount can be graduated by a limit type. The limit types are the same as for graduated prices and surcharges.

#### How to enter a graduated discount

1. Go to menu Master data > Partners > Customers > Customer discounts.
   Dialog Discount management pops up.
   ⇨ Software Reference, "Discount Management (Customers, Suppliers)" on page B-847
2. Enter a new discount or select the discount to be graduated.
   ⇨ "Defining a discount" on page B-424
3. Go to tab Graduated discount to enter the steps for the graduation.

*Fig. B-225 Define the graduation*
- **A** Limit type for the graduation
- **B** Column header for discount levels

4. Go to field Quantity limit unit (A) and choose the limit type, e. g. pcs.
   The setting appears in the column header (B).
5. Use the <Tab> key to go to the next field and press <Ins>.

---
*A+W Business Master data, B-426*

*Fig. B-226 Fields for graduated discount are accessible*
- **A** Value of the level (limit)
- **B** Amount of discount

6. Enter the value (A) for the first level, e. g. 5 (pcs.).
7. Enter the value (B) for the discount, e. g. 0 (%) if the discount shall be granted from 6 pcs. upwards.
8. Press <Ins> and repeat steps 6 to 8 until all levels have been defined.
   You can define the discount graduation in the same way as the graduated vector price.
9. Select in the menu Start > Save to save the data.
   The data will be saved. The new discount appears on tab Discount list.

*Fig. B-227 Graduated discount - overview*

### Defining an Exchange Discount

Exchange discounts are granted for elements which are used in a BOM instead of the original element. If a surcharge is applied when a lite of an IG unit

---
*A+W Business Master data, B-427*

is exchanged, the resulting exchange price may be reduced by the exchange discount.
An exchange discount can refer to a single product or to a whole product group.

#### How to enter an exchange discount

1. Go to menu Master data > Partners > Customers > Customer discounts.
   Dialog Discount management pops up.
2. Enter a new discount or select the discount to be edited.
   ⇨ "Defining a discount" on page B-424
3. Go to tab Exchange discounts to enter the exchange product for which the discount shall be granted.

*Fig. B-228 Define an exchange discount*
- **A** Product (or PGR) for which a different discount shall be granted for an exchange
- **B** Discount rate for the product
- **C** Accessible line
- **D** Product replacing the original one
- **E** Exchange discount for the product

⇨ Software Reference, "Discount Management (Customers, Suppliers)" on page B-847

The fields for the discount information (A, B) have been filled in when the discount was defined. The exchange discount for a product is entered as described below.
The procedure is the same for a product group.

4. Select the first line (C) in section Products and press <Ins>.

---
*A+W Business Master data, B-428*

You can repeat pressing the <Tab> key until the cursor is on section Products.

5. Go to field Product (D) and choose the new product to be used.
   The product name appears on the list.
6. Go to field Discount (E) and enter the percentage to be granted for the exchanged product.
7. Select in the menu Start > Save to save the data.

The data will be saved. To enter further exchange discounts, select the last entry on the list and repeat steps 4 to 7.

---
*A+W Business Master data, B-429*

### Defining a Diversion of Rates

Prices, discounts, and surcharges are always allocated to a rate (price list and key). When a product is entered in a document, price and surcharges are loaded from the allocated price list. You can define however that the prices and/or surcharges for certain customers shall be loaded from another rate, e. g. if an order refers to a project for which special rates have been defined.

#### How to define the diversion to another rate

1. Go to menu Master data > Partners > Customers > Customer discounts.
   Dialog Discount management pops up.
   ⇨ Software Reference, "Discount Management (Customers, Suppliers)" on page B-847
2. Enter a new discount or select the discount to be edited.
   ⇨ "Defining a discount" on page B-424
3. Go to tab Divergences to select other rates.

*Fig. B-229 Divergences to other rates*
- **A** Product (or PGR) for which the divergences shall be valid.
- **B** Project for which the divergences shall be valid.
- **C** Different rate for prices
- **D** Different rate for group surcharges
- **E** Different rate for exchange and shape processing surcharges
- **F** Different discount

In this example, divergences are defined for a project if a certain product is entered in an order for this project. The procedure is the same for a product group.

---
*A+W Business Master data, B-430*

4. Choose the project (B) for which the different rates shall be valid.
5. Choose the product (A) for which the different rates shall be valid.
6. Enter a different discount (F) for the product if required.
7. Select the different rates:
   - for the prices (C)
   - for the price group-related surcharges (D)
   - for the price group-independent surcharges (E).
   If no different rate is set, the standard rate will be used.
8. Choose another Misc. surcharge for this customer is required.
   Another miscellaneous surcharge has to be selected only if this surcharge shall differ from the surcharge entered in the product definition.
9. Select in the menu Start > Save to save the data.
   The data will be saved. The divergences for the rates have been defined.

---
*A+W Business Master data, B-431*

### Copying and Changing Discounts

You can copy discounts, increasing or reducing them at the same time.

> **Prerequisite**
> If a discount for a new rate (price list, key) shall be copied, the new rate must be defined first.
> ⇨ "Editing rates" on page B-292

There are the following instructions on this subject.
- "How to copy discounts" on page B-432
- "How to change discounts in general" on page B-434

#### How to copy discounts

1. Go to menu Master data > Partners > Customers > Customer discounts.
   Dialog Discount management pops up.
   ⇨ Software Reference, "Customer" on page B-846
2. Go to menu Functions > Copy discounts.

*Fig. B-230 Sources and target data for copying*
- **A** Select the group
- **B** Customer whose discounts will be copied
- **C** Rate (year, key)
- **D** Choose the product group
- **E** Action for target discounts

⇨ Software Reference, "Change/Copy Discounts" on page B-853

In this example, a customer's PGR discount is copied to a customer group.

3. Choose the customer (B) whose PGR discount shall be copied.

---
*A+W Business Master data, B-432*

The customer name is loaded when you press <Tab> to continue.
4. Check the option Group (A) and select the customer group to which the discount shall be transferred.
5. Check the checkboxes for the rate (C).
   The fields Price list and Key for the source and the target are accessible.
6. Select the price list and the key.
7. Check the checkbox PGR (D).
   The fields for selecting the product groups are accessible.
8. Select the PGR or the series of product groups the discounts of which shall be copied.
   If you enter the same PGR in both fields, just this one will be copied.
9. Check the checkboxes (E) for the target discount:
   - The existing discounts can be changed. If you do not check the checkbox, the existing discounts will not be changed but completed by the new discounts.
   - All copied discounts can get the default discount code. This code will be deleted for the existing discounts.
10. Click on [OK] to adopt the data.

*Fig. B-231 Copy discounts*

The discounts are copied and saved for the customer group. A message will tell you how many discounts were copied. In discount management you can view the discounts for the customer group and edit them if required.

---
*A+W Business Master data, B-433*

#### How to change discounts in general

1. Go to menu Master data > Partners > Customers > Customer discounts.
   Dialog Discount management pops up.
2. Go to menu Functions > Change discounts.
   Dialog Copy discounts appears with the tab Change discounts.

*Fig. B-232 Change discounts*
- **A** Value of the change
- **B** Type of change
- **C** Select all discounts
- **D** Select the customer or group
- **E** Rate (year, key)
- **F** Discounts to be changed
- **G** Target rate (price list, key) for copying

3. Choose one of the following options from the fields in section Source:
   - Check the checkbox all (C) to change all discounts. Enter the price list and the key (E) to which the discounts have been allocated.
   - Determine the discount by selecting the customer (D) or customer group, the price list, the key, the product group, and the product.
4. In section Change discount, choose the option (B) for the change and enter the corresponding value (A):
   - **Absolute** and a number, e. g. 5 or -5 if the discounts are to be increased or reduced by 5 Euros.
   - **Percentage** and a number, e. g. 2 or -2 if the discounts are to be increased or reduced by 2%.
   - **Fixed** if a fixed value shall be applied to the discounts, e. g. 12 to set all selected discounts to 12%.

---
*A+W Business Master data, B-434*

5. First choose the price list and the key (G) in which the changes shall be saved.
6. Now check the checkboxes (F) for the discounts to be changed.
7. Click on [OK] to adopt the data.
   The data will be saved.

---
*A+W Business Master data, B-435*

### Exercises

- Enter the following discounts for your training customer:
  - Standard discount for colored float glass
  - Graduated discount for laminated glass lites of 8 mm thickness
  - Exchange discounts for the PGR IG
- Copy these discounts to another rate and raise the discount rate by 5%.
- Define a divergence of rates for your customer where the price group-independent exchange surcharges are diverted to PGR 2**.

**Additional information**
⇨ Software Reference, "Change/Copy Discounts" on page B-853
⇨ Software Reference, "Delete Discounts" on page B-856
⇨ Software Reference, "Company Data > Price Calculation" on page B-970

---
*A+W Business Master data, B-436*

## Additional Information on the Company

Company-related settings can be made in various dialogs, e. g. to define access rights for A+W Business or for maintaining clients and subsidiaries. The major settings are explained in connection with this set of topics.

This includes the following training sessions:
- "Firmenbezogene Daten" auf Seite B-476
- "Mitarbeiterverwaltung" auf Seite B-491

---
*A+W Business Master data, B-437*

### Company-related Data

#### Objectives
- Getting an idea of the global settings.
- Introducing clients and subsidiaries.
- Entering one's own bank accounts.
- Defining sales representatives and commissions.

#### Benefit
- General settings control the program behaviour, irrespective of customer, prices, and products.
- These settings are valid for a client with its subsidiaries.
- Commissions are paid to the sales representatives based on the sales for product groups and/or territories.

#### Note

| Topic | Description |
| :--- | :--- |
| **System settings** | Global settings apply to the client for whom they have been entered. They refer e. g. to pricing, interfaces, archiving. |
| **Database** | The current data are maintained in the main database. Invoiced documents are archived in separate databases. Documents can be copied from archives database to the main database. |
| **Financial accounting (FinAcc)** | There are different interfaces for exchanging data with financial accounting (FinAcc) programs. Various functions depend on the financial accounting program used, e. g. the external key, receivables reports. |
| **Data transfer** | Data transfer to other programs is usually controlled by a workflow task, e. g. transfer to financial accounting or archives. |
| **Clients** | Clients access the same server and the same database. They use the same master data, e. g. products, product groups, prices, terms. |
| **Subsidiaries** | Several subsidiaries can be defined for a client. They use the same customer and order data. Subsidiaries of clients can be billed separately. |
| **Sales territory** | A sales territory has the following functions: Calculation of commission (sales commission), Sorting criterion in A+W Business sales statistics. |
| **Sales representative** | Sales representatives are entered as employees. To define an employee as a sales representative, he is assigned a sales territory. |
| **Commission** | Commission can refer to single sales persons, product groups, and/or rates. |

---
*A+W Business Master data, B-438*

| Note | |
| :--- | :--- |
| **Commission splitting** | Commissions can be split proportionally to two sales persons. The actual splitting is defined in the order. |

---
*A+W Business Master data, B-439*

### System Settings

You can define the standard settings for your company in Company data. Apart from financial accounting and other interfaces, this includes price calculation, e.g. the currency to be used, and how discounts shall be applied.

A+W Business allows to manage several clients and their subsidiaries. For every client, you can define the default settings to match his business processes.

#### Financial accounting (FinAcc)

By default, A+W Business is installed with interfaces to various financial accounting programs. This is why you have to choose the right interface for importing and exporting invoice data. Various functions depend on the financial accounting program used, e. g. the external key.

Depending on the interface, invoices are transferred to financial accounting automatically or manually. The status defines the minimum status an invoice has to have for this purpose. A lock status is defined to make sure it is not transferred to financial accounting a second time.
⇨ Tutorial 2, "Lock status" on page B-497

Cash sales invoices are excluded from transfer to financial accounting by giving them a special status.

If your financial accounting system allows to import customers and suppliers entered in A+W Business via interface, you do not have to keep your customers' and suppliers' data twice. The customer or supplier number is used to allocate and book orders and purchase orders.

Minor customers are invoiced as so-called Miscellaneous customers, for which a collective account in your financial accounting system is used. This saves you from having to create individual accounts for those customers.

The receivables report lists all unpaid invoices, stating the sum, reminder date, and reminder level. The credit limit and the credit limit snapshot complete the current state of accounts for the individual customer.

#### Database

The main database includes all documents entered in A+W Business. To keep up the usual processing speed, old documents have to be archived and deleted from this database.

Documents are simultaneously transferred to archives and statistics, before being deleted from the main database by default. Generally, transfer to statistics is based on the month in which the document was issued while archiving is based on the year.

Upon transfer of the data to archives, the main database is re-initiated to restore the usual processing speed.

#### Archiving

Completed business transactions will remain in the main database for a defined period after which they are automatically archived. This is based on the

---
*A+W Business Master data, B-440*

minimum status you have defined for archiving. All document data are saved as they are. Copies can be loaded from archives.

*Fig. B-233 Settings for archiving*
- **A** Global settings for archiving
- **B** Document-related settings
- **C** Archiving year
- **D** Requirements for archiving

This example shows the settings that can be made in general (A) and those for the individual document types (B).

Archives form separate databases, each summing up a year (C). At the change of year, the system archives the documents in the corresponding archives, based on the invoice date.

Documents can be transferred to archives manually, by means of a number manager. Since archiving requires a lot of computer capacity, it is done automatically in the evenings.

#### Statistics

The Statistics module in A+W Business offers a number of reports. Documents are transferred to statistics for analysis. For every document type, you can define whether and when the corresponding document is to be transferred.

---
*A+W Business Master data, B-441*

Documents are simultaneously transferred to statistics and archives. For statistics, certain order data are saved in a special table in the main database.

#### Day-end closing

Invoices can be transferred to financial accounting e.g. once a day, in a nightly batch. When transferred to financial accounting, documents are usually (automatically) transferred to archives and to statistics.

By means of the defined deadlines (storage days) the system checks how long these shall remain in the main database before they are automatically deleted.

All data older than the defined deadline will be deleted from the main database. You can define the deadline by document type.

**Example**
To create annual overviews, you should enter a long interval to have sufficient time for creating the analysis.

Commission statistics are based on the rhythm in which commissions are calculated.

### Clients and Subsidiaries

Clients are used if several companies want to access the same server and database. Clients use the same master data, e. g. products, product groups, prices, terms. They maintain their own customer data however.

Your company can manage subsidiaries as well as clients with subsidiaries. The version you choose depends on how customer data and orders shall be managed:
- Set up clients if your subsidiaries shall maintain their own customer data and orders.
- Set up subsidiaries if the subsidiaries use the same customer data.

The financial accounts for each client can be maintained separately. Internal work or services can be invoiced among clients.

---
*A+W Business Master data, B-442*

*Fig. B-234 Company, client, subsidiaries - master data, customers, orders*

This example shows that e. g. the number ranges for the customer numbers are defined per client. The document numbers are taken from separate number ranges.

The settings for documents and pricing are made by client. Among other things, this defines how items are entered and shown in the document. The parameters for pricing partly overrule the standard calculation defined in master data. Basically, the price and discount settings for individual customers or customer groups have top priority.

In case of subsidiaries, master data are only maintained by headquarters and are transferred to the subsidiaries (replication). If a product is deleted at headquarters, it will not be automatically deleted at the subsidiaries however. It has to be deleted manually in all subsidiaries. This way, the subsidiaries can delete a product from product management when it has been sold out.

Prerequisite for replication is that all subsidiaries are using A+W Business and that all databases have the same release.

---
*A+W Business Master data, B-443*

### Definition of Clients

A+W Business allows to manage several clients with several subsidiaries each. Company settings are valid for a client with its subsidiaries. Clients cannot be deleted (referential integrity).

Before entering a client you should define the facts that distinguish him from other clients. This will help you amend the specific settings for the client, e. g. number ranges, automatic surcharges, rounding allocations, customer numbers.

> **Maintaining the settings per client**
> Please note that new clients should be entered based on existing data. Afterwards you should check and amend the settings in all dialogs.

#### How to enter a client

1. Go to menu Master data > Company > Company data.
   Dialog Company data appears.
2. Go to tab Table and select the client that matches the new client best.
3. Go to the menu Start > New to switch to the input mode.

*Fig. B-235 Fields for new the new client are accessible*
- **A** Number, internal company number
- **B** Address
- **C** Communication data

⇨ Software Reference, "Company Data - Client" on page B-943
4. Amend the client and company numbers.

---
*A+W Business Master data, B-444*

Once it has been saved, the client number cannot be changed.
5. Enter a unique matchcode if required.
6. Enter at least the address and communication data.
7. Select in the menu Start > Save to save the data.
   The data will be saved.
8. If necessary, amend further settings in dialog Company data.
9. Select in the menu Start > Save to save the data.
   The data will be saved. You should now check which other amendments this client requires, e. g. number ranges, automatic surcharges.

### Enter the Bank Account

You can enter several accounts with different banks for your own company and for every client.

If several bank accounts have been entered for a client, one of them must be marked as the main bank.

> **Prerequisite**
> A client's account number can be entered only if the bank data have been defined before. The IBAN can only be calculated automatically if all bank data have been entered.
> ⇨ "Banks" on page B-151

#### How to enter bank accounts for a client

1. Go to menu Master data > Company > Banks.
   Dialog Banks appears.
   ⇨ Software Reference, "Banks" on page B-1045
2. Choose the client for which data shall be entered.
3. Go to the menu Start > New to switch to the input mode.
   All fields will be deleted if no bank account has been entered for the selected client yet.

---
*A+W Business Master data, B-445*

*Fig. B-236 Fields for the new bank account are accessible*
- **A** Select bank
- **B** Account number
- **C** Code for the main bank

4. Click on the zoom icon to choose the bank (A).
   The bank data are loaded now.
   If no bank data have been entered yet you can use the directory icon to open the corresponding dialog and add the data.
5. Enter the account number (B).
   The IBAN is automatically determined and displayed.
6. If necessary, check the checkbox Main bank (C).
   You can change this code later, after you have entered all bank accounts.
7. Choose the client for which data shall be entered.
   You only need to select the client when you enter the first bank account. This step can be omitted when you enter further bank accounts for this client.
8. Select in the menu Start > Save to save the data.
   The data will be saved.

---
*A+W Business Master data, B-446*

### Sales Commission

Dialog Sales commission serves to enter the commission rates for the individual sales persons. You have to enter a commission rate for every salesman and at least for every main product group (MPG).
Commissions can be distinguished by price list. If <n.e.> is selected for the price list and the key, the commission rate is valid for all rates.

*Fig. B-237 Administration – Sales commission*
- **A** Commission is generally applicable
- **B** Calculation basis
- **C** Quantity (units) for which the commission rate is calculated
- **D** Commission rate per graduated quantity

The commission can be graduated at random.

**Examples: Graduated by discount, graduated by sales**

| Up to % Discount | % commission | up to sales | % Commission |
| :--- | :--- | :--- | :--- |
| 10 | 5 | 999,999,999 | 5 |
| 20 | 3 | 5,000 | 3 |
| 40 | 1 | 1,000 | 1 |
| 99 | 0 | 0 | 0 |

The graduated quantity depends on the commission type.

---
*A+W Business Master data, B-447*

**Example**

| Commission type | Quantity |
| :--- | :--- |
| Discount % | Discount granted per order/item |
| Marginal income % | Marginal income in percent |
| Sales | Total sales of the salesman |
| Marginal income | Marginal income |
| Price/PU | Price per quantity unit |

#### Commission splitting and manual commission rates

Sales representatives are allocated in partner data. If two sales representatives are entered you can define how the commission is going to be distributed. Calculation of sales commissions is based on orders.

*Fig. B-238 Customer data - tab Sales*

The entries in customer data are adopted for the order and can be changed if required.

*Fig. B-239 Order – preset entries for sales representatives*
- **A** Tab Document: Salesman 1
- **B** Tab Supplement: Salesman 2
- **C** Share in commission

If no details are entered for the second salesman (in the order), he will get no commission for this order. Commission splitting refers to the commission which calculated based on the entries in dialog Sales commission.

The settings made at item entry can be changed in the order.

*Fig. B-240 Item - tab Supplement*

You can enter two different commission rates per item. These will be allocated to salesman 1 and salesman 2 respectively.

---
*A+W Business Master data, B-448*

**Calculation examples**

| | |
| :--- | ---: |
| Commission 0.75 % on the glass price | |
| Order = 2000.00 € for glass, commission splitting | 15.00 € |
| Salesman 1 | 10.05 € |
| Salesman 2: 33.5 % | 4.95 € |
| Item = 2000.00 €, manual commission rates | |
| Salesman 1: 1.00 % | 20.00 € |
| Salesman 2: 0.75 % | 15.00 € |

#### Calculation of commissions

The sales commission is calculated per item, based on the PGR of the item. If complaints are taken into account for calculation, the commission will be lower. For statistical analysis, the orders can be transferred to commission statistics. In this case, orders will be transferred to commission statistics when they are transferred to archives. These functions have to be enabled in company data.

⇨ Software Reference, "Company Data > Archives" on page B-989

By default, the sales commission is calculated when documents are transferred to archives. The following settings must be enabled in company data for this purpose:
- On tab Archives, the checkbox Transfer to commission statistics.
- On tab Parameters, the checkbox Interactive sales commission.

*Fig. B-241 Company data - tab Parameters*

If this function is not active, the commission rates defined in master data for calculating the commission will be loaded only when the order is transferred to commission statistics.

Orders can also be transferred manually. This is done by means of the archiving dialog in module Documents.

These settings for commissioning are valid for orders and credit notes.

---
*A+W Business Master data, B-449*

### Entering the Commission

In this example we are going to enter a graduated commission which shall be valid for all price lists.

#### How to enter a sales commission

1. Go to menu Master data > Company > Sales commission.
   Dialog Sales commission appears.
   ⇨ Software Reference, "Commission" on page B-1043
2. Go to the menu Start > New to switch to the input mode.

*Fig. B-242 Fields for new commission rate are accessible*
- **A** Salesman
- **B** Rate
- **C** Commission type
- **D** Quantity graduation
- **E** Percentage of the commission

3. Enter the rate (price list and key) if required (B).
   If you enter <n.e.> in both fields, the commission will be valid for all price lists.
4. Choose the salesman (A).
   Only the employees entered in dialog Sales areas will be offered for selection as sales representatives. If you choose <n.e.>, the commission will be valid for all sales representatives.
5. Choose the commission type (C), e. g. sales.
   These are the minimum entries for the header. These details cannot be changed afterwards. If you enter the commission rate now, you can only

---
*A+W Business Master data, B-450*

add the graduation and the percentage of the commission. To differentiate the commission further, please enter data on customers, etc.

6. Select a customer, the product group and/or the product if required.
   If no entries are made in these fields, the commission will be valid for all customers, product groups, and products.

> **Changing the details**
> The entries made in steps 3 to 6 cannot be changed later. You should therefore check the fields thoroughly before performing the next step. Should you detect later that the commission has been defined incorrectly, you will have to delete all data and enter them again.

7. Enter the value for the graduated quantity (D) and the commission rate (E).
   If the commission shall not be graduated, enter 99999999 for the quantity.
8. Select in the menu Start > Save to save the data.
   The data will be saved.

#### How to enter a graduated commission

1. Enter a commission rate as defined in the previous paragraph.
   The size of the first graduation step does is irrelevant.
2. Select the commission rate for which another level shall be defined.
3. Go to the menu Start > New to switch to the input mode.
   Please make sure to adopt the settings in section Select salesman/product group as they are.
4. Enter the value for the graduated quantity (D) and the commission rate (E).
5. Select in the menu Start > Save to save the data.
   The data will be saved.
6. Repeat steps 3 to 5 until all levels have been defined.

| Salesman ID | Name | Commission type | Graduated qty. | % Commissi... | Valid from date | Price list | Price key | Customer Na... |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| | T** | Training Turnover | 1,000.00 | 0.250 | 01.01.2013 | <K.A> | <K.A.> | 4000 A+WT |
| | T** | Training Turnover | 10,000.00 | 0.500 | 01.01.2013 | <K.A> | <K.A.> | 4000 A+WT |
| | T** | Training Turnover | 100,000.00 | 0.750 | 01.01.2013 | <K.A> | <K A.> | 4000 A+WT |

The sequence in which the commission rates are listed has no effect on the calculation. They can be sorted by double-clicking on a column header.

#### How to delete a sales commission

1. Go to menu Master data > Company > Sales commission.
   Dialog Management - Sales commission appears.
2. Select the commission rate to be deleted.
3. Go to menu Start > Delete.

---
*A+W Business Master data, B-451*

4. Confirm the security check by [Yes].
   The selected commission rate will be deleted.

---
*A+W Business Master data, B-452*

### Management of Employees

#### Objectives
- Entering employee data and managing them by means of groups.
- Defining access rights for employees.

#### Benefit
- Only registered employees can use A+W Business. This helps to prevent unauthorised access to the data.
- Users can have different rights. This way you can define which employees can access certain data.

#### Note

| Topic | Description |
| :--- | :--- |
| **Data protection** | Personal data are subject to data protection. Please make sure that this kind of data is protected from improper use by means of the appropriate access rights. |
| **Employee data** | Using A+W Business requires entering the employees' access data. Only registered users will be able to start the program. |
| **User rights** | Your company's employees can have different access rights for the data in A+W Business. These rights are defined by restrictions. |
| **User group** | The following groups of employees/users are set by default: Manager, Supervisor, User, Management. Each of these groups has different access rights which are based on the operational tasks. |
| **Profile** | Allocation of rights is made easy by predefined profiles. |
| **Prerequisite** | You can enter new users only if you have system administrator's rights. |

> **Employees (m/f)**
> Female as well as male employees can use A+W Business of course. In this session we are going to use the male form for reasons of legibility. The female sex is included as a matter of fact. Combinations (male and female employees) do not conform to the rules of German spelling and are therefore not used.

---
*A+W Business Master data, B-453*

#### Staff

All users working with A+W Business have to be entered in the system. The user's real name will be saved for all of his actions. This name will appear in some of the dialogs, e. g. in dialog Number manager. You can also define special number ranges for every user. Every user can create his own number manager.
Program login requires a password. The login can be linked with the Windows login in company data.

> **Data protection**
> Personal data are subject to data protection. Please make sure that this kind of data is protected from improper use by means of the appropriate access rights.

User data cannot be deleted. If a user does no longer work for the company, he has to be blocked in user management.

#### Presetting for documents and order areas

Settings for documents and order areas allow to allocate the processing of documents to a client, an order area, and certain document types. These settings can be changed in the actual documents.

*Fig. B-243 Presetting for documents*
- **A** Document types and order areas
- **B** Standard document for this user

This example shows that for purchase orders, a certain document type has been assigned to the user.

---
*A+W Business Master data, B-454*

If you enter the order area as well you define that the documents of this user will be automatically allocated to the order area, using numbers from the corresponding number range.

The entry in column General (A) will overrule the entries for the other document types and order areas. This means that you cannot choose at random in this case:
- **<n.e.> or another selection:**
  All other columns are <inactive>.
- **<inactive>:**
  The document type or order areas can be selected in the other columns.

---
*A+W Business Master data, B-455*

**Example: Order area - column General**

| Value | Description |
| :--- | :--- |
| **<n.e.>** | If no settings have been made for the documents, no presetting will be used for the order areas. In this case, the user has to make sure to select the right order area and document type. |
| **Tempered glass** | No presetting can be made for documents. When the user enters a document, the order area TG will be preset by default. The document will get a number from the corresponding number range. The number will be assigned when the document is saved. |

### Employee Groups

The following user groups exist by default: manager, supervisor, user, management. Each group has different access rights, depending on their tasks in the company. Predefined user groups and user rights can be edited and completed by new ones.

In case of extensive modifications, it might be better to create a new group with the appropriate rights.

If you allocate a (new) user to a user group, he will automatically get all the rights defined for this group. If he is to get other rights, these can be completed or amended especially for him.

### User Rights

Your company's employees can be granted different access rights to the data in A+W Business so that you can specify which areas shall be open or locked for the individual users.

The following rights can be granted or withdrawn:
- **Change:**
  Data can be edited.
- **Insert:**
  New records can be entered.
- **Delete:**
  Records can be deleted.
- **Execute/read:**
  The dialog can be opened.

For these settings you have to bear the logical connections in mind: If a user is entitled to enter data he also has to have the right to open the corresponding dialog.

The allocation of rights refers to all program sections in A+W Business, down to dialog level, and partly the fields as well.

**Example**
If a user shall be able to see prices in archived orders in module Documents, he has to have the right of executing the program items 0055 Documents-Archives-Search order and 0002 Price view.

---
*A+W Business Master data, B-456*

*Fig. B-244 Management of rights*
- **A** User group or user
- **B** Program and sub-right
- **C** Display of rights for the selected program

This example shows that the selected group is entitled to read the sales prices in an order but cannot change, add, or delete them (C).

> **Rights are defined by restrictions**
> All displayed program items are defined with limited rights. Program items that are not displayed can be used without restrictions.

Rights are granted or withdrawn according to the following system:

| Program item (dialog, field) | Right |
| :--- | :--- |
| Not listed. | Full access |
| Listed, no checkbox checked. | Dialog or field is locked. |
| Listed, but one or more checkboxes have been checked. | The corresponding action can be taken. |

#### User profiles

Allocation of rights is made easy by predefined profiles. These offer the following settings:

---
*A+W Business Master data, B-457*

- **All programs without rights**
  Records are created for all programs; the rights to execute, change, add, and delete are disabled, e. g. for employees who have left the company.
- **All programs executable:**
  Records will be created for all programs. Only the right to execute is enabled. All others are disabled. Dialogs can only be opened.
- **All programs with all rights**
  In this case, all entries are deleted for the group in question which, like the supervisor, is granted all rights.

---
*A+W Business Master data, B-458*

### Examples of Group and User Rights

In dialog Management of rights, rights are granted or withdrawn by means of checkboxes.

When a checkbox is checked, this is always an exception from the general rule/setting. This is demonstrated in the following examples.

These very basic examples deal only with the main programs as it would be quite confusing to mention all sub-items. It goes without saying that rights can be allocated to sub-items as well.

#### Group: Supervisor = System administrator

*Tab. B-17 Access rights - supervisor*

| Program | Sub-right | Execute | Change | Add | Deletion |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Master data | x | | | | |
| Documents | x | | | | |
| Production | x | | | | |
| Statistics | x | | | | |
| Stock | x | | | | |
| Capacity planning | x | | | | |
| Utilities | x | | | | |
| References | x | | | | |

x: all rights (no entry)

The supervisor is automatically granted all rights. This is why no programs are listed and no checkboxes are checked.

#### Group: User

*Tab. B-18 Access rights - user*

| Program | Sub-right | Execute | Change | Add | Deletion |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Master data | | ☑ | ☐ | ☐ | ☐ |
| Documents | | ☑ | ☑ | ☑ | ☑ |
| Production | | ☑ | ☐ | ☐ | ☐ |

x: all rights (no entry)

---
*A+W Business Master data, B-459*

*Tab. B-18 Access rights - user (continued)*

| Program | Sub-right | Execute | Change | Add | Deletion |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Statistics | | ☐ | ☐ | ☐ | ☐ |
| Stock | | ☑ | ☐ | ☐ | ☐ |
| Capacity planning | | ☑ | ☐ | ☐ | ☐ |
| Utilities | | | | | |
| | Order info | ☐ | ☐ | ☐ | ☐ |
| | Debt./Cred. | ☐ | ☐ | ☐ | ☐ |
| References | x | | | | |

x: all rights (no entry)

The group Users can enter, change, delete, and execute documents. In modules Master data, production, stock, and capacity planning this group can only open certain dialogs because the checkboxes Change, Add, and Delete have not been checked. In module Utilities this group cannot open the dialogs Order info and Debtors/Creditors to FinAcc but has full access to all other dialogs of this module. This group has no rights for the modules Statistics and references.

#### Employee: Marc Tender, user

*Tab. B-19 User's access rights*

| Program | Sub-right | Execute | Change | Add | Deletion |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Master data | | ☑ | ☐ | ☐ | ☐ |
| | Partner | ☑ | ☑ | ☑ | ☑ |
| Documents | | ☑ | ☑ | ☑ | ☑ |
| Production | | ☑ | ☐ | ☐ | ☐ |
| Statistics | x | | | | |
| Stock | | ☑ | ☐ | ☐ | ☐ |
| Capacity planning | x | | | | |
| Utilities | | | | | |
| | Order info | ☐ | ☐ | ☐ | ☐ |
| | Debt./Cred. | ☐ | ☐ | ☐ | ☐ |
| References | x | | | | |

x: all rights (no entry)

---
*A+W Business Master data, B-460*

The user Marc Tender belongs to the group Users. He has also full access to the modules Statistics, Capacity planning, and References. He can also enter, edit, and delete partners in master data.

---
*A+W Business Master data, B-461*

### Input of User Data

When you enter the data for a user you have to define the so-called real name. Once saved, this entry cannot be changed.

You also have to enter a password by means of which the user can log into A+W Business. If the login function in connection with the Windows login is active in company data, the user name and the password for the Windows login must be entered in A+W Business.
⇨ Software Reference, "Use Windows registration for A+W Business login" on page B-1000

> **Prerequisite**
> You can enter new users only if you have system administrator's rights.

There are the following instructions on this subject.
- "How to enter a user" on page B-463
- "How to copy the standard settings for documents" on page B-465

> **Data protection**
> Personal data are subject to data protection. Please make sure that this kind of data is protected from improper use by means of the appropriate access rights.

In the following steps, a trainee for stock management is defined who belongs to the Users group, with limited rights.

---
*A+W Business Master data, B-462*

#### How to enter a user

1. Go to menu Master data > Company > Employees.
   Dialog Employees appears.
2. Go to the menu Start > New to switch to the input mode.

*Fig. B-245 Fields for new employee data are accessible*
- **A** Real name
- **B** Domain
- **C** Login name

⇨ Software Reference, "Employees - Employees" on page B-1031
3. Enter the data in section Identification:
   - **Name (plain)(A):**
     Employee's name, preferable the last name. Once saved, cannot be changed.
     The real name is saved with every action the user performs in A+W Business. The real name appears on selection lists, e.g. at order entry.
   - **Domain (B):**
     Name of the domain if the computer in installed in a network.
   - **Login name (C):**
     Name the employee uses to log into the system.
   The other fields are not mandatory. For external users, communication data may be useful for instance.
4. Go to tab Specification.

---
*A+W Business Master data, B-463*

*Fig. B-246 Specific settings for calling A+W Business*
- **A** Client for which the user is working
- **B** Restricting the document input
- **C** Password
- **D** Locking a user
- **E** User group
- **F** Language

5. Check the checkbox (B) if the user may only enter documents for a certain client.
   The combo box (A) for selecting the client is accessible.
   If this checkbox is not checked, the user can enter documents for all clients.
6. Choose the client if required.
7. Enter the password (C) the employee has to use for identification.
   The user can change this password when he logs into A+W Business.
8. Select the group (E) to which the employee shall belong.
   When he is allocated to the group, the user will gets all rights granted to this group. These can be modified as required.
   ⇨ Tutorial 1, "How to edit user rights" on page B-471
9. Select the language (F).
   This setting only refers to the language of the main menu.
10. Select the printer and the fax.
    All necessary data have been entered. If you save your entries now, the real name cannot be changed any more. You can immediately delete the employee's data however. Once he has logged into A+W Business he cannot be deleted.
11. Select in the menu Start > Save to save the data.

---
*A+W Business Master data, B-464*

The data will be saved. Tab Settings is accessible. You can add further data and amend the user rights now.

#### How to copy the standard settings for documents

1. Go to tab Settings and select the user whose settings you want to copy.
2. Go to tab Settings.

*Fig. B-247 Copy user settings*
- **A** Source
- **B** Copy the setting
- **C** Target user
- **D** List of employees

⇨ Software Reference, "Employees > Settings" on page B-1034
3. Go to combo box Target (C) and select the new user.
4. Click on [User settings] (B) to copy the settings.
   A safety query appears and allows checking the source and the target; these have to be acknowledged. After that, the settings will be transferred.
   You can amend these settings as required.
5. Select the new employee from the list (D).

---
*A+W Business Master data, B-465*

*Fig. B-248 Amend the user settings*
- **A** Adopted setting
- **B** Amend the settings.

The setting for the document type P.O. (A) was adopted. Please note that the settings in the individual columns can be amended only if the column General shows the entry <disabled>.

6. Choose the standard settings for the other document types and for the order areas (B).
   Click on a line to select the required data from the combo box.
7. Select in the menu Start > Save to save the data.
   The data will be saved.

> **Deletion of data**
> The user's data can be deleted before he logs into the program for the first time. To do this you have to enter your password for the system.
> If rights had already been allocated they have to be deleted first.

---
*A+W Business Master data, B-466*

#### Change Password

The password for logging into A+W Business can be changed by the corresponding user.

**How to change your password**
1. Click on the icon for starting A+W Business.
2. Check the checkbox Change password.
3. Enter your old password and your new password in the appropriate fields.
4. Enter the new password again in field Confirmation.
5. Click on [OK] to save the data.
   The password is changed; A+W Business is started. Next time you start A+W Business you have to untick the checkbox Change password.

---
*A+W Business Master data, B-467*

#### Locking of Users

User data cannot be deleted once the user has been working in A+W Business. You can block his access to A+W Business however.

> **Prerequisite**
> You can lock users only if you have system administrator's rights.

**How to lock a user**
1. Go to menu Master data > Company > Users.
   Dialog Employees appears.
2. Go to tab Employee and select the user to be locked.
3. Go to tab Specification.

*Fig. B-249 Locking a user*
- **A** Checkbox

⇨ Software Reference, "Employees - Specification" on page B-1033
4. Check the checkbox Locked (A).
   The user can no longer work in A+W Business and cannot be selected from the dialog combo boxes either.
5. Select in the menu Start > Save to save the data.
   The data will be saved.

---
*A+W Business Master data, B-468*

### Editing of User Rights

A user normally gets the same rights as the user group to which he belongs. These rights can be extended or restricted. If the user is allocated to another group he will automatically get this group's rights. You can complete these rights by copying the rights of another group so that the user is granted the rights of both groups.

> **Prerequisite**
> User rights are defined for a group or for a single employee. Rights can be allocated only if both the group and the user have been entered before. You can define user rights only if you have got system administrator's rights.

There are the following instructions on this subject.
- "How to complete user rights by copying" on page B-469
- "How to restrict user rights" on page B-473

The following steps describe how rights can be defined quickly and easily by means of the copy function.

#### How to complete user rights by copying

1. Go to menu Master data > Company > Employee rights.

*Fig. B-250 Define an employee's rights*

⇨ Software Reference, "Employee Rights" on page B-1037
2. Go to menu Functions > Copy rights.

---
*A+W Business Master data, B-469*

*Fig. B-251 Copy employees' rights*
- **A** Select the source
- **B** Define the target
- **C** Delete or keep existing rights

3. Choose the group in section Source (A).
   In this example, the rights of a group shall be transferred to an employee.
4. Choose the employee in section Target (B).
5. Decide whether the existing rights (C) shall be deleted or kept:
   - When you check the checkbox, all rights of the target will be deleted and replaced by the source's rights.
   - If you do not check this checkbox, only the rights that had not been granted before will be transferred.
   In this example, the existing rights are completed by the new rights: The checkbox is left unticked.

6. Click on [OK] to start copying.
   When this process is completed, a message pops up showing the number of rights that have been transferred.
7. Acknowledge the message and close dialog Copy rights.

---
*A+W Business Master data, B-470*

*Fig. B-252 Copied rights*

The rights of the new group or of the new user are listed in dialog Management of rights in section Overview. You can now edit the rights if required.

#### How to edit user rights

1. Go to menu Master data > Company > Employee rights.
   Dialog Management of rights appears.
2. Select the option Employee and choose an employee.
   The group and the employee appear on the list.

---
*A+W Business Master data, B-471*

*Fig. B-253 Editing of granted rights*
- **A** Staff
- **B** Granting or withdrawing of rights
- **C** Open the list

3. Open the list of existing rights by clicking on [+].
   The list shows all rights granted to the employee or group of employees. For all program items or dialogs that are not listed, unlimited rights apply.
4. Select the program item for which the rights shall be changed.
   The rights are shown in the checkboxes (B).
5. Go to section Rights and check the checkboxes (B) to restrict the right as required:
   - **Change:** Data can be edited.
   - **Insert:** New records can be entered.
   - **Delete:** Records can be deleted.
   - **Execute/read:** The dialog can be opened.
   Please note that when a checkbox is left unticked, the corresponding right will be withdrawn. If you check e. g. the checkbox Execute, the user can open the dialog in question but cannot edit it.
6. Go to the menu Start > Save to save the changes.
   The new rights for the user will be saved and come into force next time he logs into A+W Business.

---
*A+W Business Master data, B-472*

#### How to restrict user rights

1. Go to menu Master data > Company > Employee rights.
   Dialog Management of rights appears.
   In the following steps, access to an additional program item is restricted for an employee.
2. Select menu Edit > New.

*Fig. B-254 Fields for allocation of rights are accessible*
- **A** Staff
- **B** Program (dialog)

3. Select the user (A) whose rights shall be restricted.
4. Select the program (B) for which the rights shall be restricted, e. g. Crystal Reports output.
5. Go to section Rights and check the checkboxes to restrict the right as required.
   Please note that when a checkbox is left unticked, the corresponding right will be withdrawn. If you check e. g. the checkbox Execute, the user can open the dialog in question but cannot edit it.
   In this example, the user shall not be able to open the dialog. Therefore, no checkbox must be checked.
6. Select in the menu Start > Save to save the data.

---
*A+W Business Master data, B-473*

*Fig. B-255 Granting additional rights to the user*

The data will be saved. The user is listed in section Overview. In this example, no checkbox is checked. This means that the user cannot open this dialog any longer.

7. Select the user again to check all his rights.

*Fig. B-256 User's rights*

---
*A+W Business Master data, B-474*

In this example, the entry Crystal Reports output is the right which has been granted in addition to the group's rights.

#### How to delete an employee's rights

1. Go to menu Master data > Company > Employee rights.
   Dialog Management of rights appears.
2. Select the employee whose rights shall be deleted.
3. Select the right to be deleted.
4. Go to menu Start > Delete and confirm the query by [Yes].
   The selected right is deleted from the list. The list shows all rights allocated to the employee. For all program items or dialogs that are not listed, unlimited rights apply.

> **Delete all rights**
> To delete all rights please go to menu Functions > Delete rights. All of the employee's rights will be deleted. You can also delete new employees who have not logged into the system yet.

---
*A+W Business Master data, B-475*

### Exercises

- Enter a (training) client.
- Allocate a sales territory to an employee. Select yourself as a salesman for this exercise.
- Define a graduated commission for this salesman, based on the sales of your training customer and on training products.

You can perform the following exercises only if you have got administrator rights. Please remember to perform these exercises for your training client.
- Define a group for stockkeepers.
- Define the rights for this group so that they can only access the stock dialogs.
- Enter a new employee, e. g. a trainee for stock management.
- Give him the same rights as the rights for the stockkeeper group.
- Withdraw the right to enter stock purchase orders and to set up the inventory list.
- Log in with his login data and check in stock management whether the rights have been granted correctly.

**Additional information**
⇨ Software Reference, "Company Data" on page B-942
⇨ Software Reference, "Field Services" on page B-1041
⇨ Software Reference, "Commission" on page B-1043
⇨ Software Reference, "Banks" on page B-1045
⇨ Software Reference, "Subsidiaries" on page B-1047
⇨ Software Reference, "Employee" on page B-1031
⇨ Software Reference, "Employee Groups" on page B-1036
⇨ Software Reference, "Employee Rights" on page B-1037

---
*A+W Business Master data, B-476*

# Tutorial 2

BA+W Business Master data

---
*Page B-477*

**This section provides information on the following subjects:**
⇨ Documents
⇨ Settings for Invoicing
⇨ Printing of Text and Documents
⇨ Complex Exercise
⇨ Additional Information

| | Page |
| :--- | :--- |
| Documents | B-480 |
| Order for testing master data | B-481 |
| Interaction of master data in an order | B-482 |
| Enter new order | B-486 |
| Number Manager | B-489 |
| Exercises | B-491 |
| Status administration | B-492 |
| Handling of business processes | B-493 |
| Status point (process name and number) | B-494 |
| Status management | B-495 |
| Status allocation | B-496 |
| Status allocation | B-497 |
| Lock code | B-499 |
| Status allocation | B-499 |
| Allocation of lock codes | B-502 |
| Number areas | B-506 |
| The function of number ranges | B-507 |
| Production preparations | B-510 |
| Definition of number ranges | B-511 |
| Exercises | B-514 |
| Roundings | B-515 |
| Rounding | B-516 |
| Rounding points | B-518 |
| Rounding allocation | B-521 |
| Rounding for partners | B-522 |
| Rounding allocation | B-523 |
| Exercises | B-526 |
| Settings for Invoicing | B-527 |
| Finance | B-528 |
| Taxes | B-529 |
| Currencies | B-530 |
| Printing of Text and Documents | B-533 |
| Text | B-534 |
| Text types | B-535 |
| Text codes and standard text | B-536 |
| Variables | B-539 |
| File Attachment | B-542 |
| Text input | B-543 |

---
*A+W Business Master data, B-478*

| | Page |
| :--- | :--- |
| Forms | B-545 |
| Form management | B-546 |
| Printing prices | B-550 |
| Printing sketches | B-552 |
| Direct printing | B-557 |
| Print jobs | B-558 |
| Definition of direct printing | B-560 |
| Entering a Print Job | B-562 |
| Complex Exercise | B-566 |
| Additional Information | B-567 |
| Project/invoice management | B-568 |
| Versions of project-/invoice management | B-569 |
| Estimated quantities | B-569 |
| Project management settings | B-570 |
| Standard project management | B-572 |
| Enter an order for a standard project | B-573 |
| Extended project management | B-575 |
| Working with extended projects | B-575 |
| Invoice management with allocated orders | B-581 |
| Invoicing of blanket orders | B-582 |
| Available document types | B-592 |
| Available limit types | B-593 |
| Available system text | B-596 |
| Available variables (wildcards) | B-597 |
| General | B-597 |
| Processings: | B-598 |
| Spacer text | B-598 |
| Patterns for leaded designs | B-600 |
| Monitoring of changes | B-601 |
| A+W Production | B-604 |
| Transfer file | B-604 |
| Master data transfer from A+W Business to A+W Production | B-604 |
| Processing catalog | B-606 |
| Mixed calculation | B-607 |
| French pricing | B-608 |
| Calculation | B-609 |
| Marginal income limits | B-610 |
| Cost and surcharge calculation | B-613 |
| Definition of primary cost calculation | B-617 |
| Complex example: IG calculation | B-619 |
| Calculation of lites | B-620 |
| Spacer calculation | B-621 |
| Gas calculation | B-621 |
| Calculation of consumables | B-622 |

---
*A+W Business Master data, B-479*

## Documents

Documents are the basis of the commercial processes in A+W Business. This set of topics will tell you how to test new or amended master data and how the processing of documents is controlled in A+W Business.

This includes the following training modules:
- "Order for testing master data" on page B-481
- "Status administration" on page B-492
- "Number areas" on page B-506
- "Roundings" on page B-515

> **Prerequisite**
> This tutorial is based on the knowledge acquired in Tutorial 1.

---
*A+W Business Master data, B-480*

## Order for testing master data

### Objectives
- Checking the interaction of master data.
- Order entry.
- Setting up a number manager.

### Benefits
You can test the new or amended master data before using them in your daily business.

### Please note

| Term | Description |
| :--- | :--- |
| **Order** | An order (document) is always transferred to a number manager. |
| **Number manager** | Number managers (NM) help organizing the processes in your daily business. A NM cannot be empty. |
| **Hierarchy of terms** | Calculation or orders (or purchase orders) takes the terms into account in the following sequence: Details from the document, Definitions from master data, Group-specific terms. |

---
*A+W Business Master data, B-481*

### Interaction of master data in an order

You have entered or edited the data for partners, products, prices, surcharges, and discounts. These data are used in the documents and form the basis for order and P.O. entry.

*Fig. B-257 Interaction of master data in the order*

This simplified chart shows an order for a customer who orders a certain product. In addition to customer master data and product master data, further master data are integrated e. g. for pricing.

Before using the new data in your daily business you have to check whether the results of pricing and scheduling meet your expectations. The following chapters describe in brief how data are entered in dialog Document management.

For a complete description of order entry please refer to section Sales.

---
*A+W Business Master data, B-482*

### The order header

The header is valid for the whole order. It consists of those parts of the order that never or rarely change for the customer, e. g. customer number, invoicing address, terms. It also shows the totals per order.

*Fig. B-258 Document management dialog*
- **A** Document type and number of the document on hand
- **B** Tab for the header
- **C** Current number manager
- **D** Status (display enabled in table properties)
- **E** Tab for item data

This brief example shows an order with the header for customer and shipping data. Tab Items can be accessed only after the header has been saved.

---
*A+W Business Master data, B-483*

### Item data

Item data are the variable part of the document. Apart from products, prices, sizes, and quantities, they provide information for production and purchasing (purchase orders).

*Fig. B-259 Item entry dialog*
- **A** Title bar: Order number, number of items, total
- **B** Items
- **C** Item prices (red letters for manual input)
- **D** Item price
- **E** Details of BOM

This screenshot shows how order items are displayed. For every item, you can see the prices and discounts loaded from master data.

For a detailed description of the documents please refer to chapter Sales.
⇨ Sales, "Comprehensive Document Entry up to the Invoicing Stage" on page C-1142

---
*A+W Business Master data, B-484*

### Number manager for orders

Orders are organized in number managers (NM) so that they can be processed together. Every document is automatically allocated to a number manager. The number managers can be used for automating the sales processes, e.g. printing order confirmations and delivery notes.

*Fig. B-260 Number Manager*
- **A** Current NM
- **B** List of documents in the NM

Number managers cannot be empty. To check the master data, you have to enter an order first. It can then be moved to a new number manager.

The functions of the number managers are described in detail in section Sales.
⇨ Sales, "Number manager" on page C-1301

---
*A+W Business Master data, B-485*

### Enter new order

The following instructions show how to enter an order in which no fields are preset from a previous order.

Working with documents is described in detail in section Sales. This is why the individual steps are only described in brief at this point.
⇨ Sales, "Enter order header" on page C-1166
⇨ Sales, "Enter order item" on page C-1213

#### How to enter an order

1. Select menu Documents > Order > Order.
   The dialog Document management opens. If necessary, remove the presetting by clicking on [Select].
2. Go to the menu Start > New to switch to the input mode.

*Fig. B-261 Fields for new order are accessible*
- **A** Header
- **B** Input field Customer Number
- **C** Items tab

⇨ Software Reference, "Partner Management" on page B-808
3. Enter the number (B) of your (training) customer.

---
*A+W Business Master data, B-486*

If you do not know the customer number you can use the zoom function to search for the customer.

4. Use <Tab> to go to the next field.
   The customer data will be loaded.
5. Select in the menu Start > Save to save the data.
   The header data will be saved. The title bar (A) shows the order number, and tab Items is accessible.
6. Click on tab Items (C).

*Fig. B-262 Fields for the new item are accessible*
- **A** Enter the product number
- **B** Search product
- **C** Quantity
- **D** Width
- **E** Height

The input field (A) for the product number is accessible. Only if you have meanwhile saved the entries or changes you have to start the input mode in menu Edit > New to enter a new item.

7. Enter the number (A) of your (training) product in the input line.
   If you do not know the product number you can select the required product by means of the search (B) function.

---
*A+W Business Master data, B-487*

8. Use <Tab> to go to the next field.
   All input fields are enabled.
9. In the next fields, enter the quantity (C) and the sizes (D, E).
   If you enter just 1 piece and the sizes 1000 x 1000 you can easily check whether the prices are shown correctly.

*Fig. B-263 Price display*
- **A** Price list
- **B** Price keys
- **C** Price unit
- **D** Item price

10. Check whether the rate (price key (B), price list (A)) and the price unit (C) are shown correctly.
    If no surcharges or discounts are applied to your product, the item price (D) must be correct. In this example, this is 71.38 €/sqm x 1.04 sqm (rounded size).
    When surcharges and discounts have been applied, the item price can be calculated accordingly.
11. Save the item using <Enter>.
    Item data will be saved and suggested as a new item in the next line. You can change the data to enter another item or ignore the data if you do not want to enter further items.
    Make a note of the order number so that you can set up a number manager for this order afterwards.
12. First close item entry, then the order.
    Set up a new number manager in which all orders entered for test purposes are going to be gathered.

---
*A+W Business Master data, B-488*

### Number Manager

You should set up a special number manager (NM) for testing master data. We are going to explain the necessary steps only in brief. The use of the number manager is described in detail in section Sales.
⇨ Sales, "Number manager" on page C-1301

#### How to create a new number manager

1. Select menu Documents > Order > NM order.
   The Number manager dialog opens. The list shows all documents included in the active number manager.
2. Go to the menu Start > New to switch to the input mode.

*Fig. B-264 Fields for new number manager are enabled*
- **A** Name of the number manager
- **B** Order number

3. Enter the name (A) of the new number manager, e.g. training.
4. Enter the number of your test order in both fields (B).
   If you do not know the number you can search for the order by restricting the selection to status 1. In this case, all orders with status 1 will be loaded into the number manager. You can however de-

---
*A+W Business Master data, B-489*

lete the unwanted orders from the number manager by selecting them and pressing <Del>.
5. Select in the menu Start > Save to save the data.
   The data will be saved. The new number manager appears in field Selection.

*Fig. B-265 New number manager*

The allocated order appears on the list.

---
*A+W Business Master data, B-490*

### Exercises

- Enter different orders - including your training products - for your training customer.
  - Just enter one piece with a size of 1000 x 1000 mm so that you can easily check the calculation of the item price.
- Check the following data:
  - Have surcharges and discounts been calculated?
  - Is marginal income and cost calculation displayed?
  - Are the route and the delivery date correct?

---
*A+W Business Master data, B-491*

## Status administration

### Objectives
- Introducing the function of the status.
- Knowing the difference between status point and user status.
- Checking the status allocation.
- Define the change of status, lock status, and status diversion.

### Benefits
- Status allocation serves to describe the business processes.
- Status allocations define how a document can be edited after it has been entered.

### Please note

| Term | Description |
| :--- | :--- |
| **Status point** | Program point which marks the end of a process. The individual statuses are fixed and cannot be changed. |
| **User status** | State of processing the document has reached in your company. The numbers and names are set up during program installation. |
| **Status allocation** | Every user status must be allocated to a status point. If this allocation is missing, certain functions cannot be executed. |
| **Status** | Number which marks the document's position in the program flow. Each status is unique. Every document is marked by a status. |
| **Change of status** | The status is automatically changed at the end of the program process. The status is always raised. Special user rights are required to reset the status by hand. |
| **Document type** | Not every status can be applied to every document, e. g. all documents have the status Document entered at one time or another but a quotation can never reach the status Delivery note printed. |
| **Manual status point** | Manual status points can only be allocated manually. It overrules the automatic raising of the status. |

---
*A+W Business Master data, B-492*

### Handling of business processes

Your business processes determine the stations an order passes between order entry and archiving.

**Example**
- An order is entered.
- The order is changed.
- The order confirmation is printed.
- Orders are transferred to capacity planning (optional).
- Orders are transferred to production.
- The production status is reported.
- Delivery note is printed.
- The invoice is printed.
- Order is transferred to financial accounting.
- Order is transferred to statistics and archives.
- Order data are deleted from the main database.

From order entry to archiving, the order passes defined program points, the so-called status points. These status points can be allocated to the stations your order passes in your company. You define the minimum status, i.e. the requirements that have been met so that the order can be passed on. You can also define when an order shall be locked for certain processes.

These connections are defined in the dialogs Status management, Status points, and Status allocation.

> **Editing of dialogs**
> Dialogs Status management and Status points do not require editing. You only have to be able to edit the status allocation, e. g. if business processes are changed.

---
*A+W Business Master data, B-493*

### Status point (process name and number)

The so-called status points are defined in the program for the automatic processing of documents. They signal the end of various, internal processes a document passes from input up to the printing of an invoice, including complaints or credit notes.

*Fig. B-266 Status points*
- **A** Internal code (status point ID)
- **B** Document type
- **C** Completed process

The status points are fixed in the system and are used to define conditions for further processing, e.g. for printing invoices. Every status point can be allocated to a user status per document type (B).

The user status shows the actual processing status of the document. This connection is described below.
⇨ "Status management" on page B-495
⇨ "Status allocation" on page B-496

Not every status can be applied to every document, e. g. all documents have the status Document entered at one time or another but a quotation can never reach the status Delivery note printed.

The following document types are available:
- 0 = all documents
- 1 = quotations
- 2 = order
- 3 = credit note
- 4 = inquiry
- 5 = P.O.

---
*A+W Business Master data, B-494*

### Status management

The so-called user status marks the state of processing a document has reached within your company's processes.

*Fig. B-267 Status management (user status)*
- **A** Status: Code in the documents
- **B** Description (in the business process)

The document status shows the whereabouts of the document in the business process. It is shown as a number with the corresponding description, e.g. at order entry or in the history.

> **Change of user status**
> Before entering or changing a user status, please discuss the matter with A+W Software GmbH. This will help to avoid system errors or incompatibilities.

---
*A+W Business Master data, B-495*

### Status allocation

Every status point can be allocated its own user status. The numbering of status points has nothing to do with the sequence of the company's workflow.

*Fig. B-268 Allocation: status point – user status*
- **A** Status points
- **B** Selected status point
- **C** Document type to which the allocation applies
- **D** Allocated user status
- **E** Minimum status the document must have reached
- **F** Lock status

In this example, status point Print invoice (B) is allocated to user status Invoice printed (D). This allocation applies to the document type Order (C). This means that when the invoice has been printed, the status of the order is shown together with the status number and status name of the user status.

#### Minimum status

For every allocation you can define the minimum status a document has to have to reach the selected status point. In this example, the minimum status (E) is the printing of delivery notes. This means that the invoice cannot be printed before the delivery note.

---
*A+W Business Master data, B-496*

### Lock status

For every allocation you can enter a lock status (F) to control the further process. In this example, the same user status (D) is defined which means that the invoice cannot be printed again as an original invoice.

In addition to the lock status, a lock code can be set for complaints and partial shipments.
⇨ "Lock code" on page B-499

### Status allocation

The status is automatically raised when the document has reached a certain status point, and if the corresponding action has been triggered.

*Tab. B-20 Examples of status allocations*

| User status | Document type | Min.-status | Lock status | Status point - Process name | Status point - No. |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 001 Enter document | All | - | - | Document entered | 001 |
| 020 Document changed | All | 001 | 750 | Document changed | 002 |
| 200 Confirmation printed | Order | 001 | 200 | Print OC | 100 |
| 300 Transfer order to purchasing | Order | 180 | 540 | Transfer to order pool | 030 |
| 390 Order released for production | Order | 001 | 390 | Production release | 035 |
| 360 Receipt of goods - complete/order | Order | 030 | 360 | Receipt of goods - complete/order | 034 |
| 450 Order transferred to production | Order | 400 | - | Transfer to production | 045 |
| 600 Delivery note printed | Order | 400 | 600 | Print delivery note | 102 |
| 750 Invoice printed | Order | 600 | 750 | Print invoice | 103 |
| 800 Transfer FinAcc data | All | 750 | 800 | Transfer to FinAcc | 097 |
| 850 Transfer to statistics | All | 800 | 850 | Transfer to statistics | 500 |
| 990 Transfer to Archives | All | 850 | 900 | Transfer to archives | 501 |
| 990 Release deletion | All | 900 | 990 | Release deletion | 502 |
| 995 Document deleted | All | 990 | - | Document deleted | 503 |

This example shows how the status of an order is changed by processing. The minimum status for transfer to purchasing is that the corresponding work order has been printed. The lock status defines that the document is locked after production and cannot be transferred again. The first column shows the sequence in which the document passes the individual processing steps.

---
*A+W Business Master data, B-497*

#### Manual status allocation

You can define that the status for special processes must be allocated by hand. A manual status point must be defined in this case. A manual status point can be allocated only by hand in a document. It overrules the automatic raising of the status.

**Example**
A manual status point is set e.g. if an invoice is to be printed only after a (manual) check. The status of an order has to be raised manually after the check so that the invoice can be printed.

Manual status allocation requires the following steps:
- Enter a new status point with a number >10,000.
- Define the user status in the business process.
- Allocate the user status to the status point.

> **Definition of status points**
> If you want to define and allocate new status points you should ask a member of the A+W Software GmbH service team for help. This will help to prevent inadvertent status changes for your documents.

#### Status allocation based on barcode reports

Special status points have to be defined also for reports from shop floor data collection (barcoding). In contrast to manual status points, the document status will be changed automatically when a report from the shop floor is received.

Status allocation based on barcode reports requires the same steps as manual status points. Moreover, the registration points have to be allocated.

Status changes based on barcode reports are described in section Production.

---
*A+W Business Master data, B-498*

### Lock code

Lock codes can be used to lock documents for certain actions while automatically raising their status. This means that the document cannot reach the locked status but is instead diverted to another status point (process).

**Example: Partial shipment without invoicing**
If no partial invoice is to be issued for a partial shipment, the status of the partial shipment is raised automatically. If the order is diverted to transfer to archives, the partial shipment cannot be edited any further.

*Fig. B-269 Lock code and diversion to another status*
- **A** Name of the lock code
- **B** Locking the lock code
- **C** Locked status (user status)
- **D** Next possible status

Locking makes sense e.g. for partial shipments, namely if the partial shipments are not to be invoiced. The lock code for partial shipments (and for complaints) is enabled in company data.
⇨ Software Reference, "Company Data > Documents" on page B-952

> **Locking the lock code**
> Do not mix up the lock code and the lock based on the checkbox Locked (B). The lock code diverts a document to another status. The checkbox Locked prevents the use of the lock code.

### Status allocation

Dialog Status allocation serves to allocate status point and user status. There are no limits for defining status, minimum status, and lock status.

---
*A+W Business Master data, B-499*

> **Discuss required changes**
> Please discuss all changes of status management and status allocation with A+W Software GmbH beforehand. This will help to avoid system errors or incompatibilities.

#### How to allocate a status point

1. Select menu Master data > Order > Status allocation.

*Fig. B-270 Status allocations*

⇨ Software reference, "Status Allocation" on page B-915
2. Go to the menu Start > New to switch to the input mode.

---
*A+W Business Master data, B-500*
