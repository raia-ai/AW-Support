---
title: "EN_AWEnterprise_MasterData_3.00"
source: "EN_AWEnterprise_MasterData_3.00.pdf"
tags: ["A+W Enterprise", "Master Data", "Software Documentation", "ERP", "Glass Industry", "Windows and Doors", "Software Reference", "Market Partner", "Product Keys", "BOM"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive software reference manual for the A+W Enterprise \"Master Data\" module, version 3.0. It details the configuration and management of core data entities required for the A+W ERP system. The manual covers the creation and maintenance of market partners (customers, suppliers), employees, products, articles, bills of materials (BOMs), and various system and product keys. It provides descriptions for every dialog, tab, and field within the Master Data module, serving as an essential guide for system administrators and end-users responsible for data setup in the glass, windows, and doors manufacturing industry."
long_description: "The A+W Enterprise Master Data manual (Version 3.0) is an in-depth technical guide designed for users and administrators of the A+W Enterprise ERP software. This document focuses exclusively on the \"Master Data\" module, which forms the foundational data structure for all other operations within the system, including sales, purchasing, production, and financials. It outlines the procedures for creating, configuring, and managing essential business entities. Key sections include a detailed breakdown of \"Market Partners,\" covering everything from customer and supplier addresses to payment terms, discounts, and delivery routes. It also explains the setup for \"Articles\" and \"Products,\" which includes physical properties, size restrictions, bill of materials (BOM) management, pricing characteristics, and technical values like sound insulation and thermal properties. The manual systematically documents every user interface dialog, tab, and field, providing technical information, database field names, and usage notes. It also covers the configuration of system-wide parameters through \"System Keys\" and \"Product Keys,\" such as currencies, tax rates, units of measure, and processing rules. With screenshots and step-by-step descriptions, this reference is indispensable for ensuring accurate and consistent data management, which is critical for the seamless operation of the A+W Enterprise system in the specialized context of glass, windows, and doors manufacturing."
---

# A+W Master Data B

**A+W Enterprise**

**A+W - Software for Glass, Windows and Doors**

---
## Introduction

This part of the documentation contains editorial notes.

### Overview of revisions

| Part Version / Date | Descriptions |
| :--- | :--- |
| 3.0/03-2023 | Extended with new dialogs in the Key area |
| 2.2/03-2022 | Field description updated in the Market Partners, Products, Notes and Discounts sections. |
| 2.1/11-2020 | Complete reworking |
| 1.11/08-2013 | Conversion to CI 2013. |
| 1.10/01-2010 | New: Section Prices and Conditions. |
| 1.00/10-2006 | Original version. |

### Editorial

The Editorial provides information on the following topics:
- Product names
- Notes on this document
- Copyrights
- Trademark
- Contact

#### Product names

In the course of strategical reorganization, the product portfolio of A+W Software GmbH has been adapted. The product names have been adapted as well. ALCIB, for instance, will be called A+W Enterprise in the future.

Since the old as well as the new product versions have been adapted and extended in the product development cycle, we shall be using only the old product names in this document, referring to both the old and new product versions.

#### Notes on this document

This document is intended exclusively for end users of A+W Enterprise.

The documentation and software described are licenses that must only be used or copied in accordance with the conditions of our license agreement. The contents of the documentation are for information purposes only and are subject to changes without prior notice.

The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full program level of A+W Enterprise.

#### Copyrights

© 2023 A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation.

The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior approval in writing.

#### Trademark

All hardware and software names mentioned in this documentation can also be registered trademarks or other property rights of third parties. Third party copyrights have to be obeyed.

#### Contact

**A+W Software GmbH**
Am Pfahlgraben 4-10
35415 Pohlheim
+49 6404 2051-0
+49 6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

## Contents

- **Introduction** B-3
- **Overview of revisions** B-3
- **Editorial** B-3
- **Contents** B-5
- **Software Reference** B-11
- **Master Data - Overview** B-13
- **Market Partner** B-14
  - Market partner header B-14
  - Market partner - context menu B-16
  - Find Market Partner B-17
  - Address tab B-20
  - Market Partner - Note texts B-23
  - Identification tab B-25
  - References tab B-28
  - Order tab B-30
  - Delivery tab B-33
  - Invoice tab B-36
  - Customized tab B-38
  - Payment tab B-40
  - Printout tab B-43
  - Limits tab B-46
  - Assessment tab B-49
  - Production tab B-51
  - Modification tab B-52
  - Private tab B-53
- **Contact Person** B-54
- **Addresses** B-56
  - Site-specific address details B-59
- **Bank Accounts** B-60
- **E-Mail Addresses** B-61
- **E-Mail Addresses - Detail** B-63
- **Discounts** B-65
- **Discount - Details** B-66
- **Exchange/Additional Rules** B-67
- **Rack Types** B-68
- **Rack Types - Details** B-69
- **Configured Market Partner Fields** B-70
- **Sales Representative Allocation** B-71
- **User Allocation** B-72
- **Group Allocation** B-73
- **Project Allocation** B-74
- **Project Texts** B-75
- **Color Allocation** B-76
- **Bonus Allocation** B-77
- **Product Allocation** B-78
- **Market Partner Texts** B-80
- **Master Texts** B-81
- **MP Product Text** B-82
- **Forms** B-83
- **Document Types** B-84
- **Search Document** B-85
- **Market Partner Info** B-86
- **Replication Data** B-87
- **Configuration** B-89
- **Site Specific Details** B-90
- **Employee** B-91
  - Employee/Authorization Groups B-92
  - Employees - Rights B-97
- **Departments** B-99
- **Market Partner Keys** B-101
  - Titles-Descriptions B-103
  - Bonus B-104
  - Groups B-106
  - Group descriptions B-107
  - Industry descriptions B-108
  - Label Texts B-109
  - Calendar B-110
  - Special Calendar B-112
  - Customer Calendar B-114
  - Client Calendar B-116
  - FinAc Clients B-118
  - Countries B-119
  - Economic Area descriptions B-121
  - Areas/Counties B-122
  - General Quality Scale B-123
  - Quality Scale Dates B-125
  - Quality Scale Prices B-127
  - Quality Scale Quantities B-129
  - Quality Scale Special B-131
  - Reasons for Complaint B-133
  - Places of Complaint B-135
  - Types of Complaint B-137
  - Discount Methods B-139
  - Discounts B-143
  - Discounts - Details B-145
- **Site Specific Master Data** B-150
- **System Keys** B-151
  - Job Titles B-153
  - Zip Codes B-154
  - Languages B-156
  - Text Additions B-159
  - Document Types B-160
  - Quantity Units B-162
  - Edge Allocation B-164
  - Shape Descriptions B-166
  - Production Area B-168
  - Packing type B-169
  - Rack Packing Types B-170
  - Dispatch Type B-171
  - Incoterms B-173
  - Routes B-174
  - Route Details II B-177
  - Route Plan B-178
  - Dispatch Area Descriptions B-179
  - Vehicles B-180
  - Customs Exit B-181
  - Customs Destination Office B-183
  - Dispatch Groups B-184
  - Rack Status Descriptions B-185
  - Rack Groups Descriptions B-186
  - Packing Methods Descriptions B-187
- **Rack Packing Allocation** B-188
- **Currency** B-189
- **Tax Types** B-192
- **Tax Rates** B-194
- **Payment Type Descriptions** B-195
- **Cash Discount Groups** B-197
- **Cash Discount Groups** B-199
- **End of Period** B-200
- **Adhoc SQL Group Descriptions** B-201
- **Report texts** B-202
- **Companies** B-204
- **Company Allocation** B-205
- **Product Keys** B-207
  - Submenu Technical Values > Groups B-209
  - Submenu Technical Values > Vectors B-209
  - Submenu A+W iQuote-specific details B-210
  - Color Variants B-211
  - Color Descriptions B-213
  - Dimension variants B-214
  - Variants B-216
  - Size Variants B-217
  - Size Variants Descriptions B-218
  - Exchange/Additional Rules B-219
  - Exchange/Additional Rules - Details B-223
  - Exchange/Additional Rules - Test Mode B-225
  - dB Groups B-227
  - U Groups B-228
  - g Groups B-229
  - Transmission Groups B-230
  - Size Restriction Groups B-231
  - Thickness Groups B-232
  - Bending Strength Groups B-233
  - Vectors for Sound Protection (dB) B-234
  - Vectors for thermal properties (U) B-236
  - Vectors for total energz transmission (g) B-238
  - Transmission vectors B-240
  - Dimension restriction vectors B-242
  - Wind Load Vectors B-244
  - Notification Bodies B-245
  - Product Standards B-246
  - Priorities B-248
  - Product Information (CEKAL) B-249
  - CE Code (CPIP) B-251
  - Declaration of Performance B-251
  - Product Encoding B-253
  - Product Purposes B-256
  - Parameter Description B-258
  - Declar. of Perform. (entry) B-259
  - Descriptions for analysis groups B-260
  - Descriptions for fitting types B-261
  - Description for Foil Types B-263
  - Production Types B-264
  - Description for Spacer Types B-265
  - Descriptions for Sealing Types B-267
  - Motif Assignment B-268
  - Stack B-269
  - Descriptions for Box Signature B-270
  - Shaping/Nesting Product B-272
- **Template Parameter** B-273
- **ITOE Exchange Rules** B-274
- **Sash size set** B-276
- **Customer Products** B-277
- **Ordered Processings** B-279
- **Site-specific details** B-281
- **LAMI/CR Inheritance** B-282
- **Article groups-descriptions** B-283
- **Processing assignment** B-284
- **Processing assignment - Details** B-285
- **Processings for Shape Edges** B-287
- **Exchange group descriptions** B-289
- **Group Allocation (Article)** B-290
- **Group allocation (Spacers)** B-291
- **Article** B-292
  - Article header B-293
  - Article context menu B-294
  - Identification B-296
  - Article - Notes B-300
  - Physical Properties B-302
  - Size Restrictions B-307
  - Assembly Restrict. B-309
  - Supplies B-311
  - Production B-314
  - Prices B-318
  - Stock B-322
  - Technical Values B-324
  - Statistics B-326
  - Modifications B-328
  - Private B-329
- **Suppliers - Allocation** B-330
- **Market Partner Info** B-332
- **Size variants** B-335
- **Size variants - Details** B-336
- **Color/Size Variants** B-338
- **Color/Size Variants - Details** B-339
- **Compulsory sizes - Size parameter selection** B-341
- **Compulsory Dimensions - View 1** B-342
- **Compulsory Dimensions - View 2** B-344
  - Default calculation B-345
- **Article Sizes – Size parameters** B-346
- **Article dimensioning - Texts** B-349
- **Article Sizes - Item Sizes** B-351
- **Article Sizes - Other Parameters** B-353
- **Shape dimensioning** B-354
- **Delete product sizes** B-355
- **BOM** B-356
- **BOM Restrictions** B-357
- **Price Characteristics** B-358
- **Other Article Descriptions** B-361
- **Article Texts** B-363
- **Customer Article Texts** B-364
- **Project Article Texts** B-365
- **Forms** B-366
- **Master Texts - Text Editor** B-367
- **Supply Types** B-368
- **Send article to A+W CAD Designer (Bars)** B-370
- **Comparing fittings** B-371
- **Replication Data** B-372
- **Product Identification** B-373
  - Technical details B-376
  - Declared Services B-378
- **Configured Fields** B-379
- **Article Icons** B-380
- **Site specific article details** B-382
- **Site specific article details - Details** B-383
- **Site-specific supplier details** B-387
- **Site-specific details - variants** B-388
- **Site-specific details - colors/sizes** B-390
- **BOM** B-392
- **BOM** B-393
- **Formula editor** B-396
- **Product groups** B-398
- **Product groups** B-399
- **Individual product groups** B-401
- **Site-Specific Product Groups** B-402
- **Finished Products** B-404
  - Product Fixing B-405
  - Product Set B-406
- **Field Configuration** B-408
  - MP Field Configuration B-409
  - Article Field Configuration B-411
  - Document Field Configuration B-413
  - Reference Configuration B-415
- **Commission** B-417
  - Commission Code B-418
  - Commission Assignment B-419
- **Text Management** B-420
  - Current Texts B-421
  - Group Texts B-422
  - Project Texts B-423
  - Product Group Texts B-424
  - Configurable Texts B-425
  - Phrases B-426
  - Variable Description B-427
  - Text Formulas B-428
- **Costs** B-429
  - Cost Types B-430
  - Cost Units B-431
  - Cost Centers B-432
- **Prices** B-434
- **Conditions** B-435
- **List Printing** B-436
- **Partindex** B-437
- **Index** B-439

## Software Reference

## Master Data - Overview

Master data is changed only occasionally, if ever. It is the core of the entire system and is linked to all other areas. The goal of master data management is to create a single, continuous data stock for all applications in use.

All dialogs and functions that relate to master data are on this menu:

| Shortcut | Description |
| :--- | :--- |
| a | ⇨ "Market Partner" on page B-14 |
| b | ⇨ "Employee" on page B-91 |
| c | ⇨ "Departments" on page B-99 |
| da | ⇨ "Market Partner Keys" on page B-101 |
| db | ⇨ "System Keys" on page B-151 |
| dc | ⇨ "Product Keys" on page B-207 |
| dd | ⇨ Price keys are discussed in a separate document |
| e | ⇨ "Article" on page B-292 |
| f | ⇨ "BOM" on page B-392 |
| g | ⇨ "Product groups" on page B-398 |
| h | ⇨ "Finished Products" on page B-404 |
| i | ⇨ "Field Configuration" on page B-408 |
| k | ⇨ "Commission" on page B-417 |
| l | ⇨ "Text Management" on page B-420 |
| m | ⇨ "Costs" on page B-429 |
| n | ⇨ "Prices" on page B-434 |
| o | ⇨ "Conditions" on page B-435 |
| p | ⇨ "List Printing" on page B-436 |

> **Prices and conditions**
> The topics prices, conditions, and list printing are described in a separate document!

## Market Partner

The market partner master data stores all customer, project, and supplier-related details, as well as one-time data (partner type Other).

The details range from entries of the company address to supplier addresses, routes, payment terms, and assessments.

### Market partner header

After you have opened the dialog, you first have to select the market partner in the header area.

The contents of the individual tabs always relate to the market partner selected in the header.

In A+W Enterprise the following market partner types are distinguished:
- Customer
- Supplier
- Other
- Project
- Owner (racks)

**Partner type**
Toggle field for market partner type. The following options are available for selection:
- **Customer:** The customer master data includes all customer-related details, including the customer-specific article definitions. You need market partners of the type Customer especially when entering sales transactions.
- **Supplier:** The supplier master data includes all supplier-related details, including supplier-specific article details. You need market partners of the type Supplier especially when entering procurement transactions. Suppliers can be entered directly in orders and in the article master data as supplier for articles to be ordered.
- **Other:** Usually One-time customers are kept under this type, for whom only the address is created. Within the expanded internal client separation, the companies are created as Other.
- **Project:** A project normally refers to a larger building project. Definitions of a technical nature, conditions of a price nature (PU and SA), and other business agreements (quantities, time, etc.) are summarized under this term. This includes a planning and an informational component. Projects can be assigned market partners, sales and purchasing transactions.
- **Owners:** Owners of racks.
  Technical info: toggle field, DB field: mp.kuliflag

**Market partner**
Selection of the number or if known, input of the same. If a new market partner should be created, press <F6>.
⇨ "Find Market Partner" on page B-17
Technical info: <F9>, DB field: mp.kunr

**Matchcode**
With the selection of an existing market partner, the matchcode is displayed and with the entry of a new market partner, you have to enter a matchcode.
The matchcode is a free text field in which a short designation for the market partner is entered. The matchcode is used for simplified searching.

### Tab

The dialog offers various tabs. The contents of the individual tabs can - depending on the partner type - be different.
- ⇨ "Address tab" on page B-20
- ⇨ "Identification tab" on page B-25
- ⇨ "References tab" on page B-28
- ⇨ "Order tab" on page B-30
- ⇨ "Delivery tab" on page B-33
- ⇨ "Invoice tab" on page B-36
- ⇨ "Customized tab" on page B-38
- ⇨ "Payment tab" on page B-40
- ⇨ "Printout tab" on page B-43
- ⇨ "Limits tab" on page B-46
- ⇨ "Assessment tab" on page B-49
- ⇨"Production tab" on page B-51
- ⇨ "Modification tab" on page B-52
- ⇨ "Private tab" on page B-53

### Market partner - context menu

Master Data > Market Partner > F4

Via the context menu (<F4>) you have access to the following areas:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Contact data | ⇨ "Contact Person" on page B-54<br>⇨ "Addresses" on page B-56<br>⇨ "Bank Accounts" on page B-60<br>⇨ "E-Mail Addresses" on page B-61 |
| b | Discounts | ⇨ "Discounts" on page B-65 |
| c | Exchange/Additional Rules | ⇨ "Exchange/Additional Rules" on page B-67 |
| d | Rack Types | ⇨ "Rack Types" on page B-68 |
| e | Configured Market Partner Fields | ⇨ "Configured Market Partner Fields" on page B-70 |
| f | Employee Allocations | ⇨ "Sales Representative Allocation" on page B-71<br>⇨ "User Allocation" on page B-72 |
| g | Group Allocation | ⇨ "Group Allocation" on page B-73 |
| | Project Allocation | ⇨ "Project Allocation" on page B-74 |
| | Color Allocation | ⇨ "Color Allocation" on page B-76 |
| h | Bonus Allocation | ⇨ "Bonus Allocation" on page B-77 |
| i | Product Allocation | ⇨ "Product Allocation" on page B-78 |
| k | Texts/print | ⇨ "Market Partner Texts" on page B-80<br>⇨ "MP Product Text" on page B-82<br>⇨ "Forms" on page B-83<br>⇨ "Document Types" on page B-84 |
| l | Search Document | ⇨ "Search Document" on page B-85 |
| m | Market Partner Info | ⇨ "Market Partner Info" on page B-86 |
| n | Replication Data | ⇨ "Replication Data" on page B-87 |
| o | EDI Configuration | ⇨ "Configuration" on page B-89 |
| p | Site Specific Details | ⇨ "Site Specific Details" on page B-90 |

> **Context menu**
> The structure of the context menu depends on the market partner type.

### Find Market Partner

Master Data > Market Partner > Field Market Partner > <F9>

On this search dialog, you create the selection criteria for the market partner search.
As soon as you make an entry in the search fields, the hit quantity is adjusted automatically.
With the Details button, you start a dialog that lists the sites assigned to you (for multi-site).

> **Data**
> The data for this search dialog is loaded into the cache and is up-to-date at the time of loading.
> If you have made a change to the market partner master data, you have to click the [Refresh] button in order to update the data displayed on the search dialog.

The Address and Identification tabs in the hit area provide you with an overview of frequently-used data for market partners.

> **Quantity of data displayed**
> Since the quantity of data to be displayed can be extremely large (e.g. all customers in a country), not all existing data is loaded automatically into the cache for the search. The numbers at the top right of the hit quantity provide information about this. Ex.: if 1:100 (14873) is in the record display. This means that the first 100 entries (the hit quantity) of 14873 are loaded (into the cache). The number of entries to be loaded (into the cache) can be configured.

> **Buttons for scrolling**
> Use the |<, <<, >>, and >| buttons to scroll through the hit quantity. Use the >> button to scroll forward (16 entries). Use the << button to scroll backward (16 entries). Use the >| button to jump to the end of the cache (100th entry) and |< to jump to the beginning of the cache (1st entry). To load additional entries, click the [More Data] button. Then the configured quantity of data (in our case, 100 records) is loaded into the cache.

#### Description of the search fields

**From No.**
Entry of a number from which the search should start.
Technical info: numeric field, DB field: mp.mpnr

**Matchcode**
Entry of the matchcode as search value. You can enter the whole matchcode or only part of it.
Technical info: alphanumeric field, DB field: mp.mpmc

**Type**
Display of the market partner type you are searching for. It is pre-populated according to the selection on the market partner dialog and cannot be changed.

**Name**
Entry of the name as search value. You can enter the whole name or just a part of it (capitalization is not considered).
Technical info: numeric field, DB field: mp.name

**Name**
Entry of the first name as search value. You can enter the whole name or only part of it.
Technical info: alphanumeric field, DB field: mp.vname

**Street**
Entry of the street as search value. You can enter the whole street or only part of it.
Technical info: alphanumeric field, DB field: mp.strasse

**Site**
Selection and input of the site number/client number as search value. Entry here only makes sense if the extended multi-client system is configured since only then can market partners be assigned to a client.
Technical info: numeric field, <F9>, DB field: mp.hausnr

**Cntry**
Selection and entry of the country as search value. The appropriate codes can be assigned via the Country (Keys > Market Partner) menu.
Technical info: alphabetic field, <F9>, DB field: mp.kfz

**PCd**
Selection and entry of the postal code as search value. You can enter the whole postal code or only part of it.
Technical info: numeric field, <F9>, DB field: mp.plz

**City**
Selection and entry of the city as search value. You can enter the whole city or only part of it.
Technical info: alphabetic field, <F9>, DB field: mp.ort

**VAT ID No.**
Entry of the VAT identification number as search value. You can enter the whole number or just a part of it (capitalization is considered).
Technical info: numeric field, DB field: mp.steuernr

**Type**
Selection of the type as search value:
- **active:** Only active market partner are displayed.
- **closed:** Only closed market partners are displayed.
- **all:** All market partners are displayed.
Technical info: alphabetic field, <F9>, DB field: mp.still

### Address tab

Master Data > Market Partner

On this tab, you enter and/or edit the invoice address for the market partner. The tab is divided into a left and right side. The left side includes the market partner's address data and is present during the entire editing process. The right side displays the data from other tabs and additional options.

Use <F5> to open a dialog on which you can store note texts for the market partner.
⇨ "Market Partner - Note texts" on page B-23

Use <Shift><F5> to open a dialog on which you can store product note texts for the market partner.
⇨ "Article - Notes" on page B-300

Use <Shift><F9> to jump to the Matchcode field.

> **Asian installations**
> Asian installations include additional text fields for the input of addresses.

**Name**
Name of the market partner.
Technical info: alphabetic field, DB field: mp.name

**1stName**
First name of the market partner.
Technical info: alphanumeric field, DB field: mp.vname

**Title**
Selection of the title, e.g. Mr. or Mrs. (Master Data > Keys > Market Partner > Titles).
Technical info: <F9>, DB field: mp.anrede

**Attn.**
For the attention of. Name of the postal recipient for company addresses.
Technical info: alphabetic field, DB field: mp.zhd

**Addition**
Field for addition, e.g. the industry.
Technical info: alphabetic field, DB field: mp.branche

**Street**
Street for the address.
Technical info: alphanumeric field, DB field: mp.str

**PCd, POB**
The postal code corresponding to the post box and the number of the post box.
Technical info: alphanumeric field, DB field: mp.pfplz / mp.postfach

**PBox City**
The city assigned to the postal code.
Technical info: alphanumeric field, DB field: mp.pfplz / mp.pfort

**PCd, City**
Postal code corresponding to the city and the city
Technical info: alphanumeric field, DB field: mp.plz / mp.ort

**Country**
Country code and the corresponding country.
Technical info: alphanumeric field, DB field: mp.kfzcode / mp.land
⇨ "Countries" on page B-119

**Distance**
The distance between your company and the market partner in kilometers. Is used in the discount/surcharge calculation (e.g. transport surcharge) as scaling basis.
Technical info: numeric field, DB field: mp.kilometer

**Phone**
Telephone number of the market partner.
Technical info: numeric field, DB field: mp.telefon

**Fax**
Fax number of the market partner. With the toggle field next to this, you control whether the market partner would like to have the documents via fax. Possible values: Y/N. Is evaluated in the form printing and with appropriate configuration, allows the automatic faxing of documents to the market partner.
Technical info: numeric field, DB field: mp.faxnr

**E-mail**
Market partner's e-mail address. Use <F5> to store several e-mail addresses. Is evaluated in the form printing and with appropriate configuration, allows the automatic sending of documents to the market partner via e-mail.
Technical info: alphanumeric field, DB field: mp.email

**Website**
Market partner's URL. Start the browser with <F5>.
Technical info: alphanumeric field, DB field: mp.website

**Language**
Selection of the language in which the customer receives documents, e.g. German or English (Master Data > System > Languages). The texts are generated according to this definition during the document entry and with appropriate configuration, the expressions for market partners are created in the specified language.
Technical info: <F9>, DB field: mp.sprkz

**Notes**
The texts serve as important information in various parts of the program. This way, the entries can be displayed in the order entry with selection of the customer on the screen. There are two different note texts:
- <F5> starts the dialog for general note texts for the market partner.
- <Shift><F5> starts the dialog for product-related note texts for the market partner.
Technical info: DB field: memo.txt

**Additional information**
⇨ "Market Partner - Note texts" on page B-23
⇨ "Article - Notes" on page B-300

### Market Partner - Note texts

Master Data > Market Partner > F5

On this dialog, you can store texts for market partners; these serve as important information in various parts of the program. At the top of the dialog, you see the market partner number for which the text applies.

> **Multilingual note texts**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Notes. However, this is only possible if you are working with the multilingualism for employees within the internal client separation module.

**Language**
Language ID.
Technical info: numeric field, DB field: xsprbez.sprkz

Enter the text in the free field and store it with <F3>. Use <Shift><F9> to specify the info location:
- **Master data:** The text is only displayed in the master data.
- **Everywhere:** The text is displayed in the master data and in the sales and purchasing documents.
- **SA-order:** The text is displayed in the sales document.
- **PU-order:** The text is displayed in the purchasing document.

Use <Shift><F10> to specify the priority:
- **high:** The text is displayed automatically in the specified info locations as soon as just one line has the Prio=high.
- **Low:** The text will not be displayed automatically; it has to be loaded via menu at document entry.
Technical info: alphanumeric field, DB field: memo.txt

> **Priority of info position master data**
> If you have selected Master data as Info position, the priority low is invalid. The text will always be displayed in the market partner's master data.

### Identification tab

Master Data > Market Partner > Identification tab

On this tab, you enter and/or edit all tax and commission-related data for the market partner.

> **Left side of the dialog**
> During editing of the right side of the dialog, the customer's master data remains visible on the left side of the dialog. If changes are required, these have to be made on the Address tab.

**VAT ID No.**
EC tax number, that is, the VAT ID number. With the entry of the VAT ID No., there is a country-specific check. This number is used primarily in the FinAc transfer.
Technical info: alphanumeric field, DB field: mp.steuernr

**Taxpay. No.**
Specification of the taxpayer number that is used primarily in the FinAc transfer. It is also possible to configure the system so that entry of credits is not possible without Taxpay. No.
Technical info: alphanumeric field, DB field: mp.finstrnr

**Company Name**
Complete company name of the market partner, e.g. Schmidt GmbH & Co. KG.
Technical info: alphanumeric field, DB field: mp.firmname

**Ext. Supplier No**
If the market partner specifies its own supplier number, you can store it here. This field is used primarily in the FinAc transfer.
Technical info: alphanumeric field, DB field: mp.exlinr

**Ext. Customer No**
If the market partner specifies its own customer number, you can store it here. This field is used primarily in the FinAc transfer.
Technical info: alphanumeric field, DB field: mp.extkundnr

**Ext. Project No.**
This field is only active if the market partner is of the type. Then you can store an external project number here.
Technical info: alphanumeric field, DB field: mp.extkundnr

**Supplier No.**
Selection of the supplier number. If the market partner is a customer that also functions as supplier, then you can assign the supplier number here. This field is used primarily in the FinAc transfer.
Technical info: <F9>, DB field: mp.lieflinr

**Matchcode**
This field is used in connection with the Supplier No. field and shows you the supplier's matchcode.
Technical info: display field

**Misc MP**
This is a market partner that orders and is deliverd to just once. In contrast to other customers in the document entry, the address for this customer can be changed:
- **Yes:** This market partner is a miscellaneous market partner.
- **No:** The market partner is kept as a permanent customer.
Technical info: toggle field, DB field: mp.divers

**Commission**
Selection of the commission code. If the amount of the representative's commission depends on the customer, a numeric commission code has to be entered here. The commission rates for the various code values are stored in the Commission Code menu element (Master Data > Commissions). The field is only available with appopriate system configuration.
Technical info: <F9>, DB field: mp.provnr

**Sales Repres.**
Selection of the relevant sales representative. The respective commission rates for the representative entered here can be booked and they are ready for invoicing. These details can be changed later in the order. Prerequisite for the selection quantity is the function allocation Representative in the employee master data. With expanded internal client separation, this detail can also be entered client-specifically.
Technical info: <F9>, DB field: mp.vertrerloe

**Field Staff**
Selection of the responsible field service employee. These details are taken over in the order entry and if necessary, output on the customer's papers. These details can be changed later in the order.
Technical info: <F9>, DB field: mp.aussenmanr

**Intern.Repr.**
Selection of the responsible internal sales employee. These details are taken over in the order entry and if necessary, output on the customer's papers. These details can be changed later in the order.
Technical info: <F9>, DB field: mp.innenmanr

**Handled by**
Selection of the employee responsible for the order processing. This employee is taken over in the order and if necessary printed out on the customer's papers. These details can be changed later in the order.
Technical info: <F9>, DB field: mp.sachmanr

**Additional information**
⇨ "Market Partner - Note texts" on page B-23
⇨ "Article - Notes" on page B-300

### References tab

Master Data > Market Partner > References tab

On this tab, you enter and/or edit all FinAc technical and some of the price-relevant data for the market partner. The right side displays the address information.

#### Descriptions of fields

**FinAc Debtor**
Selection of the FinAc debtor number. It is a reference to the customer receiving the invoice. That's why the FinAc debtor and customer number should be the same. In case of central invoice management of a company with several locations, the FinAc debtor has to be assigned the customer number of the invoicing office to which the invoices are booked and issued.
Technical info: <F9>, DB field: mp.stddebnr

**Debtor statistics**
Selection of the statistics debtor. Regardless of the FinAc debtor, the statistical sales can be cumulated for other statistics debtors. This could be the customer number of an ordering branch office, for example. The statistical data provides information about the sales development of the individual branch offices.
Technical info: <F9>, DB field: mp.statdebnr

**Debtor conditions**
Selection of the customer number whose conditions should apply for the documents entered. With extended internal client separation, the debtor conditions can also be assigned client-specifically.
Technical info: <F9>, DB field: mp.konddebnr

**Debtor exch./add.**
Selection of the customer number. The exchange-addition rules that were stored for the customer that was noted in this field apply analogously in document entry.
Technical info: <F9>, DB field: mp.azdebnr

**Debtor**
Selection of whether debtor:
- **Yes:** The market partner is a debtor.
- **No:** The market partner is not a debtor.
Technical info: <F9>, DB field: mp.debitor

**Debtor site no.**
Is only active if the Debtor field has the entry Yes. Then you can assign the debtor a site. These details are only relevant with expanded internal client separation. For more details, see the A+W Enterprise configuration instructions.
Technical info: <F9>, DB field: mp.debhausnr

**Cond. branch**
Selection of the industry, e.g. carpenter, metal construction, etc. The appropriate conditions are stored on the Industry menu (Master Data > Keys > Market Partner > Industry).
Technical info: <F9>, DB field: mp.kbranche

**Economic area**
Selection of the economic area in which the market partner is located, e.g. France, Netherlands, Belgium, etc. The economic area is often used in a company's own statistical evaluations.
Technical info: <F9>, DB field: mp.kwrtraum

**Area**
Selection of the area in which the market partner is located, e.g. Hessia, Lower Saxony, Bavaria, etc. The areas are stored on the Region/States menu (Master Data > Keys > Market Partner > Region/States).
Technical info: <F9>, DB field: mp.region

**Cost Center**
Selection of the market partner's cost center, e.g. insulated glass, TG, racks, etc. Cost centers are logical business areas (departments, groups) incurring calculable costs. The selected cost center can be evaluated later. Cost centers are stored on the Cost Centers menu (Master Data > Cost Master Data > Cost Centers).
Technical info: <F9>, DB field: mp.kostenst

**Departm.**
Selection of a department, e.g. cutting, shipping, etc.
Technical info: <F9>, DB field: mp.abtnr

**Calendar**
Selection of a market partner-specific calendar number.
Technical info: <F9>, DB field: mp.kalnr

**Additional information**
⇨ "Market Partner - Note texts" on page B-23
⇨ "Article - Notes" on page B-300

### Order tab

Master Data > Market Partner > Order tab

All order-related information for the market partner is stored on this tab. The right side displays the address information.

#### Descriptions of fields

**Edge Prot.**
Selection of the desired edge protection item that should be applied for IGUs. This way, there is an automatic entry for the customer-exchange-addition rules, which are evaluated during order entry.
Technical info: <F9>, DB field: mp.kantschutz

**Std. glazing**
Selection of the desired glazing item that should be applied for IGUs. This way, there is an automatic entry for the customer-exchange-addition rules, which are evaluated during order entry.
Technical info: <F9>, DB field: mp.stdverglas

**Glazing**
Selection of where the glazing is displayed:
- Show in item and footer
- Calculate in item
- Show in footer only
Technical info: toggle field, DB field: mp.verglasung

**Proj. Force**
Definition of whether a project must be assigned to the customer in the order:
- **Yes:** A project must always be assigned to the customer in the order.
- **No:** Project assignment is optional.
Technical info: toggle field, DB field: mp.objmuss

**Ext.No.Req.**
Definition of whether a third-party number must be assigned to the customer in the order:
- **Yes:** A third-party number must always be assigned to the customer in the order.
- **No:** The assignment of a third-party number is optional.
Technical info: toggle field, DB field: mp.exaufmuss

**Refer. requ.**
Definition of whether a commission must be assigned to the customer in the order:
- **Yes:** A commission must always be assigned to the customer in the order.
- **No:** The assignment of a commission is optional.
Technical info: toggle field, DB field: mp.kommmuss

**Dimens. unit**
Selection of the dimensional unit:
- Metric
- Imperial
The system has to be configured appropriately for the use of the imperial dimensional unit.
Technical info: toggle field, DB field: mp.massystem

**Standard AIR**
Here you can specify the value for a standard spacer in mm. This value is then used to pre-populate IG items without fixed AIR in the order entry.
If a non-changeable AIR is defined for an IG article, the AIR of the article is used. If, however, the AIR is defined as changeable, the customer-specific AIR is used.
If the AIR is defined as changeable in the article master data, the customer-specific AIR can also be changed in the item entry.
Technical info: numeric field, DB field: mp.defszr

**min IG tot Thickn.**
Here you can specify the minimum thickness of a total IG unit.
Technical info: numeric field, DB field: mp.minszr

**max IG tot Thickn.**
Here you can specify the maximum thickness of a total IG unit.
Minimum and maximum thickness are checked within the restriction check in the order entry. If an order contains items that do not fulfill this restriction, the order can only be entered by authorized employees. For additional information, consult the A+W Enterprise EDP module description.
Technical info: numeric field, DB field: mp.maxszr

**Min. order value**
Here you can store a minimum order value (customer) or a minimum order value (for suppliers). This value is taken over as a calculation basis in the order. If the order value < minimum value, the minimum value is calculated.
The minimum order value must be specified in the customer currency. Otherwise, with a currency change in the order, there is no conversion of the minimum value.
Technical info: numeric field, DB field: mp.relimwert

**Additional information**
⇨ "Market Partner - Note texts" on page B-23
⇨ "Article - Notes" on page B-300

### Delivery tab

Master Data > Market Partner > Delivery tab

All information that relates to the supply of the market partner is stored on this tab. The right side displays the address information.

#### Descriptions of fields

**Stand. Route**
Selection of the route. For displatch planning, each customer should be assigned to a route. The route is taken over in the order; if necessary, it can be changed. From there, the route is transmitted to the dispatch control system. The routes are stored in the Routes menu element (Master Data > Keys > System > Dispatch > Routes).
Technical info: <F9>, DB field: mp.routenr

**Route 2-4**
Definition of alternative routes that can be used if the standard route does not optimally fit the customer's requested date. For delivery date determination in the order, it is then calculated whether an alternative route is cheaper. The fields Route 2-4 can only be changed if the system is not configured for routes from the address master data.
Technical info: <F9>, DB fields: mp.routenr2, routenr3, routenr4

**Load.Seq.**
Definition of the loading sequence. During the composition of a route, order items from different customers are loaded onto a truck. The sequence of the loading can be specified by the Load. Seq. The entry is made freely and displayed in the dispatch control system and can be evaluated on the loading papers. Use <F9> to get an overview of which loading sequences have already been assigned.
With use of the OTR module, the loading sequence is taken over from OTR.
Technical info: <F9>, DB field: mp.routeposnr

**Disp.Type**
Selection of the dispatch type, e.g. truck, transport company, etc. This field has only an informative character for the dispatch department. The dispatch types are created on the Packing Type menu (Master Data > Keys > System > Dispatch > Disp. Type).
Technical info: <F9>, DB field: mp.versandart

**Pack.Type**
Selection of the packing type, e.g. rack, box, pallet cage, etc. This field has only an informative character for the dispatch department. The packing types are created on the Packing Type menu (Master Data > Keys > System > Dispatch > Pack. Type).
Technical info: <F9>, DB field: mp.verpackart

**Incoterm**
Selection of the delivery condition, e.g. carriage free, self pick-up, etc. This text is intended for output on the customer papers. The delivery types are created on the Packing Type menu (Master Data > Keys > System > Dispatch > Suppliers).
Technical info: <F9>, DB field: mp.lieferart

**Collective Del. Note**
Selection of whether or not a collective delivery note is possible for the market partner:
- **Yes:** A collective delivery note is possible.
- **No:** A collective delivery note is not possible.
Technical info: toggle field, DB field: mp.lsammel

**Partial Shipment**
Selection of whether or not the market partner allows partial shipments.
- **Yes:** Partial shipments are allowed.
- **No:** Partial shipments are not allowed.
Technical info: toggle field, DB field: mp.teilliefkz

**Handling Time**
Is the time between the completion of the product and the day of delivery. Such a time can be necessary if the customer makes particular specifications for the picking of its goods. It is entered as a deadline and thus considered by the date and capacity planning. The time can be entered in days or hours (configurable).
Technical info: numeric field, DB field: mp.hzeit

**Call before delivery**
Selection whether or not the market partner should be contacted by telephone before delivery.
- **Yes:** The market partner would like to be called before delivery.
- **No:** No call is necessary.
Technical info: toggle field, DB field: mp.anruf

**Travel Time**
You can store the travel time to the market partner in days here. This value is then considered during the calculation of the delivery date.
Technical info: numeric field, DB field: mp.anfahrt

**Ship Via**
Selection whether the shipment is via another site. For more details, see the documents about plant logic.
Technical info: <F9>, DB field: mp.vsvia

**Type of EDI**
If this market partner is an internal customer, it is possible to define here how internal orders are exchanged via EDI. The setting especially affects how the addresses in the POs generated are treated:
- **none:** There is no automatic internal PO transmission.
- **SACoupling:** The parts to be ordered are from the order in the distributor. An order is generated directly in the supplier's system.
- **PU 1:1:** The parts to be ordered are from the order in the distributor. Here, first a corresponding PO is generated at the distributor and from it, an order is generated directly in the supplier's system. For this setting, a PO contains only ordered parts from an order.
- **PU 1:n:** The parts to be ordered are from the order in the distributor. Here, first a corresponding PO is generated at the distributor and from it, an order is generated directly in the supplier's system. Here, a PO can include ordered parts from several orders.
Technical info: <F9>, DB field: mp.dfuetyp

**Direct P.O.**
Selection for direct PO. The field is only active if the market partner is a supplier. This way, you control whether or not a PO is triggered immediately for this supplier after order release:
- **Yes:** PO is triggered immediately.
- **No:** The PO is not triggered immediately, but instead placed in the PO pool and can be triggered later.
Technical info: toggle field, DB field: mp.direktbestkz

**Delivery note transfer**
With this checkbox, you control the automatic delivery note transfer:
- The delivery note transfer is done automatically via OpenTRANS.
- There is no delivery note transfer.
Technical info: toggle field, DB field: mp.liefdfuekz

**Additional information**
⇨ "Market Partner - Note texts" on page B-23
⇨ "Article - Notes" on page B-300

### Invoice tab

Master Data > Market Partner > Invoice tab

All information that relates to the invoicing of the market partner is stored on this tab. The right side displays the address information.

#### Descriptions of fields

**Account**
9-digit account number. With the introduction of the IBAN, this field is no longer evaluated.
Technical info: numeric field, DB field: mp.konto

**Invoice Type**
Selection of the desired invoice form of the market partner:
- Individual invoice
- Cover invoice
- Collective invoice (weekly, every 14 days, monthly)
Technical info: toggle field, DB field: mp.rechnungsart

**Coll. Invoice Limit**
Here you enter how high the invoice limit for the collective invoices is.
Technical info: numeric field, DB field: mp.srechlimit

**Coll. Invoice Type**
Selection of the interval at which the collective invoices are written:
- weekly
- every 14 days
- monthly
Technical info: toggle field, DB field: mp.srechart

**FinAc**
If the connected financial accounting does not allow the separate transfer of various payment terms, this field can alternatively be provided with any alphanumeric code that is transferred to financial accounting. The concrete usage of this field depends largely on the FinAc system used.
Technical info: numeric field, SELO (<F9>), DB field: mp.fibukey

**Invoice Transfer**
Selection whether the invoice transfer in openTRANS format is possible.
- : Transfer is possible in the openTRANS format.
- : Transfer is not possible.
Technical info: toggle field,

**Calculate Racks**
Selection of whether or not the market partner allows partial shipments.
- **Yes:** Racks are invoiced.
- **No:** Racks are not invoiced.
Technical info: toggle field, DB field: mp.gsfaktura

**Rent-Free Days**
If you leave your customer the racks for a certain number of days when the racks do not cost anything, you can specify this number of days here.
Technical info: numeric field, DB field: mp.gsmietfrei

**Additional information**
⇨ "Market Partner - Note texts" on page B-23
⇨ "Article - Notes" on page B-300

### Customized tab

Master Data > Market Partner > Customized tab

The tab is only active if the market partner is an object and is configured appropriately. This tab summarizes all information that relates to the project. The right side displays the address information.

#### Descriptions of fields

**Sales Repres.**
Each project can be assigned a sales employee who is used as revenue representative for all orders participating in the project and flows into the representative commission
Technical info: <F9>, DB field: mp.vertrerloe

**Cost Center**
Whether the cost center should be replaced project-specifically in the order processing depends on the selected cost center procedure. If a project-related cost center assignment is desired, it can be set up by A+W.
Technical info: <F9>, DB field: mp.kostenst

**Proj. Force**
If the entry in this field is Y, a project must absolutely be entered in the order entry.
Technical info: toggle field, DB field: mp.kommmuss

**Limit check**
Project-oriented limit check:
- **FinAc Debtor:** Limit check during order entry.
- **MP project:** Project-oriented limit check.
Technical info: toggle field, DB field: mp.objlimitpruef

**Cred. Limit**
This field is only brought to bear if the Cred. Limit field is set to Y. If an order value including the open items and the open orders exceeds the credit limit stored here, a warning is issued.
Technical info: numeric field, DB field: mp.firmlimit

**VAT**
Selection of the VAT code. The necessary tax codes are stored on the Tax Types menu (Master Data > Keys > System > Taxes).
Technical info: <F9>, DB field: mp.mwst

**Discount 1/2**
Selection of the cash discount key. The required cash discount codes are stored on the Cash Discount Groups menu (Keys > System > Discount Groups).
Technical info: toggle field, DB field: mp.skonto1/2

**Invoice type**
Selection of the desired invoice form of the project:
- Individual invoice
- Cover invoice
- Collective invoice (weekly, every 14 days, monthly)
Technical info: toggle field, DB field: mp.rechnungsart

**Stand. Route**
Any project route applies during the order processing and replaces the customer route stored in the customer master data.
Technical info: toggle field, DB field: mp.routenr

### Payment tab

Master Data > Market Partner > Payment tab

All information that relates to the market partner's payment options is stored on this tab. The right side displays the address information.

#### Descriptions of fields

**Cash D. 1-3**
In the cash discount field, customer-specific cash discounts can be assigned as codes. Up to three scaled cash discounts are possible, whose term and percentage has to vary accordingly. The required cash discount codes are stored on the Cash Discount Groups menu (Codes > System).
Technical info: <F9>, DB field: mp.skonto1-3

**Consider Vacation**
Selection whether the cash discount period is extended if the invoice recipient is on vacation:
- The cash discount period is extended.
- The cash discount period is not extended.
Prerequisite is that the calendar for the invoice recipient in question is maintained.
Technical info: toggle field, DB field: mp.htag_skonto_rel

**Pay.Term**
This refers to the latest possible time of net payment. After expiry of the payment term, the dunning period begins. Entry is made in days.
Technical info: numeric field, DB field: mp.zahlziel

**Val.Date**
The value date in days determines the beginning of the cash discount periods and the payment term starting with the invoice date (including mailing time).
Technical info: numeric field, DB field: mp.valuta

**Charact.**
With this code, payment characteristics for market partner can be noted (debit, booking, etc.). The codes are stored on the Payment Characteristic menu (Codes > System).
Technical info: <F9>, DB field: mp.zahlngmerk

**Bonus**
Here you define whether and in what amount within which period of time the customer/project receives a bonus. The bonus is not calculated automatically. This specification serves only a company's own statistical purposes. The bonus codes are stored on the Bonus menu (Codes > System > Market Partner).
Technical info: <F9>, DB field: mp.bonus

**Paym. transact.**
Selection of the payment transaction:
- Direct debiting
- Prepayment
- On delivery
- By arrangement
- Check
- Bank debit
Technical info: toggle field, DB field: mp.azahlkz

> **Payment fields for Marktet partner type = Project**
> With appropriate system configuration, the fields Cach D.1 - Payment transaction can also be stored for projects. These payment conditions are then taken over in the block in the order insofar as the project is entered. If the fields in question remain empty for Project, the information is taken over from the customer master data.

**Reminder**
Selection whether in case of delay there should be a reminder.
- The customer will be reminded..
- The customer will not be reminded..
Technical info: toggle field, DB field: mp.mahnkz

**Remind.**
For information, it can be noted how many reminders have already been sent to the customer/project. This value can be transmitted to financial accounting if necessary.
Technical info: numeric field, DB field: mp.mahnanz

**Last CIC Inquiry**
Here you can enter the date of the last CIC inquiry.
Technical info: date field, DB field: mp.ltzschufa

**Partial invoicing**
Selection of whether or not the market partner allows partial invoicing.
- **Yes:** Partial invoices are allowed.
- **No:** Partial invoices are not allowed.
Technical info: toggle field, DB field: mp.teilfakkz

**Currency**
The multi-currency system is optional. Selection of the currency in which the market partner should be invoiced. The currency codes are stored on the Currency menu (Master Data > Keys > System).
Technical info: <F9>, DB field: mp.waehrung

**Calculate in**
The multi-currency system is optional. Selection of the current in which orders should be invoiced:
- Own currency
- Customer's foreign currency if the customer currency deviates from the company's own currency, e.g. customer in Switzerland.
Technical info: toggle field, DB field: mp.waehrprs

**Print in**
If you specified Foreign currency in the Calculate in field, then you control here in which currency the customer papers should be output. Possible values are:
- Calculated currency
- Foreign currency in the footer
- Foreign currency in item and footer
- Calc. currency + Euro in footer
- Calc. currency + Euro in item and footer
- Foreign currency + in footer
- Foreign currency + Euro in item and footer
Technical info: numeric field, DB field: mp.waehrdru

> **The fields Calculate in and Print in**
> The Calculate in and Print in fields are only accessible if the foreign currency module is licensed and a currency was assigned to the customer that deviates from the company's own currency.

### Printout tab

Master Data > Market Partner > Printout tab

All information that relates to the printing options for the market partner is stored on this tab. The right side displays the address information.

#### Descriptions of fields

**Print gross price**
Selection whether the gross price should be printed:
- Yes
- No
Technical info: toggle field, DB field: mp.preisdrkz

**Print MP-factor**
Selection whether the market partner factor should be printed:
- Yes
- No
Technical info: toggle field, DB field: mp.rabdrkz

**Print Process. Steps**
With this field, you control whether the processing prices should be generated already in the document entry in the processing texts to be printed:
- Yes
- No
- P: Configurable possibility for generating the processings only in the texts if they are present (processing price > 0)
Technical info: toggle field, DB field: mp.explbearbkz

**Sub-total**
Selection whether a commission-dependent subtotal should be printed:
- Yes
- No
Technical info: toggle field, DB field: mp.sumkomis

**OC incl. Muntins**
Selection whether the muntin structure should be printed with the order confirmation:
- Yes
- No
Technical info: <F9>, DB field: mp.sprossenab

**Gross/Net flag**
Selection for gross or net flag:
- **G:** Gross flag
- **N:** Net flag
Technical info: <F9>, DB field: mp.brutnetkz

**Cust.-indiv. items**
Selection for customer-specific item flags if there is an appropriate reference in the customer master data:
- **Item:** For customers who bear this flag, the customer item field is switched on in the order processing in order to enter the desired customer item designation. These details appear on all customer papers and labels.
- **Type:** This is the possibility for typical entry, as is frequently required for schedules of services for public bids. With this procedure, each product is assigned a specified typical designation in the course of the order entry. The printout of such an order confirmation shows in the item section only the respective type designation, while the precise product description appears in the footer of the document.
- **None**
Technical info: toggle field, DB field: mp.kndposkz

**Label**
Selection for label text The codes can be assigned via the Label Texts menu (Master Data > Keys > Market Partner).
Technical info: <F9>, DB field: mp.etikett

**Label Text**
If the market partner is a Project, you can enter another text for labels here.
Technical info: <F9>, DB field: mp.etitxt1

**Project Abbr.**
Since there is frequently little space available on labels, a two-letter project abbreviation can be printed on the label.
Technical info: alphanumeric field, DB field: mp.etitxt2

**Price Presentat.**
Selection for the price display on the papers according to the market partner's preference:
- No price
- QU price
- Unit price
- QU + unit price
Technical info: <F9>, DB field: mp.prsdarst

**Text Formulas**
Selection of the text formula.
Technical info: <F9>, DB field: mp.prsdarst

**Max. email size**
Maximum size of the e-mail with attachment in MBytes. When sending e-mail, by default the attachment is compressed in the zip format. With a system configuration, you can set whether the entire attachment is compressed or only if the attachment exceeds the e-mail size entered here in the field.
Technical info: <F9>, DB field: mp.mailsize

### Limits tab

Master Data > Market Partner > Limits tab

All information that relates to the market partner's limits is stored on this tab. The right side displays the address information.

#### Descriptions of fields

**Check limit via**
Selection of the limit check:
- **FinAc Debtor:** The limit check is done during order entry for the appropriate customer (FinAc debtor).
- **MP project:** The limit check is done during order entry if this project is assigned to the order and the system is configured appropriately.
Technical info: <F9>, DB field: mp.objlimitpruef

**Cred. Limit**
Amount in own currency up to which the company grants the customer credit. With appropriate configuration, the order value including the open items and the open orders is checked against the company limit stored here.
Technical info: numeric field, DB field: mp.firmlimit

**Insured up to**
The expiration date of the credit limit can be stored in this field.
Technical info: numeric field, DB field: mp.firmlimverfall

**Assu. Lim.**
Amount in own currency up to which the company grants the customer credit. With appropriate configuration, the order value including the open items and the open orders is checked against the assu company limit stored here.
Technical info: numeric field, DB field: mp.akvlimit

**Insured up to**
The expiration date of the insurance can be stored in this field.
Technical info: numeric field, DB field: mp.limverfall

**Limit check order**
With this field, you control what happens with orders whose order value including the open items and the open orders exceeds the limit stored in the fields Cred. Limit and Assu. Lim. If the employee has appropriate rights, the order can be entered and it will then land in a release pool (configurable). Orders that are in the release pool can only be released by authorized people. If the employee does not have these rights, he cannot enter the order:
- **Companies:** The value in the Cred. Limit field is used.
- **Assu. Lim.:** The value in the Assu. Lim. field is used.
- **Assu. + Cred. Limit:** The values in the Cred. Limit and Assu. Lim. fields are used.
- **None:** There is no limit check.
Technical info: <F9>, DB field: mp.limpruefkz

**Input Stop**
With this field, you control whether or not a document for this market partner may be entered when the limit is reached.
- **Only quotation:** When the limit is reached, no more quotations can be entered. Only orders can be entered for this market partner.
- **Only order:** When the limit is reached, no more orders can be entered. Quotations can still be entered for this market partner.
- **Order+Quotation:** When the limit is reached, neither quotations nor orders may be entered.
- **No:** No entry stop was entered for this market partner.
Technical info: toggle field, DB field: mp.erfasstop

**Delivery stop**
With this field you control whether or not a delivery note for this market partner may be printed if the limit is reached.
- **Yes:** There is no more delivery when the limit has been reached.
- **No:** With the reaching of the limit, orders can still be entered.
Technical info: toggle field, DB field: mp.lieferstop

**Invoice stop**
With this field you control whether or not an invoice for this market partner may be printed if the limit is reached.
- **Yes:** With the reaching of the limit, no more invoices can be issued.
- **No:** With the reaching of the limit, invoices can still be issued.
Technical info: toggle field, DB field: mp.fakturastop

**VAT**
Selection of the VAT code. The tax codes are stored on the Tax Types menu (Master Data > Keys > System > Taxes).
Technical info: <F9>, DB field: mp.mwst

**Int. VAT**
Internal VAT. The field is only active if the market partner is a supplier.
Technical info: <F9>, DB field: mp.mwstint

### Assessment tab

Master Data > Market Partner > Assessment tab

On this tab, you can assess the reliability, delivery time, quality, etc. The right side displays the address information.

#### Descriptions of fields

**Cat.**
Assessment of the class. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qklass

**Reliability**
Assessment of the reliability. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qzuverl

**Delivery Time**
Assessment of the delivery time. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qzeit

**Prices**
Assessment of the prices. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qpreis

**Quality**
Assessment of the quality. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qqual

**Service**
Assessment of the service. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qservice

**Consultation**
Assessment of the consultation. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qberat

**Courtesy**
Assessment of the courtesty. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qkulanz

**Fin.standing**
Assessment of the financial standing. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
Technical info: <F9>, DB field: mp.qbonitaet

### Production tab

Master Data > Market Partner > Production tab

The fields on this dialog served the transfer to PMS. With the introduction of A+W Production, the production transfer has changed. For additional information, please contact a service employee of A+W Software GmbH.

#### Descriptions of fields

**Determine prod. sequence**
Selection of whether a production sequence should be specified.
- **Yes:** Production sequence should be specified
- **No:** No production sequence is specified.
Technical info: toggle field, DB field: mp.prodfolge

**Rack Load**
This criterion determines the sort sequence on a rack, depending, e.g. on item, AIR, HM (hard dimension), etc.
Technical info: toggle field, DB field: mp.gbelad

**Rack weight (max)**
The maximum rack weight can be entered.
Technical info: <F9>, DB field: mp.gmaxgew

### Modification tab

Master Data > Market Partner > Modification tab

This tab shows when and by whom the market partner was created, when and by whom changes were made, and when the market partner was replicated. The right side displays the address information.

In the replication area area, you see at which sites the market partner was replicated.

**Additional information**
⇨ "Market Partner - Note texts" on page B-23
⇨ "Article - Notes" on page B-300

### Private tab

Master Data > Market Partner > Private tab

For individual evaluations or additional customer information, there are two alphanumeric fields available. On request, these can be given individual labels and configured in the system. For customer-specific adjustments, contact your A+W Software GmbH contact person.

**Additional information**
⇨ "Market Partner - Note texts" on page B-23
⇨ "Article - Notes" on page B-300

## Contact Person

Master Data > Market Partner > <F4> Contact Data > Contact Person

On this dialog, you can store various contact people for a market partner. Here, you can add more data records with <F6>.
With several stored contact people, use <F5> to determine a main contact.

### Descriptions of fields

**Name**
Last name of the contact.
Technical info: alphanumeric field, DB field: anspr.apname

**1stName**
First name of the contact.
Technical info: alphanumeric field, DB field: anspr.apvname

**Title**
Selection of the title for the contact. The appropriate keys can be assigned via the Titles (Master Data > Keys > Market Partner) menu.
Technical info: <F9>, DB field: anspr.anrede

**Departm.**
Contact's department.
Technical info: alphanumeric field, DB field: anspr.abteilung

**Position**
Contact's position.
Technical info: alphanumeric field, DB field: anspr.position

**Birthday**
Contact's birthday.
Technical info: numeric field, DB field: anspr.gebdat

**Phone**
Contact's telephone number, e.g. +4964042051-0.
Technical info: numeric field, DB field: anspr.telefon

**Fax**
Contact's fax number, e.g. +4964042051-877.
Technical info: numeric field, DB field: anspr.telefax

**Mobile**
Contact's mobile phone number, e.g. +491777500000.
Technical info: numeric field, DB field: anspr.telex

**E-mail**
Contact's e-mail address.
Technical info: numeric field, DB field: anspr.email

**Comment**
Text comment fields.
Technical info: alphanumeric field, DB field: adr.text1-3

## Addresses

Master Data > Market Partner > <F4> Contact Data > Addresses

You can assign the market partner additional addresses on this dialog. The invoice address is the main address and cannot be changed. You can add more data records with <F6>. If the delivery address is different from the main address, the corresponding address has to be determined as default address with <F5>.

### Descriptions of fields

**Name**
Last name or company name.
Technical info: alphanumeric field, DB field: adr.adrname

**1stName**
First name.
Technical info: alphanumeric field, DB field: adrvname

**Title**
Title, e.g. Mr., Mrs., company. The codes are stored in the Titles (Master Data > Keys > Market Partner) menu.
Technical info: <F9>, DB field: anspr.anrede

**Attn.**
For the attention of (last name, first name).
Technical info: alphanumeric field, DB field: adr.zhd

**Addition**
Enables entry of additional address information for output on customer papers.
Technical info: alphanumeric field, DB field: adr.branche

**Street**
Street name.
Technical info: alphanumeric field, DB field: adr.str

**PCd, POB**
Postal code and post box.
Technical info: numeric field/alphanumeric field, DB field: adr.pfplz/postfach

**POB City**
Postal box and city.
Technical info: numeric field/alphanumeric field, DB field: adr.pfort

**PCd.City**
Postal code and city.
Technical info: numeric field/alphanumeric field, DB field: adr.plz/ort

**Dispatch Region**
Selection of the dispatch region. The appropriate codes can be assigned via the Dispatch Regions (Master Data > Keys > System > Dispatch) menu.
Technical info: <F9>, DB field: adr.vsregion

**Country**
Selection of the country code. The appropriate codes can be assigned via the Countries (Master Data > Keys > Market Partner) menu.
Technical info: <F9>, DB field: adr.kfzcode

**Distance**
Distance to the delivery address in km.
Technical info: numeric field, DB field: adr.kilometer

> **Site-specific details about distance and travel time**
> Details about Distance and Travel Time should be entered per site (client) when using internal client separation. The entry dialog starts automatically in such a configuration.
>
> ⇨ "Site-specific address details" on page B-59

**Travel Time**
Duration of the travel time to the delivery address in days.
Technical info: numeric field, DB field: adr.fahrtzeit

> **Handling time, Arrival time and Unloading point**
> The fields Handling Time, Arrival Time and Unloading Point are only released with appropriate configuration.

**Handling Time**
Is the time between the completion of the product and the day of delivery. Such a time can be necessary if the customer makes particular specifications for the picking of its goods. It is entered as a deadline and thus considered by the date and capacity planning. The time can be entered in days or hours (configurable). The handling time can be stored per delivery address with appropriate configuration.
Technical info: numeric field, DB field: adr.handlingszeit

**Arrival Time**
Arrival time in HH:MM for delivery of the goods.
Technical info: numeric field, DB field: adr.ankunftszeit

**Unloading Point**
Place where the goods will be unloaded on delivery.
Technical info: numeric field, DB field: adr.anlieferstelle

**Fax Pho.**
Fax number and telephone number of the address.
Technical info: numeric field/alphanumeric field, DB field: adr.fax/telefon

**E-mail**
E-mail address.
Technical info: alphanumeric field, DB field: adr.email

**Std. Route**
Selection field. If the delivery address cannot be reached via the standard route stored in the customer master data, it is possible to assign the address to a separate route.
Technical info: <F9>, DB field: adr.routenr

**Remark**
Any information.
Technical info: alphanumeric field, DB field: adr.text1

> **Address logic**
> At the time of order entry, the stored default delivery address with the associated route number is taken over in the rules for the customer in question. If a default delivery address with separate route number has been stored for the customer, the route number entered in the customer master data is overridden. There are various deviations in this function; these are usually configuration-dependent. If you have questions or need additional information, contact the responsible A+W Software GmbH employee.

### Site-specific address details

On this dialog, you can store site-specific address data per site. This dialog appears automatically if you are using the internal client separation and you enter the Distance field on the Addresses dialog.
⇨ "Addresses" on page B-56

#### Descriptions of fields

**Site**
Selection of the site number.
Technical info: <F9>, DB field: mdzu.hnr

**Name**
The site name is displayed automatically in plain text when you leave the Site field.

**Distance**
Distance to the delivery address in km for the current site.
Technical info: numeric field, DB field: adr.kilometer

**Travel Time**
Duration of the travel time to the delivery address in days or hours for the current site.
Technical info: numeric field, DB field: adr.fahrtzeit

## Bank Accounts

Master Data > Market Partner > <F4> Contact Data > Bank Accounts

The market partner-specific bank details are stored on this dialog. Here, you can add more data records with <F6>. If there are several bank accounts, the main bank account has to be determined with <F5>.

### Descriptions of fields

**Bank name**
Name of the bank.
Technical info: alphanumeric field, DB field: bankv.bname

**Branch**
Branch of the bank.
Technical info: alphanumeric field, DB field: bankv.sitz

**Country**
Selection field. The country code.
Technical info: <F9>, DB field: bankv.kfzcode

**Bk.Cd**
Bank code of the bank.
Technical info: numeric field, DB field: bankv.blz

**Acc. No.**
Account number at the bank.
Technical info: numeric field, DB field: bankv.blz

**BIC**
Business Identifier Code.
Technical info: alphanumeric field, DB field: bankv.bic

**IBAN**
International bank account number.
Technical info: alphanumeric field, DB field: bankv.iban

## E-Mail Addresses

Master Data > Market Partner > <F4> Contact Data > E-mail Addresses

On this dialog, you have the possibility to store various e-mail addresses. The data stored is maintained in the associated database table xemail. It contains the details for the e-mail dispatch of forms. The MP type, market partner, form type, employee, and the department and the e-mail addresses can be specified here. If an employee is entered, no department can be entered. If a department is entered, no employee can be entered. It is possible to create values for a market partner and an employee (or a department), for a market partern, a form type, and an employee (or department) or just for a market partner. The e-mail address to which the form associated with the document is sent is determined precisely in this sequence when dispatching the forms.

The data stored here always relates to the document for which a form should be dispatched; that is, the employee number stored here has to match the person entering the document so that the appropriate e-mail address can be determined.

### Descriptions of fields

**Form**
Select the desired form (quotation, invoice, etc.).
Technical info: <F9>, DB field: xemail.formart

**Employ.**
Select the desired employee number. If the e-mail should not go to an employee but rather to a department, then leave this field blank and select the appropriate department in the Department field.
Technical info: <F9>, DB field: xemail.manr

**Departm.**
Select the department to which the e-mail should go. If you have entered an employee number in the Employ. field, you cannot make any entry in this field.
Technical info: <F9>, DB field: xemail.abtnr

**E-mail**
Enter the appropriate e-mail address here.
Technical info: alphanumeric field, DB field: xemail.email

**C**
If the e-mail address is one that has been closed for this form type:
- **Y:** The mail address is closed for this form type.
- **N:** The mail address is active for this form type.
Technical info: toggle field, DB field: xemail.still

**Additional information**
⇨ "E-Mail Addresses - Detail" on page B-63

### E-Mail Addresses - Detail

Master Data > Market Partner > <F4> Contact Data > E-mail Addresses > F2

This dialog displays additional information about the selected e-mail addresses.

#### Descriptions of fields

**Partn. Type**
The field is pre-populated with the partner type from which you opened the context menu. You can change the type.
Technical info: toggle field

**MktPt.**
The field is pre-populated with the market partner from whom you opened the context menu. You can change the market partner.
Technical info: <F9>, DB field: xemail.mpnr

**Form**
The field is pre-populated with the form that you selected on the previous dialog. You can change the form.
Technical info: <F9>, DB field: xemail.formart

**Employee**
The field is pre-populated with the employee that you selected on the previous dialog. You can change the employee.
Technical info: <F9>, DB field: xemail.manr

**Departm.**
The field is pre-populated with the department that you selected on the previous dialog. You can change the department.
Technical info: <F9>, DB field: xemail.abtnr

**E-mail**
The field is pre-populated with the e-mail address that you selected on the previous dialog. You can change the address.
Technical info: alphanumeric field, DB field: xemail.email

**E-mail from**
Different sender address when using this e-mail address.
Technical info: alphanumeric field, DB field: xemail.emailabs

**CC**
Additional CC address for use of this e-mail address.
Technical info: alphanumeric field, DB field: xemail.cc

**BCC**
Additional BCC address for use of this e-mail address.
Technical info: alphanumeric field, DB field: xemail.bcc

**Disp. Type**
Dispatch type of the file attachment:
- **0 (default):** One PDF file per e-mail
- **1:** Use several file attachments per e-mail
- **2:** Combine all file attachments into one PDF.
Technical info: alphanumeric field, DB field: xemail.bcc

**Password**
You can assign a password here.
Technical info: alphanumeric field, DB field: xemail.passwort

**Suspended**
The field is pre-populated with the flag that you set on the previous dialog. You can change the flag.
Technical info: toggle field, DB field: xemail.still

## Discounts

Master Data > Market Partner > <F4> Discounts

You assign the selected market partner discounts here. Key areas of the dialog are described in detail here:
⇨ "Discounts" on page B-143

The values for the respective discount method can be agreed upon individually per market partner and changed.

### Discount - Details

Master Data > Market Partner > <F4> Discounts > Details

This dialog presents a detailed view of the discounts. The dialog is described in detail here:
⇨ "Discounts - Details" on page B-145

## Exchange/Additional Rules

Master Data > Market Partner > <F4> Exchange/Additional Rules

The Exchange/Additional Rules menu element allows the storage of customer-specific rules according to which the BOM can be added and parts exchanged for individual articles or article types.

The dialog is described in detail here:
⇨ "Exchange/Additional Rules" on page B-219
⇨ "Exchange/Additional Rules - Details" on page B-223
⇨ "Exchange/Additional Rules - Test Mode" on page B-225

## Rack Types

Master Data > Market Partner > <F4> Rack Types

On this dialog, you specify on which racks the goods should preferably be delivered to a customer.
With use of priority-controlled packing optimization, a priority can also be specified, for which rack type is the most desirable and which is the least favored. The priority number can be selected between 1 and 100 and then specifies the sequence of the racks. Larger values cause a preferring of this rack type before others with lower priority values.
The information stored here uses the automatic rack planning to load the order as well as possible onto the racks preferred by the customer, heeding lite sizes and limits of the rack types For automatic rack planning, either the rack type or the main group can be stored here.

Use <F2> to reach the rack details dialog.
⇨ "Rack Types - Details" on page B-69

### Descriptions of fields

**Type**
Selection of the rack type. The rack types are stored in the Rack Types menu element (Logistics > Rack Management > Rack Master Data). After selecting the rack type, the associated designation appears in the second field.
Technical info: <F9>, DB field: kugest.gtypnr

**Main group**
Selection of the main group. The main groups are stored in the Main Groups menu element (Logistics > Rack Management > Rack Master Data). After selecting the main group, the associated designation appears in the last field. With use of the priority-controlled configuration, entry of the main group is not possible.
Technical info: <F9>, DB field: kugest.gtypnr

**Priority**
Rack priority from the customer's perspective. The field is only visible for customer-specific configuration.
Technical info: numeric field, DB field: kugest.prioritat

### Rack Types - Details

Master Data > Market Partner > <F4> Rack Types > F2

On this dialog, you can store a customer-specific packing text and define whether it should be printed on the packing order.
Return to the main dialog with <F2>.
⇨ "Rack Types" on page B-68

#### Descriptions of fields

**Text**
Customer-specific packing text.
Technical info: alphanumeric field, DB field: kugest.kuspectxt/kuspectxt1

**Purchase Flg**
Should the text be printed on the PO:
- Yes
- No.
Technical info: toggle field, DB field: kugest.bestelldru/bestelldru1

## Configured Market Partner Fields

Master Data > Market Partner > <F4> Configured MP-fields

Each field on this dialog is configured and evaluated customer-specifically. The fields can be defined under the menu element MP-Field Configuration (Master Data > Field Configuration).
⇨ "MP Field Configuration" on page B-409

The evaluation of the fields can only be designed individually. For additional information, please contact a service employee of A+W Software GmbH.
The data in the screenshot above serves only as an example.

## Sales Representative Allocation

Master Data > Market Partner > <F4> Employee Allocation > Representative Allocation

On this dialog it is possible to assign a customer several representatives (employees).
Selection is made with <F9>. Only those employees are available for selection to whom a representative function is assigned in the employee master data.
Use <F5> to specify a representative as main representative (= sales representative).

### Descriptions of fields

**Empl.no.**
Selection of the employee number. The name is displayed in the Sales Repr. field.
Technical info: <F9>, DB field: mitarbzu.manr

## User Allocation

Master Data > Market Partner > <F4> User Allocation

On this dialog it is possible to assign a customer several users (employees). Selection is made with <F9>.

### Descriptions of fields

**Empl.no.**
Selection of the employee number. The name is then displayed in the Operator field.
Technical info: <F9>, DB field: mperfasszu.manr

**Ord. Confirm.**
Use this field to control how the employee should receive copies of the OC to the customer. The following values are possible:
- **no:** The employee receives no copy of the OC.
- **via Email:** The employee receives the copy via e-mail.
- **via Fax:** The employee receives the copy via fax.
Technical info: toggle field, DB field: mperfasszu.abflag

## Group Allocation

Master Data > Market Partner > <F4> Group Allocation

On this dialog, a customer can be allocated to various groups with <F9>. Maintenance of the group codes is done on the Groups menu (Master Data > Market Partner).
The various market partner groups can be assigned various texts in the course of text processing (Master Data > Text Management > Group Texts) that can be output on the market partner's papers. This way, the market partner group Window Manufacturers can be informed about the introduction of a new insulated glass product.

### Descriptions of fields

**Group**
Selection of the group code. The name is then displayed in the Description field.
Technical info: <F9>, DB field: grpzu.grpnr

**Categ.**
Group classification. Via the defined Class, you can make statistical evaluations.
Technical info: numeric field, DB field: grpzu.klasskz

## Project Allocation

Master Data > Market Partner > <F4> Project Allocation

On this dialog, one or several projects (e.g. large construction sites) can be assigned to a customer. The projects are displayed with <F9> and entered with their project number.
use <F3> to open the dialog for customer-specific Project Texts in which you assign the project texts and define on which papers the text is printed.
Use <F5> to define the default project.

### Descriptions of fields

**Proj.**
Selection of the project number. The name of the project is then displayed in the Project Name field.
Technical info: <F9>, DB field: okkond.objnr

**Additional Information**
⇨ "Project Texts" on page B-75

## Project Texts

Master Data > Market Partner > <F4> Project Allocation <F3>

On this dialog, you assign a project text and determine on which papers the text will be printed.

### Descriptions of fields

**File**
Selection of the text file in which the texts are saved. If you enter a new file name, the Master Texts dialog opens, on which you can enter the new text.
Technical info: <F9>, DB field: objtxtzu.datei

**No**
Use this field to control the sequence in which the project texts are printed.
Technical info: <F5>, DB field: objtxtzu.lfdnr

**Printing pos.**
Selection of the printing position:
- Header text
- Footer text
Technical info: toggle field, DB field: objtxtzu.ludrupos

> **Forms**
> Use <F5> to specify on which form types (order confirmation, invoice, etc.) the files are printed in the sequence specified here.

**Additional information**
⇨ "Master Texts" on page B-81

## Color Allocation

Master Data > Market Partner > <F4> Color Allocation

This dialog is only available for Market partner type=Supplier. The data stored here is relevant for the BMECat master data import. This is an application for importing suppliers' article master data. During the import of a new supplier master data file, it is checked using the corresponding table lieffarbzu whether or not the colors of an item to be imported are already created in AWE as AWE colors. If it is detected that a supplier color is not yet created as AWE color, it is created during the import.
The dialog then delivers the overview of all created supplier colors to the user.
It can also happen that a color is needed for an order for a supplier that is not yet created because after the last supplier master data import from the supplier, new colors were made available. In this case, the new supplier color can be created manually via the dialog in order to enter the PO.

### Descriptions of fields

**No**
No The colors are stored on the Colors menu element (Master Data > Keys > Products > Variants > Colors).
Technical info: <F9>, DB field: lieffarbzu.farbnr

**AWE color**
AWE color designation. After the color number selection, the appropriate designation is displayed in this field.
Technical info: <F9>, DB field: lieffarbzu.farbnr

**No**
Supplier's color number.
Technical info: <F9>, DB field: lieffarbzu.lifarbnr

**Supplier's color**
Supplier's color designation
Technical info: <F9>, DB field: lieffarbzu.lifarbbez

## Bonus Allocation

Master Data > Market Partner > <F4> Bonus Allocation

You can assign the market partner a bonus on this dialog.

### Descriptions of fields

**Rank**
Specification for the priority. Use this field to control the allocation in the order entry to the individual order items. The lowest rank number with the most matching points in the product group will be used here.
Technical info: numeric field, DB field: bonuszu.rang

**PGRP Cd**
Use this field to allocate the bonus to a particular product group or product group range.
Technical info: <F9>, DB field: bonuszu.wagrp

**Remark**
You can store a remark here, e.g. why a bonus was awarded.
Technical info: alphanumeric field, DB field: bonuszu.txt

**Bonus**
Selection of the desired bonus. The appropriate codes can be assigned via the Bonus (Codes > Market Partner > Bonus) menu.
Technical info: <F9>, DB field: bonuszu.bonusnr

## Product Allocation

Master Data > Market Partner > <F4> Product Allocation

You can assign the market partner several articles with specific details on this dialog. Display the articles with <F9> and enter their article numbers.

### Description of the fields on the Overview tab

**Article**
Selection of the article number.
Technical info: <F9>, DB field: artkuzu.artnr

**Description**
Article description.

**Art. Type**
Article type of the selected article.

**Ext. Article**
Market partner's article number. With this number, the order item can be entered directly.
Technical info: alphanumeric field, DB field: artkuzu.kuartnr

**External Article Name**
Market partner's article name.
Technical info: alphanumeric field, DB field: artkuzu.kuartbez

**Price**
Customer article price. Depending on the price type, it is then calculated in the order.
Technical info: numeric field, DB field: artkuzu.preis

**Type**
Price type:
- **CU/piece:** currency unit per piece.
- **CU/QU:** currency unit per quantity unit.
Technical info: toggle field, DB field: artkuzu.ptyp

### Description of the fields on the Details tab

**Preferred suppl**
Enter the market partner's favorite supplier for this article in this field.
Technical info: <F9>, DB field: artkuzu.liwunsch

**Additional Name**
Enter the additional name this partner uses for the article in these fields. There are three fields for this purpose. Enter the field with <Enter>.
This name will override the article name in document management (for this customer).
Technical info: alphanumeric field, DB field: artkuzu.zusatz1, artkuzu.zusatz2, artkuzu.zusatz3

**EAN Code**
Enter the EAN code this market partner uses for the article in this field. This will be printed on all customer-bound documents. The EAN code can be used to convert external articles into A+W Enterprise articles at automatic order import.
Technical info: numeric field, DB field: artkuzu.eancode

**Spacer Text No.**
Enter the spacer text number the partner uses for an IG article in this field. The text formula is entered on the Text management > Text creation > Text formula menu.
This formula is analyzed when text is created at order entry, and will be printed on the spacer.
Technical info: numeric field, DB field: artkuzu.rahmtxtnr

**Size 1-20**
You can enter article sizes used by the market partner in these fields. These will override the values from the parameters defined for this article during article dimensioning.

> **There will be no feasibility check!**
> Your entries here have to make sense.

Technical info: numeric fields, DB fields: artkuzu.gv1 - artkuzu.gv20

## Market Partner Texts

Master Data > Market Partner > <F4> > Text/Print > MP Texts

On this dialog, you assign market partner texts for printing on the forms.
Use <F3> to open a dialog on which you can store the master texts.

> **Forms**
> Use <F5> to specify on which form types (order confirmation, invoice, etc.) this file is printed in the sequence specified here.

### Descriptions of fields

**File**
Selection or input of the text file in which the texts are saved.
Technical info: <F9>, DB field: kltxtzu.dateiname

**No**
Use this field to control the sequence in which the market partner texts are printed.
Technical info: <F5>, DB field: kltxtzu.lfdnr

**Printing pos.**
Selection of the printing position:
- **Header:** The file is printed in the header.
- **Footer:** The file is printed in the footer.
Technical info: toggle field, DB field: kltxtzu.ludrupos

**Additional information**
⇨ "Master Texts" on page B-81

## Master Texts

Master Data > Market Partner > <F4> > Text/Print > MP Texts > <F3>

On this dialog, new text blocks are entered and managed in several languages for printout of the forms. With this it is possible, for example, to store Christmas greetings, general customer notes or text for advertising campaigns in order to print them out on the customer-bound papers.

### Descriptions of fields

**File**
Name of the text file in which the texts are saved.
Technical info: alphanumeric field, DB field: xtxtnr.datei

**Language**
Selection of the language. Only the languages are available for selection that are stored in the system master data (Master Data > Keys > System > Languages)
Technical info: <F9>, DB field: xtxtnr.sprkz

**Text**
Entry of the appropriate text. Multi-line inputs are possible. A maximum of 160 characters on a line can be entered. The individual lines are distinguished with the sequence number.
Technical info: alphanumeric field, DB field: stammtxt.stammtxt, stammtxt.seqnr

**Additional information**
⇨ "Market Partner Texts" on page B-80

## MP Product Text

Master Data > Market Partner > <F4> > Text/Print > MP Product Text

This dialog is used to store market partner-specific article texts in different languages. Depending on the customer language code, these texts can be output on the forms.

### Descriptions of fields

**Article**
Selection of the appropriate article number. The article description appears in the field here.
Technical info: <F9>, DB field: artxtzu.artnr

**File**
Name of the text file in which the texts are saved. Use <F3> to switch to the Master Data dialog where you can store new texts.
Technical info: alphanumeric field, DB field: artxtzu.datei

## Forms

Master Data > Market Partner > <F4> > Text/Print > Forms

On this dialog, it is possible to store a customer-specific report for the existing form type.

### Descriptions of fields

**Form**
Select the desired form type (quotation, invoice, etc.). The description is then displayed in the Description field.
Technical info: <F9>, DB field: kundruckanz.formart

**Copies**
Determines the customer-specific default output quantity of the form.
Technical info: numeric field, DB field: kundruckanz.anzahl

**Comm**
With this field, you control whether commission texts should be output.
- Commission texts are printed.
- ☐ Commission texts are not printed.
Technical info: toggle field, DB field: kundruckanz.kommdrkz

**Report name (w.o. extension)**
Different, customer-specific report name.
Technical info: alphanumeric field, DB field: kundruckanz.repname

## Document Types

Master Data > Market Partner > <F4> > Text/Print > Document Types

On this dialog, you can store various document types and the type of output. The dialog is described in detail here:
⇨ "Document Types" on page B-160

## Search Document

Master Data > Market Partner > <F4> > Search Document

Use of the document search was already discussed in the chapters Sale and Purchasing; please consult those sections for details!

## Market Partner Info

Master Data > Market Partner > <F4> > MP Info

Various statistical information about the market partner is kept under this element:
- Amounts of open items for a FinAc connection
- Amounts of unpaid invoices (open items)
- Amounts of orders in progress (not yet invoiced)
- Date, number, site, and amount for the last order, the last quotation, and the last invoice
- Total sales in the current year.

### Descriptions of fields

**Cust.**
Selection of the customer number. The customer name is displayed in plain text after the number is selected.
Technical info: <F9>, DB field: kuplus.kunr

> **Market Partner Info**
> The fields on this dialog are for information purposes only and cannot be changed. The amounts are taken from the database table kuplus. The remaining fields are determined from daily business and displayed.

## Replication Data

Master Data > Market Partner > <F4> > Replication Data

Depending on the configuration, on this dialog you can specify a limit distribution for the individual branch offices.

### Descriptions of fields

**tot. Limit**
Display of the company limit. The value comes from the Company Limit field (Master Data > Market Partner > Limits tab).
Technical info: display field

**tot. Assu.Lim.**
Display of the assu. limit. The value comes from the AKV Limit field (Master Data > Market Partner > Limits tab).
Technical info: display field

**Site**
Selection of the site for which the limit data applies.
Technical info: <F9>, DB field: limits.hausnr

**Limit**
Company limit for the appropriate site. If you leave the field, in the next field you will see the percentage that this value represents in relation to the total limit.
Technical info: <F9>, DB field: limits.limit

**Assu. Lim.**
Assu. company limit for the appropriate sites. If you leave the field, in the next field you will see the percentage that this value represents in relation to the total assu. limit.
Technical info: <F9>, DB field: limits.akvlimit

**Route**
Selection of the route. In the next field, you will see the route name. The Routes and their Names are stored under Master Data > Keys > System > Dispatch > Route > Routes.
Technical info: <F9>, DB field: limits.routenr

**Def.Site**
Default site for the clients. Use <F5> to select the current site as default site for all entries.
Technical info: <F9>, DB field: limits.defhausnr

> **Insured up to**
> Neither the total limit nor the total assu. limit can be exceeded. If they are exceeded, there will be a message to that effect.

> **Lower dialog area**
> In the lower dialog area, you will see the total values both for the amounts as well as for the percentages.

## Configuration

Master Data > Market Partner > <F4> > EDI Configuration

On this dialog, you configure the control of the EDI.
For additional information, please contact a service employee of A+W Software GmbH.

### Descriptions of fields

**Partn. Type**
Selection of the partner type.
Technical info: <F9>, DB field: mpdfuectrl.kuliflag

**Market partner**
Selection of the market partner number. The customer name is displayed in plain text after the number is selected.
Technical info: <F9>, DB field: mpdfuectrl.mpnr

**Type of EDI**
Selection of the EDI type. In the next field, you will see the description. Type of EDI decides about the type and manner of data transmission and should be selected very carefully. You can make the selection in the dialog header. In this case, new configuration entries can also only be made for this Type of EDI.
Technical info: <F9>, DB field: mpdfuectrl.dfuetyp

**Control Mode**
Control mode of the EDI. In the next field, you will see the description.
Technical info: <F9>, DB field: mpdfuectrl.id

**Val.**
Control value.
- The EDI type is active.
- The EDI type is not active.
Technical info: <F9>, DB field: mpdfuectrl.value

## Site Specific Details

Master Data > Market Partner > <F4> > Site Specific Details

The site-specific details are used for the multi-site system. Here you can assign individual representatives and condition debtors to different sites.

### Description of the fields

**Site**
Selection of the site number.
Technical info: <F9>, DB field: mdzu.hnr

**Name**
The site name is displayed automatically in plain text when you leave the Site field.

**Sales Repres.**
Selection of the relevant sales representative. The respective commission rates for the representative entered here can be booked and they are ready for invoicing.
Technical info: <F9>, DB field: mpmdzu.lager

**Name**
Name of the representative responsible for the sales is displayed automatically in plant text when you leave the Sales Repres. field.

**Debtor conditions**
Selection of the customer number whose conditions should apply for the documents entered.
Technical info: <F9>, DB field: mpmdzu.konddebnr

**Name**
The customer name is displayed automatically in plant text when you leave the Debtor conditions field.
Technical info: <F9>, DB field: mp.name

**VAT**
Selection of a VAT. If the sites are in different VAT areas, the differing VAT for a market partner can be specified here.
Technical info: <F9>, DB field: mpmdzu.mwst

**VAT (%)**
After selecting the VAT, the name is displayed here in plain text.
Technical info: <F9>, display field

## Employee

Master Data > Employee

All identifying details (such as employee number, name, code, etc.) for the employee, system services, and authorization groups are specified in the employee master data.

In addition, all EDI rights and restrictions that affect the employee or an authorization group are stored here. This makes sure that employees can access only certain areas, and are given the appropriate rights in A+W Enterprise.

This chapter provides information on the following subjects:
- "Employee/Authorization Groups" on page B-92
- "Employees - Rights" on page B-97

### Employee/Authorization Groups

Master Data > Employee

All details about employees, employee groups, and system services are stored on this dialog.

#### Description of the fields in the Employee Data section

**Empl. No.**
Selection of the employee number. If this is a new employee, enter the desired number.
Technical info: <F9>, DB field: mitarb.manr

**Type**
This field specifies the type of master data record. The following values are possible:
- **Employee:** Each employee number can only be assigned once. With <F6> you have the opportunity to let the system assign the next free number.
- **System service:** An employee record with employee number -1 should be created as system service. The existence of this record is necessary since all A+W Enterprise background processes (e.g. background order processing, etc.) report with employee number -1.
- **Authorization group:** An authorization group is created with program access rights for a particular personnel area. Employees in this task area are then assigned the group number in the Authorization Group field. This eliminates the assignment of the individual group-specific module access authorizations for each individual employee.
Technical info: toggle field, DB field: mitarb.matyp

**Name**
Employee's last name. Use <F5> to open the Remark Texts dialog on which you can store the information about the employee. Use <F3> to open the dialog for the overview of the employee rights.
Technical info: alphabetic field, DB field: mitarb.maname

> **Employee and department notes**
> Employee and department notes with priority high and location everywhere can be displayed directly when starting the A+W Enterprise main menu or when starting the Dispatch module. This way, important employee-related information can be presented at the start. Your system must be configured appropriately.

**1stName**
Employee's first name.
Technical info: alphabetic field, DB field: mitarb.mavname

**Sex**
Toggle field. Employee's sex.
- female
- male
Technical info: toggle field, DB field: mitarb.sex

**Title**
Selection of the title. The appropriate codes can be assigned via the Titles (Master Data > Keys > Market Partner) menu.
Technical info: <F9>, DB field: mitarb.anrede

**Birth Dt.**
Employee's date of birth
Technical info: numeric field, DB field: mitarb.gebdat

**Initials**
Employee's initials.
Technical info: alphanumeric field, DB field: mitarb.zeichen

#### Description of the fields in the Last Modification section

**Name**
This field displays the employee who made the last modification to the master data record.

**Date**
This field displays the date on which the master data record was last modified.

#### Description of the fields in the Login Information section

**Login**
A+W Enterprise Login name, which together with the password permits the user to start the program. When using the A+W Enterprise Web application and A+W iQuote, the name entered here is also used for login.
Technical info: alphanumeric field, DB field: mitarb.loginname

**Password**
Password, which together with the A+W Enterprise login name entitles the employee to start the program. The password can only be entered or changed by the administrator. For the use of the A+W Enterprise standard application, the password is assigned via the Unix or Linux administrator. The password from this field entitles the employee to log into the A+W Enterprise Web application or A+W iQuote.

#### Description of the fields in the Restrictions section

**Shell**
Shell authorization. If the operating system level should also be accessible, please check this box.
Technical info: toggle field, DB field: mitarb.shjn

**Department Restriction**
If this checkbox is active, various evaluations (e.g. list of uninvoiced orders, production release, etc.) are restricted to the documents of the department to which the employee is assigned.
Technical info: toggle field, DB field: mitarb.abtview

**Client Limitation**
If this checkbox is active, various evaluations (e.g. list of uninvoiced orders, production release, etc.) are restricted to the documents of the client.
Technical info: toggle field, DB field: mitarb.hausview

#### Description of the fields in the Employee/Contact Data section

**DirectNo.**
Internal telephone extension.
Technical info: numeric field, DB field: mitarb.durchw

**Fax**
Fax number.
Technical info: numeric field, DB field: mitarb.faxnr

**E-mail**
Employee's e-mail address.
Technical info: alphanumeric field, DB field: mitarb.email

**Client**
Plant or branch office number (main client). Use <Shift> + <F5> to open the dialog for the site assignment. There, you can assign the employee to additional sites.
Technical info: alphanumeric field, DB field: mitarb.hnr

**Job Title**
Selection of the employee's job title.
Technical info: <F9>, DB field: mitarb.pos

**Function**
Selection whether the employee is active as managing director or sales representative. This way, e.g. only people who are identified as sales representatives can be assigned as such to a customer in the customer master data.
Technical info: <F9>, DB field: mitarb.funktion

**Mail subs.**
Selection of the employee number for the forwarding of an e-mail.
Technical info: <F9>, DB field: mitarb.vertretung

**activate**
With this checkbox, you activate the e-mail forwarding.
Technical info: toggle field, DB field: mitarb.vertr_aktiv

**Departm.**
Number of the department. For statistical program access reasons, each employee should be assigned to a department. The department is then displayed in the next field. The appropriate departments are assigned via the menu by the same name.
Technical info: <F9>, DB field: mitarb.abtnr

**Customer**
Here you can assign a customer to the employee.
Technical info: <F9>, DB field: mitarb.manrkunr

**External Employee**
Activate the checkbox if this is an external employee (with restricted rights).
Technical info: toggle field, DB field: mitarb.externflag

**SQL authorization group**
Selection of the authorization group.
Technical info: <F9>, DB field: mitarb.logingrp

#### Description of the fields in the RightGroups section

**Group**
Selection of the group number. The description is displayed in the next field. This eliminates the assignment of the individual group-specific module access authorizations for each individual employee.
Technical info: <F9>, DB field: bengrpzu.grp

**Site**
Selection of the assigned site number.
Technical info: <F9>, DB field: bengrpzu.hausnr

#### Description of the fields in the Rights section

**EDP Mod.**
Selection of the EDP module in which the employee can exercise his or her EDP rights. * stands for all program modules. The module description is displayed in plain text in the next field. Use <F9> to search for a particular module. For the overview of all modules and their significance, please contact a A+W Software GmbH employee.
Technical info: <F9>, DB field: login.modul

**Terminal**
Selection of the terminal or terminal group for which the employee has rights for the module in question. * stands for all terminals.
Technical info: <F9>, DB field: login.ort

**Rights**
Selection of the employee rights:
- **-:** No rights.
- **r:** Read right
- **w:** Write right
Technical info: toggle field, DB field: login.rwx

**Site**
Selection of the assigned site number in which this restriction applies (for multi-site systems). The site-specific restrictions can only be made for local rights. For additional information, consult the responsible A+W Software GmbH employee.
Technical info: <F9>, DB field: login.hausnr

### Employees - Rights

Master Data > Employee > Rights (Overview) <F3>

On this dialog, you specify the employee number and site number for which you would like to see the rights.

#### Descriptions of fields

**Employee**
Entry of the employee number.
Technical info: numeric field

**Site**
Entry of the site number.
Technical info: numeric field

If you leave the dialog with [OK], the desired information is displayed on the next dialog:

#### Descriptions of fields

**Module**
Display of the module number. A * stands for all modules.
Technical info: display field

**Right**
Display of the right:
- **-:** No rights.
- **r:** Read right
- **w:** Write right
Technical info: display field

**User/Group**
Here you can see whether this is a user right or a group right:
- **U:** User right
- **G:** Group right
Technical info: display field

**Print**
With this button, you can print out the overview of employee rights.

## Departments

- Master Data > Departments > Descriptions
- Master Data > Departments > Individual Descriptions
- Master Data > Departments > All Descriptions

All of the identifying details (such as name, abbreviation, etc.) for the departments at the company are specified on this dialog.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Departments.

Use <F5> to open the Remark Texts dialog on which you can store the information about the department.

> **Employee and department notes**
> Employee and department notes with priority high and location everywhere can be displayed directly when starting the A+W Enterprise main menu or when starting the Dispatch module. This way, important employee-related information can be presented at the start. Your system must be configured appropriately.

### Descriptions of fields

**Departm.**
Selection of the department.
Technical info: <F9>, DB field: abteilung.abtnr

**Abbreviation**
Displays the abbreviation for the name.
Technical info: alphanumeric field, DB field: abteilung.abtid

**Description**
Department description. The description can be overwritten.
Technical info: alphanumeric field, DB field: abteilung.bez

**Cost Center**
Selection of the cost center. The entry can be used for statistical purposes. The appropriate codes can be assigned via the Cost Center (Master Data > Cost Center) menu.
Technical info: <F9>, DB field: abteilung.kostenst

**Message for**
Selection of the message recipient. The system message recipient of the department is the person or group of people who receive messages from other employees of this department.
Technical info: <F9>, DB field: abteilung.manr

**Form group**
An entry in the form group that uses this department is taken into consideration when printing forms. Generally one form group per department is stored.
Technical info: numeric field, DB field: abteilung.formgrp

**Fax**
If there is an individual fax connection, this number can be stored here.
Technical info: numeric field, DB field: abteilung.faxnr

**Last Change**
This field displays the employee who made the last change to the data and the corresponding date.

**Langu.**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

## Market Partner Keys

Master Data > Keys > Market Partner

In this area, characteristics for describing the market partner (customer, supplier, etc.) are created. They are then available for the entry of the market partner. The individual characteristics are explained below.

You have access to the following areas:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a a/b | Titles | ⇨ "Titles-Descriptions" on page B-103 |
| b | Bonus | ⇨ "Bonus" on page B-104 |
| ca | Groups | ⇨ "Groups" on page B-106 |
| c b/c | Group designations | ⇨ "Group descriptions" on page B-107 |
| d a/b | Industries | ⇨ "Industry descriptions" on page B-108 |
| e | Label Texts | ⇨ "Label Texts" on page B-109 |
| fa | Calendars | ⇨ "Calendar" on page B-110 |
| fb | Special Calendar | ⇨ "Special Calendar" on page B-112 |
| fc | Customer Calendar | ⇨ "Customer Calendar" on page B-114 |
| fd | Client Calendar | ⇨ "Client Calendar" on page B-116 |
| g | FinAc Clients | ⇨ "FinAc Clients" on page B-118 |
| ha | Countries | ⇨ "Countries" on page B-119 |
| h b/c | Country names | ⇨ "Countries" on page B-119 |
| i a/b | Economic Areas | ⇨ "Economic Area descriptions" on page B-121 |
| ja/b | Region/Federal states | ⇨ "Areas/Counties" on page B-122 |
| ka | Quality Scale | ⇨ "General Quality Scale" on page B-123 |
| kb | Qual. scale dates | ⇨ "Quality Scale Dates" on page B-125 |
| kc | Qual. scale prices | ⇨ "Quality Scale Prices" on page B-127 |
| kd | Qual. scale quantities | ⇨ "Quality Scale Quantities" on page B-129 |
| ke | Qual. scale special | ⇨ "Quality Scale Special" on page B-131 |
| la | Reason for Complaint | ⇨ "Reasons for Complaint" on page B-133 |
| lb | Places for Complaint | ⇨ "Places of Complaint" on page B-135 |
| lc | Types of Complaint | ⇨ "Types of Complaint" on page B-137 |
| ma | Discount Methods | ⇨ "Discount Methods" on page B-139 |
| na | Discounts | ⇨ "Discounts" on page B-143<br>⇨ "Discounts - Details" on page B-145 |
| n | Site Specific Details | ⇨ "Site Specific Master Data" on page B-150 |

> **Multi-language support**
> All language-dependent key data is saved in the table xsprbez. For the dialog in question, e.g. Market Partner > Titles, a view is built at runtime that contains the data for the titles. This view can also be accessed from the database level. That's why we have provided the information about the view on the dialogs that are affected by this. In some cases, there is also language-independent data. It is kept via xx*-View.

### Titles-Descriptions

- Master Data > Keys > Market Partner > Titles > Individual Descriptions
- Master Data > Keys > Market Partner > Titles > All Descriptions

Both of these dialogs include the title forms that can occur when entering market partners, in the relevant languages.

#### Descriptions of fields

**Number/No**
Key number. To create a new title, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xanrede.anrkz

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the title, e.g. Company.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xanrede.anrkz

### Bonus

- Master Data > Keys > Market Partner > Bonus > Bonus
- Master Data > Keys > Market Partner > Bonus > Individual Descriptions
- Master Data > Keys > Market Partner > Bonus > All Descriptions

On this dialog, you enter the rules for the bonus. The assignment of a bonus can be done in the market partner master data or during order entry.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Bonus.

#### Descriptions of fields

**Bonus/No**
Selection of a process. By entering a new number, a new process is created.
Technical info: <F9>, DB field: xbonus.bonusnr

**Description**
Textual explanation of the process.
Technical info: alphanumeric field, DB field: xbonus.bonbez

**Tpe**
Selection of the criteria according to which the bonus should be granted.
First field:
- **CU:** The bonus is granted according to the order volume in the currency unit.
- **QU:** The bonus is granted according to the quantity purchased in square meters.
Technical info: <F9>, DB field: xbonus.bonart

Second field:
- **QU/sqm:** Here you control whetehr the bonus is calculated using the currency unit per square meter.
- **Max %:** Here you control whether the bonus is a maximum percentage value.
Technical info: <F9>, DB field: xbonus.bontyp

In the next field, you enter the corresponding calculation value.
Technical info: numeric field, DB field: xbonus.satz

**Accounting period**
Here, the maximum amount of the granted bonus is kept as information, e.g. 3 means every 3 months.
Technical info: numeric field, DB field: xbonus.zeitraum

**in Month**
Here you specify when exactly the check should be done. Enter a y in the desired month. In the fields that are marked with an n, there is no calculation.
Technical info: toggle field, DB field: xbonus.zp1-12

**Bonus**
After the general area comes the bonus scale. The Bonus column indicates the assignment to the bonus key. There are several lines available for the scaling, in which it is described starting with which sales or which purchase quantity % rate is granted.

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

### Groups

Master Data > Keys > Market Partner > Groups > Groups

This dialog displays the market partner group in the client language. The groups can be divided into classes for informational purposes. However, the class has no effect.

Deleting individual groups is only possible on this dialog.
Technical info: table xxgrp

**Additional information**
⇨ "Group descriptions" on page B-107

### Group descriptions

- Master Data > Keys > Market Partner > Groups > Individual Descriptions
- Master Data > Keys > Market Partner > Groups > All Descriptions

Both of these dialogs include the market partner groups that can occur when entering market partners, in the relevant languages.

#### Descriptions of fields

**Group**
Key number. To create a new group, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xgrp.grpnr

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the group, e.g. IG production.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xgrp.atxt

### Industry descriptions

- Master Data > Keys > Market Partner > Industries > Individual Descriptions
- Master Data > Keys > Market Partner > Industries > All Descriptions

This dialog contains the industries that can occur when entering market partners, in the relevant languages. All special conditions can be maintained using these industries.

#### Descriptions of fields

**Number/No**
Key number. To create a new industry, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xbranche.branchenr

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the industry, e.g. IG manufacturer.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xbranche.branche

### Label Texts

Master Data > Keys > Market Partner > Label Texts

On this dialog, you store customer-specific label texts.
The entry in the Product Name field appears as customer-specific additional information on the sheet labels. The long text is referenced with the freely-selectable abbreviation.

#### Descriptions of fields

**Number**
To create a new label text number, select the next free number.
Technical info: numeric field, DB field: xetikett.txtnr

**Product Name**
In this field, you assign the customer or project.
Technical info: alphanumeric field, DB field: xetikett.etitxt1

**Abbrev.**
The long text is referenced with the freely-selectable abbreviation.
Technical info: numeric field, DB field: xetikett.etitxt2

**Text**
This text appears as customer-specific additional information on the sheet labels.
Technical info: alphanumeric field, DB field: xetikett.etitxt3

### Calendar

- Master Data > Keys > Market Partner > Calendar
- System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Calendar

You maintain your operating calendar on this dialog.
If you are working with a multi-site system, this is the main client's calendar. You can maintain different site calendars under
⇨ "Client Calendar" on page B-116

There are two different views available (<F2>):
- Daily view
- Monthly view

#### Descriptions of fields

**Date**
Each individual date is displayed here.

**Day**
Each individual day is displayed here.

**CW**
The calendar week is displayed here.

**H**
Selection of whether this is a business day.
Technical info: toggle field, DB field: alkal.htag

**PD**
Selection of whether this is a production day.
Technical info: toggle field, DB field: alkal.ptag

**T-CL**
Here you can see whether this day is a site-specific business day. The entry here overrides the entry in the Dt field. The site-specific business days are maintained in System > Keys > Market partner > Calendar > Site Calendar and cannot be changed here.

**P CL**
Here you can see whether this day is a site-specific production day. The entry here overrides the entry in the P field. The site-specific business days are maintained in System > Keys > Market partner > Calendar > Site Calendar and cannot be changed here.

**Remark**
You can store an appropriate remark in this field.
Technical info: alphanumeric field, DB field: alkal.bem

> **Working with A+W Production**
> If you are working with A+W Production, the system can be configured so that this calendar is also evaluated in production. This configuration is done in A+W Production.

### Special Calendar

- Master Data > Keys > Market Partner > Calendar > Special Calendar > Special Calendar
- Master Data > Keys > Market Partner > Calendar > Special Calendar > Individual Descriptions
- Master Data > Keys > Market Partner > Calendar > Special Calendar > All Descriptions
- System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Special Calendar
- System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Special Calendar > Individual Descriptions
- System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Special Calendar > All Descriptions

On this calendar, you can store dates for events, for example.

#### Descriptions of fields

**Calendar**
Selection of the calendar number.
Technical info: <F9>, DB field: almpkal.kalnr

**Date**
You specify the date here.
Technical info: numeric field, DB field: almpkal.datum

**Day**
If you leave the Date field, the day is displayed automatically.

**CW**
If you leave the Date field, the calendar week is displayed automatically.

**CTD**
Here you can see whether or not this is a business day.

**H**
In this field, you can define days that are normally not workdays (e.g. Sundays) as business days.
Technical info: toggle field, DB field: almpkal.htag

**Remark**
You can store an appropriate remark in this field.
Technical info: alphanumeric field, DB field: almpkal.bem

**Calendar**
Key number. To create a new calendar, enter the next free number.
Technical info: numeric field, DB field: xsprbez.id
View: xkalender.kalnr

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the calendar, e.g. supplier.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xkalender.atxt

### Customer Calendar

- Master Data > Keys > Market Partner > Calendar > Customer Calendar
- System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Customer Calendar

For market partners of the type Customer and Other, you can store your own data in the customer calendar. That is, market partner-specific business and production days and holidays can be stored.

#### Descriptions of fields

**Partn. Type**
Selection of the partner type.
Technical info: <F9>, DB field: almpkal.kuliflag

**Market partner**
Selection of the market partner number.
Technical info: <F9>, DB field: almpkal.mpnr

**Date**
You specify the date here.
Technical info: numeric field, DB field: almpkal.datum

**Day**
If you leave the Date field, the day is displayed automatically.

**CW**
If you leave the Date field, the calendar week is displayed automatically.

**CTD**
Here you can see whether or not this is a business day.

**H**
In this field, you can define days that are normally not workdays (e.g. Sundays) as business days.
Technical info: toggle field, DB field: almpkal.htag

**Remark**
You can store an appropriate remark in this field.
Technical info: alphanumeric field, DB field: almpkal.bem

### Client Calendar

- Master Data > Keys > Market Partner > Calendar > Client Calendar
- System Menu (<Ctrl> + <F4>) > Information Services >Calendar > Client Calendar

After you have selected the client number, the calendar opens.
This calendar function is used for the multi-site system. Here you can store your own data for each internal site in the operating calendar. This way, you can store client-specific business and production day and holiday data.

There are two different views available:
- Daily view
- Monthly view

#### Descriptions of fields

**Date**
Each individual date is displayed here.

**Day**
Each individual day is displayed here.

**CW**
The calendar week is displayed here.

**H**
Here you can see whether or not this day is a business day for the main client. The main client-specific business days are maintained in System > Keys > Market Partner > Calendar and cannot be changed here.

**PD**
Here you can see whether or not this day is a production day for the main client. The main client-specific production days are maintained in System > Keys > Market Partner > Calendar and cannot be changed here.

**T-CL**
Selection of whether this is a business day.
Technical info: toggle field, DB field: alkal.htag

**PCL**
Selection of whether this is a production day.
Technical info: toggle field, DB field: alkal.ptag

**Remark**
You can store an appropriate remark in this field.
Technical info: alphanumeric field, DB field: alkal.bem

**Additional information**
⇨ "Calendar" on page B-110

### FinAc Clients

Master Data > Keys > Market Partner > FinAc Clients

You specify the FinAc clients on this dialog. For additional information, please contact a service employee of A+W Software GmbH.

### Countries

- Master Data > Keys > Market Partner > Countries > Countries
- Master Data > Keys > Market Partner > Countries > Individual Descriptions
- Master Data > Keys > Market Partner > Countries > All Descriptions

This dialog contains the different countries that can occur when entering market partners, in the relevant languages.

#### Descriptions of fields

**CCd**
Country codes, e.g. A (Austria). To create a new country, enter the appropriate code.
Technical info: <F9>, DB field: xsprbez.cid
View: xland.kfz

**IG**
Country code according to ISO standard, e.g. AT (Austria).
Technical info: alphanumeric field, DB field: xxland.iso

**Country**
Description of the country, e.g. Belgium.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xland.atxt

**FinAc**
This field contains the appropriate country code for financial accounting.
Technical info: alphanumeric field, DB field: xxland.fib

**Intracode**
This field contains the appropriate specification of the Federal Statistical Office for intra-commercial statistics.
Technical info: alphanumeric field, DB field: xxland.fib

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

### Economic Area descriptions

- Master Data > Keys > Market Partner > Economic Areas > Individual Descriptions
- Master Data > Keys > Market Partner > Economic Areas > All Descriptions

The free division of the country into economic areas grants the later assignment of market partners to an economic area, regardless of the federal state.
This dialog contains the different economic areas that can occur when entering market partners, in the relevant languages.

#### Descriptions of fields

**Number/No**
Key number. To create a new economic area, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xwrtraum.wrtnr

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the economic area, e.g. middle.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xwrtraum.wrtraum

### Areas/Counties

- Master Data > Keys > Market Partner > Areas/Counties > Individual Descriptions
- Master Data > Keys > Market Partner > Areas/Counties > All Descriptions

The areas entered here can be assigned to customers and suppliers in the market partner master data. The assignment of the key number should be done for the intra-trade statistics according to the appropriate specification of the Federal Statistical Office.
This dialog contains the different areas and counties, in the relevant languages.

#### Descriptions of fields

**Number/No**
Key number. To create a new region, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xregion.regnr

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Area/County**
Description of the region, e.g. middle.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xregion.region

### General Quality Scale

- Master Data > Keys > Market Partners > Quality Scale > General > Quality Scales
- Master Data > Keys > Market Partners > Quality Scale > General > Individual Descriptions
- Master Data > Keys > Market Partners > Quality Scale > General > All Descriptions

On these dialogs, you create the general quality characteristics with priorities and in different languages. These keys serve to assess the market partner and are used for all assessment criteria.

#### Descriptions of fields

**No**
Key number. To create a new quality, enter the next free number.
Technical info: numeric field, DB field: xxqual.qualkz

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description, e.g. very good quality
Technical info: alphanumeric field, DB field: xsprbez.bez1

**Rank**
The rank that the assessment occupies within the assessment scale.
Technical info: alphanumeric field, DB field: xxqual.rang

### Quality Scale Dates

- Master Data > Keys > Market Partners > Quality scale > Dates > Quality Scale Dates
- Master Data > Keys > Market Partners > Quality Scale > Dates > Individual Descriptions
- Master Data > Keys > Market Partners > Quality Scale > Dates > All Descriptions

To assess the suppliers with regard to adherence to dates, free descriptions are created and scaled with a ranking.
The dialog shows you the keys created, which are available for manual assessment of the suppliers in the market partner master data.

#### Descriptions of fields

**No**
Key number To create a new key number, enter the next free number.
Technical info: numeric field, DB field: xsprbez.id
View: xtermin.terminkz

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Key description, e.g. on-time.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xtermin.atxt

**Rank**
The rank that the assessment occupies within the assessment scale.
Technical info: alphanumeric field, DB field: xxtermin.rang

### Quality Scale Prices

- Master Data > Keys > Market Partners > Quality Scale > Prices > Qual. Scale Prices
- Master Data > Keys > Market Partners > Quality Scale > Prices > Individual Descriptions
- Master Data > Keys > Market Partners > Quality Scale > Prices > All Descriptions

To assess the suppliers with regard to prices, free descriptions can also be created and scaled with a ranking.
The dialog shows you the keys created, which are available for manual assessment of the suppliers in the market partner master data.

#### Descriptions of fields

**No**
Key number To create a new key number, enter the next free number.
Technical info: numeric field, DB field: xsprbez.id
View: xpreis.preiskz

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Key description, e.g. cheap.
Technical info: alphanumeric field, DB field: xxpreis.atxt

**Rank**
The rank that the assessment occupies within the assessment scale.
Technical info: alphanumeric field, DB field: xxpreis.rang
View: xpreis.atxt

### Quality Scale Quantities

- Master Data > Keys > Market Partners > Quality Scale > Quantity > Qual. Scale Qties.
- Master Data > Keys > Market Partners > Quality Scale > Quantity > Individual Descriptions
- Master Data > Keys > Market Partners > Quality Scale > Quantity > All Descriptions

To assess individual suppliers' quantities supplied, free descriptions can also be created and scaled with a ranking.
The dialog shows you the keys created, which are available.

#### Descriptions of fields

**No**
Key number To create a new key number, enter the next free number.
Technical info: numeric field, DB field: xsprbez.id
View: xmenge.mengekz

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Key description, e.g. good stock.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xmenge.atxt

**Rank**
The rank that the assessment occupies within the assessment scale.
Technical info: alphanumeric field, DB field: xxmenge.rang

### Quality Scale Special

- Master Data > Keys > Market Partners > Quality Scale > Special > Qual. Scale Special
- Master Data > Keys > Market Partners > Quality Scale > Special > Individual Descriptions
- Master Data > Keys > Market Partners > Quality Scale > Special > Individual Descriptions

The Special quality scale offers an additional possibility to assess suppliers using freely-definable descriptions to which a rank is assigned.
The dialog shows you the keys created, which are available.

#### Descriptions of fields

**Number**
Key number. To create a new quantity level, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xspec.speckz

**Rank**
The rank that the assessment occupies within the assessment scale.
Technical info: alphanumeric field, DB field: xxspec.rang

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the quantity level, e.g. good stock.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xspec.atxt

### Reasons for Complaint

- Master Data > Keys > Market Partners > Complaint > Reasons > Reasons for Complaint
- Master Data > Keys > Market Partners > Complaint > Reasons > Individual Descriptions
- Master Data > Keys > Market Partners > Complaint > Reasons > All Descriptions

The complaint types are stored as text here and provided with a freely-selectable key. They are needed for recording and assessing complaints.
In addition, the codes of the business type for the intra-trade statistics are maintained in this table.

#### Descriptions of fields

**No**
Key number To create a new key number, enter the next free number.
Technical info: numeric field, DB field: xxrart.reklamart

**Reason for Complaint**
Key description, e.g. defective packaging.
Technical info: alphanumeric field, DB field: xxrart.bez

**Intrastat**
The code according to the specifications of the Federal Statistical Office.
Technical info: alphanumeric field, DB field: xxrart.intrageschart

**No headings**
You can define both columns without headings individually using environment variables.
Technical info: alphanumeric field, DB field: xxrart.private_long1/2

**S**
Closed ID.
Technical info: toggle field, DB field: xxrart.lustill

**Number**
Selection of the key number. To create a new key number, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: rart.reklamart

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Reason for Complaint**
Description of the reason for complaint, e.g. defective packaging.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: rart.atxt

### Places of Complaint

- Master Data > Keys > Market Partners > Complaint > Places > Reason for Complaint
- Master Data > Keys > Market Partners > Complaint > Places > Individual Descriptions
- Master Data > Keys > Market Partners > Complaint > Places > All Descriptions

The text specifications for the complaint place can be defined freely. They are significant for the complaint processing and statistics.

#### Descriptions of fields

**Number**
Key number. To create a new place, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: rort.reklamort

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Reason for Complaint**
Key description, e.g. production.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: rort.atxt

**S**
Closed ID.
Technical info: toggle field, DB field: xxrart.still

### Types of Complaint

- Master Data > Keys > Market Partners > Complaint > Types > Types for Complaint
- Master Data > Keys > Market Partners > Complaint > Types > Individual Descriptions
- Master Data > Keys > Market Partners > Complaint > Types > All Descriptions

The complaint types are stored as text on these dialogs and provided with a freely-selectable key. They are needed for recording and assessing complaints.

#### Descriptions of fields

**Number/No**
Type number. Enter the description in the next field. To create a new key number, enter the next free number.
Technical info: numeric field, DB field: xsprbez.id
View: xxrspec.reklamspec

**Description/Type of Complaint**
Description of the type, e.g. breakage.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xspec.atxt

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**No headings**
You can define both columns without headings individually using environment variables.
Technical info: alphanumeric field, DB field: xxrspec.private_long1/2

**S**
Closed ID.
Technical info: toggle field, DB field: xxrspec.still

### Discount Methods

- Master Data > Keys > Market Partners > Process Discounts > Discount Methods > Discount Methods
- Master Data > Keys > Market Partners > Process Discounts > Discount Methods > Individual Descriptions
- Master Data > Keys > Market Partners > Process Discounts > Discount Methods > All Descriptions

This dialog serves to define valid discount methods that are described with different characteristics and then defined as document and market partner-specific discounts. Information is stored in the discount method that is valid for the entire method.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Discount Methods.

#### Description of the fields

**Method**
Method number. To create a new method, select the next free number.
Technical info: numeric field, DB field: rabattmeth.methode

**Name**
Name of the discount method, e.g. energy surcharge.
Technical info: alphanumeric field, DB field: rabattmeth.methodenname

**Sequen.**
In case of several simultaneous discounts, controls the sequence in which the discounts are applied.
Technical info: numeric field, DB field: rabattmeth.seqnr

**Criterion**
In this field, you specify which document criterion has to be fulfilled so that the discount of this method is effective:
- 0: No dependency
- 1: Rush order
- 2: Route
- 3. Disp.type
- 4: Packing type
- 5: Incoterm
- 6: Destination
Technical info: numeric field, DB field: rabattmeth.qualfier

**Cre.Note**
With this field, you control how the discount is treated for credits:
- **Yes:** The discount is taken over automatically in credits.
- **No:** The discount is not taken over automatically in credits.
- **Query:** You will be asked whether the discount should be taken over into the credit.
Technical info: toggle field, DB field: rabattmeth.gutschrift

**Weight**
With this field you control how the discount is handled for credit notes.
- **Only inv. gls wt:** The discount applies only for the invoiced glass weight.
- **Inv. gls wt:** The discount applies for the invoiced glass weight.
- **Itm wgt:** The discount refers to the item weight.
- **Only itm wgt:** The discount refers only to the item weight.
- **Gls wt:** The discount applies for the glass weight. If this is zero, the item weight is used.
- **Inv. itm wgt:** The discountapplies to the invoiced item weight.
Technical info: toggle field, DB field: rabattmeth.glasgewicht

**Shs**
With this checkbox, you can mark a discount method so that this method deactivates discounts for delivery note generation if there is already a delivery note within this delivery.
Technical info: toggle field, DB field: rabattmeth.lieferzuschlag

**Rab**
With this field, you control whether later discounts apply to the discount of this discount:
- **YesL:** The amount of this discount is considered in the basic amount for subsequent discounts.
- **No:** The amount is not considered.
Technical info: toggle field, DB field: rabattmeth.rabattierbar

**Nul**
With this field, you control whether for quantity calculations items with a zero amount are considered.
- **Yes:** Items with zero amount are considered.
- **No:** Items with zero amount are not considered.
Technical info: toggle field, DB field: rabattmeth.nullpositionen

**Gen**
With this field, you control whether this discount method can be maintained on a general level.
- **Yes:** This method can be maintained on a general level.
- **No:** This method cannot be maintained on a general level.
Technical info: toggle field, DB field: rabattmeth.allgemein

**P.**
With this field, you control whether this discount method can be maintained on a market partner level.
- **Yes:** This method can be maintained on a market partner level.
- **No:** This method cannot be maintained on a market partner level.
Technical info: toggle field, DB field: rabattmeth.marktpartner

**Prj**
With this field, you control whether this discount method can be maintained on a project level.
- **Yes:** This method can be maintained on a project level.
- **No:** This method cannot be maintained on a project level.
Technical info: toggle field, DB field: rabattmeth.objekt

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

### Discounts

Master Data > Keys > Market Partners > Process Discounts > Discount Methods > Discounts

In the discount methods, information is stored that is valid for the entire method. These discounts should not be understood as concrete discount, but rather as a particular grouping of discounts such as energy surcharge or rush surcharge. In the following, no distinction is made between the terms surcharge and discount. The term more comprehensible in the respective context will be used. You define the specific discounts that are generally valid or valid for market partners here:
⇨ “Discounts" on page B-65

The dialog consists of the tabs:
- General
- Details

#### Descriptions of fields

**Method**
Selection of the discount method. The appropriate codes can be assigned via the Discount Methods (Codes > Market Partner > Process Discounts) menu.
Technical info: <F9>, DB field: rabstamm.methode

**Name**
Name of discount method. This entry can be overwritten here.
Technical info: alphanumeric field, DB field: rabstamm.rabatttext

**Criterion**
The criterion stored for the method is displayed here.
Technical info: <F9>, DB field: rabstamm.qualifierwert

**Type**
Type of discount method:
- **Sales:** Sales-related discount.
- **Costs:** Cost-related discount.
- **Purchasing:** Purchasing-related discount (only in the Purchasing menu).
Technical info: toggle field, DB field: rabstamm.ekvkkz

**Prdgrp.**
Product group of the discount method. The discount method only affects the products in this product group in the order.
Technical info: <F9>, DB field: rabstamm.wgrnr

**Value**
The value specified is interpreted differently depending on the discount type and is used for calculation of the discount amount.
Technical info: numeric field, DB field: rabstamm.wert

**Record type (column without header)**
The value specified is interpreted differently depending on the discount type and is used for calculation of the discount amount. Possible values are:
- **+:** Surcharge
- **-:** Discount
Technical info: numeric field, DB field: rabstamm.satzart

**DiscTpe**
Via the discount type, you specify according to what the discount amount should be calculated.
- **GR:** Fixed value
- **%:** Percentage
- **GR/unit:** Value per unit
- **GR/sqm:** Value per sqm of glass
- **GR/kg:** Value per kilogram of glass
- **%SA:** Cost discount based on the sales amount. This discount is calculated like % cost discount with the basis value of the sales order
- **GR/W*D:** Value per weight in kg multiplied by the distance in km. This discount is only applied if the distance was stored in the addresses or the market partner.
Technical info: numeric field, DB field: rabstamm.rabattart

**Itm**
With this checkbox, you control whether or not the discount entered is redistributed across the individual items.
- ✔ The discount is redistributed to the individual items.
- The discount is not redistributed.
Technical info: toggle field, DB field: rabstamm.verteil

### Discounts - Details

Master Data > Keys > Market Partners > Process Discounts > Discounts > Details <F2>

#### Descriptions of fields

**Method**
Selection of the discount method. The appropriate codes can be assigned via the Discount Methods (Codes > Market Partner > Process Discounts) menu.
Technical info: <F9>, DB field: rabstamm.methode

**Name**
Name of discount method. This entry can be overwritten.
Technical info: alphanumeric field, DB field: rabstamm.rabatttext

**Criterion**
The criterion stored for the method is displayed here.
Technical info: <F9>, DB field: rabstamm.qualifierwert

**Type**
Type of discount method:
- **Sales:** Sales-related discount.
- **Costs:** Cost-related discount.
- **Purchasing:** Purchasing-related discount (only in the Purchasing menu).
Technical info: toggle field, DB field: rabstamm.ekvkkz

**Prod. Group**
Product group of the discount method. The discount method only affects the products in this product group in the order.
Technical info: <F9>, DB field: rabstamm.wgrnr

**Discount Value**
The value specified is interpreted differently depending on the discount type and is used for calculation of the discount amount.
Technical info: numeric field, DB field: rabstamm.wert

**Scaling basis**
Selection of the scaling basis. If you specify a scaling basis, you must then apply the scaling levels with <F5>:
- qm - square meters of glass
- kg - kilograms of glass
- km - kilometers
- Pc. - pieces
- GR - value
Technical info: <F9>, DB field: rabstamm.staffelbasis

**Minimum Value**
Minimum discount total.
Technical info: numeric field, DB field: rabstamm.minbetrag

**Maximum Value**
Maximum discount total.
Technical info: numeric field, DB field: rabstamm.maxbetrag

**Redistribute**
Redistribution of the discount to the items. By means of redistribution, the discounts are distributed to the respective item and automatically transmitted to FinAc by the program. If you do not use redistribution, you must manually transmit the discounts to FinAc. For this purpose, you must transmit the information from the Stat. product group and Cost center fields to FinAc.
- The discount is redistributed to the individual items.
- The discount is not redistributed.
Technical info: toggle field, DB field: rabstamm.verteil

**Stat. Product Group**
This field is only active if the current record is not marked as redistributable. Then a statistical product group must be specified for statistics bookings.
Technical info: <F9>, DB field: rabstamm.statwgrnr

**Cost Center**
This field is only active if the current record is not marked as redistributable. Then a cost center must be specified to which the booking should be made.
Technical info: <F9>, DB field: rabstamm.kstelle

**Account**
This field is only active if the current record is not marked as redistributable. Then an account must be specified to which the booking should be made.
Technical info: <F9>, DB field: rabstamm.konto

**Discount valid from**
Date from which the discount should be used.
Technical info: numeric field, DB field: rabstamm.gueltigvon

**Discount valid to**
Date until which the discount should be used. With appropriate system configuration, you can activate the validity check during order entry. The configuration permits the following possibilities:
- There is a check whether discounts expired in the last X days (the number of days can also be configured).
- There is a check whether the discounts expired in the past and a message is also output about whether there are also discounts that expire today.
- It is only reported if discounts are determined that expire today.
Technical info: numeric field, DB field: rabstamm.gueltigbis

**Partial document**
For discounts of the type GR, it must be decided how the program proceeds for the generation of partial delivery notes or partial invoices. The discount is either taken over into the first partial document, taken over in all partial documents or transformed into a percentage discount. Possible values are:
- **in 1. Pd:** Discount is taken over into the first partial document.
- **in all Pd:** Discount is taken over into all partial document.
- **proportion:** There is a transformation into a proportional discount.
Technical info: numeric field, DB field: rabstamm.fixerabatte

**VAT**
Selection of the VAT rate. This field is only active if the current record is not marked as redistributable. The assignment to the value added tax rates only has an effect if the logic is activated for several value added taxes in the system.
Technical info: <F9>, DB field: rabstamm.steuerzu

**Cash D.-able**
The checkbox is only active if discounts are not redistributable. The flag does not affect discounts of the type Costs.
- The discount is cash discountable.
- The discount is not cash discountable.
Technical info: toggle field, DB field: rabstamm.skonto

**openTRANS - Id**
This field allows the assignment of discounts from purchasing orders that were received from OpenTRANS.
Technical info: numeric field, DB field: rabstamm.otrabattid

**Glazing**
The glazing flag is only evaluated for percentage discounts. There, the total of the glazing amounts of the items is used as basic value. On the cost side, glazing discounts always have an amount of 0.
- The discount only applies to glazing.
- The discount applies to everything.
Technical info: toggle field, DB field: rabstamm.verglkz

**Glass Weight**
With this field, you can control to which weight the discount should refer. This information overrides the information from the method master data, so that discounts of a method can now have different reference weights. The glass weight influences the basic value of the discount type GR/kg and the drawing of the scaling level within the processes.
- **Itm wgt:** Item weight.
- **Only glass wt.:** Only glass weight.
- **Glass wt.:** Glass weight
- **Inv. itm wgt.:** Invoiced item weight.
- **Only inv. gls wt:** Only invoiced glass weight.
- **Inv. glass wt.:** Invoiced glass weight.
Technical info: toggle field, DB field: rabstamm.glasgewicht

**Min. Amount for Zero**
With this checkbox, you can decide that the minimum amount is also drawn if the calculated amount is 0.0 GR.
- The discount is redistributed to the individual items.
- The discount is not redistributed to the individual items.
Technical info: toggle field, DB field: rabstamm.minbeinullbetragk

**SP call**
Flag that indicates whether the stored procedure rabattanpassung must be called, which adjusts the discount for each individual process.
- The SP must be called.
- The SP is not called.
Technical info: toggle field, DB field: rabstamm.spaufrufkzkauf

**Item**
Flag that indicates whether the stored procedure rabattzuord should be called, which then decides which process items are considered by this discount and which are not.
- The SP is called.
- The SP is not called.
Technical info: toggle field, DB field: rabstamm.spaufrufkz

**Discount - Id center**
This variable controls the replication of the data from the central office to the corresponding site.
Technical info: toggle field, DB field: rabstamm.rabattidz

**Discount-Id**
Unique assignment to the discount rate.
Technical info: numeric field, DB field: rabstamm.rabattid

### Site Specific Master Data

Master Data > Keys > Market Partners > Site Specific Details

On this dialog, you can store the site-specific details for market partners. The dialog is only active if you are working with the multi-site system.

#### Descriptions of fields

**Partn.type**
Selection of the partner type.
Technical info: toggle field, DB field: mpmdzu.kuliflag

**Market partner**
Selection of the market partner.
Technical info: <F9>, DB field: mpmdzu.mpnr

**Site**
Selection of the site number. The name is displayed in the next field.
Technical info: <F9>, DB field: mpmdzu.hnr

**Sales rep.**
Selection of the relevant sales representative. The respective commission rates for the representative entered here can be booked and they are ready for invoicing. The name is displayed in the next field.
Technical info: <F9>, DB field: mpmdzu.lager

**Debtor conditions**
Selection of the customer number whose conditions should apply for the documents entered.
Technical info: <F9>, DB field: mpmdzu.konddebnr

## System Keys

Master Data > Keys > System

Values for various areas are defined here; these will be available for selection later on.
For example, the licensed language is entered, which is required for report generation in various languages.

You have access to the following areas:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a a/b | Item | ⇨ "Job Titles" on page B-153 |
| b | Zip Codes | ⇨ "Zip Codes" on page B-154 |
| c | Languages | ⇨ "Languages" on page B-156 |
| d a/b | Text additions | ⇨ "Text Additions" on page B-159 |
| e | Document Types | ⇨ "Document Types" on page B-160 |
| f a/b | Quantity units | ⇨ "Quantity Units" on page B-162 |
| ga | Shapes - edge allocation | ⇨ "Edge Allocation" on page B-164 |
| g b/c | Shapes | ⇨ "Shape Descriptions" on page B-166 |
| h | Production area | ⇨"Production Area" on page B-168 |
| ia | Dispatch - packing type | ⇨ "Packing type" on page B-169 |
| ib | Dispatch - rack packing types | ⇨ "Rack Packing Types" on page B-170 |
| ic | Dispatch - dispatch type | ⇨ "Dispatch Type" on page B-171 |
| id | Dispatch - supply types | ⇨ "Incoterms" on page B-173 |
| iea | Dispatch - routes) | ⇨ "Routes" on page B-174 |
| jeb | Dispatch - route plan | ⇨ "Route Plan" on page B-178 |
| i f a/b | Dispatch - dispatch regions | ⇨ "Dispatch Area Descriptions" on page B-179 |
| ig | Dispatch - vehicles | ⇨ "Vehicles" on page B-180 |
| ih | Dispatch - customs exit | ⇨ "Customs Exit" on page B-181 |
| ii | Dispatch - destin. customs | ⇨ "Customs Destination Office" on page B-183 |
| ij | Dispatch - dispatch groups | ⇨ "Dispatch Groups" on page B-184 |
| ja/b | Rack status | ⇨ "Rack Status Descriptions" on page B-185 |
| ka a/b | PMO - rack groups | ⇨ "Rack Groups Descriptions" on page B-186 |
| ka a/b | PMO - packing methods | ⇨ "Packing Methods Descriptions" on page B-187 |
| kc | PMO - rack Packing Allocation | ⇨ "Rack Packing Allocation" on page B-188 |
| l | Currency | ⇨ "Currency" on page B-189 |
| ma | Taxes - tax types | ⇨ "Tax Types" on page B-192 |
| mb | Taxes - tax rates | ⇨ "Tax Rates" on page B-194 |
| n | Payment terms | ⇨ "Payment Type Descriptions" on page B-195 |
| oa | Cash discount groups | ⇨ "Cash Discount Groups" on page B-197 |
| o b/c | Cash discount group names | ⇨ "Cash Discount Groups" on page B-199 |
| p | End of period | ⇨ "End of Period" on page B-200 |
| q a/b | Adhocsql groups | ⇨ "Adhoc SQL Group Descriptions" on page B-201 |
| r | Report texts | ⇨ "Report texts" on page B-202 |
| sa | Companies/Corporations | ⇨ “Companies" on page B-204 |
| sb | Companies/corporations - company assignment | ⇨ "Company Allocation" on page B-205 |

