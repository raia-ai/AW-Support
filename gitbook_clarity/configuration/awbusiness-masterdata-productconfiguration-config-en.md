---
description: "EN_AWBusiness_Master_Data_9_7-3"
---


# Software Reference

---
## Products

> **i Adapt field names**
> The following field names can be adapted to your company's requirements in dialog System text (system text no. 111–118).
> ⇨ "System Text" on page B-1041

**Ug value in W/sqm Thermal transmission coefficient**
The Ug value is the central unit of measure during determination of the heat loss of a construction element. The unit of measure is W/sqm. K. The smaller the Ug value, the higher the thermal insulation.

**g value in % Total energy transmission in %**
The value is composed of the direct transmission of solar energy and of the secondary heat emission to the inside due to long wave radiation and convection.
The g value is the secondary parameter after the k value.

**b factor Average transmission factor**
Represents the average transmission factor for solar energy referring to the total energy transmission ratio of a 4 mm lite. This is necessary for calculating the cooling load of a building.

### Table (overview)
List of records for IG structures. The fields in section Glass Structure will be filled when you select a record.

## Processing Restrictions
*Master Data > Products > Product > Processing Restrictions*

This dialog is used for defining the rules that will apply to processing steps for certain product classes.

If these restrictions are not met at order entry, the system will issue a message to which the user must react appropriately.

### Allocation

**Product class**
Restrictions usually apply to the processing of toughened and laminated glass lites. You can also choose other product groups however.

**Thickness**
Glass thickness for which the restriction is valid. If different restrictions are valid for a product class depending on the glass thickness, you have to define a suitable rule for every thickness.

**Rule**
The rules have been defined with variables the values of which are loaded from the parameter fields.
[p1], [p2] to [p5] apply to parameters 1 to 5.

**Parameters 1–5**
Fields for the values that are inserted in the rule by means of the variable. The fields are released according to the selected rule. If a rule without variables has been selected, no field are accessible, e. g. for rule 201 - Remaining edge >= depth of cut-out.

**Level**
Choose an option to specify the reaction of A+W Business to a violation of restrictions:
- **Info:** Just one bit of information will be displayed at order entry.
- **Warning:** A warning appears at item entry. The user should change the processing details or the glass.
- **Error:** An error report appears at item entry. Neither processing nor item can be saved. The user must change the processing details or the glass.

### Restrictions
List of defined restrictions including parameters.

## Patterns
*Master Data > Products > Product > Patterns*

On this dialog, you specify patterns for coatings, silk screens, sandblasting, enameling, coloring, and frosting. You can insert the specified patterns in the order in the order entry on the Shapes/Processings tab using the silk screen number.

⇨ "Coating, frosting, screen printing, area enameling, sandblasting, coloring" on page C-476

### Pattern

**Silk screen**
Number of the silk screen.

**Name**
Name of the pattern. It should be clear and meaningful.

**File**
Path and name of the pattern file. A preview of the pattern is displayed in the frame in the right top corner of the dialog.

**Max. dimensions**
Specification of the maximum width and height of the silk screen in mm. You can adjust the width and height of the pattern in the order in the item entry on the Shapes/Processings tab up to the specified maximum value.

### Table
Overview of the defined patterns with the stored parameters.

## Shape Edge Qualities
*Master Data > Products > Product > Shape Edge Qualities*

On this dialog, you assign the individual edges of the various shapes particular edge qualities.

### Selection

**Product**
Number and name of the processing type.

**Shape**
Number of the shape whose edges should be processed. Standard shapes use the shape no. 1-99, the shape for stepped insulated glass has the number 999.

### Edge qualities

**Segment 1-8**
Specification of the edge quality per shape segment. The fields are released depending on the shape's number of edges. The associated numbering of the segments is displayed in the graphic with the red figures.

### Table
Overview of the defined shapes with the stored parameters.

## Fitting Allocation
*Master Data > Products > Product > Fitting Allocation*

