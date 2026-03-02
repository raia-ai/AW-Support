---
description: "EN_AWBusiness_Master_Data_9_7-4"
---


# Prices

---
## Copy Exchange Prices – Price Change

> Master Data > Prices > Exchange surcharges > Functions menu > group Copy > General > Price change tab

*Fig. B-72 Copy exchange prices – price change*

Enter the details of the change.

If you have entered the same table as a source and target, the surcharges will be changed without being copied to other tables.

The fields in sections Copy from and Copy to are described in connection with the Source tab.
⇨ "Copy Exchange Prices - Source, Target" on page B-674

**Surcharge, Deduction**: This selected option determines whether the defined value should be added to or deducted from the surcharges in the tables.

**Rounding**: You can change the rounding for the selected table.

**Per cent, Absolute**: If the actual surcharges are to be changed, enter a percentage or an absolute value.

## Copy Prices per Exchange Product Completely

> Master Data > Prices > Exchange surcharges > Functions menu > group Copy > all per exchange article

You can copy or change one or more exchange surcharges for lites to be replaced.

This dialog offers the following tabs:
- "Copy all Exchange Surcharges – Source, Target" on page B-677
- "Copy all Exchange Surcharges – Price Change" on page B-679

### Copy all Exchange Surcharges – Source, Target

> Master Data > Prices > Exchange surcharges > Functions menu > group Copy > all per exchange article > Source tab

*Fig. B-73 Copy all exchange prices - source*

This dialog is used for copying the surcharges from one table to another table or to another rate. Only the exchange surcharges that are applied to lites to be replaced will be copied.

⇨ Tutorial 1, "Copying and Changing Replacement Surcharges" on page B-296

If you only want to change the surcharges, enter the same table for the source and target. You can enter the amended values on tab Change prices.

⇨ "Copy all Exchange Surcharges - Price Change" on page B-679

### Copy from, Copy to

**Table**: Number of the exchange table.

**Replacement**: Number of the product to be removed from the unit.

**Price list, key**: Price list and key (rate) allocated to the exchange surcharge.

**IG, LG, Both**: Product type to which the surcharge is applied. Lites can be exchanged only in IG unit or laminated glass. It does not matter which of the lites is exchanged, e.g. if it is the second or third lite of a triple IG unit. Select the option Both if exchange prices for IG and laminated glass are to be copied.

**Change prices**: To transfer the surcharges to a filled-in table you have to decide whether the surcharges in the target table should be changed.
- The surcharges in the target table will not be changed. The additional surcharges from the source table will be added.
- All existing surcharges in the target table will be changed.

**Price type**: Choose an option to specify where the surcharges should be applied:
- **General**: General surcharge, calculated irrespective of business partners or partner groups (standard exchange surcharge).
- **Customer group, Supplier group**: Surcharge for the selected group of customers or suppliers
- **Customer, supplier**: Surcharge for the selected customer or supplier

**Project**: This field is locked if you have selected the option General. When you select a group or a partner, you can also define the project for which the surcharge table should be changed.

### Copy all Exchange Surcharges – Price Change

> Master Data > Prices > Exchange Surcharges > Functions menu > Copy group > All per exchange article > Price change tab

*Fig. B-74 Copy all exchange prices – price change*

Enter the details of the change.

If you have entered the same table as a source and target, the surcharges will be changed without being copied to other tables.

The fields in sections Copy from and Copy to are described in connection with the Source tab.

⇨ "Copy all Exchange Surcharges - Source, Target" on page B-677

**Surcharge, Deduction**: This selected option determines whether the defined value should be added to or deducted from the surcharges in the tables.

**Rounding**: You can change the rounding for the selected table.

**Per cent, Absolute**: If the actual surcharges are to be changed, enter a percentage or an absolute value.

## Delete Exchange Surcharges

> Master Data > Prices > Exchange Surcharges > Functions menu > Delete Prices

*Fig. B-75 Delete exchange surcharges*

This dialog is used to delete individual exchange surcharges or a sequence of exchange surcharges.

### Price type

Choose an option to define for whom the surcharge to be deleted is valid:
- **General**: General surcharge, calculated irrespective of business partners or partner groups (standard exchange surcharge).
- **Customer group, Supplier group**: Surcharge for the selected group of customers or suppliers
- **Customer, supplier**: Surcharge for the selected customer or supplier

### Project

