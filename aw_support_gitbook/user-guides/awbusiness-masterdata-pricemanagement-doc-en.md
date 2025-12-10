---
description: "EN_AWBusiness_Master_Data_9_8-1"
---


# Software Reference - Prices

After copying, the text can be translated into other languages. Please make sure that the key for the basic language is not changed in the translated text.

---
## Overview

**Price unit**
The units can be interpreted as price and/or quantity unit; the unit sqm can be used as a quantity unit as well as a price unit for example while the unit Net-% is only used as a price unit.

**Code**
Identification number (ID) of the unit. It is preset by the system and must not be changed.

**Remark**
You can change this text if required.

**Inch**
If you are using both metric and imperial measures, there will be two entries for the same key for certain measures.
The parallel use of both measures should always be discussed with A+W Software GmbH.

**External key**
The external key can be used for communicating with other programs, e.g. for transfer to production or for statistical analysis.

**Locked**
A unit can be locked for input in price management and in documents if it is no longer required.
- The unit can be allocated.
- The unit is locked and cannot be allocated. If it has been allocated to products and in documents, it will still be shown however.

## Insurance Prices

**Master Data > Prices > Insurance Prices**

When entering order items, the *Insurance prices* module can be used to calculate repair or emergency glazing according to the rules of the price lists of Frankfurter Versicherung or Gothaer Versicherung.

We basically distinguish repair and emergency glazing. At order entry, the system will want to know which type of glazing you are going to enter.

This dialog serves for managing the corresponding insurance conditions.

Dialog *Insurance prices* offers the following tabs:
- Insurance Prices - Repair Glazing
- Insurance Prices – Emergency Glazing
- Insurance Prices – Surcharges/Discounts
- Insurance Prices - Additional Services

### Insurance Prices – Repair Glazing

**Master Data > Prices > Insurance Prices > Repair Glazing tab**

This tab serves for defining how to calculate repairs. Repairs, disposal, and working time surcharges have to be entered as products of the product type and group Services/surcharges.

**Calculation type**
Insurances to which the calculation settings apply. The illustrated examples are only valid for Germany.

**Rate**
- **Price list**: Insurance price list.
- **Key**: Key for insurance prices.

**Repair/disposal allocation**
- **Repair**: Repair product number for the selected product type or product group.
- **Disposal**: Product number for the disposal of the selected product type or product group.

**By product type, by product class**
- **Product type, product class**: Product type and product class to which the repair or disposal products have been allocated.
- **Repair, disposal**: These two table fields show the product numbers from the fields Repair and Disposal.

**Work outside regular working hours**
- **Night work/work on Sundays/bank holidays**: Product number of the work to be charged for night shifts or for work performed on Sundays and public holidays.
- **Outside regular working hours**: Product number of the service to be charged for work performed on working days outside regular working hours.

**Table**
This list offers all tables for insurance prices matching the selection criteria.

### Insurance Prices – Emergency Glazing

**Master Data > Prices > Insurance Prices > Emergency Glazing tab**

This tab is used for defining how emergency glazing should be calculated. The fields *Calculation type* and *Rate* are described in connection with the tab *Repair glazing*. (⇨ "Insurance Prices – Repair Glazing" on page B-703)

**Emergency glazing**
- **Emergency glazing**: Surcharge product for emergency glazing.
- **Min. order value**: Amounts to be calculated as a minimum value for:
    - Emergency glazing (material)
    - Night shifts and work on public holidays (surcharge)
    - Work performed outside regular working hours
If the actual price for emergency glazing lies below this minimum value in the order in question, the program will automatically calculate the minimum value. Every single value will be checked.
- **Night work/work on Sundays/bank holidays**: Product number of the work to be charged for night shifts or for work performed on Sundays and public holidays.
- **Outside regular working hours**: Product number of the service to be charged for work performed on working days outside regular working hours.
- **Disposal**: Product number for disposal.

### Insurance Prices – Surcharges/Discounts

**Master Data > Prices > Insurance Prices > Surcharges/Discounts tab**

This tab is used for defining the surcharges and discounts for the insurance in question. The available fields depend on the selected insurance.

The fields *Calculation type* and *Rate* are described in connection with the tab *Repair glazing*. (⇨ "Insurance Prices - Repair Glazing" on page B-703)

**Surcharges for lites**
(only for "Frankfurter Versicherung")

- **to ... sqm ... pcs**: You can define up to four levels for surcharges. The surcharge per piece is entered for every step.

> **Example**
> Up to 0.25 sqm, 80.00 € will be added per lite.
> Up to 0.80 sqm, 60.00 € will be added per lite.
> etc.

