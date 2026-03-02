---
description: "EN_AWBusiness_Sales_4_3-3"
---


---
## Copy Documents

### Exercises

**Copy entire document**
Copy an order so that an identical order is created.

**Copy document, item by item**
Copy the order with IG items containing grills. Adopt the following details:
- Change the quantity of item 1.
- Do not adopt item 2.
- Adopt item 3 as it is.

**Additional information**
- "Updating order totals" on page C-139
- "Enter Complaint" on page C-281
- Software Reference, "Copy Documents" on page C-527
- Software Reference, "History" on page C-547
- Software Reference, "Recalculate" on page C-671

## Partial Deliveries

### Objectives
- Entering partial delivery

### Benefits
- You can schedule capacities more effectively by handling a major order by means of smaller, partial deliveries.
- You can enter partial deliveries for an order without having to enter new data.
- Orders with (several) partial deliveries can be billed by partial invoices.

### Note

**Partial delivery**
Partial deliveries are entered in A+W Business based on the following conditions:
- Shipping of a partial quantity of an order item
- Shipping an individual item if the order includes several items.
Partial delivery creates an order of the type *Partial delivery*.
A separate number area is used for partial deliveries.

**Document**
Partial deliveries can be created in various ways:
- by copying an order
- by entering a new document

**Invoice**
Partial deliveries can be created with or without a partial invoice.

**Partial invoice**
Partial invoices are created by means of a print item. Like (common) invoices, they are not separate documents.

**Default settings**
Master data:
- Status Administration
- Status allocation
- Number areas
- Customer Data

Company data:
- Parameter tab (delete items, date)
- Documents tab (lock code)
- Tab Stock / PU / EDI (registration point assignment)

### Partial Delivery for an Order
Partial deliveries are agreed by customer. Enable the function in the customer's master data and also define whether partial deliveries can be invoiced. The function *Partial delivery* will then be automatically enabled in document management.

**Fig. C-137: Customer master data - partial delivery, partial invoice**
*UI screenshot showing checkboxes for "Partial delivery" and "Partial invoice" enabled in customer master data.*

The partial delivery is created from an order but the partial delivery note is a separate document with its own document number, which is loaded from a separate number area.

The document *Partial delivery* is created by using the copy function. You can see the original order quantity, the quantities already shipped and the quantities ordered.

The delivery date for the partial delivery can be defined in the same way as the delivery date for the original order. Apart from the delivery date for the partial delivery, you can also amend the delivery date for the original order.

You can also define in the company data that the date defined in the order shall be used by default.

**Fig. C-138: Company data – Parameters tab**
*UI screenshot showing company data parameters with options "Do not delete partial shipment item" and "Adopt partial delivery date from original order" checked.*

You can furthermore define whether the partially delivered quantities should be deleted from the original order.

### Overview Partial Deliveries
You can display all partial deliveries for an order in the list of partial deliveries. It shows the items and quantities shipped, and the partial deliveries for which partial invoices have been issued.

**Fig. C-139: List of partial deliveries for an order**
*UI screenshot showing an overview of partial deliveries for a specific order. The view lists original quantities, partially delivered quantities, and item quantities.*

- **A** Original quantities
- **B** Quantity of partial delivery
- **C** Partial delivery
- **D** Total quantities of original order

The values for quantities shipped (B) and, if applicable, the amount of the partial invoice are displayed per partial delivery. The totals of the partially shipped quantities and partial invoices are displayed for the original order (D).

### Invoice
If partial deliveries must not be invoiced, the order will be locked for invoicing until the last partial delivery has been created. A lock code must be set in the master data for this purpose. This lock code must also be entered in the company data.

**Fig. C-140: Company data - Documents tab**
*UI screenshot showing the 'Lock Codes' section in company data, with a specific code set for 'Partial delivery'.*

If you have arranged partial shipment(s) with a customer, you can decide for every individual order whether a partial invoice shall be issued for a partial delivery, or whether the overall invoice shall be issued together with the last shipment.

Partial deliveries are accompanied by delivery notes. If, in addition to partial deliveries, partial invoices are permitted, completely delivered items can be deleted from the original order.

**Fig. C-141: Company data – Parameters tab**
*UI screenshot showing company data parameters with the "Do not delete partial shipment item" checkbox enabled.*

The last delivery note only shows the remaining items and quantities.

### Partial Invoice
A partial invoice is printed from the document *Partial delivery (print item)*.

Calculation of the shipping fee is disabled for partial deliveries by default. This option can be enabled in the dialog *Copy Document*.

**Fig. C-142: Copy document - Options menu**
*UI screenshot of the Options menu showing general settings, including a checkbox for "No delivery fee for partial deliveries".*

