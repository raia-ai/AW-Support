---
description: "EN_AWBusiness_Purchasing_3_30_1-1"
---


# A+W Purchasing D

---
## A+W Business

A+W - Software for Glass, Windows and Doors

## Introduction

This part of the documentation contains editorial notes.

### Revision Overview

| Section Version/Date | Description |
| :--- | :--- |
| 3.30/04-2020 | Receipt of goods updated |
| 3.20/11-2019 | Software reference: Receipt of goods dialog updated, Tutorial: Chapter for boxes moved to the part Box management. |
| 3.10/10-2017 | Structural revision, new dialog reorder, dialog OC supplier updated. |
| 3.01/01-2017 | Product and company names adjusted. |
| 3.00/06-2013 | Complete revision of ALFAK documentation and adjustment to A+W Business. |
| 2.10/02-2012 | Update of the chapters on the receipt of goods |
| 2.00/02-2010 | Update and conversion to documentation concept 2010 |
| 1.00/10-2008 | New Purchasing section Separated from section Documents |

### Editorial

The editorial provides information on the following topics:
*   Notes on this document
*   Copyrights
*   Trademarks
*   Contacts

#### Notes on this document
This document is intended for end users of A+W Business.

The documentation and software described are licenses that must only be used or copied in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH can-not be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of A+W Business.

### Copyrights
© 2020, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademarks
All hardware and software names mentioned in this documentation can also be registered trademarks or other property rights of third parties. Third-party copyrights must therefore be observed.

### Contacts
**A+W Software GmbH**

Am Pfahlgraben 4-10
D-35415 Pohlheim
*   Phone: +49 6404 2051 0
*   Fax: +49 6404 2051 877
*   Email: Zentrale@a-w.com
*   Web: http://www.a-w.com

## Contents

*   **Introduction** D-3
    *   Revision Overview D-3
    *   Editorial D-3
*   **Tutorial** D-9
    *   Overview D-11
    *   Documentation D-12
    *   Tutorial structure D-12
    *   Display conventions D-13
    *   Menu overview D-14
    *   Basic ideas on purchasing D-17
    *   Master data for purchasing D-20
        *   Product definition D-21
        *   Purchase code D-22
        *   Checking a product's master data D-25
        *   Definition of stock sizes D-27
    *   Suppliers D-29
        *   Market partner supplier D-30
        *   Checking a supplier's master data D-31
        *   Supplier file amendment D-32
    *   Purchase prices D-34
        *   Price lists D-35
        *   Check price master data D-36
    *   Document status D-38
        *   Status allocation D-39
        *   Status allocation D-40
    *   Purchase orders D-41
        *   P.O. transfer vs. manual purchase order D-42
        *   Document P.O. D-43
        *   Checking the default settings for purchase orders D-45
        *   P.O. items in the order D-48
        *   Customer order D-49
        *   Supplier for order item D-50
        *   Changes in ordered items D-51
        *   Enter a P.O. item in the order D-52
        *   Change supplier in order D-54
        *   Change ordered item D-55
    *   P.O. transfer D-58
        *   Order pool D-60
        *   Transfer document to order pool D-66
        *   Changing a P.O. in the order pool D-70
        *   Compare prices in the order pool D-72
        *   Order and P.O. info D-76
    *   Manual purchase order D-77
        *   Independent P.O.s D-78
        *   Entering an independent P.O. D-79
        *   Enter stock P.O. D-81
    *   Supplier's order confirmation D-84
        *   Supplier's OC D-85
        *   Overdue deliveries D-86
        *   Order confirmation entry D-87
        *   Enter order confirmation and check prices D-91
        *   Remind supplier D-95
    *   Delivery date check D-98
        *   Delivery date check and correction D-99
        *   Change delivery dates, notify customer D-100
        *   Check and change all dates D-103
    *   Inquiry D-108
        *   Inquiry for P.O. items or purchase orders D-108
        *   Create an inquiry for a P.O. item D-110
        *   Create a purchase order from an independent inquiry D-113
    *   Exercises D-115
    *   Deliveries in receipt of goods D-117
        *   Receipt of goods D-118
        *   Deliveries D-119
        *   Check the default settings for receipt of goods D-124
        *   Enter receipt of goods D-125
        *   Check receipt of goods D-131
    *   Receipt of boxes D-133
        *   Dealing with boxes D-134
        *   Check company data D-134
        *   Checking the settings for ID numbers D-134
        *   Enter the receipt of boxes D-136
    *   Price and invoice control D-141
        *   Incoming invoice D-142
        *   Checking the invoice D-144
    *   Exercises D-147
    *   Electronic document exchange D-148
        *   Export/Import (openTRANS) D-149
        *   Document exchange D-151
        *   Document check D-154
        *   Check the services D-157
        *   Status allocation D-158
        *   Check the default settings for data exchange D-159
        *   Check the currency settings D-160
        *   Check status definitions D-161
        *   Set the data export via open TRANS D-164
        *   Check Partner Master Data D-166
        *   Import of electronic documents D-167
        *   Check the electronic document D-168
        *   Create a partial delivery from an electronic document D-170
        *   Allocate items in electronic documents D-171
        *   Allocate surcharges/discounts manually D-172
    *   Data export/import (EDI) D-174
        *   Data exchange in ASC format D-175
        *   Check company data D-175
        *   Check the settings D-175
        *   Exporting of purchase orders D-179
