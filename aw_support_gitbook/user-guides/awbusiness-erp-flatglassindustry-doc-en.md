---
title: "EN_AWBusiness_Overview_5.21"
source: "EN_AWBusiness_Overview_5.21.pdf"
tags: ["A+W Business", "ERP", "Flat Glass Industry", "Software Documentation", "Order Processing", "Production Planning", "Stock Management", "Capacity Planning", "A+W Software GmbH"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a comprehensive overview of A+W Business, a modern ERP system designed for the flat glass, windows, and doors industry. It details the software's features, modular structure, and core capabilities, including master data management, order processing, production planning, stock management, and capacity planning. The guide is intended for end-users to understand the system's architecture, functionality, and how it integrates with other A+W applications to streamline business processes from sales and purchasing to production and dispatch."
long_description: "This is an in-depth overview of the A+W Business software, an Enterprise Resource Planning (ERP) system from A+W Software GmbH, specifically tailored for the flat glass, windows, and doors manufacturing sector. The document serves as a user guide and technical reference, starting with an introduction that covers revision history, copyright information, and contact details. It then moves into a detailed tutorial section explaining the system's features, architecture, and modular structure. Key topics include master data management (products, partners, BOMs), document handling (quotations, orders, purchasing), and production control. It describes how A+W Business supports automated processes like credit limit checks, form printing, and data transfer to production systems. The document also covers advanced modules and integrations, such as A+W Business Pro (Production Manager), A+W Business Capacity Planner, A+W Discovery for business intelligence, and route optimization for shipping. It provides guidance on working with the software, including navigation, standard functions, and hotkeys. The document is designed to help end-users leverage the full scope of A+W Business to manage complex commercial and administrative processes efficiently, from initial quotation to final invoicing and analysis."
---

# A+W Business Overview

**A+W - Software for Glass, Windows and Doors**

---
## Introduction

This part of the documentation contains editorial notes.

### Revision Overview

| Version/Date | Description |
| :--- | :--- |
| 1.00/03-1998 | Original version |
| 1.10/08-2000 | Revision |
| 1.20/04-2001 | Revision |
| 2.00/12-2003 | Structural conversion to program structure 4.0 |
| 3.00/12-2007 | Revision |
| 3.01/08-2008 | Illustrations updated |
| 3.02/09-2010 | Layout adapted to documentation concept 2010 |
| 4.00/08-2013 | Adaptation of ALFAK documentation to A+W Business. |
| 5.00/05-2014 | Complete revision of the part Overview |
| 5.01/07-2014 | Update of expansion stages |
| 5.20/11-2015 | List of hotkeys for document entry added. |
| 5.21/01-2017 | Product and company names adjusted. |

### Editorial

This editorial provides information on the following topics:
*   Notes on this document
*   Copyrights
*   Trademarks
*   Contact

#### Notes on this document

This document is intended for end users of A+W Business.

The documentation and software described are licenses that must only be used or copied in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of A+W Business.

#### Copyrights

© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

#### Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. Third party copyrights must be complied with.

#### Contact

**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
📞 +49 6404 2051-0
📠 +49 6404 2051-877
📧 zentrale@a-w.com
🌐 http://www.a-w.com

## Tutorial

### Overview

A+W Business is a modern ERP system with the purpose to concentrate on the requirements and demands of the flat glass industry. A+W Business supports the input of documents within the scope of sales and purchasing and enables control of related sectors and processes, e.g. stock management, capacity planning, shipment, etc.

Quotations, order processing, purchasing, dispatch and invoicing can be controlled and monitored easily and efficiently with A+W Business.

A+W Business is incorporated in the product portfolio of A+W Software GmbH and communicates with the respective products. Overall, the product portfolio of A+W Software GmbH looks as follows:

**Fig. A-1: Product portfolio**
This overview shows the products of A+W Software GmbH with their respective core capabilities. The portfolio is structured into the following main categories:
*   **ERP (Enterprise Resource Planning):**
    *   ERP Solution: A+W Enterprise, A+W Business
    *   Core Capabilities: Sales, Purchase, Stock, Dispatch, Statistics, eCommerce
*   **PPS (Production Planning System):**
    *   PPS Solution: A+W Production, A+W Business Pro
    *   Core Capabilities: Capacity Planning, Production Planning (Rough- and Detailed Scheduling), Cutting Optimization
*   **Machine Control:**
    *   Control Units: Production Terminal, Realtime Optimizer, Rack Optimizer, DynOpt
    *   Core Capabilities: Monitoring, Controlling, Barcoding
*   **Machines:**
    *   Examples: Cutting Line, IG Line, Lamy Line
*   **Production Monitoring:**
    *   Controlling & Monitoring: A+W Production Cockpit, A+W Dashboard
*   **Additional Tools:**
    *   CAD Construction: CAD Designer
    *   Statistics & Analyses: A+W Discovery

#### Distinguishing A+W Business from A+W Enterprise

A+W Software GmbH offers two commercial software solutions: A+W Business and A+W Enterprise. Both systems fulfil the requirements of the flat glass industry in the commercial/administrative sector. Their deployment depends on the company size and structure:

*   **A+W Business** is designed for individual companies or company groups acting like individual companies. The system is based on a modern Windows-based 2-layer architecture on an MS SQL server database.
*   **A+W Enterprise** has been designed for larger companies with a distinct subsidiary structure. The system is based on a UNIX/LINUX-based 3-layer architecture on an Informix database.

#### Features of A+W Business

With its fully graphical interface, A+W Business can be operated easily and quickly and simplifies company-internal processes around order processing.

**Ergonomics, Transparency and Clear Arrangement**

A+W Business is a multi-dialog application:
*   Several dialogs, e.g. quotation, order and master data dialogs, can be opened and edited at the same time.
*   The dialogs can be positioned where desired and can be scaled steplessly.
*   With an editor, documents and reports can be easily and quickly formatted and adjusted to the requirements of your company.

**Main Functions**
*   Master data management
*   Quotations
*   Order processing, including creating partial deliveries and complaints
*   Creating all commercial documents e.g. order confirmation, delivery note, etc.
*   Route planning and optimization
*   Stock management
*   Integrated production planning and control, e.g. capacity planning, rough scheduling, detailed scheduling, optimization, barcoding.

#### Automation for Sales Documents

The system provides comprehensive technical support in processing orders and quotations.
*   Entered elements are displayed true to scale and represented graphically in order to prevent errors during input and to accelerate the entire process.
*   Pricing is very flexible and allows for versatile division into standard prices and customer-specific conditions. The calculation is controlled on a system-wide basis and can also be adjusted manually.
*   Delivery notes and invoices are created from the order data in accordance with configurable settings.

#### Connection to further Applications

The A+W Business package can be supplemented by further applications:
*   EDI solution for the electronic exchange of orders and invoices
*   Extended CAD functions
*   Internal rack management
*   Microsoft Outlook connection
*   Interface to various financial accounting and document management systems
*   Analyzes in the form of reports and statistical reports
*   Extended production monitoring and control by connection to the Premium PPS-System A+W Production
*   Microsoft Sharepoint connection for integrated document management and archiving

### System Environment

Special attention was paid to the below areas in order to meet the basic requirements of a high-performance IT system:
*   Operational security
*   System availability
*   Supported hardware platforms
*   Extensibility
*   Networking options
*   Access restriction and control

Due to its client/server architecture, A+W Business can be adjusted and extended step-by-step to meet operational requirements.

**Fig. A-2: 2-layer architecture**
A diagram shows a 2-layer architecture.
*   **Client PC (Windows):** Contains the "Logic and display layer". Multiple client PCs are shown connecting to the server.
*   **Server:** Contains the "Data layer", represented by a database cylinder.

#### System Architecture

A+W Business is based on Windows operating systems and can be run on modern Microsoft client/server systems.

The system can be adjusted to accompany requirements very flexibly due to the clear separation of data management, data processing and the user interface in the 2-layer architecture. As a result, it is possible to add more performance to computers in the application layer when the number of users increases without having to change the databases and settings on the user PCs.

For data management, the relational MS SQL server database is deployed. The underlying data model can be viewed via an online documentation. This serves in particular the extensibility and the option to create reports and statistical reports quickly and efficiently.

A+W Business supports you with easy-to-use tools and integrated standard functions, such as Crystal Reports.

A+W Business can be integrated into the existing network topology. Interfaces to email, fax and telephone system are integrated parts.

### Data Security

The application is transaction-protected. This means that the program will fully complete actions, e.g. when invoices are created. If this is not possible, a started action is completely aborted. This precludes that the database is filled with errors or data fragments. The components that are being deployed allow that the data is completely and consistently recreated even in the event of a system crash. The backup runs automatically at a definable time or parallel to running operations.

### User Interface

A+W Business runs on a fully graphical user interface on Windows platforms. With it, the functions of the daily business are intuitively operable.

### Access Rights

The A+W Business basic version includes the management of access rights: You can define which programs may be run for each individual user or for user groups.

You can define detailed access rights using rights management, e.g. the right to read, but not change data.

By default, A+W Business is delivered with four predefined employee groups. You can create additional groups and profiles, e.g. to withdraw rights or additionally allocate them. This might be useful, e.g. for employees from production who only require production-relevant information from A+W Business, but who may not change any data.

### Maintenance and Support

Each A+W Business installation includes a high-performance support concept. Support includes regular updates that are sent via the network and are installed outside of the regular operation hours. Maintenance is always performed via network linking so that data transfer can take place simultaneously. This enables a very effective support.

By means of the A+W Premium Maintenance and Service Agreement Value+ you can also access a multitude of documents, best-practice training courses, and tips and tricks – and it's free.

Of course, we also offer these premium services specifically adapted to your individual requirements.

### Modular Structure

The modular structure of A+W Business allows for a flexible mapping and control of the complex business processes in your company.

**Fig. A-3: Overview of Modular Structure**

This simplified overview shows the interaction between the different modules in the A+W Business Modular system.

*   **Core Module: Master Data**
    *   Basic data, partners, products, product groups, prices, terms, access rights.
    *   Connects to: Orders, Stock.

*   **Sales & Quoting**
    *   **Quotations:** Input/processing, conversion into order, printing of standard forms, alternative quotes. Feeds into **Orders**.
    *   **Orders:** Input/processing, printing of standard forms, copying of documents, partial shipment, complaint orders. Feeds into **Route optimization**, **Production**, **Purchasing**, **Invoices/credit notes**, and **Archive**.

*   **Planning & Production**
    *   **Capacity planning:** Master data, order scheduling, purchase price updates, overviews, transfer to production. Interacts with **Production**.
    *   **Route optimization:** Route calculation, loading, delivery times, cost calculation. Feeds into **Dispatch**.
    *   **Production:** Production overview, shipment, transfer to production, Production manager. Receives data from **Orders** and **Capacity planning**. Reports breakage on the shop floor. Feeds into **A+W Production**.
    *   **A+W Production:** Networked production. Feeds back into **Production**.

*   **Logistics & Fulfillment**
    *   **Dispatch:** Shipment, partial shipment, printing of delivery notes. Receives data from **Route optimization**. Reports breakage during shipment. Feeds into **Rack management**.
    *   **Rack management:** Manages racks. Feeds into **Invoices/credit notes**.
    *   **Invoices/credit notes:** Printing of invoices/credit notes. A **Partial shipment** can loop back to the **Orders** module. Feeds into **Transfer to FinAcc** and **Archive**.

*   **Purchasing & Stock**
    *   **Stock:** Stocktaking, inventory management, stock movements, transfer to purchasing, inventory statistics.
    *   **Purchasing:** Enquiries/purchase orders, dispatch via standard email/fax/RDT, goods received bookings, invoice checks, purchase price updating. Receives data from **Orders** and **Stock**.

*   **Post-Processing & Archiving**
    *   **Transfer to FinAcc:** Transfers financial data.
    *   **Statistics:** Sales / Purchasing.
    *   **Archive:** Quotations, orders (invoices), credit notes, enquiries, purchase orders.
    *   **Deletion of documents.**

*   **Software Tiers:**
    *   **A+W commercial software:**
        *   Basic version - Sales
        *   Supplement
    *   **A+W production software**

## A+W Business Modules

A+W Business distinguishes between master data and transaction data:
*   **Master data** is entered and is rarely changed afterwards.
*   **Transaction data** relates to the commercial processes and change depending on the entered document.

The continuous data exchange always ensures up-to-date information between the modules.

The basic version Sales offers the option to enter and process customer inquiries and orders, all the way to archiving.

With supplemental modules, you can extend the processing of commercial documents relating to purchase orders, stock management and various interfaces, e.g. for electronic data exchange with customers and suppliers, or for Production, etc.

**Fig. A-4: Program interface with modular structure**

The program interface screenshot shows a navigation pane on the left with the following main modules:
*   **A Master data:** Creating and maintaining master data, e.g. product management, market partners.
*   **B Documents:** Entering and processing commercial documents, e.g. orders, quotations, purchase orders, printing the commercial documents.
*   **C Production:** Transferring the order items to capacity planning, and production and checking of the production status.
*   **D Statistics:** Analysis of the commercial processes according to different criteria.
*   **E Inventory Management:** Managing and acquiring the stock for the material warehouse.
*   **F Capacity planning:** Managing master data for capacity planning.
*   **G Utilities:** System-wide settings for data exchange.

### Master Data

The organization and maintenance of master data is the basis of A+W Business and its modules. Master data is transferred to all areas of the system: All business areas access the same master data, e.g. customers, products, prices, status, and currencies.

You define common parameters for your company or per client of your company in the company data.

Interfaces are used to transfer master data to other programs, e.g. to A+W Production.

**Fig. A-5: Master data**
*   **A: Program areas of the Master Data module:** Shows the navigation tree for Master Data including General, Products, Prices, Stock, Partner, etc.
*   **B: Example: Customer master data:** Shows the main window for editing a specific customer's data, including address, contact info, delivery terms, and financial details.

#### Basic Data

Basic data includes, e.g. number areas and status management. Status management allows you to handle your business processes in A+W Business. You are able to reflect your internal processes and work processes by assigning status, minimum status and lock status.

#### Partners

Partner management distinguishes between customers, suppliers, and other partners. For all partners, you define additional parameters in addition to the addresses. These parameters make the input of quotations and orders easier, e.g. delivery route, alternative rounding, staff and subsidiaries, payment terms, projects.

The integrated export function allows you to export your customer data to Microsoft Word for creating serial letters.

#### Products

In A+W Business, you can map your company's product structure. In A+W Business, product relates to everything that is to be executed as a separate item in the order. The result is that processing steps, down-payments and surcharges, or all-glass systems are created as products, the same as IG units or single glass.

You can define any kind of article number, as well as alphanumerical match codes.

#### Bill of Material (BOM)

A product can consist of several products, e.g. an IG pane with two pieces of glass, a frame and a round shape. These components constitute the bill of materials. Every single component is a product itself.

You can thus design your products in a way that entry as an order item is mostly automated.

The following functions are based on the bill of material:
*   Price calculation
*   Product names in documents, e.g. on the order confirmation.
*   Inventory management planning
*   Organization of production control
*   Production time calculation

**Fig. A-6: BOM component of an IG product (order)**
A diagram shows a hierarchical breakdown of an Insulating Glass (IG) unit.
*   **A Main product:** IG (e.g., 724 / IG 4/16/Th4 A+W)
*   **B 1st component:** Float glass (e.g., 104 / Float 4 mm A+W)
*   **C 2nd component:** Spacer with gas (e.g., 716 / Spacer 16 mm ALU A+W, 796 / Argon A+W)
*   **D 3rd component:** Heat-protection glass (e.g., 134 / Therm 4 mm A+W)
*   **E 4th component:** Shape (e.g., 8001 / Schräge Kante (rechts) MODELL)
*   **F 5th component:** Step (e.g., 8999 / Stufung (Außenansicht))

BOM components can be individual products as well as processing steps or further bills of material, so-called assemblies. All BOM components have to be entered as products in master data.

The BOM breakdown options are unlimited: Multiple IG, multiple LG or TG can be kept in BOM format. With A+W Business, it is even possible to consider different conditions for price calculation for each component of a BOM.

#### Variants

Since the program distinguishes article variants for the products, Float 4 mm exists only once, for example. All variants of Float 4 mm are kept under the same number, and will be automatically recognized at order entry. These variants can relate to stocksizes, fixed dimensions, boxes, units, colors, etc. Each variant can be assigned to another product group.

#### Muntins

In A+W Business, muntins are usually created for cavity (spacer) and divided by construction types. All muntins, connecting pieces and edge felts are created as a product so that they can be entered in the order.

Muntins can be entered symmetrically or asymmetrically with reference to the fields or drill points.
*   You can enter individual sizes for muntin construction so that drill holes or fields are arranged asymmetrically.
*   In case of automatic calculation, you can define whether the symmetry shall be related to the drill holes or to the fields.

**Fig. A-7: Symmetrical calculation of grill pattern**
Two diagrams compare a "Drill hole-symmetrical" muntin pattern with a "Field-symmetrical" pattern, showing how the internal divisions are calculated based on different reference points.

#### Shapes

For entering shapes, the A+W Business standard version offers the A+W shape catalog. The shape specifications from the catalog are created without dimensions and glass as products. In the order item, you assign a glass product with a non-rectangular shape from the shape catalog and supplement the requested dimensions.

**Fig. A-8: Schematic layout of a shape**
*   **A Shape with wildcard sizes:** A diagram of a shape with placeholder dimensions (e.g., W[600], H1[250]).
*   **B Shape sizes in the order:** The same shape diagram updated with specific order dimensions (e.g., W 1200, H 1800, H1 900).
*   **C Shape number:** The unique identifier for the shape in the catalog (e.g., 8002).

Initially, shape 2 (C) is shown without sizes (A). The display is updated after the item sizes have been entered (B).

You can also enter your shapes using the shape catalog of Bystronic or Billco.

#### Organization of Product Groups

All products are assigned to product groups. These are divided into the three levels of the main product group, product superior group, and product group.

In addition to these levels, you are able to define combinations of product groups. Furthermore, to each product group level, TOP product groups can be allocated.

**Fig. A-9: Hierarchic product group structure**
A screenshot shows a tree view of product groups.
*   **A MPG: Main product group** (e.g., 2** Float)
*   **B SPG: Product superior group** (e.g., 20* Float klar / clear)
*   **C PGR: Product group** (e.g., 200 Float 2-10 mm FM/CTS)
*   **D MPG with alphanumerical number** (e.g., T** Training)

The main product group 0**, superior product group 00*, and product group 000 are fixed. All other product groups can be numbered according to your own rules.
*   The **main product group (MPG)** serves for discount allocation and statistical analysis.
*   The **superior product group (SPG)** serves for discount allocation and statistical analysis.
*   The **product group (PGR)** serves for discount allocation, product organization, and statistics. Products can be allocated only to this level.

If you are working with a program for financial accounting, the accounts are allocated via the product groups.

### Prices and Surcharges

No other industrial sector has such complex price calculation mechanisms like the flat glass industry. Since we cannot change these mechanisms, we have made the maintenance and administration of price lists and tables as easy as possible.

For this reason, price calculation in A+W Business consists of flexible modules, covering all methods of price calculation. Price matrixes can be used for merchandise as well as for IG. Standard price lists can be imported, as well as exported.

For each product, you assign the requested price table, surcharges and statutory tax rate.

**Fig. A-10: Product management - Price/surcharge**
A screenshot of the product pricing setup screen with labeled sections:
*   A Tax rate
*   B Automatic surcharges
*   C Cost accounting details
*   D Price view
*   E Price tables
*   F Surcharges
*   G Rounding for pricing purposes
*   H Price code

Prices and surcharges can be defined as standard or individually for customers or customer groups:
*   **Prices:**
    *   Matrixes, e.g. for insulating glass, patterned glass
    *   Vectors, e.g. graduation by quantity per order
    *   Unit prices, e.g. for single glass
    *   Price cubes, e.g. for grinding matrixes
*   **Surcharges for the main product:**
    *   Muntin surcharges
    *   Shape surcharges
    *   Group/replacement surcharges
*   **Other surcharges, e.g.:**
    *   **Special discounts and price surcharges:** By default, special discounts and price surcharges are integrated. In addition, another eight special discounts are available and you can use them as desired. For these discounts, you can specify a validity duration and then use them for special promotions.
    *   **Energy surcharge:** With the help of this energy surcharge, you can pass along energy costs that were added to the glass price by the glass factory to your customers. Surcharge, either only on the glass weight, or on the entire weight of the glass items. Price per kg/lbs. Adjustable per customer and document. Surcharge as a separate item, or split onto all glass items. Automatic updating of the energy surcharge after a change to the document.
    *   **Transport/toll costs:** Calculation per kilometer of distance, distance available as a quantity limit in price management (minimum price, maximum price).
    *   Surcharges for cavity, small glass/oversizes, minimum quantities, thickness.

#### Preparing a new price list – made easy

Price management includes the option to copy the prices completely or partially, and to change them absolutely or proportionally: If you have to introduce completely new prices for the next year, you can prepare them without rushing. Just copy the price tables to the new price lists and change the prices. Activate these price tables in the Rates dialog only when day X has arrived on which the prices are valid. The new prices are transferred to every new order immediately.

#### Automatic Price Calculation

Apart from a convenient maintenance of the price data, automatic calculation of the prices is important. It does not matter if it is standard or individual prices or surcharges that are added to the basic price: All information for calculating the items is automatically used without you having to think about it. And of course, you are also able to manually override every price in a quotation or order without the data being transferred back to the price tables.

### Discounts

The tree-shaped discount overview gives a clear view of the existing discount rates.

Discounts can be granted in general for a product or per customer/supplier. You can combine customers or suppliers for whom the same price and discount conditions apply in customer or supplier groups, which makes the maintenance of discounts significantly easier.

You can maintain different discounts:
*   Standard discounts for a price list and a price key (rate)
*   Graduated discounts with a quantity limit
*   Exchange discounts

A discount is automatically applied to the order when the product is entered. If no discount has been defined, a percentage can be entered in the order. This manual discount can either be entered in the order header for the whole order, or at item entry for an item or a BOM component.

You can create a global discount for the different product group levels or for combinations of product groups. Product group combinations for discount rates may differ from those in statistics.

### Documents

Transaction data includes all data of commercial processes and stock management.
*   Commercial processes are entered and monitored in documents, e.g. from quotations and orders to invoices and archiving.
*   In stock management, you can also check the stock of your warehouse and verify values of goods.

#### Sales - Orders and Quotations

Order processing is the central component of A+W Business. It unites all data from the master data.

Depending on the expansion stage of the program, order data is transferred to stock, purchasing, capacity planning, and production for further processing. The results are written to the order.

In order processing a clear arrangement and quick entry are necessary. Therefore, A+W Business distinguishes between the following areas:
*   **Order header:** Name and address of customer, delivery terms and date, payment terms. This information is imported from the master data for the corresponding customer. It can be changed for each order.
*   **Order items:**
    *   Product and product structure, e.g. glass, IG, muntins incl. restriction checks
    *   Sizes and processing steps, e.g. shapes, cut-outs incl. SN entry
    *   Prices and discounts, incl. check for minimum order value
    *   Macro search for product structure incl./excl. prices
    *   Surcharges, e.g. for transport

**Fig. A-12: Sales order**
A screenshot displays a sales order screen, divided into two main parts:
*   **A Order header:** Shows customer details, document number, dates, and terms.
*   **B Order items:** A grid showing the individual products (glass, spacers, etc.), quantities, sizes, and prices for the order.

### Shape Entry

In addition to the standard shape entry that was mentioned in connection with the master data, A+W Business offers the so-called Technical Order Entry (TOE). For this purpose, you can create complex templates and/or macros in A+W CAD Designer and quickly and easily transfer them into orders and quotations via the integration function in A+W Business. This will make your work significantly easier and saves time and money.

**Fig. A-13: Template for TOE (Technical Order Entry)**
*   **A A+W CAD Designer: Template of a studio door (detail):** A detailed CAD drawing of a glass door with cut-outs and edge work.
*   **B Order item: Shape 'studio door' (cut-out):** The resulting shape as it appears in an order, showing the final dimensions and specifications.

### Automated Business Processes

When the necessary data has been entered in the order, the items must be produced, packed and sent. It may be necessary to purchase additional articles for production which are not kept on stock. The order thus triggers other business transactions which are automated as much as possible:
*   Printing of other documents, e.g. order confirmation, delivery note, and invoice
*   Purchase order issued by purchasing
*   Calling stock articles for production
*   Transfer of order data to production
*   Report from production once the order has been produced and is ready to be shipped
*   Shipment
*   Checking the customer's payments
*   Transfer of invoices to financial accounting

### Credit Limit Check

You can enter two different values for the credit limit for every customer, which can be automatically checked when a new order is entered. Credit limit 2 can be used as an internal, uninsured credit limit.

To check the credit limit you have to make the following decisions:
*   Determine the credit limit for each customer in the customer data
*   Define the reaction in case the credit limit is exceeded:
    *   Normally, the status will be raised. If the credit limit is exceeded, new orders will be set to a defined status and will be locked for processing. This status can be reset manually to release the orders for processing.
    *   New orders can be entered and saved. There is a message however pointing out that the credit limit is overdrawn. It is up to the user to decide whether the order shall be processed or rejected.

The corresponding code for every customer or subsidiary is set in partner management.

If you are working with subsidiaries, the credit limit can be checked on two levels:
*   Checking the subsidiary's credit limit.
*   Checking the main customer's credit limit:
    *   Check via subsidiary code
    *   Check via main account: The subsidiary's credit limit will be ignored.

### Form Printing

All commercial documents are printed as forms and can be output on paper or electronically. In addition, further printing functions are available, e.g.:
*   List of orders on hand containing a specific article and the same delivery date.
*   Dimensioned sketches
*   Shape lists
*   Labels
*   Freight lists and shipping documents

### Quotations

Your customers requests alternative quotations for various IG items in the quotation. For this purpose, certain float sheets shall be replaced by e.g. coated glass or, as an option, by LG. In addition, in case of a LG replacement, the cavity (spacer) shall be modified.

This is no problem at all with A+W Business. The following options are available:
*   Create an alternative quotation for the entire quotation.
*   Create an alternative quotation for only a few items.
*   Replace all glasses and cavities.
*   Add shapes, muntins and processings to items, delete them from existing items or search and replace them by different ones.
*   Create additional texts or attach other documents.

The price calculation can be activated immediately in order to have a comparison: Original or alternative. An overview indicates for which quotation alternative quotations have been created.

When a customer accepts a quotation, you can change the quotation into an order.

### Purchasing – Inquiries and Purchase Orders

Inquiries and purchase orders are entered and processed the same as quotations and orders. In addition, the following functions are available:
*   Delivery date check
*   Price comparison in the event of several possible suppliers
*   Incoming goods inspection
*   Reminder for outstanding deliveries
*   Price and invoice control

### Production

The Production module is used for data processing and transfer to production. After the data has been transferred to production, the production software sends reports to A+W Business. Thus, you can view production-relevant information.

You can use A+W Business in different system expansion stages:
*   **Expansion stage 1:** A+W Business + connection to an external production software
*   **Expansion stage 2:** A+W Business + A+W Business production planning and controlling (A+W Business Pro)
*   **Expansion stage 3:** A+W Business + A+W Business production planning and controlling (A+W Business Pro) + A+W Business Capacity Planner
*   **Expansion stage 4:** A+W Business + A+W Business production planning and controlling (A+W Business Pro) + A+W Business Capacity Planner + A+W Business Barcoding
*   **Expansion stage 5:** A+W Business + A+W Production
*   **Expansion stage 6:** A+W Business + A+W Production + A+W Production Capacity Planner
*   **Expansion stage 7:** A+W Business + A+W Production + A+W Production Capacity Planner + A+W Production Barcoding

The expansion stages are listed in ascending order, by size and capacity of the programs, modules and the coupling.

Within these expansion stages, different modules and functions can be activated or deactivated as required.

Which expansion stage you select depends on your requirements, company size and processes. The solutions and programs of A+W Software GmbH offer you the option to grow in the long term and to increase the expansion stage flexibly at any time.

#### Data Transfer and Feedback from Production

By means of the ERP Web Service, the product-relevant data is directly forwarded to the production software A+W Production where it is imported.

**Fig. A-14: Transfer to production and dispatch organization**
A flowchart shows the data flow from an order in A+W Business to A+W Production and back.
1.  An **Order** in A+W Business has its status monitored.
2.  Items are transferred to **Production** in the A+W Production software.
3.  The Production software sends a **Report** back to A+W Business, updating the status.
4.  If an item requires purchasing, a **P.O.** is created. After **Receipt of goods**, the item in the production order can proceed.
5.  If an item has direct delivery, it bypasses production.
6.  **Deadline monitoring** and **Route planning** in A+W Business lead to **Shipping** to the **Customer**.

The order status controls the correct booking sequence so that an order can only be transferred to production if it has the appropriate status, for example.

The current state of production is reported back to A+W Business. Based on this, the status of each order item is changed, and finally that of the entire order. Depending on how a company is organized, the status is raised automatically or manually. The data including the change of status can be entered via barcodes, which helps to reduce input errors considerably.

#### Material Overview

You can display a preview of the required material quantities you will be needing to produce certain product groups.

**Fig. A-15: Schedule by product groups**
A screenshot shows a material overview report, listing the quantity, area, weight, and net amount of materials required for orders within a specific date range, broken down by main product group (MPG).

> In this simple overview you can check whether there is sufficient raw material in stock and whether the scheduled dates are realistic. The displayed data is loaded directly from the orders.
> **A+W Business Capacity Planner:** A comprehensive range of functions is available in A+W Business Capacity Planner for planning production capacities.

#### Optimization of Quotations

If you have entered rarely used glass types in a quotation, it is essential to make sure that the sales price is calculated so as to avoid losses. You can transfer the quotation to production in order to plan the cutting and thus determine the glass required as well as the waste.

After transferring quotations to A+W Production, you can analyze and evaluate the quotation data with respect to the production capacities and the material consumption. This includes the following checks for example:
*   Checking if the requested delivery date is possible or checking for the earliest production and delivery dates.
*   Calculation of material and machine costs.
*   Calculation of the glass yield from different optimization points of view.

#### Reservation Orders

Orders can be transferred to Production without triggering immediate production. This function is controlled by means of the document type:
*   **Calculation:** Calculation of material and machine costs. The orders are not released for production and are not saved in A+W Production.
*   **Reservation:** Reservation of capacities. The orders are saved in A+W Production, but are not released for production.

Orders that have been transferred this way are only produced when they are transferred again to production as a "regular" order.

### A+W Business Pro (Production Manager)

In program version A+W Business Pro the Production Manager and necessary production master data are integrated.

**Fig. A-16: Production module – Production Manager**
A screenshot of the Production Manager interface, which allows for batch creation, scheduling, optimization, and outputting production lists and machine control files.

The Production Manager supports you in the planning and preparation process for production. This includes batch creation up to printing production documents and creating machine codes.

**Fig. A-17: Standard process for the production solution**
A flow diagram shows the process:
Order Element selection -> Batch creation -> Rack organization -> Optimization -> Release

The orders are automatically released for internal capacity planning by means of a defined status or manually. The full expansion stage is reached by supplementing shifts and shift times in capacity planning.

You can use the Production Manager in two modes:
*   **Standard mode:** In this mode, a wizard guides you through the program. As a result, you go through the entire process with only one mouse click and the possibility to change a few settings. By that the system automatically creates the batch, does the rack allocation and calculates the yield. At the end of the process, the optimization results are shown. You can then decide which optimization result (different variants) shall be used.
*   **Expert mode:** In this mode, you execute the individual steps manually. You can influence the individual batch creation and processing steps in detail and quite specifically.

### Shop Floor Data Collection (Barcoding)

Two solutions are available for tracking the production progress in A+W Business:
*   After transfer to the integrated production solution A+W Business Pro, the integrated barcoding solution (optional) allows you to track the production progress for your orders by item. For this purpose, booking points (registration points) are set up, where the status of an item is recorded by means of a scanner.
*   Alternatively to this entry-level solution, you can access advanced functions and options when coupling with A+W Production, e.g. accessing the display and booking of the display host systems of the A+W Production Terminal. In these systems, the status at the monitors and registrations points is recorded exactly by lites and entered in the database.

If an item has been reported as being completed at a registration point, the status of the order item in A+W Business changes to the corresponding status. The order status will be raised only when all items have been reported complete, e.g. produced or ready to be shipped. You can check the current production status of the order in the Status Report dialog.

**Fig. A-18: Barcoding - Receipt of goods**
A diagram shows a simple menu on a scanner device. The options are:
*   Receipt of goods
*   Completion notification
*   Stock movement
*   Special functions
*   Back

For data entry you can use scanners, for example from Denso or Datalogic. With these scanners you can report the receipt of goods, stock movements or production progress of an item via simple booking menus.

### Shipping

In Shipping you organize the delivery of orders through your own fleet of vehicles.

**Fig. A-19: Consignment**
A screenshot of the shipping module, where orders are assigned to a route, lorry, and driver. It shows the total quantity and weight of items to be loaded.

Using consignment, you create route and loading lists, allowing the vehicles to be loaded optimally based on the weight permitted and on route.

### Route Optimization

Using route optimization, you shorten transportation times and routes and thus reduce fuel consumption significantly. As a result, the environmental impact is reduced, vehicles are subjected to less wear and drivers are not burdened with unnecessary mileage.

The Optimizer for Transport Routes (OTR) organizes your destinations, customer addresses or stopping points into a useful and efficient sequence.

In addition to your fleet of vehicles, this sequence considers the defined route restrictions, e.g. tunnels or toll roads. The technology is based on Nokia Maps and updates overview maps on the basis of accessible roads, route points, traffic jams and construction zones. The technology takes into account the weight restrictions of bridges and roads, as well as the height restriction of underpasses.

You can design the routes and optimize them so that on there and back routes, for example, empty racks can be picked up and returned. To this you can add new destination points and take them into account for the entire route.

**Fig. A-20: Standard process for the optimization**
A flow diagram shows the process:
Planning -> Geolocation -> Optimization -> Result

*   **Planning:** Compile the tour(s) or edit existing tours. Within the tours, you can add destination locations (stopping points), edit or delete individual locations. During this phase, you have access to the individual items in order to obtain an overview.
*   **Geolocation:** The program checks whether all way points exist in Nokia Maps and can be reached.
*   **Optimization:** The route is optimized. On the overview map, you will see the routing and list of the individual stations (way points). You can exchange individual stations and have access to the optimization factors.
*   **Result:** The total result of the route is divided into the individual routes, the graphical route plan and list of the destination locations.

**Fig. A-21: Result of the optimization**
A screenshot shows the Logistics Optimizer interface with a map displaying the optimized route and a list of destinations with delivery details.

OTR takes several trucks into account and analyzes driving times in order to ensure that deliveries or pick-ups are within the planned schedules. The routes are adjusted to the traffic in order to obtain the best result.

When calculating the ideal route, important parameters, e.g. storage space, business arrangements, delivery times, standing times or priorities, are taken into consideration. The optimization process generates orders with which destinations with a high priority status can be delivered first.

### Capacity Planning

With the capacity planning you plan the utilization of your production capacities and calculate the production and time costs. The planning data will help to detect bottlenecks well in advance and allow you to make corrections. Two versions are available:
*   **A+W Production Capacity Planner:** With this version, the order data is transferred to production and is analyzed and scheduled. You receive detailed information in the documentation for A+W Production.
*   **A+W Business Capacity Planner:** With this version, you schedule the orders prior to the transfer to production to capacity planning. The orders are only released to production after the checks have been carried out. This version is only working in interconnection with A+W Business Pro.

#### Main Features of A+W Business Capacity Planner

*   Flexible definition of master data for capacity planning
*   Determination of capacity bottlenecks
*   Delivery date check
*   Production cost calculation
*   Control station with overviews and rescheduling functions

#### Mapping of Production Processes

In A+W Business master data, basic products have been created, e.g. single glass, LG, TG, surcharges, shapes, muntins, etc. These products are allocated to the work types and machines to define the production sequence.

**Fig. A-22: Examples for allocating work types to product types**
A diagram shows how different work types are allocated to product types.
*   **Work types:** Cutting, Washing, IG production, Dispatch
*   **Product types:** Single glass, LG, Processings, IG
*   **Allocations:**
    *   Cutting -> Single glass, LG, Processings, IG
    *   Washing -> LG, Processings, IG
    *   IG production -> IG
    *   Dispatch -> Single glass, LG, Processings, IG

You create the master data for capacity planning and coordinate it so that it reflects your production processes.

In this context, explicit and implicit allocations are distinguished:
*   With **explicit (direct) allocations**, the product group Rounded corners, for example, is allocated to the work type CNC processing.
*   With **implicit (indirect) allocations**, the product type Single glass, for example, is allocated to the work type Cutting. Even if there is no product called Cutting in A+W Business master data, it is clear that the single glass has to be cut to the appropriate order size.

#### Time and Costs per Machine

For every machine you have to enter details based on which the machine costs are calculated and the time required to produce an order item.

The defined times are used to calculate the capacities for the individual machine and for the entire production area.

**Fig. A-23: Entries for calculating times and costs per machine**
A diagram illustrates the components for calculating machine time and cost.
*   **Machine** (e.g., cutting table A) is linked to:
    *   **Number of units per hour**
    *   **Cost per hour** (Wages, Machine cost, Variable costs)
    *   **Work types** (e.g., Autom. cutting)

The number of units per hour results from the time taken for this work type. The machine capacity is the result of:
*   Units per hour
*   Number of hours per shift
*   Number of shifts the machine is working.

#### Basic Scheduling Elements

In addition to the order quantity, the following details are considered for scheduling:

**Fig. A-24: Times**
A flowchart shows how different time elements are combined.
*   A **Work type/machine** (e.g., arrissing) has a **Default time**.
*   A **Surcharge** (e.g., for thickness) adds a **Graduated surcharge**.
*   An **Allocation** (e.g., for processing shapes) adds a **Factor** (e.g., per edge).
*   A **Production area** (e.g., toughening furnace) has **Dwell days** and can have a **Transition time** (via a Transition matrix) to another **Work type** (e.g., washing) or another **Production area** (e.g., dispatch).

*   **Default time:** defines the time a work type requires at a certain machine.
*   **Time surcharges:** are usually graded surcharges which, under certain circumstances, increase the default times for rectangular sheets.
*   **Time surcharges and factors:** increase or reduce under certain circumstances the default time, e.g. for producing non-rectangular sheets (shapes).
*   **Dwell days:** define the time a unit spends in a certain production area.
*   **Transition times:** define how long it takes a unit to get from a certain work type to another or from a certain production area to another.
*   **Set-up times:** define the time that is necessary to set up a machine for the next work process. Set-up times are usually entered as a times surcharge.

#### Scheduling

Scheduling starts from the delivery date. The individual work processes are counted back from there.
*   **Backward scheduling:** The check for free capacities always starts with the last work type in the last shift before the delivery date, e.g. packing in shift 2, then goes back to shift 1. If all machines are used to capacity for a work process on a certain day, the program tries to move the process to the day before, etc.
*   **Forward scheduling:** If backward scheduling is not successful, the program searches for a new delivery date based on the next possible route day. Backward scheduling then starts again from that new date. This process can be repeated until scheduling is successful.

Apart from the production times for a machine, dwell and transition times will be taken into account. Here is a summary of criteria:
*   Change of production area, e.g. from cutting to wet area.
*   Change of work type, e.g. from cutting a speech hole to fine polishing of the hole edge.
*   Rest time on the shop floor, e.g. cooling after the toughening furnace.

#### Scheduling Orders in A+W Business Capacity Planner

Orders are continuously transferred in a workflow task to production. At the control station the data of all scheduled orders are united. In this dialog you can change dates and allocated machines, e.g. to squeeze in an urgent order.

**Fig. A-25: Control station - Machines**
A screenshot shows a capacity overview grid, with machines listed as rows and dates as columns. Each cell shows the scheduled load versus the available capacity (e.g., 15.90/28.0).

After the data has been transferred to production, production sends reports to A+W Business. Changes of the scheduled production date are automatically rebooked in capacity planning.

With the change of item and order status, the production progress of items is visible to Sales.

### Statistics and Reports

The success of your company depends on the ability to control current events and make the right decisions. The data from the documents must be reproduced in meaningful presentations. And the most important key figures must be created based on your information.

For this purpose, the following modules (additional modules) are available:
*   With the A+W Business module **Statistics**, you can analyze the following data:
    *   Current orders on hand, turnover, complaint and commission statistics
    *   With Gupta Report Builder the data is displayed in graphical format.

**Fig. A-26: Order info - Graph**
A screenshot shows several graphs generated from order data, displaying metrics like Quantity, Area, Sales Price (SP), and Purchase Price (PP) by month and by customer.

#### Crystal Reports

Use Crystal Reports to create reports in RPT format. The execution of reports can be prevented or permitted by defining the appropriate rights for certain users. A special module is used for printing the Crystal Reports. It is accessible from the A+W Business start menu.

### A+W Discovery

A+W Discovery is the state-of-the-art Business Intelligence System from A+W Software GmbH that is aligned with and geared towards the specific requirements of a modern glass manufacturer or glass refiner. The structure and integration with A+W Production and A+W Business enable you to view the corresponding statistical key figures and indicators from different perspectives, allocate them and infer the necessary strategic, commercial or production-relevant decisions and measures as a result.

**Fig. A-27: Analysis of statistical data with A+W Discovery**
A screenshot of an Excel-based dashboard showing "Share of super product groups in turnover" as a pie chart and "Subsidiaries contribution margin" as a bar chart.

E.g. you can collect data that show you the contribution margin and turnover volume of certain locations or subsidiaries in a defined time frame, e.g. per month or year. As a result, you can adjust your cost structures and motivate your employees and sales partners to increase turnover in the following year. In addition, you can analyze productive key figures over a defined period of time, e.g. machine down-times or the volume of breakage per workstation.

Moreover, A+W Discovery provides you with the option to interrelate and aggregate ERP and PPS data via A+W standard reports. This way you are always in full control of all commercial and product-relevant data - products, resources, costs, time and capacities.

### A+W Dashboard

A+W Dashboard is a service with a web-based interface that allows you to view KPI data from production, e.g. A+W Production.

A+W Dashboard can be started in any new version browser. The address to the requested server can be saved as a favorite or link on the desktop - the same as all internet addresses.

A+W Dashboard is a tool to visualize production. It shows the current performance of machines and employees in the form of graphics.

**Fig. 2: Monitor display (some examples)**
A screenshot shows several dashboard widgets with bar charts and pie charts visualizing production KPIs like booking data and machine state.

> Database tables with the barcode bookings are used for analysis. Usually a time period of max. 24 hours is taken into account. This is how A+W Dashboard differs from A+W Discovery since it allows statistical analyzes over longer periods of time.
> **Correct display only if barcode bookings are correct:** You need complete barcode bookings for meaningful displays.

### Stock Management

A+W Business's module Stock Management allows you to manage jumbo sizes, stock sizes, residue plates, boxes, all-glass doors, fittings, frame parts and accessories such as mirror mountings, sealing tape, etc.

It is possible to display your company's stock organization in the program. You define the locations, corridors, shelves, up to the individual trays and specify which single articles, sqm articles and linm articles are located at which storage location.

**Fig. A-1: Overview of stock management**
A flowchart shows the processes in stock management.
*   **Order** generates a need for stock articles.
*   **Stock on hand** is affected by **Reservation** (from orders) and **Booking out of stock** (from delivery notes/invoices).
*   If there is a **Stock shortage**, a P.O. item is sent to **Purchasing**.
*   **Purchasing** issues an order to a **Supplier**.
*   **Receipt of goods** from the supplier leads to **Booking addition to stock**, which increases **Stock on hand**.
*   All these processes feed into **Analyzes**.

All commercial transactions in A+W Business are based on master data. In connection with sales and purchasing, the following processes are created:
*   **Order:** An order defines the customer's purchase order. You enter all the items that must be produced in accordance with the customer's specifications.
*   **Transfer to production:** Order items to be produced are transferred to production. The required materials are reserved and are booked out of stock when the delivery note or invoice is printed. At the same time, the available stock on hand is updated.
*   **Stock P.O.:** If stock articles fall short of the minimum stock, these stock articles must be entered in the form of a stock P.O. and transferred to purchasing.
*   **Stock addition:** The stock on hand of the stock articles is updated by entering the receipt of goods. Articles that are not kept as stock articles cannot be kept as stock on hand.
*   **Inventory:** With the inventory you correct the stock on hand figures in A+W Business.

#### Stock Info – Future Stock on Hand

**Fig. A-2: Stock info - future stock on hand**
A screenshot shows a report forecasting the stock level for an article over the next several days. It starts with the current "Stock on hand", subtracts "Reservation", adds incoming "P.O."s, and calculates the "Closing inventory" for each day.

When entering order items, you are already checking whether the current stock is sufficient to give reliable delivery date confirmations. In stock management you plan the P.O. in accordance with the reservations.
The preview always starts with the current date. You define the number of days for the preview, e.g. 14 days.

#### Stock Query

Various queries serve to give you an overview of the bookings, the total value of the stock on hand, statistics, and a list of reservations.
*   **Booking journal:** The booking journal offers analyzes on stock bookings created from orders and purchase orders. You can view stock bookings by product, for example.
*   **Stock history:** Stock history gives a quick overview of the daily events on stock, by product.
*   **Stock statistics:** Stock statistics inform you which of your stock articles are hits and which are slow sellers. This provides you with a criterion to decide whether articles should be added or withdrawn from stock.
*   **Stock movement:** The current value of the entire stock can be checked at all times, apart from during the inventory taking.
*   **Reserved stock articles:** Stock articles reserved by orders can be listed by number manager. The reserved stock articles are shown by article number and storage location.

#### Inventory

Stocktaking determines the existing stock by type, quantity, and value. Inventory lists are created for this statutory annual stocktaking which help to count and enter the actual stock on hand.

The inventory list can refer to selected stock articles and/or storage locations. This way, stock can be taken in several steps which present less of an obstruction to the daily business.

Stocktaking is possible by conventional methods, or by means of barcode registration.

With the final inventory, stock quantities are updated in A+W Business.

## Working with A+W Business

As a result of the intuitive graphic user interface (GUI), working with A+W Business can be learned quickly and easily. For your initial introduction you will find information in the following sections. Specific approaches are taught in the training sessions.

This section provides information on the following subjects:
*   "Documentation" on page A-57
*   "Starting and exiting A+W Business" on page A-50
*   "Elements of the Program Window" on page A-51

### Starting and exiting A+W Business

A+W Business can be started in various ways:
1.  Select [Start] > All Programs > A+W > A+W Business.
    or
2.  (Double-) Click the shortcut on your desktop.

If the program start is not linked with the Windows login, the dialog **Database Login** is displayed.
1.  Enter your user name and the password. If you are working with different databases and servers you must enter the corresponding data.
2.  Click [OK] to start the program.

If A+W Business is integrated in the PC's auto-start function, the program icon will be displayed on the task list when the system is started.

To exit A+W Business, click the Close icon on the top right-hand side of the program window.

### Elements of the Program Window

The program window of A+W Business offers all modules, menus, and functions necessary to display, enter, and edit data. The program window consists of the following sections:

**Fig. A-3: Areas of the program window**
*   **A Ribbon:** Menus and buttons for the active dialog.
*   **B Navigation bar:** Display of modules. You can adapt this section as required. Click on a module to open it. A double click on an entry in the navigation bar will open the corresponding dialog.
*   **C Editing area:** Display of dialogs.

### Standard Menus

The following menus are displayed by default when you open a dialog:
*   **Start:** Use this menu to access buttons to navigate between the records and to start actions.
*   **Functions:** Use this menu to open other dialogs without closing the current one. The entries that are available depend on the current dialog.
*   **Options:** This menu allows you to define the default settings for the current dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.
*   **Printing:** Use this menu to start the output of a list or analysis on the screen or printer.
*   **Communication:** This menu allows you to send an email or a fax.
    *   Mail management allows to send an email to a colleague who is defined as a user in A+W Business. This message is displayed on the recipient's screen when he/she closes the present dialog.
        *   To save this message, quit the mail dialog with [OK].
        *   To delete the message, quit the dialog with [End].
    *   The function Fax message allows to send a fax or email to customers or suppliers. You can use the fax numbers and email addresses entered in the master data, or enter alternatives.

### Standard Buttons

The following buttons are displayed when you open a dialog. If a function is not available or if the conditions for executing this function are not met, the button in question is inaccessible.

**Tab. A-1: Buttons of the ribbon**

| Icon | Function | Icon | Function |
| :--- | :--- | :--- | :--- |
| **Close** | Close the active dialog. `<Esc>` | **Filter** | Switches to search mode (QBE mode). `<Ctrl>+<A>` |
| **Help** | Open the Online Help. `<F1>` | **Search** | Start the search. `<Enter>` |
| **About** | Provides information on the program, e.g. the version number. | **New** | Create a new record (Release the input fields). `<Ctrl>+<N>` |
| **First** | Display the first record of the table. `<F5>` | **Delete** | Delete the current record. `<Ctrl>+<L>` |
| **Previous** | Display the previous record of the table. `<F6>` | **Save** | Save a new record or the amendments. `<Ctrl>+<S>` |
| **Next** | Display the next record of the table in question. `<F7>` | **Execute** | Start the action. `<Enter>` |
| **Last** | Display the last record of the table. `<F8>` | | |

### Hotkeys in document entry

To enter documents and items the following keyboard shortcuts (hotkeys) are available.

#### Common functions

| Function | Hotkey |
| :--- | :--- |
| Close window | `<Esc>` |
| Create record | `<Ctrl>+<N>` |
| Customer information | `<Shift>+<Ctrl>+<C>` |
| Delete | `<Ctrl>+<L>` |
| First record | `<F5>` |
| Last record | `<F8>` |
| Next record | `<F7>` |
| Open online help | `<F1>` |
| Previous record | `<F6>` |
| Produktionsübersicht | `<Ctrl>+<B>` |
| Save | `<Ctrl>+<S>` |
| Selection criteria | `<Ctrl>+<A>` |
| Send e-mail | `<Ctrl>+<M>` |
| Send fax message | `<Ctrl>+<F>` |
| Show document | `<Shift>+<Ctrl>+<D>` |

#### Documents & Orders

| Function | Hotkey |
| :--- | :--- |
| Article info | `<Shift>+<Ctrl>+<I>` |
| Change address | `<F11>` |
| Check receivables | `<Ctrl>+<O>` |
| Cost and surcharge calculation | `<Ctrl>+<U>` |
| Document data | `<Shift>+<Ctrl>+<F12>` |
| History | `<Ctrl>+<H>` |
| Input freight costs | `<Ctrl>+<K>` |
| Item entry | `<F9>` |
| List of alternative quotations | `<Ctrl>+<F>` |
| List of complaints | `<Ctrl>+<G>` |
| List of down payments | `<Ctrl>+<A>` |
| List of partial shipments | `<Ctrl>+<T>` |
| Order/P.O. info | `<Ctrl>+<I>` |
| Production status | `<Ctrl>+<B>` |
| Show duplicates | `<Shift>+<Ctrl>+<D>` |
| Stock preview | `<Shift>+<Ctrl>+<S>` |
| Stock search | `<Shift>+<Ctrl>+<F11>` |

#### Items

| Function | Hotkey |
| :--- | :--- |
| Apply price settings to following items | `<Shift>+<Ctrl>+<T>` |
| Article info | `<Shift>+<Ctrl>+<I>` |
| Change locked items | `<Shift>+<F12>` |
| Complaint | `<Shift>+<Ctrl>+<R>` |
| Copy from item | `<Shift>+<Ctrl>+<Y>` |
| **Cost and surcharge calculation** | |
| - Overview | `<Ctrl>+<U>` |
| - Detail - Item | `<Ctrl>+<P>` |
| - Detail - BOM | `<Ctrl>+<D>` |
| Delete and recalculate | `<Ctrl>+<U>` |
| Delete BOM item settings | `<Shift>+<Ctrl>+<L>` |
| Delete item settings | `<Shift>+<Ctrl>+<V>` |
| Delete preset item price | `<Shift>+<Ctrl>+<P>` |
| Enter quantity for current item | `<Ctrl>+<Q>` |
| Insurance prices | `<F12>` |
| Muntins entry | `<F10>` |
| New item | `<Ctrl>+<N>` |
| No recalculation of automatic surcharges | `<Shift>+<Ctrl>+<O>` |
| Price recorder | `<Shift>+<Ctrl>+<F10>` |
| Processings entry | `<F11>` |
| Production status | `<Ctrl>+<B>` |
| Quick entry | `<Shift>+<Ctrl>+<S>` |
| Reason for manual price setting | `<Shift>+<Ctrl>+<F11>` |
| SN editor | `<F4>` |
| **Muntins** | |
| - Drill hole-symmetrical | `<Ctrl>+<Q>` |
| - Field symmetrical | `<Ctrl>+<W>` |
| - Drill hole-asymmetrical | `<Ctrl>+<E>` |
| - Field-asymmetrical | `<Ctrl>+<R>` |
| Start price calculation | `<Ctrl>+<Y>` |
| Stock search | `<F3>` |
| **Structure** | |
| - Pattern 1st sheet rotate | `<Shift>+<F1>` |
| - Pattern 2nd sheet rotate | `<Shift>+<F2>` |
| - Pattern 3rd sheet rotate | `<Shift>+<F3>` |
| - Coating 1st sheet rotate | `<Ctrl>+<F1>` |
| - Coating 2nd sheet rotate | `<Ctrl>+<F2>` |
| - Coating 3rd sheet rotate | `<Ctrl>+<F3>` |
| - Macro search for structure | `<Ctrl>+<Y>` |
| Terms / Individual prices | `<Shift>+<Ctrl>+<K>` |

### Documentation

The modules and processes of A+W Business are described in separate documents. Each part includes training documentation (tutorials) and software references:
*   The tutorials describe the functions of the software. They each include detailed instructions regarding the operation and prerequisites.
*   The Online Help describes the program dialogs in detail. You can open this context-sensitive Help function by using the `<F1> `key in A+W Business. You will also find the dialog descriptions in the software references of the manuals.
*   In addition to this user documentation, the extensive database documentation is available, e.g. to create queries and reports.

#### Online Help

The A+W Business Online Help can be opened as follows:
*   Button [Help]
*   Key `<F1>`

The Online Help is context-sensitive, i.e. exactly for the currently open dialog. If no current help topic is available, the start page of the help is displayed.

Use the arrow keys to go to the next or previous Online Help topic. The tabs offer you the following options to search for information:
*   **Content:** The individual parts are shown as a navigation tree. You can open the topics with the book icon to view the help text.
*   **Index:** The index entries are shown in alphabetical order.
*   **Search:** The full-text search finds all the topics that include the search term.
*   **Favorites:** Use this tab to create links to topics that you require more frequently.