The data *Customer, Route* and *Shipping date* are used to calculate the shipping fee. If a customer gets two shipments on the same day for instance, the shipping fee will be charged for both. This also applies for invoices that are part of a collective invoice.

If you have defined that the items of the partial delivery shall be deleted from the order upon partial invoicing, the final invoice only lists the last shipped items.

### Enter a Partial Delivery
This training module shows you how to enter a partial delivery for an order.
If partial invoicing is not permitted for an order, the original order will be invoiced only after the last partial delivery has been made. A lock code can be set in the master data for this purpose.

**■ How to enter a partial delivery**
1. Open the order for which you want to enter a partial shipment.
2. If necessary, change to the Supplements tab and check whether the checkbox *Partial delivery* has been ticked.
   
   *UI snippet showing checkboxes for "Partial delivery" and "Partial invoice" are ticked.*

   If a partial invoice shall be issued at the same time, please also tick the checkbox *Partial invoice*.
3. Select the menu `Functions > Document group > Partial delivery`.
   The dialog *Copy documents* opens in the mode *Partial delivery*. Only the fields relevant for partial deliveries are enabled.
4. Go to the tab *Copy by item*.
5. Change the quantity of the item for which you want to enter the partial delivery in the column *Target quantity (New)*.

   **Fig. C-143: Create partial delivery**
   *UI screenshot of the 'Copy by item' tab for creating a partial delivery. It shows columns for the original item quantity, partially delivered quantity, and remaining quantity.*
   - **A** Total item quantity
   - **B** Partial deliveries in total
   - **C** Quantity already partially delivered
   - **D** Remaining quantity in the original order

   **Fig. C-144: Enter quantity of partial shipment**
   *UI screenshot showing quantities being entered in the 'Target quantity (New)' column for specific items to be partially shipped.*
   
   Once you have made an entry, the item will be ticked.

6. Repeat step 5 for all items for which you want to define a partial quantity.
7. Go to the tab *Further options - Target document* to edit the dates. Check the date for the partial delivery and adjust it if necessary.

   **Fig. C-145: Enter dates for the partial delivery**
   *UI screenshot of the 'Further options - target document' tab, showing fields for setting the delivery date, shipping date, and delivery address.*
   
   If several shipping addresses have been entered in the customer master data, these will be listed. A selected shipping address can be adopted by means of the 'arrow up' key.
8. Go to the menu `Start > Execute` to create the partial delivery.

   **Fig. C-146: Partial delivery created**
   *UI screenshot showing the completed partial delivery. The new partial delivery document number is displayed in the 'Target' section.*

   The items will be checked and copied. The partial delivery is saved. The number of the partial delivery is shown in the section Target.
   The items are listed with the same item numbers as in the original order.
9. Close the dialog.
   The dialog Document management reopens. The document list shows the new document, marked by an arrow in the line header.

   **Fig. C-147: Partial delivery**
   *UI screenshot of the main document management screen, showing the original order and the newly created partial delivery document listed below it.*
   
   > Dates and shipping address can also be amended in the new partial delivery if required.
   > You can display all partial shipments for an order in the list of partial deliveries.

**Open partial delivery as a document**
To search for partial deliveries, restrict the search in the field *Type* to partial deliveries.

### Create Partial Deliveries with Reference to Completion Report/Goods Receipt or Rack
In this unit you will learn how to create a partial delivery. You can enter the partial delivery for items reported complete or racks that are assigned to the order.

> **Prerequisites**
> Status management and status allocation must be set up appropriately in the master data. The registration point assignment must be set up appropriately in the company data.
> Should you have questions about this, please contact your service employee at A+W Software GmbH.

This includes the following training sessions:
- "How to create a partial delivery per completed report or goods receipt" on page C-263
- "How to create a partial delivery per rack" on page C-265

#### How to create a partial delivery per completed report or goods receipt
1. Select `Documents > Order > Partial delivery`.
   The *Partial delivery* dialog opens. The *Per completion report/goods receipt* tab is open.
2. Select in the menu `Start > Filter` to switch to the search mode.

   **Fig. C-148: Entering partial quantities per completion report/goods receipt - selecting a number manager**
   *UI screenshot of the 'Per completion report/goods receipt' tab, showing a selection area for the Number Manager (A) and a list of documents.*

3. On the combo box (A) in which the documents with the report from production are located.
4. To do this, select `Start > Search` to start the search.
   In the Documents area, all orders from the selected number manager are displayed.
   
   > **Prerequisite**
   > A partial delivery can only be triggered for order items that are reported as *Complete*. The percentage of the items reported complete is displayed in the *Produced %* column.

5. Mark the order (A) for which you want to trigger a partial delivery.
   In the *Items* area, all order items for the marked order are displayed.
