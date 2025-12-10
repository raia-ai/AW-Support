---
title: "EN_AWBusiness_Box_Management_1_1-1"
source: "EN_AWBusiness_Box_Management_1_1-1.pdf"
tags: ["A+W Business", "Box Management", "Software Tutorial", "Stock Management", "Inventory Management", "Glass Manufacturing", "ERP", "Master Data"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical user guide for the A+W Business Box Management module. This document provides a tutorial on managing boxes of cut glass, including configuration of basic settings, master data, stock principles, and order processing."
long_description: "This document is a comprehensive tutorial for the 'Box Management' module within the A+W Business software, a system designed for the glass, windows, and doors industry. It details the processes for managing boxes of cut glass from stock entry to dispatch. The guide begins with an introduction covering revision history and editorial notes. The core of the document is a tutorial that explains the basic principles of stock management, including stock control, reservations, and BOM consumption. It provides step-by-step instructions for configuring essential 'Basic Settings' such as prices, company data parameters for stock, and status changes. The manual also covers the creation and management of 'Master Data for Boxes,' detailing how to define stock sizes, stock articles, and handle boxes with a Bill of Materials (BOM). The tutorial is intended for end-users familiar with the general concepts of A+W Business and guides them through the specific functions and dialogs required for effective box management."
---

# A+W Box Management
**A+W Business**
A+W - Software for Glass, Windows and Doors

---
## Introduction
This part of the documentation contains editorial notes.

### Revision Overview

| Section | Version/Date | Description |
| :--- | :--- | :--- |
| Introduction | 1.10/012-2019 | Updating the settings in the master data. Transfer of box purchase orders from Purchase part and stock bookings from Production part. |
| | 1.00/012-2018 | Original version box management: Separation from Stock, Purchase and Production parts. |

### Editorial
The editorial provides information on the following topics:
- Notes on this document
- Copyrights
- Trademarks
- Contact

### Notes on this document
This document is intended for end users of A+W Business.

The documentation and software described are licenses that must only be used or copied in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of A+W Business.

### Copyrights
© 2020, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation.

The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without 's prior written approval.

### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. Third party copyrights must be observed.

### Contact
**A+W Software GmbH**

Am Pfahlgraben 4-10  
D-35415 Pohlheim  
Tel: +49 6404 2051 0  
Fax: +49 6404 2051 877  
Email: aw.zentrale@a-w.com  
Web: http://www.a-w.com

## Tutorial

### Overview
The box management tutorial discusses the settings for entering and booking boxes containing cut glass.

> **The functions depend on the enabled modules**
> Please note that the individual functions are only available if the corresponding modules and interfaces have been installed and enabled.
> If you detect functions in this description that are not available in your version, please contact A+W Software GmbH.

**Subjects**
This tutorial includes the following subjects:
- Basic Principles of Stock
- Basic Settings
- Master Data for Boxes
- Orders
- Stock Management for Boxes

**Required knowledge**
The tutorial is meant for those who work with boxes in A+W Business. The participants must be familiar with the concept of master data, sales, and purchasing in A+W Business.

### Documentation
The following documents are available for the Box Management module:

| Format | Volume |
| :--- | :--- |
| PDF | Complete documentation<ul><li>Tutorial</li><li>Software reference</li></ul> |
| Online help `<F1>` | Context-sensitive dialog help of A+W Business software reference and tutorials. |

Additional descriptions are available in the Stock, Purchasing, and Production parts, each of which is available via the online help.

### Tutorial Structure
The tutorial consists of subjects with several training modules each. Each training module consists of the following elements:

**Overview**
Each training module starts with an overview of the major topics:

**Concepts**
First, the concepts and terms of the corresponding training module will be explained.

**Instruction**
The instructions are intended as examples to demonstrate the flow. The names they contain are fictitious.

### Display Conventions
Certain parts of sentences are specially marked. The meanings are:

*Italic*
marks character strings describing the software elements, e. g. the *Stock info* dialog.

**Bold**
marks character strings to be entered via the keyboard, e.g.: Enter the value **0**.

`>`
The so-called breadcrumb trail marks the way to open a dialog, e.g. *Master data > Product > Article > Stock size*.

`[]`
Square brackets mark buttons in a dialog, e. g. [OK] to save the data.

`< >`
Angle brackets refer to keys or shortcuts on the keyboard, e. g. `<F1>` is used to open the online help.

### Menu Overview
This chapter provides a brief overview of the program sections that contain the dialogs that are displayed in this documentation.

**Master data**
- **Stock size:** Use this dialog to enter the boxes with different price keys.

**Stock management**
- **Stock management:** Use this dialog to enter and maintain data for stock articles.
- **Stock movement:** Use this dialog to book goods received and issued, changes of stock locations and opening of boxes.
- **Search:** Use this dialog to check the product availability during a certain time period.

**Production**
- **Goods issues boxes:** Use this dialog to enter stock issue of boxes that are assigned to an order.

**Documents**
- **Goods received:** Use this dialog to enter the boxes that should be included in the inventory.

## Basic Principles of Stock
A+W Business's Stock Management module allows you to manage jumbo sizes, stock sizes, residual plates, boxes, all-glass doors, fittings, frame parts and accessories, such as mirror mountings, sealing tape, etc.

A detailed description of stock is in the Stock Management section. The most important points for box management will be summarized only briefly here.

### Stock control
Before you set up your stock in A+W Business, you have to decide on the basis of how your stocks should be managed: as an area (sqm) or in numbers of pieces. A third possibility is the combined stockkeeping, whereby the size-dependent stock mode is combined with the reports from the optimization so that in addition to the stock dimensions, the stock sizes cut can be booked out automatically.

After deciding about the mode, allocate the corresponding stock code per glass product and define the stockkeeping mode in the company data.

### Stock control mode and reservation
When a product with procurement type Stock Withdrawal is entered in a (production) order, the corresponding quantity (plus waste in the case of fixed sizes) of the stock article is marked as reserved. The reservation can optionally either be booked out of the current stock on hand or automatically when the delivery note or invoice is printed.

These settings are shown in the stock quantities display in dialog *Stock Info* (stock preview) and the automatic purchase order suggestions that can be triggered when minimum quantities are reached.

### Consumption of BOM elements in production orders
For production orders, the consumption of BOM elements in stock can be booked. Boxes then have a BOM if picture frame glass is packed in paper and these paper packages are on a pallet.

> **Example**
> In a production order, LAMI with 2xFloat 3 is entered. After reporting of the production order, the LAMI is booked to the stock, the Float 3 is booked out of the stock.
> If for the same LAMI a normal customer order is entered, only the LAMI is withdrawn from the stock. The Float 3 is not kept in the stock since it has already been withdrawn from the stock by the production order.

### Supplier list
If a box with the identical dimensions is purchased, you must enter the supplier in the supplier list. The supplier is found via the product group that is assigned to the box in the stock dimensions.

### Stock Sizes
The stock size Box is mandatory for stock bookings. For entering a box as an order or purchase order item, a stock article/size called Box must therefore have been created.

If you have created a stock size in the master data, A+W Business provides you with the option to immediately switch to stock management.

Each stock size can be allocated to a separate price table.

If you work with the stock code size-related, you must create stock articles for all stock sizes.

### Stock Management
Every (glass) product is related to a stock size and a stock article.
Each stock article can be created in different variants, e. g. Float 5 mm in several sizes.

In stock sizes (master data), a box can be defined for every product with the procurement type Stock withdrawal, e.g. one box per size.

If there are boxes of the same size but with different numbers of sheets, separate stock articles must be defined for them. To define the exact box article, width and height (among others) are analyzed to determine the minimum stock.

A stock article is therefore required for every box variant, specifying the product number, the size, and the number of sheets.

You can link several stock sizes in stock management by defining a main stock product. The inventory check in *Stock info* dialog is executed only for the main stock product in this case; a minimum stock has to be defined only for this article.

If the stock on hand is not checked for each storage location, a main product must be allocated to determine the available square meters of the glass.

## Basic Settings
In addition to the products and the stock articles, additional setting must be specified so that the boxes can be managed correctly.

This section provides information on the following basic settings:
- "Prices" on page K-16
- "Company Data" on page K-18
- "Status Changes due to Additions and Dispatches" on page K-21
- "Stock Categories" on page K-22

### Prices
Via the price lists for boxes, the prices in purchasing and sales are calculated, e.g. also if individual sheets from a box are sold.

If you want to calculate the glass in boxes with other prices, you must create appropriate price lists for sale and purchase. If you also want to use different glas prices depending on the quantity, additional price lists are also required for this.

The prices are described in detail in the *Master Data* section.

In this example, you see that the prices for the glass in a box are calculated differently, e.g. for the whole box or for a single sheet from the box.

The following conditions must be fulfilled to calculate the average purchase price:
- The product has to be defined also as a stock article.
- The PP code must be set in company data.

#### How to check the master data of your price lists
1. Go to menu *Master data > Prices* and check the settings in the dialogs *Year*, *Key*, and *Rate*. You only need to check the entries used for the prices (and other internal calculations) for stock sizes and boxes.
2. Select menu *Master Data > Prices > Prices*.
3. Please check if all purchase and sales prices have been defined and are up to date, and complete or correct them as necessary.
4. Go to the tab in which the price is defined, check if the purchase price has been entered correctly, and correct it if necessary.
5. Go to menu *Start > Save* to save the data. The data is saved.

### Company Data
In the company data, the settings for the receipt of boxes and stock receipts are specified through production orders. These settings are described in detail in the *Stock management* section.

#### Checking settings for boxes
1. Select menu *Master Data > Company > Company Data*.
2. Switch to the *Parameter* tab and check the settings for the virtual item numbers.
   The virtual item number is necessary for booking the receipt of box items with a quantity of > 1 correctly.
3. Go to the *Stock / PP / EDI* tab.
4. Select the settings for stock P.O.s.
   For the boxes, it is only important how the purchase price should be determined. The settings for determining the purchase price are described in the *Master Data* section.

There are two ways of entering additions to stock based on production orders:
- If the status of the production order exceeds the defined status due to a report from production, the addition to stock is booked automatically.
- If you do not use production reports, you can enter the addition to stock by means of the manual status report in the *Production* module. If you set the production order there to a status above the aforementioned limit, the stock withdrawal of the material consumed and the addition of produced stock articles to stock are booked automatically.

If no other storage location has been defined, the order quantity is allocated to the standard storage location.

5. Select the functions that should be considered when updating the stock on hand in the *Stock Control Mode*.
    - **Reservation w/o stock update:** Enable this option if reserved quantities should not be booked out of the current stock. You must then manually carry out the withdrawal booking. The current stock is therefore not shown at order entry.
    - **Reservation with stock update:** This option is enabled by default so that reserved quantities are booked out from the current stock when the delivery note or invoice is printed.
    - **Stock control on BOM level:** Check this checkbox if products should be managed in the stock even if they are part of a BOM.
    - **Execute stock booking before document printout:** Check this checkbox if stock articles should be booked out before the document is printed. In the event of a problem with the stock withdrawal booking, the order is removed from the documents to be printed and is therefore not printed.
    - **Delete articles with ID if there is no stock on hand:** Boxes with the stock = 0 are no longer present in stock. Enable this checkbox if in the stock management the boxes with the ident numbers from the overview should be deleted for which no inventory is displayed.
    - **Consumption of BOMs in production orders:** If you are working with production orders, you can specify whether the consumption of BOM elements is booked out of stock automatically.
6. Enter the number of workdays.
   The number of workdays is analyzed for the preview in the *Stock Info* dialog. It specifies the time period for which the future stock on hand will be shown.
7. Go to the menu *Start > Save* to save the changes.
   The data is saved. You should restart A+W Business after changing the company data.

> **Status allocation for stock withdrawal booking**
> If you have enabled the option *Execute stock booking before document printout* you should check the status allocation for the stock withdrawal booking. The minimum, assigning and lock status must be organized in a manner that stock withdrawal bookings can be executed prior to printing. If the status allocation does not allow reversal of the order it may be possible that the stock withdrawal booking is not executed.

### Status Changes due to Additions and Dispatches
Goods dispatches and receipts can change the status of documents and result in stock changes due to the status change. If the status points and status allocations are defined correspondingly, this will also apply to partial deliveries.

If you have enabled the option *Execute stock booking before document printout*, the minimum, assigning and lock status must be organized in a manner that stock withdrawal bookings can be executed prior to printing. If the status allocation does not allow reversal of the order it may be possible that the stock withdrawal booking is not executed.

#### Check Status Allocations
A detailed description of stock sizes can be found in the *Stock Management* section.

**How to check the status management**
1. Go to menu *Master data > Order > Status management*.
2. Check whether the user status for stock additions and stock dispatch exists. Create them if necessary. Next, check the status allocations.
3. Select menu *Master data > Order > Status allocation*.
4. Check whether the status allocations of stock addition and stock dispatch for document types *Order* and *P.O.* have been defined:
   - **Stock goods dispatch:** Status *Delivery note printed* or *Invoice printed*
   - **Stock goods receipt:** Status *Goods receipt booked*
5. Create missing allocations and correct existing ones if necessary.

### Stock Categories
The stock categories are allocated to stock articles in the *Stock management* dialog. The stock articles are summed up in groups (stock categories) that can be used as search criteria.

#### Check stock category

**How to define a stock category**
1. Select menu *Master data > Stock > Category*.
2. Go to the menu *Start > New* to switch to the input mode.
3. Enter an ID for the stock category, e. g. figures or names, such as raw material, boxes, production, etc.
4. Go to the menu *Start > Save* to save the data. The data is saved.

## Master Data for Boxes
This chapter contains information about how you create the data in order to differentiate the price calculation for boxes and manage boxes in stock. This includes the definition of the stock sizes and the definition of the stock articles.

This section provides information on the following subjects:
- "Box Data" on page K-24
- "Box with BOM" on page K-29

### Box Data

**Objectives**
- Define stock sizes and stock articles for boxes.
- Define products (articles) for boxes.

**Benefits**
- If the products are defined correctly, pieces and surfaces can be calculated and reserved.
- The display of the actual stock on hand including reservations makes purchasing easier.

**Please note**

**Products**
The products from the master data are used for entry and pricing in documents. They are not automatically kept as stock on hand; this is only the case as a result of additional settings and definitions.

**Stock articles**
All products that are kept in the warehouse with stock quantities must be created as stock articles.

**Jumbo size**
Glass plate as delivered by the manufacturer. It is used to cut the glass pieces for sales.

**Stock plate**
Glass in certain sizes that is actually on hand in the warehouse, e. g. Float 4 mm in 1200 x 1800 mm or 3500 x 5100 mm. Stock plates with defined sizes are also called stock size. Stock plates can be processed as a whole (1200 x 1800). However, it is also possible to use them to cut glass pieces, e. g. 600 x 900 from the plate 1200 x 1800 or from the plate 3210 x 5100.

**Stock size (fixed dimension)**
Sheets defined as stock sizes are sold without being cut. They have special price tables (stock size tables) allocated. A size-related stock article is always also a stock size.

**Stock code (stock booking type)**
The stock code defines whether the stock on hand for an article is evaluated as a surface (sqm) or a quantity (pieces).

**Procurement type**
This code defines the standard way of obtaining a product, e. g. by cutting, stock withdrawal, production, purchase order.

**Default settings**
None

### Define stock sizes for boxes
The stock size *Box* is mandatory for stock bookings. For entering a box as an order or purchase order item, a stock article/size called *Box* must therefore have been created.

#### How to define stock sizes in master data
1. Select menu *Master data > Product > Products > Stock sizes*.
   The *Stock sizes* dialog opens.
2. Go to menu *Start > New* and enter the stock size.
   If you have already defined a corresponding stock article in stock management, enter the same values for width and height.
3. Enter the number of sheets in the box in the *Contents* field.
4. Enter the price code for sales and purchasing.
   You must create an individual stock dimension if you calculate different prices, e.g. for the sale of the entire box, for individual sheets from the box, and/or for the cutting of individual sheets that are removed from the box.
