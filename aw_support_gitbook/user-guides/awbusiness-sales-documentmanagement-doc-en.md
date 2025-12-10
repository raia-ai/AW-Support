---
description: "EN_AWBusiness_Sales_4_1-2"
---


# Comprehensive Document Entry up to the Invoicing Stage

**Tutorial**

In this thematic block you will learn how to enter and amend orders and order items.

---
## Documents and Subsequent Documents

### Objectives
*   Getting to know the document concept.
*   Allocating subsequent documents.
*   Getting to know the number manager concept.
*   Tracking the document status and history.

### Benefits
*   These documents reflect the commercial processes of your business.
*   All sales transactions are handled via document management in A+W Business. A document can be used as a basis for subsequent documents. No need to enter the order data all over again each time.

### Please note:

**Document**
All documents are entered and edited in the Document management dialog. Document management incorporates the master data in the commercial process and creates data for sales, purchasing and production.

**Document type**
Documents are distinguished by type:
*   Quotation
*   Order
*   P.O.
*   Supplier inquiry
*   Credit note

**Order**
Document type Order again includes different document types:
*   Down payment
*   Partial delivery
*   Complaint

---

### Please note:

**Subsequent documents from order**
The following documents can be created from the document type Order by selecting the print mode:
*   Order confirmation
*   Delivery note
*   Work order
*   Invoice

**History**
Any editing of a document will be saved in a history. This way, you can trace changes to a document back to its original creation. This history also displays the status changes that have been made manually or via number managers.

**Status**
Every document is allocated a status within the process, which defines where the document is located and the next step that can or has to follow.
This sequence can be defined in the status allocation by the following entries:
*   User status
*   Minimum status
*   Lock status

**Document header**
The document header is used for entering general data:
*   Data referring to the customer are, for example, the name, invoicing address and the shipping address.
*   Data for managing the order in A+W Business, e. g. delivery and production dates, order areas, business type, priority, number areas, lock codes, document type, categories.

**Item**
All products defined in the master data can be entered as order items and modified if required.

**Default settings**
*   **Master data:**
    *   Customer data (market partners)
    *   Products
    *   Prices
    *   Order (status management, status allocations)
    *   Forms
*   **Company data:**
    *   Parameters tab
    *   Pricing tab
    *   Print tab

---

## Order
Orders are the basis for the following processes. They serve e. g. to issue purchase orders, print delivery notes and invoices, and issue complaints.
Orders comprise the information from the master data, completed by details on the order items such as sizes and quantities. The entire sales process up to the invoice is based on the details in an order.
The order number is automatically loaded from the assigned number area. Number areas can be set up by client, user, and order area. If you have defined several number areas for orders, you should authorize a number area check.
Orders can be issued from quotations, using the copy function. This means that the order items do not have to be reentered.

## Subsequent documents
Orders are the basis for the following processes. They are used to create subsequent documents:
*   Order confirmation
*   Production documents
*   Purchase orders
*   Delivery notes
*   Invoices
*   Complaints
*   Credit notes

## Number area
Number areas are logical organizational units which have been introduced in the training on master data. This subject is therefore just summed up at this point.

You can and should amend the number areas as necessary for your company's needs. This is especially true for the following areas:
*   Document numbers
*   Production
*   FinAcc

The document number is automatically assigned from the allocated number area when you create a document. The number areas must not overlap to make sure that these numbers are unique.

The number areas for the documents can be defined by client and by order management (OM area). This allows you to allocate a document by means of its number.

Within these document number areas, special number areas can be defined per user:
*   Different number areas for users

---

*   Different number areas by OM areas. The users in charge can then select the corresponding number area.

Individual number areas can be locked. This way you can define that certain documents cannot be included in special areas.

> **Example**
> It is not permitted to enter orders for the tempered glass production area. You can lock the numbers for orders in this area by entering 0 for from and to, and 1 for current. This prevents the input of orders because the number 1 cannot be raised.

### Examples for number areas in the different OM areas

**Tab. C-1: Examples of number areas**