On this dialog, you specify the processings that are required for mounting fittings (hardware) on a glass lite. If a fitting in the order is inserted into the BOM in the item entry, associated processings and processing parameters are taken over into the BOM. If the fitting is deleted or changed in the order from the BOM, the associated processings are also deleted or changed.

### Identification

**Fitting**
Number and name of the fitting.

**Mounting**
Mounting type of the fitting.

**Mounting priority**
Sequence in which fittings with the same product number should be mounted. If fittings are inserted several times in the BOM in the order in the item entry, the fitting assignments are arranged by priority, e.g. hinge top with the priority number 1 is displayed in the first position, hinge middle with the number 2 in the second position, etc.

**Hinge side**
Side on which the hinge should be mounted. You can choose between Left, Right, and Both.
- **Left:** The hinge will be mounted on the left.
- **Right:** The hinge will be mounted on the right.
- **Both:** The hinge can be mounted on both sides.

**Processing**
Display of the processing type. In the Parameters field, you can change the processing parameters.

**Exchange**
Exchange fitting that can be specified optionally. Fittings can be selected as exchange fittings that have different product numbers for another hinge side. The name of the exchange fitting is displayed automatically after entry of the product number.

### Processings
With the [Insert] button, you can add processings to the glass lite that are required for the mounting of the selected fitting. In the Parameters field you can adjust the associated processing parameters. With the [Delete] button, you can remove processings.

### Parameters
The fields displayed may differ, depending on the selected processing.
The parameters are described in detail in the Sales section.
⇨ Sales, "Parameters" on page C-467

> **i Formulas instead of values**
> You can also enter formulas instead of values in the processing parameters.
> 
> **Example**
> For example, for a handle in the parameters Drilling 1 [x/y], Drilling 2 [x/y], you can also enter formulas.
> If you want to use formulas, please contact your service employee at A+W Software GmbH.

### Hardware parts
The overview displays all created fittings that correspond to the search criteria.

## iTOE Rules
*Master Data > Products > Product > iTOE Rules*

On this dialog, you create the rules for the import of SN files with processings (TOE = Technical Order Entry). Each processing from the A+W CAD Designer must be assigned the appropriate processing in A+W Business.

> **i Requirements**
> The TOE module, which requires a license, assumes the database system Microsoft SQL Server 2016. Contact A+W Software GmbH if you want to use the module.

### SN processing
In this area, you select the processing that are defined in A+W CAD Designer. Additional fields are displayed per selected processing in order to make the assignments more precise. For a detailed description of the parameters, see the Sales section on item entry.
⇨ Sales, "Items - Processing" on page C-466

**Processing type**
Number and description of the processing type from A+W CAD Designer.

**Priority**
If you create several assignments for a processing type, you must specify with which priority the system should evaluate the details.

**to product type**
The rule can be restricted to one product type.
- The rule for the selected processing can be applied to all product types.
- The rule should only apply if the selected processing is applied to a particular product.
The field for selecting the products stored in A+W CAD Designer is activated.

**Formula**
The rule can be restricted to a processing that is calculated with a formula.
- The rule applies for the selected processing.
- The rule only applies for the selected processing if the processing is calculated with a formula.
The field for selecting the formulas stored in A+W CAD Designer is activated.

**Edge quality**
The rule can be restricted to on processing if different edge qualities can be generated.
- The selected processing does not refer to different edge qualities.
- The rule only applies for the selected processing if the processing generates a particular edge quality.
The field for selecting the edge qualities stored in A+W CAD Designer is activated.

### Will become Product

**Product**
Number and description of the processing in A+W Business that is assigned.

### Rules
The defined rules are displayed in the overview.

## Prices
*Master Data > Prices*

Price lists, discounts, surcharges and reductions are available for the pricing of an order. This section describes the dialogs on the price lists and on surcharges and reductions.

Discounts are described in section Business partners.
⇨ "Discount Management (Customers, Suppliers)" on page B-803

> **i Sequence of dialog descriptions**
> The dialog descriptions in this chapter do not entirely match the sequence of dialogs in the software. For reasons of legibility, pricing is described in a separate chapter.

