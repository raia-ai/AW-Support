---
title: "EN_AWBusiness_Master_Data_9_6-3"
source: "EN_AWBusiness_Master_Data_9_6-3.pdf"
tags: ["A+W Business", "Master Data", "Software Reference", "ERP", "Glass Manufacturing", "Window Production", "Door Production", "General Settings", "Product Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A software reference guide for the A+W Business 'Master Data' module. It details the configuration of core data used across all other modules, including general settings, product data, pricing, partners, and company information."
long_description: "This document is a comprehensive software reference for the 'Master Data' module within the A+W Business software suite, which is designed for the glass, window, and door manufacturing industries. The guide provides detailed instructions on how to enter and maintain all foundational data that is used comprehensively by all other A+W Business modules. It is structured into several key sections, starting with 'General' settings like languages, calendars, and country codes. It then moves to the 'Products' section, covering the definition of product types, classes, groups (PGR), variants, colors, and other product-related attributes. The document serves as a crucial manual for system administrators and power users responsible for the initial setup and ongoing maintenance of the ERP system's core data, ensuring consistency and accuracy across the entire software platform."
---

# A+W Master Data B
---
## Software Reference
### A+W Business
A+W - Software for Glass, Windows and Doors

## Overview

The **Master Data** module serves to enter and maintain all A+W Business data that is to be used comprehensively by all modules.

Master data are split into the following sections:
- "General"
- "Products"
- "Prices"
- "Stock"
- "Partners"
- "Shipping"
- "Production"
- "Order"
- "Financial Data"
- "Company"
- "Text"
- "Forms"
- "CEKAL"
- "CE Code”
- "B2B"

> **Dialog buttons**
> The standard buttons and menus are described in detail in the Overview section and in the tutorials. We are therefore not going to describe them in connection with the dialogs.

## General
**Master Data > General**

This part of the program serves to enter general data. The General menu offers the following entries:
- "Languages"
- "Months"
- "Days"
- "Country Code"
- "Calendar"
- "Basic Number Ranges"

### Languages
**Master Data > General > Languages**

This dialog serves to enter all the languages in which you correspond with your customers in written form. The main language used for correspondence comes first. It cannot be changed afterwards.

This dialog is only available in connection with the *Multi-lingual* operation module.

**Functions menu**
From this menu you can open the **Define price/quantity unit for multiple languages** dialog in order to copy the names of price and quantity units to a new language.

- **Name**: Name of the language.
- **External key**: External key for communicating with other programs, e.g. for transfer to production or financial accounting.

### Price/Quantity Unit for Multi-Lingual Operation
**Master Data > General > Languages > Functions menu > Copy units**

This dialog is used to copy the names of price and quantity units to a newly defined language provided you are using the *Multi-lingual* operation module. You have to translate these names into the new language afterwards.

**Price/quantity unit**

- **Source language**: The basic language is suggested by default. You can choose any other language in which these price and quantity units exist.
- **Target language**: Target language to which the price and quantity units should be copied.

The names have to be translated afterwards on the appropriate language tab in dialog Price/quantity.
⇨ "Price and Quantity Unit"

### Months
**Master Data > General > Months**

The names of the months are preset by the basic language by default and should not be changed.

- **Name**: Name of the month.
- **External key**: External key for communicating with other programs, e.g. for statistical analysis.

### Days
**Master Data > General > Days**

The names of the weekdays are preset in the basic language by default and should not be changed.

- **Name**: Name of the weekday.
- **External key**: External key for communicating with other programs, e.g. for statistical analysis.

### Country Code
**Master Data > General > Country code**

This dialog serves for managing the international country codes and allocating the default rounding for taxation.

- **Country code**: Country code, e.g. D = Germany, F = France, USA = United States of America. These codes are allocated to your customers and suppliers in dialog Partner management so that the text is shown and printed in the customer's national language, e.g. the quantity units.
⇨ "(Country, state)"

- **Name**: Name of the country, e.g. Germany, France.
- **VAT rounding**: For every country you can define a value to which the VAT should be rounded. 1 for instance means that the value should be rounded up or down to the next value while 5 means that it should be rounded up or down to the next 5.
⇨ Tutorial 2, "Roundings"
⇨ "Rounding (Customer, Supplier)"
⇨ "Rounding"

- **External key**: External key for communicating with other programs, e.g. for statistical analysis.

- **Locked**: Country codes can be locked for entry in partner management and in documents if it is no longer needed.
    - ☐ The country code can be allocated.
    - ☑ The country code is locked and cannot be allocated. If it has been allocated to partners and in documents, it will still be shown however.

- **International code**: Two-digit international country code, e.g. DE = Germany, FR = France, US = United States of America.

### Calendar
**Master Data > General > Calendar**

This dialog is used for managing the holidays and daily working hours in your company. If the entry in field *Hours* is over 0, it is considered to be a working day. To define a day as a holiday, enter 0 in this field.
⇨ Tutorial 1, "Drawing up a General Calendar"

**Working week**

- **Weekday**: Number of regular working hours per weekday. The holidays must be set to 0 (hours).
    - ☐ The weekday is not included in the working week.
    - ☑ The weekday is included in the working week.

**Selection**

- **Year, week**: Choose the year and the calendar week to display the corresponding calendar week in the overview.
- **[Apply to year]**: Applies the changes to all appropriate weekdays of the whole calendar year. Holidays have to be set to 0 afterwards.
- **[Apply to week]**: Applies the changes to all days of the current calendar week. The corresponding weekdays for the rest of the year remain as they are.
- **[Current calendar week]**: You can use this button to display the current calendar week.

**Overview**
The overview shows all calendar weeks for the current calendar year, with the daily working hours. The weekends are shown in red.

### Country Calendar
**Master Data > General > Country Calendar**

On this dialog, you maintain the holidays in the countries and provinces where the companies you're working with are located.

**Identification**
- **Province**: Selection of the province for which the holiday calendar applies. The provinces are stored under Market Partners > General.
⇨ "State"
- **Year**: Selection of the year in which the holidays apply.
- **Country**: Selection of the country to which the province belongs. The countries are stored under Master Data > General.
⇨ "Country Code"

**Table**
The table displays all calendars for the provinces for which the special holidays apply.

### Basic Number Ranges
**Master Data > General > Basic number ranges**

This dialog shows the number of records you can enter in the corresponding master data table, and the number of records already assigned. The start and end numbers are usually fixed and do not have to be adapted.

These numbers can be maintained per database (DB). This means that the number areas of master database and slave databases can differ. These settings will not be replicated.

The number of valid records is limited to the highest number in the listed master data dialogs. You have to raise the highest number if you want to enter more records.

> **Number ranges for documents**
> Number ranges for documents are defined in program section Order.
> ⇨ "Number Ranges"

**Overview**

- **Table**: Names of the master data tables for which number ranges are kept.
- **Last number**: Number of the last assigned record in this number range.
- **Highest number**: Highest number that can be assigned in this number range.

## Products
**Master Data > Products**

This program section serves to define the general data for managing products and well as product master data.

Menu Products offers the following entries:
- "General"
- "Products"

### General
**Master Data > Products > General**

General product data are defined in this section. Menu General offers the following entries:
- "Product Types"
- "Product Classes"
- "PGR"
- "Combined PGR"
- "Top PGR"
- "Variants/Colors"
- "Grill Types"
- "Complaint Cause"
- "Complaint Reasons"
- "Pattern"
- "Pattern Side"
- "Coating Side"
- "Coating Type”
- "Glass Type Groups"
- "Quality Text"
- "Declaration of Performance, Management"
- "Exchange Groups"
- "Exchange Allocations"
- "Classifiers - Product"

### Product Types
**Master Data > Products > General > Product types**

This dialog shows the product types available in A+W Business. These cannot be renamed or completed.
⇨ Tutorial 1, "Product Types and Product Groups"

- **Name**: Name of the product type.
- **Code**: Key number (ID) that clearly identifies the product type in the system.
- **External key**: External key for communicating with other programs, e.g. for transfer to production.
- **Locked**: A product type can be locked for input in product management and in documents if it is no longer needed.
    - ☐ The product type can be allocated.
    - ☑ The product type is locked and cannot be allocated. If it has been allocated to products and in documents, it will still be shown however.

> **Additional product types**
> If you need more product types please contact a member of the A+W Software GmbH service team.

### Product Classes
**Master Data > Products > General > Product Classes**

This dialog serves to manage the product classes you are using in A+W Business. Names of new product groups can be chosen at random. After that, allocate the product type.
⇨ Tutorial 1, "Product Types and Product Groups"

- **Product type**: Product type allocated to a product class.
- **Name**: Name of the product group.
- **Code**: Key by which the product group is clearly identified in the system.
- **External key**: External key for communicating with other programs, e.g. for transfer to production.
- **A+W Production key**: External key used for exchanging data with A+W Production. This key also has to be entered for the corresponding product class in A+W Production.
- **Locked**: A product class can be locked for input in product management and in documents if it is no longer needed.
    - ☐ The product class can be allocated.
    - ☑ The product class is locked and cannot be allocated. If it has been allocated to products and in documents, it will still be shown however.

### PGR
**Master Data > Products > General > PGR**

This dialog serves to manage the product groups you are using in A+W Business. Product groups are classified on three levels:
- Main product group (MPG)
- Super product group (SPG)
- Product group (PGR)

The abbreviation PGR is also used for product groups in general.

MPG 0**, PSG 00* and PGR 000 are fixed.

Product group 000 usually only includes shapes. This way, the shape turnover can be automatically allocated to the turnover of the main product in statistics for example.

Grills and processing steps usually have their own product group.
⇨ Tutorial 1, "Product Groups"

> **Combined product groups**
> If you want to use combined product groups you have to define them like any other product group. The required product groups can be combined and allocated in dialog Combined PGR.
> ⇨ "Combined PGR"

#### Product Group

- **Number**: Number of the product group. Depending on the level you can enter up to three alpha-numerical digits, e.g. 1AT.
- **Lead days**: Lead days for calculating the shipping date. They only apply to purchased articles. The entry defines how many days in advance an article has to be ordered from the supplier to make sure that it is available in due time for production.
- **Name**: Unique name of the product group.
- **External key**: External key for communicating with other programs, e.g. for transfer to production or financial accounting. External keys can be used to calculate prices by product group. In the price definition dialog you can use it for the limit type External PGR key.
⇨ "Prices"

> **Exact quantity limit for the external PGR key**
> The quantity limit 140 Exact External PGR key can be used to define an exact quantity limit for the external PGR key. The corresponding function can be enabled in company data.
> ⇨ "Calculate external PGR key as an inexact quantity limit"

#### Cost and Surcharge Calculation

- **Special surcharge**: Proportional surcharge for a product group. This special surcharge is used for cost price calculation and is identified accordingly.
- **Tax code**: For tax accounting, the data can be transferred to the Avalara Web-Service. For the correct tax accounting, so-called tax codes must be entered for each product group. During the transfer, the tax code for each item is determined using the combi product group of the main product and transferred to Avalara. The access data must be set up in the company data.
⇨ "Company Data > Tax"
- **Bitmap**: Bitmaps that can be allocated to a product group. Serves for quick identification of the product type or class.
- **Top product groups**: Top product groups from dialog Top PGR. You can allocate a product group to a top product group only on product group level (PGR), not on main product group level or product super group level.
    - ☐ The product group has not been allocated.
    - ☑ The product group is allocated to the top PGR.
⇨ Tutorial 1, "Top PGR"
⇨ "Top PGR"

### Combined PGR
**Master Data > Products > General > Combo PGR**

This dialog is used to define combined product groups (combined PGR). If you select a line form the list, the appropriate values appear in the fields and can be edited.
⇨ Tutorial 1, "Rules for PGR Combinations"
⇨ Tutorial 1, "Combine Product Groups"

**Basic product groups**
- **Product group 1, 2**: First and second product group that are combined. All product group levels are valid.

**Combined product groups**
- **Product group**: Combined PGR by the rules of which product group 1 and product group 2 should be combined. Valid combined product groups have to be defined in dialog PGR.
⇨ "PGR"
- **External key**: External key for communicating with other programs, e.g. for statistical analysis.

- **Valid for discount calculation**: You can define whether the combined PGR should be taken into account for discount calculation.
    - ☐ The combined PGR will not be used for pricing.
    - ☑ The combined PGR is considered for price and discount calculation. Checkbox *Create combined discount only on main item level* is checked.

- **Valid for statistics**: You can define whether the combined PGR should be included in statistics.
    - ☐ The combined PGR will not be included in statistics.
    - ☑ The combined PGR is included in statistics. Checkbox *Create combined statistics only for main item* is checked.

- **Create combined discount only on main item level**: This checkbox is only enabled if checkbox *Valid for discount calculation* has been checked.
    - ☐ The total turnover for single annealed and processing will be used for discount calculation.
    - ☑ Only the main item will be used for discount calculation.

| Example combined product group: 100 + 400 = 401 | | |
| :--- | :--- | :--- |
| **Product** | **PGR** | **Combined PGR result** |
| | | ☐ | ☑ |
| Float | 100 | 401 | 401 |
| Processing | 400 | 401 | 400 |

- **Create combined statistics only for main item**: This checkbox is accessible only if the checkbox *Valid for statistics* has been checked.
    - ☐ The total turnover of single annealed and processing will be booked to the product group combination.
    - ☑ This analysis shows how much single annealed has been produced with and without processing.

**Overview**
The overview shows the existing combined product groups.

### Top PGR
**Master Data > Products > General > Top PGR**

This dialog serves to define the top product groups (top PGR). You can analyse these top product groups in turnover statistics.

- **Name**: Name of the top product group. The required product group can be allocated in dialog PGR.
⇨ "PGR"
- **External key**: External key for communicating with other programs, e.g. for statistical analysis.

### Variants/Colors
**Master Data > Products > General > Variants/Colors**

This dialog serves to enter colors that can be used for defining product variants.
⇨ "Product Variants"

- **Language**: In case of multi-lingual operation, please choose the language. Use the same keys for all languages. The name can be translated.
- **Variant**: Internal number of the color. You will need this number for allocating the color to the product variant.
- **Name**: Name of the color.
- **External key**: For Dorma articles, this is the Dorma color code. The external key can be used for communicating with other programs, e.g. for transfer to production.
- **Color selection**: Opens the dialog Color where you can define the color in which e.g. Grills are displayed at item entry. This color is not transferred to production.
- **Preview**: Shows the selected color.
- **Special color**: A special color can be used in the order for certain colors, e.g. for screen printing.
    - ☐ The color will not be used as a special color.
    - ☑ With this setting, the color to be used can be defined in the order.

> **Example**
> For a customer order you want to enter screen printing with a certain pattern, e. g. a formula 1 racecar.
> For such a case, a variant with the code Special color must be defined for the product Screen printing. At item entry, select this product variant for the processing step Screen printing. Another field appears in which you can enter the name of the pattern. This name will be transferred to production.

- **Locked**: A variant can be locked for input in product management and in documents if it is no longer needed.
    - ☐ The variant can be allocated.
    - ☑ The variant is locked and cannot be allocated. If it has been allocated to products and in documents, it will still be shown however.

### Grill Types
**Master Data > Products > General > Grill types**

This dialog is used to define the grill types. Every grill is allocated to a grill type in product management.
⇨ "Pattern"

> **New grill types**
> If you are using A+W Production please agree new grill types with a member of the A+W Software GmbH service team.

- **Type**: Internal number. This number must match the number in the production software.
- **Name**: Name of the grill type.
- **Edge stopper size**: Entry for the edge stopper size in mm. The edger stopper size is analyzed in connection with pricing of the grill pattern.
⇨ Sales, "Grid"
- **Continuity code**: Details of the connection with other grill:
    - **0 - none**: The code has not been set; grill of this type can be processed at random.
    - **1 - horizontal**: Horizontal grills of this type must be continuous.
    - **2 - vertical**: Vertical grills of this type must be continuous.
    - **3 - horizontal + vertical**: Horizontal and vertical grills of this type must be continuous.
    - **6 - overlap**: Horizontal and vertical grills of this type can overlap.
    - **7 - longest bar**: The longest grill of this type must be continuous.
⇨ Tutorial 1, "Grill construction types"
- **Milling depth**: Depth of the incision in the spacer.
- **Special joint**: Some grill types require connecting joints.
    - ☐ This grill type requires no special joint.
    - ☑ This grill type requires a special joint. The width must be entered as well. With this setting, the continuity code and the milling depth have to be set to 0 (none).
- **Width of special joint, 0=width of grill**: Width of the special joint in mm. An entry of 0 shows that the width of the special joint depends on the width of the grill.

### Complaint Cause
**Master Data > Products > General > Complaint Cause**

This dialog is used to enter the cause of the complaint. The entries can be selected when the complaint is entered. They will be analyzed by module Complaint statistics.

- **Name**: Area causing the complaint, e. g. production, order entry, dispatch. This should differ from the reason of complaint.
- **External key**: External key for communicating with other programs, e.g. for the transfer to financial accounting or statistical analysis.
- **Locked**: The cause of complaint can be locked for document input if it is no longer required.
    - ☐ The cause of complaint can be assigned.
    - ☑ The cause of complaint is locked and cannot be assigned. If it has been assigned before in a document, it will still be shown however.

### Complaint Reasons
**Master Data > Products > General > Complaint Reasons**

This dialog is used to enter the reasons that have led to the complaint.

- **Name**: Describes the reason of the complaint, e. g. material fault, production error, breakage.
- **Combined PGR**: Combined PGR for analysis. Combined PGRs can be used to evaluate the quantities produced as a result of complaints. The loss of turnover is analyzed in complaint statistics in module Statistics.
- **External key**: External key for communicating with other programs, e.g. for the transfer to financial accounting or statistical analysis.
- **Locked**: The reason of complaint can be locked for document input if it is no longer required.
    - ☐ The reason of complaint can be assigned.
    - ☑ The reason of complaint is locked and cannot be assigned. If it has been assigned before in a document, it will still be shown however.
