---
title: "EN-CONFIG-AW_Business-9"
source: "EN-CONFIG-AW_Business-9.pdf"
tags: ["A+W Business", "ERP Configuration", "openTrans", "Invoice Export", "Stock Management", "Logistics Optimizer", "FIFO", "LIFO", "Repurchasing", "A+W Production"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides configuration and operational instructions for various modules within the A+W Business software, including openTrans integration, invoice and credit note exports, stock management, repurchasing processes, and logistics integration."
long_description: "This technical manual is a configuration guide for the A+W Business ERP system. It covers a wide range of functionalities, detailing the necessary setup and operational procedures. Key topics include the integration of openTrans for electronic data interchange, with specific instructions for exporting dispatch notifications, invoices, and credit notes in openTrans 2.1 format. The guide explains how to manage overall surcharges and discounts, and configure automatic allocations based on supplier product reference numbers. It provides in-depth instructions for handling repurchases of broken or unusable parts from production, including notification workflows, generating repurchase orders, and messaging to the production system. A significant portion of the document is dedicated to stock management, covering configuration for stockkeeping of glass articles, automatic stock orders, handling goods in boxes with Bills of Materials (BOM), and stock evaluation using FIFO/LIFO methods. It also details the integration with Hegla warehouse systems and the A+W Logistics Optimizer for route optimization. The manual is intended for system administrators and technical users responsible for configuring and maintaining the A+W Business environment, featuring numerous screenshots, flowcharts, and step-by-step instructions."
---

If a document's overall surcharge/discount is distributed to several purchase orders, the proportional amounts have to be maintained. Based on the surcharge basis, the program tries to find and offer sensible suggestions. These can be changed any time.

**Reverse manual item allocation**
This function cancels all manual allocations

Apart from the functions there are two options:

**Suppress automatic allocations**
If this option is active, overall surcharges/discounts will not be allocated automatically even if this would be possible based on the product number. This option can be used if the automatic allocation is incorrect. When this option has been changed, the document in question has to be imported again to make sure that the changes become effective.

**Trusting the supplier's product reference numbers**
You can enter a product reference number in the openTRANS document. This means that the supplier knows one's own product numbers and uses them in documents. Based on this product reference number, overall surcharges/discounts can be allocated automatically if this option is active.

---
### 6.6.2. Dispatch notifications
Now it is possible to create dispatch notifications in openTrans format. The file suffix for dispatch notifications is `*.awotdis`. Imported dispatch notifications can be used as template for booking in receipt of goods.

## 6.7. Export of invoices

### 6.7.1. Preparations
First, run all update scripts that have not been run so far. Now enter the status allocations for status point „830 invoice export" acc. to the customer's situation. In customer master data, enter the external customer number you have got for the recipient of the invoice export (vl)!! Please note that invoices will be exported right after printing; the minimum and lock status has to take this fact into account.

Next, set the EDI type to „Standard (openTRANS-based)“ in reference management, „Customer – invoice export", and set the directories accordingly. This has to be done for all customers to be included in the export.

Now, only the A+W Business Interface service must be installed and started.

When you print invoices, an export record will be saved in a transfer table which is then processed by the A+W Business Interface service, and is saved as an XML file in the defined place. From there, the file has to be transferred to the corresponding customers e.g. by means of VB scripts.

## 6.8. openTrans 2.1 and credit notes
Starting with version 13.04.112 it is possible to export documents in format openTrans 2.1. In dialog B2B > Customer > Document Export set the export type to Standard (based on openTrans 2.1). For one customer only one openTrans version can be used.

**Image: openTRANS Document Export Configuration**