Menu Prices offers the following dialogs:
- "Price List" on page B-660
- "Price Keys" on page B-661
- "Rates" on page B-662
- "Price Management" on page B-710
- "Miscellaneous Surcharges" on page B-664
- "Exchange Surcharges" on page B-666
- "Price Groups" on page B-684
- "Price Group Allocation" on page B-685
- "Group Surcharges" on page B-687
- "Mixed Price Calculation" on page B-696
- "Shape Processing Surcharges" on page B-697
- "Price and Quantity Unit" on page B-700
- "Insurance Prices" on page B-702
- "Price Elements of Grills" on page B-709

## Price List
*Master Data > Prices > Price Lists*

This dialog is used for entering the price lists. The annual price list is actually a collection of different price lists. In A+W Business pricing, the price lists are combined with price keys to create fixed rates.

⇨ Tutorial 1, "Price List" on page B-222
⇨ “Rates" on page B-662

Check the checkbox (Std) to define the price list that should be used as the standard price list for automatic pricing. These settings are adopted for the rates.

**Std SLS**
The columns IG, SA, Proc., and Shape apply to sales.

**Std. PCH**
The columns PCH, Proc., and Shape apply to purchasing.

**From, to**
Space of time for which the price list should be valid. These details do not affect the availability of the individual price list.

**Locked**
A price list can be locked for input in product management and in documents if it is no longer required.
- The price list can be assigned.
- The price list is locked and cannot be assigned. If it has been allocated to products and in documents already, it will still be shown however.

**Comment**
Comments, e.g. peculiarities of the price list.

## Price Keys
*Master Data > Prices > Price Keys*

This dialog is used for entering the price keys. A price key is always linked to a price list, which it subdivides.

The combination of a price key and one or more price lists produces the rates used for pricing.

⇨ Tutorial 1, "Price key" on page B-222
⇨ "Rates" on page B-662

**Locked**
A price key can be locked for input in product management and in documents if it is no longer required.
- The price key can be assigned.
- The price key is locked and cannot be assigned. If it has been allocated to products and in documents already, it will still be shown however.

## Rates
*Master Data > Prices > Rates*

This dialog is used for defining the rates, each consisting of a combination of price key and a price list. This combination is adopted for order and P.O. input (sales, purchasing) where it can be changed if required.

You have to define the rates before you can enter the prices in price management.

⇨ Tutorial 1, "Definition of Rates" on page B-223

### Price list
This section shows the price list that has been defined as the standard price list for the year in question. Even the price list <n.e.> can be used in combinations. It can also be used for defining prices.

### Price Keys
This section shows the defined price keys. Even the price key <n.e.> can be used in combinations.

### Rate allocation
Here you can combine the annual price list and the price key to define a rate.
The price list defines the price list to be used for standard pricing, e.g. the same price list for all sales prices (SLS) and purchase prices (PCH).

As for the rate, you can define e.g. that Price list 07 and price key Works 06 is valid for IG sales while for single annealed sales, Price list 07 and the price key Fixed size applies.

> **i Only defined rates can be used for pricing**
> Please note that you have to define a rate for every price list/price key combination to be used for sales or purchasing. This rate must be defined even if it is not going to be used as the standard rate.

The checked checkboxes show the rates that are to be used by default for sales and purchase price calculation.

**Basic IG table**
A+W Business calculates the IG prices by default based on an IG matrix for each of the standard structures, e. g. for IG with 2 x float 4 mm, 2 x float 6 mm, 2 x float 8 mm.

If you base the prices on a single matrix, using proportional surcharges and discounts for the different thicknesses and replacement lites, you have to create a new, so-called basic IG table. For every rate, enter the number of this basic IG table so that the prices can be calculated acc. to this pattern.

**Production cost calculation**
When working with the production cost calculation module you have to specify which of the rates will be used for calculating the production costs.
- The rate will not be used for cost calculation.
- The rate is used for production cost calculation.

## Miscellaneous Surcharges
*Master Data > Prices > Miscellaneous surcharges*

