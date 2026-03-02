---
description: "EN_AWBusiness_Master_Data_9_5-1"
---


# Tutorial 1: Additional Information on the Company

---
## How to restrict user rights

1.  Go to menu **Master data > Company > Employee rights**.
    Dialog **Management of rights** appears.
    In the following steps, access to an additional program item is restricted for an employee.
2.  Select menu **Edit > New**.

    [Image: Screenshot of the 'Employee Rights' dialog, highlighting fields for user selection (A) and program selection (B). Labeled fields include Identification (Group, Employee), Programme, Sub rights, and an Overview area.]
    *Fig. B-249: Fields for allocation of rights are accessible*
    *   **A**: Staff
    *   **B**: Program (dialog)

3.  Select the user (A) whose rights shall be restricted.
4.  Select the program (B) for which the rights shall be restricted, e. g. **Crystal Reports output**.
5.  Go to section **Rights** and tick the checkboxes to restrict the right as required.

    > Please note that when a checkbox is left unticked, the corresponding right will be withdrawn. If you tick e. g. the checkbox **Execute**, the user can open the dialog in question but cannot edit it.
    >
    > In this example, the user shall not be able to open the dialog. Therefore, no checkbox must be ticked.

6.  Select in the menu **Start > Save** to save the data.

    [Image: Screenshot titled 'Granting additional rights to the user', showing the 'Employee Rights' dialog after rights have been configured for a 'Trainee' for the program '1200-Crystal Reports - Ausgabe'.]
    *Fig. B-250: Granting additional rights to the user*

    The data will be saved. The user is listed in section **Overview**. In this example, no checkbox is ticked. This means that the user cannot open this dialog any longer.

