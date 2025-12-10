---
title: "EN-UM-AWEnterprise_5"
source: "EN-UM-AWEnterprise_5.pdf"
tags: ["A+W Enterprise", "Master Data", "ERP", "Software Reference", "Article Management", "BOM", "Pricing", "Stock Management", "Product Configuration", "Technical Specifications"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference manual for the A+W Enterprise Master Data module. It provides detailed explanations of the fields and settings for managing articles, pricing, stock, Bill of Materials (BOM), and various product configurations. It covers topics such as technical specifications, supplier allocation, and site-specific details, serving as a guide for system administrators and advanced users."
long_description: "This comprehensive software reference guide details the Master Data module within the A+W Enterprise system. It is designed for system administrators and advanced users responsible for setting up and maintaining the core product and operational data. The document provides an in-depth exploration of the 'Article' management section, covering numerous configuration tabs such as Physical Properties, Prices, Stock, Technical Values, and Statistics. It explains how to define article attributes, including alternative types, production documentation, labeling, and inheritance rules for laminated or cast resin products. The pricing section outlines various methods for price calculation, recording, and presentation, including cost calculation, material loss, and tax rates. The stock management chapter describes how to configure default, box, and slot warehouses, and how to set up rules for stock changes and checks. Furthermore, the manual covers the setup of Bill of Materials (BOMs), including BOM restrictions and size inheritance formulas. It also details the configuration of product variants (size, color), compulsory dimensions, supplier allocations, market partner specific data, and other site-specific settings. This guide is essential for leveraging the full capabilities of the A+W Enterprise Master Data module to ensure accurate product definition, pricing, and production planning."
---

# Software Reference

---
## Article

### Alternative type
If you have selected a muntin construction type in the **Muntin Type** field, you can enter a second type here.
If different muntins are to be fit into an IG unit, A+W Enterprise will check at order entry whether the types of the muntins are compatible. If not, A+W Enterprise will check if the defined Alternative type is compatible. If not, A+W Enterprise will issue a message.
**Technical info:** numeric field, `<F9>`, DB field: artikel.sprfor

### Production doc.
In this field, you can select whether or not the print code should be pre-populated in the BOM at document entry when an article is replaced.
- Print code will be pre-populated in the BOM at document entry when the article is replaced.
- Print code will be pre-populated in the BOM at document entry when the article is replaced.

**Technical info:** toggle field, DB field: artikel.pdruckkz

### Spacer text no.
If **Article type IG** has been entered, you can enter the spacer text number.
The text formula is entered on the **Text management > Text creation > Text formula** menu. This formula is analyzed when text is created at order entry, and will be printed on the spacer.
**Technical info:** numeric field, DB field: artikel.rahmtextnr

### Can be label.
In this field you can select if a label can be created for the article.
- Article can be labelled.
- Article cannot be labelled.

**Technical info:** toggle field, DB field: artikel.barcflag

### LAMI/CR inheritance
If the selected Article type is **Processing for LAMI** or **Cast resin**, you can choose LAMI/cast resin inheritance. For production, processing steps have to be defined for the individual lites. To make order entry for cast resin and LAMI units easier, you can set the inheritance code here. This way, the processing can be entered on the top BOM level, and will be automatically inherited to the elements below. Processing will not be inherited to the commercial area or to pricing.
The following options are available for selection:
- **Yes:** The processing will be inherited to the BOM.
- **No:** The processing will not be inherited to the BOM.

**Technical info:** toggle field, DB field: artikel.bearbcopy

### Item text
In this field, you can select if the article appears in the item text at document entry.
- Article will appear as item text.
- Article will not appear as item text.

**Technical info:** toggle field, DB field: artikel.poskompltxt

---
*A+W Enterprise Master Data*
*B-401*

## Prices

**Master Data > Article > Prices tab**