The surcharge can refer to a certain project. All projects will be offered for selection. This field is locked if you have selected the option General.

### Price selection

**Table**: Number of the exchange table to be deleted.

**IG, LG, Both**: Product type to which the surcharge is applied. Select the option Both to delete the exchange prices for IG and laminated glass.

**Exchange from, Exchange - to**: Product numbers of the exchange lites for which the exchange surcharge has been defined.

**Quantity**: Number of records to be deleted.

**Price list, key**: Price list and key (rate) allocated to the exchange surcharge.

## Change Exchange Prices

> Master Data > Prices > Exchange Surcharges > Functions menu > Change prices

You can change one or more exchange surcharges together.

This dialog offers the following tabs:
- "Change Exchange Prices – Price Type" on page B-681
- "Change Exchange Prices – Price Change" on page B-683

### Change Exchange Prices – Price Type

> Master Data > Prices > Exchange Prices > Functions menu > Change prices > Price Type tab

*Fig. B-76 Change exchange prices – Price type tab*

Choose the exchange surcharges to be changed.

⇨ Tutorial 1, "Copying and Changing Replacement Surcharges" on page B-296

#### Price selection

**Table**: Number of the exchange table the prices of which should be changed.

**Quantity**: Number of records.

**From no, to**: Numbers of the records to be changed.

**Price list, key**: Price list and key (rate) allocated to the exchange surcharge.

**IG, LG, Both**: Product type to which the surcharge is applied. Lites can be exchanged only in IG unit or laminated glass. It does not matter which of the lites is exchanged, e.g. if it is the second or third lite of a triple IG unit. Use the option Both to change the exchange prices for IG and laminated glass.

#### Price type

Choose an option to define for whom the surcharge to be changed is valid:
- **General**: General surcharge, calculated irrespective of business partners or partner groups (standard exchange surcharge).
- **Customer group, Supplier group**: Surcharge for the selected group of customers or suppliers
- **Customer, supplier**: Surcharge for the selected customer or supplier

**Project**: This field is locked if you have selected the option General. When you select a group or a partner, you can also define the project for which the surcharges should be changed.

### Change Exchange Prices – Price Change

> Master Data > Prices > Exchange Prices > Functions menu > Change prices > Price change tab

*Fig. B-77 Change exchange prices - Price change tab*

Enter the details of the change.

The fields in section Price selection are described in connection with the Price type tab.
⇨ "Change Exchange Prices - Price Type" on page B-681

**Surcharge, Deduction**: This selected option determines whether the defined value should be added to or deducted from the surcharges in the tables.

**Rounding**: You can change the rounding for the selected surcharges.

**Per cent, Absolute**: If the actual surcharges are to be changed, enter a percentage or an absolute value.

## Price Groups

> Master Data > Prices > Price Groups

*Fig. B-78 Price Groups*

This dialog is used for defining the price groups. The price groups are used for calculating prices for patterned glass and exchange surcharges so as to avoid having to keep a special price table for every single product.

The products are allocated to the price groups in dialog Price group allocation.
⇨ "Price Group Allocation" on page B-685

**Name**: The price groups are usually numbered in alphabetical order.

**Remark**: Comments, e.g. regarding the use of the price group.

## Price Group Allocation

> Master Data > Prices > Price group allocation

*Fig. B-79 Price Group Allocation*

This dialog is used for allocating a price list and a price group to the individual products.

Each price group can be allocated an exchange surcharge on the Group surcharges dialog that makes the management of prices and surcharges much easier.

⇨ Tutorial 1, "Price Group Allocation" on page B-274

### Functions menu

You can use this menu for accessing the dialog Copy key where you can copy the key from one price list to another.
⇨ "Copy Price Group Allocation" on page B-686

### Identification - Rate

**Sales list, Purchase list**: Choose an option to define the type of rate to which price groups should be allocated.

**Price list, key**: Price list and key (rate) where the price is specified.

### Product selection

This section allows selecting the products to be exchanged in an IG unit and/or laminated glass.

**Article/MCode, Name**: Number, matchcode and name of the product to be allocated to the price group.

### List of allocations

This table lists all products matching the defined criteria.

**PG IG, PG LG**: From the columns PG IG and PG LG select the price groups to which the exchange product should belong.

## Copy Price Group Allocation

> Master Data > Prices > Price group allocation > Functions menu > Copy

*Fig. B-80 Price group allocation - copy*