7.  Select the user again to check all his rights.

    [Image: Screenshot titled 'User's rights', displaying the 'Employee Rights' dialog. The overview section shows a long list of programs and the rights associated with the selected 'Trainee'.]
    *Fig. B-251: User's rights*

In this example, the entry **Crystal Reports output** is the right which has been granted in addition to the group's rights.

## How to delete an employee's rights

1.  Go to menu **Master data > Company > Employee rights**. Dialog **Management of rights** appears.
2.  Select the employee whose rights shall be deleted.
3.  Select the right to be deleted.
4.  Go to menu **Start > Delete** and confirm the query by **[Yes]**.

The selected right is deleted from the list. The list shows all rights allocated to the employee. For all program items or dialogs that are not listed, unlimited rights apply.

> ℹ️ **Delete all rights**
> To delete all rights please go to menu **Functions > Delete rights**. All of the employee's rights will be deleted. You can also delete new employees who have not logged into the system yet.

## Exercises

*   Enter a (training) client.
*   Allocate a sales territory to an employee. Select yourself as a salesman for this exercise.
*   Define a graduated commission for this salesman, based on the turnover of your training customer and on training products.

You can perform the following exercises only if you have got administrator rights. Please remember to perform these exercises for your training client.

*   Define a group for stockkeepers.
*   Define the rights for this group so that they can only access the stock dialogs.
*   Enter a new employee, e. g. a trainee for stock management.
*   Give him the same rights as the rights for the stockkeeper group.
*   Withdraw the right to enter stock purchase orders and to set up the inventory list.
*   Log in with his login data and check in stock management whether the rights have been granted correctly.

### Additional information
*   ⇨ Software Reference, "Company Data" on page B-917
*   ⇨ Software Reference, "Field Services" on page B-1015
*   ⇨ Software Reference, "Commission" on page B-1017
*   ⇨ Software Reference, "Banks" on page B-1020
*   ⇨ Software Reference, "Subsidiaries" on page B-1022
*   ⇨ Software Reference, "Employee" on page B-1003
*   ⇨ Software Reference, "Employee Groups" on page B-1009
*   ⇨ Software Reference, "Employee Rights" on page B-1010

---

# Tutorial 2: A+W Business Documents

## Documents

Documents are the basis of the commercial processes in A+W Business. This set of topics will tell you how to test new or amended master data and how the processing of documents is controlled in A+W Business.

This includes the following training modules:

*   "Order for Testing Master Data" on page B-408
*   "Status Administration" on page B-418
*   "Number Areas" on page B-432
*   "Roundings" on page B-441

> ℹ️ **Prerequisite**
> This tutorial is based on the knowledge acquired in Tutorial 1.

## Order for Testing Master Data

### Objectives
*   Checking the interaction of master data.
*   Order entry.
*   Setting up a number manager.

### Benefits
*   You can test the new or amended master data before using them in your daily business.

### Please note
*   **Order**: An order (document) is always transferred to a number manager.
*   **Number manager**: Number managers (NM) help organizing the processes in your daily business. A NM cannot be empty.
*   **Hierarchy of terms**: Calculation or orders (or purchase orders) takes the terms into account in the following sequence:
    *   Details from the document
    *   Definitions from master data
    *   Group-specific terms

### Interaction of Master Data in an Order
You have entered or edited the data for partners, products, prices, surcharges, and discounts. These data are used in the documents and form the basis for order and P.O. entry.

[Image: A simplified chart showing how various Master Data points (Route, Discounts, Customer group, Surcharges, Product type, Product class, Price) flow into a Business Type and Products, which are then integrated into a final Order document.]
*Fig. B-1: Interaction of master data in the order*

This simplified chart shows an order for a customer who orders a certain product. In addition to customer master data and product master data, further master data are integrated e. g. for pricing.

Before using the new data in your daily business you have to check whether the results of pricing and scheduling meet your expectations. The following chapters describe in brief how data are entered in dialog **Document management**.

For a complete description of order entry please refer to section Sales.

### The order header
The header is valid for the whole order. It consists of those parts of the order that never or rarely change for the customer, e. g. customer number, invoicing address, terms. It also shows the totals per order.

[Image: Screenshot of the Document management dialog, showing the order header. Labeled sections are A (Document type and number), B (Tab for the header), C (Current number manager), D (Status), and E (Tab for item data).]
*Fig. B-2: Document management dialog*
*   **A** Document type and number of the document on hand
*   **B** Tab for the header
*   **C** Current number manager
*   **D** Status (display enabled in table properties)
*   **E** Tab for item data

This brief example shows an order with the header for customer and shipping data. Tab **Items** can be accessed only after the header has been saved.

### Item data
Item data are the variable part of the document. Apart from products, prices, sizes, and quantities, they provide information for production and purchasing (purchase orders).

[Image: Screenshot of the Item entry dialog, showing a detailed view of an order's items. Labeled sections are A (Title bar), B (Items list), C (Item prices), D (Item price details), and E (Details of BOM).]
*Fig. B-3: Item entry dialog*
*   **A** Title bar: Order number, number of items, total
*   **B** Items
*   **C** Item prices (red letters for manual input)
*   **D** Item price
*   **E** Details of BOM

This screenshot shows how order items are displayed. For every item, you can see the prices and discounts loaded from master data.
For a detailed description of the documents please refer to chapter Sales.

⇨ Sales, "Comprehensive document entry up to the invoicing stage" on page C-26

### Number manager for orders
Orders are organized in number managers (NM) so that they can be processed together. Every document is automatically allocated to a number manager. The number managers can be used for automating the sales processes, e.g. printing order confirmations and delivery notes.

[Image: Screenshot of the Number Manager dialog. Labeled sections are A (Current NM) and B (List of documents in the NM).]
*Fig. B-4: Number Manager*
*   **A** Current NM
*   **B** List of documents in the NM

Number managers cannot be empty. To check the master data, you have to enter an order first. It can then be moved to a new number manager.
The functions of the number managers are described in detail in section Sales.

⇨ Sales, "Number Manager" on page C-179

## Enter New Order
The following instructions show how to enter an order in which no fields are preset from a previous order.
Working with documents is described in detail in section Sales. This is why the individual steps are only described in brief at this point.
*   ⇨ Sales, "Enter order header" on page C-50
*   ⇨ Sales, "Enter Order Item" on page C-95

### How to enter an order
1.  Select menu **Documents > Order > Order**.
    The dialog **Document management** opens. If necessary, remove the presetting by clicking on **[Select]**.
2.  Go to the menu **Start > New** to switch to the input mode.

    [Image: Screenshot showing an empty new order form. Labeled sections are A (Header), B (Input field Customer Number), and C (Items tab).]
    *Fig. B-5: Fields for new order are accessible*

3.  Enter the number (B) of your (training) customer.
    If you do not know the customer number you can use the zoom function to search for the customer.
4.  Use `<Tab>` to go to the next field.
    The customer data will be loaded.
5.  Select in the menu **Start > Save** to save the data.
    The header data will be saved. The title bar (A) shows the order number, and tab **Items** is accessible.
6.  Click on tab **Items** (C).

    [Image: Screenshot of the item entry screen for a new order. The fields for entering product details are shown. Labeled points are A (Enter the product number), B (Search product), C (Quantity), D (Width), and E (Height).]
    *Fig. B-6: Fields for the new item are accessible*

    > The input field (A) for the product number is accessible. Only if you have meanwhile saved the entries or changes you have to start the input mode in menu **Edit > New** to enter a new item.

7.  Enter the number (A) of your (training) product in the input line.
    If you do not know the product number you can select the required product by means of the search (B) function.
8.  Use `<Tab>` to go to the next field.
    All input fields are enabled.
9.  In the next fields, enter the quantity (C) and the sizes (D, E).
    If you enter just 1 piece and the sizes 1000 x 1000 you can easily check whether the prices are shown correctly.

    [Image: A close-up view of the item line in the order entry screen, showing the price display. Labeled parts are A (Preisjahrgang/Price year), B (Price keys), C (Price unit), and D (Item price).]
    *Fig. B-7: Price display*

10. Check whether the rate (price key (B), price list (A)) and the price unit (C) are shown correctly.
    If no surcharges or discounts are applied to your product, the item price (D) must be correct. In this example, this is 71.38 €/sqm x 1.04 sqm (rounded size).
    When surcharges and discounts have been applied, the item price can be calculated accordingly.
11. Save the item using `<Enter>`.
    Item data will be saved and suggested as a new item in the next line. You can change the data to enter another item or ignore the data if you do not want to enter further items.
    Make a note of the order number so that you can set up a number manager for this order afterwards.
12. First close item entry, then the order.
    Set up a new number manager in which all orders entered for test purposes are going to be gathered.

## Number Manager
You should set up a special number manager (NM) for testing master data. We are going to explain the necessary steps only in brief. The use of the number manager is described in detail in section Sales.

### How to create a new number manager
1.  Select menu **Documents > Order > NM order**.
    The **Number manager** dialog opens. The list shows all documents included in the active number manager.
2.  Go to the menu **Start > New** to switch to the input mode.

    [Image: Screenshot of the Number Manager dialog in input mode. Labeled fields are A (Name of the number manager) and B (Order number).]
    *Fig. B-8: Fields for new number manager are enabled*

3.  Enter the name (A) of the new number manager, e.g. `training`.
4.  Enter the number of your test order in both fields (B).
    If you do not know the number you can search for the order by restricting the selection to status 1. In this case, all orders with status 1 will be loaded into the number manager. You can however delete the unwanted orders from the number manager by selecting them and pressing `<Del>`.
5.  Select in the menu **Start > Save** to save the data.
    The data will be saved. The new number manager appears in field **Selection**.

    [Image: Screenshot showing the newly created 'training' Number Manager with one allocated order.]
    *Fig. B-9: New number manager*

    The allocated order appears on the list.

### Exercises
*   Enter different orders - including your training products - for your training customer. Just enter one piece with a size of 1000 x 1000 mm so that you can easily check the calculation of the item price.
*   Check the following data:
    *   Have surcharges and discounts been calculated?
    *   Is marginal income and cost calculation displayed?
    *   Are the route and the delivery date correct?

---

# Status Administration

### Objectives
*   Introducing the function of the status.
*   Knowing the difference between status point and user status.
*   Checking the status allocation.
*   Define the change of status, lock status, and status diversion.

### Benefits
*   Status allocation serves to describe the business processes.
*   Status allocations define how a document can be edited after it has been entered.

### Please note
*   **Status Point**: Program point which marks the end of a process. The individual statuses are fixed and cannot be changed.
*   **User status**: State of processing the document has reached in your company. The numbers and names are set up during program installation.
*   **Status Allocation**: Every user status must be allocated to a status point. If this allocation is missing, certain functions cannot be executed.
*   **Status**: Number which marks the document's position in the program flow. Each status is unique. Every document is marked by a status.
*   **Change of status**: The status is automatically changed at the end of the program process. The status is always raised. Special user rights are required to reset the status by hand.
*   **Document type**: Not every status can be applied to every document, e. g. all documents have the status `Document entered` at one time or another but a quotation can never reach the status `Delivery note printed`.
*   **Manual status point**: Manual status points can only be allocated manually. It overrules the automatic raising of the status.

## Handling of Business Processes
Your business processes determine the stations an order passes between order entry and archiving.

> **Example**
> *   An order is entered.
> *   The order is changed.
> *   The order confirmation is printed.
> *   Orders are transferred to capacity planning (optional).
> *   Orders are transferred to production.
> *   The production status is reported.
> *   Delivery note is printed.
> *   The invoice is printed.
> *   Order is transferred to financial accounting.
> *   Order is transferred to statistics and archives.
> *   Order data are deleted from the main database.

From order entry to archiving, the order passes defined program points, the so-called **status points**. These status points can be allocated to the stations your order passes in your company. You define the minimum status, i.e. the requirements that have been met so that the order can be passed on. You can also define when an order shall be locked for certain processes.

These connections are defined in the dialogs **Status management**, **Status points**, and **Status allocation**.

> ℹ️ **Editing of dialogs**
> Dialogs **Status management** and **Status points** do not require editing. You only have to be able to edit the **status allocation**, e. g. if business processes are changed.

## Status Point (Process Name and Number)
The so-called status points are defined in the program for the automatic processing of documents. They signal the end of various, internal processes a document passes from input up to the printing of an invoice, including complaints or credit notes.

[Image: Screenshot of the Status Points dialog, showing a list of internal codes, applicable document types, and the name of the completed process.]
*Fig. B-10: Status Points*
*   **A** Internal code (status point ID)
*   **B** Document type
*   **C** Completed process

The status points are fixed in the system and are used to define conditions for further processing, e.g. for printing invoices. Every status point can be allocated to a user status per document type (B).

The user status shows the actual processing status of the document. This connection is described below.
*   ⇨ "Status Management" on page B-421
*   ⇨ "Status Allocation" on page B-422

Not every status can be applied to every document, e. g. all documents have the status `Document entered` at one time or another but a quotation can never reach the status `Delivery note printed`.

The following document types are available:
*   0 = all documents
*   1 = quotations
*   2 = order
*   3 = credit note
*   4 = inquiry
*   5 = P.O.

## Status Management
The so-called user status marks the state of processing a document has reached within your company's processes.

[Image: Screenshot of the Status Management dialog, listing user statuses with their number (A) and description (B).]
*Fig. B-11: Status management (user status)*
*   **A** Status: Code in the documents
*   **B** Description (in the business process)

The document status shows the whereabouts of the document in the business process. It is shown as a number with the corresponding description, e.g. at order entry or in the history.

> ℹ️ **Change of user status**
> Before entering or changing a user status, please discuss the matter with A+W Software GmbH. This will help to avoid system errors or incompatibilities.

## Status Allocation
Every status point can be allocated its own user status. The numbering of status points has nothing to do with the sequence of the company's workflow.

[Image: Screenshot of the Status Allocation dialog, showing the link between a Status Point and a User Status.]
*Fig. B-12: Allocation: status point – user status*
*   **A** Status Points
*   **B** Selected status point
*   **C** Document type to which the allocation applies
*   **D** Allocated user status
*   **E** Minimum status the document must have reached
*   **F** Lock status

In this example, status point **Print invoice** (B) is allocated to user status **Invoice printed** (D). This allocation applies to the document type **Order** (C). This means that when the invoice has been printed, the status of the order is shown together with the status number and status name of the user status.

### Minimum status
For every allocation you can define the minimum status a document has to have to reach the selected status point. In this example, the minimum status (E) is the printing of delivery notes. This means that the invoice cannot be printed before the delivery note.

### Lock status
For every allocation you can enter a lock status (F) to control the further process. In this example, the same user status (D) is defined which means that the invoice cannot be printed again as an original invoice.

In addition to the lock status, a lock code can be set for complaints and partial shipments.
⇨ "Lock Code" on page B-425

### Status allocation
The status is automatically raised when the document has reached a certain status point, and if the corresponding action has been triggered.

*Tab. B-1: Examples of status allocations*
| User status | Document type | Min.-status | Lock status | Status Point Process name | No. |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **001** Enter document | All | - | - | Document entered | 001 |
| **020** Document changed | All | 001 | 750 | Document changed | 002 |
| **200** Confirmation printed | Order | 001 | 200 | Print OC | 100 |
| **300** Transfer order to purchasing | Order | 180 | 540 | Transfer to order pool | 030 |
| **390** Order released for production | Order | 001 | 390 | Production release | 035 |
| **360** Receipt of goods - complete/order | Order | 030 | 360 | Receipt of goods - complete/order | 034 |
| **450** Order transferred to production | Order | 400 | - | Transfer to production | 045 |
| **600** Delivery note printed | Order | 400 | 600 | Print delivery note | 102 |
| **750** Invoice printed | Order | 600 | 750 | Print invoice | 103 |
| **800** Transfer FinAcc data | All | 750 | 800 | Transfer to FinAcc | 097 |
| **850** Transfer to statistics | All | 800 | 850 | Transfer to statistics | 500 |
| **990** Transfer to Archives | All | 850 | 900 | Transfer to Archives | 501 |
| **990** Release deletion | All | 900 | 990 | Release deletion | 502 |
| **995** Document deleted | All | 990 | - | Document deleted | 503 |

This example shows how the status of an order is changed by processing. The minimum status for transfer to purchasing is that the corresponding work order has been printed. The lock status defines that the document is locked after production and cannot be transferred again. The first column shows the sequence in which the document passes the individual processing steps.

## Manual Status Allocation
You can define that the status for special processes must be allocated by hand. A manual status point must be defined in this case. A manual status point can be allocated only by hand in a document. It overrules the automatic raising of the status.

> **Example**
> A manual status point is set e.g. if an invoice is to be printed only after a (manual) check. The status of an order has to be raised manually after the check so that the invoice can be printed.

Manual status allocation requires the following steps:
*   Enter a new status point with a number >10,000.
*   Define the user status in the business process.
*   Allocate the user status to the status point.

> ℹ️ **Definition of status points**
> If you want to define and allocate new status points you should ask a member of the A+W Software GmbH service team for help. This will help to prevent inadvertent status changes for your documents.

### Status allocation based on barcode reports
Special status points have to be defined also for reports from shop floor data collection (barcoding). In contrast to manual status points, the document status will be changed automatically when a report from the shop floor is received.

Status allocation based on barcode reports requires the same steps as manual status points. Moreover, the registration points have to be allocated.

Status changes based on barcode reports are described in section Production.

## Lock Code
Lock codes can be used to lock documents for certain actions while automatically raising their status. This means that the document cannot reach the locked status but is instead diverted to another status point (process).

> **Example: Partial shipment without invoicing**
> If no partial invoice is to be issued for a partial shipment, the status of the partial shipment is raised automatically. If the order is diverted to transfer to archives, the partial shipment cannot be edited any further.

[Image: Screenshot of the Lock Codes dialog. It shows settings for diverting a document to another status point.]
*Fig. B-13: Lock code and diversion to another status*
*   **A** Name of the lock code
*   **B** Locking the lock code
*   **C** Locked status (user status)
*   **D** Next possible status

Locking makes sense e.g. for partial shipments, namely if the partial shipments are not to be invoiced. The lock code for partial shipments (and for complaints) is enabled in company data.
⇨ Software Reference, “Company Data > Documents" on page B-928

> ℹ️ **Locking the lock code**
> Do not mix up the lock code and the lock based on the checkbox **Locked (B)**. The lock code diverts a document to another status. The checkbox Locked prevents the use of the lock code.