### Job Titles

- Master Data > Keys > System > Job Tittle > Individual Descriptions
- Master Data > Keys > System > Job Tittle > All Descriptions

On this dialog, you define the positions of the employees at the company. They serve later for the master data entry as specification of the employee's position.

#### Descriptions of fields

**Number/No**
Key number. To create a new position, enter the next free number.
Technical info: numeric field, DB field: xsprbez.id
View: xpos.posnr

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Name of the position, e.g. Managing Director.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xpos.atxt

### Zip Codes

Master Data > Keys > System > ZIP Codes

On this dialog, you can store all zip codes that you need later during order entry. The zip codes stored here make entering addresses easier.
In the Select fields area, you can enter search criteria and thus limit the number of hits. Without a search quantity, all zip codes will be displayed. * stands for all entries.
In the lower area you can correct the details or add new entries.

#### Descriptions of fields for selection

**ZIP code**
Selection and entry of the zip code as search value. You can enter the whole zip code or only part of it. * stands for all.
Technical info: <F9>, DB field: xplzk.plz

**City**
Selection and new specification of the city as search value. You can enter the whole city or only part of it. * stands for all.
Technical info: <F9>, DB field: xplzk.ort

**Country**
Entry of the country as search value. You can enter the whole country or only part of it. * stands for all.
Technical info: <F9>, DB field: xplzk.kfz

