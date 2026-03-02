---
description: "EN_AWBusiness_Sales_4_3-1"
---


# Comprehensive Document Entry up to the Invoicing Stage

---
## Print Labels

This section describes the process of printing labels for documents.

*(Fig. C-109: Print labels)*
The user interface for printing labels shows several sections:
- **A. Number Manager:** Field to select the number manager.
- **B. Label:** Dropdown to select the label type.
- **C. Print mode:** Options to define how labels are printed (e.g., by unit, by item).
- **D. Special print:** Checkboxes for special print options like "Repeat printout".
The bottom part of the window lists documents with details like Number, Date, Customer, Status, and Amount.

1.  Select the number manager (A) and the print mode (C).
    The section **Documents** lists all documents included in the current number manager.
2.  Select the label (B) for the current print.
    You can only choose labels matching the defined print mode.
3.  Check the output type in the section **Print as**.
4.  Tick the checkbox for the required special printout (D).
    By default, labels are not printed for glass that has not been optimized. You can enable the printout for these types of glass.
    
    > **Repeat printout**
    > Please note that you have to tick the checkbox **Repeat printout** if the document has already been printed before. It does not matter whether the first printout was done via printer or displayed on screen.
    
5.  Select the document for which you want to print labels.
6.  To start the activity, go to the menu **Start > Execute**.
    Based on your settings, the labels are sent to the printer.

## Exercises

### Print order confirmation from NM

Open your number manager with the documents of status 1 or 2.

- Print the order confirmation for the first order by displaying it on screen.
- Now try to print this order confirmation via printer. Alternatively, you can display it on screen again. Please remember that you have to start a repeat printout in both cases.
- If a printer (paper) is available: Print all order confirmations together.

### Print order confirmation from document

- Open an order and print the order confirmation using the **Start > Print** menu.
- Now print the delivery note and the invoice.

### Additional information
- Software Reference, "Printout" on page C-458
- Software Reference, "Shape / grill" on page C-505
- Master Data, "Shape sketch, Grill sketch" on page B-599
- Master Data, "Price Parameters" on page B-602
- Master Data, "Form Management" on page B-1045

## Invoices

### Objectives
- Printing invoices.
- Entering receipt of payment.
- Checking receivables and issue reminders.

### Benefits
- Complete an order by printing the invoice. Depending on the customer, you can issue individual invoices, collective invoices or monthly invoices.
- You can check whether invoices are reported as receivables by the financial accounting system.

### Note

| Term | Definition |
| :--- | :--- |
| **Invoice** | An invoice is not an independent document. It is created by printing. |
| **Due date** | Different due date calculations can be allocated for each customer. |
| **Receipt of payment** | Minor differences in the payments received can be ignored. |
| **Default settings** | Master data:<ul><li>Number areas</li></ul>Company data:<ul><li>Documents tab</li></ul> |

## Invoice Types

The following invoice types can be created and booked from orders:

- **Invoices:** The entire order is invoiced. You can also collect invoices for a customer and issue monthly invoices, for example.
- **Partial invoices:** For partial shipments, you can either issue an invoice for the entire order, or a separate invoice for each partial shipment.
- **Down payments**

Printing an invoice will raise the order status. The transfer of invoices to a financial accounting (FinAcc) program is based on this status.

### Invoice printing
Invoices are no separate documents but a print point. You can create an invoice by printing an order in **Invoice mode**.

## Due Dates

Due dates are calculated based on the document date and the following entries in partner management and the document:

- Due date calculation mode
- Accounting date (=ACD)
- Days gross (=payment term)
- Date of payment (=settlement day)

### Due date calculation
Due dates are calculated by one of the following modes:

| No. | Text | Calculation |
| :-- | :--- | :--- |
| 0 | Document date | The invoice is due immediately. |
| 1 | Document date + payment term | By default: invoice date + 30 days; further payment terms can be entered. |
| 2 | Document date + payment term rounded to the first date of payment or the month's end | If a date of payment is defined, the due date is calculated from the rounded document date + payment term. If no date of payment is defined, the date will be rounded to the month's end. |
| 3 | Document date + payment term rounded to the 15th of the month, or month's end | As 2, rounded to the 15th of the month or to the month's end. |
| 4 | Document date + payment term rounded to the 10th or the 20th of the month, or month's end | As 2, rounded to the 10th or 20th of the month, or month's end. |
| 5 | Document date + month's end + payment term | The payment term is added starting from the first day of the month following the invoice date. |
| 6 | Document date + month's end + payment term rounded to first date of payment | As 5 but rounded to the first date of payment. |
| 7 | Document date + payment term rounded to first, second, or third date of payment | As 5 but rounded to the nearest date of payment. |
| 8 | Document date + payment term based on the second date of payment, rounded to the first or third date of payment | As 5 but rounded to the first or third date of payment. |
| 11 | Due date = shipping date + payment term | Delivery date + payment term. |