- **for max. ... lites**: You can restrict the lite surcharges to a maximum number of lites. If more lites are entered in the order, surcharges will not be taken into account.

**Travel costs**
- **Product number**: Product number for the travel costs.
- **Up to net order value**: You can enter a (net) order value up to which the surcharge should be applied. No surcharge will be applied if the order value is higher.

**Workshop labour**
- **Installation costs refund**: Proportional surcharge to be billed for workshop labour for repairs. The surcharge is based on the order value.

**Surcharge for roofing work**
- **Surcharge**: Proportional surcharge to be billed for roofing work for repairs. The surcharge is based on the order value.

**Qty. discount per project**
(only "Gothaer Versicherung")

- **Window/patterned glass**: Surface in sqm from which on a quantity discount should be granted.
- **Other glass**: Quantity (units) from which on a quantity discount should be granted.

### Insurance Prices - Additional Services

**Master Data > Prices > Insurance Prices > Additional services tab**

This tab is used for defining the additional services that apply for the corresponding insurance. Glue and cement must be defined as products for this purpose. The available fields depend on the selected insurance.

The fields *Calculation type* and *Rate* are described in connection with the tab *Repair glazing*. (⇨ "Insurance Prices - Repair Glazing" on page B-703)

**Min. installation costs**
(only "Gothaer Versicherung")

- **for work on site, for workshop labour**: You can enter different minimum amounts for the first lite and all following lites that will be applied if the actual price for the work lies below the minimum price.
- **max. ... lites**: You can restrict the minimum installation costs to a maximum number of lites. If more lites are entered in the order, these minimum costs will be ignored.

**Glue/cement**
(all insurances)

- **Glue (incl. dissolv., cleaning, glue)**: Product number for the glue.
- **Cement (incl. dissolv., cleaning, stick.)**: Product number for the cement.
- **Glue (w/o dissolving, total loss)**: Product number for the glue in case of a total loss.
- **Cement (w/o dissolvent, total loss)**: Product number for the cement in case of a total loss.

## Price Elements of Grills

**Master Data > Prices > Elements of Grill Price**

This dialog shows the grill elements that can be used for pricing of the order. The element numbers have to match the numbers in A+W CAD Designer. You can add further elements. These have to be defined in A+W CAD Designer as well.

The prices for these grill elements are entered in dialog Prices:
⇨ "Prices - Grills" on page B-721

## Price Management

**Master Data > Prices > Prices**

A+W Business price management serves to define the prices for your products. You can e. g. handle prices for single annealed glass by price matrices and the prices for IG units by cubes.

This section provides information on the following subjects:
- "Price Management Menus" on page B-710
- "Prices" on page B-713
- "Change Prices" on page B-724
- "Copy Prices" on page B-726
- "Delete Prices" on page B-727
- "Import Price Matrix" on page B-728
- "Export Price Matrix" on page B-731

Before entering the prices you have to define the rates. The descriptions of the corresponding dialogs can be found in section Prices:
⇨ "Prices" on page B-659

### Price Management Menus

**Master Data > Prices > Prices**

The product management menus allow defining the default settings for the dialog and open other dialogs without closing price management.

This section provides information on the following subjects:
- "Options Menu" on page B-710
- "Functions Menu" on page B-711
- "History Menu" on page B-712

> **History menu only in connection with Gupta database**
> Menu History is only available in connection with the SQL Gupta database. MS SQL server database does not show this menu.

### Options Menu

**Master Data > Prices > Prices > Options menu**

This menu allows you to define the default settings for this dialog. You can enable or disable this option.

- **Preset last rate**: Shows in the fields Year and Key the entries for the last selected rate.

### Functions Menu

**Master Data > Prices > Prices > Functions menu**

Use this menu to open other dialogs without closing the current one.

**Prices group**
- **Change**: Opens the dialog *Change prices* to change one or more prices at once. (⇨ "Change Prices" on page B-724)
- **Copy**: Opens the dialog *Copy prices* to transfer prices from one price list or price key to another. (⇨ "Copy Prices" on page B-726)
- **Delete**: Opens the dialog *Delete prices* in order to delete prices. (⇨ "Delete Prices" on page B-727)

**Data exchange group**
- **Automatic import**: Opens the dialog *Prices* or *Price matrix import* for importing the IG price matrix from an existing file. (⇨ "Import Price Matrix" on page B-728)
- **Interactive import**: Opens the dialog *Prices* or *Price matrix import* for importing the IG price matrix from an existing file. (⇨ "Import Price Matrix" on page B-730)
- **Export price matrix**: Opens the dialog *Price matrix export* to save the IG price matrix in a file. (⇨ "Export Price Matrix" on page B-731)