**Dispatch Region**
Selection of the dispatch region as search value. You can enter the dispatch region or select it with <F9>. Dispatch regions are in the menu element by the same name Master Data > Keys > System > Dispatch. -1 stands for no selection.
Technical info: <F9>, DB field: xplzk.vsregion

#### Descriptions of fields for the hit quantity

**PostCod**
ZIP code. To create a new zip code, insert a new line.
Technical info: numeric field, DB field: xplz.plz

**City**
The city that belongs to the zip code.
Technical info: alphanumeric field, DB field: xplz.ort

**CCd**
The country code that belongs to the zip code.
Technical info: alphabetic field, DB field: xplz.kfz

**Dispatch Region**
Selection of the dispatch region with <F9>. The dispatch region is displayed in the next field. Dispatch regions are in the menu element by the same name Master Data > Keys > System > Dispatch.
Technical info: numeric field, DB field: xplz.vsregion

### Languages

Master Data > Keys > System > Languages

This dialog is used to manage the licensed languages. The languages are defined with a language ID. It serves to print out customer reports in the local language and to be able to assign each market partner its own languages.
The number can be assigned freely. However, in a corporate group with several databases, the number assignment has to be uniform.

The following example should make this clearer:
A corporate group headquartered in France has branches in Germany, England, and Italy. Both the central office and the branches have customers in other countries in Europe.

