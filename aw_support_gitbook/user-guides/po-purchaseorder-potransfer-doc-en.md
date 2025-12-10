---
title: "Create Only One PO When Using PO Transfer for Orders with Different Delivery Dates"
source: "PO_Transfer_to_one_PO.pdf"
tags: ["A+W Business", "Purchase Order", "PO Transfer", "Order Consolidation", "Supplier Management", "ERP", "Software Guide", "PO Settings"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A guide on configuring A+W Business software to consolidate multiple orders, even with different customer delivery dates, into a single Purchase Order (PO) by adjusting PO Transfer settings."
long_description: "This technical document provides a step-by-step guide for users of A+W Business software, specifically for glass, windows, and doors industries. The primary objective is to configure the system to create a single Purchase Order (PO) from multiple sales orders that may have different customer delivery dates. The process involves modifying the PO Transfer settings. Key steps include disabling the 'Order related transfer' option, which normally creates one PO per order. Additionally, it requires setting up a 'User-defined' sorting sequence under the 'Extended' settings, prioritizing sorting by Supplier, Supplier Delivery Date, and then Order Number. The guide emphasizes that for consolidation to work, the selected orders must share the same supplier and the same supplier delivery date. The document uses annotated screenshots to clearly illustrate each step in the A+W Business user interface, from initial settings to verifying the final consolidated PO."
---

# Create Only One PO When Using PO Transfer for Orders with Different Delivery Dates

---
### Changelog
| Name | Date | Change |
| :--- | :--- | :--- |
| Henrik J | 03-12-2021 | Created document. |

---

## Settings

To make it possible for A+W Business to create one Purchase Order (PO) for several orders, you first need to configure the following settings.

### 1. Disable Order Related Transfer

Make sure that you have **“Order related transfer”** disabled. When this option is active, one PO is created for each individual order.

*(Image: Screenshot of the A+W Business PO Transfer screen with the "Order related transfer" checkbox highlighted and unchecked.)*

### 2. Configure Extended Sorting

Now, open the settings under the menu **“Extended”**.

*(Image: Screenshot of the PO Transfer screen with the "Extended" menu option highlighted.)*

In the "Further settings" window that opens, go to tab **2. Sorting**.

Here you need to configure the sorting criteria as follows:

1.  Under "Sort by", select the **"User-defined"** radio button.
2.  From the "Available sorting criteria" box on the left, select the following items and move them to the "Selected criteria and sequence" box on the right using the `>` button:
    *   `Supplier`
    *   `Delivery date supplier`
    *   `Order No.`
3.  Ensure the sequence in the right-hand box is exactly as listed above. You can adjust the order using the arrow buttons below the box.

*(Image: Screenshot of the "Further settings" window on the "Sorting" tab, showing the "User-defined" option selected and the correct criteria and sequence in the right-hand box.)*

> **Note:** The user-defined sorting causes several orders to be combined into one purchase order if the supplier delivery date has been selected as a criterion and the option of order-related transfer is not active.

### 3. Verify Order Details

Before creating the PO, make sure the orders or positions that you want to combine into a single PO have the **same supplier** and the **same supplier delivery date**.

*(Image: Screenshot of the Order pool showing two different orders (200770 and 200771) with the same Supplier "7025-Glass & More Stevenage" and the same "Supplier's deliv. date" of 15.12.2021, while their "Delivery to customer" dates are different (17.12.2021 and 16.12.2021).)*

## Execution and Verification

When you execute the transfer, a single PO will be created. As shown below, the two orders (200770 and 200771), which had different delivery dates to the customer, have been consolidated into one PO.

*(Image: Screenshot of the created Purchase Order header. The P.O. field shows a reference to both original orders: "200770/200771". The supplier delivery date is shown as 15.12.2021.)*

### Position Level View

At the position level, you can see the two distinct line items from the two separate orders are now included in this single PO.

*(Image: Screenshot of the PO items list. Item 1 and Item 2, corresponding to the original separate orders, are now listed together under the new, single Purchase Order.)*
