---
description: "EN_AWBusiness_Sales_4_4-1"
---


# Tutorial: Purchase Orders

This section covers the process of creating and managing Purchase Orders (P.O.s) after they are transferred from an order.

---
### Fig. C-176: P.O. numbers after transfer

This screen shows a list of orders in the "Order - 20 Entries" window after P.O.s have been generated.

**Key Observations:**
*   **A: Do not transfer item:** This points to orders where no P.O. number was generated, likely because the item was not flagged for purchase.
*   **B: Number of the order and created P.O.:** This points to an order (e.g., 20284) that now has a corresponding P.O. number (e.g., 7000019) in the "P.O. number(s)" column.

**Table: Order List**
| Order number | P.O. number(s) | Customer number | Customer | Status | Date Entry | Shipping date |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 20281 | | 1060 | Wolf Glasbau | 390 | 16.08.2013 | 16.08.2013 |
| 20282 | | 1000 | A+W Training | 390 | 27.08.2013 | 30.08.2013 |
| 20283 | | 4000 | A+W Training | 390 | 27.08.2013 | 02.10.2013 |
| 20284 | 7000019 | 4000 | A+W Training | 300 | 01.10.2013 | 18.10.2013 |
| 20285 | | 4000 | A+W Training | 390 | 01.10.2013 | 31.10.2013 |
| ... | ... | ... | ... | ... | ... | ... |

You can open and edit the purchase orders in **Documents > P.O.**
⇨ "Purchase Orders" on page C-309

## Change a P.O. in the Order Pool

If several suppliers have been entered for a product, you can compare prices and delivery terms in the order pool and select another supplier if required.

In addition, you must allocate a supplier to an item if no supplier is specified for the corresponding product in the master data.

The following instructions exist for this training module:
- "How to change the delivery date and the supplier" on page C-302
- "How to compare prices in the order pool" on page C-304

### How to change the delivery date and the supplier

1.  Go to **Documents > Order > P.O. transfer**.
2.  Go to the tab **Order pool**.

#### Fig. C-177: Change delivery date at risk

The "Order pool" screen lists items flagged for purchase that are ready to be transferred to a P.O.

**Key Observations:**
*   **A: Selection:** Checkbox to select an item for an action.
*   **B: P.O. already created:** Indicates that a P.O. (7000019/M) has already been created for this item.
*   **C: Date at risk:** A warning message "Delivery might not be on time" is displayed, indicating a potential scheduling conflict.

**Table: Order Pool**
| Select | Order | Item | Product | Supplier | Qty. | Width | Height | Delivery at customer's site | Supplier's deliv. date | Transfer to |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| X | 20284 | 2 | IG 4/16/Th4 A+W | 7025-Glass & More | 5 | 1200 | 1800 | 18.10.2013 | 18.10.2013 | 7000019M |
| X | 20284 | 5 | IG 4/16/Th4 A+W | 7025-Glass & More | 1 | 1200 | 1800 | 18.10.2013 | 18.10.2013 | |
| X | 20304 | 1 | Safe 6 mm A+W | 7010-ESG-Lieferant | 5 | 1200 | 1000 | 09.10.2013 | 09.10.2013 | |

3.  Select the item (A) for which you want to change the delivery date. Double-click on the corresponding line header. Only items marked with an X have been selected.
    If you have selected several items, the new delivery date is allocated to all items.
    If you only want to change one individual item, you can open the following dialog via double-click.

4.  Go to the menu **Functions > Change supplier/delivery dates**.

#### Fig. C-178: Change delivery date

This dialog allows you to modify the supplier and delivery dates for a selected purchase item.

**Dialog Fields:**
*   **Supplier/matchcode:** 7010 ESG-Lieferant Frankfurt/Main
*   **✔ Delivery at customer:** 09.10.2013
*   **✔ Supplier's deliv. date:** 09.10.2013
*   **Create reg. P.O. instead of internal order**

5.  Enter the new delivery dates.
6.  Search for another supplier if required.
7.  Click on [OK] to adopt the change.
    The dialog **Change supplier and delivery date** closes. The order pool shows the order item with the new date.
8.  To start the activity, go to the menu **Start > Execute**.
    The activated checks will be executed. Depending on the number of orders, this may take some time. Confirm the corresponding informative messages by selecting [Yes] or [No] to proceed with the checks. The P.O.s will be transferred after all checks have been completed.
    The changed dates are saved in the order.