### History Menu

Menu *History* allows to define the master data changes to be monitored. You can view the monitored changes.

> **History menu only in connection with Gupta database**
> Menu History is only available in connection with the SQL Gupta database. This menu is not available in the MS SQL database.

This menu is available in the following dialogs:
- Customer management
- Supplier management
- Price Management
- Discount management

The following entries are displayed:
- **Analysis**: Opens the dialog *History of changes* to analyse the detected changes. (⇨ "History of Changes" on page B-732)

> **Entry 'Analysis'**
> The entry Analysis is accessible only if the monitoring of changes has been enabled in module *Utilities > System > Monitoring of changes*.

## Prices

**Master Data > Prices > Prices**

Dialog *Prices* offers the following tabs:
- Prices - Price Selection
- Prices - Matrix
- Prices - Vector
- Prices - Individual Price
- Prices - Shape
- Prices - Grills
- Prices - Cube
- Prices - Price Formula

This dialog is used for maintaining prices in different rates and price lists. (⇨ Tutorial 1, "Price Tables" on page B-230)

> **Tip**
> New price lists can be quickly created by copying and changing an existing price list.
> ⇨ Tutorial 1, "Copying and Changing Prices" on page B-245

### Prices - Price Selection

**Master Data > Prices > Prices > Price Selection tab**

This tab serves to select the rate and allocate groups, surcharges, and projects. You can also define if the prices should be valid for alternatives.
(⇨ Tutorial 1, "Input of Unit Prices" on page B-236)

> **Selection mode**
> The selection mode appears by default when you open this dialog. You can restrict the search for price lists to customers, suppliers, groups, and projects if required.

The list shows all price tables matching the search criteria for the price list and key.

Based on the selection criteria, the entries are shown in the following groups:
- Standard (general prices)
- Customer groups or supplier groups
- Customer or supplier

Prices are grouped by price list. Select a price list to release the tab in which the price is defined.

Double-click on the entry **Allocated products** to view the products calculated according to this price list.

**Identification**
- **Table, from-to**: Number of the price table. The number of the table is usually the same as the number of the product to which the table refers.
- **Price list, key**: Price list and price key (rate) for which the prices have been entered. The fields are shown at order entry and can be changed per item in order to use another rate for pricing.
- **Key text**: The name of the (price) key must be the same as the key text.
- **Remark**: Comment, e.g. regarding the validity.

**Miscellaneous Surcharges**
- **Table**: Surcharge table number. These surcharges will be automatically applied in the order but can be disabled if required.

**Deviations**
You can define deviations from the standard product for which other prices have to be calculated.

- **Shape group**: If a shape belonging to a shape group is entered in the order, other values should be applied for the surface price. You can e.g. use different shape surcharges for several IG price keys. You can use a shape group to avoid entering shape surcharges for the individual price keys. Shape surcharges are entered on tab Shapes. (⇨"Prices - Shape" on page B-720)
- **Rounding width, Rounding height**: Values for the rounding of width and height that differ from the standard rounding for the products. These roundings are only valid for pricing. For cutting, the values entered in the product definition will be applied.
- **Min. width, Min. height**: Values for the minimum width and minimum height that differ from the values entered in product definition.
- **Next key**: You can enter a 'next' key if the price should be valid only up to a certain size. The next key defines the price table to be used for pricing if the standard price table shows no prices for the size entered in the order.

**Prices for**
When you select one of the price tables on the list, this section shows all products for which customers, suppliers, or groups have been defined. You can restrict the search to partner- and project-related price tables by selecting the appropriate criteria.

> **Individual prices**
> Individual prices always have priority over all other prices and discounts for the pricing of documents.

### Prices - Matrix

**Master Data > Prices > Prices > Matrix tab**

This tab permits to enter a price matrix with up to two limit types.
⇨Tutorial 1, "Limit Types for Graduations" on page B-249
⇨Tutorial 1, "Defining a Graduated Price with Limits" on page B-256

**Limit type1, Limit type2**
The limit types can be used for price graduation. The limit type defines the measure for graduation. You can choose different units for the two limit types, e. g. thickness and weight. The input field for the limit type is accessible when you add a new column. The limit value refers to the limit type. If `<n.e.>` is entered as a limit type, the price is valid per price unit.

**Min. values**
The minimum values are checked at order entry. If the actual entries fail to reach the defined minimum price or quantity, a message appears and/or a surcharge is applied.
- **Gross price, Net price**: Minimum price for an order item.
- **Quantity**: Minimum order quantity.