| Documents | Tempered glass production | | | Laminated glass production | | | <n.e.> | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| | **from** | **current** | **to** | **from** | **current** | **to** | **from** | **current** | **to** |
| Quotation | 300 | 300 | 19,999 | 20,000 | 20,000 | 39,999 | 0 | 1 | 0 |
| Orders | 100,000 | 100,000 | 199,999 | 200,000 | 200,000 | 299,999 | 0 | 1 | 0 |
| Purchase orders | 300,000 | 350,000 | 399,999 | 400,000 | 400,000 | 499,999 | 0 | 1 | 0 |
| Supplier inquiries | 500,000 | 500,000 | 599,999 | 600,000 | 600,000 | 699,999 | 0 | 1 | 0 |
| Invoices | 700,000 | 700,000 | 799,999 | 800,000 | 800,000 | 899,999 | 0 | 1 | 0 |
| Credit notes | 100 | 100 | 199 | 200 | 200 | 299 | 0 | 1 | 0 |
| Delivery notes | 40,000 | 40,000 | 49,999 | 50,000 | 50,000 | 99,999 | 0 | 1 | 0 |
| **Production** | | | | | | | | | |
| AWPOOL sequential number | 0 | 1 | 0 | 0 | 1 | 0 | 1 | 1 | 9,999 |
| Partial delivery | 2,000,000 | 2,000,000 | 2,099,999 | 3,000,000 | 3,000,000 | 3,099,999 | 0 | 1 | 0 |
| Complaint when breakage | 2,100,000 | 2,100,000 | 2,199,999 | 3,100,000 | 3,100,000 | 3,199,999 | 0 | 1 | 0 |
| **FinAcc** | | | | | | | | | |
| FinAcc sequential number | 0 | 1 | 0 | 0 | 1 | 0 | 1 | 1 | 99,999,999 |

In this example, all documents are entered in the OM area tempered or laminated glass production. As the OM area `<n.e.>` exists by default in A+W Business, but no orders shall be entered in this area, it is locked by entering 0, 1, 0 whereby 1 marks a blank document.

---

*   The AWPOOL sequential number shall be assigned consecutively regardless of the OM area. In this case, all OM areas are locked, except the standard OM area `<n.e.>`.
*   While in order area tempered glass production the number area for the document Order ranges from 100,000 to 199,999, the numbers 2,000,000 to 2,099,999 have been reserved for partial shipments, and 2,100,000 to 2,199,999 for complaints. Overlapping is therefore prevented.

## Interfaces
Order data is transferred to stock, purchasing, capacity planning (optional), and production for further processing.

In connection with an order, you can also e.g. calculate the production cost as well as sales commissions.

For detailed descriptions of these topics, please refer to the following documentation:
*   Stock management section
*   Purchasing section
*   Production section
*   Capacity planning section

In connection with a financial accounting program (FinAcc), receivables as well as the credit limit can be checked.

## Production
If transfer to capacity planning is active, the corresponding item data will be booked into capacity planning when data is transferred to production, before they are actually transferred to production.

Automatic data transfer must be enabled in the interface service in the master data. In the interface service you can also define the interval for running a search for orders with a status equal to/higher than the minimum status of transfer to production, but lower than the status for transfer to production.

> **Workflow for data transfer**
> In A+W Business, data transfer will only be implemented as a workflow task. The workflow task uses a special formula to search for orders, the status of which permits the transfer, e. g. to production.
> Please contact a member of the A+W Software GmbH service team if you intend to implement a workflow task.

The section Master data provides a list of parameters which are transferred to A+W Production for production purposes.

If you are using the functions of the A+W CAD Designer (Shapes), an SN file can be automatically created for every item transferred to production. This file is created for rectangles and standard shapes and also includes the data for the following processing steps:
*   Edges
*   Cut-off corners

---

*   Notched corners
*   Rounded corners
*   Edge notches
*   Drill holes

This allows you to print true-to-scale sketches on work orders.

## Lock codes
Lock codes can be used to control the transfer of a document when it has reached a certain status. You can use lock codes to lock documents for certain actions.

A lock code makes sense for partial shipments without partial invoicing because these partial shipment orders must not be invoiced. The lock code locks the document Partial shipment for the status Print invoice, and automatically passes it on to status FinAcc transfer.

You can enter the lock code for partial shipments in the company master data. It will then be applied to all corresponding documents.

Complaints or exceeded credit limits are usually connected with a lock status as well.