### How to compare prices in the order pool

1.  Go to **Documents > Order > P.O. transfer**.
2.  Go to the tab **Order pool**.
3.  Select the item for which you want to compare supplier prices. Double-click on the corresponding line header. Only items marked with an X have been selected.

#### Fig. C-179: Item to be allocated to a more favorable supplier

This view is the same as the "Order pool" tab, where you select an item to begin the price comparison process.

4.  Go to the menu **Functions > Supplier prices**.

#### Fig. C-180: Changing suppliers for an order

The "Price comparison" dialog opens, showing prices from different suppliers for the selected item.

**Dialog: Price Comparison for "Safe 6 mm A+W"**

| Supplier | 7010-ESG-Lieferant | 7001-Glashütten-AG |
| :--- | :--- | :--- |
| **PCH Item** | **248.35** | **159.05** |
| Discount | 0.00% | 0.00% |
| Delivery time | 4 | 5 |
| Deliv. supplier | 09.10.2013 | 09.10.2013 |
| Deliv. to cust. | 09.10.2013 | 09.10.2013 |
| Price list | EK/Purchase | EK/Purchase |
| **TOTAL VALUES** | **248.35** | **159.05** |
| Selection Checkbox | (selected) | (unselected) |

> **Key:**
> *   **Low-price supplier**
> *   **Default and low-price supplier**

5.  Tick the checkbox left from the supplier to whom the purchase order for this item is to be sent.
6.  Click on [OK] to adopt the change.
    The dialog **Price comparison** closes. The order pool shows the order item with the new supplier.

#### Fig. C-181: Item with new supplier

The "Order pool" view now shows the item with the newly selected, more favorable supplier (7001-Glashütten-AG).

## Change P.O. Code

In the number manager, you can change the procurement type and the supplier of an order. If you only change the procurement type, the purchase items are ordered from the standard supplier.

### How to change the P.O. flag

1.  Select **Documents > Order > NM Order**. The **Number manager** dialog opens.
2.  Select the menu **Functions > Edit group > Change P.O. flag**.

#### Fig. C-182: Change P.O. flag (code) on item level

The "Change P.O. flag" dialog allows for bulk changes to procurement settings.

**Dialog Options:**
*   **A - Mode (Level of change):**
    *   Change on item level
    *   Change on BOM level
    *   Change on document level
*   **B - Supplier:**
    *   ✔ Change supplier
    *   [Dropdown for supplier selection, e.g., 7003 Dorma Glas GmbH]
*   **C - Procurement types (Flag for changing):**
    *   ✔ Change procurement type
    *   From: `000 - Produktion/Production`
    *   By: `009-Bestellung/Purchase product`
*   **D - Restriction to product:**
    *   Only for product [Product number input]

3.  Select the mode (A).
    In the below example, we choose **Change on item level** to amend the flag for the order items (main product) in general.
4.  Tick **Change procurement type (C)** and choose the previous and the new procurement type.
    The procurement type for all items is changed. If you have selected the procurement type **Purchase product**, you can also select a certain supplier.
5.  If the change shall apply to a certain product only, enter the product number (D). The product name is shown.
6.  Tick the checkbox **Change supplier (B)** if necessary and select a new supplier. All purchase items are ordered from the chosen supplier. You can also select this setting without changing the procurement type.
7em.  If required, tick the checkbox **P.O. directly to customer**. In this case, the ordered goods will be delivered directly to the customer's site. This is only useful if the ordered parts are not required for production.
8.  Click on [OK] to save the data. The new flag is saved in all documents of the current number manager.
9.  Click on [End] to close the dialog. The dialog **Change P.O. flag** closes. The changes will be saved in the orders.

> **If items were changed that had already been transferred, you must decide what to do next:**
> *   **The supplier has already confirmed the order:** Discuss the changes with purchasing and with the supplier. Cancel the old P.O. if necessary and transfer the changed item again.
> *   **The P.O. has not been sent to the supplier yet, or the supplier has not yet confirmed the order:** Transfer the item once more and notify purchasing of the change if necessary.
> The dialog **Document data** can be used to edit the dates and notify the customer of the changes.

7.  Transfer the items for the purchase order to purchasing, as described in the first activity sequence above.

---

## Exercises

