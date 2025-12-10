---
title: "EN_AWBusiness_Production_3-4"
source: "EN_AWBusiness_Production_3-4.pdf"
tags: ["A+W Business Production", "Software Reference", "Production Management", "Date Overview", "Customs Management", "Shipping Control", "Production Preview", "Order Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical reference guide for the A+W Business Production software, covering modules like Date Overview, Production Preview, Customs Management, and Shipping Control. It details functionalities for managing product groups, order status, delivery dates, and generating various lists and reports."
long_description: "This document serves as a detailed software reference for the A+W Business Production system. It provides comprehensive instructions and descriptions for several key modules. The 'Date Overview' section explains how to filter and evaluate product groups, bills of material (BOM), and order statuses based on delivery dates. The 'Production Preview' section details how to view summaries of glass surfaces and product types, configure display columns, and exclude specific business types from previews. The 'Customs Management' section provides a guide for creating customs lists for goods export, including managing loading lists, resetting list numbers, and exporting data for customs programs. Finally, the 'Shipping Control' module is explained, covering the organization of shipping, allocation of orders to forwarders, creation of shipping documents, and management of packing lists, partial deliveries, and surcharges. The document uses a structured approach with clear navigation paths, dialog box descriptions, and field explanations for each function."
---

---
## Date Overview

### Product groups

- **All**: You can select individual product groups. The choice depends on the selected breakdown level.
- **Individual product groups should be evaluated**: The selection fields are accessible. You can enter a start and end number. If you evaluate the bills of material as well, their product groups will not be hidden because of your selection.
- **All product groups should be evaluated**.

### With BOM

Bills of material can be included in the evaluation.
- The bills of material will not be evaluated. This means, for example, that the float glass necessary for producing IG will not be taken into account.
- Bills of material will be evaluated too. This setting is useful if you want to know how many spacers or Georgian bars have been entered, for instance.

### Order status

**From, to**: You can restrict the evaluation to order status. To get a preview, you should set the status up to transfer to Production.

### Delivery date

**From, to**: You can restrict the evaluation to orders which have to be delivered within a certain period.

### Overview

The list shows - by date - all MPG, PSG, or PGR matching the selection criteria.
- **Delivery date**: Delivery date within the defined period. The last entry for the date displayed is followed by a total line showing the figures in red.
- **MPG, PSG, PGR**: Product group number. The display depends on the selected breakdown level.
- **Description**: Name of the product group.
- **Qty**: Number of all order items belonging to the product group.
- **Surface**: Total surface of all order items belonging to the product group.
- **Weight**: Total weight of all order items belonging to the product group.
- **Net amount**: Sales values of all order items belonging to the product group.
The bottom part of the list shows the totals for the product group displayed.

## Production Preview

*Production > Date Overview > Production Preview*

You can view the sum of the glass surfaces with the product types insulating glass, single glass, tempered glass and laminated glass per delivery date.

This chapter provides information on the following subjects:
- "Production Preview (Dialog)" on page E-278
- "Definition of Preview Columns" on page E-279
- "Exclusion of Business Types" on page E-280

### Options Menu

*Production > Date Overview > Production Preview*

Use this menu to open other dialogs without closing the production preview. The following entries are displayed:

#### Display group

- **Column definition**: Opens the dialog Definition preview columns, where you can determine which columns are displayed.
  - See "Definition of Preview Columns" on page E-279
- **Hide business types**: Opens the GA-exclusion dialog, where you can determine which transaction types are not shown.
  - See "Exclusion of Business Types" on page E-280

#### Date group

With this menu you determine the date to which the preview refers.
- **By delivery date**: The preview refers to the delivery date.
- **By production end**: The preview refers to the production end.

### Production Preview (Dialog)

*Production > Date Overview > Production Preview*

*Fig. E-136 Production preview*

This dialog shows you a preview of the quantity of individual products or product types. The preview data for the respective glass type is displayed under the various tabs.

The columns can be set individually for every terminal.

See Tutorial, "Production Preview" on page E-159

The production preview analyzes all orders in terms of quantity and informs you about the future utilization, by product type and product category. Analysis includes all current orders with a shipping date equal or bigger than the present date. Analysis criteria are a combination of product type and product group.

The evaluation result is saved in a database table and shown immediately upon calling up the dialog. The display can be updated manually. The last update is shown in hours and minutes.

### Definition of Preview Columns

*Production > Date Overview > Production preview > Options menu > Display group > Column definition*

*Fig. E-137 Column definition for production preview*

In this dialog you determine which settings are to apply on an inter-company level. You need administrator rights to open this dialog.

#### Columns

- **No.**: The continuous counter is set at the column input.
- **Designation**: The title for the column header can be chosen freely, e.g. insulating glass
- **Description 2**: The title for the column header can be chosen freely, e.g. the quantity unit.
- **Type MP**: The type selection based on the main product:
  - 1 = Product type
  - 2 = Product class
- **MP**: The main product equates to the key number of the product type or product group stored in the article master data.
- **Type 0**: The type selection based on the main product:
  - 1 = Product type
  - 2 = Product group
- **No. 0**: The key number for the product type or the product group depending on type.
- **Piece/sqm**: Illustration of quantities (measurement units)
  - 1 = piece
  - 2 = sqm
- **Size category**: The size categories are determined by from-to values which refer to the measurement unit.

### Exclusion of Business Types

*Production > Production Preview > Functions menu > Hide Business Types*

*Fig. E-138 Exclusion of business types*

In this dialog you determine the business types which are not to be displayed. You need administrator rights to open this dialog.

All business types deposited in Master data > Order are available.

## Customs Management

*Production > Customs Management*

This section can be used to create various customs lists for the export of goods.

This chapter provides information on the following subjects:
- "Customs Management List" on page E-281
- "Reset List Number" on page E-285
- "Product Group with Item Quantity" on page E-285
- "Customs Export" on page E-286
- "Article Master Data Export" on page E-288

### Customs Management List

*Production > Customs Management > Customs List*

You can draw up different bills of lading for the customs documents.

This dialog offers the following tabs:
- "Loading List – Number Manager" on page E-282
- "Loading List – Customs Lists" on page E-284

#### Functions menu

This menu offers the following functions:
- **Reset list number**: Opens the dialog of that name, in which you can reset the last used number of the customs list.
  - See "Reset List Number" on page E-285
- **Product group without BOM breakdown**: Opens the dialog Product group with item quantities, which can be used to exclude certain products.
  - See "Product Group with Item Quantity" on page E-285

### Loading List – Number Manager

*Production > Customs Management > Customer List > Number Manager tab*

*Fig. E-139 Loading list – Number Manager*

You can use this dialog to select the number manager in which you have collected the orders for the customs management list.

> **Prerequisites**
> You can only print customs documents if customs tariff numbers have been allocated to the products and/or product groups.

#### Identification

- **Client**: If there are different clients, these will be offered for selection.
- **Employee**: Name of the employee logged in to A+W Business.
- **Number Manager**: Select the number manager in which the invoices are collated for the goods export.

#### Input

- **Border crossing from, border crossing to**: Select the border crossings used by the truck. All border crossing points defined in master data will be offered for selection. For a detailed description, please refer to the section Master Data.
  - See Master Data, "Zolltouren" on page B-876
- **NM pro forma invoice**: Select the number manager in which the invoices are collated.
- **Weight factor**: Specification of weight factor if the gross weight is consulted as a measurement basis to calculate customs.
- **Delivery date**: Specification of delivery date to be printed in the customs documents.

#### Overview

The overview shows all orders from the number manager.
- **Order**: Order number.
- **Cust./Suppl. number, customer/supplier**: Customer or supplier name and number.
- **Status**: Order status.
- **Delivery note**: Delivery note number.
- **Delivery date**: Delivery date defined in the order.
- **Total quantity**: Total of all items of this order
- **Total weight**: Total weight of all items per order

### Loading List – Customs Lists

*Production > Customs Management > Customs List > Customs Management Lists tab*

*Fig. E-140 Loading list - Customs management lists*

This tab can be used to display and print the customs management lists.

#### Input

- **Customs management lists no.**: This field shows the number of the customs management list. This number is automatically issued by the system when a new list is created. The selection mode allows you to display any list that has been created before.

This option defines the type of list:
- **Show customs management list**: Use this option to display the drawn-up customs management lists.
- **Customs management list proof**: Use this option to display the articles entered in a customs management list.

### Reset List Number

*Production > Customs Management > Customs List > Functions menu > Reset List Number*

*Fig. E-141 Reset list number*

Use this dialog to reset the customs management list number.

### Product Group with Item Quantity

*Production > Customs Management > Customs List > Functions menu > Product Group without BOM breakdown*

*Fig. E-142 Product group without BOM breakdown*

This dialog can be used to select the product group for which the BOM quantity shall not be taken into account.

This means that for product groups of the product type Article, only the item quantities will appear on the customs management list.

## Customs Export

*Production > Customs Management > Customs Export*

### Functions menu

*Production > Customs Management > Customs Export > Functions menu*

You can use this menu to open the dialog in which you can enter the path for an interface file for master data.
- See "Article Master Data Export" on page E-288

### Customs Export (Dialog)

*Production > Customs Management > Customs Export*

*Fig. E-143 Customs export*

Use this dialog to write an interface file that can be imported by customs management programs.

#### Mode

The file can be created for various interfaces. The combo box lists all interfaces for which an export file can be written.

#### Identification

- **Number Manager**: The list only shows orders matching the defined number manager.
- **Status from, to**: You can restrict the display of orders to a status, e.g. to Delivery note or Invoice printed.
- **Output path file**: Specification of the location where the interface files are to be saved.
- **Client**: If you are working with clients, you can create interface files for each separate client. Enter the name of the client in this field.

#### Output file format

Choose the file format:
- **ANSI**: This setting creates a genuine ASCII file acc. to the ANSI standard.
- **OEM**: This setting creates a file based on the format of another manufacturer which matches the standard.

#### Documents

This list shows all orders matching the selection criteria.
- **Order number**: Order number
- **Customer number, customer**: Number and name of the customer in this order
- **Post code, city**: Customer's place of business.
- **Country**: Country in which the customer has his place of business.
- **Net amount, net amount in FC**: Net amount of the order in home and foreign currency.
- **Date invoice**: Invoice date.
- **Status**: Status of the order.
- **Product number**: Number of the product acc. to the master data.
- **No. of products**: Number of products.
- **IG, laminated glass**: IG/laminated glass quantity.

### Article Master Data Export

*Production > Customs Management > Customs Export > Functions menu > Export of Master Data*

*Fig. E-144 Export of article master data*

You can use this dialog to save the product master data or customer master data in an interface file. The program will only export the data of the orders shown in the Customs export dialog.

#### Output path file

Enter the path for saving the interface file.

#### Export

By selecting the option, you specify whose master data should be exported.
- **Article**: The article's master data will be exported.
- **Customer**: The customer's master data will be exported.

## Optimization of Quotations

*Production > Optimization of Quotations*

This is where you can transfer your quotes to Production for test purposes, e.g. to determine how many stock sizes are required for cutting. For special glass types, this can be taken into account for pricing.

These dialogs have already been described in detail.
- **Number Manager**: The Number Manager dialog is explained in the Sales section.
  - See Sales, "Number Manager" on page C-629
- **Transfer to Production**: The function of this dialog is the same as the transfer of orders.
  - See "Transfer to Production" on page E-168

## Shipping Control

*Production > Shipping Control*

This area serves to organize the part of shipping that cannot be handled by your own fleet. You can create various shipping documents and loading lists for your forwarders.

This chapter provides information on the following subjects:
- "Shipping (forwarder)" on page E-289
- "Delete Shipping Orders" on page E-296
- "Rack Packing List" on page E-297
- "Partial Delivery" on page E-298
- "Loading Lists" on page E-300

### Shipping (forwarder)

*Production > Shipping Control > Shipping*

The Shipping dialog serves to allocate orders, racks, and storage locations.

This dialog contains the following tabs:
- "Shipping Control – Collect" on page E-291
- "Shipping Control – Shipping Info" on page E-293
- "Shipping Control - Packing + Transport" on page E-294

#### Functions menu

This menu allows you to open other dialogs without closing Shipping Control.

##### Shipping group

- **Group orders**: Orders can be collected in groups.
- **Create shipping file**: Saves the shipping list in a file.
- **Resolve shipping orders**: Opens the Delete shipping orders dialog, in which you can remove individual orders from a shipping order.
  - See "Delete Shipping Orders" on page E-296

##### Print group

With the buttons, open the Form/Label Printing dialog in the appropriate print mode. The following print modes are available:
- Shipping labels
- Container list
- Load list
- Packing list

For a detailed description please see the Sales chapter.
- See Sales, "Form/Label Printing" on page C-638

### Shipping Control – Collect

*Production > Shipping control > Shipping > Collect tab*

*Fig. E-145 Shipping - Collect*

Under this tab you collect the orders for a loading list. All orders must be for the same customer.

> **Remove order from the list**
> If you have selected a (wrong) order by mistake, you can remove it from the list in the menu Functions > Resolve shipping orders.
> - See "Delete Shipping Orders" on page E-296

#### Select by

Choose an option to define the criterion for collecting orders. The corresponding fields will be activated.
- **ID/rack number**: Specification of ID number or rack number where the order items are deposited.
- **Order #**: Specification of order number of order reported ready.
- **Storage location**: Select the storage location where the finished order items are deposited.

#### Target

- **Number Manager**: The collected orders are automatically copied to a number manager. When you enter a new name, the number manager will be created.
- **Production preparation**: If you are using production preparations, you can select the preparation to which the orders belong.

#### Orders

The list shows all orders you have compiled.
- **Order**: Order number
- **Item**: Order item number
- **Qty**: Item quantity
- **Weight**: Item weight
- **Width, height**: Width and height of the lites
- **Description**: Product name
- **ID/Rack**: ID or rack number

### Shipping Control – Shipping Info

*Production > Shipping Control > Shipping > Shipping Info tab*

*Fig. E-146 Shipping - Shipping info*

Use this tab to enter details for the loading list for which you have compiled the orders.

#### Shipping details

- **Loading list**: Number of loading list.
- **Truck**: You can select a truck from the list.
- **Driver**: You can select a driver from the list.

#### Shipping text

You can select an existing text or enter your own text. The text will be printed on the loading list.
- **Number**: You can enter the text code or search for the desired text. The selected text can be modified in the display field.

### Shipping Control – Packing + Transport

*Production > Shipping Control > Shipping > Packing + Transport tab*

*Fig. E-147 shipping - Packing + Transport*

This is where you can add a surcharge for packing and/or transport.

#### Surcharge

- **Product**: You can select a surcharge that should be added to all or individual orders on the list. Use the search function to get a list of all products of the product type Services/surcharges.
- **Quantity**: Specification how often the selected surcharge is to be charged.
- **Price/PU, PU**: Specification of the amount per quantity unit and selection of quantity unit to which the amount refers.
- **[Insert]**: Use this button to apply the surcharge to the selected orders. The surcharge will not be calculated if no order is selected.

#### Price view

Surcharges can be shown individually, and/or added to the bill of material.
- **Explicit**: You can also choose the way in which prices are presented.
  - The surcharge will be included in the order item (implicit).
  - The surcharge appears as a separate item.

#### Insert mode

This option defines where the surcharge shall be added. If the surcharge is applied to the edge work, for example, it is useful to add it to the bill of material. If it is applied to a transport insurance, it will be better to show it as a separate item.
- **In BOM**: The surcharge is added to the bill of material. In the case of implicit price view, it is included in the BOM elements.
- **As item**: The surcharge is added to the order as a separate item. In this case, the price view explicit should be selected.

#### Shipping orders

**[All]**, **[none]**: Use these buttons to select all orders to which the surcharge shall be applied, or deselect all orders. The surcharge will not be calculated if no order is selected.

The list shows all orders you have selected on tab Collect.
- **Shipment no.**: Order number for shipping
- **Customer/place**: Customer name and place of business stated in the order
- **Weight**: Total weight of all order items
- **Net amount**: Order total

### Delete Shipping Orders

*Production > Shipping Control > Shipping > Functions menu > Resolve Shipping Orders*

*Fig. E-148 Delete shipping orders*

You can use this dialog to remove individual orders from the list in the Shipping dialog.

#### Document

- **Shipment no.**: Specification of order number from which you want to delete an order. The customer name and his place of business will appear automatically.

#### Documents to be deleted

The list shows all documents belonging to the corresponding shipment number.
- **Shipment no.**: Number of the shipping order
- **Container**: Packaging number
- **Customer order**: Order number acc. to A+W Business
- **Status**: Order status

## Rack Packing List

*Production > Shipping Control > Rack Packing List*

### Functions menu

*Production > Shipping Control > Rack Packing List > Functions menu*

- **Empty table**: Use this menu to delete all entries from the table.

### Rack Packing List (dialog)

*Production > Shipping Control > Rack Packing List*

*Fig. E-149 Rack packing list*

This dialog serves to check the rack load.

#### Selection

This option defines how the list should be displayed.
- **All unprinted**: Only shows racks that have not been printed yet.
- **Rack**: Shows the load of a single rack.

#### Table

The list shows the racks based on the defined settings.
- **Rack**: Rack number.
- **Unit**: Unit if the order item consists of several units.
- **Order**: Order number.
- **Item**: Number of the order item.
- **Qty**: Item quantity.
- **Width, height**: Width and height of the item.
- **Product**: Product number of the item.

## Partial Delivery

*Production > Shipping Control > Partial Delivery*

*Fig. E-150 Overview - Partial delivery*

This dialog can be used to display the orders of a number manager that still show open quantities.

### Identification

- **Client**: If there are different clients, these will be offered for selection.
- **Area**: If there are several production areas, you can select the area to which the orders belong.
- **Employee**: Name of the employee logged in to A+W Business.
- **Number Manager**: If you select a number manager, all orders from this number manager will be listed.

### Output to

This option defines the output type:
- **Printer**: The list will be sent to the printer.
- **Screen**: The list appears on screen.

### Overview

The overview lists all orders from the selected number manager.
- **Document**: Order number.
- **Item**: Item number from the order.
- **Delivery date**: Delivery date.
- **Width, height**: Width and height of the item.
- **Product customer**: The reference number is displayed for customer products.
- **Product number, description**: Number and name of the product in A+W Business.
- **P.O. text/Cust. item**: P.O. text or customer item stated in the order.
- **Qty. original, delivered, open**: Total item quantity plus quantity delivered and quantity open.
- **Status number, description**: Order status.
- **Customer number, name**: Customer name and number.

## Loading Lists

*Production > Shipping Control > Loading Lists*

You can compile loading lists by customer for your forwarder. The recipient of the goods or of the invoice must be the same for all orders.

> **Prerequisite**
> You can only save a loading list if you have chosen a forwarder. Forwarders are defined as 'lorries' in the master data.

This dialog contains the following tabs:
- "Loading List – Shipping Info" on page E-301
- "Loading List - Orders" on page E-303

### Functions menu

*Production > Shipping Control > Loading Lists > Functions menu*

Use this menu to start the printout. The entries are only accessible if the displayed loading list has been saved.
- **Print loading list**: Opens the dialog Form/label printing in print mode Bill of lading. For a detailed description please see chapter Sales.
  - See Sales, "Form/Label Printing - Forms" on page C-639
- **Print labels**: Opens the dialog Form/label printing in print mode Labels. For a detailed description, please see the chapter Sales chapter.
  - See Sales, "Form/Label Printing - Labels" on page C-645