A separate module deals with this subject in more detail:
> **Note:** See "Lock Code" on page C-223

---

## Invoice
Generally, an invoice will be issued after shipment. Invoicing is based on the delivery and payment terms agreed for the order. You can issue partial, collective, or monthly invoices. Moreover, down payment invoices can be issued.

The legal parts of the invoice are normally adopted from the customer data and the order. You can however enter an alternative invoicing address in the order. Due dates and the cash discount calculation type are also adopted from the customer data and can be changed for individual orders.

Every invoice will get its own invoice number. The order number serves as a reference.

In addition to the order items, the invoice shows the surcharges and special discounts, the total, and - if applicable - down payments or partial invoices.

An invoiced order (invoice) is not meant to be edited any further. A lock status is therefore allocated to the status Invoice. Should amendments still be necessary, e. g. of the prices, these can only be made by means of a credit note or an additional invoice.

> **Partial invoice**
> An invoice is not a separate (saved) document but a print item. Likewise, a partial invoice is based on the printing of a partial delivery.

### Monthly invoice
You can collect the invoices for a customer and send them just once a month or once every fortnight. The corresponding code has to be set in the customer data.

During daily invoicing, all orders of customers with monthly invoices are automatically assigned the status Monthly invoice. These orders can be selected later by means of this status, to be invoiced at the desired date.

Invoices are printed separately on the invoice form including their individual invoice number.

### Printing of collective invoices
Invoices can be printed collectively. The corresponding code has to be set in the customer data.

Since collective invoices always include minor rounding differences, these will be balanced in the last order. To make sure that the system recognizes such an order, a flag is set when the collective invoice is printed so that the VAT is not automatically recalculated should the order be changed.

To make sure that all of a customer's orders are included in the collective invoice, these invoices have to originate from the same number manager and have to have consecutive numbers. The invoices will be checked before printing, e. g. customer number, collective invoice printing code in the order. If a collective delivery note is to be printed, the shipping address will be checked as well.

A collective invoice (or collective delivery note) can only be printed if the following characteristics are identical:

---

*   Customer number
*   Code 'print collective invoice' in the order
*   Payment terms and due date
*   Currency
*   VAT code 1 and 2
*   Automatic surcharges: Invoicing surcharge
*   Order area (if delivery note number by order area has been activated)
*   Invoice address (name 1)
*   Shipping address (for collective delivery notes per shipping address)

The collective invoice will be printed with one (individual) invoice number, listing the individual orders and order totals. The same applies to the collective delivery note.

### Payment plan
The payment term is calculated from the defined details when the invoice is printed. This will be omitted if the document shows a due date.
The due date of an invoice can be defined per order. The date is preset from the payment plan defined in the customer data.

### Tax
The VAT will be checked when the invoice is printed. It will be corrected only for collective invoices if necessary.
> **Note:** See "Printing of collective invoices" on page C-32

Generally, the VAT is calculated from the order total. It can however be calculated by item if required by the country's tax laws. If this option is set, the tax is shown separately for explicit BOM components. The item tax is calculated from the total BOM tax and share of the main item.

The total tax results from adding up the tax amounts per item. The total tax amount will be transferred to financial accounting (FinAcc).

## Document management
Input is quick and easy and is designed so it can be done during a telephone conversation with the customer. Every document differentiates between the header and the item data.
*   **Document header:**
    The header is valid for the entire order. It consists of those parts of the order that never or rarely change for the customer, e. g. customer number, invoicing address, terms. It also shows the totals per order.

---

*(Image: Screenshot of the Order Header dialog in A+W Business, showing fields for customer identification, address, dates, and other header-level data.)*

**Fig. C-3: Order header**
*   **A**: Document header
*   **B**: Items
*   **C**: Totals

For a detailed description of this dialog, please refer to the Order module:
> **Note:** See "Document management dialog" on page C-39
> **Note:** See "Order data" on page C-42

*   **Order item:**
    Item data are the variable part of a document. Apart from products, prices, sizes, and quantities, they provide information for production and purchasing.

---

*(Image: Screenshot of the Order Items dialog, showing a Bill of Materials (BOM) on the left and a list of order items on the right, with details like product, quantity, dimensions, and price.)*

**Fig. C-4: Order items**
*   **A**: Components of the BOM
*   **B**: List of order items