This dialog is used for entering and editing size surcharges. These surcharges depend on the length, the surface, the weight, the airspace, etc. You can use two limit types for the graduation.

⇨ Tutorial 1, "Surcharges" on page B-266
⇨ Tutorial 1, "Defining a Miscellaneous Surcharge" on page B-318

> **i Please stick to the sequence of surcharge levels**
> A new step is always added after the last step. The sequence of steps will not be changed or analyzed at pricing. This means that the limit of 1200 mm will not be taken into account if it has been entered after the limit 1800 mm. The same surcharge will be applied to all sizes below 1800 mm in this case.

In the surcharge calculation, the sequence is only validated within the same surcharge unit. The sequence of steps is essential and will be considered if a surcharge unit, e.g. gross%, is valid for different limit types, e.g. smallest edge length or longest edge length.

- Surcharges for elements of the BOM are calculated before those surcharges that affect the item. This applies also reciprocally: surcharges on the item are calculated before those surcharges that apply to the item out of BOM elements.
- Surcharges per sqm, linear m and piece are calculated before gross/net% surcharges. Here it is decisive what they affect: the price per price unit, the gross price or the net price.

Here, the surcharge type must also be considered. In case of non-additional calculation, the previous surcharge will not be taken into account for calculating the next surcharge.

**Example**
| | Basic price 100.00 € | |
| :--- | :--- | :--- |
| | **additional** | **non-additional** |
| Shape surcharge + 20% | + 20,00 € | + 20,00 € |
| **Sub-total** | **= 120,00 €** | |
| Coating + 25% | + 30,00 € | + 25,00 € |
| **Total** | **= 150,00 €** | **= 145,00 €** |

### Surcharge tab
This tab shows the graduations for the surcharge selected on tab Table.

#### Surcharge for

**Number**
Surcharge table number.

**Name**
Surcharge table name.

**Limit type 1, 2**
Limit types can be used for surcharge graduation. The limit type defines the measure for graduation. You can choose different measures for the two limit types, e.g. height and width.

**Up to limit 1, 2**
Graduation value. The limit value refers to the limit type. If <n.e.> is entered as a limit type, the surcharge applies per price unit.

**OR**
If you want to use two different limit types for the graduation you have to define whether these should be analyzed together or alternately.
- Both limits and limit types will be taken into account for surcharge calculation.
- Only one of the two limits/limit types will be taken into account.

> **Example**
> In price management you have set up a matrix for a patterned glass where height and width must not be mixed up.
> For calculating a surcharge on the edge length it does not matter whether height or width reach the limit.
> Enter the level 1200 for limit 1 and 2.
> Select Height as limit type 1 and Width as limit type 2.
> - When you check the checkbox OR, the edge that reaches the 1200 mm step first will be taken into account.
> - If you do not check the checkbox, the surcharge will be applied only if both edges reach at least a length of 1200 mm.

**Surcharge, unit**
Amount and unit of the surcharge, e.g. 2.5% of the gross price.

**Surcharge type**
The surcharge type defines the basis for calculating the surcharge.
⇨ Tutorial 1, "Calculation by surcharge type" on page B-311

**Valid for price definition**
The price can be changed by hand in the order. The surcharge can be calculated if required. The setting applies to all orders and cannot be changed in the actual order.
- The surcharge will not be calculated if the price is changed by hand in the order.
- The surcharge will be calculated always.

### Tab Table
The table shows all miscellaneous surcharges matching the selection criteria.

## Exchange Surcharges
*Master Data > Prices > Exchange Surcharges*

Exchange surcharges are not based on groups and refer to the lites that should not or cannot be combined in groups. Product by product, you can define the surcharge to be added if a lite is exchanged in an IG unit or laminated glass.

Dialog Exchange Surcharges offers the following tabs:
- Exchange Surcharges - Table
- Exchange Surcharges - General, by Thickness, by Product
- Exchange Surcharges – Customer-, Supplier Prices
⇨ Tutorial 1, "Replacement Surcharges" on page B-287

