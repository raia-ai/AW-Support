---
title: "Delivery_flatrate"
source: "Delivery_flatrate.pdf"
tags: ["Delivery Flat Rate", "A+W Business", "ERP", "Surcharges", "Pricing", "Order Management", "Invoicing", "Shipping"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical guide on how to configure and apply a delivery flat rate within the A+W Business ERP system. It covers product definition, pricing, customer setup, and conditional application rules."
long_description: "This document provides a step-by-step tutorial for setting up a delivery flat rate functionality in the A+W Business software. It details the entire process, starting from defining the delivery fee as a service product with specific product types and classes. It then explains how to set the price for this service. The guide covers system-wide configurations, such as assigning the delivery fee as a standard surcharge in the company's basic data. It also outlines customer-specific settings, like enabling the flat rate in the partner management module, and how to create exceptions based on delivery routes. The document illustrates the end-to-end workflow, from order creation to automatic inclusion of the flat rate on the final invoice. Additionally, it specifies important pre-conditions for the calculation, such as matching tour and delivery dates, and addresses advanced scenarios like applying the fee only when the total order value for a delivery date falls below a certain threshold. Finally, it points out a key system setting that determines whether the fee is calculated based on the delivery date or the shipment date."
---

# Delivery flat rate

---
## 1. Define the Product as a Service

First, you have to define the product as a service, including its product type and product class.

In the **A+W Business - [Product]** screen:
- **Number**: 6501
- **Match code**: LIEFERPAUSCHALE
- **Name**: Lieferpauschale / Delivery flatrate
- **Quantity Unit**: Stk
- **Product Type**: Leistungen / Surcharges
- **Product Class**: Sonstige Leistungen / Misc.

The settings should look similar to the following screenshot:

