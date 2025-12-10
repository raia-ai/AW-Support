---
title: "EN_AWBusiness_Master_Data_9_1-3"
source: "EN_AWBusiness_Master_Data_9_1-3.pdf"
tags: ["A+W Business", "Master Data", "Customer Data", "ERP", "Software Tutorial", "Order Management", "Invoicing", "Subsidiaries", "Classifiers"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial from the A+W Business Master Data guide, focusing on entering and managing customer data. It covers creating new customer records, configuring order and invoice settings, managing subsidiaries and employees, and using text modules and classifiers."
long_description: "This document is a detailed tutorial chapter from the A+W Business Master Data manual. It provides step-by-step instructions for users on how to manage customer information within the A+W Business software. The tutorial begins with the fundamental process of entering new customer data, including mandatory fields, addresses, and communication details. It then delves into more advanced configurations, such as setting up order and sales invoice parameters. This includes defining order priorities, standard rounding for pricing, minimum order values, and various invoicing methods like collective, monthly, and partial invoices. The guide also explains how to manage related entities, such as adding subsidiaries as additional shipping addresses and recording employee contact information for better customer relationship management. Furthermore, it covers the use of text modules for inserting standard or customized text into documents and the application of classifiers for filtering and analyzing customer data for purposes like turnover analysis. The document uses screenshots of the user interface with clear callouts to guide the user through each process."
---

# Tutorial 1: Customer Data

---
## How to enter customer data

1.  Go to menu **Master data > Partners > Customer > Customers**.
    Dialog **Partner management** appears with the tab **Address**.
2.  Go to the menu **Start > New** to switch to the input mode.

[Image: The Partner management screen for entering a new customer's data on the 'Address' tab. The screen is divided into sections for Identification, Address, Connections, Specification, and a table view at the bottom.]

*   **A** Mandatory fields
*   **B** Standard shipping and invoicing address
*   **C** Communication data
*   **D** Customer's language
*   **E** Shipping details

*Fig. B-16 Fields for new partner are accessible*

3.  If several clients have been defined, choose the client now.
4.  Enter the number and the matchcode in the mandatory fields (A).
    You can choose the numbers for your customers, suppliers, and other business partners at random; every number must however be assigned just once. You can view the free numbers by clicking on the [Zoom] icon.
5.  Enter the address data (B).
    If the required data cannot be found in the combo box yet, you can click on the file symbol to open the corresponding dialog and add the data.
6.  Enter the communication data (C).
7.  Choose the main route (route 1), an alternative route (route 2) (E), and the delivery terms.
    If you communicate in another language (D) with your new customer, please select this language. The corresponding language key will be used in the documents so that e.g. the product names are printed in the defined language.
    For a description of multi-lingual operation please refer to the Software Reference.
8.  Select in the menu **Start > Save** to save the data.
    With this you have entered the main data for identifying a customer. You can now add the invoicing data on tab **Order**.

## Order and Sales Invoice

### Objectives

*   Defining the priority of orders
*   Knowing the settings for invoices, monthly invoices, and collective invoices
*   Knowing the settings for partial shipments and partial invoicing

### Benefit

*   Settings from customer master data are applied to the order and do not have to be entered again.
*   Most settings from master data can be adapted in the order.

### Note

| Term | Description |
| :--- | :--- |
| **Priority** | The order priority defines the urgency for producing a certain order. It is transferred to capacity planning and thus to production. |
| **Invoice** | Settings for invoices can be made by customer: <br> • Standard rounding <br> • Minimum invoice value <br> • Invoice printing (single, collective) |
| **Standard rounding** | The glass surface is rounded for pricing purposes. This rounding is not valid for production purposes. |
| **Type of invoice** | Collective invoices, monthly invoices, or partial invoices can be issued only if these have been set as valid types in customer master data. |

## Order Settings

Tab **Orders** serves to enter details for invoicing and shipping.

[Image: The 'Partner management – Order' tab screen, showing various settings for orders, including priority, rounding, surcharges, and invoice details.]

*   **A** Standard rounding of height and width
*   **B** Invoicing details
*   **C** Priority of orders
*   **D** Invoice details

*Fig. B-17 Partner management – Order*

The invoice details (A, B, D) and priority (C) can be changed in the order. These settings will be described in detail below.

### Priority of orders

The order priority defines the urgency for producing a certain order. It is transferred to capacity planning and thus to production.
*   **Express**: These orders are produced with top priority.
*   **Normal**: These orders are fitted into the usual schedule.
*   **Extra**: The order shall be produced from residue (plates) left over from cutting other orders.
*   **On call**: Orders are produced on call.

## Invoice Settings

Settings for invoices can be made by customer:
*   Standard rounding
*   Minimum invoice value
*   Invoice printing (single, collective)

[Image: The 'Customer master data - tab Order' screen with various invoice settings highlighted.]

*   **A** Size rounding for pricing purposes
*   **B** Surcharge for minimum invoice value
*   **C** Minimum value (amount)
*   **D** Code for collective invoice
*   **E** Printing of invoice and prices
*   **F** Partial shipment and partial invoice
*   **G** Application of standard surcharges
*   **H** Monthly invoice

*Fig. B-18 Customer master data - tab Order*

### Standard rounding

The glass surface is rounded for pricing purposes (A). In Germany, pricing is based on rounding to thirty. This means that calculation is based on the next value that can be divided by 30. For a lite of 1000 mm x 1000 mm, pricing will be based on a surface of 1.04 sqm (= 1020 x 1020). French companies e.g. round the glass surface in steps of ten.

This rounding is not valid for production purposes.

The size rounding defined in partner data can be overruled by other settings. A+W Business will search for the settings in the following sequence: Unit prices > Discounts > Prices > Partner master data. Detailed training on pricing will be provided in connection with the Sales module.

### Invoicing surcharge

The invoicing surcharge (G) must be defined as a *Miscellaneous surcharge*. These surcharges will be introduced in the corresponding training session.
*   **For every first invoice of the month**: The surcharge will be applied only to the first invoice of the month. For all other invoices of the current month, this surcharge will be omitted.
*   **For every invoice**: The invoicing surcharge will be applied to every invoice.

### Min. order value

You can enter a minimum value (C) per order. The difference from the minimum order value can be shown in two ways in an order:
*   **As a separate item**: If the order value lies below the defined minimum order value, the surcharge item *Minimum order value* will be added automatically, showing the difference.
*   **Split to all items**: The difference is split to all items.

There are two calculation options:
*   You can define a surcharge to be applied to the order if the minimum value is not reached.
*   The minimum value will be automatically calculated if the order value falls below the defined limit.

### Monthly invoice

Invoices can be printed and sent off individually, collectively, or as a monthly invoice (H), e.g. every month or every fortnight. When printing delivery notes for this customer's orders, they will automatically be marked as *Monthly invoice* based on which you can select the maturity for invoicing.
The appropriate print point and status point have to be entered on tab **Print** in company data for this purpose.

[Image: A small dialog box for 'Monthly invoices' settings showing fields for 'Print point' and 'Status point'.]

*Fig. B-19 Company data - Printing*

### Collective invoice

If a customer does not want to receive individual invoices, all of his orders will be marked for collective invoicing (D). This code can be used to select the invoices due.

The following criteria have to be the same in all orders of the corresponding customer so that they can be combined in a collective invoice:
*   Customer number
*   Code 'print collective invoice' in the order
*   Payment terms and due date
*   Currency
*   VAT code 1 and 2
*   Automatic surcharges: Invoicing surcharge.
*   Order area
*   Invoice address (name 1)
*   Delivery date

If one of these criteria differs in an order, printing of the collective invoice will stop at this order. This order and all those following in the number manager will automatically get a new invoice number. This means that two invoices will be issued in this case. Another invoice number will be assigned should further differences surface.

### Partial Shipment, Partial Invoice

If partial shipments have been agreed with a customer (F) you have to decide whether or not the partial shipment shall be accompanied by a partial invoice.

Partial invoicing means that the customer will get an invoice for every partial shipment. The amount and quantity of this partial invoice will be deducted from the original order.

If partial invoicing is not permitted, the original order is blocked for invoicing until the last partial shipment has been made.

> **Partial shipment in an order**
> You can create a partial shipment from an order only if the checkbox *Partial shipment* has been ticked in this customer's master data.

## Editing the Settings for the Customer's Order

The following instructions are based on the steps described in the previous session.

### How to complete the data for customer documents

1.  Select menu **Master Data > Partners > Customer > Customers > Orders** tab.

[Image: The 'Addresses and shipping data' screen, which is the 'Order' tab in Partner management.]

*   **A** Standard size rounding
*   **B** Invoicing
*   **C** Document dispatch
*   **D** Partial shipment, partial invoice
*   **E** Route hierarchy

*Fig. B-20 Addresses and shipping data*

2.  Check whether the values for the size rounding (A) have been entered correctly.
3.  Define the invoicing mode (B).
4.  Select the buttons (C) for fax and email dispatch of documents. This function can be enabled separately for the following documents:
    *   Order confirmation (OC)
    *   Quotation (Qu)
    *   Invoice (In)
    *   Credit note (Cr)
    Please remember to enter the corresponding fax numbers and email addresses on tab **Address**.
5.  Define whether partial shipments and partial invoices are permitted for this customer (D).
6.  Check whether the number for route hierarchy (E) and the priority have been set correctly.
7.  Select in the menu **Start > Save** to save the data.
    The data will be saved. You can now add subsidiaries and employees for this customer.

## Employees and Subsidiaries

### Objectives

*   Using subsidiaries as additional shipping addresses.
*   Introducing transactions.

### Benefit

*   Subsidiaries can serve as additional shipping addresses if e.g. the customer has got several warehouses. The applicable shipping address can be selected in the order.
*   Further details on employees serve for improving customer relations so that the persons in charge can be addressed directly.

### Note

| Term | Description |
| :--- | :--- |
| **Subsidiaries** | For your partner's subsidiaries, the same data will be entered as for the headquarters. |
| **Employees** | The data on your customer's employees serve for information only. |
| **Transaction** | Transactions can be used to trace certain customer contacts. |

### Customer's Subsidiaries

For your partner's subsidiaries, the same data will be entered as for the headquarters. The latter will be preset in the corresponding fields and can be adjusted as required.

[Image: A screenshot showing the 'Subsidiary' creation screen within the customer management interface.]
*Fig. B-21 Subsidiary*

**Defining the standard shipping address as a subsidiary**
Apart from the company address you can enter further addresses for shipping and invoicing. These addresses are entered as subsidiaries. The checkbox **Standard** has to be ticked on tab **Address** in section **Address** for the subsidiary that is to be used as the standard shipping address.

### Customer's Employees

You can enter the names of your customer's employees for information.

[Image: The 'Employees' data entry screen, showing fields for name, address, department, position, contact details, and classifiers.]
*Fig. B-22 Employees*

You can add further details like his department, his position, and his extension. You can define whether this person is the sole contact in questions regarding orders and/or sales.

These details can be used for analysis via ODBC interface.

### Transaction

So-called transactions can e.g. be used to note which employee of the customer has called asking for information, and when.
At the same time you can note when this transaction was completed, and by whom.

[Image: The 'Transaction management' screen, showing fields to log a customer interaction, including receipt date, type, responsible person, and follow-up actions.]
*Fig. B-23 Transactions*

## Add Subsidiaries

Choose the subsidiary number so that the connection with its headquarters becomes evident, e.g. 10000 for the customer, 10100, 10200, ... for the subsidiaries.

### How to enter a subsidiary

1.  Go to menu **Master data > Partners > Customer > Customers**.
    The **Partner management** dialog pops up.
2.  Search the record of the partner required.
3.  Go to menu **Functions > Details group > Subsidiary**.

[Image: The partner management screen showing the fields accessible for a new subsidiary.]

*   **A** Standard shipping address
*   **B** Close subsidiary and show main company
*   **C** Independent subsidiary

*Fig. B-24 Fields for the new subsidiary are accessible*

4.  Enter at least the address and communication data.
    You can add further data on the tabs as described in the instructions for entering customer data.
5.  Select in the menu **Start > Save** to save the data.
    The data will be saved. On tab **Address**, the checkbox **Standard (A)** and the button **[back to main company] (B)** are accessible.
6.  Amend the subsidiary's data, e.g. the routes. Please obey the following settings:
    *   Tick the checkbox **Standard (A)** if this subsidiary is the standard shipping address.
    *   Tick the checkbox **Independent subsidiary (C)** if this subsidiary can place its own orders.
7.  Select in the menu **Start > Save** to save the data.
    The data will be saved.
8.  Click on button **(B)** to close the dialog.
    The main company's data appear again.

## Add Employees

You can define the area for which the employees of your partners are responsible. This detail only serves for information.

### How to enter details on your partner's employees

1.  Go to menu **Master data > Partners > Customer > Customers**.
    The **Partner management** dialog pops up.
2.  Search the record of the partner required.
3.  Go to menu **Functions > Details group > Employee**.

[Image: The data entry screen for a new employee of a customer.]

*   **A** Name of customer's employee
*   **B** Employee's position (for information only)
*   **C** Communication data
*   **D** Release fields

*Fig. B-25 Fields for new employees are accessible*

If a customer's employees have already been entered, the appropriate data are shown.

4.  Click on **[New] (D)** to release the fields. If the customer's employees have already been entered you can change the data.
5.  Enter at least the name (A) and the phone number (C).
6.  Add further details if these are important for communicating with this employee, e.g. the employee's function (B).

With that you have entered the main data.

[Image: The employee data entry screen after data has been entered, with the 'New' button highlighted.]

*   **A** Save employee's data

*Fig. B-26 Fields for new employees are accessible*

7.  Click on **[New] (A)** to save the data.
    The data will be saved. You can now enter details of other employees by repeating the steps 5 to 7.
8.  Click on **[End]** to close the dialog.
    Dialog **Partner Management** reappears in the foreground. Tab **Empl./Subsid./Settings** shows the employees.

## Text

### Objectives

*   Entering customized text.
*   Introducing text codes.

### Benefit

*   Text provides information on certain facts, e. g. special requests in connection with production.

### Note

| Term | Description |
| :--- | :--- |
| **Customised text** | Text which is used just for a single customer can be entered in customer master data, to be automatically added to the document. |
| **General text** | Frequently used text can be entered as 'general text' which can be automatically inserted in a document by means of customer master data. |
| **Text codes** | Text codes serve to define the documents in which the text shall be printed, e. g. order confirmations, delivery notes. |

### Text and Text Codes

Recurring text can be saved, e.g. to be included in the document automatically. We distinguish system-, default-, and spacer text.

Standard text is distinguished by means of text codes, e. g. text code Q for quotations, P for production, D for delivery note. Text codes can be entered according to your company's requirements.

**Examples**
*   **Info text (text code /):**
    Shall be printed on all documents, e.g. to announce company holidays.
*   **Delivery note text (text code D):**
    To be printed only on delivery notes, e.g. deadlines for complaints.
*   **Quotation text (text code Q):**
    To be printed only on quotations, e.g. the validity of the quote.

Text codes are not only used for grouping your standard text. Text codes can also serve to define when text shall be printed.

> **Example**
> Production text (text code P) shall not be printed on delivery notes. In management of forms you can define - for every form - the text codes that shall not be printed.

You can enter special spacer text for every IG unit, and allocate them to the product.

In partner and product master data you can enter text that shall always be used in documents. This can be standard text or text which is entered just for the partner or the product.

> **Detailed description of text**
> Text modules are described in detail in Tutorial 2.
> ⇨ Tutorial 2, "Text" on page B-460

## Entering Text in Customer Master Data

This example describes a text module in customer master data. Text for suppliers or products can be entered in the same way.

There are the following instructions on this subject.
*   "How to allocate standard text" on page B-69
*   "How to enter customised text" on page B-71

> **Fonts and type size**
> The settings for the fonts and the type size only apply to the display on screen. They will not be used for printing.

### How to allocate standard text

1.  Go to menu **Master data > Partners > Customer > Customers > tab Text**.

[Image: The 'Text' tab in partner management, showing the fields for adding a new standard text.]

*   **A** Release fields
*   **B** Number of the standard text
*   **C** Check the text code

*Fig. B-27 Release the fields for new text*

2.  Click on the (A) icon to release the input fields.
3.  Enter the number (B) of the desired standard text or select it using the magnifier symbol.
    If you enter the text number directly you have to press the `<Tab>` key to go to the next field to make sure that the text is loaded.

[Image: The 'Text' tab after a standard text module has been allocated, showing the list of allocated texts and the editing field.]

*   **A** List of allocated text modules
*   **B** Editing field

*Fig. B-28 Allocated standard text*

The standard text appears in the editing field (B). You can edit it and change it as required for the customer in question.

4.  Select in the menu **Start > Save** to save the data.
    According to the text code, the standard text will be printed on the appropriate forms or is transferred to production.
    Enter the spacer text in the same way.

### How to enter customised text

1.  Go to menu **Master data > Partners > Customer > Customers > Text** tab.

[Image: The 'Text' tab with fields ready for custom text input.]

*   **A** Release fields
*   **B** Text Number
*   **C** Select text code
*   **D** Text input

*Fig. B-29 Text input*

2.  Click on the (A) icon to release the input fields.
3.  Choose a text code (C), e. g. *I Information text*.
    The text code defines how the text shall be used. If the text shall be transferred to production for example, choose text code P. If no text code is entered, the text will not be transferred.
    Keep the entry 0 in the **Number (B)** field.
4.  Enter the desired text in the input field (D).

[Image: The 'Text' tab showing a custom text 'Rack one-side loading only' entered into the text block.]
*Fig. B-30 Customised text*

5.  Select in the menu **Start > Save** to save the data.
    The data will be saved and will be used only for this customer acc. to the text code.
    In the same way, you can enter text for individual suppliers, partners, or products.

## Classifiers

### Objectives

*   Defining classifiers.
*   Allocating classifier values.

### Benefit

*   Classifiers serve as filters for additional analyses, e. g. turnover.

### Note

| Term | Description |
| :--- | :--- |
| **Classifiers** | Classifiers are defined for all partners, or just for customers, suppliers, or partners. |
| **Classifier values** | Classifier values can be numerical, alpha-numerical, or dates. |

## Classifier and Classifier Value

Classifiers are defined in order to use them as filters for additional analyses, e. g. turnover, birthday, hobbies. You can also define whether the entry is numerical, alpha-numerical, or a date. Classifiers which are no longer required can be deleted.

Working with classifiers is based on two steps:
*   Define a classifier.
*   Enter a name for the classifier and define the values it can adopt.
*   Allocate a classifier value.

### Enter a Classifier

Classifiers for customers, suppliers, or partners can be entered in the corresponding partner management.

#### How to enter a classifier

1.  Go to **Master data > Partners > Customer > Customer > menu Functions > Classifier group > Classifier definition**.

[Image: The 'Classifier definition' screen with tabs for Common, Customers, Suppliers, and Partners.]

*   **A** Tab defining the validity
*   **B** Release fields

*Fig. B-31 Enter a Classifier*

Classifiers entered in tab **Common** are valid for all partners. The other three tabs serve to define classifiers that apply to the corresponding group only.

2.  Select the required tab, e. g. **Common**.
    On this tab, enter a classifier that is valid for all partners.
3.  Click on **[New]** to get access to the next line.

[Image: The 'Classifier definition' screen showing the fields for a new classifier being entered.]

*   **A** Name can be chosen at random
*   **B** Comments, e.g. regarding the use
*   **C** Classifier type:
    *   N: numerical
    *   A: alpha-numerical
    *   D: date

*Fig. B-32 Fields for new classifier are accessible*

4.  Make your entries:
    *   In field **Name (A)** e. g. group turnover.
    *   In field **Comment (B)** e. g. ABC classification.
5.  Tick one of the checkboxes (C) to define if the entry has to be numerical, alpha-numerical, or a date.
    This defines the way in which the classifier values can be entered in partner management, and how they will be analysed.
6.  Click on **[New]** to save the data.
    The data will be saved. All classifiers on tab **Common** are listed for all partners in partner management on tab **Classifiers**. All other classifiers will only be listed for the corresponding partners.

### Allocate Classifier Value

Classifier definition determines the type of values a classifier can have. This definition determines the way in which the value is allocated.

There are the following instructions on this subject.