| Branch | has customer in |
| :--- | :--- |
| Central office: France | France<br>Germany<br>Italy |
| Branch: Germany | Denmark<br>Germany<br>Netherlands |
| Branch: England | England |
| Branch: Italy | Germany<br>Greece<br>Italy<br>Slovenia |

In order to cover the language needs of all branches and their customers, the corporate group has nine language licenses.

> **Inter-country order transfer**
> So that an inter-country order transfer is possible within a corporate group, the ID number of a licensed language has to be the same company-wide. The report language number depends on the design of the report and has to be selected accordingly.

The following table shows how the languages can be created in the central office and the branches:

| A+W Enterprise database | has customers in | Licensed languages | No | Language |
| :--- | :--- | :--- | :--- | :--- |
| Central office: France | France | French | 1 | 1 |
| | Germany | German | 2 | 2 |
| | Italy | Italian | 3 | 3 |
| | Spain | Spanish | 4 | 4 |
| | | Danish | 5 | |
| | | English | 6 | |
| | | Greek | 7 | |
| | | Slovenian | 8 | |
| | | Dutch | 9 | |
| Branch: Germany | Denmark | Danish | 5 | 1 |
| | Germany | German | 2 | 2 |
| | Netherlands | Dutch | 9 | 3 |
| Branch: England | England | English | 6 | 1 |
| Branch: Italy | Germany | German | 2 | 1 |
| | Greece | Greek | 7 | 2 |
| | Italy | Italian | 3 | 3 |
| | Slovenia | Slovenian | 8 | 4 |