This dialog is used for copying the price group allocation to another rate.

The fields are described in connection with the dialog Price group allocation.
⇨ "Price Group Allocation" on page B-685

## Group Surcharges

> Master Data > Prices > Group Surcharges

*Fig. B-81 Group-based surcharges*

This dialog is used for defining general surcharges for the price groups that will be applied when a lite is exchanged. In contrast to exchange surcharges, the glass thickness is used as the limit type.

⇨ Tutorial 1, "Defining a Group Surcharge" on page B-277

### Functions menu

Use this menu to open other dialogs without closing the current one. The following entries are displayed:

- **Copy prices**: Opens the dialog Copy exchange prices in order to copy group surcharges.
  ⇨ "Copy Exchange Prices" on page B-673
- **Delete price**: Opens the dialog Delete prices by price group in order to delete group surcharges.
  ⇨ "Delete Group Surcharges" on page B-692
- **Change price**: Opens the dialog Change price to change a number of surcharges at once.
  ⇨ "Change Prices" on page B-724

### Identification - Rate

**Sales list, Purchase list**: Choose an option to define the type of rate to which group surcharges should be allocated.

**Price list, key**: Price list and key (rate) to which the group surcharge is allocated.

**Product type IG, LG**: Product type for which the group surcharge is applied. Lites can be exchanged only in IG unit or laminated glass. It does not matter which of the lites is exchanged, e. g. if it is the second or third lite of a triple IG unit.

**Thickness**: Thickness of the lite to be replaced. This is the lite that is going to be removed from an IG or laminated glass unit.

### Select customers/customer groups, suppliers/supplier groups

This section is used to allocate a price group surcharge to a customer, a supplier, or to a customer group or to a supplier group.

Choose an option to define where the surcharge should be applied:
- **General**: General surcharge
- **Customer group, Supplier group**: Surcharge for the selected group of customers or suppliers
- **Customer, supplier**: Surcharge for the selected customer or supplier

**Name 1, Name 2**: Names of the selected partners.

### Overview

This list shows all group surcharges matching the defined criteria.

- **Glass thickn.**: Thickness of the lite to be removed from the IG unit or from the laminated glass.
- **Price group**: Price group for which the surcharge is valid.
- **Surcharge**: Surcharge per thickness. Depending on the surcharge type, this value will be interpreted as a proportional surcharge or as an amount.
- **Surcharge type**: The surcharge type defines how the entry in field Surcharge should be interpreted, e.g. as a proportional surcharge on the price, as amount per length, etc.
- **Min. surface**: When you enter a minimum surface for a lite to be changed in, this surface will be used as a basis for the surcharge whenever the order surface is smaller.
- **Min. price gross, Min. price net**: If you enter a minimum price, it will always be used as a basis for the surcharge if the price of the exchange product is lower in the order.
- **Roundg. width, Roundg. height**: You can enter different rounding values for the width and the height that will be applied if the group surcharge is used for pricing.
- **Misc. surcharges**: You can define a miscellaneous surcharge in addition to the exchange surcharge, e.g. for cutting. This surcharge is applied to the new product. Miscellaneous surcharges are entered in the dialog of that name:
  ⇨ "Miscellaneous Surcharges" on page B-664
- **Price key, Price list**: Shows the allocated key and year.

### Select project

The surcharge can refer to a certain project. All projects will be offered for selection.

### Table

List by customer/customer group, supplier/supplier group
The list shows customers/customer groups, suppliers/supplier groups, or projects for which group surcharges have been entered in the selected rate.

## Copy Group Surcharges

> Master Data > Prices > Group surcharges > Functions menu > Copy prices

You can change one or more group surcharges together.
This dialog offers the following tabs:
- "Copy Group Surcharges – Source, Target" on page B-690
- "Copy Group Surcharges - Price Change" on page B-691

### Copy Group Surcharges – Source, Target

> Master Data > Prices > Group surcharges > Functions menu > Copy prices

*Fig. B-82 Copy price group-related surcharges – source tab*

This tab is used to copy the group surcharges, e. g. to transfer the surcharges for a certain thickness to another rate.

⇨ Tutorial 1, "Copying a Group Surcharge" on page B-283

#### Copy from, Copy to

**Thickness from**: Glass thickness for which a group surcharge should be calculated.

**Price list, key**: Price list and key (rate) to which the group surcharge is allocated.