*   **Software Reference** D-181
    *   Overview D-183
    *   Inquiry (menu) D-184
    *   Inquiry (document management) D-185
    *   Purchase order (menu) D-186
    *   Purchase order (document management) D-188
    *   Replenishment Order D-189
    *   Export (EDI) D-191
        *   Functions menu D-192
        *   Export - export D-193
        *   Export - pool D-194
    *   OC supplier D-195
        *   Options menu D-195
        *   OC supplier - documents D-196
        *   OC supplier - items D-200
        *   OC Supplier - change delivery dates D-201
    *   Order confirmation D-202
    *   Price control D-203
        *   Functions menu D-203
        *   Options menu D-204
        *   Price control - purchase orders D-205
        *   Price control - item D-208
        *   Price control – BOM D-210
    *   Electronic price control D-211
        *   Functions menu D-212
        *   Options menu D-212
        *   Electronic price control - document import D-214
        *   Electronic price control - item overview D-217
    *   Selection (prod. no. for balancing item) D-218
    *   Settings for Xternal D-219
    *   Manual allocation of items D-219
    *   Distribution of footer surcharges/discounts D-220
    *   Filter settings D-221
    *   Reminder D-223
    *   Receipt of goods D-225
        *   Receipt of goods (dialog) D-225
        *   Functions menu D-226
        *   Options menu D-226
        *   Print menu D-227
        *   Receipt of goods - selection D-228
        *   Receipt of goods -complete D-230
        *   Receipt of goods - by item D-232
        *   Receipt of goods - ID numbers D-235
        *   Receipt of goods - protocol (ID numbers) D-237
    *   Settings (ID) D-238
    *   Inspection of goods received D-239
        *   Inspection of goods received – complete P.O.s D-239
        *   Inspection of goods received - Qty. discrepancies D-241
    *   Invoice D-243
        *   Invoice control D-243
        *   Functions menu D-244
        *   Options menu D-244
        *   Invoice control - Purchase orders D-246
        *   Invoice control - items D-249
        *   Invoice control - BOM D-251
    *   Invoice date D-253
    *   Electronic invoice control D-254
        *   Functions menu D-254
        *   Options menu D-254
        *   Electronic invoice control - document import D-257
        *   Electronic invoice control - item overview D-260
    *   Invoicing of basic glass D-262
*   **Section Index** D-263
    *   Index D-265

# Tutorial

## Overview

The tutorial for the Purchasing module deals with the basics of purchasing in A+W Business. This tutorial is based on existing knowledge of the master data and on sales.

> **The functions depend on the enabled modules**
> Please note that the individual functions are only available if the corresponding modules and interfaces have been installed and enabled.
>
> If you detect functions in this document that are not available in your version, please contact A+W Software GmbH.

### Subjects
This tutorial offers the following subjects:
*   Basic ideas on purchasing
*   Master data for purchasing
*   Purchase orders
*   Deliveries in receipt of goods
*   Electronic document exchange

### Required knowledge
This tutorial is intended for those who process purchase in A+W Business. Participants must be familiar with the master data concept in A+W Business and with the Document management dialog.

