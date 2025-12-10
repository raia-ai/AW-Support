---
title: "EN-UM-AWBusiness_23"
source: "EN-UM-AWBusiness_23.pdf"
tags: ["A+W Business", "Software Reference", "Invoice Control", "Electronic Invoice", "Production Transfer", "Logistics", "ERP", "Purchasing", "Capacity Planning", "Software Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference and tutorial for the A+W Business software, covering modules for Invoicing, Production, and Logistics. It details procedures for invoice control, electronic invoice processing, transferring orders to production with and without capacity planning, and managing dispatch logistics."
long_description: "This document serves as a comprehensive guide for users of the A+W Business software, combining a detailed software reference with practical tutorials. It is divided into several key sections. The 'Invoice' section covers the management of invoices, including handling multiple currencies, exchange rates, and VAT calculations. It details the process of invoice control through the 'Items' and 'BOM' (Bill of Materials) tabs, and explains how to manage electronic invoices, from document import to item overview. The 'Production' section provides a tutorial on transferring orders from the ERP system to production. It outlines various transfer methods, including manual transfer, automatic transfer via workflow tasks, and transfers with or without capacity planning using either A+W Business Capacity Planning or A+W Production Capacity Planner. The guide includes schematic process flows, instructions for setting up transfer parameters, and steps for canceling transfers. The 'Reports from Production' section explains how to monitor production progress through file-based and file-less reports, detailing the setup of registration points and the A+W Business Interface Service. Finally, the 'Logistics' section covers dispatch management, including route planning, defining routes, changing delivery dates, and printing route lists and delivery notes. The document is intended for users responsible for purchasing, invoice verification, production planning, and shipping logistics."
---

# Software Reference

---
## Invoice

> i
> **Exchange rate** If you are using more than one currency, the exchange rate defined in the master data is shown here. It can be changed. If you are using only Euro as a currency, the entry in this field must be 1.

### Fix exchange rate

You can define a different exchange rate for each purchase order. This will be used automatically for price control calculations. You can only change it if it has not been fixed in the purchase order.

-> Sales, "Rate fixed for invoicing" on page C-1557

### Target Number Manager

These two fields are released only if the option Fill target NM is enabled. Invoices will be moved to the defined Number Manager after invoice control, e.g. in order to release them for payment.

-> "Options menu" on page D-2025

**Employee** Name of the employee allocated to the target Number Manager.

**Number manager** Number Manager to which the invoices shall be moved after the check.

### Purchase orders

The list shows all purchase orders included in the Number Manager. If you have used the purchase order numbers as a filter in the P.O. data section, only the corresponding purchase orders will be displayed.

The VAT and foreign currency amount columns are displayed only if a mode with VAT and/or a foreign currency has been selected.

**Total** These fields show the totals of the listed purchase orders and the total VAT amount.

### Underlying VAT record

This field shows the percentage for VAT calculation defined in the purchase order which belongs to this invoice.

-> Sales, "Tax rate" on page C-1636

## Invoice control – items

> Documents > P.O. > Invoice > Invoice control > Items tab