This list shows how due dates are calculated.

### Reference date

The document date and the accounting date form the first reference date. This is the basis for calculating the payment term.

- **Accounting date = 0:** The first reference date equals the document date.
- **Accounting date ≠ 0:** The document date is rounded to the accounting date and forms the first reference date.

**Examples**

| Doc. date | ACD | 1st reference date | Remarks |
| :--- | :-- | :--- | :--- |
| 03/13 | 0 | 03/13 | 1st Reference date = Document date |
| 03/13 | 25 | 03/25 | The document date is rounded to the 25th of the same month. |
| 03/27 | 25 | 04/25 | Since the accounting date is less than the document date, the document date is rounded to the 25th of the following month. |

These examples show how the first reference date is calculated from the document date (invoice date) and the accounting date.

### Calculation examples

| CD | Doc. date | ACD | 1st reference date | Gross day | 2nd reference date | Date of payment 1/2/3 | Payment term |
| :-- | :--- | :-- | :--- | :--- | :--- | :--- | :--- |
| 0 | 03/13 | 0 | 03/13 | 0 | | 0 | 03/13 |
| 0 | 03/13 | 15 | 03/15 | 0 | | 0 | 03/15 |
| 100 | 03/13 | 15 | 03/15 | 30 | | 100 | 04/14 |
| 2 | 03/13 | 0 | 03/13 | 30 | 04/12 | 0 | 04/30 |
| 2 | 03/13 | 0 | 03/13 | 30 | 04/12 | 17 | 04/17 |
| 3 | 03/13 | 0 | 03/13 | 0 | | 0 | 03/15 |
| 3 | 03/17 | 0 | 03/17 | 0 | | 0 | 04/01 |
| 4 | 03/03 | 0 | 03/03 | 0 | | 0 | 03/11 |
| 4 | 03/11 | 0 | 03/11 | 0 | | 0 | 03/20 |
| 4 | 03/25 | 0 | 03/25 | 0 | | 0 | 03/31 |
| 5 | 03/13 | 100 | 03/31 | 60 | | 0 | 05/31 |
| 6 | 03/13 | 0 | 03/31 | 60 | 05/31 | 20 | 06/20 |
| 7 | 03/13 | 0 | 03/13 | 30 | 04/12 | 5 / 15 / 20 | 04/15 |
| 7 | 03/26 | 0 | 03/26 | 30 | 04/25 | 20 / 5 / 0 | 05/05 |
| 8 | 03/13 | 0 | 03/13 | 30 | 04/12 | 10 / 15 / 20 | 04/10 |
| 8 | 03/26 | 0 | 03/26 | 30 | 04/25 | 10 / 15 / 20 | 04/20 |

## Receipt of Payment

Outside a program for financial accounting, **A+W Business** allows you to enter payments received, dispatch bank statements (transfer forms) for customer invoices and dispatch reminders.

You can enter payments even if the amount received does not match the invoice amount. You can manually enter several payments per invoice. The difference between the invoice amount and payments received is displayed when a payment is received. Slight differences can be ignored; the invoice can be marked 'paid'.

The subject **Financial Accounting** is addressed in a separate module.
⇨ "Financial Accounting (FinAcc)" on page C-350

## Reminder

The **Reminders** module allows the manual booking of paid invoices (in A+W Business). The total receivables are automatically reduced by the booked amounts, taking into account the deducted discounts. These amounts can be total or partial invoice amounts including discount.

Reminders for unpaid invoices can be faxed directly to the customer, with or without a fee. The reminder fee is charged in addition to the invoice and is shown separately.

In connection with a financial accounting (FinAcc) program, you can get an overview of the receivables for every customer.

> **Data exchange with FinAcc**
> All functions in connection with FinAcc, such as reports on receivables or reminders, depend on the financial accounting program installed. The settings can be made by your A+W Software GmbH contact.

