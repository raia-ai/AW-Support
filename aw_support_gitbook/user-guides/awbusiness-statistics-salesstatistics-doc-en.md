---
title: "EN_AWBusiness_Statistics_4.01"
source: "EN_AWBusiness_Statistics_4.01.pdf"
tags: ["A+W Business", "Statistics", "Software Documentation", "Sales Statistics", "Purchasing Statistics", "Commission Statistics", "Reporting", "Data Analysis", "Glass Industry", "Windows and Doors"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a user manual for the Statistics module of A+W Business, a software solution for the glass, windows, and doors industry. It provides detailed instructions on how to use various statistical evaluation tools for company analysis."
long_description: "This comprehensive guide details the features and functionalities of the A+W Business Statistics module. It is intended for end-users of the software, providing a thorough reference for performing various data evaluations. The document covers several key areas of business analysis, including Sales Statistics, Purchasing Statistics, Commission Statistics, and Intrastat messaging. For each area, it explains how to configure options, set selection criteria and restrictions, and interpret the resulting tables and graphs. Specific topics include evaluating order stock (entered, produced, invoiced, open), analyzing turnover, managing super statistics for multi-site comparisons, tracking complaints, analyzing consumption, and calculating commissions. The manual is structured to guide the user from a general overview to specific, detailed functions, complete with screenshots, field descriptions, and examples. It also includes editorial information, such as a revision history, copyright notices, and contact details for A+W Software GmbH."
---

# A+W Statistics

---
## A+W Business

A+W - Software for Glass, Windows and Doors

---

## Introduction

This section of the documentation contains editorial notes.

### Revision overview

| Section Version / Date | Description |
| :--- | :--- |
| 1.00/03-1998 | Original version |
| 2.00/08-2000 | Reworking of statistics |
| 3.00/12-2003 | Structural conversion to program structure 4.0 |
| 3.01/08-2008 | Correction of typos |
| 3.02/09-2008 | Figure and section numbers adjusted. |
| 3.03/09-2010 | Layout adapted to documentation concept 2010. |
| 3.04/01-2013 | Layout adjusted to A+W Business. |
| 4.00/06-2016 | Complete reworking |
| 4.01/01.2017 | Product and company names adjusted. |

### Editorial

The editorial provides information on the following topics:
- Notes on this document
- Copyrights
- Trademarks
- Contacts

#### Notes on this document

This publication is written exclusively for end users of A+W Business.

The documentation and software described therein are licensed only and must be used or copied only in accordance with the terms of our license agreement. The contents of the documentation are for information purposes only and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH assumes no liability for errors or omissions unless these are based on intentional or grossly negligent behavior.

This document describes the full scope of A+W Business.

#### Copyrights

© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without prior written approval from A+W Software GmbH.

#### Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. Copyrights of third parties must be complied with.

#### Contacts

**A+W Software GmbH**

Am Pfahlgraben 4-10
D-35415 Pohlheim
+49 6404 205 10
+49 6404 205 1877
Zentrale@a-w.com
http://www.a-w.com

---

# Software Reference

## Overview

A+W Business offers various evaluation possibilities. Here, as described below, a distinction is made between current order stock evaluation, sales, complaint, and commission statistics.
- "Sales Statistics" on page F-10
- "Purchasing Statistics" on page F-44
- "Commission Statistics" on page F-54
- "Intrastat Message" on page F-56

> **System settings**
> In the company data, you can specify details for the transfer of the orders and purchase orders into the statistics. For a detailed description, see the Master data section.
> ⇨ Master Data, "Company Data – Archives" on page B-931

## Sales Statistics

The statistics in A+W Business provide an important instrument for company analysis. They include evaluations of your customers, industries, products, business areas, representatives, etc. For these evaluations, you can select whether you want to evaluate the data year by year or month by month.

This chapter provides information on the following subjects:
- "Order Information" on page F-10
- "Selection" on page F-20
- "Turnover Sales" on page F-21
- "Super Statistics" on page F-32
- "Super Statistics – Export" on page F-34
- "Super statistics - Import" on page F-35
- "Complaints Statistics Sales" on page F-36
- "Statistics by Structure" on page F-37
- "Customers by Order Area" on page F-42

### Order Information

**Statistics > Order info**

On this dialog, you evaluate your order stock. Here you can distinguish between the new orders, orders transferred to production, and invoiced orders.

This dialog offers the following tabs:
- "Order Info - Options" on page F-11
- "Order Info - Entered" on page F-15
- "Order Info - Produced" on page F-16
- "Order Info - Invoiced" on page F-17
- "Order Info - Open" on page F-18
- "Order Info - Graph" on page F-19

#### Print menu

**Statistics > Order info**

Use this menu to start the printing of the evaluation on the screen or printer:
- **Default:** Opens the Selection dialog to specify which data should be printed. ⇨ "Selection" on page F-20
- **Sales:** Starts the printing of the sales data and the comparison data from the previous year. The work days are specified by month in the table display. The display closes with the values for the average sales per working day.

### Order Info – Options

**Statistics > Order info > Options tab**

On this tab, you specify the options for selection and output. The result of the search is output on the Entered, Produced, Invoiced, and Open tabs.