**IG, LG, Both**: Product type for which the group surcharge is applied. The option Both is used to copy the group surcharges for IG and laminated glass.

**Change prices**: To transfer the surcharges to a filled-in table you have to decide whether the surcharges in the target table should be changed.
- The surcharges in the target table will not be changed. The additional surcharges from the source table will be added.
- All existing surcharges in the target table will be changed.

**Price type**: Choose an option to specify where the surcharges should be applied:
- **General**: General surcharge, calculated irrespective of business partners or partner groups (standard exchange surcharge).
- **Customer group, Supplier group**: Surcharge for the selected group of customers or suppliers
- **Customer, supplier**: Surcharge for the selected customer or supplier

**Project**: This field is locked if you have selected the option General. When you select a group or a partner, you can also define the project for which the surcharge table should be changed.

### Copy Group Surcharges – Price Change

> Master Data > Prices > Group surcharges > Functions menu > Copy prices

*Fig. B-83 Copy price group-related surcharges - tab price change*

Enter the details of the change.
The fields in sections Copy from and Copy to are described in connection with the Source tab.

⇨ "Copy Group Surcharges – Source, Target" on page B-690

**Surcharge, Deduction**: This selected option determines whether the defined value should be added to or deducted from the surcharges in the tables.

**Rounding**: You can change the rounding for the selected surcharges.

**Per cent, Absolute**: If the actual surcharges are to be changed, enter a percentage or an absolute value.

## Delete Group Surcharges

> Master Data > Prices > Group surcharges > Functions menu > Delete prices

*Fig. B-84 Delete price group-related surcharges*

This dialog is used to delete individual group surcharges or a sequence of group surcharges.

### Price type

Choose an option to define where the surcharge should be applied:
- **General**: General surcharge, calculated irrespective of business partners or partner groups (standard exchange surcharge).
- **Customer group, Supplier group**: Surcharge for the selected group of customers or suppliers
- **Customer, supplier**: Surcharge for the selected customer or supplier

### Project

The surcharge can refer to a certain project. All projects will be offered for selection.

### Price selection

**From thickness, to thickness**: Glass thickness for which the group surcharge has been defined.

**Quantity**: Number of records.

**IG, LG, Both**: Product type to which the surcharge is applied. Select the option Both to delete the delete prices for IG and laminated glass.

**Quantity**: Number of records to be deleted.

**Price list, key**: Price list and key (rate) to which the group surcharge is allocated.

## Change Group Surcharges

> Master Data > Prices > Group Surcharges > Functions menu > Change Prices

You can change one or more group surcharges together.
This dialog offers the following tabs:
- "Change Group Surcharges - Price Type" on page B-693
- "Change Group Surcharge - Price Change" on page B-695

### Change Group Surcharges - Price Type

> Master Data > Prices > Group Surcharges > Functions menu > Change Prices

*Fig. B-85 Change price group-related surcharges and tab Price change*

Select the group surcharges to be changed.
Group surcharges are changed in the same way as exchange surcharges.

⇨ Tutorial 1, "Copying and Changing Replacement Surcharges" on page B-296

#### Price selection

**From no., to**: Glass thickness for which the group surcharge has been defined.

**Quantity**: Number of records.

**Price list, key**: Price list and key (rate) to which the group surcharge is allocated.

**IG, LG, Both**: Product type to which the surcharge is applied. Select the option Both to delete the delete prices for IG and laminated glass.

#### Price type

Choose an option to specify where the surcharges should be applied:
- **General**: General surcharge, calculated irrespective of business partners or partner groups (standard exchange surcharge).
- **Customer group, Supplier group**: Surcharge for the selected group of customers or suppliers
- **Customer, supplier**: Surcharge for the selected customer or supplier

**Project**: This field is locked if you have selected the option General. When you select a group or a partner, you can also define the project for which the surcharges should be changed.

### Change Group Surcharge - Price Change

> Master Data > Prices > Group Surcharges > Functions menu > Change Prices

*Fig. B-86 Change price group-related surcharges and tab Price change*

Enter the details of the change.

**Surcharge, Deduction**: This selected option determines whether the defined value should be added to or deducted from the surcharges in the tables.

**Rounding**: You can change the rounding for the selected surcharges.

**Per cent, Absolute**: If the actual surcharges are to be changed, enter a percentage or an absolute value.

## Mixed Price Calculation

> Master Data > Prices > Mixed price calculation

*Fig. B-87 Mixed Price Calculation*