## Enter Receipt of Payment

You can enter the receipt of several payments for the same invoice. All payments received will be listed. All amounts will be automatically updated when you enter a payment.

### How to enter payments received

1.  Select the menu **Documents > Reminders**.
    *(Fig. C-110: Reminders UI shows sections for Invoice details, Effected payments, Customer details, and a list of open invoices at the bottom.)*
2.  Enter the invoice or customer number for which you want to enter the payment received.
    Start the search without defining search criteria to show all open invoices.
3.  To start the search, go to the menu **Start > Search**.
    The open invoices are imported.
4.  In the overview, select the invoice for which you would like to enter receipt of payment.
    *(Fig. C-111: Open invoices UI shows an invoice selected, with details populated in the Invoice, Customer, and Payment sections.)*
    The fields in the sections **Invoice** and **Customer** show details for the selected invoice.
5.  Select the menu **Payment > New payment**.
    *(Fig. C-112: Fields for payments received enabled. The payment section is now active for data entry.)*
    - **A:** Checkbox "Invoice is settled".
    - **B:** Field for "Amount paid".
6.  Enter the amount (B) that has been paid by the customer and the discount percentage, if applicable.
    You can also enter the paid amount if it does not equal the invoice amount, e. g. if the customer is paying in installments.
7.  If necessary, correct the payment date.
8.  Go to the menu **Start > Save** to save the data.
    The data will be saved. The section 'Effected payments' shows the new payment. If the amount paid did not settle the invoice amount, the difference will be shown in the field **Open**.
9.  Tick the checkbox **Settled (A)** if the payment received matches the invoice amount.
    In this manner, you can also conclude invoices that reflect a minor difference, e. g. due to differences in rounding.
10. Go to the menu **Start > Save** to save the changes.
    The data is saved. The settled invoice is deleted from the overview.

## Send Reminder

You can issue a reminder for every open invoice. The invoice will be automatically marked by a reminder level. The reminder level can be reset.

### Prerequisites
> Reminders can be faxed automatically provided that a fax number has been entered in the customer data, and fax dispatch is permitted for the order. The option Faxing has to be enabled in the dialog **Reminders**. The 'locked for reminders' code must not be set in the customer master data.

### How to enter a reminder

1.  Select the menu **Documents > Reminders**.
    The dialog **Reminders** opens.
2.  Enter the invoice or customer number for which you want to enter the payment received.
    Start the search without defining search criteria to show the open invoices.
3.  To start the search, go to the menu **Start > Search**.
    The fields in the sections **Invoice** and **Customer** show details for the selected invoice.
4.  Select the invoice for which you want to issue a reminder.
    *(Fig. C-113: Open invoice UI, showing details of an open invoice.)*
    The fields in the sections **Invoice** and **Customer** show details of the invoice.
5.  Select the reminder level.
    *(Fig. C-114: Send reminder for open invoice. The Reminder type is set to "Anwalt / Lawyer" and a fee is automatically populated.)*
    The field **Fee** automatically shows the appropriate fee. You can change the fee if required.
6.  Go to the menu **Start > Save** to save the data.
    The data is saved. If the option **Faxing** is active, the reminder will automatically be sent to the customer's fax number.

> **Reset reminder**
> You can remove the reminder level in the same way. To remove the reminder code from the invoice, enable the function **Reset reminder level**. Ensure that only the invoice is shown for which you want to reset the reminder level.

## Document History

### Objectives
- Understanding the document history.

### Benefits
- You can check the processing steps for a document to see who has processed it, when and in which way.

### Note

| Term | Definition |
| :--- | :--- |
| **History dialog** | You can open the document history for every document. |
| **History** | The history is kept automatically and cannot be edited. |
| **Default settings** | None. |

### Document History Dialog

The history is kept for every document, listing all manual editing steps as well as automatic status changes. The entries are made automatically and cannot be edited.

*(Fig. C-115: Document history dialog)*
The dialog shows a detailed log of all actions performed on a document. The columns include Date/time, Transaction/action, Status, Person in charge, Reference, and Comment.
- **A** Editing date and time
- **B** Current document type
- **C** Editing type
- **D** Document number and current status
- **E** Status after editing
- **F** User who has edited the document
- **G** References to other documents
- **H** Current status
- **I** Status change based on printing
- **J** Number of the P.O. created through transfer to purchasing
- **K** Printing of the job confirmation
- **L** Manual change of document (here: the price)
- **M** Customer number and balance at the time the order was created
- **N** Checkbox to change the view ("Show last action first")