#### Descriptions of fields

**No**
Language ID. To create a new language ID, select the next free number.
Technical info: numeric field, DB field: xplz.sprkz

**Language**
Name of the language, e.g. German.
Technical info: alphabetic field, DB field: xsprzu.atxt

**Report Lang.**
Selection of the language in which the report should be output.
Technical info: numeric field, DB field: xsprzu.repsprkz

**AWE Language**
Selection of the language in which the program is displayed. The language ID appears in the next field.
Technical info: numeric field, DB field: xsprzu.alenvsprkz

### Text Additions

- Master Data > Keys > System > Text Additions > Individual Descriptions
- Master Data > Keys > System > Text Additions > All Descriptions

The text additions serve to provide text for articles and products during order entry and the generation of reports. For more information about the precise use of these text additions, see the A+W Enterprise configuration instructions.

#### Descriptions of fields

**Number**
Key number. To create a new text, enter the next free number.
Technical info: <F9>, DB field: xzustxt.txtnr

**Lng**
Language ID.
Technical info: <F9>, DB field: xzustxt.txtnr

**Text constant**
Description of the text, e.g. horizontal.
Technical info: alphanumeric field, DB field: xzustxt.zustxt

### Document Types

Master Data > Keys > System > Document Types

On this dialog, you can store various document types and the type of output. Foe declaration(s) of performance, the document type Declaration of performance has been fixed which is firmly linked with Document type 1.
The Output Type defines whether or not a market partner should receive the selected type via e-mail. The e-mail sending requires additional system-wide settings and configuration.