### Documentation
The following documents are available for the Purchasing module:

*   **Handout**: Printout of tutorial for training session
*   **PDF**: Complete documentation
    *   Tutorial
    *   Software reference
    *   Index
*   **Online help <F1>**: Context-sensitive dialog help for the A+W Business software references and tutorials on the basic version

### Tutorial structure
This tutorial consists of subjects with several training modules each. Each module consists of the following elements:

*   **Overview**: Each training module starts with an overview of the major topics:
    *   **Objectives:** What knowledge is to be conveyed?
    *   **Benefit:** What can this knowledge be used for?
    *   **Maxims:** Which correlations are to be remembered?
*   **Concepts**: First, the concepts and terms of the corresponding training module will be explained. This is followed by examples and instructions.
*   **Exercises**: For some of the modules, exercises with certain tasks and suggested solutions are available.
*   **Cross-references**: At the end of each training module there is a section with cross references pointing out additional information in the software reference and in other sections. This will help you to extend your newly acquired knowledge.

#### Reading instructions
The contents of a training module are based on the knowledge conveyed in the previous module. We therefore recommend not to skip any modules.
If you are already familiar with a subject, you should at least read the summary at the start of the module in order to bring the main details to mind.

### Display conventions
Certain parts of sentences are specially marked. The meanings are:

*   **Italics**: marks character strings describing the software elements, e.g. the *Number Manager dialog*.
*   **Bold**: marks character strings to be entered via the keyboard, e.g.: Enter the value **0**.
*   **>**: The so-called breadcrumb trail marks the way to open a dialog, e.g. Documents > P.O. > Export.
*   **[]**: Square brackets mark buttons in a dialog, e.g. [OK] to save the data.
*   **< >**: Angle brackets refer to keys or shortcuts on the keyboard, e.g. <F1> is used to open the online help.

### Menu overview
This chapter provides a brief overview of the program sections that will be addressed in the subjects of this training.
The Documents menu also includes the program sections for handling Sales. These are described in section Sales.

*Fig. D-1: Documents module - Purchase order menu*
(Image displays the A+W Business software interface, specifically the Purchase Order (P.O.) screen. The screen shows various tabs for document details, addresses, terms, and technical parameters. The main area includes fields for P.O. number, supplier information, dates, and document status. A list of existing documents is visible at the bottom.)

#### P.O.
Use this section to create and manage purchase orders.
⇨ "Purchase orders" on page D-41

#### Replenishment
Use this dialog you manage orders with ordered parts that are reported as broken and decide whether they should be reordered, whether a complaint should be lodged, whether they should be invoiced or deducted from the order quantity.
⇨ Software Reference, “Replenishment Order" on page D-189

#### Print P.O.
In this dialog you print the purchase orders you are going to send to suppliers. This function is described in detail in the Sales section.
⇨ Sales, "Print" on page C-152

#### Export
You can use this dialog to export purchase orders in order to transfer them to the respective supplier via the EDI interface.
⇨ "Exporting of purchase orders" on page D-179

#### Journal
This dialog gives you an overview of the purchase orders. This function is described in detail in the Sales section.
⇨ Sales, "Journal" on page C-337

#### OC supplier
In this dialog you enter the order confirmations you have sent to your suppliers.
⇨ "Supplier's OC" on page D-85

#### Order confirmation
In this section you can check the prices in order confirmations.
⇨ "Checking the invoice" on page D-144

#### Receipt of goods
This section is used to check and create receipt of goods for your purchase orders.
⇨ "Receipt of goods" on page D-118

#### Invoice
This area is used to enter and check invoices from suppliers.
⇨ "Check the electronic document" on page D-168

#### Transfer to financial accounting
This dialog is used to transfer the invoices received to your financial accounting system. This function is described in detail in the Sales section.
⇨ Sales, "Debit Entry FinAcc" on page C-590

#### Transfer to archives
This dialog is used to transfer your purchase orders to archives. This function is described in detail in the Sales section.
⇨ Sales, "Transfer to Archives" on page C-594

#### Document data
In this dialog you can view lists of purchase orders and the corresponding orders and correct dates if necessary. This function is described in detail in the Sales section.
⇨ Sales, "Document Data" on page C-644