**Enter purchase item**
Open an order and enter two items.
*   Select the **P.O. flag** for one of the items.
*   For the other item, select the flag **P.O. (complete)**.

**Transfer order**
Move the order to the order pool.
*   Check the suppliers and the prices in the order pool.
*   Change the delivery date.
*   Transfer the purchase orders:
    *   Check whether a P.O. has been created for all items with the P.O. flag.
    *   Check the dates and supplier in the new P.O.s.

---

# Purchase Orders (Overview)

## Objectives
*   Getting familiar with purchase orders.
*   Reference P.O. versus stock P.O.

## Benefits
*   You will know the difference between reference purchase orders and independent purchase orders.
*   You can view a list of purchase orders created from a certain order to see whether the order can be processed further.

## Note

| Feature | Description |
| :--- | :--- |
| **Create document** | Purchase orders can be created in different ways: <br> - Transfer to purchasing creates purchase orders from an order. <br> - By entering a purchase order. These purchase orders usually serve to replenish the stock. They will be dealt with in the module on Purchasing. |
| **P.O.** | Purchase orders are structured in the same way as orders. |
| **References** | References point to the order from which the purchase order has been created. |
| **Purchasing info**| Shows all purchase orders referring to the order in question. |
| **Changes** | If a date is changed in a reference P.O., this amendment will be saved in the order. |
| **Default settings**| None. |

## P.O. Document Header

In this module, purchase orders will be created from orders containing items for which the P.O. flag has been set. Purchase orders which do not refer to orders are described in closer detail in the section Purchasing.

For the order created in the previous training module, two purchase orders were issued. Both purchase orders have the same structure as the orders handled at the start of this training session.

### Fig. C-183: P.O. from an order

The following screen shot shows the document header of the first purchase order. The delivery date at the customer has been changed for this purchase order additionally.

**Key Observations:**
*   **A: Changed delivery date:** The delivery date has been set to 28.08.2015.
*   **B: Order for which the P.O. was created:** This section lists related documents. In this case, it might refer to the original customer order number.

## P.O. Item

The items of a P.O. also refer to the customer order.

### Fig. C-184: Purchase item based on the order

This screen shows the item details within a Purchase Order.

**Key Observations:**
*   **A: Reference to customer:** This section indicates the customer-facing details, such as "Customer item".
*   **B: Note:** The "Note" column explicitly states "Item already scheduled in a...", indicating its origin from a customer order.

In the column **Note (B)**, you can see that this P.O. has been created from an order.

## Order/P.O. Info

From the section on the history, you will know that all reference documents for an order are displayed. This history does not show any details of the documents however. Information on purchase orders referring to a certain order is available from the dialog **Order/P.O. info**.

### Fig. C-185: Order and P.O. info

This dialog lists all purchase orders issued for the items of a specific customer order.

**Dialog View:**
*   Shows P.O. number `7000019` related to Order number `20284`.
*   Lists the item, quantity, dimensions, price, and delivery date.
*   Tells you for which purchase orders goods have been received so far and when the delivery in total can be expected.

## Exercises

**Enter purchase order**
Enter an independent P.O.
*   Enter five boxes of float 5 mm for an item.
*   Enter five boxes of float 5 mm for an item.

**Change P.O.**
Change the supplier in the reference P.O.
*   Change the supplier for item 1.
*   Change the supplier for the entire order.

**Show references**
Check the references:
*   in the dialog **Order/P.O. info**
*   in the dialog **History**.

---

# Document Data

## Objectives
*   Getting familiar with the functions of the dialog.
*   Changing the delivery date in the order.
*   Collecting documents for common changes.

## Benefits
*   You can check and change the dates and suppliers in reference documents in one go.
*   If you have organized your number managers accordingly, you can carry out changes for all the documents collected therein in one go.

## Note

| Feature | Description |
| :--- | :--- |
| **Document data dialog** | In the dialog **Document data**, you can check the dates for the following documents and reference documents: Quotation, Order, P.O., Inquiry, Credit note. |
| **Reference documents** | Reference purchase orders are only shown for one single order. They are not shown when documents of a number manager are listed. |
| **Common changes** | Status, dates, route and delivery terms can be changed for several documents at once. |
| **Default settings** | **Master data:** <br> - Customer: Fax number and/or e-mail address <br> **Text:** <br> - Standard text for customer notifications <br> **Forms management:** <br> - Print items, forms <br> **Status:** <br> - Status points must have been created and assigned. |