For a detailed description of this dialog, please refer to the Order items module:
> **Note:** See "Order Items" on page C-57
> **Note:** See "Controls in the item entry" on page C-59

The data for the order header and for products and prices are loaded from the master data. They are completed for the individual items by further details such as quantities and sizes.

If all product variants have been defined in the master data, order items can be entered quickly and safely. A+W Business leaves enough space for defining the products according to the customer's requirements. Data is adopted from the master data for an order and can be changed, if necessary.

After saving and closing the item entry, the Totals tab is displayed in which you can check the current order totals and the credit limit.

---

## Manual changes
Prices, discounts, minimum quantities, etc. can be changed manually in document management. Any amended entry is displayed in red.

By means of a menu function, all settings in the dialogs can be reset to the master data settings.

An order can be corrected until it has reached the lock status. Once the document is locked, it can no longer be edited.

Necessary corrections are entered in the same dialogs that were used at input. Corrected entries will be displayed immediately and prices will be recalculated if necessary.

## Automatic check for documents entered twice
A+W Business automatically checks - when the document is entered or edited - whether there is another document including the same product, product structure and sizes.

For this purpose, the user status `Duplicate existing` must be defined in the status management. The criteria for searching for duplicates must be entered in the Utilities module.

Quotations and orders in the main database for example are checked for identical product structures. Archives will not be searched. Should the program find a duplicate, the freshly entered document will be automatically locked and a message to that extent will be issued. Use the function `Show duplicates` to display duplicates of the present document.

Duplicate checks will not be run for complaints, partial shipments and down payments.

A separate module deals with this function in more detail.
> **Note:** See "New Order based on Copying" on page C-241

---

## Reference documents
For every document, you can display a list of reference documents:
*   **List of alternative quotations:**
    Lists all alternative quotations for an order. Tick an alternative to show the details.
*   **Down payment list:**
    Shows all down payment invoices for an order. The amounts are listed per down payment.
*   **List of partial shipments:**
    All partial shipments for the order will be listed. The values for quantities shipped and - if applicable - the amount of the partial invoice are displayed per partial shipment. The total of the partially shipped quantities and partial invoices are displayed for the original order.
*   **List of complaints:**
    Shows a list of all complaints related to this order. Quantities, gross unit prices, discounts and total amount per complaint are displayed.
*   **Production overview:**
    Shows the current status for each item based on production reports. Quantities will be taken into account as well.

## Additional information in the Master Data section
> **Note:** See Master Data, "Credit Limit Analysis" on page B-94
> **Note:** See Master Data, "Document parameters" on page B-767
> **Note:** See Master Data, "Partner Management - Finances" on page B-773
> **Note:** See Master Data, "Partner Management – Balance" on page B-778
> **Note:** See Master Data, "Number Ranges" on page B-890
> **Note:** See Master Data, "Lock Code" on page B-897
> **Note:** See Master Data, "Company Data" on page B-917

---

# Order Header

### Objectives
*   Getting to know the Document management dialog.
*   Getting familiar with the scheduling process.
*   Entering and editing the order header.
*   Adding text on special agreements as an attachment or footer.

### Benefits
*   Once you have entered the document header, you can proceed with the order items. You must be familiar with the main elements and reports/messages in the order header for this purpose.
*   To edit the shipping data safely, you have to be aware of the effects of date changes.

### Please note:

**Dialog structure**
Document management is the same for all document types.

**Save document**
You can only enter an item if the document header has been filled out and saved.

**Customer master data**
Input of the order header requires that the customer's data has been defined in the master data.

**Recurring orders**
You can copy documents with identical or similar items, and edit both the header data and the items in the new document.

**Default settings**
Company data:
*   Documents tab
*   Parameters tab
*   System tab

---

## Document management dialog
This module introduces you to the control elements in document management. Document management (header data) offers the following elements:

*(Image: Screenshot of the A+W Business Document Management dialog, annotated with letters A through L pointing to different interface elements.)*

**Fig. C-5: Document management - Header data**

*   **A**: Document type
*   **B**: Number of the document
*   **C**: Customer's name
*   **D**: Tab for additional entries
*   **E**: Header
*   **F**: Document header tab
*   **G**: Items tab
*   **H**: Totals tab
*   **I**: List of documents in the current number manager
*   **J**: Document status
*   **K**: Dispatch mode for:
    *   Order confirmation (OC)
    *   Quotation (Q)
    *   Invoice (In)
    *   Credit note (Cr)
