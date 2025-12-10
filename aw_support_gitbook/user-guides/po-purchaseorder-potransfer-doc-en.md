---
description: "Create Only One PO When Using PO Transfer for Orders with Different Delivery Dates"
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