## Show Delivery Data

An overview of the document data is available in the dialog **Document data**. This dialog permits to edit parts of the header such as the status or the dates. You can change a single document or several documents at once. The documents can be loaded from a number manager or collected by means of their document numbers. This dialog also allows to list all reference purchase orders together with the order. In this constellation, the changes will also be applied to the reference purchase orders.

### Fig. C-186: Check dates for orders containing purchase items

The "Document data" dialog displays both the customer order and its associated reference P.O.s in separate panes.

*   **A: Order with purchase items:** The top pane shows the customer order details (e.g., Order 1168).
*   **B: Reference P.O.s:** The bottom pane lists the purchase orders linked to that order (e.g., P.O. 51855).

## Delivery Date Check

You can check the delivery dates of orders and purchase orders and correct them if necessary. This is done in two steps:
*   Check and correct the dates in the dialog **Document data**. This way, the dates will be automatically amended in the order and in the purchase order.
*   Use the dialog **Customer information (delivery date check)** to inform the customer of the delay. You can also use the options in the menu **Communication** to inform the customer, or just call him/her.

P.O.s can be checked by means of the delivery date check. If shipments are delayed, you can change the dates and inform the customer right away.

## Document View

The document view can be viewed and printed from the dialog **Document data**. You can check the document details without leaving the dialog **Document data**.

When printing the document view, the system will not use the defined forms; nor will the document status be raised. This printout should not be mixed up with the "official" printout because, in this case, the main headers and footers are omitted.
⇨ "Form and Label Printing" on page C-187

## Check and Change Delivery Date

The dialog **Document data** can be used to view the reference P.O.s together with the order in order to check dates and change them if necessary.

The following instructions exist for this training module:
*   "How to check and change referenced documents" on page C-317
*   "How to inform the customer of the new delivery dates" on page C-319

### How to check and change referenced documents

1.  Go to **Documents > Document data**. The dialog **Documents** opens.
2.  Make sure that the checkbox **Number manager** is unchecked. The field for the order number is only enabled if no number manager is displayed.
3.  Enter the order number and adopt the data by pressing <Enter>.

#### Fig. C-187: Check dates for orders containing purchase items

The header data of the order and purchase order(s) are displayed.
*   **A: Adjust shipping date:** In the top "Order" pane, you can adjust the customer-facing shipping date.
*   **B: Adjust confirmed date of supplier:** In the bottom "P.O." pane, you can adjust the delivery date confirmed by the supplier.

4.  Adjust the delivery date **(B)** that the supplier has specified for the P.O.
5.  Adjust the date for the shipping date **(A)** and/or delivery at the customer's site. If you select the dates from the calendar, you can take the customer's route days into account.

#### Fig. C-188: Changed dates

This screen shows the **Document data** dialog after the dates have been updated. For example, the P.O. delivery date is now 22.03.2013 and the order shipping date is 25.03.2013.

6.  Go to the menu **Start > Save** to save the data. The new dates are saved and adopted for the corresponding documents. You can inform the customer of the new date now.

### How to inform the customer of the new delivery dates

> **Prerequisite**
> An email address must be defined in the customer's master data. In the order itself, the checkbox **Email** must be ticked in the **Address** section.

1.  Select **Documents > Customer information**. You can also open this dialog from an order. However, using this method, you can no longer change the delivery date of the current order since it is open and thus locked.

#### Fig. C-189: Customer information

The "Customer information" dialog is used to manage and communicate delivery date changes.

**Dialog Sections:**
*   **A: Mode:** Select `Orders` or `P.O.s`.
*   **B: Restriction to number manager:** Filter documents by a specific number manager.
*   **C: Restriction to status:** Filter documents up to a certain status.
*   **D: Restriction to date:** Filter for a specific delivery date.

2.  Select the mode **(A)** `Orders` or `P.O.s`. In the following example, a customer is to be informed about the delivery date postponement of its order.
3.  Restrict the selection to a number manager **(B)** or a status **(C)**. If the number manager includes a large number of documents, you can restrict the view to one delivery date **(D)**.
4.  To import the data, go to the menu **Start > Search**.

#### Fig. C-190: Change delivery date at the customer's site