6. Mark the order item (C) for which you want to trigger a partial delivery.
7. In the *Ready for part. Del. %* field (B), enter the desired quantity for the partial delivery.

   **Fig. C-149: Entering partial deliveries per completion report/goods receipt - selecting an order item**
   *UI screenshot showing an order (A) selected, an item within that order (C) selected, and a quantity being entered for partial delivery (B).*

8. From the start menu, select `Start > Execute` to trigger the partial delivery.
   A new document with new order number and reference to the original order is created for the partial delivery.
   The query to start the delivery note printing is displayed:
   - Select [Yes] if you want to print the delivery note. The *Print form/label* dialog opens. (See "Print" on page C-186)
   - Select [No] if you want to print the delivery note later. Delivery note printing can be started at any time via the *Print* menu.

#### How to create a partial delivery per rack
1. Select `Documents > Order > Partial delivery`. The *Partial delivery* dialog opens.
2. Change to the *Per rack* tab.

   **Fig. C-150: Selection of the search criteria for orders with rack**
   *UI screenshot of the 'Per rack' tab, showing selection criteria fields for Number manager/customer (A), delivery date/status (B), and a list area for orders on racks (C).*

3. In the *Selection* area, select the desired option:
    - **Number manager:** All orders of the member manager are displayed that are booked to a rack.
    - **Customer:** All orders of one or several customers are displayed that are booked to a rack.
    
    The selection can also be restricted:
    - **Delivery date:** All orders of the selected delivery date or delivery period are displayed that are booked to a rack.
    - **Order status:** All orders with the selected number status or number status range are displayed that are booked to a rack.

4. Select `Start > Search` from the menu to start the search.
   In the *Rack - orders* area, all production jobs are displayed that correspond to the filter conditions. In the *Rack - items* area, all order items of the marked order are displayed that are booked to the corresponding rack.

   **Fig. C-151: Create partial delivery per rack – order overview**
   *UI screenshot showing a list of orders on a specific rack, with corresponding items displayed below.*
   
   > **Prerequisite**
   > A partial delivery can only be triggered for order items that are reported as *Complete* by production and booked to a rack. The percentage of items reported complete on the rack is displayed in the *Qty (on rack)* column.

5. Mark the order on the rack for which you want to trigger a partial delivery. You can also mark orders on several racks.
   Double-click on the corresponding line header. Only the orders are marked that are identified with a red X.

   > **Partial delivery per rack**
   > The partial delivery is triggered per rack. If you mark an order on a rack to which additional orders are booked, these are also marked.

   **Fig. C-152: Create partial delivery per rack – order overview with marked orders**
   *UI screenshot showing orders on a rack marked with a red 'X' to be included in the partial delivery.*

6. Select in the menu `Start > Execute` to create the partial delivery.
   The query to start the delivery note printing is displayed:
   - Select [Yes] if you want to print the delivery note. The *Print form/label* dialog opens. (See "Print" on page C-186)
   - Select [No] if you want to print the delivery note later. Delivery note printing can be started at any time via the *Print* menu.

### Exercises

**Create partial delivery**
Open the order with 3 items and create a partial delivery consisting of the following items:
- Copy item 1 completely.
- Adopt half of the defined quantity for item 2.

**Create partial deliveries with reference to completion report/ goods receipt or rack**
Open the *Partial deliveries* dialog.
- Trigger a partial delivery for two items of an order.
- Trigger a partial delivery for a rack.

**Additional Information**
- "Copy order item" on page C-131
- "Lock Code" on page C-223
- Software Reference, “Invoice" on page C-422
- Software Reference, "Partial Deliveries" on page C-611
- Master Data, "Number Ranges" on page B-890
- Master Data, "Lock Code" on page B-897
- Master Data, "Do not delete partial delivery item" on page B-935
- Master Data, "Adopt partial delivery date from original order" on page B-935

## Down Payments

### Objectives
- Entering down payment as an invoice.
- Entering down payment as an order item.

### Benefits
- You can enter different down payments, with or without invoices.
- You can enter the down payment for a customer with whom prepayment has been agreed.

### Note

**Down payment**
Down payments are entered in A+W Business in the following circumstances:
- Down payment for part of the order total
- Prepayment
The down payment results in a down payment item or a down payment invoice.

**Down payment product**
A down payment must be defined as a product in the master data.

**Down payment item**
The down payment item is saved in the order and is only invoiced with the final invoice.

**Down payment invoice**
An order of the type down payment is created for a down payment invoice. This order can be invoiced.

**Document**
A separate number area is used for down payment invoices.
Down payment invoices can be created in various ways:
- by copying an order
- by entering a new document

