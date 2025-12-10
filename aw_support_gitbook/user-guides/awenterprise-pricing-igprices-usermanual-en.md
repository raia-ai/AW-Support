---
title: "EN-UM-AWEnterprise_8"
source: "EN-UM-AWEnterprise_8.pdf"
tags: ["A+W Enterprise", "software reference", "pricing", "IG prices", "matrix editor", "PCD prices", "surcharges", "muntin prices", "LAMI prices", "technical manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical software reference manual for the A+W Enterprise system, focusing specifically on the configuration and management of prices. It covers various pricing methods, including those for Insulating Glass (IG), PCD, and special articles, detailing how to set up rounding rules, export price matrices, and apply numerous types of surcharges."
long_description: "This comprehensive technical guide provides detailed instructions on managing the 'Prices' module within the A+W Enterprise software. It serves as a reference for users responsible for setting up and maintaining price structures for various glass products. The document is divided into several major sections, each addressing a different aspect of pricing. Key topics include defining rounding specifications (up, down, commercial), exporting price lists and matrices to external formats like Excel, and configuring Insulating Glass (IG) prices. The IG pricing section covers base prices, single lite prices, the matrix editor for complex pricing structures, matrix limits, and various surcharges (e.g., AIR, decorative glass, offset, size). It also explains how to handle exchange lists for different lite types (patterned, special, LAMI, TG). The manual then moves on to 'PCd Prices,' which are applicable to all pricing methods except IG. This includes creating and assigning article vectors, processing vectors for different product groups, and managing matrix assignments for processing. It details the setup of LAMI basic prices, exchange/additional prices, and prices for colored or variant articles. Finally, the guide covers the management of 'Muntin Prices,' explaining how to define price classes, calculation types, and assignments. Throughout the document, navigation paths, field descriptions, technical database information, and practical examples are provided to aid in configuration. It is an essential resource for system administrators and pricing managers to ensure accurate and efficient price calculations within the A+W Enterprise ecosystem."
---

---
## Prices

### – CU:
The price is reduced by the amount entered.
**Technical info:** alphanumeric field, toggle field, numeric field

### Offset 1-20, rounding
Specification how the prices should be rounded after the change. In the first field, enter the type of rounding; in the second, the value in question to which rounding should be done.

*   **Up:** The price is rounded up to the specified decimal place.
*   **Down:** The price is rounded down to the specified decimal place.
*   **Com:** The price is rounded up or down to the specified decimal place.

**Example**

| Rounding | Value | from | to |
| :--- | :--- | :--- | :--- |
| to 50 | 4.38 € | 4.50 € | rounded up |
| | 4.78 € | 5.00 € | |
| from 50 | 4.38 € | 4.00 € | rounded down |
| | 4.78 € | 4.50 € | |
| Com 10 | 4.38 € | 4.40 € | rounded up |
| | 4.78 € | 4.80 € | |
| | 4.34 € | 4.30 € | rounded down |
| | 4.73 € | 4.70 € | |
| Com 100 | 4.38 € | 4.00 € | rounded down |
| | 4.78 € | 5.00 € | rounded up |

**Technical info:** alphanumeric field, toggle field, numeric field

### PU Price
Currently not used.

## Export matrices

**Master data > Prices > Export price lists**