### Functions menu
*Master Data > Prices > Exchange surcharges > Functions menu*

This menu allows to open other dialogs without closing dialog Exchange Surcharges.

#### Copy group
- **General:** Opens the dialog Copy exchange prices in general for copying the prices for exchange lites.
⇨ "Copy Exchange Prices" on page B-673
- **All per exchange article:** Opens the dialog Copy all exchange prices to copy the prices for the lites to be replaced.
⇨ "Copy Prices per Exchange Product Completely" on page B-677

#### Delete group
- **Delete price:** Opens the dialog Delete exchange prices to dele an exchange surcharge.
⇨ "Delete Exchange Surcharges" on page B-680

#### Change group
- **Change price:** Opens the dialog Change prices to change an exchange surcharge.
⇨ "Change Exchange Prices" on page B-681

## Exchange Surcharges - Table
*Master Data > Prices > Exchange Surcharges > Table tab*

Use this tab to check the defined exchange surcharges.
⇨ Tutorial 1, "Replacement Surcharges" on page B-287
⇨ Tutorial 1, "Defining an Exchange Surcharge" on page B-291

### Identification - Rate

**Table**
Just one table (no. 0) is usually created. If you create different tables for exchange surcharges you can allocate them in product master data.
⇨ "Exchange surcharge table" on page B-603

**Price list, key**
Price list and key (sales rate) allocated to the exchange surcharge.

**IG, LG**
Product type to which the surcharge is applied. lites can be exchanged only in IG unit or laminated glass. It does not matter which of the lites is exchanged, e.g. if it is the second or third lite of a triple IG unit.

### Product

**Replacement**
BOM element to be added.

**Exchange**
BOM element to be removed, i.e. that is going to be replaced by another element.
This field appears only for general and product-related exchange surcharges.

**Exchange thickness**
Thickness of the BOM element to be replaced by another element. It does not matter which product type or product group this glass belongs to.
This field appears for thickness-related exchange surcharges.

### Exchange prices
The surcharge can be graduated into maximally three levels. The limit types for the product are preset on tab General.

The limits of the highest level are automatically adopted from the fields of the second level. This means that only the surcharge value can be entered. This will be calculated whenever the lite is larger than the second level.

**Surcharge**
Surcharge per level. Depending on the surcharge type, this value will be interpreted as a proportional surcharge or as an amount.
⇨ "Surcharge types" on page B-670

### Exchange table
This table lists all surcharges matching the defined criteria.
- **Product number:** Product number of the exchange product, e.g. glass, cast resin.
- **Replacement:** Number and name of the new product.
- **Exchanged:** Description of the article to be replaced, i.e. product or thickness.
- **Tab.:** Number of the exchange table, usually 0.
- **Key:** Price key assigned to this surcharge.
- **Rate:** Price list assigned to this surcharge.

## Exchange Surcharges - General, by Thickness, by Product
*Master Data > Prices > Exchange Surcharges > General tab, by Thickness, by Product*

The tabs General, by thickness, and by product are used to enter the exchange surcharges for IG units and laminated glass. The surcharges always refer to sales prices (SLS).

⇨ Tutorial 1, "Replacement Surcharges" on page B-287

The fields in sections Identification - Rate, Product, and Exchange prices are described in connection with the tab Table.
⇨ "Exchange Surcharges - Table" on page B-668

### Surcharge types
The surcharge type defines how the entry in field Surcharge is to be interpreted, e. g. as a proportional surcharge on the price, as an amount per length, etc.

### Miscellaneous surcharges
**Number, Table**
You can define a Miscellaneous surcharge in addition to the exchange surcharge, e.g. for cutting. Miscellaneous surcharges are entered in the dialog of the same name:
⇨ "Miscellaneous Surcharges" on page B-664