**Default settings**
Master data:
- Number areas
- Product Down payment for down payment item
- Product allocation surcharges (down payment) (optional)

### Invoiced Down Payment
Production of an order may be based on a down payment. There are two methods of entering and booking these down payments:
- Down payment invoice
- Down payment item (This type of down payment is described in the next module).

Down payments can be entered as down payment invoices and automatically transferred to financial accounting, archives and statistics. If prepayment has been defined for a customer or a single order, a down payment invoice will be issued for the order total.

The document *Down payment invoice* is created by means of the copy function. It will automatically receive its own document number, which originates from the partial shipment number area. Further down payment invoices can be created until the final invoice for this order is issued. Every down payment invoice will receive its own invoice number.

In the original order, the down payment amount is shown as a negative item, automatically reducing the total and the VAT by the down payment amount.

The down payment amount is booked to a separate proceeds account, *Down payment*. In statistics, this amount is booked to the allocated product group *Down payment*. Only when the original order is transferred to financial accounting and statistics are the proceeds account and product group credited with the down payment. The original document is booked to the regular accounts and product groups. This ensures that all accounts in statistics and in financial accounting are duly booked.

The final invoice is created from the original order. After the individual items, the order form shows the order total, net amount, VAT and gross amount. After that, all down payment invoices are listed with their individual amounts, i.e. net amount, VAT and gross amount. The last line shows the remaining invoice amount.

**Down payment invoice**
Prior to creating the document *Down payment*, define whether the items should be listed on the down payment invoice.

*UI screenshot of the Options menu with the 'Down payment invoice with items' option highlighted.*

If the original items should not be listed, then only the *Down payment* item is included on the down payment invoice.

### Down Payment as an Order Item
You can enter a down payment in the current order. The entered amount will not be transferred to FinAcc however but will be listed like an item. The order total will not be reduced by the down payment amount.

> The down payment amount will only be booked when an invoice is issued based on the order.
>
> **Down payment - a product**
> To enter a down payment item, *Down payment* must be defined as a product in the master data.

### List of Down Payments
All down payment invoices for an order are listed.

**Fig. C-153: List of down payments for an order**
*UI screenshot showing a list of down payments for an order, with columns for the down payment invoice number (A) and the down payment item (B).*

Both the invoiced down payments (down payment invoices) and the down payment items are shown on the down payment list.

### Enter Down Payment
This module shows you how to enter down payments. The following instructions exist for this training module:
- "How to enter a down payment with invoicing" on page C-273
- "How to enter a down payment without invoicing" on page C-275

#### How to enter a down payment with invoicing
1. Open the order for which you want to enter a down payment.
2. Select the menu `Functions > Document > Down payments`.
   The dialog *Copy documents* opens in the mode *Down payment*. Only the fields relevant for down payments will be enabled.
   
   **Fig. C-154: Create a down payment invoice**
   *UI screenshot of the 'Copy documents' dialog in 'Down payment' mode. It highlights the down payment amount field (A) and the 'Down paym' mode option (B).*

3. Make sure that the *Down payment* mode (B) is active.
4. Check in the menu `Options > Down payment amount` whether the amount is to be entered as a gross, net or proportional amount.
5. Use the menu `Options` to define whether the down payment invoice shall show items.

   *UI screenshot of the Options menu showing 'Down payment invoice with items' selected.*

6. Enter the down payment amount (A).
   If you have agreed on prepayment, you have to enter the order total.
7. Go to the tab *Text* if you want to add a note on the down payment.
8. To start the activity, go to the menu `Start > Execute`.
   The document *Down payment* is created.
9. Close the dialog.
   The dialog *Document management* reopens. The document list shows the new document, marked by an arrow in the line header.

   **Fig. C-155: Down payment invoice**
   *UI screenshot of the Document Management screen showing the newly created down payment invoice document.*

> The tab *Totals* in the down payment invoice shows the amount of the down payment.
> The order history shows the down payment invoice number as a reference.
> You can display all down payments for an order in the list of down payments.
>
> ⇨ Software Reference, "List of Down Payments" on page C-556

**Open down payment as a document**
To search for down payments, restrict the search in the field *Type* to *down payments*.

#### How to enter a down payment without invoicing
1. Open the order for which you want to enter a down payment.
   ⇨ "Search for order" on page C-50
2. Go to the tab *Totals* and select the field *Deposit amount* in the section *Total value*.

   **Fig. C-156: Payment management**
   *UI screenshot of the 'Payment management' dialog. It highlights the Payment date (A), Type of payment (B), and Amount/currency (C).*

   - **A** Date when the down payment was received
   - **B** Select the type of payment
   - **C** Amount and currency

3. Check the date (A).
   Shows the current date.
