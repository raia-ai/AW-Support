---
title: "EN_AWBusiness_Inventory_Management_6_1-2"
source: "EN_AWBusiness_Inventory_Management_6_1-2.pdf"
tags: ["Inventory Management", "A+W Business", "Master Data", "Stock Control", "Product Definition", "Purchase Price", "ERP", "Tutorial", "Software Guide"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial from the A+W Business Inventory Management guide, focusing on master data setup. It covers configuring company data, stock control modes, product definitions, stock sizes, and pricing rules, including average purchase price calculations."
long_description: "This document is a detailed tutorial for the A+W Business Inventory Management software, version 6.1. It guides users through the essential setup of Master Data required for effective inventory control. The tutorial is divided into several modules, starting with company-wide settings for reservations and stock previews. It then delves into status allocations for stock additions and dispatches. A significant portion is dedicated to Product Definition, explaining the distinction between products, stock articles, and stock sizes, and how they interact for pricing and consumption. The guide details various procurement types and stock booking methods (size-related, not size-related, combined). It provides step-by-step instructions, complete with screenshots, for configuring product attributes, pricing parameters, and Bill of Materials (BOM) components. The final sections focus on defining stock sizes for differentiated pricing and calculating purchase prices, including the logic for average purchase price (PP) determination. The document is intended for system administrators or key users responsible for setting up and maintaining the inventory management module."
---

# Master Data Tutorial

---
## Exercises

-   Rename all four stock levels.
-   Create four different storage locations from which at least one is intended for raw materials.

**Additional information in the Master Data section**
-   ⇨ Master Data, "Level 1 to 4" on page B-735
-   ⇨ Master Data, "Stock Definition" on page B-736
-   ⇨ Master Data, "Stock Categories" on page B-738

---

## Company Data

### Objectives
-   Getting familiar with settings for reservations (Stock Control mode).
-   Getting to know the settings for determining the purchase price.
-   Define the time period for the stock preview.

### Benefits
-   Reservations have an impact on the stock on hand. The stock on hand can already be updated with the reservation so that reserved quantities are no longer available.
-   The stock preview shows the current stock on hand and the reserved quantities for a time period that you define.
-   The purchase price of stock articles can be updated automatically. Then, either the average PP is calculated or the one that was last entered.

### Please note:
| Term | Description |
| :--- | :--- |
| **Stock control mode** | The Stock Control mode in the company table defines how reservations influence the stock on hand. |
| **Stock code** | The stock code defines whether the stock on hand for an article is evaluated as a surface (sqm) or a quantity (pieces). |
| **Reservation** | To produce an order item, the required quantities are reserved. The quantities are marked in the stock on hand or booked out. |
| **Default settings** | None |

---

## Stock Control Mode and Reservation

When a product with procurement type Stock Withdrawal is entered in an order, the corresponding quantity (plus waste in the case of fixed sizes) of the stock article is marked as reserved. The reservation can optionally either be booked out of the current stock on hand or automatically when the delivery note or invoice is printed.

-   **Reservation without stock update:**
    The quantity is marked as reserved, but is not yet booked out from the stock. Booking out must be carried out manually.
-   **Reservation with stock update:**
    The reserved quantity is booked out from the current stock by printing the delivery note or invoice. The status allocation determines which document triggers the booking process.
-   **Execute stock booking before document printout:**
    Stock articles can be booked out before the document is printed. In the event of a problem with the stock withdrawal booking, the order is not printed.

These settings are shown in the stock quantities display in dialog Stock Info (stock preview) and the automatic purchase order suggestions that can be triggered when minimum quantities are reached.

---

## Check Company Data

This module shows you how to set the parameters to evaluate the stock and for the stock control mode.

### How to check the settings for the stock
1.  Select menu `Master Data > Company > Company Data`.
2.  Switch to the **Parameter** tab and check the settings for the virtual item numbers.