**Price specification**
- **Price unit**: The price unit refers to the details defined in the matrix.
- **Currency**: If you are using different currencies you have to define the currency for which the gross and net price should be valid.
- **Triangle**: In a matrix or cube, you can enter prices so that the defined limits can be exchanged, e.g. width and height.
    - The limit types may not be switched. In this case, a price must be entered for every column/line in all fields. You should choose this setting for lites for which the cutting direction is important.
    - The limit types may be switched. In this case, the price has to be entered only for one of the combinations of limit types.
(⇨Tutorial 1, "Triangle" on page B-253)

**Matrix**
Enter - in every field per line and column - the price that will be applied to the corresponding combination of limit types.
(⇨ Tutorial 1, "Matrix” on page B-253)

### Prices - Vector

**Master Data > Prices > Prices > Vector tab**

Define the price and a limit type.

Prices can also be graduated by the number of lites for example. The quantity limit *Number of lites* determines the number of lites on the levels below the parent glass. If the parent glass has no children, 1 will be returned. This kind of graduation is suitable for surcharges on gas for example.
⇨ Tutorial 1, "Vector" on page B-252
⇨ Tutorial 1, "Defining a Graduated Price with Limits" on page B-256

The fields are described on the Matrix tab.
⇨ "Prices - Matrix" on page B-716

### Prices - Individual Price

**Master Data > Prices > Prices > Individual price tab**

This tab is used to define the individual price, e.g. for fittings or for single annealed per sqm.
⇨ Tutorial 1, "Unit Price" on page B-231
⇨ Tutorial 1, "Input of Unit Prices" on page B-236

### Prices - Shape

**Master Data > Prices > Prices > Shape tab**

This tab is used to define the price of a shape, considering a limit type if required.

Shape prices are usually a surcharge on the glass price. These surcharges can be defined for all glass types used for the production of shapes.
⇨ Tutorial 1, "Defining a Shape Price" on page B-241

The fields are described on the Matrix tab.
⇨ "Prices - Matrix" on page B-716

### Prices - Grills

**Master Data > Prices > Prices > Grills tab**

This tab is used to define the price of grills, considering a limit type if required.

This list shows all grill elements for which prices can be entered. You can enter a separate price per element or a total price for the pattern.
⇨ Tutorial 1, "Grill Price" on page B-234

The fields are described on the Matrix tab.
⇨ "Prices - Matrix" on page B-716

### Prices - Cube

**Master Data > Prices > Prices > Cube tab**

This tab is used to enter a price in the shape of a cube, considering up to three limit types, e.g. width, height, and thickness.
⇨ Tutorial 1, "Cube" on page B-255
⇨ Tutorial 1, "Limit Types for Graduations" on page B-249

The fields are described on the Matrix tab.
⇨ "Prices - Matrix" on page B-716

### Prices - Price Formula

**Master Data > Prices > Prices > Price formula tab**

Enter the price in the shape of a formula. The formula can be directly entered in the formula editor.

**Formula editor**
- **[Syntax check]**: When you have entered a formula you can use this button to check its syntax. Only correct formulas can be used for pricing.
- **[Insert formula]**: Use this button to open the dialog *Formula management* from where you can copy a formula in order to modify it. (⇨ "Formulas" on page B-1026)

## Change Prices

**Master Data > Prices > Prices > Functions menu > Change prices**

This dialog is used for changing individual prices. You can increase or reduce the price or surcharge by a fixed amount or a percentage.
⇨ Tutorial 1, "Copying and Changing Prices" on page B-245

**Price selection**
- **From no., to**: Number(s) of the price list(s) to be changed.
- **Quantity**: Number of records.
- **Price list, key**: Choose the price list and the key for which price lists should be amended.
- **Price units**: Generally, all price units will be adopted. You can however adapt the selection to your requirements.

**Price type**
Choose an option to define the price type to be changed:
- **General**: The general price tables will be changed.
- **Customer group, Supplier group**: The price tables for a customer group or supplier group will be changed. This option releases the field *Group* from where you can select the required group.
- **Customer, Supplier**: The price tables for a customer or a supplier should be changed. This option releases the field *Partner* from where you can select the required partner.

**Project**
This field is locked if you have selected the option *General*. When you select a group or a partner, you can also define the project for which the price table should be changed.

**Price change**
- **Surcharge, Deduction**: This option determines whether the defined value should be added to or deducted from the prices in the price tables.
- **Per cent, Absolute**: If the actual prices are to be changed, enter a percentage or an absolute value.
- **Rounding**: You can change the rounding for the selected price table.