#### Descriptions of fields

**Tpe**
Key number To create a new key number, select the next free number.
Technical info: numeric field, DB field: xdokutype.dokuart

**Description**
Description of the document type, e.g. declaration of performance.
Technical info: alphabetic field, DB field: xdokutype.dokubez

**Document Type**
Assignment to a document type.
Technical info: alphabetic field, DB field: xdokutype.dokutyp

**Output Type**
Use this field to control the output type. For the declaration of performance, this field is pre-populated with e-mail:
- **none:** The market partner receives no declaration of performance.
- **via e-mail:** The market partner receives the declaration of performance via e-mail.
Technical info: toggle field, DB field: xdokutype.ausgabeart

**CF**
With this field, you control whether the data in the document should be taken over:
- The data should be taken over.
- The data should not be taken over.
Technical info: toggle field, DB field: xdokutype.vorgangflag

**Prod**
With this field, you control whether the data should be transferred to production:
- The data should be taken over.
- The data should not be taken over.
Technical info: toggle field, DB field: xdokutype.prodflag

### Quantity Units

- Master Data > Keys > System > Ouantity Units > Individual Descriptions
- Master Data > Keys > System > Quantity Units > All Descriptions

You define the quantity units on this dialog.

#### Descriptions of fields

**Number/No**
Selection of the key number. To create a new quantity unit, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xme.symb

**Lng**
Selection of the language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Abbr**
Abbreviation of the quantity unit, e.g. mtr.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xme.kurzbez

**Description**
Description of the quantity unit, e.g. meters.
Technical info: alphanumeric field, DB field: xsprbez.bez2
View: xme.atxt

**Dimension**
Dimension of the quantity unit, e.g. linear meters (LM)
Technical info: alphanumeric field, DB field: xsprbez.bez3
View: xme.dim

### Edge Allocation

Master Data > Keys > System > Shapes > Edge Allocation

On this dialog, you specify how the shape edges are interpreted for circumscribing rectangles. For shape 7 (figure above), e.g., the diagonal edge is treated as the height.

#### Descriptions of fields

**Shape**
Selection of the shape number for which the price-relevant edge should be defined. The description is displayed in the next field.
Technical info: <F9>, DB field: modkparam.modnr

**Edge**
For this edge, it should be defined whether it should be entered in the price calculation as height or width.
Technical info: numeric field, DB field: modkparam.kante

**Calculat.**
Defines how the edge goes into the price calculation:
- 0: no calculation
- 1: as height
- 2: as width
- 3: as height + width
- 4: 2x height + width
- 5: height + 2x width
- 6: 2x height + 2x width
Technical info: toggle field, DB field: modkparam.berechnung

**SE**
With this field, you control whether the edge to be processed is a shape edge.
- This edge is a shape edge.
- This edge is not a shape edge.
Technical info: alphanumeric field, DB field: modkparam.modellkante

### Shape Descriptions

- Master Data > Keys > System > Shapes > Individual Descriptions
- Master Data > Keys > System > Shapes > All Descriptions

On this dialog, you store the designations for the shapes to be processed. The texts stored here for the shapes are required both in order entry and for customers papers and the creation of the lite labels.

> **Available shapes**
> Which shapes are available here depends on the Catalog type system setting.

#### Descriptions of fields

**No**
Selection of the shape number. The shape number corresponds to the shapes in the A+W shape catalog or the shape catalog that was set up during installation.
Technical info: <F9>, DB field: modkparam.modnr

**Language**
Selection of the language ID.
Technical info: <F9>, DB field: modelle.sprkz

**Description**
The shape description corresponds to the shapes in the A+W shape catalog or the shape catalog that was set up during installation.
Technical info: alphanumeric field, DB field: modelle.bez

**Print Descript.**
The print description can be changed if necessary.
Technical info: alphanumeric field, DB field: modelle.drubez

**Inp**
With this field, you control whether or not the shape can be entered. It can happen that you are working with the A+W shape catalog, but the shapes are not cut at your company.
- **Y:** The shape number can be entered.
- **N:** The shape number cannot be entered.
Technical info: toggle field, DB field: modelle.erfassbar

**Online**
This field is relevant for online entries. With it, you control whether or not the shape can be entered online.
- **Y:** The shape number can be entered online.
- **N:** The shape number cannot be entered online.
Technical info: toggle field, DB field: modelle.online

**Edges**
Number of edges.
Technical info: numeric field, DB field: modelle.kantanz

### Production Area

Master Data > Keys > System > Production Area

This dialog serves to define individual production areas that can be assigned in order entry.

#### Descriptions of fields

**No**
Number of the production area.
Technical info: numeric field, DB field: xpbbereich.bereich

**Area Description**
Description of the production area, e.g. screen printing.
Technical info: alphanumeric field, DB field: xpbbereich.bez

### Packing type

Master Data > Keys > System > Dispatch > Packing Type

On this dialog, you specify the packing types in the respective languages. This way, they can be output in the local language on customer papers.

#### Descriptions of fields

