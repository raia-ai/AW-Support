---
title: "EN-CONFIG-AW_Business-7"
source: "EN-CONFIG-AW_Business-7.pdf"
tags: ["A+W Business", "ERP", "Stock Management", "Work Order", "Production Configuration", "OrderXML", "Price Calculation", "Barcode Management", "Surplus Production", "ALCIM"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides configuration details for the A+W Business ERP system, covering automatic stock management, work order creation, completion reporting, surplus handling, and data transfer processes. It serves as a technical guide for system administrators and advanced users."
long_description: "This is a detailed technical manual for the configuration and operation of the A+W Business ERP system. It focuses on advanced modules related to stock management, production orders, and data interchange with other systems like ALCIM. The guide provides step-by-step instructions on how to automatically create work orders based on stock shortfalls, report work order completion, and manage raw material withdrawal. It explains the process of using Bill of Materials (BOM) elements in production, linking master data between ALFAK and ALCIM, and handling surplus production. The document also covers the transfer of production data via the OrderXML format, including fileless transfer methods, and configuring settings for capacity planning, advanced price calculations, and location-spanning barcode management. It includes process flow diagrams, UI screenshots, and specific configuration settings, making it an essential resource for implementing and customizing these functionalities."
---

---
### 4.8.2.2. Automatic creation through a shortfall of the stock on hand

Based on the definition of a minimum stock and a standard order quantity for the stock article, the system can automatically create purchasing suggestions. Dialog Stock P.O. in stock management is used for this purpose. Usually, this dialog serves to create purchase orders of the type Stock P.O. By defining suitable references in the supplier file, work orders can be created automatically however.

On product group or article number level, an internal customer is entered in the supplier file for whom the work order is created automatically.