For special IG or laminated glass structures you can refer to special prices, e. g. for IG 4/6.
Prerequisite is that the price share of the elements for calculation purposes is defined in company master data.

⇨ "Company Data > Documents" on page B-928

At item entry, IG is entered as a mixed product on tab Supplement. The item has to be entered in a certain sequence:
- Nothing must be entered in the main product itself but only on tab Supplement > Mixed calculation.
- The IG products and - if applicable - the mixed factor are entered from the outside inwards.
- Now enter the quantity, width, and height and - if applicable - an exchange on the first tab.

Other surcharges will be taken into account only if they have been defined in Prices.

## Shape Processing Surcharges

> Master Data > Prices > Shape Surcharges

*Fig. B-88 Shape processing surcharges*

This dialog is used for entering processing surcharges for shapes. These surcharges can differ from price table to price table, e.g. per shape for edgework and corner processing. Prerequisite for this is that a price table has been created for every single processing step.

⇨ Tutorial 1, "Defining a Shape Processing Surcharge" on page B-302

### Functions Menu

This menu is used for accessing the dialog Copy surcharges where you can copy the shape surcharges from one surcharge table to another.

⇨ "Copy Surcharges" on page B-699

### Processing

**Price table**: Number of the price table for processing.

**Price list, Price key**: Price list and key (rate) to be used for shape processing.

**Price type**: The price type defines how the entries in the Segment fields should be interpreted, e. g. as a proportional surcharge on the price, as an amount per length, or per piece.

### Surcharges

Depending on the shape, the fields Segment 1 to Segment 8 are released in which you can enter the surcharges. Depending on the price type, this will be interpreted as a proportional surcharge or as an amount (for all segments).

Based on the difficulty of the processing, these values may differ in size. For processing a curved edge, a higher surcharge may be applied than for processing a straight edge.

### Shape

**Number**: Number of the shape for which the surcharge should be calculated. If you have entered a shape, field Sketch shows a schematic view of the shape and its segments for which entries can be made.

**Sketch**: Schematic view of the shape showing the number of segments. The numbers on the outside refer to the edge and those on the inside, to the corners.

### Min. entry

**Min. price**: If you enter a minimum price, this will always be used as a basis for the surcharge if the processing price defined in the order is lower. This entry is not suitable for the price type Piece.

**Min. quantity**: If you enter a minimum quantity, it will always be used as a basis for the surcharge if the processing price defined in the order is lower. This entry is especially suitable for the price type Pieces.

### Table

This table lists all shape surcharges matching the selection criteria.

## Copy Surcharges

> Master Data > Prices > Shape Surcharges

*Fig. B-89 Copy shape processing surcharges*

This dialog is used for copying shape surcharges from one surcharge table to another.

### Source, Target

These fields define the price list from which the surcharges are copied and the price list to which they should be transferred.

**Price list, Price key**: Price list and key (rate) to which the surcharge table is allocated.

**Select price table**: You can restrict the transfer to a certain surcharge table.
- All shape processing surcharges of the selected price list will be copied.
- Field Price table is released so that you can choose the surcharge table to be copied.

**Price table**: Select the surcharge table to be copied. This field is accessible only if the checkbox Select price table has been checked.

**Overwrite existing records**: If the target table already contains shape processing surcharges, you have to decide whether these should be kept or changed.
- Existing surcharges will be kept and completed by the new surcharges from the source table.
- The surcharges in the target table will be replaced by the surcharges from the source table. Additional surcharges will be added.

## Price and Quantity Unit

> Master Data > Prices > Price/Quantity

> **Dialog locked**
> Usually, this dialog can only be accessed by the system administrator. Amendments have to be agreed with A+W Software GmbH.

Price and quantity units are fixed. These units cannot be deleted. You can add quantity units but these will be neglected by the system.

*Fig. B-90 Price and quantity units*

In this dialog, price and quantity units can be locked or edited, i.e. translated into other languages.

Price units are allocated to the corresponding prices in price management.
⇨ "Price Management" on page B-710

Quantity units are allocated to the corresponding products in product management.
⇨ "Product Management" on page B-587

### Language

If you are using the Multi-lingual operation module, the units must exist on all languages tabs.
Menu > Copy units in dialog Languages can be used to copy the price and quantity units from the basic language to any other language.

⇨ "Price/Quantity Unit for Multi-Lingual Operation" on page B-555