#### Stock search
Use this dialog to check product availability and search for stock sizes. This function is described in detail in the Sales section.
⇨ Sales, "Stock Search" on page C-649

#### Article info
In this dialog you can display information on the products entered in A+W Business. You can check the product structure, prices and availability. This function is described in detail in the Sales section.
⇨ Sales, "Product Information" on page C-521

#### Fax message
This dialog allows you to issue and dispatch fax messages to your customers and suppliers directly from A+W Business. This function is described in detail in the Overview section.
⇨ Einleitung, "Standard-Menüs" auf Seite A-53

## Basic ideas on purchasing
Purchasing is one of the commercial tasks within a company. Purchasing is typically structured in this or a similar way in A+W Business:

*Fig. D-2: Purchasing scheme in A+W Business*
(A flowchart illustrates the purchasing process. An optional "Inquiry" can lead to a "P.O." (Purchase Order). A "Customer order" can also be transferred to create a "P.O.". The P.O. undergoes "OC + price control". "Stock" can feed into "Receipt of goods". The "Receipt of goods" then undergoes "OC + price control" and can also feed into "Production", which is linked back to the "Customer order". The legend indicates that blue boxes are "Documents", yellow boxes are "Sections", and dotted lines represent "optional" paths.)

All commercial transactions in A+W Business are based on master data. Purchasing can work properly only if the master data is in order and up to date:

*   **Inquiry:** Inquiries are used to get quotations from your suppliers. If the quotation is convincing, you can create the purchase order right from the inquiry without having to enter the data again.
    ⇨ "Inquiry" on page D-108
*   **Purchase order:** In a manual purchase order you enter the order items and select the required supplier. The reference purchase order is created from the customer order by means of the order pool.
    ⇨ "Manual purchase order" on page D-77
*   **Order confirmation (OC) from the supplier:** Enter the order confirmation number and check the prices and delivery dates. In case of delays you can notify the customer if necessary. Changed and confirmed prices can be saved in the PP calculation.
    ⇨ "Order confirmation and delivery date" on page D-85
*   **Receipt of goods:** Check the receipt of goods and add stock purchase orders automatically to the stock on hand. Reference purchase orders are transferred to production and/or sales in order to edit the corresponding customer order, or finish it.
    ⇨ "Enter receipt of goods" on page D-125
*   **Invoice control:** Check the invoice and correct the purchase prices if you accept the price changes. The invoice can now be released for payment.
    ⇨ "Price and invoice control" on page D-141

### The purchasing process
Purchasing documents are usually processed on the basis of the following steps:
*   Create inquiry (optional)
*   Purchase order
    *   Enter header data
    *   Enter items
    *   Edit BOM
*   Print purchase order (send by fax, email, electronically)
*   Enter supplier's order confirmation
*   Check the prices
*   Correct dates and route planning based on feedback
*   Enter receipt of goods
*   Check the invoice
*   Transfer to archives and statistics
*   Delete document from main database

If the purchase order was created by P.O. transfer from a customer order, the data does not need to be created manually.

> **Daily procedure**
> The easiest way of arranging your daily procedure is by using the Number Managers. Empty the corresponding Number Manager or create a new one for that day.
> Now create the new documents in this Number Manager. This helps you keep track of the documents that are new and can or have to be processed.

## Master data for purchasing
This subject shows you how to adapt the master data for purchasing.
This includes the following training modules:
*   "Product definition" on page D-21
*   "Suppliers" on page D-29
*   "Purchase prices" on page D-34
*   "Document status" on page D-38

### Product definition

**Objectives**
*   Adapting product master data for purchasing purposes.
*   Learning about procurement types for purchase orders.
*   Learning about the use of purchase codes in orders.

**Benefits**
*   The purchase code points out products to A+W Business which have to be ordered.
*   By means of the purchase code, a purchase order is automatically created for a customer order in the order pool. Therefore, the purchase order does not have to be entered by hand.

**Please note:**

*   **Procurement type**: The code *Procurement type* defines how the product entered in the order or in the purchase order shall be acquired, e.g. by producing it, taking it from stock, or ordering it.
*   **Purchase code**: The following procurement types are called purchase codes:
    *   P.O.
    *   P.O. (complete)