*   **L**: Current number manager

Enter the document header in Document management. The screenshot shows the main elements of the Document tab. The details and all other tabs are described in detail in the Software Reference which is accessible in A+W Business via the online help function `<F1>` too.

---

### Controls in the document header
Use the Options menu in the dialogs to select settings to adapt the dialogs to the requirements of your business processes. The main controls and settings are listed in brief.

The general menus and buttons of the A+W Business dialog have already been introduced in the training session on the Master data module.

### Input via mouse or keyboard
Several options are available for data input. This training document describes the operating steps by using a mouse.

Input of data by means of the number pad on your keyboard will not be described separately. The individual fields are also accessible via the `<Tab>` key and function keys.

You can also use the hot keys in the pull-down menus, e.g. in `Functions > Documents` the key combination `<Ctrl+T>` to open the `List of partial shipments` dialog. Hot keys are available in all menus in which they are displayed. They will not be described separately.

There are different ways of accessing the input fields in the dialogs:
*   Using the mouse, position the cursor on the required field.
*   Use the `<Tab>` key to move from field to field.
*   Use `<+>` on the number pad to move from field to field.

### Open mode for document header
Two different modes are available for the dialog:
*   **Edit mode:**
    `Document management > Options menu > Documents > New input by default` is disabled. When you open the document header, the system will automatically show the document that has been edited last.
*   **New input mode:**
    `Document management > Options menu > Documents > New input by default` is active. When you open the document header, the system will automatically create a new document.

The other settings in this dialog are described in the Software Reference in the Options menu section.

---

### Buttons in search dialogs
The search dialogs show the results of the search as a table (hit list). You can adopt the documents you have selected from this list into the processing dialog.

There are various options for selecting several documents at once:
*   To select a continuous sequence of documents, select the first one and keep the `<Shift>` key pressed while marking the last document of the requested sequence.
*   To select several, individual documents, press the `<Ctrl>` key and select the required entries on the list.

**Tab. C-2: Buttons in search dialogs**

| Button | Function |
| :--- | :--- |
| *(Icon: Single document)* | Adopts only the selected line from the hit list. |
| *(Icon: Multiple documents)* | Adopts all entries from the hit list. |
| *(Icon: Deselect)* | Deselects all. |

---

## Order data
The data for the order header is loaded from the master data. This is why it is important that the master data is as complete and correct as possible.

Many of the transferred master data entries can be changed in an individual order, e.g. the shipping address in the order header or the sheets of an IG unit in the order item.

*(Image: Two small screenshots. A shows customer master data with an address. B shows an alternative shipping address entered for the specific order.)*

**Fig. C-6: Address changed in the order**
*   **A**: Customer master data
*   **B**: Shipping address in the order

The changes only apply to the current document.

You can add text or file attachments to the order to document special agreements.

Order items can be entered only after the order header has been filled out and saved. This makes sure that the prices and discounts defined for each respective customer will be used for pricing.

### Change order
After saving the order, you can further edit it and add or delete items until the invoice is printed. After that, the order is usually not edited any further.

### OM area
For order management, you can define so-called OM areas to which orders are allocated.
OM areas are defined for example for maintaining number areas per department, such as departments for tempered or laminated glass production. Interfaces are used to transfer the orders automatically to the appropriate order area for production. The OM area also serves as a sorting criterion in A+W Business turnover statistics.

---

Typically, OM areas refer to individual departments or subsidiaries of a company that generally work together. The OM area 'tempered glass production' for example is responsible for producing tempered glass.

Every OM area must be assigned its own number area so that orders can be passed on correctly.

Moreover, every employee can be allocated to an OM area and document type. The orders are then automatically entered in this OM area and the corresponding number area. Both can be changed manually in the order.

### Business type
Business types are used to define proceeds accounts and for statistics. They can be allocated to different OM areas.

### Priority
Priorities control the transfer to production. They are preset by A+W Business. If priorities are allocated to the customer or supplier in the master data, they are automatically displayed in the order where they can be changed if required.

