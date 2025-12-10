---
title: "EN_AWBusiness_Master_Data_9_5-2"
source: "EN_AWBusiness_Master_Data_9_5-2.pdf"
tags: ["A+W Business", "Master Data", "Status Allocation", "Lock Codes", "Number Ranges", "Rounding Rules", "Software Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a series of tutorials for configuring master data within the A+W Business software. It covers key setup processes including status allocation, defining and enabling lock codes to control document processing, setting up number ranges for various document types, and configuring rounding rules for financial calculations."
long_description: "This technical document serves as a tutorial guide for system administrators and power users of the A+W Business software, focusing on the setup and management of critical master data. The guide is divided into several key sections. The 'Status Allocation' section explains how to allocate status points and user statuses to documents, which control their lifecycle and processing steps. 'Allocation of Lock Codes' details how to create and apply lock codes to exclude documents from specific automatic processes, such as invoicing for partial shipments, and provides a step-by-step guide to enabling these codes in the company data settings. The 'Number Ranges' section offers an in-depth look at defining unique number sequences for different document types (e.g., orders, invoices, credit notes) across various organizational areas like clients and order areas, emphasizing the importance of non-overlapping ranges to ensure data integrity. Finally, the 'Roundings' section explains how to define and allocate rounding rules for calculated values like prices, taxes, and surcharges. It covers the creation of rounding methods (commercial, upwards, downwards) and their application to specific rounding points, clients, or partners, ensuring financial data accuracy and compliance with different currency requirements."
---

---
## Status Allocation

The **Status allocation** dialog is used to allocate status points and user statuses. There are no limits for defining status, minimum status, and lock status.

> **Discuss required changes**
> Please discuss all changes of status management and status allocation with A+W Software GmbH beforehand. This will help to avoid system errors or incompatibilities.

### How to allocate a status point

1.  Select menu **Master data > Order > Status allocation**.
    The **Status Allocation** window appears, showing the `Status allocation table` and the `Status allocation` details for the selected entry.

    *   **Fig. B-14 Status allocations** shows the main window with a list of status points on the left and the allocation details on the right.
    *   **Status point**: `001 Dokument erfaßt/Document entered`
    *   **Document type**: `all`
    *   **User status**: `001 Dokument erfasst / Document entered`
    *   **Min. status**: `000-`
    *   **Lock status**: `000-`

2.  Go to the menu **Start > New** to switch to the input mode. The fields for the new allocation become accessible.

    *   **Fig. B-15 Fields for the new allocation accessible** highlights the editable fields:
        *   **A**: Status point to which the user status shall be allocated
        *   **B**: Document to which the allocation applies
        *   **C**: User status to be allocated to the status point
        *   **D**: Minimum status the document has to have
        *   **E**: Lock status which must not be reached by the document

3.  Choose the **status point (A)** and the **document type (B)** for which this allocation shall be valid.
    > Please check the selected document type. If you select **all**, this status will be valid for all document types even if this does not make sense or does not help at all.

4.  Choose the **user status (C)** to be allocated to the status point and to the document type.

5.  If required, select a suitable **minimum status (D)** and the **lock status (E)**.
    > Please make sure that the new allocation does not contradict any existing allocations.

6.  Select in the menu **Start > Save** to save the data.
    The data will be saved. The new allocation will be used as a document status.

## Allocation of Lock Codes

Lock codes are used to exclude documents from certain steps of automatic processing.

For instructions on this subject, please see:
*   "How to set a lock code" on page B-428
*   "How to enable the lock code" on page B-430

> **Discuss required changes**
> Please discuss changes of the lock codes beforehand with A+W Software GmbH. This will help to avoid system errors or incompatibilities.

### How to set a lock code

1.  Select menu **Master data > Order > Lock code**. The **Lock Codes** window appears.

2.  Go to the menu **Start > New** to switch to the input mode. The fields become accessible.
    *   **Fig. B-17 Fields for new lock code are accessible** shows the editable fields:
        *   **A**: Name of the lock code
        *   **B**: User status to be locked
        *   **C**: Next possible status

3.  Enter the **description (A)**, e.g., `partial shipment without invoice`.

4.  Choose the **user status (B)** to be locked, e.g., `invoice printing`.

5.  Choose the **user status (C)** the document shall be diverted to, e.g., `transfer to financial accounting`.
    *   **Fig. B-18 New lock code** shows an example of a new lock code:
        *   **Name**: `Teillief. o. Rechnung / Partial delivery`
        *   **Status restriction**: `750-Rechnung gedruckt/Invoice printed`
        *   **Deviation to status point**: `097-FIBU Übergabe`

6.  Select in the menu **Start > Save** to save the data.
    The lock code for partial shipment without invoicing is saved. It has to be enabled in company data now.

### How to enable the lock code

1.  Go to menu **Master Data > Company > Company data**. The **Company data** dialog appears with the tab **Client**.

2.  Go to tab **Documents**.

3.  Select the lock code in field **Partial shipment (A)**. In **Fig. B-19 Company data > Documents**, this is shown in the "Lock Codes" section, where the "Partial delivery" dropdown is set to `Teillief. o. Rechnung`.

4.  Select in the menu **Start > Save** to save the data.
    The data will be saved. Invoices for partial shipments can no longer be issued. This entry is valid for all customers.

## Additional information

⇨ Software Reference, "Status Management" on page B-884
⇨ Software Reference, "Status Points" on page B-885
⇨ Software Reference, "Status Allocation" on page B-886
⇨ Software Reference, "Lock Code" on page B-897
⇨ Software Reference, “Company Data > Documents" on page B-928

## Number Areas

### Objectives
*   Introducing the function of number ranges.
*   Definition of number ranges.

### Benefits
*   Number ranges fix the allocation of unique (document) numbers.
*   Unique numbers guarantee that documents (and other sequence numbers) are passed on correctly in the business process.

### Please note

*   **Number areas**:
    *   Logical units of organization.
    *   A means of combining work processes which are triggered by number manager.
    Number ranges can be maintained for documents, for production, and for financial accounting. Within the individual number ranges, the sequences (serial numbers) are fixed, e. g. for documents. Number ranges must not overlap.

*   **Basic number areas**: The basic number ranges for master data are predefined; additional number ranges cannot be added.

*   **Client, order area, employee**: Separate number ranges can be defined for clients, order areas, and users. These number ranges must not overlap either.

*   **Document type**: The numbers for the individual document types are defined in different number ranges. A document number from the allocated number range is automatically assigned when the document is entered.

## The Function of Number Ranges

Number ranges are logical organization units as well as a means to combine work processes triggered by a so-called number manager.

The number ranges for documents and other sequence numbers have to be defined as required for your company. This is especially true for the following areas:
*   Document numbers
*   Production
*   FinAcc

Number ranges can be defined for every client and for every order area. This allows allocating a document based on its number. For every number range you define the range of numbers within which (serial) numbers can be allocated.

*   **Fig. B-20 Number areas** shows the number ranges for documents. The window is described by the following fields:
    *   **A**: Areas for number ranges (Client, Order area, Employee)
    *   **B**: Document types (Quotations, Orders, P.O.s, etc.)
    *   **C**: First valid number (`From`)
    *   **D**: Last allocated number (`Current`)
    *   **E**: Last valid number (`to`)
    *   **F**: Number of allocated numbers (`by period`)

This example shows the number ranges for documents. For every document type listed (B) you can define the number ranges (C, E) to be allocated. The document number is automatically assigned from the allocated number area when you create a document. The number areas must not overlap to make sure that these numbers are unique. This applies to all number ranges, i.e. document numbers, financial accounting numbers, and production numbers.

Individual number ranges can be locked. This way you can define that certain documents cannot be included in special areas.

## Document numbers

The following table provides examples of number areas. In this example, documents are entered in the order areas `toughened glass production` and `laminated glass production`. No documents can be entered outside these areas.

**Tab. B-2 Examples of number areas**

| Documents | Tempered glass production | Laminated glass production | `<n.e.>` |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| | **from** | **to** | **from** | **to** | **from** | **current** | **to** |
| Quotations | 300 | 19,999 | 20,000 | 39,999 | 0 | 1 | 0 |
| Orders | 100,000 | 199,999 | 200,000 | 299,999 | 0 | 1 | 0 |
| Purchase Orders | 300,000 | 399,999 | 400,000 | 499,999 | 0 | 1 | 0 |
| Supplier inquiries | 500,000 | 599,999 | 600,000 | 699,999 | 0 | 1 | 0 |
| Invoices | 700,000 | 799,999 | 800,000 | 899,999 | 0 | 1 | 0 |
| Credit notes | 100 | 199 | 200 | 299 | 0 | 1 | 0 |
| Delivery notes | 40,000 | 49,999 | 50,000 | 99,999 | 0 | 1 | 0 |
| **Production** | | | | | | | |
| AWPOOL sequential number | 0 | 0 | 0 | 0 | 1 | 1 | 9,999 |
| Partial Del. | 2,000,000 | 2,099,999 | 3,000,000 | 3,099,999 | 0 | 1 | 0 |
| Complaint when breakage | 2,100,000 | 2,199,999 | 3,100,000 | 3,199,999 | 0 | 1 | 0 |
| **FinAcc** | | | | | | | |
| ... | ... | ... | ... | ... | ... | ... | ... |

*   In the order area of toughened glass production, the number range for the document **Order** is from 100,000 to 199,999. For partial shipments, a range from 2,000,000 to 2,099,999 has been reserved and for complaints, 2,100,000 to 2,199,999. A clashing of number ranges is thus avoided. Overlapping is therefore prevented.
*   The order area `<n.e.>` is a standard area for which no orders shall be entered however. The number range is therefore locked by the values 0 (from) and 0 (to). 1 (current) represents a blank document.
*   The **AWPOOL sequential number** shall be assigned consecutively regardless of the OM area. In this case, number range (1 to 9999) is entered in order area `<n.e.>`. All other order areas are locked.

Partial shipments and complaints belong to the document type **Orders**. This is why these number ranges must not overlap. Individual number ranges are also kept for invoices and credit notes. As a special function, the same number range can be used for these two document types.
⇨ Software Reference, "Credit note/invoice number" on page B-930

For documents, you can also define different number ranges per user. If you are using different order areas you can e. g. allocate the document entry user to the order area for which he is responsible.
⇨ Software Reference, "Input parameters" on page B-1008

> **Other number ranges**
> The basic number areas for master data are defined by default and cannot be extended. These number ranges are listed in dialog **Basic number ranges**.
> The number range for rack management is defined in dialog **company data**.
> ⇨ Software Reference, "Company Data - Shipment" on page B-990

## Production Preparations

For order management, you can define so-called OM areas, for allocating orders to.

You can e.g. set up order areas especially for new customers or for managing internal orders. Interfaces are used to transfer the orders automatically to the corresponding order area for production. The order area also serves as a sorting criterion for turnover statistics.

*   **Fig. B-21 Production preparations** shows the **Order Areas** dialog with the following columns:
    *   **A**: Name of the order area
    *   **B**: Valid document types

Typically, OM areas refer to individual departments or subsidiaries of a company that generally work together. Order area toughened glass production for example is responsible for producing toughened glass.

Every order area has to be allocated to special number ranges so that documents can be passed on correctly.

Moreover, every employee can be allocated to an order area and document type. If e.g. the order area IG (A) is only meant for managing finished IG units (stock articles), it has to be allocated to the document type (B) Work order. The orders are then automatically entered in this OM area and the corresponding number area. Both can be changed manually in the order.
⇨ Software Reference, "Input parameters" on page B-1008

Order areas are set up like all basic tables.
⇨ Tutorial 1, "Extending basic tables" on page B-33

> **Order areas for different clients**
> Define all order areas your clients require. When the number ranges are set up, the order areas will be allocated to the corresponding client. Clients are described in a separate chapter.
> ⇨ Tutorial 1, "Clients and Subsidiaries" on page B-371

## Definition of Number Ranges

Number ranges must not overlap. This is why the number ranges are separately defined for each document type, e.g. to distinguish order numbers and invoice numbers.

> **Do not change the number range during operation**
> Changing the number range during operation may cause conflicts with old document numbers. Before changing the number range please check that the number managers contain no unprocessed documents.

> **Prerequisite**
> If you are going to work with clients these have to be defined before number ranges are set up. Define a training client even if you are not going to use clients for your business processes. You can always delete it after doing the exercises.

For instructions on this subject, please see:
*   "How to define the number ranges" on page B-437
*   "How to lock a number range for an order area" on page B-439

### How to define the number ranges

1.  Select menu **Master Data > Order > Number Ranges**. The dialog **Number Ranges** appears.
    ⇨ Software Reference, "Number Ranges" on page B-890
    Check and make a note of the number ranges which are still free. If no "gaps" are visible please reduce the number ranges of the current client. It may be possible to release the higher number ranges, e.g. from 100000 to 99999999.

2.  Go to the menu **Start > New** to switch to the input mode. The number ranges are preset by the values reserved for the first client.

3.  If required, select the **client (A)**, e.g. your training client.

4.  Please choose the entry **<n.e.>** for both the **order area (B)** and the **employee (C)**.

5.  Enter the numbers for quotations (D) in the fields **from** and **to**. Numbers may have up to eight digits. To lock the selected combination of client, order area, and employee for input, enter 0 in the fields **from** and **to** and 1 in field **current**.

6.  Repeat this step for all documents.

7.  Go to menu **Functions > Check**. If clashes with other number ranges are detected, the system will issue an appropriate message.
    > **Message [1720]**
    > Order area Vitropur, number area Credit note and Order area Isolierglasfertigung, number area Credit note are overlapping
    > Order area Vitropur, number area Credit note and Order area ESG-Fertigung, number area Credit note are overlapping
    > Order area Vitropur, number area Credit note and Order area <k.A.>, number area Credit note are overlapping
    > Order area Isolierglasfertigung, number area Credit note and Order area ESG-Fertigung, number area Credit note are overlapping
    > Order area Isolierglasfertigung, number area Credit note and Order area <k.A.>, number area Credit note are overlapping
    > Order area ESG-Fertigung, number area Credit note and Order area <k.A.>, number area Credit note are overlapping

    This message will tell you which number ranges have been causing conflicts.

8.  Correct your entries until the check reveals no further errors.

9.  Repeat the steps 5 and 7 on the other tabs to enter further sequence numbers. Use tab **Table** to check which number ranges have been defined already.

10. Select in the menu **Start > Save** to save the data. The data will be saved.

### How to lock a number range for an order area

1.  Select menu **Master Data > Order > Number Ranges**.
2.  Go to the menu **Start > New** to switch in the input mode.
3.  Select the order area.
4.  For quotations, enter 0 in the fields **from** and **to**.
5.  Enter 1 in field **current**.
6.  Select in the menu **Start > Save** to save the data.
    The data will be saved. It is now impossible to enter quotations in the selected order area. Repeat the steps for all document types which shall not be entered in this order area.

## Exercises

To edit the number ranges in this exercise you will need a new (special) client. Clients are entered in company data. There is a separate chapter on this subject. The following instructions are therefore strongly abridged.

### How to enter a client for this exercise

1.  Select menu **Master Data > Company > Company Data**. The **Company data** dialog appears.
2.  Go to the menu **Start > New** to switch to the input mode. The fields will be enabled.
3.  Enter the number, the matchcode, and the name.
4.  Select in the menu **Start > Save** to save the data. The data will be saved.

Enter the number ranges for your training client.
*   Make a note of the numbers which have already been reserved for documents.
*   Enter the number ranges for documents.
*   Check if there are clashes and correct if necessary.
*   Enter an order for this client and check if the order number has been taken from the right number range.

### Additional information

⇨ Tutorial 1, "Financial accounting (FinAcc)" on page B-369
⇨ Software Reference, "Number Ranges" on page B-890
⇨ Software Reference, "Company Data - Client" on page B-918
⇨ Software Reference, "Order Areas" on page B-1014

## Roundings

### Objectives
*   Checking the settings for rounding.
*   Allocation of roundings.
*   Defining rounding for individual partners

### Benefits
Values calculated by the program can be rounded to the desired number of digits. The settings for rounding always refer to a certain rounding point. They can thus be finely adjusted.

### Please note

*   **Rounding rate**: The following settings are made in the rounding record:
    *   Number of remaining decimal places.
    *   Value to be rounded to (last digit to be kept).
    *   Rounding method.
*   **Rounding type**: The rounding type defines whether rounding shall be made upward or downward.
*   **Rounding point**: Rounding points define the object rounding. The rounding points are fixed and cannot be edited. Common objects of rounding are:
    *   Prices
    *   Surcharges
    *   Tax
    *   Surface
*   **Rounding Allocation**: Rounding point and rounding have to be allocated so that the calculated value can be rounded. General allocations can apply to certain product groups. Special partners or partner groups can be rounded in different ways.

### Rounding Settings

The following settings are used for calculating the rounding:
*   The rounding itself: It defines the number of digits and the rounding type, e.g. upwards.
*   The rounding point: It defines the object of rounding, e. g. price, tax, surface.

*   **Fig. B-23 Rounding** shows an example with the following fields:
    *   **A Rounding**: The value to round to (e.g., 1, 5, 10, 50, 100).
    *   **B Digits to be rounded to**: The number of decimal places.
    *   **C Rounding method**: The type of rounding (e.g., Commercially, Upwards).

This example shows that apart from the rounding type (C), the number of digits (B) and the value (A) the figure shall be rounded to have been defined.

There are the following rounding types:
*   **Commercial**: Amounts from 0 to 4 will be rounded downwards and amounts from 5 to 9, upwards.
*   **Upwards**: The digits from 1 to 9 will be rounded upwards.
*   **Downwards**: The digits from 1 to 9 will be rounded downwards.

### Rounding Examples

**Tab. B-3 Rounding examples with two digits**
This example shows the results of the different rounding types.

| Rounding value | Digits | Example value | commercial | upwards | downwards |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 2 | 10.2237 | 10.22 | 10.23 | 10.22 |
| 1 | 2 | 10.2279 | 10.23 | 10.23 | 10.22 |
| 5 | 2 | 10.2237 | 10.20 | 10.25 | 10.20 |
| 5 | 2 | 10.2421 | 10.25 | 10.25 | 10.20 |
| 10 | 2 | 10.2237 | 10.20 | 10.30 | 10.20 |
| 10 | 2 | 10.2711 | 10.30 | 10.30 | 10.20 |
| 20 | 2 | 10.2237 | 10.20 | 10.40 | 10.20 |
| 20 | 2 | 10.3392 | 10.40 | 10.40 | 10.20 |
| 50 | 2 | 10.2237 | 10.00 | 10.50 | 10.00 |
| 50 | 2 | 10.4566 | 10.50 | 10.50 | 10.00 |
| 100 | 2 | 10.2237 | 10.00 | 11.00 | 10.00 |
| 100 | 2 | 10.6389 | 11.00 | 11.00 | 10.00 |

## Rounding Points

Rounding points define the object of rounding, e.g. the price for the surface, the price for processing, the surcharge. Rounding points are fixed in A+W Business and cannot be edited.

The following table lists all rounding points used for sales price calculation. Column **Description** refers to the example that deals with the corresponding rounding point in the example dialogs.

**Tab. B-4 Rounding points**

| No. | Rounding points - sales | No. | Rounding points - purchasing | Description |
| :-- | :--- | :-- | :--- | :--- |
| 1 | sqm price/QU glass item | 51 | PP sqm price/QU glass item | Example 2 |
| 2 | sqm price/QU surcharges | 52 | PP sqm price/QU surcharges | Example 3 |
| 3 | sqm price/QU processing | 53 | PP sqm price/QU processing | Example 3 |
| 4 | Gross/pc. glass item | 54 | PP: gross/pc. glass item | Gross prices will not be shown. |
| 5 | Gross/pc. surcharges | 55 | PP gross/pc. surcharges | |
| 6 | Gross/pc. processing | 56 | PP gross/pc. processing | |
| 7 | Gross/pc. per glass item | 57 | PP gross/pc. per glass item | |
| 8 | Gross/pc. per surcharge | 58 | PP gross/pc. per surcharge | |
| 9 | Gross/pc. per processing | 59 | PP gross/pc. no. of processing steps | |
| 10 | Net/pc. glass item | 60 | PP net/pc. glass item | Example 2 |
| 11 | Net/pc. surcharges | 61 | PP net/pc. surcharges | Example 3 |
| 12 | Net/pc. processing | 62 | PP net/pc. processing | Example 3 |
| 13 | Total item net Glass item * | 63 | PP total net per glass item | |
| 14 | Total net item surcharges | 64 | PP total item net - surcharges | Example 3 |
| 15 | Total net items Processing | 65 | PP total item net - processing | Example 3 |
| 16 | sqm IG | | | Example 2 |
| 17 | sqm other products | | | Example 2 |
| 18 | VAT 1 | | | Example 1 |
| 19 | VAT 2 | | | Example 1 |
| 20 | Miscellaneous | | | |
| 21 | Net/pc. per glass item | 71 | PP net/pc. per glass item | Example 2 |
| 22 | Net/pc. per surcharge | 72 | PP net/pc. per surcharge | Example 3 |
| 23 | Net/pc. per processing | 73 | PP net/pc. per processing | Example 3 |
| 24 | Total item net per glass item * | 74 | PP total item net per glass item | |
| 25 | Total item net per surcharge | 75 | PP total item net per surcharge | Example 3 |
| 26 | Total item net per processing | 76 | PP total item net per processing | Example 3 |
| 27 | Total item net | 77 | PP total item net | Example 2 |
| 28 | Total w/o VAT | 78 | Total PP | Example 1 |
| 79 | Detailed production cost calculation | | | Production price calculation |
| 118 | FC VAT 1 ** | | | Example 1 |
| 119 | FC VAT 2 | | | Example 1 |
| 128 | FC total w/o VAT | | | Example 1 |

*This price will not be shown. It results from net price x item quantity.*
**FC = foreign currency*

### Rounding examples

The following examples explain the allocation of rounding points and fields at document entry. The red numbers refer to the corresponding numbers in the column of rounding points for sales and the green numbers, to the column for purchasing.

*   **Example 1: Order – tab Totals (Fig. B-24)**
    *   `28`: Total w/o VAT
    *   `128`: FC total w/o VAT
    *   `18`, `118`: Tax 1
    *   `19`, `119`: Tax 2

*   **Example 2: Item entry – tab IG/article (Fig. B-25)**
    *   `27`: Net price
    *   `10`: Net price per piece
    *   `16/17`: Sqm price
    *   `1`: Sqm price
    *   `21`: Net price per piece

*   **Example 3: Item entry - tab BOM (Fig. B-26)**
    *   `2/3`: Surcharge Net
    *   `11/12/22/23`: Surcharge Net Total
    *   `14/15/25/26`: Surcharge Net Total
    *   `17`: Sqm price for details

## Rounding Allocation

The defined rounding and rounding points have to be allocated to each other. Allocations for product types/product groups, for clients and for partners can be defined in different ways.

The allocations made in dialog **Rounding allocation** are valid for all calculations for a client unless they are overruled by allocations for customers or suppliers.

*   **Fig. B-27 Standard allocation of roundings per client** shows the allocation screen with the following key fields:
    *   **A**: Client for which the roundings have been defined
    *   **B**: Rounding point (what shall be rounded)
    *   **C**: Rounding to net price
    *   **D**: Reference to the rounding (value, digits, rounding type) in the `Rounding table` field.

This example shows that in the selected line, the calculated surface price is rounded to three digits after the decimal point. This setting applies to all product types and product groups.

> **Size rounding**
> Size rounding is not affected by the settings for rounding. Size rounding is made in various dialogs for product and price definition. The program usually searches for details in the following sequence: Individual prices > Discounts > Prices > Products > Partners. The search ends as soon as details have been found.

### Rounding for Partners

Apart from the general rounding allocations, other rounding records can be defined and allocated to certain customers or suppliers. For currencies the smallest monetary unit of which is 0.05, amounts will have to be rounded accordingly.

For Swiss customers, the VAT is rounded (5 centimes) for instance. This requires defining the corresponding record and allocating it to your Swiss customers.

*   **Fig. B-28 Rounding allocation per customer** shows an example for a specific customer:
    *   **A**: Customer for whom these settings are valid
    *   **B**: Different roundings (table of specific rounding allocations)
    *   **C**: Rounding to net price

This example shows that a special rounding shall be used for the selected customer if the product is IG. For all other products, the general rounding applies.

### How to define a rounding

Rounding usually has to be reallocated only in case of changes, e. g. for a new customer or a new client. The following instructions describe the whole process of definition, i.e. how to define and allocate a rounding.

1.  Go to menu **Master data > Order > Rounding**. Dialog **Rounding** appears. To change a rounding, just amend the fields in question.
2.  Go to the menu **Start > New** to switch to the input mode. The fields become accessible.
    *   **Fig. B-29 Fields for new rounding are accessible** shows:
        *   **A**: (Descriptive) name
        *   **B**: Rounding value
        *   **C**: Digits
        *   **D**: Rounding type
3.  Enter the **name (A)**. Choose an expressive name, e.g. Swiss VAT.
4.  Enter the **value (B)** to be rounded to, e.g. 0.05.
5.  Enter the number of **digits (C)**, e.g. 2.
6.  Choose the **rounding type (D)**, e.g. commercial.
7.  Select in the menu **Start > Save** to save the data.
    The data will be saved. You can select this rounding now for all generally applicable rounding allocations or for partner-related rounding allocations. It is called **Rounding table** in the dialogs in question.

### How to allocate a rounding table

The following example describes the allocation for a customer. The steps are the same for suppliers and partner groups as well as for general rounding allocation, e.g. for a new client.

1.  Go to menu **Master data > Partners > Customer > Rounding**. Dialog **Rounding** appears. If rounding allocations have already been made for customers, these are displayed.
2.  Go to the menu **Start > New** to switch to the input mode.
    *   **Fig. B-30 Fields for the new rounding allocation are accessible** shows:
        *   **A**: Customer to whom this rounding is applied
        *   **B**: Rounding point
        *   **C**: Product type / Product class
        *   **D**: Price unit
        *   **E**: Rounding table
        *   **F**: Alternative rounding allocations
3.  Choose the **customer (A)**.