The history can be opened from several dialogs, e.g. document management or one of the number managers.

## Check Document History

This training module shows you how to open the document history.

### How to check the document's editing sequence

1.  Select the order you want to check.
    You can open the history from several dialogs, e. g. document management or one of the number managers.
2.  Select the menu **Functions > History**.
    The dialog of that name opens.
3.  If required, tick the checkbox **Show last action last** to reverse the view of the sequence of entries.

## Exercises

### Check invoices
Open the **Reminders** dialog.
- View the order for which you have already printed an invoice.
- Enter a partial amount and check the remaining amount.
- Now enter the remaining amount so that the invoice is settled.

### Issue a reminder
- View all unsettled invoices for your customer.
- Issue a reminder for the customer.
- Charge a fee for this reminder.

### Check the document history
Open your order and view the history.

### Additional information
- "Status" on page C-217
- "Receivables" on page C-356
- Software Reference, "Terms / Order volume" on page C-427
- Software Reference, "History" on page C-547
- Software Reference, "Reminding" on page C-728

## Status

The processing of documents is controlled by the status. Status management and status allocation serve to show your business processes in **A+W Business**.

This thematic block describes how to define and allocate a user status, how to change the status and how to control status changes by means of user rights.

## Internal Processes and Document Status

### Objectives
- Introducing status points in A+W Business.
- Introducing the distinction between status point and user status.
- Allocating of internal processes to the processes in A+W Business.
- Linking the user status to a status point.

### Benefits
- You can allocate internal processes to your operational processes.
- Controlling the processing of documents by means of statuses prevents incorrect handling of documents.
- Status changes can be tied to a minimum status.
- A lock status prevents that documents of a certain status will be processed further.
- A status change can be tied to user rights so that only certain users can perform certain actions.

### Note

| Term | Definition |
| :--- | :--- |
| **Program sequence** | Processes running in A+W Business are called status points. |
| **Process numbers** | The process number is an internal number within the process. It is not the same as the status. |
| **Status point** | Status points in A+W Business are the internal processes and/or their numbers. |
| **Document type** | Every status point is allocated to a document type: <ul><li>0 = All documents</li><li>1 = Quotations</li><li>2 = Order</li><li>3 = Credit note</li><li>4 = Supplier inquiry</li><li>5 = P.O.</li></ul> |
| **Allocation** | Every user status must be allocated to the corresponding program point in A+W Business. |
| **Minimum status** | The minimum status is a prerequisite for a document running through a certain process in A+W Business. |
| **Lock status** | The lock status prevents further processing of a document. |
| **Exclusive status** | Allocation of an exclusive status can be tied to certain users. ⇨ "User Rights" on page C-237 |
| **Default settings** | None. |

## Status Point

So-called status points (process names and numbers) are defined in A+W Business for the automatic processing of documents. They signal the end of various internal processes that a document passes from input up to the printing of an invoice, including complaints or credit notes.

A status point is allocated to a user status which represents an operational process within your company.

The status points are fixed in the system and are used to define conditions for further processing, e.g. for printing invoices. Every status point can be allocated to a user status.

Status points referring to printing or fax dispatch are also called print items.

*(Fig. C-116: Status points UI shows a list of status points.)*
- **A. Internal process number:** The code for the process.
- **B. Document type:** The type of document the status point applies to.
- **C. Internal process name:** The descriptive name of the process.

## Status Management

First, define the stations an order passes through in your operational process. These stations are defined as user status in A+W Business. The user status marks the state of a document in the operational process of your company. It is shown as a number and with the appropriate name, e.g. in the history together with a note concerning the process.

*(Fig. C-117: Status points (management) UI shows a list of user statuses.)*
- **A. Status:** The numerical code for the user status.
- **B. User status name:** The descriptive name of the user status.

You can define any user status. It needs to be allocated to one of the processes in A+W Business to be applied to the documents.

## Status Allocation

When you have defined the status of the order in your operational process, you have created the user status. Now allocate this status to the corresponding program point in A+W Business.

