---
title: "EN_AWEnterprise_Stock_1.01"
source: "EN_AWEnterprise_Stock_1.01.pdf"
tags: ["A+W Enterprise", "Stock Management", "Software Manual", "Inventory", "Warehouse Management", "Glass Industry", "Window Manufacturing", "ERP", "A+W Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is the software reference manual for the A+W Enterprise Stock module, providing detailed instructions on stock management, master data administration, inventory processes, evaluations, and reporting functionalities."
long_description: "The A+W Enterprise Stock manual is a comprehensive guide for end-users of the A+W Enterprise software, specifically focusing on the Stock module. This document outlines the full range of functions required for effective stock management in the glass, windows, and doors manufacturing industry. It covers core processes such as booking stock receipts (warehouse in) and issues (warehouse out) for various stock types including standard, box, slot, stack, and rack stocks. The manual details the procedures for master data management, such as setting up stock rooms and defining article-specific stock limits (minimum, alarm, maximum). It provides step-by-step instructions for conducting inventories, comparing counted stocks with system-booked numbers, and making necessary corrections. Furthermore, the guide explains the evaluation functions for assessing the value of circulating assets and the extensive information system for monitoring stock data through various filters, hit lists, and detailed views. It also touches upon system administration tasks like correcting prices and managing logs, and how to print labels and lists. This reference is essential for users to efficiently manage warehouse operations, plan for incoming and outgoing articles, and maintain accurate stock records."
---

# A+W Stock E

**A+W Enterprise**

*A+W - Software for Glass, Windows and Doors*

---
## Introduction

This section of the documentation contains editorial notes.

### Revision overview

| Section Version / Date | |
| :--- | :--- |
| 1.00 / 01-2016 | English edition. |
| 1.01 / 01-2017 | Product and company names adjusted. |

### Editorial

The editorial provides information on the following topics:

- Notes on this document
- Copyrights
- Trademarks
- Contacts

### Notes on this document

This publication is written exclusively for end users of A+W Enterprise.

The documentation and software described therein are licensed only and must be used or copied only in accordance with the terms of our license agreement. The contents of the documentation are for information purposes only and are subject to changes without prior notice.

The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH assumes no liability for errors or omissions unless these are based on intentional or grossly negligent behavior.

The descriptions in this documentation rely on the full version of A+W Enterprise.

### Copyrights

© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without prior written approval from A+W Software GmbH.

### Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. Copyrights of third parties must be complied with.

### Contacts

**A+W Software GmbH**

Am Pfahlgraben 4-10
35415 Pohlheim
📞 +49 6404 2051-0
📠 +49 6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

## Contents

- **Introduction**
    - Revision overview
    - Editorial
- **Software Reference**
    - Overview
    - Menus in the Stock module
        - Booking menu
        - Master data menu
        - Inventory menu
        - Evaluation menu
        - Info system menu
        - Print menu
        - System menu
        - Additional menu
    - Search Functions
- **Stock Management**
    - Warehouse in
        - Warehouse in - Pieces
        - Warehouse in – Quantity
    - Warehouse out
    - Box warehouse in
        - Box warehouse in - Pieces
        - Box warehouse in - Quantity
    - Box warehouse out
    - Slot warehouse in
        - Slot warehouse in - Pieces
        - Slot warehouse in - Quantity
    - Slot warehouse out
    - Stack warehouse in
    - Modify stack warehouse
    - Rack storage receipt
    - Rack storage exit
        - Rack storage exit - Order related
        - Rack storage exit - Transfer
    - Outgoing stocks (order-related)
    - Correction - Overview
    - Booking correction - Details
- **Master Data Management**
    - Stock room administration
    - Article master data stock
- **Inventory Management**
    - Inventory - Standard stock
    - Inventory - Box stock
    - Inventory - Slots
    - Inventory - Stack stock
    - Inventory - Rack stock
- **Evaluation**
    - Evaluation - Standard stock
    - Evaluation - Box stock
    - Evaluation – Slot stock
    - Evaluation - Stack stock
    - Rack stock evaluation
- **Information System**
    - Info: Stock products
        - Info: Stock products - Filter dialog
        - Info: Stock products - Hit list
        - Info: Stock products – Hit list details
    - Info: Stock variants
        - Info: Stock variants - Filter dialog
        - Info: Stock variants - Hit list
        - Info: Stock variants - Hit list details
    - Info: Stock slots
        - Info: Stock slots
        - Info: Stock slots - Hit list
        - Info: Stock slots - Hit list details
    - Info: Stock racks
        - Info: Stock racks - Filter dialog
        - Info: Stock racks - Hit list details - General
        - Info: Stock racks - Hit list details
    - Info: Stock stacks
        - Info: Stock stacks - Filter dialog
        - Info: Stock stacks - Hit list
        - Info: Stock stacks - Hit list details
    - Info: Stock sheets
        - Info: Stock sheets - Filter dialog
        - Info: Stock sheets - Hit list
    - Info: Stock history
        - Info: Stock history - Filter dialog
        - Info: Stock history - Hit list
        - Info: Stock history - Hit list details
    - Orders/Purchase Orders
        - Orders/Purch. Orders - Filter dialog
        - Orders/Purch. Orders - Hit list
        - Orders/Purch. Orders - Hit list details
    - Booking Status
        - Booking Status – Unbooked
        - Booking Status – Error
        - Booking Status - Inventory
        - Booking Status – Correction
    - Stock Information - Pick list
    - Stock Information - Hit list
    - LVR Status
    - Range - Stock Forecast
    - Range - Hit list
    - Available stock
    - Stock forecast
- **Print**
    - Print labels for boxes
    - List printing
- **System Administration**
    - Delete stock log
    - Stock price correction
- **Service Functions**
- **Section index**
    - Index

## Software Reference

### Overview

In the Stock module, you have all functions that are required for successful stock management, e.g. stock maintenance, stock bookings, inventories, as well as the planning of incoming and outgoing articles. All prices are specified as net prices in this module.

The Stock section covers the following topics:

- "Stock Management" on page E-15
- "Master Data Management" on page E-49
- "Inventory Management” on page E-53
- "Evaluation" on page E-64
- "Information System" on page E-71
- "Print" on page E-115
- "System Administration” on page E-118
- "Service Functions" on page E-120

### Menus in the Stock module

The dialogs of the Stock module have the following menus:

- "Booking menu" on page E-9
- "Master data menu" on page E-10
- "Inventory menu" on page E-10
- "Evaluation menu" on page E-11
- "Info system menu" on page E-11
- "Print menu" on page E-12
- "System menu" on page E-12

### Booking menu

The first level of the Booking menu includes the following entries:

- **Warehouse in:**
    - "Warehouse in" on page E-16
- **Warehouse out:**
    - "Warehouse out" on page E-22
- **Boxes in:**
    - "Box warehouse in" on page E-23
- **Boxes out:**
    - "Box warehouse out" on page E-28
- **Slots in:**
    - "Slot warehouse in" on page E-29
- **Slots out:**
    - "Slot warehouse out" on page E-34
- **Stack management:**
    - Customer-specific functions will be explained in detail in a separate section.
- **Stack in:**
    - "Stack warehouse in" on page E-35
- **Stack modification:**
    - "Modify stack warehouse" on page E-36
- **Rack receipt:**
    - "Rack storage receipt" on page E-38
- **Rack shipment:**
    - "Rack storage exit" on page E-40
- **Stack booking (doc.rel.):**
    - Customer-specific functions will be explained in detail in a separate section.
- **Outg. Stocks (order-rel.):**
    - "Outgoing stocks (order-related)" on page E-44
- **Correction:**
    - "Correction – Overview" on page E-46

### Master data menu

The Master data menu includes the following entries:

- **Location:**
    - "Stock room administration" on page E-50
- **Article:**
    - "Article master data stock" on page E-51
- **Slots:**
    - Customer-specific functions will be explained in detail in a separate section.
- **Stack types:**
    - Customer-specific functions will be explained in detail in a separate section.

### Inventory menu

The Inventory menu includes the following entries:

- **Stock:**
    - "Inventory - Standard stock" on page E-54
- **Box stock:**
    - "Inventory – Box stock" on page E-57
- **Slot stock:**
    - "Inventory - Slots" on page E-59
- **Stack stock:**
    - "Inventory - Stack stock" on page E-60
- **Rack stock:**
    - "Inventory - Rack stock" on page E-61

### Evaluation menu

The Evaluation menu includes the following entries:

- **Stock:**
    - "Evaluation - Standard stock" on page E-65
- **Box stock:**
    - "Evaluation – Box stock" on page E-67
- **Slot stock:**
    - "Evaluation – Slot stock" on page E-68
- **Stack stock:**
    - "Evaluation - Stack stock" on page E-69
- **Rack stock:**
    - "Rack stock evaluation" on page E-70

### Info system menu

The first level of the Info system menu includes the following entries:

- **Article:**
    - "Info: Stock products - Filter dialog" on page E-72
- **Variant:**
    - "Info: Stock variants – Filter dialog" on page E-75
- **Slot:**
    - "Info: Stock slots" on page E-80
- **Rack:**
    - "Info: Stock racks - Filter dialog" on page E-83
- **Stack:**
    - "Info: Stock stacks - Filter dialog" on page E-87
- **Sheet:**
    - "Info: Stock sheets - Filter dialog" on page E-90
- **History:**
    - "Info: Stock history - Filter dialog" on page E-93
- **Orders/Purchase orders:**
    - "Orders/Purch. Orders - Filter dialog" on page E-98
- **Booking status:**
    - "2nd level menu - Booking status" on page E-12
- **Order list:**
    - "Stock Information - Pick list" on page E-108
- **Status:**
    - At present, this dialog is not used.
- **Range:**
    - "Range - Stock Forecast" on page E-110
- **Available stock:**
    - "Available stock" on page E-112
- **Forecast:**
    - "Stock forecast" on page E-113

#### 2nd level menu - Booking status

- **No booking:**
    - "Booking Status - Unbooked" on page E-102
- **Error:**
    - "Booking Status – Error" on page E-104
- **Inventory:**
    - "Booking Status - Inventory" on page E-105

### Print menu

The Print menu includes the following entries:

- **Labels:**
    - "Print labels for boxes" on page E-116
- **List printing:**
    - This dialog is described in the Sales section.
    - Sales, "List printing" on page D-162

### System menu

The System menu includes the following entries:

- **Delete stock transcript:**
    - "Delete stock log" on page E-119
- **Price correction:**
    - "Stock price correction" on page E-119

### Additional menu

`<F4>`
The Additional menu includes the following entries:

#### 1st menu level

- **PCD prices:**
    In the warehouse ins, you can assign articles pre-defined prices via price codes. You can select the price codes from a pre-defined list.
- **Booking - no Price:**
    In the warehouse ins, you can assign articles the price = 0.
- **Trans.bookings:**
    Transfer selected data record to another stock. The booking must be completed with [OK].
- **Contract book.:**
    Assign selected data record to an object (e.g. construction site).
- **Boxes:**
    - "2nd level menu - Boxes" on page E-13

#### 2nd level menu - Boxes

- **Book box:**
    Removes the box of the current data record from the box stock and books the articles of the box automatically into the normal stock. The booking must be completed with [OK].
- **Resolve box:**
    Removes the box of the current data record from the box stock and books the articles into a target stock. The booking must be completed with [OK].
- **Single sheet information:**
    - "3rd level menu - Individual sheet information" on page E-13

#### 3rd level menu - Individual sheet information

- **Display:**
    - "Footer area individual sheet information" on page E-25
- **Edit:**
    - "Footer area – individual sheet information" on page E-25

## Search Functions

You can search for information via the search functions, e.g. about articles, stock types, orders or purchase orders.
- "Information System" on page E-71

## Stock Management

In the stock management, you record and edit the bookings for the goods warehouse, e.g. warehouse in receipts for articles or booking corrections.
This section explains the following dialogs:

- "Warehouse in" on page E-16
- "Warehouse out" on page E-22
- "Box warehouse in" on page E-23
- "Box warehouse out" on page E-28
- "Slot warehouse in" on page E-29
- "Slot warehouse out" on page E-34
- "Stack warehouse in" on page E-35
- "Modify stack warehouse" on page E-36
- "Rack storage receipt" on page E-38
- "Rack storage exit" on page E-40
- "Outgoing stocks (order-related)" on page E-44
- "Correction - Overview" on page E-46
- "Booking correction – Details" on page E-47

### Warehouse in

**Booking > Warehouse in**

On this dialog, you record and book the stock receipts for the stock articles of the selected stock.

This dialog offers the following tabs:

- "Warehouse in – Pieces" on page E-16
- "Warehouse in – Quantity" on page E-20

#### Warehouse in – Pieces

**Booking > Warehouse in > Pieces**

_Fig. E-1: Warehouse in – pieces_
