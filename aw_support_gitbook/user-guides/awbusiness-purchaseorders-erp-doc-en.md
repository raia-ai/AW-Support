---
title: "EN_AWBusiness_Purchasing_3_30_2-1"
source: "EN_AWBusiness_Purchasing_3_30_2-1.pdf"
tags: ["Purchase Orders", "A+W Business", "ERP", "Inventory Management", "Supplier Management", "Order Processing", "Delivery Dates", "Inquiry", "Technical Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical tutorial on managing purchase orders within the A+W Business Purchasing module. It covers checking and changing delivery dates, handling postponements, creating inquiries for P.O. items, and converting inquiries into purchase orders."
long_description: "This document provides a detailed, step-by-step tutorial for the A+W Business Purchasing module. It is designed to guide users through various purchasing-related tasks. The first major section focuses on managing purchase orders, specifically how to check and adjust delivery dates. This includes instructions for searching for orders, restricting views by date, and updating delivery schedules for customers. The tutorial explains how to handle postponed deliveries and notify customers of changes. It then moves on to a more advanced feature: checking and changing all dates collectively using the 'Document data' dialog. This allows for bulk updates to multiple orders and purchase orders simultaneously. The second major section details the process of creating and managing inquiries. It explains the benefits of using inquiries to agree on dates and capacities with suppliers before committing to a purchase. The tutorial outlines how to create an inquiry from a customer order (for a P.O. item), and how to convert an accepted inquiry back into a formal purchase order, both from a referenced order and as an independent inquiry. The document includes screenshots of the user interface with labeled components to guide the user through the software's dialogs and menus. The final part includes exercises and references to related topics like receipt of goods, stock management, and master data setup."
---

# Tutorial: Purchase orders

---
## Check delivery dates

1.  Select the option **(A) Orders** or **P.O.s** and the Number Manager if required. If the Number Manager includes very many documents, you can restrict the view to the originally scheduled delivery date **(B)**.
2.  To import the data, go to the menu **Start > Search**.

*(Fig. D-59 shows the "Check delivery dates" screen. It highlights (A) the 'Orders' radio button, (B) the 'To delivery date' filter, and (C) the 'New delivery date' column. A legend explains that 'A' indicates a customer has not been informed of a new date, 'B' is the scheduled delivery date from the order, and 'C' is the new delivery date.)*

*   **A**: Customer has not been informed of the new date yet
*   **B**: Scheduled delivery date stated in the order
*   **C**: New delivery date

5.  Select the order for which you want to change the date of delivery to the customer and go to the **Postponement** tab.

*(Fig. D-60 shows the "Change the date of delivery to the customer" screen within the Postponement tab. It highlights (A) the 'New delivery date at customer's site' field and (B) the selected order row for which the change applies.)*

6.  Select the order **(B)** for which the customer date is to be postponed. You can select several orders if they all have the same delivery date and route.
7.  Enter the new date **(A)** and change the route if necessary.
8.  Go to the menu **Start > Save** to save the changes. You can print the new date for the customer and dispatch it via the usual communication channel.
9.  Go to the **Print menu** and select the printer. The notification is created and can be dispatched. If you have changed several dates, a notification will be issued for each customer.

## Check and change all dates

The **Document data** dialog can be used to view all purchase orders and orders to check the delivery dates as well as the production dates and change them if necessary. You can compile orders, e.g. in order to change the dates in several orders at the same time.

The following instructions exist for this training module:
*   "How to check and change document data" on page D-103
*   "How to collect documents for common changes" on page D-106

### How to check and change document data

1.  Go to **Documents > Document data**.

*(Fig. D-61 shows the empty "Document data" dialog. It highlights (A) the 'Document type' selection dropdown (e.g., Order) and (B) the 'Number' field for the document to be searched.)*

2.  Select the document type, e.g. **order** or **purchase order**. You can also view all documents from one Number Manager. In this example, one single order is to be checked. You can change the dates for several orders and/or purchase orders that are not in a collective Number Manager. (See "How to collect documents for common changes" on page D-106)
3.  Enter the order number and adopt the data by pressing `<Enter>`.

*(Fig. D-62 shows the "Document data" dialog populated with data for a specific order. The fields in the 'Order' area show data from the order header. The P.O. data appears in the fields in the 'P.O.' area. It highlights (A) the customer date fields like 'Shipping date' and 'Delivery', and (B) the supplier date fields like 'Delivery date' in the P.O. section.)*

4.  Adapt the supplier date **(B)** and customer dates **(A)**. If you select the dates from the calendar, you can take the customer's route days into account.
5.  Go to the menu **Start > Save** to save the data. The new dates are saved and adopted for the corresponding documents.

*(Fig. D-63 shows the same dialog after the dates have been changed and saved. You can inform the customer of the new date now.)*

### How to collect documents for common changes

1.  Go to **Documents > Document data**.

*(Fig. D-64 shows the "Document data" dialog for collecting documents. It highlights (A) the 'Document type' (e.g., Order), (B) the 'Number' field for entering an order number, and (C) the unchecked 'Number Manager' checkbox.)*

2.  Select the document type, e.g. **order (A)**.
3.  Make sure that the checkbox **(C) Number Manager** is unchecked.
4.  Enter the order number **(B)** and adopt the data by pressing `<Enter>`. The order data is shown on the overview. The section P.O. lists the reference purchase orders.
5.  Repeat this step until you have compiled all orders to be changed together. Make sure that all orders with the same route can be delivered and that they have the same delivery date.

*(Fig. D-65 shows the "Orders for collective date change" view, where multiple orders are listed in the overview. It highlights (A) the 'Order dates' and (B) the 'P.O. dates' that can be changed collectively.)*

6.  Select all listed orders by keeping the `<Ctrl>` key pressed.
7.  Change the dates **(A, B)**.
8.  Check the route and change it if necessary.
9.  Go to the menu **Start > Save** to save the data. The new dates will be applied to all listed orders and the reference purchase orders. You can notify the customer now.

# Inquiry

**Objectives**
*   Obtaining inquiries from suppliers
*   Generating a P.O. from an inquiry
*   Obtaining inquiries for an order item

**Benefits**
*   To agree on dates and capacities, inquiries can be made via the order pool.
*   An inquiry can be turned into a purchase order without having to enter the data again.

**Please note:**
*   **Inquiries**: Like purchase orders, inquiries can be entered manually or can be created from a customer order by means of the order pool.
*   **P.O.**: Purchase orders can be created from any type of inquiry.
*   **References**: References to order items are kept in the inquiry and in the purchase order if these are created from the order pool. If a purchase order is created by copying an inquiry, the reference exists only between these two documents.
*   **Default settings**: Master data: Supplier > Order tab

## Inquiry for P.O. items or purchase orders

Inquiries are created and sent to the supplier in the same way as purchase orders. When the quotation comes in and is accepted, you can turn the inquiry into a purchase order without having to enter the data once more. You can use the function **Copy document** for this purpose.

You can also create inquiries for P.O. items from a customer order.

*(Fig. D-66 provides a flowchart illustrating the "Inquiry - P.O." process.
- An Order can lead to an Inquiry via "P.O. transfer Direct inquiry", which can then be copied to a P.O. (with no reference to the original order).
- An Order can also go into the "Order pool", become an Inquiry (with a reference to the order), and then a P.O. (also with a reference to the order).
- An "Independent inquiry" can be created and copied to an "Independent P.O.")*

If the option **Direct inquiry** was selected during the P.O. transfer, inquiries from a customer order are also generated. If this is done by means of the order pool, you can even create inquiries for individual order items and select a certain supplier.

Of course, these inquiries can also be turned into purchase orders. The reference to the order will be kept only if the resulting purchase orders are created by means of the order pool as well.

Independent inquiries are created in the same way as orders and purchase orders. The **Documents** module offers the **Inquiries** menu for this purpose.

## Create an inquiry for a P.O. item

You can create an inquiry for a P.O. item, e.g. to find out whether the supplier can offer the necessary capacity. Every inquiry can be turned into a purchase order by means of the order pool.

The following instructions exist for this training module:
*   "How to create an inquiry based on a customer order" on page D-110
*   "How to create a P.O. from a reference inquiry" on page D-111

### How to create an inquiry based on a customer order

1.  Go to **Documents > Order > P.O. transfer**.

*(Fig. D-67 shows the "Transfer orders from the Number Manager" screen. It highlights (A) the 'Transfer mode' set to 'Direct inquiry', (B) the selected 'Number Manager with orders for transfer', and (C) the 'Target Number Manager' where the inquiries will be placed.)*

2.  Select the mode **Direct inquiry (A)** and the Number Manager **(B)** you used to collect the orders with P.O. items.
3.  Select the target Number Manager **(C)** to which the inquiries shall be made. You can enter a new name and thus create a new Number Manager. If you select another user, the Number Manager will be allocated to him/her.
4.  Choose the **Client** and the **OM area** in the section **Target number area** if required.
5.  To transfer the items, go to the menu **Start > Execute**. Confirm the positive report. An inquiry has been created for every P.O. item. You can use **Documents > Inquiry** to open and print the inquiries and send them to the supplier.

### How to create a P.O. from a reference inquiry

1.  Open the **P.O. transfer** dialog.

*(Fig. D-68 shows the "Transfer orders from the Number Manager" screen again. This time it highlights (A) the 'Transfer mode' set to 'Fill pool', (B) the 'Number Manager' containing the inquiries, and (C) the 'Target Number Manager'.)*

2.  Select the Number Manager **(B)** that includes the orders for which you have created inquiries.
3.  Choose the option **Fill pool (A)**.
4.  To move the orders to the order pool, go to the menu **Start > Execute**. The P.O. items are imported and the display changes to the **Order pool** tab.

*(Fig. D-69 shows the "Create P.O.s for orders" screen in the Order pool tab. The document numbers of the inquiries are shown for the inquiry items from the order. It highlights (A) the 'P.O.s' mode, (B) the list of inquiries generated, and (C) the 'Target Number Manager' for the new P.O.s.)*

5.  Select the option **P.O.s (A)** and the target Number Manager **(C)** for P.O.s.
6.  Select the items for which a purchase order is to be created. Double-click on the corresponding line header. Only items marked with an **X** have been selected.
7.  To generate purchase orders, go to the menu **Start > Execute**. Purchase orders have been created. The transferred items are removed from the order pool. You can use **Documents > P.O.** to open and print the purchase orders and send them to the supplier.

## Create a purchase order from an independent inquiry

You can create a purchase order from any inquiry with the copy function, no matter whether the inquiry is referenced or not. References to customer orders will not be adopted however. The copy function is described in detail in the **Sales** section.

### How to enter a purchase order for an inquiry

1.  Open the inquiry for which you want to enter a purchase order.
2.  Select the menu **Functions > Document group > Copy documents**.

*(Fig. D-70 shows the "Creating a P.O. from an inquiry" dialog (Copy documents). It highlights (A) the 'Target document type' being set to 'P.O.', (B) the 'Copy mode', and (C) the 'Target Number Manager'.)*

3.  Select the document type **P.O. (A)**. The Target area automatically shows the first Number Manager for purchase orders.
4.  Choose a different target Number Manager **(C)** if required.
5.  Check the other settings.
6.  To generate the purchase order, go to the menu **Start > Execute**. The items are checked and copied. The purchase order is saved.
7.  Close the dialog. The **Copy documents** dialog disappears and is replaced by the **Document management** dialog. The inquiry and P.O. history shows the reference. You can use **Documents > P.O.** to open and print the generated purchase order and send it to the supplier.

# Exercises

The structure of the exercises is such that every aspect of purchasing is conveyed. This means that the purchase orders created by means of these exercises can be processed further in the next subject.

> **Checking prerequisites and master data**
> When working with your own system please make sure that the settings in master data meet the requirements for the smooth entry of documents and goods received.
> Please also make sure that the document status is changed correctly if the documents are to be processed further, e.g. in the order pool.

### Enter a P.O. item in the order

Enter a customer order with the following items:
*   Items with different purchase codes.
*   Items which can be provided by different suppliers.
*   Items which do not have to be ordered.

> **Tip**
> Create 2-3 copies of the orders and of the manual purchase orders so that you can check the different effects of amendments, e.g. change of supplier on different levels.

### Enter a manual P.O.

Enter a purchase order with the following items:
*   Items with stock articles and products which are not kept on stock.
*   Items with different boxes.
*   At least five boxes per item

### Transfer the order to Purchasing

Transfer the orders to Purchasing:
*   at least one order directly (without order pool).
*   at least one order via the order pool.
*   Now check the new purchases order for differences.

### Enter order confirmation and check prices

Enter an order confirmation for at least one reference and one manual purchase order each.

### Check and amend delivery dates, notify customer

Enter the following changes:
*   Enter a larger amount in an item in a reference order and transfer the item again.
*   Select another supplier because he cannot keep the originally confirmed dates.
*   Change the delivery date in a purchase order, then inform the customer of the delay.

### Remind supplier

Search for purchase orders for which you have not entered an order confirmation yet, and send a reminder to the supplier.

### Additional information

*   "Supplier file" on page D-30
*   "Deliveries in receipt of goods" on page D-117
*   "Dealing with boxes" on page D-134
*   "Receipt of boxes" on page D-133
*   "Electronic document exchange" on page D-148

### Sales section

*   Sales, "Copy Documents" on page C-206
*   Sales, "Copy Documents" on page C-461
*   Sales, "Order/P.O. Info" on page C-486
*   Sales, "Document Data" on page C-644

### Master data section

*   Master Data, "Product" on page B-139
*   Master Data, "Currencies" on page B-450
*   Master Data, "Stock Sizes" on page B-626
*   Master Data, "Prices" on page B-701
*   Master Data, "Customers, Suppliers" on page B-745
*   Master Data, "Company Data" on page B-900
*   Master Data, "Show items w/o stock code at receipt of goods on stock" on page B-933

### Stock management section

*   Inventory Management, "Stock Management" on page G-60
*   Inventory Management, "Stock P.O. (automatic)" on page G-107
*   Inventory Management, "Stock Management - Stock Articles" on page G-198
*   Inventory Management, “Stock Movement – Dispatch, Addition” on page G-208

# Deliveries in receipt of goods

This subject shows you how to check the prices and invoices and enter the receipt of goods.

This includes the following training modules:
*   "Receipt of goods" on page D-118
*   "Receipt of boxes" on page D-133
*   "Price and invoice control" on page D-141

Receipt of goods usually includes the following steps:
*   Enter a delivery as receipt of goods
*   Check receipt of goods for outstanding or incomplete deliveries
*   Check the invoice.
*   Transfer documents to archives and statistics.
*   Delete document from main database.

This sequence more or less matches the sequence of dialogs in A+W Business. Some of the steps can be executed in different dialogs however. This is why they have been summed up in one training session.

The prices on the order confirmation are naturally checked prior to the receipt of goods. This tutorial describes price control and invoice control together because the corresponding dialogs are structured in the same way.

Archiving of documents has already been introduced in the Sales tutorial which is why we are not going to deal with this again at this point.

## Receipt of goods

**Objectives**
*   Learning about the Receipt of goods dialog.
*   Learning about the difference between goods received for stock P.O.s and for reference P.O.s.
*   Checking received goods for completeness.
*   Being able to add omitted 'goods received' bookings.

**Benefits**
*   Deliveries must be entered so that customer order can be completed and shipped.
*   The stock is updated when goods received for stock are entered so that you always have a good idea of the actual stock on hand.
*   Receipt of goods can be entered even if the ordered quantity differs from the quantity delivered.

**Please note:**
*   **Incomplete delivery**: Partial receipt of goods can be entered if the delivered quantity does not match the quantity ordered.
*   **Surplus quantities**: If the stock articles delivered (with a stock ID) exceeds the number of stock articles ordered, this quantity will be booked on stock. The receipt of goods of surplus quantities will only be booked if you have ticked the **Accept** checkbox. Surpluses for customers orders must be permitted and restricted in the master data.
*   **Default settings**:
    *   **Company data**:
        *   Parameters tab
        *   Stock/PP/EDI tab
    *   **Master data (surplus)**:
        *   Customer, supplier
        *   Product

## Deliveries

When entering goods received, a distinction is made between the receipt of boxes, stock P.O.s, independent, and reference purchase orders.

*(Fig. D-71 shows a diagram of "Receipt of goods and stock bookings".
- **Stock P.O.** -> Booking in stock on hand
- **Box** -> Assignment of IDs -> Booking in stock on hand, Status in ref. documents
- **Reference P.O.** -> Booking in stock on hand only for stock articles
- **Independent P.O.** -> No booking in stock on hand)*

This distinction helps Stock Management to maintain the stock data. After booking the receipt of goods, all automatic surcharges for the purchase order are recalculated and saved.

### Receipt of goods for stock P.O.s

Booking the receipt of goods for stock P.O.s updates the stock on hand. The **Stock info** dialog shows the reserved quantities in addition to the stock on hand. This gives you a proper idea of the current and the future stock on hand even at item entry.

Even stock P.O. items that include articles without stock codes are displayed at receipt of goods, and can be booked. These bookings will not change the stock on hand however.

### P.O. item for production

If you have entered a P.O. item in a customer order which is necessary for producing this order, it can be processed further only after receipt of goods. When you enter the receipt of goods, production must be informed so that the order can be produced.

You can enable an option in receipt of goods which automatically triggers the transfer as soon as the receipt of this item has been entered.

For order items with the code P.O.(complete), the status is changed and passed on to the order so that the order can be shipped.

*(Fig. D-72 shows the "Receipt of goods - Purchase orders in the Number Manager" screen. It highlights (A) Delivery date of the selected P.O., (B) Completely booked receipts in blue, (C) An indicator for a lock status, and (D) The reference order for the selected P.O.)*

### Items without stock codes

If you enter stock P.O.s with items which are not recorded as stock items, they will not be displayed at receipt of goods. You can however enable the corresponding option in the company data.

*(Fig. D-73 shows the Company data – Stock/PP/EDI tab, highlighting (A) the "Show items w/o stock code at receipt of goods on stock" checkbox to activate the display.)*

### Partial receipt of goods

Receipt of goods can be booked in full or partially. Partial receipt of goods can apply to individual items as well as to partial deliveries for individual items, e.g. items 5 and 7 of a purchase order or 15 pcs. of an item for which 30 pcs. had been ordered. The status of the purchase order and/or the order will be set accordingly afterwards.

### Receipt of goods for BOM elements

BOM elements are not listed individually in receipt of goods but belong to the corresponding main product. The article description shows the BOM elements separated by "/".

### Deliveries with surpluses

If a supplier delivers more pieces of an item than have been ordered (surplus), you can enter this delivery at receipt of goods. In case of stock articles (with a stock ID) from a document of the type Stock P.O., the delivered quantity is added to stock. In the P.O. itself, the quantity is changed accordingly.

The same applies to shortfalls which are rather infrequent in practice however. The surpluses and shortfalls are defined in the following dialogs:
*   **Per customer and per product**: Relative amount of divergence.
*   **Per product**: Relative amount of divergence.
*   **Per order item**: also divergent quantity

### Inspection of goods received

The **Inspection of goods received** dialog offers a quick overview of open or incomplete deliveries.

*(Fig. D-74 shows the "Control of the receipt of goods" dialog. It highlights (A) P.O. number, (B) Ordered quantity, (C) Delivered quantity, and (D) a checkbox for 'Receipt of goods complete'.)*

You can make up for the booking of purchase orders or P.O. items for which the receipt of goods has not yet been entered although they have been delivered.

### Check the default settings for receipt of goods

The default settings for the receipt of goods have to be made in company data. The corresponding parameters and options are found on the following tabs:
*   Parameters
*   Stock/PP/EDI

*(Fig. D-75 shows the Company data – Parameters tab, highlighting (A) the "Use virtual item numbers" checkbox for the receipt of boxes.)*

Virtual item numbers are created so that the boxes received can be booked correctly. This function is described in the unit on the receipt of boxes. (See "Receipt of boxes" on page D-133)

### Stock on hand

To be able to update the stock on hand based on the booked receipts, the reservation option and the stock management on BOM level have to be enabled in company data.

*(Fig. D-76 shows the Company data – Stock/PP/EDI tab. It highlights (A) 'Update of inventory in case of reservations' for reservation and updating of stock on hand, and (B) 'Stock control on BOM level'.)*

## Enter receipt of goods

You can use receipt of goods to enter the supplier's order confirmation (OC) number and change the delivery date. You can book partial deliveries by entering the quantity delivered for an item, or by just marking individual items as completely delivered.

**Entry in receipt of goods**
Generally the document numbers are entered via the barcode scanner. They are entered manually for the following examples. All other steps are identical for both variants.

The following instructions exist for this training module:
*   "How to enter complete receipt of goods" on page D-126
*   "How to enter partial receipt of goods" on page D-128