### Document type
Documents are distinguished by type, e. g. order, purchase order, complaint. The allocated document type defines - among other things - how the document in question is to be processed further. When a document is created, the document type is set automatically and should usually not be changed. The document type `<n.e.>` is entered for an order.

### Shipping data
The shipping address is loaded from the customer data by default. You can enter an alternative shipping address in the order however.

Every shipment of an order is accompanied by a delivery note. On the one hand, it serves as a proof for the customer and on the other hand shows the status of order processing. Delivery notes can be issued individually or collectively, via a number manager.

Delivery notes are created by printing them. Every delivery note receives its own delivery note number. The order number is specified as a reference. The delivery note shows the delivery date by default. Printing the delivery note will change the order status.

> **Only partial shipment is a separate document**
> A delivery note is not a separate (saved) document but a print item. A partial shipment by contrast is a document with its own document number, because a sub-order has been created from the items of the main order.

---

## Dates
When you enter the order header, the production and shipping date will be calculated based on the delivery date. If you change the suggested shipping date, you can check if the selected date is a route day. The order can be saved even if the shipping date is not a route day.

When you enter a partial shipment, the dates of the original order will be checked. Both the date of the partial shipment and the date in the original order can be changed if necessary.

Based on the defined production and shipping dates and the requested shipping date, the system automatically calculates the dates for purchasing, production and shipping. These dates are shown on the order header.

Jeopardized shipping dates will not be corrected automatically. Use the shipping date check to redefine the dates and inform the customer of the change.

The deadlines for calculating the dates are defined in the company data.

*(Image: Screenshot showing 'Lead days' settings in Company Data for production start, production LG, and resubmission of quotations.)*
**Fig. C-7: Company data - System tab > Lead days**

### Delivery time
The delivery time is defined by customer. A route is usually completed within the day.

*(Image: Screenshot of the Delivery time per customer configuration screen, showing a list of customers with their assigned route, priority, and delivery time in days.)*
**Fig. C-8: Delivery time per customer**

---

The delivery time defined will be considered at order entry to determine the production date.

> **Example**
> *   **Shipping date**: Date on which the goods are handed over to the driver
> *   **Delivery**: Delivery date = arrival of goods at the customer's site
> *   **Delivery time**: 3 days
>
> **Tab. C-3: Delivery time**
>
> | Shipping date | Delivery time | Delivery |
> | :--- | :--- | :--- |
> | 18.05. | 19.05. -> 20.05. | 21.05. |
>
> In this example, the order must be produced and/or reported complete on 18 May.

## Credit limit
You can define a credit limit, and have it checked automatically. In connection with a financial accounting program (FinAcc) that reports the receivables, you will get a comprehensive overview of the customer's current financial status. This function is described in the Master data section.

*(Image: Screenshot showing the financial values for a customer, including credit limits, receivables, orders, and balances.)*
**Fig. C-9: Customer's credit limit**

The settings for the credit limit check are defined in the customer data.
If you do not use receivables reports, the check will include all orders that have not yet been transferred to financial accounting.

You can define the type of check:
*   No check
*   Limit 1 + Message Limit 2
*   Limit 2 + Message Limit 1
*   Check of credit limit 1
*   Check of credit limit 1+2
*   Check of credit limit 2
*   Prepayment

---

The order header shows the credit limit and the receivables. This allows you to check every individual order and discuss with the customer, if applicable, whether a new order can be accepted. In this area, data will be updated after transfer to financial accounting and after financial accounting's report.