*   **P.O. (complete)**: This code is used for products with a bill of materials, which are to be ordered as a whole, e.g. an entire door including the fittings.
*   **P.O.**: This code is used for products for which individual elements are to be ordered, e.g. only the fittings.
*   **Default settings**:
    *   **Master data Product management:**
        *   Price/Surcharge tab
        *   Stock/Purchasing tab
    *   **Company data:**
        *   Stock/PP/EDI tab
        *   Documents tab
        *   Parameters tab
        *   Calculation tab

#### Purchase code
Purchasing refers to the products managed in A+W Business. To buy a product, it needs to be entered in a purchase order.

You can define how every product is to be used for pricing, discount calculation, production, purchasing, etc. Only the appropriate codes permit, for example, automatic transfer to interfaces, invoicing, or printing in the documents.

The procurement type requires special attention in connection with purchasing because it tells A+W Business when a product or a product element has to be purchased.

*   **P.O. item (complete):**
    The P.O. includes all processing steps defined in the bill of materials. If, for example, a laminated glass unit consists of float sheet 5 mm, a film layer and tempered glass 5 mm, the laminated unit will be ordered as a whole. (Please also note the difference from P.O. items.)
*   **P.O. items:**
    Only the concerned product is ordered, without taking into account the content of the bill of materials (e.g. processing steps). If, on the other hand, e.g. a laminated unit consists of a float sheet, a film layer and a tempered sheet and if the code *Purchase article* has now been set for the tempered sheet, only the tempered sheet will be ordered from the supplier. The laminated unit will be produced in-house.

This purchase code is automatically adopted for the order item. Every item can be allocated a purchase code in the order itself however.

#### Procurement type
These procurement types for the purchase code are defined in the product master data. It is used by default when a product is entered in a document. It can be changed in the order and in the P.O.

*Fig. D-3: Purchase code in BOM*
(A diagram illustrates how different purchase codes (`*` for P.O., `**` for P.O. complete) on a Bill of Materials (BOM) item affect the outcome.
1.  If "Float 4 Bronze" is marked with `*` (P.O.), the "Float 4 Bronze is delivered unarrissed", and the final "IG is produced" in-house with the arrissed edges.
2.  If "Float 4 Bronze" is marked with `**` (P.O. complete), the "Float 4 Bronze is delivered arrissed", and the final "IG is produced" in-house.
3.  If the top-level "IG 150000" is marked with `**` (P.O. complete), the entire "IG is delivered complete".)

If a main item or a superordinate BOM element is marked with the procurement type P.O. (complete), the corresponding BOM elements will not be withdrawn from stock if their procurement types are set to Stock withdrawal. The procurement type cannot be changed for these elements in this case.

The procurement type can be defined per Client and/or production preparation. In this case, please activate the option *Activate different procurement type per client/PS area* in the company data.

*Fig. D-4: Company data – Parameters tab*
(Image shows a settings screen with a checkbox labeled "Enable deviating procurement type per client/order area" which is checked.)

**A:** Different procurement type per client or production preparation.

#### Prices and surcharges
Price tables are created for both purchasing and sales. They have to be allocated to every single product to make sure that the corresponding prices are calculated automatically.

### Checking a product's master data
For purchasing, in particular all product data that are ordered by default has to be completely entered.
The Master data section describes in detail how to define the master data for your products. The following description therefore only deals with the peculiarities you have to consider in connection with purchasing.

**■ How to check a product's master data**
1.  Select **Master Data > Products > Articles > Articles**.
    The *Product management* dialog appears.
    ⇨ Master Data, "Product Management - Stock / Purchasing" on page B-598
2.  Search the product you want to check and go to the *Price/surcharge* tab.

*Fig. D-5: Product management – Price/surcharge*
(Image shows the 'Price/surcharge' tab in the Product Management screen for an article. It highlights two checkboxes: (A) 'Price relevant SP' for sales and (B) 'Price relevant PP' for purchasing. The text explains their function.)

3.  Check whether price tables and the checkboxes **Price relevant for sales (A)** and **purchasing (B)** are correctly selected.
    Checkbox **Price relevant PP** has to be ticked only if you are using purchase price calculation.
