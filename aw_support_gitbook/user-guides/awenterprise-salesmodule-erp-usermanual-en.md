---
title: "EN-UM-AW_Enterprise-Sales_4_1"
source: "EN-UM-AW_Enterprise-Sales_4_1.pdf"
tags: ["A+W Enterprise", "Sales Module", "ERP", "Glass Manufacturing", "Window Manufacturing", "Order Entry", "User Manual", "Software Documentation", "Search Functions", "Invoicing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a user manual for the A+W Enterprise Sales module, version 4.00. It provides a comprehensive software reference for end-users, detailing functionalities for managing sales documents, including quotations, orders, invoices, and credit notes. The guide covers order entry, pricing, search functions, and document management."
long_description: "This is the official user manual for the A+W Enterprise Sales module, a component of the A+W software suite designed for the glass, windows, and doors industry. The document serves as a detailed software reference, guiding end-users through the various features and functions of the Sales module. It begins with an introduction that includes a revision history, copyright information, and contact details for A+W Software GmbH. The core of the manual is the 'Software Reference' section, which provides an in-depth overview of managing sales-related documents such as quotations, orders, deliveries, and invoices. It meticulously documents the structure of the application's menus, including the main Sales Menu, Supplementary Menu, Info Menu, and various submenus for handling addresses, texts, prices, and product details. A significant portion is dedicated to 'Search Functions,' explaining how to efficiently find documents, market partners, articles, and products using various criteria. The manual also covers technical details, bill of materials (BOM) management, packaging planning, and document status tracking. It is intended to be a comprehensive resource for users to successfully navigate and utilize the full capabilities of the A+W Enterprise Sales module in their daily operations."
---

# A+W Sales D

---
## A+W Enterprise

**A+W - Software for Glass, Windows and Doors**

---

## Introduction

This part of the documentation contains editorial notes.

### Revisions Overview

| Part Version / Date | Initial version |
| :--- | :--- |
| 1.00 / 02-2006 | Initial version |
| 2.00 / 12-2006 | Change of tab Sales |
| 2.10 / 02-2007 | Combination of Sales/Purchasing |
| 2.20 / 01-2008 | Price calculation |
| 2.30 / 01-2010 | Minor corrections/identifier |
| 3.00 / 07-2013 | Complete revision and adjustment to new CI |
| 3.01 / 01.2017 | Product and company name adjusted |
| 4.00 / 03.2020 | Complete revision |

### Editorial

The Editorial provides information on the following topics:
- Notes on this document
- Copyrights
- Trademark
- Contacts

#### Notes on this document

This document is intended exclusively for end users of A+W Enterprise.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice.

The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full program level of A+W Enterprise.

#### Copyrights

© 2020 A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, either electronically, mechanically, or by recording or in any other way, without A+W Software GmbH's prior written approval.

#### Trademark

All hardware and software names mentioned in this documentation can also be registered trademarks. Third party copyrights have to be obeyed.

#### Contacts

**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
📞 +49 6404 2051 0
📠 +49 6404 2051 877
📧 Zentrale@a-w.com
🌐 http://www.a-w.com

---

## Contents

- **Introduction** D-3
  - Revisions Overview D-3
  - Editorial D-3
- **Software Reference** D-11
  - Overview D-13
  - Sales Menu D-14
    - Invoices submenu D-15
    - Overview submenu D-16
  - Supplementary Menu D-16
    - Addresses submenu D-18
    - Texts submenu D-18
    - Special texts submenu D-19
    - Prices submenu D-19
    - Order prices submenu D-20
    - Product details submenu D-20
    - Technical values submenu D-21
  - Info Menu D-22
    - Notes submenu D-23
  - Search Functions D-24
  - Find Orders D-25
    - Find Orders - Document Key D-25
    - Find Orders - Item Code D-28
    - Find Orders - Direct Search D-30
  - Find Orders - Hit List D-31
    - Find Orders - Delivery Information D-32
    - Find Orders - Miscellaneous D-34
    - Find orders - Quantities D-35
    - Find Orders - Properties D-37
    - Find Orders - Reference D-39
  - Find Market Partner D-41
  - Employee/Authorization Groups D-45
  - Find Reference Document D-47
  - Find Addresses D-49
  - Find Article D-51
    - Find Article - header, footer areas D-52
    - Find Article - Names D-55
    - Find Article - Article codes D-57
    - Find Article - Details D-59
  - Find Article by Types D-61
  - Find Product by Element D-62
    - Find Product by Element - Header, Footer area D-63
    - Find Product by Element - Cust. Article D-65
    - Find Product by Element - Names D-67
    - Find Product by Element - Tech. Values D-68
  - Find Project D-69
    - Find Project - header, footer areas D-70
    - Find Project - Address D-72
    - Find Project - Identification D-73
  - Enter Value - Extended Search D-74
  - Enter Value - search for reference D-75
  - Enter Value - search for original number D-76
  - Document Management D-78
  - Explanation of Symbols D-79
  - Quotation Entry D-82
  - Entry w/o Prices D-83
  - Order Entry D-84
    - Order Entry - header, footer area D-85
    - Order entry - Addresses D-92
    - Order Entry - Properties D-95
    - Order Entry - Miscellaneous D-101
    - Order Entry - Totals D-106
    - Order Entry - Detailed View Discounts D-111
  - Order Items D-116
    - Order Entry - General D-116
    - Order Entry - Properties D-129
    - Order Entry - Prices D-134
    - Order Items - Status D-137
    - Order Entry - Costs D-139
  - Site Change D-140
  - New Delivery Address D-141
  - End customer address D-143
  - Market Partner Info D-145
  - Contacts D-147
  - Cancel D-148
  - Staff Allocation – Special D-149
  - Configurable Fields D-149
  - Overview D-150
  - Product Sets (Sash Master) D-151
  - Article Dimensions D-153
  - Stock Forecast D-154
  - Product Replacement D-157
    - Product Replacement D-158
    - Product Replacement for Items D-160
  - Complaint D-161
  - Order Types D-162
  - Article Details for Dimensioned Variants D-164
  - Variant and Color/Thickness Selection D-167
  - Private Fields D-168
  - External Data - Import D-169
  - Document Types D-171
  - Allocation of Document Types D-172
  - File Allocation D-174
  - DXF Import D-175
  - Amendment Log D-176
  - Delivery Date Change Log D-178
  - Shape Catalog D-179
  - Shape - Dimensions D-180
  - Payment Management D-182
  - Payment Plan D-184
  - Error Information System D-186
  - Production Monitor D-188
  - Technical Details D-189
  - Declaration of Performance D-189
  - Order Entry - Technical Values D-190
    - Order Entry - Calculated Technical Values D-190
    - Order Entry - Declared Services D-193
  - Bill of Materials (BOM) D-198
  - BOM View D-198
    - BOM View - BOM Structure D-199
    - BOM View - Product Structure D-202
    - BOM View - Production Sketch D-203
    - BOM View - Current BOM Level D-205
    - BOM View – Processing Param. (short) D-210
    - BOM View – Addresses D-211
    - BOM View - All Parameters/Sketch D-212
  - Edge Allocation D-220
  - Item Processing D-221
  - Dimensions of Individual BOM Elements D-222
  - Spac. Offset D-224
  - Sealing Depths D-225
  - Stepped Entry (Relevant Parts) D-226
  - Step Reductions D-228
  - Muntin Entry D-229
    - Muntin Entry – Muntins D-229
    - Muntin Entry – Add. Info D-232
  - Muntin Product - Product Number D-233
  - Muntin Editor D-234
  - Drill Point D-235
  - Clear Field D-235
  - Muntin Sections D-236
  - Grid Pattern D-237
  - Packaging Planning D-239
  - Specs. Packaging Planning D-239
  - Rack Planning D-245
  - Notes D-247
  - Document Notes D-249
  - Market Partner, Project, Article Notes D-250
  - Customer Article, Supplier Article, Project Article Notes D-253
  - Texts D-255
  - Header and Footer Texts D-256
  - Article and Item Texts D-258
  - Special Texts D-259
  - Phrases D-260
  - External Information D-262
  - Box Signature D-263
  - Prices and Conditions D-265
  - Order Conditions D-266
  - Order Prices D-271
  - Order Muntin Prices D-273
  - Order Exchange Prices D-276
  - Order Sub-part Prices D-278
  - Post Calculation D-279
  - Step Prices D-282
  - Conditions for PCD Processing D-283
    - Conditions for PCD, PCD BASIC GLASS Processing D-284
    - Conditions for PCD BASIC GLASS D-288
    - Conditions IG D-290
    - Conditions IG (SWITZERLAND) D-295
    - Conditions for PCD COLORED ARTICLE D-299
    - Conditions for PCD PRICES GENERAL D-300
    - Conditions for PCD GLASS DOORS D-302
  - Conditions for Manual Prices D-305
  - LAMI Exchange/Additional Prices D-306
  - Item Conditions - Processing Prices (Sls), (Purch), Detail View D-309
  - Item Conditions - Muntin Prices D-312
  - Production Cost Calculation D-315
    - Production Cost Calculation - Overview D-316
    - Production Cost Calculation - Details D-318
  - Price Calculation D-322
  - Release D-323
  - Order Release D-323
  - Authorization D-326
  - Delivery D-328
  - Deliv. Plan D-329
  - Delivery Information - Delivery Details D-331
  - Delivery Notes (automatic) D-335
  - Delivery Notes (manual) D-337
  - Delivery Notes Log D-339
  - Invoices D-340
  - Invoices (automatic) D-341
  - Item Info D-344
  - Invoices (manual) D-346
  - Cash Transaction D-347
  - Booking of Invoices D-348
  - Partial Invoice (automatic) D-350
  - Partial Invoice (manual) D-352
  - Final Invoices (automatic) D-353
  - Final Invoices (manual) D-354
  - Invoice Log D-355
  - Credit Notes D-356
  - Credit Notes D-356
  - Book Credit Notes D-358
  - Forms D-360
  - Direct Printing D-360
  - Form Printing D-361
  - E-mail D-365
  - Print on D-367
  - List Printing D-368
  - Order Status D-369
  - Order Information D-369
    - Document Info - Order D-370
    - Document Info - Items D-371
    - Document Info – Purchasing D-372
    - Document Info - Goods Received D-374
    - Document Info - Production D-375
    - Document Info – Dispatch D-377
    - Document Info - Barcoding D-378
    - Document Info - Racks D-380
    - Document Info - Stock D-381
    - Document Info - Linked Production D-382
    - Document Info - Intermediate Disp. D-383
  - Document Research D-384
  - Search Document D-384
    - Search Document - search mode D-384
    - Search Document - Overview D-388
    - Search document - Employees D-390
    - Search Document - Details D-391
    - Search Document - Document Change Log D-394
  - Items D-396
    - Items - Overview D-396
    - Items - Details D-398
  - Overviews of Documents D-400
  - Order Display D-400
  - Quotation Display D-401
  - Resubmission D-402
  - Completion Report D-403
  - Document Change D-405
  - Overview of Documents D-408
  - Sales D-410
- **Section Index** D-411
- **Index** D-413

---

# Software Reference

## Overview

In the Sales module you manage the documents that are required for the successful processing of the sales business. They include, e.g. quotations, orders, and credits and create invoices.

In the Sales section you will find the following topics:

- "Search Functions" on page D-24
- "Document Management" on page D-78
- "Technical Details" on page D-189
- "Bill of Materials (BOM)” on page D-198
- "Packaging Planning" on page D-239
- "Notes" on page D-247
- "Texts" on page D-255
- "Prices and Conditions" on page D-265
- "Release” on page D-323
- "Delivery" on page D-328
- "Invoices" on page D-340
- "Credit Notes" on page D-356
- "Forms" on page D-360
- "Order Status" on page D-369
- "Document Research" on page D-384
- "Overviews of Documents" on page D-400
- "Sales" on page D-410

## Sales Menu

Some of the available menu entries branch out to submenus. If these include more than three entries, they are listed separately according to the following overview. The displayed entries depend on the respective configuration.

For additional documentation that is not included in this section for the Sales menu or if you have questions, please contact your partner at A+W Software GmbH.

> **Context menus**
> On the context menus (right mouse button), only the menu elements are offered that make sense in the context for the individual fields of the dialogs. You can also call up the functions on the context menus via the menus described. Generally, the menu elements on the context menu correspond to the functions offered on the prompt display.

You can reach all dialogs and functions relating to sales via the Sales menu:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Quick entry | ⇨ Not used any longer |
| b | Quotation entry | ⇨ "Quotation Entry" on page D-82 |
| c | Order entry | ⇨ "Order Entry" on page D-84 |
| d | Pricing | ⇨ "Price Calculation" on page D-322 |
| e | Entry without prices | ⇨ "Entry w/o Prices" on page D-83 |
| f | Delivery notes | |
| fa | • Automatic release | ⇨ "Delivery Notes (automatic)" on page D-335 |
| fb | • Manual delivery notes | ⇨ "Delivery Notes (manual)" on page D-337 |
| fc | • Log | ⇨ "Delivery Notes Log" on page D-339 |
| g | Invoices | ⇨ "Invoices submenu" on page D-15 |
| h | Credit notes | |
| ha | • Enter credit notes | ⇨ "Credit Notes" on page D-356 |
| hb | • Book credit notes | ⇨ "Book Credit Notes" on page D-358 |
| i | Release order | |
| ia | • Release | ⇨ "Order Release" on page D-323 |
| ib | • Authorization | ⇨ "Authorization" on page D-326 |
| j | Forms | |
| ja | • Print | ⇨ "Form Printing" on page D-361 |
| jb | • E-Mail/Fax | ⇨ "E-mail" on page D-365 |
| None: | Print list | ⇨ "List Printing" on page D-368 |
| l | Overview | ⇨ "Overview submenu" on page D-16 |
| m | Background check | ⇨ "Error Information System" on page D-186 |
| n | Resubmission | ⇨ "Resubmission" on page D-402 |
| o | Completion report | ⇨ "Completion Report" on page D-403 |
| p | Document change | ⇨ "Document Change" on page D-405 |
| r | Sales | ⇨ "Sales" on page D-410 |

### Invoices submenu
*Sales > Invoices*

Use this menu to access all dialogs on which you create and manage invoices.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Automatic release | ⇨ "Invoices (automatic)" on page D-341 |
| b | Manual invoice | ⇨ "Invoices (manual)" on page D-346 |
| c | Cash invoice | ⇨ "Cash Transaction" on page D-347 |
| d | Book invoices | ⇨ "Booking of Invoices" on page D-348 |
| None: | Partial invoice | |
| ea | • Automatic release | ⇨ "Partial Invoice (automatic)" on page D-350 |
| eb | • Manual invoice | ⇨ "Partial Invoice (manual)" on page D-352 |
| f | Final invoice | |
| fa | • Automatic release | ⇨ "Final Invoices (automatic)" on page D-353 |
| fb | • Manual invoice | ⇨ "Final Invoices (manual)" on page D-354 |
| g | Log | ⇨ "Invoice Log" on page D-355 |

### Overview submenu
*Sales > Overview*

Use this menu to access all dialogs on which you can display an overview of the various documents.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Orders not invoiced | ⇨ "Overview of Documents" on page D-408 |
| b | Invoices not booked | |
| c | Deliveries not complete | |
| d | Orders with invoice block | |
| e | Status of processing | This module is no longer used. |
| f | Number determination | This module is no longer used. |
| g | Order display | ⇨ "Order Display" on page D-400 |
| h | Quotation display | ⇨ "Quotation Display" on page D-401 |
| i | Order information | ⇨ "Order Information" on page D-369 |
| j | Search document | ⇨ "Search Document" on page D-384 |

### Supplementary Menu

The supplementary menu can be called up with `<F4>` for entering various documents, e.g. for an order.

Depending on the dialog and area, the entries on the supplementary menu are displayed differently. The example described here is the entries that are displayed when calling up the supplementary menu in the document entry:
- Supplementary menu for the header and footer area (document entry)
- Supplementary menu for the item level (document entry)

#### Supplementary menu for the header and footer area (document entry)

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Text | |
| a a | • HeaderText | ⇨ "Header and Footer Texts" on page D-256 |
| a b | • Footer | ⇨ "Header and Footer Texts" on page D-256 |
| a c | • External information | ⇨ "External Information" on page D-262 |
| b | Addresses | ⇨ "Addresses submenu" on page D-18 |
| c | Contact person | ⇨ "Contacts" on page D-147 |
| d | Cancel | ⇨ "Order Items" on page D-116 |
| e | Prices | ⇨ "Prices submenu" on page D-19 |
| f | Product details | ⇨ "Product details submenu" on page D-20 |
| g | Representation | ⇨ "Resubmission" on page D-402 |
| h | Transfer to production (again) | Transfer the order automatically to production after saving. |
| i | Production monitor | ⇨ "Production Monitor" on page D-188 |
| j | Delivery plan | ⇨ "Deliv. Plan" on page D-329 |
| k | Delivery information | ⇨ "Delivery Information - Delivery Details" on page D-331 |
| l | Payment plan | ⇨ "Payment Plan" on page D-184 |
| m | Payment management | ⇨ "Payment Management" on page D-182 |
| None: | Configurable fields | ⇨ "Configurable Fields" on page D-149 |
| o | Site change | ⇨ "Site Change" on page D-140 |
| p | Direct printing | ⇨ "Direct Printing" on page D-360 |

#### Supplementary menu for the item level (document entry)

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Text | ⇨ "Texts submenu" on page D-18 |
| b | Addresses | ⇨ "Addresses submenu" on page D-18 |
| c | Cancel | ⇨ "Order Items" on page D-116 |
| d | Private fields | ⇨ "Private Fields" on page D-168 |
| e | Prices | ⇨ "Prices submenu" on page D-19 |
| f | Product details | ⇨ "Product details submenu" on page D-20 |
| g | Representation | ⇨ "Resubmission" on page D-402 |
| h | Consignments | |
| ha | • New consignment | Change to the Commis field on the Items tab in order to create or edit a consignment text. |
| hb | • Change consignment | ⇨ "Order Entry - General" on page D-116 |
| i | Delivery plan | ⇨ "Deliv. Plan" on page D-329 |
| j | Stock | |
| ja | • Stock (Ctrl+P) | Display the Stock field on the General tab. The stock display is an optional function and is configured customer-specifically. For customer-specific adjustments, contact your contact person at A+W Software GmbH. |
| jb | • Stock forecast (Ctrl+G) | ⇨ "Stock Forecast" on page D-154 |
| k | Payment plan | ⇨ "Payment Plan" on page D-184 |
| l | Configurable fields | ⇨ "Configurable Fields" on page D-149 |

### Addresses submenu
*<F4> > Addresses*

Use this menu to manage the addresses document-specifically.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Find delivery address(Ctrl+L) | ⇨ "Find Addresses" on page D-49 |
| b | New delivery address (Ctrl+N) | ⇨ "New Delivery Address" on page D-141 |
| c | Delete delivery address | Delete the delivery address from the document. |
| d | End customer address | ⇨ "End customer address" on page D-143 |

### Texts submenu
*<F4> > Texts*

Use this menu to manage the texts. The entries Article text (F5), Item text (Shift+F5) and Special texts are only displayed on the item level.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | HeaderText | ⇨ "Header and Footer Texts" on page D-256 |
| b | Footer | ⇨ "Header and Footer Texts" on page D-256 |
| c | External information | ⇨ "External Information" on page D-262 |
| d | Article text (F5) | ⇨ "Article and Item Texts" on page D-258 |
| e | Item text (Shift+F5) | ⇨ "Article and Item Texts" on page D-258 |
| f | Special texts | ⇨ "Special texts submenu" on page D-19 |

### Special texts submenu
*<F4> > Texts > Special Texts*

Use this menu to manage all special texts that you can assign to the document or the item. Special texts is an optional function and is configured customer-specifically. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Spacer text | ⇨ "Special Texts" on page D-259 |
| b | Product code | |
| c | Shape texts | |
| d | Logo texts | |

### Prices submenu
*<F4> > Price info*

Use this menu to manage the prices and conditions for a document or individual items.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Order conditions | ⇨ "Conditions for PCD Processing" on page D-283 |
| b | Order prices | ⇨ "Order prices submenu" on page D-20 |
| c | Partial calculation | ⇨ "Production Cost Calculation" on page D-315 |

The following entries are only displayed for the document items:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| d | + | ⇨ "Conditions for PCD Processing" on page D-283 |
| e | Download conditions | Determine the sales price with the item conditions and recalculate the price. |
| f | Price calculation | Recalculate the item price. |
| g | Price control | Display the fields for Price control on the General tab. |

### Order prices submenu
*<F4> > Price Info > Order Prices*

Use this menu to manage the order prices for individual items.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Article prices | ⇨ "Order Prices" on page D-271 |
| b | Muntin prices | ⇨ "Order Muntin Prices" on page D-273 |
| c | Exchange prices | ⇨ "Order Exchange Prices" on page D-276 |
| d | Sub-element prices | ⇨ "Order Sub-part Prices" on page D-278 |

### Product details submenu
*<F4> > Product Details*

Use this menu to manage the details for the products, e.g. exchange and additional rules.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Product replacement | ⇨ "Product Replacement" on page D-157 |
| b | E/A rules | ⇨ Master data |

The following entries are only displayed on the item level:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| c | Prod. group | Edit the product group. The cursor changes to the Prodgrp. field. |
| d | Technical values | ⇨ "Technical values submenu" on page D-21 |

### Technical values submenu
*<F4> > Product Details > Technical Values*

Use this menu to manage the technical values.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Show technical details | Show the technical values. ⇨ "Items tab (left area)" on page D-117 |
| b | Change technical details | Edit the technical values. The cursor changes to the db value field of the technical values on the Items tab. ⇨ "Items tab (Info area - graphic, technical values)" on page D-119 |
| c | Declaration of performance | ⇨ "Declaration of Performance" on page D-189 |
| d | Show hidden dimensions | Show the hidden dimensions on the Items tab. ⇨ "Items tab (Info area - graphic, technical values)" on page D-119 |
| e | Change hidden dimensions | ⇨ "Article Dimensions" on page D-153 |

## Info Menu
*<Shift> + <F4>*

Depending on the dialog and area, the entries on the Info menu are displayed differently. The example described here is the entries that are displayed when calling up the Info menu in the document entry:
- Info menu for the header and footer area (document entry)
- Info menu for the item level (document entry)

### Info menu for the header and footer area (document entry)

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Document notes | ⇨ "Notes" on page D-247 |
| b | Market partner notes | |
| c | Project notes | |
| d | Search document | ⇨ "Search Document" on page D-384 |
| e | Document overview | ⇨ "Overview" on page D-150 |
| f | Market partner information | ⇨ "Market Partner Info" on page D-145 |
| g | Change log | ⇨ "Amendment Log" on page D-176 |
| h | Delivery date changes | ⇨ "Delivery Date Change Log" on page D-178 |
| i | Order information | ⇨ "Order Information" on page D-369 |
| k | Case signature | ⇨ "Box Signature" on page D-263 |
| l | Document types | ⇨ "DXF Import" on page D-175 |
| m | Document overview | ⇨ "Allocation of Document Types" on page D-172 |

### Info menu for the item level (document entry)

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Notes | ⇨ "Notes submenu" on page D-23 |
| b | Search document | ⇨ "Search Document" on page D-384 |
| c | Document overview | ⇨ "Overview" on page D-150 |
| d | Market partner information | ⇨ "Market Partner Info" on page D-145 |
| e | Change log | ⇨ "Amendment Log" on page D-176 |
| f | Delivery date changes | ⇨ "Delivery Date Change Log" on page D-178 |
| g | Order information | ⇨ "Order Information" on page D-369 |
| h | Case signature | ⇨ "Box Signature" on page D-263 |
| i | Document overview | ⇨ "Allocation of Document Types" on page D-172 |

### Notes submenu
*<Shift> + <F4> > Notes*

Use this menu to manage all internal information about documents, market partners, and projects.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Document notes | ⇨ "Notes" on page D-247 |
| b | Article notes | |
| c | Customer notes | |
| d | Customer/article notes | |
| e | Project remarks | |
| f | Project/article remarks | |
| g | Supplier notes | |
| h | Supplier/article notes | |

---

## Search Functions

In the Sales module, you can search via various categories for documents, market partners, addresses, and articles.

The search dialogs are structured the same way for all document types in Sales. They are described in this chapter using the example Order. Deviations will be described explicitly.

The following dialogs are described in this section:
- "Find Orders" on page D-25
- "Find Orders – Hit List" on page D-31
- "Find Market Partner" on page D-41
- "Employee/Authorization Groups" on page D-45
- "Find Reference Document" on page D-47
- "Find Addresses" on page D-49
- "Find Article" on page D-51
- "Find Article by Types" on page D-61
- "Find Product by Element" on page D-62
- "Find Project" on page D-69
- "Enter Value – Extended Search" on page D-74

### Find Orders
*Sales > Order Entry > Order field > <F9>*

You can search for orders on this dialog. Specify the search criteria in the header area. With each criterion that you specify, you can reduce the hit quantity.

This dialog contains the following tabs in the header area:
- "Find Orders – Document Key" on page D-25
- "Find Orders – Item Code" on page D-28
- "Find Orders – Direct Search" on page D-30

The search results are shown in the hit list. The hit list is only displayed if you have started the search.
⇨ "Find Orders - Hit List" on page D-31

#### Find Orders – Document Key
*Sales > Order Entry > Order field > <F9>*

**Fig. D-1: Find Orders - Document Key**

You can search for orders on this tab using order data. You can configure in which search criterion field you are first located for input when you open the dialog. Configurable as first input fields on the Document Key tab are the fields Orders from, Customer, Proj., InvoiceNo., Deliv. Date, P.O.Date, VAT ID No., Operator, Input Date, and Currency.

You can also specify search criteria on the Item Code tab. Configurable as first input fields on the Item Code tab are the fields Article, Qty. Unit, and Dimension Variant.

- Use `<F2>` to change the tab in the header area.
- Use `<F3>` to start the search.

**Document Key Fields**

- **Orders from:** Number starting from which orders are searched for. The search is restricted to all orders whose number is equal to or greater than the specified order number. The field name varies depending on the dialog from which you open the search, e.g. Quotations.
  *Technical info: numeric field, DB field: kauf.auftrnr*
- **Customer:** Customer number. The search is restricted to all orders for this customer. If you specify a number, the customer name is displayed in plain text.
  *Technical info: numeric field, display field, DB field: kauf.kunr, kauf.orgname*
- **Site No.:** Site number. By default, the number of your own site is filled in. The search is restricted to all orders from this site. The field can only be edited if you are working with internal site separation.
  *Technical info: numeric field, DB field: kauf.hausnr*
- **Proj.:** Project number for which orders will be searched for. The search is restricted to all orders with this project. The project name is displayed in plain text after input of the number.
  *Technical info: numeric field, display field, DB field: kauf.objnr, kauf.orgname*
- **External No.:** Order number that is specified by the customer. The search is restricted to all orders with this external number.
  *Technical info: alphanumeric field, DB field: kauf.exaufnr*
- **Act.Ref.No:** Original document number for transferred documents. The search is restricted to all orders with this reference number.
  *Technical info: numeric field, DB field: kauf._orgauftrnr*
- **Invoice No.:** The search is restricted to all orders for which this invoice was created.
  *Technical info: numeric field, DB field: kauf.rechnr*
- **Deliv. Date:** Desired delivery date for the order. The search is restricted to all orders with this delivery date. The delivery date can be specified as date or calendar week. The planned delivery date is displayed in the hit list.
  *Technical info: date field, DB field: kauf.ltplan*
- **P.O. Date:** PO date of the order. The search is restricted to all orders with this PO date.
  *Technical info: date field, DB field: kauf.bdat*
- **VAT ID No.:** Customer's VAT ID. The search is restricted to all orders with this identification number.
  *Technical info: alphanumeric field, DB field: kaufp.steuernr*
- **Operator:** Employee number of the operator who entered the orders. The search is restricted to all orders by this operator.
  *Technical info: numeric field, DB field: kauf.eusr*
- **Input Date:** Date on which the order was entered. The search is restricted to all orders with this input date.
  *Technical info: date field, DB field: kauf.edat*
- **Currency:** Currency that is assigned to the order. The search is restricted to all orders with this currency.
  *Technical info: numeric field, DB field: kauf.waehrung*

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
⇨ "Find Orders - Hit List" on page D-31

**Footer**
- **New Search:** Deletes all search criteria for a new search. Alternatively, you can use `<Ctrl> + <F7>` to delete the search criteria.
- **Search:** Starts the search with the specified criteria. Alternatively, you can start the search with `<F3>`.

#### Find Orders - Item Code
*Sales > Order Entry > Order field > <F9> > Item Code tab*

**Fig. D-2: Find Orders - Item Code**

You can search for orders on this tab using item codes. You can also specify additional search criteria on the Document Key and Direct Search tabs.
- Use `<F2>` to change to the header area of the tab.
- Use `<F3>` to start the search.

**Item Code Fields**

- **Article:** Article number. The search is restricted to all orders that contain this article as item article. If you specify a number, the article name is displayed in plain text. The BOMs of the items are not checked.
  *Technical info: numeric field, DB field: kpos.artnr*
- **Cust. Product:** Reference number for customer-specific products from the master data. The search is restricted to all orders with articles of this customer-specific number.
  *Technical info: alphanumeric field, DB field: kpos.kuposnr*
- **Width, Height:** Width and height of the item in millimeters. The search is restricted to all orders with articles with these dimensions.
  *Technical info: numeric fields, DB fields: kpos.laenge, kpos.breite*
- **Reference:** Reference text. The search is restricted to all orders that contain the specified reference text.
  *Technical info: alphanumeric field, DB field: komm.kommtxt*
- **Quantity Unit:** Quantity unit for the item, e.g. square meter. The search is restricted to all orders with this quantity unit.
  *Technical info: numeric field, DB field: kpos.me*
- **Dimens. Variant:** Dimensional variant of the article. The search is restricted to all orders with these variant articles.
  *Technical info: numeric field, DB field: kpos.var*

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
⇨ "Find Orders - Hit List" on page D-31

**Footer**
The buttons in the footer are described for the Item Code tab:
⇨ "Find Orders - Document Key" on page D-25

#### Find Orders – Direct Search
*Sales > Order Entry > Field Order > <F9> > Direct Search tab*

**Fig. D-3: Find Orders - Direct Search**

You can search for orders on this tab starting with a particular order number. You can also specify additional search criteria on the Document Key and Item Code tabs.

If the search function should be restricted to the direct search for order numbers, the dialog can be configured so that the Document Key and Item Code tabs are deactivated. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

- Use `<F2>` to change to the header area of the tab.
- Use `<F3>` to start the search.

**Direct Search Field**

- **Orders from:** Start number from which orders are searched for in ascending order. The search is restricted to all orders whose number is equal to or greater than the order number specified. The field name varies depending on the dialog from which you open the search, e.g. Quotations from.
  *Technical info: numeric field, DB field: kauf.auftrnr*

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
⇨ "Find Orders - Hit List" on page D-31

**Footer**
The buttons in the footer are described for the Item Code tab:
⇨ "Find Orders - Document Key" on page D-25

### Find Orders – Hit List
*Sales > Order Entry > Field Order > <F9> > Enter search criteria > <F3>*

The hit list contains the following tabs:
- "Find Orders – Delivery Information" on page D-32
- "Find Orders – Miscellaneous" on page D-34
- "Find orders - Quantities" on page D-35
- "Find Orders – Properties" on page D-37
- "Find Orders - Reference" on page D-39

#### Find Orders – Delivery Information
*Sales > Order Entry > Field Order > <F9> > Enter search criteria > <F3>*

**Fig. D-4: Find Orders - Delivery Information**

This tab displays the delivery information and additional details about the orders that fit the search criteria. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the Find Orders dialog:
⇨ "Find Orders" on page D-25

**Record display for the document overview**
The number of hits in the list is indicated on the right, above the tabs, in a spacer. The display means `Document overview: No. of the currently marked hits in the list: Total number of hits.`

**Delivery Info tab Columns**
- **Site:** Site number.
  *Technical info: display field, DB field: kauf.hausnr*
- **Order:** Order number. The column name and number vary depending on the document from which you open the search, e.g. quotation and quotation number for the quotation search.
  *Technical info: display field, DB field: kauf.auftrnr*
- **SubNo:** Number of the partial delivery note or partial invoice.
  *Technical info: display field, DB field: kauf.subnr*
- **Deliv. Date:** Planned delivery date.
  *Technical info: display field, DB field: kauf.ltplan*
- **Customer:** Customer name.
  *Technical info: display field, DB field: kauf.orgkunr*
- **Proj.:** Project number for orders to which a project is assigned.
  *Technical info: display field, DB field: kauf.objnr*
- **Invoice:** Invoice number for invoiced orders.
  *Technical info: display field, DB field: kauf.rechnr*
- **Act.Ref.No.:** Original reference number for transferred documents.
  *Technical info: display field, DB field: kauf._orgauftrnr*
- **Cancelled:** Specification of the processing state, e.g. cancellation status.
  - 0: Order not cancelled.
  - 1: Order cancelled by the operator.
  - 2: Order cancelled by the system.
  - -3, -10, -x: Order in background processing.
  *Technical info: display field, DB field: kauf.still*

**Footer**
The buttons in the footer are described for the Item Code tab:
⇨ "Find Orders - Document Key" on page D-25

#### Find Orders – Miscellaneous
*Sales > Order Entry > Field Order > <F9> > Enter search criteria > <F3> > Miscellaneous tab*

**Fig. D-5: Find Orders - Miscellaneous**

This tab displays various information about the orders that fits the search criteria. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the Find Orders dialog: ⇨ "Find Orders" on page D-25

**Show record**
The number of hits in the list is indicated on the right, above the tabs, in a spacer. The display means `Document overview: No. of the currently marked hits in the list: Total number of hits.`

**Miscellaneous tab**
The columns are described for the Delivery Information tab. ⇨ "Find Orders - Delivery Information" on page D-32. In addition, the following columns are displayed:
- **Entry:** Date on which the order was entered.
  *Technical info: display field, DB field: kauf.edat*
- **Operator:** Name of the operator who entered the orders.
  *Technical info: display field, DB field: kauf.eusr*
- **VAT ID No.:** Customer's VAT ID.
  *Technical info: display field, DB field: kaufp.steuernr*
- **Ref.:** Document number that is being referenced in the document entry.
  *Technical info: display field, DB field: kauf.referenz*

**Footer**
The buttons in the footer are described for the Item Code tab: ⇨ "Find Orders - Document Key" on page D-25

#### Find orders – Quantities
*Sales > Order Entry > Field Order > <F9> > Enter search criteria > <F3> > Quantities tab*

**Fig. D-6: Find orders – Quantities**

This tab displays item information about the orders that fit the search criteria. One line is displayed per order item. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the Find Orders dialog: ⇨ "Find Orders" on page D-25

**Show record for the item overview**
The number of hits in the list is indicated on the right, above the tabs, in a spacer. The display means `Item overview: No. of the currently marked hits in the list: Total number of hits.`

**Quantities tab**
The columns are described for the Delivery Information tab. ⇨ "Find Orders - Delivery Information" on page D-32. In addition, the following columns are displayed:
- **Itm:** Item number in the order.
  *Technical info: numeric field, DB field: kpos.posnr*
- **ArtNo, Article:** Article number and article name of the header article.
  *Technical info: numeric field, alphanumeric field, DB fields: kpos.artnr, kpos.artbez1*
- **Qty:** Item quantity.
  *Technical info: numeric field, DB field: kpos.menge*
- **Shipped:** Quantity of the item already shipped.
  *Technical info: numeric field, DB field: kpos.gelief*
- **kmp.:** An asterisk `*` indicates if the item has been delivered completely.
  *Technical info: display field*
- **Invcd:** An `F` indicates if the item has been invoiced completely.
  *Technical info: display field*
- **kmp.:** An `F` indicates if the item has been invoiced completely.
  *Technical info: display field*

**Footer**
The buttons in the footer are described for the Item Code tab: ⇨ "Find Orders - Document Key" on page D-25

#### Find Orders – Properties
*Sales > Order Entry > Field Order > <F9> > Enter search criteria > <F3> > Properties tab*

**Fig. D-7: Find Orders - Properties**

This tab displays additional item information for orders. One line is displayed per order item. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the Find Orders dialog: ⇨ "Find Orders" on page D-25

**Show record for the item overview**
The number of hits in the list is indicated on the right, above the tabs, in a spacer. The display means `Item overview: No. of the currently marked hits in the list: Total number of hits.`

**Properties tab**
The columns are described for the Delivery Information and Quantities tab:
- ⇨ "Find Orders - Delivery Information" on page D-32
- ⇨ "Find orders - Quantities" on page D-35

In addition, the following columns are displayed:
- **QU:** Quantity unit for the item, e.g. square meter.
  *Technical info: display field, DB field: kpos.me*
- **sf:** Glass area in square meters.
  *Technical info: display field, DB field: kpos.qm*
- **ft:** Length specification for the item per piece in linear meters.
  *Technical info: display field, DB field: kpos.umlfdm*
- **Weight:** Weight of the item in kilograms.
  *Technical info: display field, DB field: kpos.gewicht*
- **Width, Hght:** Dimensions of the item in millimeters.
  *Technical info: display fields: DB field: kpos.laenge, kpos.breite*
- **Dimens. Variant:** Dimensional variant of article.
  *Technical info: display field, DB field: kpos.var*

**Footer**
The buttons in the footer are described for the Item Code tab: ⇨ "Find Orders - Document Key" on page D-25

#### Find Orders – Reference
*Sales > Order Entry > Field Order > <F9> > Enter search criteria > <F3> > Reference tab*

**Fig. D-8: Find Orders - Reference**

This tab displays information about the references of the orders that fit the search criteria. One line is displayed per order item. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the Find Orders dialog: ⇨ "Find Orders" on page D-25

**Show record for the item overview**
The number of hits in the list is indicated on the right, above the tabs, in a spacer. The display means `Item overview: No. of the currently marked hits in the list: Total number of hits.`

**Reference tab**
The columns are described for the Delivery Information and Quantities tab:
- ⇨ "Find Orders - Delivery Information" on page D-32
- ⇨ "Find orders - Quantities" on page D-35

In addition, the following columns are displayed:
- **Reference:** Reference text.
  *Technical info: display field, DB field: komm.kommtxt*

**Footer**
The buttons in the footer are described for the Item Code tab: ⇨ "Find Orders - Document Key" on page D-25

### Find Market Partner
*Sales > Order Entry > Field Customer > <F9>*

**Fig. D-9: Find Market Partner**

You can search for market partners on this dialog. You enter the search criteria in the header area. If you open Find Market Partners, you will see all market partners in the hit list that are stored in the master data and not yet disabled. With internal site separation, only the market partners are listed that are assigned to the site. Using the filter criteria, you can restrict the hit list.

You can configure in which search criterion field you are first located for input when you open the dialog. Configurable as initial input fields are the fields `From No.`, `Matchcode`, `Name`, `1stName`, `Cntry`, `PCd`, and `City`.

You can call up the market partner search via various menu paths. The dialog always looks the same.
- Use `<F3>` to start the search.
- Use `<F2>` after the search to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

The hit list displays the addresses and information for identification of the market partners:
- "Address tab" on page D-43
- "Identification tab" on page D-44

> **Default setting for the market partner types**
> Depending on which menu path you use to open the dialog, the market partner type you're looking for can be set already, e.g. customer or supplier. The hit list is then filtered accordingly. The selection of the market partner types is only possible when searching in the master data.

**Search fields**
- **From No.:** Start number from which market partners are searched for in ascending order. The market partners whose number is smaller than the number specified are excluded from the hit list.
  *Technical info: numeric field, DB field: mp.mpnr*
- **Matchcode:** Alphanumeric matchcode of the market partner. The market partners whose match code does not include the data specified are excluded from the hit list.
  *Technical info: alphanumeric field, DB field: mp.mc*
- **Type:** Display of the market partner type. The type is stored in the market partner master data. The field is automatically pre-populated by the system.
  *Technical info: display field, DB field: mp.kuliflag*
- **Name, 1stName:** Name and first name of the market partner. The market partners whose names do not include the data specified are excluded from the hit list.
  *Technical info: alphanumeric fields, DB fields: mp.name, mp.vaname*
- **Street:** Street address of the market partner. The market partners whose street address does not include the data specified are excluded from the hit list.
  *Technical info: alphanumeric field, DB field: mp.strasse*
- **Site:** Site number with internal site separation. The market partners that are not assigned to the specified site are excluded from the hit list.
  *Technical info: numeric field, DB field: mpmdzu.hnr*
- **Country:** International country code of the market partner. The market partners whose country codes do not include the specified data are excluded from the hit list.
  *Technical info: alphanumeric field, DB field: mp.land*
- **PCd, City:** Postal code and city name for the market partner's address. The market partners whose postal code and city do not include the data specified are excluded from the hit list.
  *Technical info: alphanumeric fields, DB fields: mp.plz, mp.ort*
- **VAT ID No.:** Market partner's VAT ID number. The market partners whose identification number does not include the specified data are excluded from the hit list.
  *Technical info: alphanumeric field, DB field: mp.steuernr*
- **Type:** Market partner status. In the order entry, only active market partners are displayed. This field cannot be edited.
  *Technical info: display field, DB field: mp.still*

> **Show record for the market partner overview**
> The number of hits in the list is indicated on the right, above the tabs, in a spacer. The display means `Item overview: No. of the currently marked hits in the list: Total number of hits in the list.`
>
> **The display of hits is loaded record by record**
> If a large number of hits has to be displayed, under some circumstances, it can take some time for the system to do this. So that the hit list can be displayed quickly, it is loaded record by record. The record size is configured in the system settings. The hits are loaded in numeric sequence, e.g. the first 100 hits numerically. Additional hits can be loaded with the [More Data] button.
>
> **Example**
> `11:100 (1256)` is displayed in the record display.
> - 11 stands for the number of the marked hit in the hit list.
> - 100 stands for the number of hits that are currently displayed in the hit list.
> - 1256 stands for the number of all hits.

**Address tab**
The columns in the hit list correspond to the fields in the header area. In addition, the following columns are displayed:
- **Number:** Market partner number.
  *Technical info: display field, DB field: mp.mpnr*
- **Addition:** Additional note, e.g. an address addition.
  *Technical info: display field, DB field: mp.branche*

**Identification tab**
The columns in the hit list correspond to the fields in the header area. In addition, the following columns are displayed:
- **Number:** Market partner number
  *Technical info: display field, DB field: mp.mpnr*
- **Disabled:** Indication of whether the market partner has been disabled.
  - Y: Market partner has been disabled.
  - N: Market partner is active.
  In the order entry, only active market partners are displayed.
  *Technical info: display field, DB field: mp.still*
- **Type:** Type of the market partner, e.g. customer, supplier.
  *Technical info: display field, DB field: mp.kuliflag*
- **Company:** Number of the company of the market partner with internal site separation. The company number is drawn from the system master data.
  *Technical info: Anzeigefeld, DB field: xcompany.compid*

**Footer**
Use the buttons in the footer to navigate in the hit list, display additional hits, and update the hit list.
- **`<`, `<<`, `>>`, `>`:** Use `[<]` and `[>]` to jump to the first or last entry in the hit list. Use `[<<]` and `[>>]` to display the previous or next page of the hit list.
- **Refresh:** Updates the entries in the search fields. Corrected or additional entries in the search fields are taken into account during the search. The button is only enabled in the Search fields area.
- **More Data:** Displays additional entries in the hit list that correspond to the search criteria. If no more hits can be displayed, the button is locked.
- **New Search:** Deletes all search criteria for a new search. Alternatively, you can use `<Ctrl> + <R>` to delete the search criteria and start a new search.

### Employee/Authorization Groups
*Sales > Order entry > Properties tab > Operator field > <F9>*

**Fig. D-10: Employee/Authorization Groups**

Use this dialog to search for employees. Enter the search criteria in the header area. If you open the employee search, all employees are displayed in the hit list. You can use the filter criteria to restrict the hit list.

You can call up the employee search via various menu paths. The dialog always looks the same.
- Use `<F3>` to start the search.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

The hit list displays the employees who correspond to the search criteria:
⇨ "Hit list" on page D-46

**Search fields**
- **From No.:** Start number from which employees are searched for in ascending order. The employees whose number is smaller than the number specified are excluded from the hit list.
  *Technical info: numeric field, DB field: mp.manr*
- **Type:** Display of the employee type. The type is stored in the employee master data. The field is automatically pre-populated by the system.
  *Technical info: display field, DB field: mitarb.matyp*
- **Name, 1stName:** Employee's last name and first name. The employees whose names do not contain the specified data are excluded from the hit list.
  *Technical info: alphanumeric fields, DB fields: mitarb.maname, mitarb.vname*
- **Departm.:** Number and name of the department. If you specify a number, the name of the department is displayed in the second field.
  *Technical info: numeric field, display field, DB fields: mitarb.abtnr, abteilung.bez*
- **Login:** User name of the employee for login to A+W Enterprise.
  *Technical info: alphanumeric field, DB field: mitarb.loginname*

**Show record for the employee overview**
The number of hits in the list is indicated on the right, above the tabs, in a spacer. The record display is described for the Find Market Partner dialog:
⇨ "Find Market Partner" on page D-41

**Hit list**
The columns in the hit list correspond to the fields in the header area. In addition, the following column is displayed:
- **Number:** Employee number
  *Technical info: display field, DB field: mitarb.manr*

**Footer**
Use the buttons in the footer to navigate in the hit list, display additional hits, and update the hit list. The fields and buttons in the footer are described in detail in the Find Market Partner section:
⇨ "Find Market Partner" on page D-41

### Find Reference Document
*Sales > Order Entry > Reference field > <F9>*

**Fig. D-11: Find Reference Document**

Use this dialog to search for documents to which you can make reference in document entry. Specify the search criteria in the header area. The search results are shown in the hit list. The hit list is only displayed if you have started the search.
- Use `<F2>` to change to the header area of the tab.
- Use `<F3>` to start the search.
- Use `<F2>` after the search to change tabs on the hit list.

The dialog is structured the same as the Find Orders dialog.
⇨ "Find Orders" on page D-25

**Item Code tab**
Most fields are described for the Item Code tab for finding orders:
⇨ "Find Orders - Document Key" on page D-25
In addition, the following fields are displayed:
- **Document:** Document type. The search is restricted to all documents of this type.
  - Quotation
  - Order
  - Supplier inquiry
  - P.O.
  *Technical info: selection field, DB field: kauf.vorgang*
> **Default setting for the document type**
> The document type is pre-set user-specifically, e.g. Quotation. You configure the default setting in the system settings.
- **Document number:** Number and subnumber of the reference document. The search is restricted to all documents with this number and/or subnumber.
  *Technical info: numeric field, display field, DB fields: kauf.auftrnr, kauf.subnr*
- **Scheduled:** Scheduled delivery date of the reference document in the format DD.MM.YYYY. The search is restricted to all documents with this delivery date.
  *Technical info: date field, DB field: kauf.ltplan*

**Direct Search tab**
- **Orders from:** Start number from which orders are searched for in ascending order. The search is restricted to all orders whose number is equal to or greater than the order number specified. The field name varies depending on the dialog from which you open the search, e.g. Quotations from.
  *Technical info: numeric field, DB field: kauf.auftrnr*

**Hit list**
The tabs in the hit list are described in detail for finding orders:
⇨ "Find Orders - Hit List" on page D-31

**Footer**
The buttons in the footer are described in finding orders for the Item Code tab:
⇨ "Find Orders - Document Key" on page D-25

### Find Addresses
*Sales > Order Entry > Header, Footer, Item level > <F4> > Addresses > Find Delivery Address*

**Fig. D-12: Find Addresses**

Use this dialog to search for the market partner's addresses. Enter the search criteria in the header area. When you open the address search, all the market partner's addresses will be displayed in the hit list. You can restrict the hit list with the filter criteria.
- Use `<F3>` to start the search.
- Use `<F2>` after the search to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

The delivery addresses and additional contact data for the market partners are displayed in the hit list.
⇨ "Address tab, Contact Data tab" on page D-50

**Search fields**
- **Name:** Customer name. The addresses of customers whose name does not contain the specified data are excluded from the hit list.
  *Technical info: alphanumeric field, DB field: adr.adrname*
- **Street:** Street address of the delivery address. The addresses whose street addresses do not contain the specified data are excluded from the hit list.
  *Technical info: alphanumeric field, DB field: adr.str*
- **PCd:** Postal code of the delivery address. The addresses whose postal code does not include the specified data are excluded from the hit list.
  *Technical info: alphanumeric fields, DB fields: adr.plz, adr.ort*
- **City:** City name of the delivery address. The addresses whose city does not contain the specified data are excluded from the hit list.
  *Technical info: alphanumeric fields, DB fields: adr.plz, adr.ort*
- **Cntry:** Country name for the delivery destination. The addresses from countries that do not contain the specified data are excluded from the hit list.
  *Technical info: alphanumeric field, DB field: adr.land*
- **Address code:** Code of the saved address. The addresses whose address code does not include the specified data are excluded from the hit list.
  *Technical info: alphanumeric field, DB field: adr.text1*
- **Tel:** Customer's telephone number. The addresses whose telephone number does not include the specified data are excluded from the hit list.
  *Technical info: alphanumeric fields, DB fields: adr.telefon, adr.email*
- **E-mail:** Customer's e-mail address. The addresses whose e-mail address does not include the specified data are excluded from the hit list.
  *Technical info: alphanumeric fields, DB fields: adr.telefon, adr.email*
- **Incl. quick entry:** Specification of whether addresses are listed that are saved via quick entry.
  - ☑ The addresses from quick entry are displayed in the hit list.
  - ☐ No addresses from quick entry are displayed in the hit list.
  *Technical info: checkbox*

**Main del. address**
The market partner's main delivery address is displayed on the right above the tabs. If the market partner is not assigned a main delivery address, no main address is displayed.

**Address tab, Contact Data tab**
The columns on the item level correspond to the fields in the header area. ⇨ "Search fields" on page D-49
In addition, the following column is displayed:
- **First name:** Customer's first name.
  *Technical info: display field, DB field: adr.adrvname*

**Footer**
- **Details:** Opens a dialog with the details about the marked delivery address. Alternatively, you can open the dialog with `<F5>`. The button is only enabled if an address is marked in the hit list.
- **New Search:** Deletes all search criteria for a new search.
