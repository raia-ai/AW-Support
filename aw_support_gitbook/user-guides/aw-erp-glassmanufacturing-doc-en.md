---
title: "AW_Sales_Tool_2025_1-1-2"
source: "AW_Sales_Tool_2025_1-1-2.pdf"
tags: ["A+W Enterprise", "ERP", "Glass Manufacturing", "Fenestration", "Software Modules", "Business Processes", "Sales", "Purchasing", "Stock Management", "Dispatch"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical overview of the A+W Enterprise ERP system, detailing its integrated modules and business processes for the glass and fenestration industry. It covers core functionalities like Sales, Purchasing, Stock Management, and Dispatch, along with specialized add-ons."
long_description: "This document provides a comprehensive presentation of the A+W Enterprise system, an ERP solution designed for the glass and fenestration sectors. It outlines the various integrated modules that automate and manage key business processes. The presentation begins with a high-level overview of the system's features and technical specifications, such as its 3-tier architecture and multi-site capabilities. It then delves into specific modules, including Sales for order management, Purchasing for procurement, and specialized entry modules like Georgian Bar Entry, Shape Entry, and Processing Entry for detailed product configuration. Further sections explain the logistics modules for Dispatch and Stock Management, highlighting features like status checks, route assignment, and inventory forecasting. The Controlling module is also covered, focusing on margin calculation and workflow management. Each section details the module's primary features, technical specifications, and associated add-ons, illustrated with user interface screenshots."
---

# A+W Enterprise: Integrated Modules & Business Processes

---
## Modules Overview

- **Overview**
- **Sales**
- **Purchasing**
- **Georgian Bar Entry**
- **Shape Entry**
- **Processing Entry**
- **Dispatch**
- **Stock Management**
- **Controlling**
- **Statistics / BI**
- **Extended Workbench**
- **Product Regulation**

### Add-on Modules
- **A+W Capa View**
- **A+W CX Dispatch**
- **A+W ITQE**
- **A+W Excel Import**
- **A+W Enterprise Add-ons**
- **A+W Common Add-ons**

---

## Overview

### Features
- Possibility of multi-site with call centre
- Distribution of quotes and orders to different sites
- Fully automatic handling of group-internal orders between different A+W Enterprise systems
- Mapping of centralized and decentralized company/group networks (branch office structures)
- Fast order processing and fulfilment through automated processes in purchasing, sales, dispatch and warehouse

### Specs
- **Architecture**: 3-tier, possible on Terminal Server
- **Operating system**: MS Windows – User Frontend, Unix - Backend
- **Database**: Informix
- **Reports**: Crystal Reports

---

## Sales

### Features
- Manage all order documents and processes
- Down payments, partial shipments, bulk billing and more
- Graphical order entry (automatic restriction checks dimensions)
- Bill of Material concept with cost calculation
- EDI Import

### Specs
- Up to 400 items per order – no single variety order necessary
- Full control at every level of an item/product
- Definition of supply conditions and prices

### Related Add-ons
- A+W iQuote
- A+W iShape
- A+W Excel Import
- A+W EDI Import & Export

---

## Purchasing

### Features
- Inter-company and external purchase orders
- Automatic purchase orders from orders
- Proposal of purchase orders automatically triggered by stock
- Supplier inquiries, goods receipt with automatic stock bookings
- Control of missing quantities and invoices, statistics and more

### Specs
- Delivery date control
- EDI export of purchase orders
- Definition of supply conditions and prices

### Related Add-ons
- A+W SMC Stock

---

## Georgian Bar Entry

### Features
- Design grid patterns for 1st and 2nd cavity
- Creation of technical drawings
- Complex construction capabilities
- Bars in different colors and variants combinable

### Specs
- Master data for bars must be configured

### Related Add-ons
- A+W CAD Designer Bars

---

## Shape Entry

### Features
- Built-in shape catalog
- Extension of your product-specific shape catalog by free constructions
- Quality improvement based on scaled display for easy control

### Related Add-ons
- A+W iShape
- A+W CAD Designer Shapes

---

## Processing Entry

### Features
- Quality improvement based on scaled graphical display and zoom functionality
- Automatic construction of technical drawings to support all necessary commercial documentation
- Instant availability of all data for subsequent optimization and production control, including optional machine control
- Automatic checking of dimensional restrictions and processing parameters

### Related Add-ons
- A+W ITOE

---

## Dispatch

### Features
- Missing quantity control
- Status check
- Automatic and manual route assignment
- Delivery forecast
- Printout of loading lists, delivery notes and more
- Plant logic for multi-site company (e.g., internal delivery from Site 1 to Site 2, which then dispatches to the end customer)

### Related Add-ons
- A+W CX Dispatch
- A+W Logistic Optimizer

---

## Stock Management

### Features
- Future stock on hand and stock forecasts
- Manual and automatic stock bookings and movements
- Strong interconnection with purchasing and goods receipt
- Stock management and control for main stock components and material
- Management of several stock locations (on site and multi-site)

### Process Flow
1.  **Order Entry / Production**: Stock articles are requested or produced.
2.  **Stock Management Check**: The system checks if the stock is available.
    - If available, it moves to the booking out of stock.
    - If not available, it checks the forecast and identifies a shortage.
3.  **Purchasing**: A stock shortage triggers a purchasing process from a supplier.
4.  **Goods Receipt**: The supplier delivers the goods, which are booked into stock via a delivery note and goods receipt.

### Specs
- Variant and color management
- Stock valuation based on FIFO, LIFO or weighted moving average
- Stock management for homogeneous cases (one size, contains all the same products) and inhomogeneous cases (different sizes, different products)

### Related Add-ons
- A+W SMC Stock
- A+W CX Stock Forecast

---

## Controlling

### Features
- Control of margin calculation with or without production costs
- Status in order entry / dispatch / purchase order
- Internal order status displayed directly in the main order
- Connected to A+W Production to monitor production progress
- Workflow and status management

### Specs
- Lock by item possible
- User rights management