*(Fig. C-118: Allocation: status point – user status)*
The UI shows a list of status points on the left and the allocation details for the selected status point on the right.
- **A. Status points:** List of all available status points.
- **B. Selected status point:** The currently selected status point for allocation.
- **C. Document type to which the allocation applies:** e.g., Order.
- **D. Allocated user status:** The user status being assigned.
- **E. Minimum status the document must have reached:** A prerequisite status.
- **F. Lock status:** A status that will lock the document from further processing.

In this example, the status point **Transfer to order pool (B)** is allocated to the user status **Transfer P.O. (D)**. This allocation applies to the document type **Order (C)**. This means that the status of the order is shown together with the status number and status name of the user status after the order has been transferred to purchasing.

This way you define how orders are passed on, whether they have to have reached a certain minimum status before being passed on, or whether they are locked. There are no limits for defining status, minimum status and lock status.

> **Example**
> The user status *Start of production* can be allocated to each individual document type. The document itself must have reached a certain status point, e.g. an order has to have the status *Production interface created*.

## Minimum and Lock Status

You can control the processes further by defining a minimum status or a lock status.

> **Example**
> You can define the minimum status a document has to have in order to be transferred to financial accounting (FinAcc), for example. Define a lock status to make sure the document is not transferred a second time to FinAcc.

Locking makes sense for partial shipments, namely if the partial shipments are not to be invoiced. A lock status can also be defined for complaints or when credit limits are exceeded.

## Exclusive Status

To change the document status, you can create and allocate status points with the code **exclusive**. Access to this kind of status can thus be controlled via management of rights. If a status has been marked as exclusive, it must be allocated to the user who is entitled to assign it. If this is not done, it will not be offered to this user for selection. The status change itself will not be locked.

## Lock Code

You can use a lock code to lock documents for certain transactions while automatically raising the status. This means that the document cannot reach the locked status but is instead diverted to another status point (process).

*(Fig. C-119: Lock status UI)*
The screen shows the configuration for a lock code.
- **A. Locked status:** The status that is to be locked (e.g., "750 Invoice printed").
- **B. Status point to which the document is diverted:** The alternative process to follow (e.g., "830 Transfer to FinAcc").
- **C. Lock code in the order header > Supplement tab:** Where the lock code is applied in an order.

### Example: Partial shipment without invoicing
Since these partial shipments must not be invoiced, the system has to be able to recognize this kind of partial shipment. In this case, no partial invoice can be created for the partial shipment. The status of the partial shipment will instead be raised automatically. After the order is diverted to **Transfer to archives**, the partial shipment cannot be edited any further.

Lock codes for complaints and partial shipments are preset in the company data. If a customer is to receive partial shipments without partial invoicing, this is defined in the customer master data.

> **Discuss required changes**
> Please discuss any changes of lock codes with A+W Software GmbH beforehand to avoid problems.

## Item Status

You can have the status from production reports displayed per item for every order. Quantities are taken into account as well.

*(Fig. C-120: Current status of order items)*
This UI displays the production status for each item in an order.
- **A. One column per item:** Each item has its own status column.
- **B. Registration points:** A list of production stages (e.g., Cutting started, IG started, produced).
- **C. Current status per item:** The current production status for the item.
- **D. Quantity that has been reported by the registration point:** The quantity of items that have passed a specific registration point.

Depending on the settings, the status of an item will be changed when the first sheet or the entire item has been produced.

You can also receive reports from production online. The reports are described in detail in the Production part.

## Allocate Status Point

This training module shows you how to edit the status allocation.

The following instructions exist for this training module:
- "How to allocate a status point" on page C-225
- "How to allocate a lock code" on page C-226

> **Testing amendments outside of the daily business hours**
> Please discuss any changes beforehand with a member of the A+W Software GmbH team.
> Test any change of status allocation first outside of business operations, using a special test document. The change should only be adopted for actual operation if the process proves to run correctly. This helps to avoid data processing problems in A+W Business.

### How to allocate a status point

1.  Select the menu **Master data > Order > Status allocation**.
    The dialog **Status allocation** opens.
2.  Go to the menu **Start > New** to switch to the input mode.
    *(Fig. C-121: Fields for status allocation are enabled)*
    The UI shows the status allocation screen in edit mode.
    - **A. Status point:** The selected process from the list.
    - **B. Document type:** The document type for the allocation.
    - **C. User status:** The user-defined status to be allocated.
3.  Select the status point (A) to be allocated to a user status.