### Limit type
Choose an option to define the limit types to be used in section Exchange prices.
- **Width x height:** The limit types Width and Height are displayed.
- **Surface (real):** The limit type sqm (square meters) is shown. Calculation will be based on the quantity entered for the order.
- **Edge size:** The limit type Edge is displayed.
- **Surface (rnd):** The limit type sqm (square meters) is displayed. For calculating the surface, the rounded values from the order and from product data will be used; in Germany, this is mostly 30.
⇨ "Size rounding width/height" on page B-604

### Diff. size rounding
You can enter a different size rounding for calculating the surface.

**Width, height**
0 is entered here by default. With this setting, the entries will be adopted from product data.

### Minimum values
You can enter the minimum values for calculating the surcharge. These will be used whenever the values defined in the order are lower.

**Min. sqft**
If you enter a minimum surface for an exchanged lite, this surface will always be used as a basis for surcharge calculation if the actual order surface is smaller.

**Gross price, Net price**
If you enter a minimum price, it will be used as a basis for surcharge calculation whenever the actual price of the exchange product is lower.

## Exchange Surcharges – Customer-, Supplier Prices
*Master Data > Prices > Exchange Surcharges > Customer prices, Supplier prices tab*

The tabs Customer prices and Supplier prices are used to define the exchange surcharges to be calculated for certain customers or suppliers.

⇨ Tutorial 1, "Replacement Surcharges" on page B-287

The fields in section Identification - Rate are described in connection with the tab Table.
⇨ "Exchange Surcharges - Table" on page B-668

### Select customers/customer groups, suppliers/supplier groups
Choose an option to define where the surcharge should be applied:
- **General:** General surcharge, calculated irrespective of business partners or partner groups (standard exchange surcharge).
- **Customer group, Supplier group:** Surcharge for the selected group of customers or suppliers
- **Customer, supplier:** Surcharge for the selected customer or supplier

### Select project
The surcharge can refer to a certain project. All projects will be offered for selection.

### List by customer/customer group, supplier/supplier group
This list shows all surcharges matching the defined criteria.

## Selection – Exchange Surcharge
*Master Data > Prices > Exchange Surcharges > Edit menu > New*

Select the type of surcharge to be defined.

## Copy Exchange Prices
*Master Data > Prices > Exchange Surcharges > Functions menu > group Copy > General*

You can copy or change one or more exchange surcharges for the replacement lites.

This dialog offers the following tabs:
- "Copy Exchange Prices – Source, Target" on page B-674
- "Copy Exchange Prices – Price Change" on page B-676

## Copy Exchange Prices – Source, Target
*Master Data > Prices > Exchange surcharges > Functions menu > group Copy > General > Source tab*

The tabs are used for copying the surcharges from one table to another table or to another rate. Only those exchange surcharges will be copied that will be charged for replacement lites.

⇨ Tutorial 1, "Copying and Changing Replacement Surcharges" on page B-296

If you only want to change the surcharges, enter the same table for the source and target. You can enter the amended values on tab Change prices.

⇨ "Copy Exchange Prices - Price Change" on page B-676

### Copy from, Copy to

**Table**
Number of the exchange table.

**Replacement number**
Numbers of the products replacing others.

**Price list, key**
Price list and key (rate) allocated to the exchange surcharge.

**IG, LG, Both**
Product type to which the surcharge is applied. Lites can be exchanged only in IG unit or laminated glass. It does not matter which of the lites is exchanged, e.g. if it is the second or third lite of a triple IG unit.
Select the option Both if exchange prices for IG and laminated glass are to be copied.

**Change prices**
To transfer the surcharges to a filled-in table you have to decide whether the surcharges in the target table should be changed.
- The surcharges in the target table will not be changed. The additional surcharges from the source table will be added.
- All existing surcharges in the target table will be changed.

**Price type**
Choose an option to specify where the surcharges should be applied:
- **General:** General surcharge, calculated irrespective of business partners or partner groups (standard exchange surcharge).
- **Customer group, Supplier group:** Surcharge for the selected group of customers or suppliers
- **Customer, supplier:** Surcharge for the selected customer or supplier

**Project**
This field is locked if you have selected the option General. When you select a group or a partner, you can also define the project for which the surcharge table should be changed.