*(Image: Screenshot showing the credit limit section within an order, displaying the customer's limits, current order total, and resulting balances.)*
**Fig. C-10: Customer's credit limit in the order**

If the credit limit is not checked, the current amounts will only be displayed. When the credit limit is exceeded and in case of prepayment, orders can generally be processed. Order entry can be locked if the credit limit is exceeded. Quotations can be entered irrespective of the credit limit and possible locks.

If the function `Individual receivables reports` is active, you can run a receivables check for the customer in question at order entry and in customer management. All open invoices will be shown.

Customers whose balance has been settled after the last receivables report will be updated in customer management with a balance of 0.

These functions depend on the settings in the financial accounting interface.

> **Check orders on hand**
> The current orders on hand can be viewed independently from order entry in the customer master data.

### Subsidiaries
If you are working with customer subsidiaries, the credit limit can be checked on two levels:
*   Checking the subsidiary's credit limit.
*   Checking the main customer's credit limit:
    *   Check via subsidiary code.
    *   Check via input in field `Main account`:
        The subsidiary's credit limit will be ignored.

Set the respective codes for the individual subsidiaries in the customer master data.

---

### Exceeding the credit limit
There are two possible reactions to exceeding a credit limit:
*   New orders can only be entered up to the point at which the limit is reached. After that, a customer is locked for further orders.
*   New orders can be entered and saved. A message points out however that the credit limit has been reached and is exceeded. It is up to the user to decide whether the order shall be processed further or rejected.

### Credit limit status
There is a separate module on the subject of Status. We therefore have to jump ahead a little below.
> **Note:** See "Status" on page C-217

The settings in the company data and the status allocation define how A+W Business is going to act in case the credit limit is exceeded:
*   A lock status is defined in status allocation beyond which further entries are impossible.
*   The status will be raised only if the option `Raise status if credit limit is exceeded` has been activated in the company master data.

If these two settings are combined, new orders cannot be entered once the credit limit is reached or exceeded.

The message `Credit limit exceeded, customer locked` also appears before the document is copied. Copying will not be executed. The credit limit will be checked even if the customer is changed in an existing order.

To process a new order even if the credit limit has been exceeded, the status has to be reduced manually. After that, the status will not be raised again automatically.

Orders can be transferred via EDI interface (electronically). If the credit limit is exceeded by a new order, it receives the status `Order locked due to credit limit`. It will be scheduled in capacity planning despite the lock status. This order has to be released manually by reducing the status. After that, it is automatically transferred to production.

> **Prepayment**
> If prepayment has been agreed for a locked customer, new orders also have to be released manually.

## Text
You can enter text for every order or order item and define whether the text shall be printed before or after the item. You can also define the text as product-related. In this case, it will be printed whenever this product is entered in an order.
At the same time, you can allocate a text code to each text or exclude the text from printing on certain forms.

---

## Enter order header
We are now going to explain how to enter a new order in which no fields are preset from a previous order.

### Entering the order header data
1.  Select `Documents > Order > Order`.
    Dialog `Document management` opens. In this description it is the **Edit mode**.
2.  Go to the menu `Functions > Document > Select NM` and check if the correct number manager has been set, and correct the setting if necessary.
    The allocation of the order to a number manager is also shown in the order header. Working with different number managers is introduced in the separate module:
    > **Note:** See "Number Manager" on page C-176
3.  Go to the menu `Start > New` to switch to the input mode.

*(Image: Screenshot of the Document Management dialog in new entry mode. The customer number field is highlighted.)*

**Fig. C-11: Customer number for new order**
*   **A**: Input field Customer Number
*   **B**: Current number manager

4.  Enter the customer number (A) and go to the next field.

---

5.  The customer data will be loaded. The input fields are enabled.
    Check the dates and correct them if necessary.
6.  Enter further details on the orders in the P.O. text fields if necessary.
7.  Check the settings for price printing and check and edit the other data.
    You will only have to go to the tab `Other address` if the shipping and/or invoicing address do not match the customer's address.
8.  Go to the menu `Start > Save` to save the data.

> The header data will be saved. Now you can go to the tab `Items`. Now enter the order items.
> The `Items` tab will be locked again if you change data in the order header. You have to save the changes to enable the `Items` tab again.

---

## Search for order
You can open any document that has been saved in the main database. To open an archived document, you will have to copy it from archives first. This function will be introduced in a separate module.
> **Note:** See "Copy Documents" on page C-240

### Searching for an order:
1.  Select `Documents > Order > Order`.
    The dialog `Document management` opens.
2.  Go to the menu `Start > Filter` to switch to the search mode.

*(Image: Screenshot of the Document Management dialog in search mode. The order number and customer number fields are highlighted, and a hit list of found documents is displayed at the bottom.)*

**Fig. C-12: Selection mode - Search for order**
*   **A**: Order number
*   **B**: Customer number
*   **C**: Found documents (hit list)

3.  Enter the order number (A) or customer number (B).
    Unless you enter a restriction for the search, the program shows all orders that have not been archived.