**No**
The key number can be assigned freely. The same number should be assigned several times if the packing type is created in several languages. In this case, the number remains the same; the Language ID and Description change.
Technical info: numeric field, DB field: xverpack.verpnr

**Description**
Description of the packing type.
Technical info: alphanumeric field, DB field: xverpack.atxt

**mm**
Depending on the configuration, enter the thickness (in mm) of the packing material between two lites here. This entry is optional.
Technical info: numeric field, DB field: xverpack.vdick

**Language**
Selection of the language. The selected language is displayed in the next field.
Technical info: <F9>, DB field: xverpack.sprkz

### Rack Packing Types

Master Data > Keys > System > Dispatch > Rack Packing Types

On this dialog, you can assign different packing types to a dispatch type (e.g. forwarding agency) depending on the destination country. The use of this function can be configured specially. For additional information, please contact a A+W Software GmbH employee.

#### Descriptions of fields

**Disp. Type**
Selection of the dispatch type, e.g. forwarding agency. The name is displayed in the next field. The appropriate codes can be assigned via the Dispatch Type (Master Data > Keys > System > Dispatch) menu.
Technical info: numeric field, DB field: gverpack.versnr

**CCd**
Selection of the country code, e.g. D. The name is displayed in the next field. The appropriate codes can be assigned via the Countries (Master Data > Keys > Market Partner > Countries) menu.
Technical info: alphabetic field, DB field: gverpack.kfz

**Packing type**
Selection of the packing type, e.g. L rack. The name is displayed in the next field. The appropriate codes can be assigned via the Dispatch Type (Master Data > Keys > System > Dispatch) menu.
Technical info: numeric field, DB field: gverpack.verpnr

**Additional information**
⇨ "Countries" on page B-119
⇨ "Packing type" on page B-169
⇨ "Dispatch Type" on page B-171

### Dispatch Type

Master Data > Keys > System > Dispatch > Dispatch Type

On this dialog, you specify the dispatch types in the respective languages. This way, the dispatch type can be output in the local language on customer papers.

#### Descriptions of fields

**No**
The key number can be assigned freely. The same number can be assigned several times if the packing type should be created in several languages. In this case, the number remains the same; the Language ID and Description change.
Technical info: numeric field, DB field: xversand.versnr

**Description**
Description of the packing type in the respective language.
Technical info: alphanumeric field, DB field: xversand.atxt

**Route**
The selection of a route is optional. The route is displayed in the next field.
Technical info: <F9>, DB field: xversand.routenr

**TrMo**
Selection of the code for the transport branch according to the specifications of the Federal Statistitical Office. The description is displayed in the next field.
Technical info: <F9>, DB field: xversand.intraverkehr

**Transp. Surcharge**
The transport surcharge in percent is an estimated value that is required for the correction of the statistical value.
Technical info: numeric field, DB field: xversand.intrasatz

**Language**
Selection of the language. The selected language is displayed in plain text in the next field.
Technical info: <F9>, DB field: xversand.sprkz

### Incoterms

- Master Data > Keys > System > Dispatch > Dispatch Type > Individual Descriptions
- Master Data > Keys > System > Dispatch > Dispatch Type > All Descriptions

This dialog shows you the defined incoterms in the respective languages. This way, they can be output in the local language on customer papers.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Incoterms.

#### Descriptions of fields

**No/Incoterm**
The key number can be assigned freely. The same number can be assigned several times if the packing type should be created in several languages. In this case, the number remains the same; the Language ID and Description change.
Technical info: numeric field, DB field: xlart.lanr

**Description**
Description of the incoterm in the respective language.
Technical info: alphanumeric field, DB field: xlart.labez

**Lng**
Selection of the language (language ID).
Technical info: <F9>, DB field: xsprbez.sprkz

### Routes

- Master Data > Keys > System > Dispatch > Routes > Routes > Route Details I
- Master Data > Keys > System > Dispatch > Routes > Routes > Individual Descriptions
- Master Data > Keys > System > Dispatch > Routes > Routes > All Descriptions

The delivery paths are described in the route management. This way, a delivery route can be assigned and considered during calculation of the delivery date.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Routes.

#### Descriptions of fields

**Route**
Unique route number.
Technical info: numeric field, DB field: route.routenr

**Route description**
The description of the route.
Technical info: alphanumeric field, DB field: route.routename

**Abbrev.**
Abbreviation of the route.
Technical info: alphanumeric field, DB field: route.kurzbez

**Travel days**
Selection of the travel days (Mo-Su).
Technical info: <F9>, DB field: route.routentag

**Depart.**
Departure time for the route.
Technical info: numeric field, DB field: route.abfahrt

**AIRte**
The alternative route refers to another line of the same table in which an alternative to the current route is located. It is used with locking of this route.
Technical info: numeric field, DB field: route.aroutenr

**Reas.**
Selection of the route type:
- **Route:** Route with several delivery points.
- **Direct:** Goods are delivered directly by the pre-supplier.
- **Pick-up:** Goods will be picked up by the customer.
- **Backlog:** Goods are on backlog (planning route).
- **Internal:** Route between two affiliated companies (viaPlant).
Technical info: <F9>, DB field: route.routenkz

**Site**
Selection of the site number to which the route belongs. The field has two meanings:
- In an A+W Enterprise instance where several sites are managed, the Site-no. specifies from which site a route is driven.
- If an order with direct delivery is transferred between two affiliated A+W Enterprise instances, where in the receiving site the route is compared to the own route master. The direct route is selected whose site no. matches the site number of the sending site. In this case, the Siteno. specifies for which site a direct delivery should occur.
Technical info: <F9>, DB field: route.hausnr

**Reg/Site**
Selection of the region to which the route belongs. The appropriate codes can be assigned via the Dispatch Regions (Master Data > Keys > System > Dispatch) menu.
Technical info: <F9>, DB field: route.region

**Prio**
Entry of the priority within a region for via plant.
Technical info: numeric field, DB field: route.prio

**TT**
Entry of the travel time in hours.
Technical info: numeric field, DB field: route.fahrtzeit

**Cal**
With this field, you control whether or not the calendar should be evaluated.
- The calendar is evaluated.
- The calendar is not evaluated.
Technical info: toggle field, DB field: route.mitkalender

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Additional information**
⇨ "Route Details II" on page B-177

### Route Details II

Master Data > Keys > System > Dispatch > Routes > Routes > F2

The fields on this dialog are identical to the fields of the Route Details I dialog, with the exception of the Dispatch Type field.

> **Route Details II**
> By default, the Route Details II tab is hidden. It can be released by an A+W Software GmbH employee.

#### Descriptions of fields

**Dispatch Type**
Selection of the dispatch type. The appropriate codes can be assigned via the Dispatch Type (Master Data > Keys > System > Dispatch) menu. The description of the dispatch type is displayed in plain text in the next field.
Technical info: <F9>, DB field: route.versnr

**Additional information**
⇨ "Routes" on page B-174

### Route Plan

Master Data > Keys > System > Dispatch > Routes > Route Plan

On this dialog, you create the precise departure times for the individual routes. Thus you can define the different departure times for a route that is driven twice a day, for example. You can assign the customer order to the route plan accordingly.

#### Descriptions of fields

**Route**
Selection of the route number. The selected route is displayed in the next field.
Technical info: <F9>, DB field: tourplan.routenr

**Date**
Date on which the tour is driven.
Technical info: alphanumeric field, DB field: tourplan.tourdate

**Depart.**
Departure time for the route.
Technical info: alphanumeric field, DB field: tourplan.tourdate

### Dispatch Area Descriptions

- Master Data > Keys > System > Dispatch > Dispatch Area > Individual Descriptions
- Master Data > Keys > System > Dispatch > Dispatch Area > All Descriptions

On this dialog, you define the individual dispatch regions in the different languages.

#### Descriptions of fields

**Number**
Key number. To create a new dispatch region, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id

**Language**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the dispatch region, e.g. Bavaria.
Technical info: alphanumeric field, DB field: xsprbez.bez1

### Vehicles

Master Data > Keys > System > Dispatch > Vehicles

On this dialog, you store all vehicles that are available for delivery of the goods.

#### Descriptions of fields

**Vehicle**
Key number of the vehicle. To create a new key number, select the next free number.
Technical info: numeric field, DB field: lkw.lkwnr

**Veh. Code**
Official license plate of the vehicle.
Technical info: alphanumeric field, DB field: lkw.kennz

**Vehicle type**
Selection of the vehicle type:
- Truck
- Semitrailer
- Trailer
Technical info: toggle field, DB field: lkw.art

**Description**
This is a free-form name used at the company for the vehicle. It appears in the dispatch control.
Technical info: alphanumeric field, DB field: lkw.bezeichnung

**Tonnage**
The tonnage of the vehicle is entered here. It serves only informational purposes and is not evaluated.
Technical info: numeric field, DB field: lkw.tonnage

### Customs Exit

Master Data > Keys > System > Dispatch > Customs Exit

On this dialog, you store the customs exit offices at the foreign borders. The use of the outgoing/destination customs function requires configuration. For additional information, please contact a service employee of A+W Software GmbH.

#### Descriptions of fields

**No.**
Key number of the customs office. To create a new key number, select the next free number.
Technical info: numeric field, DB field: xazstelle.azsnr

**Customs Exit Office**
Description of the customs exit office according to the customs details.
Technical info: alphabetic field, DB field: xazstelle.bez

**DesCoun**
Selection of the destination country. The description is displayed in the next field.
Technical info: <F9>, DB field: xazstelle.beland

**CustomsType**
Selection of the customs type. The description is displayed in the next field:
- **MCO:** Main customs office
- **GCO:** German customs office
- **CO:** Customs office
- **DispOff:** Dispatch office
Technical info: <F9>, DB field: xazstelle.zaart

**TranspMode**
Selection of the mode of transport. The description is displayed in the next field:
- 1 - Sea transport
- 2 - Railway
- 3 - Highway
- 4 - Air transport
- 5 - Via post
- 7 - permanently installed
- 8 - domestic ship transport
- 9 - own company
- 99 - other
Technical info: <F9>, DB field: xazstelle.vkzweig

### Customs Destination Office

Master Data > Keys > System > Dispatch > Destin. Customs

On this dialog, you store the destinations customs offices at the foreign borders. The use of the destination customs function requires configuration. For additional information, please contact a service employee of A+W Software GmbH.

#### Descriptions of fields

**No.**
Key number of the customs office. To create a new key number, select the next free number.
Technical info: numeric field, DB field: xbzstelle.bzsnr

**CCd**
Selection of the country in which the customs office is located. The description is displayed in the next field
Technical info: <F9>, DB field: xbzstelle.kfz

**Customs Office of Destination**
Customs office of destination according to customs details.
Technical info: alphabetic field, DB field: xazstelle.bez

### Dispatch Groups

Master Data > Keys > System > Dispatch > Dispatch Groups

You can define dispatch groups on this dialog. They are evaluated in the dispatch control and serve the purpose of data selection.

#### Descriptions of fields

**Dispatch Group**
Key number of the dispatch group. To create a new key number, select the next free number.
Technical info: numeric field, DB field: xvsgruppe.vsgruppenr

**Description**
The description of the dispatch group, e.g. IG group.
Technical info: alphanumeric field, DB field: xvsgruppe.bez

**Standard Group**
In this field, you define whether the dispatch group is a standard group. With the start of dispatch control, the appropriate field is populated with this value.
- This group is a standard group.
- This dispatch group is not a standard group.
Technical info: alphabetic field, DB field: xvsgruppe.stdgruppe

### Rack Status Descriptions

- Master Data > Keys > System > Rack Status > Individual Descriptions
- Master Data > Keys > System > Rack Status > All Descriptions

On this dialog, you define the status for racks in various languages. The rack status is required in the rack management.

#### Descriptions of fields

**No**
Key number. To create a new rack status, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id

**Language**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the rack status, e.g. sold.
Technical info: alphanumeric field, DB field: xsprbez.bez1

### Rack Groups Descriptions

- Master Data > Keys > System > PMO > Rack Groups > Individual Descriptions
- Master Data > Keys > System > PMO > Rack Groups > All Descriptions

On this dialog, you define main groups for racks in different languages. That is, you can combine rack types into rack main groups.

#### Descriptions of fields

**No**
Key number. To create a new rack group, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xghgr.ghgrnr

**Language**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Short Name**
The short name of the rack main group, e.g. GG.
Technical info: alphanumeric field, DB field: xsprbez.bez1
View: xghgr.kurzbez

**Description**
The description of the rack main group, e.g. large rack.
Technical info: alphanumeric field, DB field: xsprbez.bez2
View: xghgr.bez

### Packing Methods Descriptions

- Master Data > Keys > System > PMO > Packing Methods > Individual Descriptions
- Master Data > Keys > System > PMO > Packing Methods > All Descriptions

On this dialog, you define the packing methods in different languages.

#### Descriptions of fields

**No**
Key number. To create a new packing method, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id

**Language**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the packing method, e.g. PMO1.
Technical info: alphanumeric field, DB field: xsprbez.bez1

### Rack Packing Allocation

Menu: access right for menu Master Data > Keys > System > PMO > Rack Packing Allocation

Permissible combinations of rack groups and packing methods can be stored on this dialog.

#### Descriptions of fields

**No**
Selection of the rack group. The rack group is displayed in the next field.
Technical info: <F9>, DB field: pmogestverp.pmogestgrpid

**No**
Selection of the packing method. The packing method is displayed in the next field.
Technical info: <F9>, DB field: pmogestverp.pmoverpackid

**Parameters**
In this field, you store the PMO parameters for this key combination. A pair of keys can exist just once.
Technical info: alphanumeric field, DB field: pmogestverp.pmoparameter

### Currency

- Master Data > Keys > System > Currency > Currency
- Master Data > Keys > System > Currency > Individual Descriptions
- Master Data > Keys > System > Currency > All Descriptions

On this dialog, you maintain the currencies and conversion factors in which the prices are displayed. You assign the currency to the market partner in the Master Data > Payment tab.

> **Requirements**
> You can only work with different currencies if the for-fee module for multi-currency capability is configured. For additional information, please contact a service employee of A+W Software GmbH.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Currency.

#### Descriptions of fields

**No**
The currency key is needed for the definition of price lists (PLCD) as well as for customer and supplier entry in order to be able to display and calculate order values in the customer's currency. To create a new currency key, enter the next free number.
Technical info: numeric field, DB field: xwaehr.wnr

**Abbrev.**
Abbreviation of the currency can be assigned freely, e.g. KRW. However, it is recommended that you use the international identifier for the currency.
Technical info: alphanumeric field, DB field: xwaehr.kurzbez

**Description**
Description of the currency can be assigned freely, e.g. Korean Won.
Technical info: alphabetic field, DB field: xwaehr.bezeichn

**Rate**
Rate at which amounts of the local currency are converted to the foreign currency.
Technical info: alphabetic field, DB field: xwaehr.kurs

**Factor**
The rate multiplied by the factor provides the actual rate. The field can be used to exchange information with FinAc.
Technical info: numeric field, DB field: xwaehr.faktor

**Min. CU**
Smallest currency unit, e.g. 0.01 EUR.
Technical info: numeric field, DB field: xwaehr.min_we

**Rounding**
Rounding type:
- **None:** There is no rounding.
- **Comm:** The number will be rounded commercially.
- **Up:** The number will be rounded up.
- **Down:** The number will be rounded down.
Technical info: toggle field, DB field: xwaehr.we_rund

**Euro fact.**
Conversion rate for the EURO.
Technical info: numeric field, DB field: xwaehr.eurokurs

**Disc.**
Currency is discontinued. A discontinued currency can no longer be selected in the market partner. The currency may remain in orders and on invoices, however. If a document is processed again, you will then be asked to change the discontinued currency.
- **Yes:** The currency is discontinued, e.g. Italian Lire.
- **No:** The currency still exists.
Technical info: numeric field, DB field: xwaehr.stillkz

**FIN. Key**
The field can be used to exchange information with FinAc.
Technical info: numeric field, DB field: xwaehr.fibuschl

**VAT acct.**
VAT account. The field can be used to exchange information with FinAc.
Technical info: numeric field, DB field: xwaehr.mwstkto

**Proc. Acc.**
Revenue account. The field can be used to exchange information with FinAc.
Technical info: numeric field, DB field: xwaehr.erloeskto

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

### Tax Types

- Master Data > Keys > System > Taxes > Tax Types > Tax Types
- Master Data > Keys > System > Tax Types > Individual Descriptions
- Master Data > Keys > System > Tax Types > All Descriptions

On this dialog, you store the tax types that are required for the entry of the market partners and document generation.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Tax Types.

#### Descriptions of fields

**Number**
Number of the tax type. To create a new tax key, select the next free number.
Technical info: numeric field, DB field: xkukz.kukz

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the tax type can be assigned freely, e.g. foreign (EC).
Technical info: alphanumeric field, DB field: xkukz.bez

### Tax Rates

Master Data > Keys > System > Taxes > Tax Rates

On this dialog, you assign the appropriate tax rates to the individual tax types.

#### Descriptions of fields

**Number**
Selection of the tax type. The tax type is displayed in the next field.
Technical info: <F9>, DB field: xmwst.kukz

**Tax rate**
Here you store the appropriate tax rate for the tax type in percent. If you need several tax rates, you can use the Tax Rates 1-3 fields.
Technical info: numeric field, DB field: xmwst.satz, satz1-3

**Valid From**
Here you store starting when the tax rate is valid for the tax type.
Technical info: numeric field, DB field: xmwst.giltab

**VAT acct.**
VAT account. The field can be used to exchange information with FinAc.
Technical info: numeric field, DB field: xmwst.mwstkto

**Input Tax Account**
Input tax account. The field can be used to exchange information with FinAc.
Technical info: numeric field, DB field: xmwst.vstkto

### Payment Type Descriptions

- Master Data > Keys > System > Payment Type > Payment Type
- Master Data > Keys > System > Payment Type > Individual Descriptions
- Master Data > Keys > System > Payment Type > All Descriptions

On these dialogs, you store the individual payment types that can be used at your company.

#### Descriptions of fields

**No**
Key number. To create a new payment type, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id
View: xzahlm.zmnr

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the payment type, e.g. prepayment.
Technical info: alphabetic field, DB field: xsprbez.bez1
View: xzahlm.atxt

**FinAc**
Abbreviation for financial accounting.
Technical info: alphabetic field, DB field: xxzahlm.fib

### Cash Discount Groups

Master Data > Keys > System > Cash Discount Groups > Cash Discount Groups

You create the cash discount groups to which you can assign market partners on this dialog. The groups are available in sales and purchasing and can be changed there.

#### Descriptions of fields

**Payment condition**
Display of the key number. To create a new cash discount group, enter the next free number.
Technical info: numeric field, DB field: xxxskonto.zahlbed

**Tpe**
Description of the cash discount type. Any text can be entered here.
Technical info: alphanumeric field, DB field: xxxskonto.art

**Month**
With this field, you control how many (full) months are added to the invoice date or to the due date.
Technical info: numeric field, DB field: xxxskonto.monat

**Deadline 1**
If necessary, an additional deadline can be added. Example: invoice date 02/14, month = 1, deadline = 15 days:
02/14 + 1 month = 03/14
03/14 + 15 days = 03/29
Technical info: numeric field, DB field: xxxskonto.frist1

**Creation date1-3/Deadline 2**
The creation dates (Creation date 1 - Creation date 3) and Deadline 2 enable an extension of the validity period for the cash discount. These fields do not always have to be filled in. The creation date 30 corresponds to the last day of the month.
Example:
Invoice date 02/10, month = 1, deadline = 10 days, creation date 1 = 15, creation date 2 = 30:
02/10 + 1 month = 03/10
03/10 + 10 days = 03/20
The list of possible invoice creation days refers to 03/31 since starting from 03/20, the next possible creation date is determined.
03/31 + 5 days = 04/05
This means that the cash discount must be claimed by 04/04.
Technical info: alphanumeric field, DB field: xxxskonto.rechlegtag1-3, frist2

**Cash Disc. Rate**
Amount of the cash discount granted in percent.
Technical info: numeric field, DB field: xxxskonto.satz

**Description**
Defined payment term in words, e.g. 10 days, 2% cash discount.
Technical info: alphanumeric field

**Next Condition**
The next condition refers to the key for an additional cash discount agreement, which goes into force for the first cash discount agreement after the deadline has passed.
Technical info: <F9>, DB field: xxxskonto.folgezahlbed

### Cash Discount Groups

- Master Data > Keys > System > Cash Discount Groups > Individual Descriptions
- Master Data > Keys > System > Cash Discount Groups > All Descriptions

These dialogs include the cash discount groups in the respective languages.

#### Descriptions of fields

**Number**
Selection of the key number. To create a new group, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id

**Lng**
Selection of the language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the group, e.g. 30 days net.
Technical info: alphanumeric field, DB field: xsprbez.bez1

### End of Period

Master Data > Keys > System > End of Period

The end of period serves in the FinAc as delimitation of the booking period.

#### Descriptions of fields

**End of Period**
Date on which the current booking period ends. Depending on the configuration, the SA period end, PU period end or both can be entered here.
Technical info: numeric field, DB field: periode.ek_periode, vk_periode

**Modified**
Date of the change. The field is filled automatically with today's date.
Technical info: numeric field, DB field: periode.aenderdat

**Frm**
Name of the person who made the change. The field is filled automatically with the name of the person logged in.
Technical info: alphanumeric field, DB field: periode.aendermanr

### Adhoc SQL Group Descriptions

- Master Data > Keys > System > Adhoc SQL Groups > Individual Descriptions
- Master Data > Keys > System > Adhoc SQL Groups > All Descriptions

On these dialogs, you create new Adhocsql groups or make changes. For these groups, you can store your own queries in the system menu <Ctrl> + <F4>.

#### Descriptions of fields

**Number/No**
Key number. To create a new group, enter the next free number.
Technical info: <F9>, DB field: xsprbez.id

**Lng**
Language ID.
Technical info: <F9>, DB field: xsprbez.sprkz

**Description**
Description of the group, e.g. 30 days net.
Technical info: alphanumeric field, DB field: xsprbez.bez1

### Report texts

Master Data > Keys > System > Report Texts

This dialog shows you all defined texts for the reports in the respective languages.

#### Descriptions of fields

**Type**
Selection field for the text type in order to restrict the hit quantity (optional).
Technical info: alphanumeric field, DB field: cr_repstrings.type

**Language**
Selection field for the language in order to restrict the hit quantity (optional).
Technical info: numeric field, DB field: cr_repstrings.sprkz

**Type**
Key description of the text. This is used in the report for reference.
Technical info: numeric field, DB field: cr_repstrings.type

**Language**
Language ID.
Technical info: numeric field, DB field: cr_repstrings.sprkz

**Description**
Name of the language, e.g. English.
Technical info: numeric field, DB field: cr_repstrings.sprkz

**Text**
Name of the report.
Technical info: alphanumeric field, DB field: cr_repstrings.text

**A+W-Flag**
Flag that specifies whether or not the text is specified by A+W.
- The text is specified by A+W.
- The text is not specified by A+W.
Technical info: alphanumeric field, DB field: cr_repstrings.awflag

### Companies

Master Data > Keys > System > Companies/Corporations > Companies/Corporations

This dialog shows you all defined companies and corporations in the respective languages. The dialog is only available if you are using the multi-site function. For additional information, please contact a service employee of A+W Software GmbH.

#### Descriptions of fields

**Company**
Company ID. To create a new company, enter the next free number.
Technical info: numeric field, DB field: xcompany.compid

**Name**
Name of the company.
Technical info: alphanumeric field, DB field: xcompany.name

