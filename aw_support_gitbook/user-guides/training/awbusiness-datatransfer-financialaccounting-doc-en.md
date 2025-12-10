---
title: "Tutorial: Data Transfer"
category: "training"
product: "AWBusiness"
doc_type: "Documentation"
language: "EN"
tags: ["AWBusiness", "DataTransfer", "FinancialAccounting", "Doc"]
version: "1.0"
last_updated: "2025-12-10"
description: "title: "EN_AWBusiness_Sales_4_4-3" source: "EN_AWBusiness_Sales_4_4-3.pdf" tags: ["A+W Business", "Data Transfer", "Financial Accounting", "FinAcc", "Statistics", "Archiving", "EDI", "Tutorial", "Software Manual", "ERP"] version: "1.0" last_updated: "2025-10-03" short_description: "This document is a tutorial for the A+W Business Sales software, focusing on data transfer processes. It provides step-by-step instructions for transferring financial data like invoices and credit notes to financial a"
source_file: "AWBusiness-DataTransfer-FinancialAccounting-Doc-EN.md"
---


title: "EN_AWBusiness_Sales_4_4-3"
source: "EN_AWBusiness_Sales_4_4-3.pdf"
tags: ["A+W Business", "Data Transfer", "Financial Accounting", "FinAcc", "Statistics", "Archiving", "EDI", "Tutorial", "Software Manual", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial for the A+W Business Sales software, focusing on data transfer processes. It provides step-by-step instructions for transferring financial data like invoices and credit notes to financial accounting (FinAcc) programs, moving documents to statistics for analysis, and archiving old records to maintain system performance. It also covers document import via EDI interfaces."
long_description: "This comprehensive tutorial details the data transfer functionalities within the A+W Business Sales software. It is designed for users who manage financial data and system administration. The guide begins by explaining the process of transferring invoices and credit notes to external financial accounting (FinAcc) systems, covering both automatic and manual transfer methods. It elaborates on critical configuration steps such as status allocation, defining booking periods, and setting up proceeds accounts based on product groups and VAT codes. The document also addresses the management of receivables and the process for transferring invoices to FinAcc with detailed procedural steps and screenshots. A significant portion is dedicated to transferring documents to the statistics module for reporting and analysis, outlining how to configure and execute these transfers. Furthermore, it covers the archiving process, explaining how to move completed documents to an archive database to maintain main database performance. This includes instructions for setting up automatic and manual archiving, defining retention policies, and handling reference checks. The final sections introduce document import functionalities via EDI interfaces, explaining how to map and convert customer data for seamless integration into A+W Business. The tutorial is supplemented with examples, screenshots, and exercises to provide practical guidance."
---

# Tutorial: Data Transfer

## Data Transfer

A+W Business provides interfaces by means of which invoices and credit notes can be transferred to programs for financial accounting (FinAcc).

Data is transferred to FinAcc via number manager. Data transfer can only be started automatically in connection with Syska FinAcc.

**Automatic data transfer**
Data transfer can be automated. There are several options available, e. g. workflow tasks. Which option you can use depends on your system configuration. Should you have any questions regarding this topic, please contact your service contact at A+W Software GmbH.

Transfer of invoices to the FinAcc program is usually triggered manually. The criteria for data transfer are the same for all invoices.

Documents are analyzed and grouped on two levels:

*   The first level compiles all items and BOM components by their PGR combination for statistics.
*   The second level regroups the result another time. The system searches for the corresponding proceeds account. Search keys are the product group, VAT 1, VAT 2 and the document's business type. If there is no such key, a dialog is displayed in which the proceeds account can be entered.

If a key has no entry for the proceeds account, the blank proceeds account will be written in the output file.

Special discounts and surcharges of the product type Services and surcharges belonging to product group 000 will not be transferred but (re)distributed to the corresponding items or BOM components.

---

## Status allocation

In status allocation, you define the minimum status a document must have reached to be transferred to FinAcc.

*Fig. C-210: Example: status for FinAcc transfer*

