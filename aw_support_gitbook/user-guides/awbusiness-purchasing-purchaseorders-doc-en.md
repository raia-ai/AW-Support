---
title: "EN_AWBusiness_Purchasing_3_30_1-3"
source: "EN_AWBusiness_Purchasing_3_30_1-3.pdf"
tags: ["A+W Business", "Purchasing", "Purchase Orders", "Order Management", "Supplier Management", "P.O. Transfer", "Order Pool", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial on managing purchase orders within the A+W Business Purchasing software. It covers creating, changing, and transferring purchase orders, managing suppliers, and using the order pool for processing."
long_description: "This document provides a detailed tutorial for the A+W Business Purchasing module, focusing on the complete lifecycle of purchase orders (P.O.s). It explains how to create P.O. items within a customer order, assign procurement types, and manage bill of materials (BOM) elements. The guide details the process for changing ordered items, including modifications to prices, quantities, and sizes, and explains how to handle locked items. It covers changing the supplier for all P.O. items in an order and the procedure for transferring orders to the P.O. pool. The tutorial elaborates on the P.O. transfer process, its objectives, benefits, and the various checks involved, such as delivery date verification and supplier route consideration. It also describes how to handle collective orders, change P.O.s within the order pool, and perform price comparisons between different suppliers to select the most favorable option. The document is illustrated with screenshots and step-by-step instructions to guide users through the A+W software interface."
---

# Tutorial: Purchase orders

---
## Changes in ordered items
Order items that have already been ordered or blocked from further processing. They can only be changed later in item entry of the order (or P.O.) if the lock is removed manually. Changes may involve, e.g. prices, quantities or sizes. The rate can be changed in spite of the lock.

The changes to purchase orders have to be saved in the reference orders. If you change the size or quantity of an ordered item, you can enter the changes in the original P.O. The P.O. must then be sent to the supplier again, informing him of the changes.

The changed order must then again be transferred to Purchasing by way of the order pool.

## Enter a P.O. item in the order
Elements or entire items can be entered in an item position from which a P.O has to be generated. To this end, the correct procurement type (purchase code) has to be assigned.

### How to enter an item for the P.O. in the order
1.  Enter the order header and go to the **Items** tab.
2.  Enter the product your customer requires.

*Fig. D-22: Purchase item in the order. A: Procurement type for the selected item, B: Order item created*

3.  Check the correct settings of the procurement type (A).
4.  Go to the menu **Start > Save** to save the data.
5.  Enter another item which includes only one BOM element.
6.  Go to the **BOM** tab.
7.  Select the element (A) that is to be ordered.
8.  Choose the procurement type (C) and the supplier (B).
9.  Go to the menu **Start > Save** to save the changes.

You can now enter more items or change the entered items.
If you want to order all P.O. items from the same supplier, select the new supplier in the order header in the **Terms** tab.
⇨ "How to change the supplier for all P.O. items" on page D-54

10. Close item entry.

If no default supplier was specified for the P.O. items, the supplier has to be specified in the **P.O. transfer – Order pool** dialog.
⇨ "How to create a purchase order for a customer order" on page D-66

*Fig. D-23: Procurement type for BOM element. A: BOM element to be ordered, B: Supplier for the element, C: Procurement type*

## Change supplier in order
You can choose a different supplier for the purchase orders in the order header. This supplier will be used for all P.O. items of this order.

> **Change purchase code in the Number Manager**
> If you need to change the purchase code in several orders, you can collect these orders in a new Number Manager. You can use the menu **Functions > Change code** in this Number Manager to change the procurement type and the supplier for all documents in one step.

### How to change the supplier for all P.O. items
1.  Open the order with all purchase items.
2.  Go to the **Terms** tab.

*Fig. D-24: Order header - Terms tab. A: Supplier for all P.O. items*

3.  Choose the desired supplier (A).
4.  Go to the menu **Start > Save** to save the data.
    A question appears: *Set purchase code for all items?*
5.  Select:
    *   **[Yes]**: The entire order is transferred to Purchasing to be ordered from the selected supplier.
    *   **[No]**: Only the P.O. items are transferred to Purchasing.
6.  Close the order.

You can now transfer the P.O.s to Purchasing.
⇨ "How to create a purchase order for a customer order" on page D-66

## Change ordered item
You can change an ordered item in the order afterwards and issue a new purchase order. Do not forget to tell your supplier which purchase order is the new one, and which of the previous purchase orders it replaces.

> **Change ordered item**
> You can change an ordered item as long as no supplier's order confirmation or receipt of goods has been entered, or a lock status has been reached.

### How to change an ordered item
1.  Open the document in which you want to change an ordered item, and go to item entry.
2.  Select the item you want to change.

*Fig. D-25: Procurement type of BOM element. A: Product structure locked, B: Item locked, only price can be changed*

The fields (A) for the ordered items are locked. The respective text is shown in the **Remark** column (B).

3.  Go to the menu **Functions > Group item > Change locked item**.
    The fields will be enabled.
4.  Enter your changes, e.g. the quantity.
5.  Go to the menu **Start > Save** to save the changes.
    The changes are saved. You can enter more changes.
6.  Close item entry.
    The **P.O. transfer – Order pool** dialog appears; you can transfer the purchase orders to Purchasing.
    ⇨ "How to create a purchase order for a customer order" on page D-66

*Fig. D-26: P.O. transfer - Order pool*

7.  Transfer the changed P.O. as described in **Transfer to Purchasing**.
    ⇨ "Transfer document to order pool" on page D-66

> **Inform supplier**
> Do not forget to tell your supplier of the change if you have already forwarded the original P.O. to him.

## P.O. transfer

### Objectives
- Transferring an order with P.O. items to the order pool
- Checking P.O. items in the order pool
- Changing supplier and delivery dates
- Transferring P.O. items to Purchasing

### Benefits
- Order items can be passed directly on to Purchasing. The P.O. items do not have to be checked in the P.O. pool.
- Prices can be compared in the order pool in order to select the most favorable (or fastest) supplier.
- Dates, prices, and suppliers of purchase orders can be checked before the transfer is made.

### Please note:
| Term | Description |
| :--- | :--- |
| **P.O. transfer** | The P.O. transfer creates purchase orders from the order items. The transfer of a purchase order must be triggered manually. Only order items with a purchase code will be transferred from the order pool to Purchasing. |
| **Order pool** | The order pool is filled by hand. It lists all documents from the selected Number Manager. |
| **P.O.s** | Purchase orders from different orders can be combined in a collective P.O. if the supplier and the delivery date are identical for these items. |
| **Supplier** | If several items with purchase codes were entered in an order, a separate purchase code will be issued for every supplier. |
| **Price comparison** | Before transferring the purchase order, you can compare the prices of suppliers who can provide the required product. For this purpose, the supplier file must be kept updated. |
| **Change of date** | If the delivery date at the customer is changed in the order pool, this change will be applied to the reference order as well. |
| **Send P.O.** | Purchase orders created by means of the order pool have to be printed and sent to the supplier via the **Form/label printing** dialog. |

| Term | Description |
| :--- | :--- |
| **Default settings** | **P.O. transfer > Options menu:**<br>- **Order-related transfer:** Purchase orders are transferred by order. Collective P.O.s can be created if this option is disabled.<br>- **P.O. number = order number:** This option is only available if the option Order-related transfer has been enabled. This setting may not be enabled if different suppliers are entered for an order. |
| **Master data:** | - Number areas<br>- Supplier file |
| **Company data:** | - **Production** tab (profit center invoicing)<br>- **Stock/PP/EDI** tab (include spacers in the P.O.) |

## Order pool
Purchase orders are automatically created from customer orders.

*Fig. D-27: P.O. items in the order pool. A: Order number, B: Item number from the order, C: (Standard) supplier, D: Product description, E: Issue P.O., F: Generate inquiry, G: Document number after transfer, H: Show BOM*

The order items are transferred to Purchasing by way of an order pool. Order items without P.O. items will not be processed further. The document status tells the program which items can be transferred to purchasing.

Customer order check in the order pool only applies to products with the procurement type P.O. or P.O. (complete).

*Fig. D-28: Process of the order check in the order pool*

Components with one of the two procurement types are searched for in the customer orders - first at the level of the main component and then at the BOM level. The products are distinguished by simple purchased elements and purchased elements for which all sub-products have to be ordered as well.

If a customer order contains several items to be ordered from different suppliers, a separate P.O. will be created for each supplier.

If a customer order states stock articles in a quantity which exceeds the current stock on hand, these stock articles have to be ordered by means of a (manual) stock P.O.

### Checks
You can activate various checks via the **Options** menu, e.g.:
- **Check delivery date:** The delivery date is checked automatically. The system will inform you if you have changed a delivery date which falls on a day that is not a route day.
- **Consider supplier's route:** If the delivery date for the P.O. is not a route day, a message to that effect will be issued. This requires that supplier's routes have been defined in the master data.
- **Determine lead days based on PGR combinations:** If lead days have been defined for PGR combinations, these shall be used to calculate the delivery date.
  ⇨ Master Data, "Lead days" on page B-560
- **Product names as per the supplier file:** The names of the ordered products are adopted from the supplier file.
- **No saving of costs:** Costs are not written back to the purchase prices of the order.
- **Consider size surcharges:** Size surcharges shall be transferred with the P.O.

### P.O. transfer
You can select the mode prior to transferring the P.O. items.

*Fig. D-29: Order mode*

*Fig. D-30: Change supplier in order pool*

With the option **Direct order**, P.O.s are generated without transferring them to the order pool. In the order pool, the dates and the suppliers can be changed.

### Supplier selection and price comparison
If a date is at risk, you can choose other suppliers. These will be loaded from the supplier file. If prices are also defined by supplier there, prices can be compared so that you can choose the most favorable supplier, irrespective of date problems.

*Fig. D-31: Change supplier in order pool*

### Delivery dates
To be able to calculate delivery dates, the delivery times of all suppliers must be kept in the supplier file. When customer orders are transferred, the delivery date is checked with the customer. The program also shows whether the delivery time defined for this supplier will allow him to supply the goods on time.

The supplier's delivery date in the order pool is determined by means of the shipping date minus the lead days defined for the corresponding product group.

Weekdays and the route will be taken into account. If no lead days were entered, the shipping date is adopted as the delivery date.

Delivery dates requested in the order that cannot be kept for the P.O. due to the delivery days defined in the supplier file are marked by a special color in the order pool.

The supplier and/or delivery date can be changed in the order pool in this case. The changes will be saved in the order.

### Generated purchase orders
Once the transfer is completed, a report shows the number of documents that could not be transferred (processed).

*Fig. D-32: Faulty documents*

These have to be checked, one by one, and corrected if necessary. The following errors are possible:
- No purchase code found.
- Order is still open.
- Status does not allow transfer.

From the order items with a purchase code, purchase orders were created which can be opened and checked in the P.O. document management. These purchase orders can be sent to the supplier in the usual way.

The status of all transferred items is changed. The status is also changed in the reference orders.

### P.O. numbers
Automatically created purchase orders usually get numbers from the corresponding number area. At the transfer you can also decide whether the order number shall be used as the P.O. number as well.

## Collective orders per supplier
Purchase orders from different orders placed with the same supplier are summed up in collective orders. The system will stick to the sequence in which the entries appear in the order pool. The order number must not be used as a P.O. number in this case however.

When you have selected all items to be ordered from the same supplier in the order pool, you can combine them in a collective P.O.

The following requirements must be met for this:
- Identical supplier
- Identical delivery date
- The code for collective orders has to be set in the supplier master data (**Order** tab).

The **Functions > Marking options** menu can be used to define the supplier for which a collective P.O. shall be issued.

*Fig. D-33: Marking options for collective orders*

With the marking options, all corresponding items in the order pool will be selected automatically. To generate the collective order, disable the menu **Options > Group transfer > Order-related transfer**.

## Transfer document to order pool
Orders are collected in a Number Manager for the transfer. The order pool accesses the Number Manager selected by you. A new Number Manager can be created with the P.O. transfer in which successful purchase orders are transferred. The P.O.s can only be generated if the orders are closed prior to transfer.

### How to create a purchase order for a customer order
1.  Go to **Documents > Order > P.O. transfer**.

*Fig. D-34: Transfer orders from the Number Manager. A: Number Manager with orders for transfer, B: Transfer mode, C: Target Number Manager, D: Target number area*

2.  Select the mode(B):
    - **Fill pool:** Use this option to display the orders on the **Order pool** tab where they can be checked before the transfer and amended if necessary.
    - **Direct order:** Use this option to transfer the data immediately to the standard supplier. This option is useful if you do not want to check prices or delivery dates first. You can print the purchase orders afterwards and send them to the supplier in the usual way, e.g. as an email attachment.
    - **Direct inquiry:** Use this option to transfer the data immediately as an inquiry to the standard supplier.

In this example, the orders are first checked in the order pool.
3.  Select the Number Manager (A) that contains the orders with the P.O. items.
4.  Select the target Number Manager (C) to which the generated P.O.s shall be moved.
    You can enter a new name and thus create a new Number Manager. If you select another user, the Number Manager will be allocated to him/her.
5.  Choose a different target number area (D) if required.
6.  To move the orders to the order pool, go to the menu **Start > Execute**.

*Fig. D-35: Order items in the order pool*

The order pool is filled. The P.O. items are shown per order.

7.  Select the items to be transferred to Purchasing.
    Double-click on the corresponding line header.

*Fig. D-36: Transfer marked order items*

Only items marked with an X have been selected.
8.  To start the action, go to the menu **Start > Execute**.
    The activated checks will be executed. Depending on the number of orders, this may take some time. Confirm the corresponding informative messages by selecting [Yes] or [No] to proceed with the checks. When all checks have been completed, the corresponding purchase orders will be created and thus transferred to Purchasing.
    The transferred items are removed from the order pool.
    The order status is raised. The order history shows the P.O. number as a reference.

*Fig. D-37: P.O. numbers after transfer*

When the items have been transferred, the P.O. number for the order is displayed.
You can open and edit the purchase orders in **Documents > P.O.** Print the new purchase order and send it to the supplier.

## Changing a P.O. in the order pool
If difficulties regarding a date are shown for an item, you can select another supplier from the order pool. You can also open the dialog to change the supplier without date difficulties to select a different supplier other than the standard supplier.

### How to change the delivery date and the supplier
1.  Go to **Documents > Order > P.O. transfer**.
2.  Move the orders to the order pool.
    This procedure is described in the previous unit.
    ⇨ "Transfer document to order pool" on page D-66
3.  Select the item for which you want to change the delivery date.
    Double-click on the corresponding line header.

*Fig. D-38: Item for the change of supplier is marked*

Only items marked with an X have been selected.
4.  Go to the menu **Functions > Change supplier/delivery dates**.
5.  Click **[OK]** to accept the change.

The **Change supplier and delivery dates** dialog closes. The purchase order pool shows the order item with the new date and/or supplier.

6.  To transfer the item to Purchasing, go to the menu **Start > Execute**.
    The activated checks will be executed. Depending on the number of orders, this may take some time. Confirm the corresponding informative messages by selecting [Yes] or [No] to proceed with the checks. When all checks have been completed, the corresponding purchase orders will be created and thus transferred to Purchasing.
    The changed dates are saved in the order.
    When the items have been transferred, the P.O. number for the order is displayed.
    You can open and edit the generated purchase orders in **Documents > P.O.** Print the new purchase order and send it to the supplier.

## Compare prices in the order pool
If several suppliers have been entered for a product, you can compare prices in the order pool and select another supplier if required.

### How to compare prices in the order pool
1.  Go to **Documents > Order > P.O. transfer**.
2.  Move the orders to the order pool.
    This procedure is described in the previous unit.
    ⇨ "Transfer document to order pool" on page D-66
3.  Select the item for which you want to compare purchase prices.
    Double-click on the corresponding line header.

*Fig. D-39: Item for price comparison is marked*

Only items marked with an X have been selected.
4.  Go to the menu **Functions > Supplier prices**.

*Fig. D-40: Price comparison for item. A: !!! For all text colors: Delivery date is at risk, B: Text color red: Standard supplier, C: Text in green: most favorable supplier in terms of price, D: Text in blue: Standard supplier is most favorable supplier in terms of price*

5.  Tick the checkbox left from the supplier to whom the purchase order for this item is to be sent.
6.  Click **[OK]** to accept the change.
    The **Price comparison** dialog closes. The order pool shows the order item with the new supplier.
7.  Select the orders or order items you want to transfer to Purchasing.
    Double-click on the corresponding line header.

*Fig. D-41: Item with changed supplier*

8.  To start the transfer, go to the menu **Start > Execute**.
    The activated checks will be executed. Depending on the number of orders, this may take some time. Confirm the corresponding informative messages by selecting [Yes] or [No] to proceed with the checks. When all checks have been completed, the corresponding purchase orders will be created and thus transferred to Purchasing.
    Transferred items are removed from the order pool.

*Fig. D-42: P.O. numbers after transfer. A: First P.O. number, B: Second P.O. number*

When the items have been transferred, the old and the new P.O. number for this order are shown.
You can open and edit the purchase orders in **Documents > P.O.** Print the new purchase order and send it to the supplier.
Do not forget to inform the former supplier of the change.