**Market partner**
Selection of the market partner. Here only the Other market partners are suggested whose mp.private_long1 is.
Technical info: <F9>, DB field: xcompany.mpnr

### Company Allocation

Master Data > Keys > System > Companies/Corporations > Company Allocation

Here you can assign a company to the individual sites (table xhaus). The data is then evaluated in all areas (document entry, SA, production) in order to guarantee the correct site assignment. On this dialog, it is not possible to enter new sites; it is only possible to make an assignment for existing sites. Please note that a site without company assignment counts as non-existent.
The dialog is only available if you are using the multi-site function. For additional information, please contact a service employee of A+W Software GmbH.

> **Changing the assignment**
> Since a change of the assignment can have massive consequences for the document handling in the entire system, there is a security query for each change, asking whether you really want to do this.

#### Descriptions of fields

**No**
Site number. The name is displayed in the next field.
Technical info: display field, DB field: xhaus.name

**Site**
Site number. The name is displayed in the next field.
Technical info: display field, DB field: site2comp.hausnr

**Company**
Selection of the company that should be assigned to the site. The appropriate keys are assigned via the Companies/Corporations menu (Master Data > Keys > System > Companies/Corporations).
Technical info: <F9>, DB field: site2comp.compid

**Customer/Supplier**
Display of the customer and supplier number. These count as internal market partners. Internal market partners must absolutely be maintained in the master data. When opening the dialog for this market partner in the Master Data > Market Partner menu, the title changes to Internal Market Partner. For internal market partners, it is also possible to store a deviating FINAC debtor. However, stricter restrictions apply here: permissible are only internal market partners that belong to the same company/corporate group. If for an internal market partner a deviating FINAC debtor has been entered, then starting from this point, there is also increased checking of the change of the company assignment.
The company assignment of an internal market partner cannot be changed if the market partner is also assigned to other internal market partners as FINAC debtor. In this case, the dependency must first be resolved (that is, the FINAC debtor of the affected other internal market partners changed) before a new company assignment can take place.
Technical info: display field, DB field: xhaus.kunr/linr

**Host**
Host name.
Technical info: display field, DB field: xhaus.xhaus.host

## Product Keys

Master Data > Keys > Products

All permissible colors and dimension variants are stored here. It is also possible to form general exchange rules that change the product structure generally.
For IGUs, the determination of the technical values is controlled via the product keys.

You have access to the following areas:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| aaa | Variants - Colors | ⇨ "Color Variants" on page B-211 |
| a a b/c | Variants - color descriptions | ⇨ "Color Descriptions" on page B-213 |
| aba | Dimensions - dimensions | ⇨ "Dimension variants" on page B-214 |
| a b b/c | Dimensions - dimension descriptions | ⇨ "Variants" on page B-216 |
| aca | Sizes - size variants | ⇨ "Size Variants" on page B-217 |
| a c b/c | Sizes - size descriptions | ⇨ "Size Variants Descriptions" on page B-218 |
| b | Exchange/additional rules | ⇨ "Exchange/Additional Rules" on page B-219 |
| ca | Technical values - groups | ⇨ "Submenu Technical Values > Groups" on page B-209 |
| cb | Technical values - vectors | ⇨ "Submenu Technical Values > Vectors" on page B-209 |
| c | Technical values - notification bodies | ⇨ "Notification Bodies" on page B-245 |
| d | Technical values - product standards | ⇨ "Product Standards" on page B-246 |
| e | Technical values - priorities | ⇨ "Priorities" on page B-248 |
| f | Technical values - product code | ⇨ "Product Information (CEKAL)" on page B-249 |
| g | Technical values - CE code | ⇨ "CE Code (CPIP)" on page B-251 |
| h | Technical value - declaration of performance | ⇨ "Declaration of Performance" on page B-251 |
| i | Technical values - product encryption | "Product Encoding" on page B-253 |
| j | Technical values - product purposes | ⇨ "Product Purposes" on page B-256 |
| k | Technical values - parameter description | ⇨ "Parameter Description" on page B-258 |
| l | Technical values - declaration of performance | ⇨ "Declar. of Perform. (entry)" on page B-259 |
| d a/b | Analysis groups | ⇨ "Descriptions for analysis groups" on page B-260 |
| e a/b/c | Fitting types | ⇨ "Descriptions for fitting types" on page B-261 |
| f a/b | Foil types | ⇨ "Description for Foil Types" on page B-263 |
| g | Production types | ⇨"Production Types" on page B-264 |
| h a/b/c | Spacer types | ⇨ "Description for Spacer Types" on page B-265 |
| i a/b | Sealing types | ⇨ "Descriptions for Sealing Types" on page B-267 |
| j | Motifs | ⇨ "Motif Assignment" on page B-268 |
| k | Stack | This is a customer-specific function that is not a component of this manual. |
| l a/b | Box signature | ⇨ "Descriptions for Box Signature" on page B-270 |
| m | Shaping/Nesting product | ⇨ "Shaping/Nesting Product" on page B-272 |
| n | Template parameters | ⇨ "Template Parameter" on page B-273 |
| o | ITOE exchange rules | ⇨ "¡TOE Exchange Rules" on page B-274 |
| p | Sash size set | This is a customer-specific function that is not a component of this manual. |
| q | Customer products | ⇨ "Customer Products" on page B-277 |
| r | Ordered processings | ⇨ "Ordered Processings" on page B-279 |
| s | Site-specific details | ⇨ "Site-specific details" on page B-281 |
| t | LAMI/CR inheritance | ⇨ "LAMI/CR Inheritance" on page B-282 |
| u | A+W iQuote - specific details | ⇨ "Submenu A+W iQuote-specific details" on page B-210 |

### Submenu Technical Values > Groups

Keys > Products > Technical Values > Groups

With this menu, you create groups that are required for the description of technical values.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Sound protection | ⇨ "dB Groups" on page B-227 |
| b | Thermal properties | ⇨ "U Groups" on page B-228 |
| c | Total energy transmission | ⇨ "g Groups" on page B-229 |
| d | Transmission | ⇨ "Transmission Groups" on page B-230 |
| e | Size restrictions | ⇨ "Size Restriction Groups" on page B-231 |
| f | Thicknesses | ⇨ "Thickness Groups" on page B-232 |
| g | Bending strength) | ⇨ "Bending Strength Groups" on page B-233 |

### Submenu Technical Values > Vectors

Keys > Products > Technical Values > Vectors

With this menu, you create vectors that are required for the description of technical values.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Sound protection | ⇨ "Vectors for Sound Protection (dB)" on page B-234 |
| b | Thermal properties | ⇨ "Vectors for thermal properties (U)" on page B-236 |
| c | Total energy transmission | ⇨ "Vectors for total energz transmission (g)" on page B-238 |
| d | Transmission | ⇨ "Transmission vectors" on page B-240 |
| e | Size restrictions | ⇨ "Dimension restriction vectors" on page B-242 |
| f | Wind load | ⇨ "Wind Load Vectors" on page B-244 |

### Submenu A+W iQuote-specific details

Keys > Products > A+W iQuote-specific details

With this menu, you maintain master data that is required for working with A+W iQuote. If you need information about this product, please contact an A+W Software GmbH employee.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Product groups | ⇨ "Article groups-descriptions" on page B-283 |
| b | Processing assignment | ⇨ "Processing assignment" on page B-284 |
| c | Processing for shape edges | ⇨ "Processings for Shape Edges" on page B-287 |
| d | Exchange groups | ⇨ "Exchange group descriptions" on page B-289 |
| dc | Group allocation (products) | ⇨ "Group Allocation (Article)" on page B-290 |
| dd | Group allocation (spacers) | ⇨ "Group allocation (Spacers)" on page B-291 |

## Partindex

### Index

**A**
- A+W iQuote-specific details
  - Article groups B-283
  - Processing assignment B-284, B-285
- Ad hoc SQL groups
  - Master data B-201
- Addresses
  - Market Partner B-20, B-56
  - Site-specific details B-59
- Analysis groups
  - Enter or change B-260
- Article B-336
  - Article sizes B-346, B-349, B-351, B-353
  - Article texts B-363
  - Article texts Forms B-366
  - Assembly restrictions B-309
  - BOM B-356, B-393
  - BOM restrictions B-357
  - Color variants B-338
  - Compare fittings B-371
  - compulsory sizes B-342, B-344
  - Customer article texts B-364
  - Defaults B-345
  - Identification B-296
  - Load graphics B-380
  - Load images B-380
  - Market partner details B-332
  - Master data B-292
  - Master texts Text editor B-367
  - Modification B-328
  - Note texts B-300
  - Other names B-361
  - Physical properties B-302
  - Price characteristics B-358
  - Prices B-318
  - Private B-329
  - Production B-314
  - Project article texts B-365
  - send to AW-Design B-370
  - Shape sizes B-354
  - Site-specific article details B-382
  - Site-specific color/size details B-390
  - Site-specific supplier details B-387
  - Site-specific variant details B-388
  - Size parameter selection B-341
  - Size restrictions B-307
  - Size variants B-335, B-336, B-338
  - Sizes B-342, B-344, B-346, B-349, B-351, B-353
  - Statistics B-326
  - Stock B-322
  - Suppliers B-330
  - Technical details B-324
  - Variants B-335, B-338
- Article Field Configuration B-411
- Article groups
  - Master data B-283
- Article text
  - Customer article texts B-364
- Article texts B-363
  - Forms B-366
  - Master texts Text editor B-367
  - Project article texts B-365
- Articles
  - Market Partner B-78
- Assembly restrictions B-309
- Authorization groups
  - enter new, change B-92
- AW-Design
  - Send data B-370

**B**
- Bank details
  - Market Partner B-60
- Bending strength groups
  - Enter or change B-233
- BOM B-393
  - Formula editor B-396
- BOMs restrictions B-357
- Bonus
  - Enter or change B-104
  - Market Partner B-77
- Box signature
  - Master data B-270

**C**
- Calendar
  - Customer calendar B-114
  - Operating calendar B-110
  - Site calendar B-116
  - Special calendar B-112
- Cash discount groups
  - Master data B-197, B-199
- CE mark
  - Default values B-251
  - Priorities B-248
- Color variants
  - Enter or change B-211
- Colors
  - Market Partner B-76
- Commission Assignment B-419
- Commission Code B-418
- Companies/corporations
  - Enter or change B-204
- Company assignment
  - Enter or change B-205
- Compare data B-372
- Compare fittings B-371
- Complaint
  - Places B-135
  - Reasons B-133
  - Types B-137
- Configurable Texts B-425
- Contact person
  - Market Partner B-54
- Context menu - F4
  - Market Partner B-16
- Control
  - Control types B-192
- Control types
  - Master data B-192
- Cost Centers B-432
- Cost types B-430
- Cost Units B-431
- Currency
  - Master data B-189
- Current Texts B-421
- Customer article texts B-364
  - Forms B-366
- Customer products
  - Master data B-277

**D**
- Declaration of performance
  - Entry B-259
  - Parameter description B-258
- Declaration of performance (documents)
  - Master data B-251
- Declaration of performance (entry)
  - Master data B-259
- Delete
  - Product sizes B-355
- Departments
  - Enter or change B-99
- Destination customs
  - Master data B-183
- Discounts
  - Market Partner B-65
- Dispatch groups
  - Master data B-184
- Dispatch regions
  - Master data B-179
- Dispatch types
  - Master data B-171
- Document discounts
  - Discount method B-139
  - Discounts B-143
- Document Field Configuration B-413
- Document types
  - Enter or change B-160
  - Market Partner B-84

**E**
- Economic areas
  - Names B-121
- Edge allocation
  - Master data B-164
- EDI configuration
  - Market Partner B-89
- E-mail addresses
  - Market Partner B-61
- Employee
  - Enter new, change B-92
- Site-specific rights overview
- Site-specific details
  - Employee rights overview B-97
- Evaluation
  - Market Partner B-49
- Exchange group descriptions B-289
- Exchange groups
  - Enter or change B-289
- Exchange rules
  - LAMI/CR inheritance B-282
- Exchange/addition rules
  - Test mode B-225
- Exchange/additional rules
  - ITOW - Exchange rules B-274
  - Market Partner B-67

**F**
- FINAC sites
  - Market Partner keys B-118
- Fitting types
  - Master data B-261
- Foil types
  - Enter or change B-263
- Foreign-languages texts
  - Other article names B-361
- Forms
  - Market Partner B-83
- Formula editor B-396

**G**
- Group assignment (article)
  - Enter or change B-290
- Group assignment (spacer)
  - Enter or change B-291
- Group text B-422
- Groups
  - Enter or change B-106
  - Group descriptions B-107
  - Market Partner B-73
- Identification
  - Article B-296
- Industries
  - Industry descriptions B-108
- iQuote-specific details B-289
  - Group assignment (article) B-290
  - Group assignment (spacer) B-291
- Item
  - item descriptions B-153
- ITOE - Exchange rules B-274

**L**
- LAMI/CR inheritance
  - Master data B-282
- Languages
  - Master data B-156

**M**
- Manufacturer code B-276
- Market Partner
  - Address B-20
  - Article assignment B-78
  - Bank details B-60
  - Bonus assignment B-77
  - Color assignmen B-76
  - Contact addresses B-56
  - Contact person B-54
  - Contex menu - F4 B-16
  - Customer-specific information B-38
  - Discounts B-65
  - Document research B-85
  - Document types B-84
  - EDI configuration B-89
  - Evaluation B-49
  - Exchange/additional rules B-67
  - Forms B-83
  - Group assignment B-73
  - Identification B-25
  - Invoice-related information B-36
  - Limit-related information B-46
- Market Partner info B-86
- Market partner texts B-80
- Master Texts B-81
- Modification B-52
- New entry B-14
- Notes B-23
- Order-related information B-30
- Payment-related information B-40
- Print-related information B-43
- Private fields B-53
- Production-related information B-51
- Project assignment B-74
- Project texts B-75
- Rack types B-68
- References B-28
- Replication data B-84, B-87
- Representative assignment B-71
- Search B-17
- Site-specific address details B-59
- Site-specific details B-90
- Supplier-related information B-33
- User assignment B-72
- Market partner
  - Article texts B-82
  - E-mail addresses B-61
- Market partner details
  - Article B-332
- Market Partner Keys
  - Bonus B-104
  - Groups B-106
- Market Partner keys
  - Calendar B-110
  - Countries
  - Countries
  - Country names B-119
  - Customer calendar B-114
  - Date-quality scale B-125
  - Discount methods B-139
  - Discounts B-143
  - FINAC sites B-118
  - General quality scale B-123
  - Group descriptions B-107
  - Industries B-108
  - Label texts B-109
  - Overview B-101
  - Places for complaint B-135
  - Prices-quality scale B-127
  - Quantities-quality scale B-129
  - Reasons for complaint B-133
  - Regions/Federal states B-122
  - Site calendar B-116
  - Site-specific market partner details B-150
  - Special-quality scale B-131
- Types of complaint B-137
- Market partner keys
  - Economic areas B-121
  - Special calendar B-112
- Master DAta
  - Titles B-103
- Master Data
  - Departments B-99
  - Product Groups B-399
- Master data
  - Article B-292
  - Article assembly restrictions B-309
  - Article color variants B-338
  - Article identification B-296
  - Article market partner details B-332
  - Article modification B-328
  - Article note texts B-300
  - Article Physical properties B-302
  - Article Prices B-318
  - Article Private B-329
  - Article production B-314
  - Article size restrictions B-307
  - Article size variants B-335, B-336, B-338
  - Article statistics B-326
  - Article stock B-322
  - Article suppliers B-330
  - Article technical details B-324
  - BOM B-393
  - Overview B-13
  - Product keys B-207
  - Master texts Text editor B-367
- Modification
  - Article B-328
  - Market Partner B-52
- Motifs
  - Master data B-268
- MP Field Configuration B-409

**N**
- Note texts
  - Article B-300
- Notes
  - Market Partner B-23
- Notification authorities
  - Master data B-245

**O**
- Ordered processings
  - Enter or change B-279
- Ordered processings on shape edges
  - Enter or change B-287
- Outbound duties

**P**
- Packaging methods
  - Master data B-187
- Parameter description
  - Master data B-258
- Payment type
  - Master data B-195
- Phrases B-426
- Physical properties
  - Article B-302
- Postal codes
  - Master data B-154
- Price characteristics B-358
- Prices
  - Article B-318
- Priorities
  - Master data B-248
- Private
  - Article B-329
- Private fields
  - Market Partner B-53
- Processing assignment
  - Enter or change B-284, B-285
- Product assignment
  - Ordered processings B-279
- Product code
  - technical data B-373
  - technical details B-376, B-378
- Product encryption
  - Master data B-253
- Product Fixing B-405
- Product group text B-424
- Product Groups
  - Master data B-399
- Product identification (CEKAL)
  - Master data B-249
- Product keys
  - Analysis groups B-260
  - Article groups B-283
  - Bending strength groups B-233
  - Box signature B-270
  - CE mark B-251
  - Color variants B-211
  - Customer products B-277
  - Declaration of performance B-251
  - Declaration of performance (entry) B-259
  - E/A rules-test mode B-225
- Exchange group descriptions B-289
- Fitting types B-261
- Foil types B-263
- Group assignment (article) B-290
- Group assignment (spacer) B-291
- ITOE - Exchange rules B-274
- LAMI/CR inheritance B-282
- Menu overview B-207
- Motif assignment B-268
- Notification authorities B-245
- Parameter description B-258
- Priorities B-248
- Processing assignment B-284, B-285
- Processings on shape edges B-287
- Processings ordered B-279
- Product encryption B-253
- Product identification (CEKAL) B-249
- Product standards B-246
- Product usages B-256
- Production types B-264
- Sash Size Set B-276
- Sealing types B-267
- Size descriptions B-218
- Size restriction groups B-231
- Size restriction vectors B-242
- Size variants B-214, B-216, B-217
- Sound insulation B-227, B-234
- Sound insulation vector B-233
- Spacer types B-265
- Stack B-269
- Template parameters B-273
- Thermal properties B-228, B-236
- Thickness groups B-232
- Total energy transmission B-229, B-238
- Transmission B-240
- Transmission groups B-230
- Wind load B-244
- Product Set B-406
- Product siezs
  - delete B-355
- Product standards
  - Master data B-246
- Product usages
  - Master data B-256
- Production
  - Article B-314
- Production area
  - Master data B-168
- Production types
  - Master data B-264
- Project
  - Market Partner B-74
  - Project article texts B-365

**Q**
- Quality scale
  - Date-quality scale B-125
  - general quality scale B-123
  - Prices B-127
  - Quantities B-129
  - Special B-131
- Quantity units
  - Master data B-162
- Quote-specific details
  - Processings on shape edges B-287

**R**
- Rack groups
  - Enter or change B-186
- Rack packaging assignment
  - Master data B-188
- Rack status
  - Master data B-185
- Rack types
  - Market Partner B-68
- Rack-packaging types
  - Enter or change B-170
- Reference Configuration B-415
- Regions/Federal states
  - Names B-122
- Replication data B-372
  - Market Partner B-84, B-87
- Report texts
  - Master data B-202
- Representative
  - Market Partner B-71
- Research
  - Market partner document research B-85
- Route plan
  - Master data B-178
- Routes
  - Master data B-174
  - Route details B-174
  - Route plan B-178

**S**
- Sash Size Set B-276
  - Classification code B-276
  - Sash Size Set B-276
- Sealing types
  - Master data B-267
- Search
  - Market Partner B-17
- Shape
  - sizes B-354
- Shapes
  - Descriptions B-166
  - Edge allocation B-164
  - Master data B-166
- Site-specific article details
  - Article master data B-382
- Site-specific colors/sizes Details
  - Article master data B-390
- Site-specific details
  - Article B-382
  - Colors/size variants B-390
  - Market Partner B-90, B-150
  - Suppliers B-387
  - Variants B-388
- Site-specific supplier details
  - Article master data B-387
- Site-specific variant details
  - Article master data B-388
- Size descriptions
  - Enter or change B-218
- Size restrictions B-307
- Size variant descriptions
  - Master data B-216
- Size variants
  - Enter or change B-217
  - master data B-214
- Sizes
  - Article B-346, B-349, B-351, B-353
  - compulsory sizes B-342, B-344
  - Defaults B-345
  - shape B-354
  - Size parameter selection B-341
- Software B-11
- Spacer types
  - Master data B-265
- Stack module
  - Master data B-269
- Statistics
  - Article B-326
- Stock
  - Article B-322
- Suppliers
  - Article B-330
- Supply
  - Size variants B-336
  - Supplier B-330
  - Variants B-336
- Supply types
  - Master data B-173
- System keys
  - Ad hoc SQL groups B-201
  - Cash discount groups B-197, B-199
  - Companies/corporations B-204
  - Company assignment B-205
  - Control types B-192
  - Currency B-189
  - Destination customs B-183
  - Dispatch groups B-184
  - Dispatch regions B-179
  - Dispatch types B-171
  - Document types B-160
  - Edge allocation B-164
  - items B-153
  - Languages B-156
  - Outbound duties B-181
  - Overview B-151
  - Packaging methods B-187
  - Payment type B-195
  - Period end B-200
  - PMO packaging methods B-187
  - PMO rack groups B-186
  - PMO rack packaging assignment B-188
  - Postal codes B-154
  - Production area B-168
  - Quantity units B-162
  - Rack groups B-186
  - Rack packaging assignment B-188
  - Rack status B-185
  - Rack-packaging types B-170
  - Report texts B-202
  - Route details B-174
  - Route plan B-178
  - Routes B-174
  - Shapes B-166
  - Supply types B-173
  - Tax rates B-194
  - Tax types B-192
  - Text additions B-159
  - Vehicles B-180
- System menu - F4
  - Calendar B-110
  - Customer calendar B-114
  - Site calendar B-116
  - Special calendar B-112

**T**
- Tax rates
  - Master data B-194
- Taxes
  - Tax rates B-194
- Technical data
  - others B-373
- Technical details
- Article B-324
- others B-376, B-378
- Technical values
  - Bending strength groups B-233
  - CE mark B-251
  - dB groups B-227
  - Declaration of performance (documents) B-251
  - Declaration of performance (entry) B-259
  - g groups B-229
  - Notification authorities B-245
  - Parameter description B-258
  - Priorities B-248
  - Product encryption B-253
  - Product identification (CEKAL) B-249
  - Product standards B-246
  - Product usages B-256
  - Size restriction groups B-231
  - Size restriction vectors B-242
  - Size restrictions B-231
  - Sound insulation B-227, B-233, B-234
  - Thermal properties B-228, B-236
  - Thickness groups B-232
  - Total energy transmission B-229, B-238
  - Transmission B-230, B-240
  - U groups B-228
  - Wind load B-244
- Template parameters
  - Master data B-273
- Text editor B-367
- Text Formulas B-428
- Text management
  - Project texts B-423
- Texts
  - Label texts B-109
  - Market partner article texts B-82
  - Market partner texts B-80
  - Master Texts B-81
  - Report texts B-202
  - Text additions B-159
- Thickness groups
  - Enter or change B-232
- Titles
  - Enter or change B-103

**U**
- User
  - Market Partner B-72

**V**
- Variable Description B-427
- Variants
  - Article B-335, B-338
  - Color variants B-338
  - Colors B-211
  - Size descriptions B-218
  - Size variant descriptions B-216
  - Size variants B-214, B-217, B-335, B-336, B-338
  - Supply B-336
- Variants supply B-336
- Vehicles
  - Enter or change B-180
- Visualize
  - Load article images B-380

