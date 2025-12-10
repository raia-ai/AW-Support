---
title: "EN_AWBusiness_Production_2-3"
source: "EN_AWBusiness_Production_2-3.pdf"
tags: ["A+W Business", "Production", "Issue of Boxes", "Inventory Management", "ERP", "Software Tutorial", "Rack Management", "Production Preview"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial and software reference guide for the A+W Business Production module. It details procedures for booking the issue of boxes, managing inventory, and using features like rack management and production preview."
long_description: "This document serves as a comprehensive guide for the Production module within the A+W Business software suite. It is divided into two main parts: a 'Tutorial' and a 'Software Reference.' The tutorial section provides step-by-step instructions on 'How to book the issue of boxes,' starting from navigating the menu, loading customer orders, scanning barcodes, allocating boxes with specific IDs, and verifying reservations in the booking journal. It explains the concept of virtual items and how they are updated as physical boxes are allocated. The second part, 'Software Reference,' offers a detailed overview of the Production module's functionalities, including automatic and manual order transfers, configuration settings for production interfaces (like OrderXML and ERP Webservices), and various transfer modes. It also covers related features like Rack Management for tracking company-owned and third-party racks, and Production Preview for analyzing order summaries by delivery date and product type. The document is intended for users who manage production workflows, inventory, and logistics within the A+W Business environment."
---

# Tutorial: Additional Features

---
## How to book the issue of boxes

1.  Go to the menu **Production > Dispatch > Issue of boxes**.
    *(Fig. E-74 shows the "Issue of boxes - load customer order" screen with various selection criteria.)*
2.  Select the option **By scanner**.
3.  Enter the barcode of the order number and item number. The numbers appear in the **Document** fields.
    If you are not using a scanner, choose the option **By order number** and enter the number.
4.  To import order data, select **Start > Execute**. The display switches to the **ID** tab.
    *(Fig. E-75 shows the "Order item with sub-items" screen, displaying a list of virtual items before ID allocation.)*
    
    Each box is shown in a separate line as a virtual item. The fields in column **ID** are empty as no box with an ID has been allocated.

5.  Scan the box ID of the first box to be reserved.
    If you do not use a scanner, go to field **ID** and select one of the displayed IDs. The list only shows box IDs of the defined type.

6.  To allocate the boxes, go to the menu **Start > Execute**.
    The ID is allocated to the first virtual item. At the same time, the line gets a virtual item number. The next line is highlighted.
    *(Fig. E-76 shows a "Sub-item with allocated box ID," where a virtual item number (A) has been assigned and an ID has been allocated (B).)*
    
    The reservation of the dummy box is now deleted and the allocated box with its ID is reserved instead. The two other boxes are still reserved as dummy boxes.
    
    This is shown in the booking journal:
    *(Fig. E-77 shows the "Dummy box reservation updated" in the booking journal, with remaining dummy reservations (A) and the new virtual item with its allocated box ID (B).)*

7.  Repeat steps 5 and 6 to allocate more boxes with IDs.
    *(Fig. E-78 shows the screen with "All boxes allocated".)*
    
    Every box gets a running, virtual item number. All items have thus been allocated a certain box with ID which exists in stock.
    
    These actual boxes are thus reserved in stock; you can check this by means of the booking journal, for example:
    *(Fig. E-79 shows the "Booking journal – reserved boxes" with all three items reserved with specific IDs.)*
    
    The virtual item numbers are saved in the order.
    *(Fig. E-80 shows the "Sub-items in the order" with virtual item numbers 1.1, 1.2, and 1.3.)*

In the **Stock info** dialog, the three boxes are marked as reserved. This tells the user that these boxes cannot be used for another order. The reservations were canceled by the dummy box.
*(Fig. E-81 illustrates the "Reservation updated in stock info," showing the dummy box reservation reset (A), IDs set in receipt boxes (B), and the reservation entered on real boxes (C).)*

Based on the setting, the boxes are withdrawn from stock upon printing the delivery note or invoice. Withdrawn boxes no longer appear in dialog **Stock info**.
*(Fig. E-82 shows a stock info screen where "Withdrawn boxes do not appear in stock info.")*

### Exercises

-   Enter an order that includes boxes.
-   Use the **Stock info** dialog to check the reservation of the box and its contents.
-   Enter the issue of boxes, then check how the stock on hand has changed.

### Additional information

-   Master Data, "Firmendaten - Parameter" on page B-946
-   Master Data, "Virtuelle Positionsnummern verwenden" on page B-953
-   Sales, "Stock Info" on page C-739
-   Software Reference, “Issue of Goods" on page E-236

## Rack Management

You can manage own as well as third party racks with A+W Business. Overviews show the current stock incl. external racks and their return deadlines.

### L-rack load

The additional function, L-rack load, is activated per customer. Own surcharges for L-racks can also be calculated.

Rack and box number have to be determined for the respective customer when using the function. The corresponding order numbers are collected in a Number Manager.

An item can be spread over several L-racks. Please observe the restrictions of the L-racks.

The program determines the start and end number per position.

**Example**
`0101 = Rack 1, Box. 1`
`0315 = Rack 3, Box 15`

The result is entered in the field consignment in the handover file. The start and end numbers are placed in front of the consignment field:
`0101-0421 + consignment field from order (up to maximum field length).`

Labels are then printed for the orders and a list of the L-rack occupation per order. The information as to whether an item can be packaged on an L-rack is also transferred to the form print.

The files are also saved in an ASCII file. The ASCII file name consists of customer number, day, and month.

There are different restriction tests for TPS and non-TPS items. The selection of the items for checking is based on the allocation to the separation article.

The following is checked:

-   **TPS**
    -   Maximum measurement: 1100 x 1700
    -   Max. installation thickness: 26 mm
    -   Number of compartments: 22
-   **Non-TPS**
    -   Maximum measurement: 1080 x 1960
    -   Max. installation thickness: 99 mm
    -   Number of compartments: 21

The text SEPA/ + is transferred to consignment in the event of a restriction violation. If an item cannot be packed on an L-rack, no record is generated.

### Rack management

A+W Business rack management comprises the definition of racks by type and number. Enter the characteristics for each rack (e.g. available, locked, lost, stationary, external rack, number of laths, wheels etc.). Define the rent and the number of free days for the reminder management.

If a rack shall be delivered to a customer, enter the issued racks and the issue date, the number of the delivery note and the customer number. When the rack is returned, booking is managed by means of the date of receipt. Thus, the rack is again available for delivery.

The reminder management allows creation of reminders for any delivered rack. Enter the maximum number of days for which the rack will be required to limit the selection for reminders. The system will automatically produce a list of all customers to print reminders for. A+W Business can differentiate between warning levels.

### External racks

Alongside own racks, you can also manage the racks of customers and suppliers available to you.
You can also save details about locations or unloading sites of (regular) deliveries in the consignment.

### Barcode rack reports

The barcode-labeled racks are scanned prior to despatch and after receipt. This data is imported in A+W Business and booked accordingly. A+W Business thus always has current information as to which racks are once again available for shipping and which are still with the customer.

### Rack history

The occupation of a rack is recorded in the history so that you can track when a rack was delivered to whom and reported back.
You can sort your racks according to type and number in rack management. Shipping and receipt of the racks are documented via booking input/issue.

## Production Preview

The production preview dialog shows the sum of the respective orders by delivery date for the product types insulating glass, single glass, tempered glass and laminated glass. All orders of the present delivery date or later will be analyzed.

50 columns are available per delivery date, which can be set individually. The system administrator defines – company-wide – the contents to be shown in the individual columns. Analysis criteria are a combination of product type and product group. The result can be shown in pieces as well as m².

The visible columns can be set for each product type and extra allocations per work space. The column width can also be adjusted per work space.

### The concept of preview columns

The following combinations can be defined in the column type HP and type 0:

| Combination | Example |
| :--- | :--- |
| Product type / product type | Insulation glass / insulation glass |
| Product type / Product class | Single glass / ornament |

The main product can also be searched for in the bill of materials with the combination of columns type 0 and No. 0.

The combination of columns type 1 and No. 1 searches on the bill of materials level.

| Column | Combination |
| :--- | :--- |
| Type 1 | Type selection on Base 1 BOM level |
| No. 1 | Product type / product group, depending on the type |

A combination of columns type 2 and No. 2 search for a product or process in the BOM, e.g. in LAMI for TGH or single glass, ornament, model etc.

| Column | Combination |
| :--- | :--- |
| Type 2 | Type selection on Base 2, BOM level |
| No. 2 | Product type / product group, depending on the type |

**Example: configuration for evaluation of single glass**

*(Fig. E-83 shows the "Definition for single glass" screen for preview columns.)*

-   **A Type HP:** 1=product type
-   **B HP:** Product type key no. 1=single glass
-   **C ST/QM (illustration of quantity):** 1=piece, 2=square meters
-   **D Type 0:** Search in bill of materials for 1= product type
-   **E No 0:** Product type key no. 1=single glass
-   **F Type 1 (BOM):** 1=product type
-   **G No 1:** Product type Key no. 20-processings

The selection in line 30 is chosen in such a way that all single glasses are shown without further limitation.

The definitions in lines 30 and 31 are only differentiated in the selected measurement for the display (m² / piece).

The selection of single glass in lines 32 and 33 is exclusively limited to ornaments and no further refinements are considered.

The focus of the analysis in lines 33 and 34 is on the processing, and in lines 35 and 36 on the model information.

*(Fig. E-84 shows the "Production preview for single glass" screen.)*

The single glasses in the evaluation are shown per date as a result in the described setting.

# Software Reference

## Overview

The Production module is used to transfer orders to Production as well as for production control and monitoring.

The Software Reference provides information on the following subjects:
-   "Production" on page E-167
-   "Barcode Transfer" on page E-192
-   "Production Data" on page E-197
-   "Logistics" on page E-202
-   "Route List" on page E-203
-   "Status Message" on page E-216
-   "Consignment" on page E-226
-   "List Printing" on page E-233
-   "Shipping of Boxes" on page E-236
-   "Rack Management" on page E-252
-   "Racks" on page E-237
-   "Date Overview" on page E-266
-   "Customs Management" on page E-281
-   "Optimization of Quotations" on page E-289
-   "Shipping Control" on page E-289

The Production module also shows the capacity planning dialogs. These dialogs are described in the section **Capacity planning**.

> **Dialogs are accessible from different points**
> Please note that some dialogs and functions in connection with Production in A+W Business can be started from various other modules. They will only be described once in this document, however. Active cross-references and hyperlinks point out the direct paths to the corresponding descriptions.

### Number manager

-   Production > Production > Number Manager
-   Production > Logistics/Shipping > Number Manager
-   Production > Date Overview > Number Manager
-   Production > Customs Management > Number Manager
-   Production > Optimization of Quotes > Number Manager

The Number Manager dialog is explained in the Sales section.
⇨ Sales, "Number Manager" on page C-629

### Form/label printing

-   Production > Production > Form
-   Production > Shipping > Form
-   Production > Customs Management > Forms

The Form/label printing dialog is described in the Sales section.
⇨ Sales, "Form/Label Printing" on page C-638

### Document data

-   Production > Document data

The Document data dialog is described in the Sales section.
⇨ Sales, "Document Data" on page C-735

### Product info

-   Production > Product info

The Article info dialog is described in the Sales section.
⇨ Sales, "Product Information" on page C-600

### Fax message

-   Production > Fax messages

The Fax message dialog is described in the Overview section.
⇨ Überblick, "Standard-Menüs" auf Seite A-53

## Production

**Path:** `Production > Production`

Production orders can be transferred to production automatically or manually. The orders are usually moved to a number manager and transferred to production by means of the Production transfer dialog. They can also be scanned individually, and transferred by barcode.

> **Automatic transfer**
> Automatic transfer to Production and the query interval have to be defined as formulas in a workflow task.

This chapter provides information on the following subjects:
-   "Transfer to Production" on page E-168
-   "Settings for Transfer to Production" on page E-172
-   "Shape List" on page E-186
-   "Rack Load" on page E-187
-   "Settings (check Rack Load)" on page E-189
-   "Production Data (Dialog)" on page E-197

**Additional information**
-   ⇨ "Barcode Transfer" on page E-192
-   ⇨ "Production Data" on page E-197

### Transfer to Production

**Path:** `Production > Production > Transfer to Production`

*(Fig. E-85 shows the "Transfer to Production" dialog.)*

This dialog is used to transfer the orders from a number manager to production. Transfer is started by [OK]. The data are saved in an XML file which can be imported by A+W Production.

Automatic transfer to Production and the query interval require the definition of a workflow task. This process is explained in the tutorial.
⇨ Tutorial, "Transfer to Production by A+W Business Capacity Planning" on page E-41

> **Quotation transfer**
> Using **Production > Quotation optimization > Production transfer** you can transfer quotations to Production to be optimized. This dialog does not differ from the dialog for transferring orders. The settings for the transfer of quotations have to be set up separately.

#### Functions menu

Use this menu to open other dialogs without closing the current one. The following entries are displayed:

-   **History:** Opens a list of processing steps and status changes for the selected document.
    ⇨ Sales, "History" on page C-550
-   **Settings:** Opens the Settings - Transfer to Production dialog where you can define the settings for the data transfer.
    ⇨ "Settings for Transfer to Production" on page E-172

#### Identification

-   **Client:** If there are different clients, these will be offered for selection.
-   **Area:** If there are several production areas, you can choose the area to which the quotations shall be transferred. This information is used for selecting the number area from which the job number for the transfer shall be loaded.
-   **Employee:** Name of the employee logged in to A+W Business.
-   **Number Manager:** When you have selected a number manager, all orders from this number manager will be transferred that have reached the minimum status.
-   **Mode:** Selection of transfer mode. The following modes are available:
    -   **Transfer to Production:** The orders shown on the list are transferred to production.
    -   **Production release:** The orders shown on the list are released for production and transferred to production.
    -   **Reservation order:** The orders shown on the list are transferred to production in order to reserve capacities in production. The orders are not released for production.
    -   **Cost calculation:** The orders shown on the list are transferred to production in order to determine the material and machine costs. The orders do not occupy any times in production and are not released for production.
    -   **Transfer of non production-relevant changes:** If the orders shown on the list have already been transferred to production, changes to non production-relevant data in the items and orders cannot be transferred after the fact, e.g.:
        -   Changes to customer address, customer and delivery address, changes to the route,
        -   Changes to the file attachments with code for production transfer or the item texts with code for production transfer,
        -   Changes to picking and customer items.
    -   **Cancellation:** The orders shown on the list will be transferred again with a cancellation code. The status of the document is changed to *Transfer to Production canceled*.
        ⇨ Tutorial, "How to cancel the transfer to Production manually" on page E-38

#### Output

This section shows the data on the order currently transferred. The settings for the transfer file are defined in the **Functions menu**:
⇨ "Settings for Transfer to Production" on page E-172

-   **Output file:** Display of path and name of transfer file.
-   **Release:** Transfer file version.
-   **Job number:** Display of the sequential number in transfer to production. This number is loaded from the number area for the section defined in the master data. Splitting the transfer into different areas is useful if you have defined several production sites.
    ⇨ Master Data, "Nummernkreise" on page B-901
-   **Item jobs:** Number of jobs created for the items.
-   **Total, total items:** Number of transferred orders and items.
-   **Order:** Number of the currently transferred order.

#### Orders

The overview shows all orders from the number manager.

-   **Number:** Order number.
-   **Cust./suppl. number:** Customer or supplier number
-   **Customer/supplier:** Customer or supplier name
-   **Status:** Current order status
-   **Prod. date IG, LG, TG:** Scheduled production date for the IG, laminated, or toughened sheet.
-   **Job no. prod. IG, LG, TG:** Number of the job in which the IG, laminated, or toughened sheet has been produced. The number is shown after the report was made.
-   **Delivery date:** Delivery date defined in the order.
-   **Delivery note:** This field is usually blank in this view. It is only filled if delivery notes were printed before the transfer to production was made.
-   **Route:** Name of the delivery route.
-   **Total weight:** Total weight of all order items.
-   **Total quantity:** Total quantity of all order items.
-   **Total sqm:** Total surface of all order items.
-   **Total lin.m.:** Linear meters of all edges.
-   **Input date:** Date on which the order was entered.

#### Export

Click on the first field in the table header in the overview to make further settings for the export.

-   **Write CSV file:** Select this function to save the data from the overview in a CSV file. The storage place can be selected from a dialog.
-   **Options:** This function defines the entries that shall be followed by a line feed.
-   **Write XML file:** This function is used to save the data from the overview in a XML file. The storage place can be selected from a dialog.

### Settings for Transfer to Production

**Path:** `Production > Production > Transfer to Production > Functions menu > Settings`
**Path:** `Production > Quotation optimization > Transfer to Production > Functions menu > Settings`

The settings for the transfer to production are made in the dialog **Transfer to Production - Settings**. The settings are made and saved separately for quotations and orders.

> **Settings per workstation**
> The settings are made per workstation, i.e. individual settings can be made for every user.

This dialog offers the following tabs:
-   "Settings for Transfer to Production - Interface" on page E-173
-   "Settings for Transfer to Production – Transfer Parameters" on page E-176
-   "Settings for Transfer to Production – Additional Interfaces" on page E-183
-   "Settings for Transfer to Production – Text/Attachments" on page E-185

#### Settings for Transfer to Production – Interface

**Path:** `Production > Production > Transfer to Production > Functions menu > Settings > Interface tab`

*(Fig. E-86 shows the "Settings - Transfer to Production - Interface" tab.)*

This tab is used to define the details on the interface by which orders shall be transferred to production.

**Production interface**
The settings for the production transfer file are made here. If you are using the OrderXML format, the production data as well as the data for CAD Designer (Bars) will be saved in the corresponding transfer file. A transfer file is created for every order.

-   **Version:** The data are transferred via OrderXML by default. To create Pool.asc files, first select the version installed on your system. In this case, disable the checkbox A+W Production on the Transfer parameters tab.
    ⇨ "A+W Production" on page E-177

-   **Without ERP Webservice:** The production transfer can optionally be made without files.
    -   ☐ The transfer files are saved by the ERP Webservice.
    -   ☑ The transfer data can be transferred filelessly without the ERP Webservice. With this setting, files can only be transferred with the exchange service. The fields in the AWDesignInterface area and the fields for ERP Webservice are locked.

-   **Fileless export:** The production transfer can optionally be transferred without files. The checkbox is only released if the **Without ERP Webservice** checkbox is checked.
    -   ☐ The transfer files are saved by the ERP Webservice.
    -   ☑ The transfer data is transferred filelessly. With this setting the **Path/File name** field is locked.

-   **Path/File name:** Enter the directory and the file name under which the transfer file should be saved. In connection with the transfer to A+W Production, please make sure that the file is saved in a directory which is monitored by A+W Production. Use the file name OrderXXXX.xml by default; the wildcard (XXXX) will be replaced by the order number and a time stamp.

**AWDesign interface**
This is where the settings for the transfer to CAD Designer (Bars) are made.

-   **Version:** Transfer via OrderXML is used by default.
-   **Path/File name:** Specification of index and file names for the transfer file to CAD Designer (Bars).

**OrderXML**
-   **Version:** Selection of the version of the Order XML interface installed on your system.
-   **ERP Webservice URL:** Web address by which the ERP Webservice is controlled, e.g. `http://localhost/albwir.erp.webservice.2011`. This URL must be entered if you are using OrderXML. This field is locked if checkbox ERP Webservice is checked.
-   **Saving the OrderXML files via ERP Webservice:** With the OrderXML transfer, the transfer file can be saved by A+W Business or the ERP Webservice.
    -   ☑ The transfer files are saved by A+W Business (default).
    -   ☐ The transfer files are saved by the ERP Webservice.
-   **Writing Unicode format:** The transfer data can be written in two different formats.
    -   ☐ The transfer files are written in standard format.
    -   ☐ The transfer files are written in Unicode format.

**Transfer mode**
Choose one of the options to define the mode for the automatic transfer:

-   **After minimum and lock status production transfer:** For automatic transfer to Production, the order status is compared with the minimum and lock status for the transfer to Production. If the order status lies in between, the order is automatically transferred to Production. This is the default setting.
-   **Documents in the capacity planning pool:** With this setting, the orders are transferred to AWCapacity Planning first. When a new order is entered or an order is changed, it goes to the pool for capacity planning. If automatic transfer to Production is active, orders in this pool will be transferred automatically. After the transfer, the order is removed from the pool. This setting locks the transfer for quotation optimization.

You can ignore this setting if transfer is not done automatically. In this case, data transfer is started manually in the **Transfer to Production** dialog from the number manager, considering the minimum and lock status.
⇨ "Transfer to Production" on page E-168