The **Postponement** tab lists orders and allows for bulk changes to delivery dates.

**Tab Features:**
*   **A: New delivery date:** Field to enter a new delivery date for selected orders.
*   **B: Delivery date postponed:** An icon or flag indicates that an order's delivery date has been postponed at least once.
*   **C: Create customer information for the selected order:** Checkbox to select which orders to include in the notification.

5.  In the **Postponement** tab, select the order **(C)** for which you have to change the delivery date at the customer's site and check the new date **(A)**. You can select several orders and define a new delivery date. In this case, you can only change the route if all orders are to be delivered with this route.
6.  Go to the menu **Start > Save** to save the data.
7.  Go to the menu **Print > Printer**. The message is displayed and can be saved and sent in accordance with the output format.

## Collect Documents for Common Changes

If you want to change the route for several orders at once, for example, you can compile these documents in a number manager and amend them. Alternatively, you can compile the orders in the dialog **Document data** and change them together.

### How to collect documents for common changes

1.  Go to **Documents > Document data**. The dialog **Document Data** opens.
2.  Go to the field **Document** and select the document type, e. g. **Order**.
3.  Make sure that the checkbox **Number manager** is unchecked.
4.  Enter the order number and adopt the data by pressing <Enter>. The order data is shown on the list.
5.  Repeat this step until you have compiled all orders to be changed together. The list shows all orders.
6.  Change e.g. the route in the section **Order**. In addition, you can change the delivery date if all orders are to be delivered on the same day.
7.  Go to the menu **Start > Save** to save the data. The new route is adopted for all listed orders.

## Exercises

**Check document data**
*   Check the reference documents in the dialog **Document data**.
*   Change the production date and change the delivery date accordingly.

**Additional Information**
*   ⇨ Software Reference, "Document Data" on page C-733
*   ⇨ Software Reference, "Customer Information (Delivery Date Check)" on page C-560

---

# Quotations

In this thematic block you will learn how to enter quotations and alternative quotations.

## Quotation Entry

### Objectives
*   Getting familiar with the difference between quotations and orders.
*   Getting familiar with the difference between alternative quotations and alternative items.
*   Entering alternative items.
*   Entering a complete alternative quotation for a quotation.

### Benefits
*   An alternative quotation can be used to enter suggestions based on the customer's wishes, and subsequently add those items to the order the customer decides to go ahead with.
*   You do not have to reenter the data from the quotations to create the corresponding order.

### Note

| Feature | Description |
| :--- | :--- |
| **Quotation** | A quotation is entered in A+W Business under the following circumstances: <br> - Estimate for the customer <br> - Alternative proposals for a future order <br> - Price alternatives for replaced sheets, grills, shapes and processing steps |
| **Document** | Quotations are independent documents. There is a separate number area for quotations. Quotations can be created in various ways: <br> - by copying an order <br> - by entering a new document |
| **Alternative quotation** | Alternative quotations are managed in the quotation number area. |
| **Default settings** | **Master data:** <br> - Number areas <br> **Company data:** <br> - System tab (resubmission) <br> - Production tab (optimization) |

## Quotation and Alternatives

The commercial process starts with a quotation. Enter all data with the required specifications. A+W Business checks - during entry - whether the entered products are available on stock or have to be produced, and whether the defined restrictions are met. This makes sure that the offered items can be actually produced.

Quotations are entered in the same way as orders.

### Alternative items
For every item, you can enter alternative items that are not included in the quoted total. When the customer has accepted a quotation, you can use the copy function to change it into an order, selecting the required items.

### Alternative quotation
In addition to alternative items, you can also create alternative quotations. For example, you can replace sheets, change, add or delete shapes, grills and processing steps for items.

When you create an alternative quotation, the data from the document header will be adopted automatically. You only have to edit the item data. The alternative quotation can be saved as a separate document. An overview shows the alternative quotations which have been created for a quotation.

### Resubmission
The dialog **Resubmission** can be used to view all quotations to be resubmitted within a certain period.

#### Fig. C-191: Automatic report at the system start
A system dialog box appears with the message:
> ? There is at least one document for resubmission. Do you want to view it/them now?
> [Ja] [Nein]

You can define a resubmission date for every quotation in every order as an automatic reminder for yourself to contact the customer again.

The resubmission function is described in detail in a separate module.
⇨ "Quotation Follow-up" on page C-338
