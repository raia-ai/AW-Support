---
description: "EN-UM-AWBusiness_6"
---


# Tutorial 2: Documents

---
## Status Allocation

| | | |
| :--- | :--- | :--- |
| **A** | Status point to which the user status shall be allocated | **D** | Minimum status the document has to have |
| **B** | Document to which the allocation applies | **E** | Lock status which must not be reached by the document |
| **C** | User status to be allocated to the status point | | |

*Fig. B-271: Fields for the new allocation accessible*

3.  Choose the status point (A) and the document type (B) for which this allocation shall be valid.
    Please check the selected document type. If you select all, this status will be valid for all document types even if this is does not make sense or does not help at all.

4.  Choose the user status (C) to be allocated to the status point and to the document type.

5.  If required, select a suitable minimum status (D) and the lock status (E).
    Please make sure that the new allocation does not contradict any existing allocations.

6.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved. The new allocation will be used as a document status.

## Allocation of lock codes

Lock codes are used to exclude documents from certain steps of automatic processing.

For instructions on this subject, please see:
*   "How to set a lock code" on page B-502
*   "How to enable the lock code" on page B-505

> **Discuss required changes**
> Please discuss changes of the lock codes beforehand with A+W Software GmbH. This will help to avoid system errors or incompatibilities.

### How to set a lock code

1.  Select menu `Master data` > `Order` > `Lock code`.
    *Fig. B-272: Setting a lock code*
    ⇨ Software Reference, "Lock Code" on page B-923

2.  Go to the menu `Start` > `New` to switch to the input mode.

| | |
| :--- | :--- |
| **A** | Name of the lock code |
| **B** | User status to be locked |
| **C** | Next possible status |

*Fig. B-273: Fields for new lock code are accessible*

3.  Enter the description (A), e.g. partial shipment without invoice.
4.  Choose the user status (B) to be locked, e.g. invoice printing.
5.  Choose the user status (C) the document shall be diverted to, e.g. transfer to financial accounting.

*Fig. B-274: New lock code*

6.  Select in the menu `Start` > `Save` to save the data.
    The lock code for partial shipment without invoicing is saved. It has to be enabled in company data now.

### How to enable the lock code

1.  Go to menu `Master Data` > `Company` > `Company data`.
    Dialog `Company data` appears with the tab `Client`.
2.  Go to tab `Documents`.

| | |
| :--- | :--- |
| **A** | Enable the lock code for partial shipments |

*Fig. B-275: Company data > Documents*

⇨ Software Reference, "Company Data > Documents" on page B-952

3.  Select the lock code in field `Partial shipment` (A).
4.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved. Invoices for partial shipments can no longer be issued. This entry is valid for all customers.

### Additional information

⇨ Software Reference, "Status Management" on page B-913
⇨ Software Reference, "Status Points" on page B-914
⇨ Software Reference, "Status Allocation" on page B-915
⇨ Software Reference, "Lock Code" on page B-923
⇨ Software Reference, “Company Data > Documents" on page B-952

## Number areas

### Objectives
*   Introducing the function of number ranges.
*   Definition of number ranges.

### Benefits
*   Number ranges fix the allocation of unique (document) numbers.
*   Unique numbers guarantee that documents (and other sequence numbers) are passed on correctly in the business process.

### Please note

*   **Number areas**
    *   Number ranges are:
        *   Logical units of organization.
        *   A means of combining work processes which are triggered by number manager.
    *   Number ranges can be maintained for documents, for production, and for financial accounting.
    *   Within the individual number ranges, the sequences (serial numbers) are fixed, e.g. for documents.
    *   Number ranges must not overlap.

*   **Basic number areas**
    *   The basic number ranges for master data are predefined; additional number ranges cannot be added.

*   **Client, order area, employee**
    *   Separate number ranges can be defined for clients, order areas, and users.
    *   These number ranges must not overlap either.

*   **Document type**
    *   The numbers for the individual document types are defined in different number ranges.
    *   A document number from the allocated number range is automatically assigned when the document is entered.

### The function of number ranges

Number ranges are logical organization units as well as a means to combine work processes triggered by a so-called number manager.

The number ranges for documents and other sequence numbers have to be defined as required for your company. This is especially true for the following areas:
*   Document numbers
*   Production
*   FinAcc

Number ranges can be defined for every client and for every order area. This allows allocating a document based on its number.

For every number range you define the range of numbers within which (serial) numbers can be allocated.

| | | |
| :--- | :--- | :--- |
| **A** | Areas for number ranges | **D** | Last allocated number |
| **B** | Document types | **E** | Last valid number |
| **C** | First valid number | **F** | Number of allocated numbers |

*Fig. B-276: Number areas*

This example shows the number ranges for documents. For every document type listed (B) you can define the number ranges (C, E) to be allocated. The document number is automatically assigned from the allocated number area when you create a document. The number areas must not overlap to make sure that these numbers are unique. This applies to all number ranges, i.e. document numbers, financial accounting numbers, and production numbers.

Individual number ranges can be locked. This way you can define that certain documents cannot be included in special areas.

### Document numbers

**Tab. B-21: Examples of number areas**

**Documents**

| | Tempered glass production | Laminated glass production | <n.e.> |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| | **from** | **to** | **from** | **to** | **from** | **current** | **to** |
| **Quotations** | 300 | 19,999 | 20,000 | 39,999 | 0 | 1 | 0 |
| **Orders** | 100,000 | 199,999 | 200,000 | 299,999 | 0 | 1 | 0 |
| **Purchase Orders** | 300,000 | 399,999 | 400,000 | 499,999 | 0 | 1 | 0 |
| **Supplier inquiries** | 500,000 | 599,999 | 600,000 | 699,999 | 0 | 1 | 0 |
| **Invoices** | 700,000 | 799,999 | 800,000 | 899,999 | 0 | 1 | 0 |
| **Credit notes** | 100 | 199 | 200 | 299 | 0 | 1 | 0 |
| **Delivery notes** | 40,000 | 49,999 | 50,000 | 99,999 | 0 | 1 | 0 |

**Production**

| | | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **AWPOOL sequential number**| 0 | 0 | 0 | 0 | 1 | 1 | 9,999 |
| **Partial Del.** | 2,000,000 | 2,099,999 | 3,000,000 | 3,099,999 | 0 | 1 | 0 |
| **Complaint when breakage** | 2,100,000 | 2,199,999 | 3,100,000 | 3,199,999 | 0 | 1 | 0 |

**FinAcc**

| | | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **FinAcc sequential** | 0 | 0 | 0 | 0 | 1 | 1 | 99,999,999 |

In this example, documents are entered in the order areas toughened glass production and laminated glass production. No documents can be entered outside these areas.

*   In the order area of toughened glass production, the number range for the document Order is from 100,000 to 199,999. For partial shipments, a range from 2,000,000 to 2,099,999 has been reserved and for complaints, 2,100,000 to 2,199,999. A clashing of number ranges is thus avoided. Overlapping is therefore prevented.
*   The order area `<n.e.>` is a standard area for which no orders shall be entered however. The number range is therefore locked by the values 0 (from) and 0 (to). 1 (current) represents a blank document.
*   The AWPOOL sequential number shall be assigned consecutively regardless of the OM area. In this case, number range (1 to 9999) is entered in order area `<n.e.>`. All other order areas are locked.

Partial shipments and complaints belong to the document type Orders. This is why these number ranges must not overlap. Individual number ranges are also kept for invoices and credit notes. As a special function, the same number range can be used for these two document types.
⇨ Software Reference, "Credit note/invoice number" on page B-954

For documents, you can also define different number ranges per user. If you are using different order areas you can e. g. allocate the document entry user to the order area for which he is responsible.
⇨ Software Reference, "Input parameters" on page B-1035

> **Other number ranges**
> The basic number areas for master data are defined by default and cannot be extended. These number ranges are listed in dialog Basic number ranges.
>
> The number range for rack management is defined in dialog company data.
> ⇨ Software Reference, "Company Data – Shipment" on page B-1017

## Production preparations

For order management, you can define so-called OM areas, for allocating orders to.

You can e.g. set up order areas especially for new customers or for managing internal orders. Interfaces are used to transfer the orders automatically to the corresponding order area for production. The order area also serves as a sorting criterion for turnover statistics.

| | |
| :--- | :--- |
| **A** | Name of the order area |
| **B** | Valid document types |

*Fig. B-277: Production preparations*

Typically, OM areas refer to individual departments or subsidiaries of a company that generally work together. Order area toughened glass production for example is responsible for producing toughened glass.

Every order area has to be allocated to special number ranges so that documents can be passed on correctly.

Moreover, every employee can be allocated to an order area and document type. If e.g. the order area IG (A) is only meant for managing finished IG units (stock articles), it has to be allocated to the document type (B) Work order. The orders are then automatically entered in this OM area and the corresponding number area. Both can be changed manually in the order.
⇨ Software Reference, "Input parameters" on page B-1035

Order areas are set up like all basic tables.
⇨ Tutorial 1, "Extending basic tables" on page B-93

> **Order areas for different clients**
> Define all order areas your clients require. When the number ranges are set up, the order areas will be allocated to the corresponding client. Clients are described in a separate chapter.
> ⇨ Tutorial 1, "Clients and Subsidiaries" on page B-442

## Definition of number ranges

Number ranges must not overlap. This is why the number ranges are separately defined for each document type, e.g. to distinguish order numbers and invoice numbers.

> **Do not change the number range during operation**
> Changing the number range during operation may cause conflicts with old document numbers. Before changing the number range please check that the number managers contain no unprocessed documents.

> **Prerequisite**
> If you are going to work with clients these have to be defined before number ranges are set up. Define a training client even if you are not going to use clients for your business processes. You can always delete it after doing the exercises.

For instructions on this subject, please see:
*   "How to define the number ranges" on page B-511
*   "How to lock a number range for an order area" on page B-513

### How to define the number ranges

1.  Select menu `Master Data` > `Order` > `Number Ranges`.
    Dialog `Number Ranges` appears.
    ⇨ Software Reference, "Number Ranges" on page B-918
    Check and make a note of the number ranges which are still free. If no "gaps" are visible please reduce the number ranges of the current client.
    It may be possible to release the higher number ranges, e.g. from 100000 to 99999999.

2.  Go to the menu `Start` > `New` to switch to the input mode.

| | | |
| :--- | :--- | :--- |
| **A** | Choose the client | **C** | Choose the employee |
| **B** | Select the order area | **D** | Define the number range |

*Fig. B-278: Fields for the new number ranges are accessible*

⇨ Software Reference, "Number Ranges" on page B-918
The number ranges are preset by the values reserved for the first client.

3.  If required, select the client (A), e.g. your training client.
4.  Please choose the entry `<n.e.>` for both the order area (B) and the employee (C).
5.  Enter the numbers for quotations (D) in the fields `from` and `to`.
    Numbers may have up to eight digits.
    To lock the selected combination of client, order area, and employee for input, enter 0 in the fields `from` and `to` and 1 in field `current`.
6.  Repeat this step for all documents.
7.  Go to menu `Functions` > `Check`.
    If clashes with other number ranges are detected, the system will issue an appropriate message.

> **Message [1720]**
> Order area Vitropur, number area Credit note and Order area Isolierglasfertigung, number area Credit note are overlapping
> Order area Vitropur, number area Credit note and Order area ESG-Fertigung, number area Credit note are overlapping
> Order area Vitropur, number area Credit note and Order area <k.A.>, number area Credit note are overlapping
> Order area Isolierglasfertigung, number area Credit note and Order area ESG-Fertigung, number area Credit note are overlapping
> Order area Isolierglasfertigung, number area Credit note and Order area <k.A.>, number area Credit note are overlapping
> Order area ESG-Fertigung, number area Credit note and Order area <k.A.>, number area Credit note are overlapping
>
> This message will tell you which number ranges have been causing conflicts.

8.  Correct your entries until the check reveals no further errors.
9.  Repeat the steps 5 and 7 on the other tabs to enter further sequence numbers.
    Use tab `Table` to check which number ranges have been defined already.
10. Select in the menu `Start` > `Save` to save the data.
    The data will be saved.

### How to lock a number range for an order area

1.  Select menu `Master Data` > `Order` > `Number Ranges`.
2.  Go to the menu `Start` > `New` to switch to the input mode.
3.  Select the order area.
4.  For quotations, enter 0 in the fields `from` and `to`.
5.  Enter 1 in field `current`.
6.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved. It is now impossible to enter quotations in the selected order area. Repeat the steps for all document types which shall not be entered in this order area.

## Exercises

To edit the number ranges in this exercise you will need a new (special) client. Clients are entered in company data. There is a separate chapter on this subject. The following instructions are therefore strongly abridged.

### How to enter a client for this exercise

1.  Select menu `Master Data` > `Company` > `Company Data`.
    The `Company data` dialog appears.
2.  Go to the menu `Start` > `New` to switch to the input mode.
    The fields will be enabled.
3.  Enter the number, the matchcode, and the name.
4.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved.

Enter the number ranges for your training client.
*   Make a note of the numbers which have already been reserved for documents.
*   Enter the number ranges for documents.
*   Check if there are clashes and correct if necessary.
*   Enter an order for this client and check if the order number has been taken from the right number range.

### Additional information
⇨ Tutorial 1, "Financial accounting (FinAcc)" on page B-440
⇨ Software Reference, "Number Ranges" on page B-918
⇨ Software Reference, "Company Data - Client" on page B-943
⇨ Software Reference, "Order Areas" on page B-1040

## Roundings

### Objectives
*   Checking the settings for rounding.
*   Allocation of roundings.
*   Defining rounding for individual partners

### Benefits
*   Values calculated by the program can be rounded to the desired number of digits.
*   The settings for rounding always refer to a certain rounding point. They can thus be finely adjusted.

### Please note

*   **Rounding rate**
    The following settings are made in the rounding record:
    *   Number of remaining decimal places.
    *   Value to be rounded to (last digit to be kept).
    *   Rounding method

*   **Rounding type**
    The rounding type defines whether rounding shall be made upward or downward.

*   **Rounding point**
    Rounding points define the object rounding. The rounding points are fixed and cannot be edited.
    Common objects of rounding are:
    *   Prices
    *   Surcharges
    *   Tax
    *   Surface

*   **Rounding Allocation**
    Rounding point and rounding have to be allocated so that the calculated value can be rounded.
    General allocations can apply to certain product groups. Special partners or partner groups can be rounded in different ways.

## Rounding

The following settings are used for calculating the rounding:
*   The rounding itself: It defines the number of digits and the rounding type, e. g. upwards.
*   The rounding point: It defines the object of rounding, e. g. price, tax, surface.

| | | | |
| :--- | :--- | :--- | :--- |
| **A** | Rounding | **C** | Rounding method |
| **B** | Digits to be rounded to | | |

*Fig. B-279: Rounding*

| Number | Name | Rounding (A) | Digits (B) | Rounding type (C) |
| :--- | :--- | :--- | :--- | :--- |
| 1 | Standard-Rundung/Standard rounding | 1 | 2 | Commercially |
| 5 | Rundung auf 0,05 / Round to 0.05 | 5 | 2 | Commercially |
| 10 | Rundung auf 0,1 / Round to 0.1 | 10 | 2 | Commercially |
| 50 | Rundung auf 0,5 / Round to 0.5 | 50 | 2 | Commercially |
| 100 | Rundung auf nächste ganze Zahl/Round 1.0 | 100 | 2 | Upwards |
| 500 | Rundung Endbetrag / Round totals | 1 | 2 | Commercially |
| 1000 | Rundung HKK / Round MCC | 1 | 5 | Commercially |
| 1001 | Rd. auf 0,01 nach oben / Round to 0. | 100 | 2 | Upwards |
| 1002 | Rundung 3NK/Rounding 3 digits | 1 | 3 | Commercially |
| 1003 | Rundung 4NK/Rounding 4 digits | 1 | 4 | Upwards |

This example shows that apart from the rounding type (C), the number of digits (B) and the value (A) the figure shall be rounded to have been defined.

There are the following rounding types:
*   **Commercial**:
    Amounts from 0 to 4 will be rounded downwards and amounts from 5 to 9, upwards.
*   **Upwards**:
    The digits from 1 to 9 will be rounded upwards.
*   **Downwards**:
    The digits from 1 to 9 will be rounded downwards.

**Tab. B-22: Rounding examples with two digits**

| Rounding value | Digits | Example value | Rounding type - commercial | Rounding type - upwards | Rounding type - downwards |
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

This example shows the results of the different rounding types.

## Rounding points

Rounding points defined the object of rounding, e.g. the price for the surface, the price for processing, the surcharge. Rounding points are fixed in A+W Business and cannot be edited.

The following table lists all rounding points used for sales price calculation. Column Description refers to the example that deals with the corresponding rounding point in the example dialogs.

**Tab. B-23: Rounding points (Section 1 of 2)**

| No. | Rounding points - sales | No. | Rounding points - purchasing | Description |
| :--- | :--- | :--- | :--- | :--- |
| 1 | sqm price/QU glass item | 51 | PP sqm price/QU glass item | Example 2 |
| 2 | sqm price/QU surcharges | 52 | PP sqm price/QU surcharges | Example 3 |
| 3 | sqm price/QU processing | 53 | PP sqm price/QU processing | Example 3 |
| 4 | Gross/pc. glass item | 54 | PP gross/pc. Glass item | Gross prices will not be shown. |
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
| 26 | Total net item per processing | 76 | PP total item net per processing | Example 3 |
| 27 | Total item net | 77 | PP total item net | Example 2 |

**Tab. B-23: Rounding points (Section 2 of 2)**

| No. | Rounding points - sales | No. | Rounding points - purchasing | Description |
| :--- | :--- | :--- | :--- | :--- |
| 28 | Total w/o VAT | 78 | Total PP | Example 1 |
| 79 | Detailed production cost calculation | | | Production price calculation |
| 118 | FC VAT 1 ** | | | Example 1 |
| 119 | FC VAT 2 | | | Example 1 |
| 128 | FC total w/o VAT | | | Example 1 |

*\* This price will not be shown. It results from net price x item quantity.*
*\*\* FC = foreign currency*

### Rounding examples

The following examples explain the allocation of rounding points and fields at document entry.
The red numbers refer to the corresponding numbers in the column of rounding points for sales and the green numbers, to the column for purchasing.

**Example 1**
*Fig. B-280: Example 1: Order – tab Totals*

The image displays the 'Totals' tab of an order, with the following fields and rounding point numbers:
-   **Order total** (28, 128)
-   **Net** (28, 128)
-   **Tax basis** for Tax 1 (18, 118)
-   **Tax basis** for Tax 2 (19, 119)
-   **Gross**

**Example 2**
*Fig. B-281: Example 2: Item entry – tab IG/article*

The image displays the 'IG/article' tab of an item entry, with the following fields and rounding point numbers:
-   **Unit price** (27)
-   **Net** (10)
-   **Item details** showing `sqm` (16/17) and `Net/pc. per glass item` (21)

**Example 3**
*Fig. B-282: Example 3: Item entry - tab BOM*

The image displays the 'BOM' (Bill of Materials) tab of an item entry, with the following fields and rounding point numbers:
-   **Net** (2/3)
-   **SPPP Net total** (11/12/22/23)
-   **Price relevant** (14/15/25/26)
-   **Supplier details** `Pce/Q/Wi/Hi` (17)

## Rounding allocation

The defined rounding and rounding points have to be allocated to each other. Allocations for product types/product groups, for clients and for partners can be defined in different ways.

The allocations made in dialog `Rounding allocation` are valid for all calculations for a client unless they are overruled by allocations for customers or suppliers.

| | |
| :--- | :--- |
| **A** | Client for which the roundings have been defined |
| **B** | Rounding point (what shall be rounded) |
| **C** | Rounding to net price |
| **D** | Reference to the rounding (value, digits, rounding type) |

*Fig. B-283: Standard allocation of roundings per client*

This example shows that in the selected line, the calculated surface price is rounded to three digits after the decimal point. This setting applies to all product types and product groups.

> **Size rounding**
> Size rounding is not affected by the settings for rounding. Size rounding is made in various dialogs for product and price definition. The program usually searches for details in the following sequence: Individual prices > Discounts > Prices > Products > Partners. The search ends as soon as details have been found.

### Rounding for partners

Apart from the general rounding allocations, other rounding records can be defined and allocated to certain customers or suppliers. For currencies the smallest monetary unit of which is 0.05, amounts will have to be rounded accordingly.

For Swiss customers, the VAT is rounded (5 centimes) for instance. This requires defining the corresponding record and allocating it to your Swiss customers.

| | |
| :--- | :--- |
| **A** | Customer for whom these settings are valid |
| **B** | Different roundings |
| **C** | Rounding to net price |

*Fig. B-284: Rounding allocation per customer*

This example shows that a special rounding shall be used for the selected customer if the product is IG. For all other products, the general rounding applies.

## Rounding allocation (Definition)

Rounding usually has to be reallocated only in case of changes, e. g. for a new customer or a new client. The following instructions describe the whole process of definition, i.e. how to define and allocate a rounding.

For instructions on this subject, please see:
*   "How to define a rounding" on page B-523
*   "How to allocate a rounding table" on page B-524

### How to define a rounding

1.  Go to menu `Master data` > `Order` > `Rounding`.
    Dialog `Rounding` appears. To change a rounding, just amend the fields in question.
2.  Go to the menu `Start` > `New` to switch to the input mode.

| | |
| :--- | :--- |
| **A** | (Descriptive) name |
| **B** | Rounding value |
| **C** | Digits |
| **D** | Rounding type |

*Fig. B-285: Fields for new rounding are accessible*

⇨ Software Reference, "Rounding" on page B-910

3.  Enter the name (A).
    Choose an expressive name, e.g. Swiss VAT.
4.  Enter the value (B) to be rounded to, e.g. 0.05.
5.  Enter the number of digits (C), e.g. 2.
6.  Choose the rounding type (D), e.g. commercial.
7.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved. You can select this rounding now for all generally applicable rounding allocations or for partner-related rounding allocations. It is called `Rounding table` in the dialogs in question.

The following example describes the allocation for a customer. The steps are the same for suppliers and partner groups as well as for general rounding allocation, e.g. for a new client.

### How to allocate a rounding table

1.  Go to menu `Master data` > `Partners` > `Customer` > `Rounding`.
    Dialog `Rounding` appears. If rounding allocations have already been made for customers, these are displayed.
2.  Go to the menu `Start` > `New` to switch to the input mode.

| | |
| :--- | :--- |
| **A** | Customer to whom this rounding is applied |
| **B** | Rounding point |
| **C** | Product type / Product class |
| **D** | Price unit |
| **E** | Rounding table |
| **F** | Alternative rounding allocations |

*Fig. B-286: Fields for the new rounding allocation are accessible*

⇨ Software Reference, "Rounding" on page B-910

3.  Choose the customer (A).
4.  Choose the rounding point (B), e.g. `VAT 1`.
    You have now defined that VAT 1 shall be rounded. If a second tax rate is applicable for the customer, this will not be rounded.
5.  Choose the product type (C) and price unit (D).
    If you choose e.g. `<n.e>`, the settings will always be valid for this customer.
    In this example, the VAT rounding is specified. The price unit is therefore irrelevant.
6.  Select the rounding table you have drawn up for this customer, e.g. 0.05.
7.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved. The new rounding will be applied to the selected customer. For all other rounding points, the general rounding allocation will still be valid for him.

## Exercises

*   Check the existing rounding settings and rounding allocations.
*   Allocate the following rounding to your training client:
    *   All glass items shall be commercially rounded to three digits.
    *   All unit prices shall be rounded to 0.05. Enter this rounding if there is no corresponding entry in dialog `Roundings`.
*   Allocate to your training customer a commercial rounding of VAT to 0.05.

### Additional information
⇨ Software Reference, "Rounding (Customer, Supplier)" on page B-876
⇨ Software Reference, "Rounding for Customer/Supplier Groups" on page B-876
⇨ Software Reference, "Rounding" on page B-910
⇨ Software Reference, "Rounding Points" on page B-912
⇨ Software Reference, "Rounding Allocation" on page B-913

## Settings for Invoicing

Apart from the settings for pricing in the dialogs for prices, partners, discounts, and rounding, further data are required for the processing of documents, e. g. for payments and VAT calculation.

This chapter shows you how to edit the appropriate settings.

This includes the following training modules:
*   "Finance" on page B-528
*   "Automatic Surcharges" on page B-394

An invoice must include at least the following elements:
*   **Details on the issuing party**
    *   Company name and address
    *   Tax number and/or VAT ID
    *These settings are made in dialog `Company Data`.*

*   **Details on the recipient (customer)**
    *   Name and address
    *These settings are made in dialog `Partner Management`.*

*   **Details on the delivery/service**
    *   Delivery date
    *   Quantity and description of the products delivered
    *   Net amounts, broken down by tax rates if required
    *   Tax
    *   Date of issue (= invoice date)
    *   Unique invoice number
    *These details are part of the order.*

Apart from that you can - among other things - enter bank accounts for printing bank transfer forms and payment terms, manage currencies, and define tax rates.

## Finance

### Objectives
*   Introducing basic data dialogs for accountancy.
*   Checking and defining the settings for payment terms.

### Benefits
*   All data required for commercial accounting and for financial accounting are entered as basic data and are allocated to the partners and products. These data are therefore entered only once, and are maintained centrally.

### Please note

*   **Tax Rates**
    *   Taxes can be calculated only if they have been defined as tax rates.
    *   Tax rates are allocated to the products and the partners. They can be changed in the documents.

*   **Currencies**
    *   Prices can be kept in different currencies.
    *   Orders can be entered in national currency or foreign currency.
    *   For statistical comparison, your home currency will be used always. The amounts are converted by A+W Business for this purpose.

*   **Banks**
    *   Based on the (complete) bank data, the IBAN can be determined in partner master data.

*   **Payment conditions**
    *   Payment terms are allocated to the partners. They can be changed in the documents.

*   **Foreign key**
    *   In the dialogs in which data for accounting are entered, an external key refers to the corresponding booking fields in the financial accounting program (FinAcc).
    *   The entry for the external key depends on the corresponding financial accounting system.

## Taxes

Tax rates have to be entered for calculating the tax in documents. These tax rates are allocated to the products and partners.

| | |
| :--- | :--- |
| **A** | Percentage of tax |
| **B** | Revenue account debtors, creditors |
| **C** | External key (based on FinAcc program) |

*Fig. B-287: Tax Rates*

| Price key | Tax rate | Comment | Pr.acc.Debt. (B) | Pr.acc.Cred. (B) | External key (C) | Locked |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 19.0000 | 19% Inland/Home tax | 8201 | 9201 | | ☐ |
| 2 | 0.0000 | 0% Ausland/Foreign... | 0 | 0 | | ☐ |
| 3 | 10.0000 | 10% Test | 0 | 0 | | ☐ |
| 4 | 16.0000 | 16% Inland/Home tax | 0 | 0 | | ☐ |

You can enter any number of tax rates. Only the first five of them can be allocated in product and partner master data however. The additional tax rates are also available in the documents.

If you are using revenue accounts (B), the tax amounts will be booked to the revenue account of the corresponding product group by default. To book the tax amounts to the revenue accounts for tax you have to enter the account numbers for creditors and debtors according to the financial accounting system (FinAcc).

## Currencies

As an international company you have to handle more than one currency. You can maintain sales and purchase prices in A+W Business even if they occur in different currencies. For your customers, prices can be stated in foreign currency on the orders.

At order entry, A+W Business can use two different currency settings:
*   **Home currency**: The currency of the country in which headquarters are located. In Europe, this is usually Euro now.
*   **Foreign currency**: The currency that differs from the home currency, e.g. the currency in which prices are shown in orders for foreign customers.

For statistical comparison, your home currency will be used always. The amounts are converted by A+W Business for this purpose.

The options for price management and calculation in the orders are:
*   Price lists and orders are kept in home currency.
*   Price lists are kept in home currency; for foreign customers, the amounts can be shown either in home or foreign currency. For this, you have to enter and update the exchange rates for the foreign currencies.
*   Price lists are kept in foreign currency; the amounts in the orders can be shown in national or foreign currency. The exchange rate is defined for internal purposes.

The currency to be used as a basis for calculation as well as the currency in which orders are entered are both defined in company data.

| | |
| :--- | :--- |
| **A** | Currency used for calculation by A+W Business |
| **B** | Default settings for order entry |
| **C** | Currency for displaying prices in the order |

*Fig. B-288: Company data – tab tax, currency settings*

This example shows that the national currency (A) is Euro. The national currency is usually chosen as the standard setting (B) for order entry. If you are using price lists in another than the national currency, select the setting `Euro` for displaying prices (C) at order entry.

### Pricing in connection with foreign currency

Price calculation with foreign currencies can produce different results if prices for quantities are calculated on different levels. This setting is made in company data.
⇨ Software Reference, "Calculate foreign currency amount from unit price x quantity" on page B-974

If the foreign currency amount shall result from the BOM and the quantity, the amounts can be calculated in the following ways.

*   The item price is the item price in national currency.

    | NC price/PU | x Factor | = FC price/PU |
    | :--- | :--- | :--- |
    | NC gross unit price | x Factor | = FC gross unit price |
    | NC net unit price | x Factor | = FC net unit price |
    | **NC item price** | **x factor** | **= FC item price** |
    *Legend: NC = national currency, PU = price unit, FC = foreign currency*

*   The item price is created from the net price in foreign currency.

    | NC price/PU | x Factor | = FC price/PU |
    | :--- | :--- | :--- |
    | NC gross unit price | x Factor | = FC gross unit price |
    | NC net unit price | x Factor | = FC net unit price |
    | **FC net price/pc.** | **x qty.** | **= FC item price** |
    *Legend: NC = national currency, PU = price unit, FC = foreign currency*

### Exchange rates

Exchange rates are entered in dialog `Currencies`. If one of the defined currencies shall not be used any longer, it can be locked.

| | |
| :--- | :--- |
| **A** | Exchange rate for foreign currency |
| **B** | Name of currency |
| **C** | Lock currency |

*Fig. B-289: Currencies*

The intensity in which the exchange rates are kept depends on the conditions in your company.
With certain customers you can agree special conversion factors which are stated in the order. In this case, the prices of the order will not be calculated using the defined conversion factor but with the factor defined for this order.

**Additional information**
⇨ Software Reference, "Tax" on page B-928
⇨ Software Reference, "Payment Conditions" on page B-930
⇨ Software Reference, "Banks" on page B-932
⇨ Software Reference, "Currency" on page B-932
⇨ Software Reference, "Currency settings" on page B-944
⇨ Software Reference, "Show currency at order entry" on page B-945

## Printing of Text and Documents

You can enter standard text for documents which can be printed in various documents as required.

In this session we are going to introduce the available text modules show you how to control the printing of forms.

This includes the following training modules:
*   "Text" on page B-534
*   "Forms" on page B-545

## Text

### Objectives
*   Introducing the different text types for automatic text.
*   Introducing the function of text codes.
*   Using text variables.
*   Entering and editing text.

### Benefits
*   Frequently required text modules can be entered and saved to be used in documents without having to key in the text word for word.
*   Variables complete a text based on the entries made in the document.

### Please note

*   **Text Types**: Automatic text is distinguished by its use:
    *   System text
    *   Standard texts
    *   Spacer text
    *   Reminder text
    *   Quality text
    *   CEKAL text
*   **Text identifier**: By means of the text code, text modules are inserted in documents and/or transferred to the interfaces (production, FinAcc).
*   **Variables**: Variables (wildcards) can be inserted in the text. These variables are then replaced by actual values in the document.
*   **Formulas**: Variables can be combined in formulas in order to calculate a value in the document.

### Text types

Recurring text can be saved, e.g. to be included in the document automatically. We distinguish system-, default-, and spacer text.

You can also enter text for reminders which can be linked with a reminder fee.

#### System text
These text modules are fixed. You cannot enter new system text or delete existing system text.

| | |
| :--- | :--- |
| **A** | Text number |
| **B** | Variable wording |

*Fig. B-290: System text*

You can change the wording of system text by analogy, e. g. by adjusting the standard in text 111.

#### Standard texts
Text frequently used in documents can be defined as standard text. This text can be entered, selected, and/or edited in different dialogs:
*   In management of forms, the defined text can be firmly assigned to a form.
*   Customer- or supplier-related text can be entered or firmly assigned in partner management. When a document is entered, this text will be displayed automatically and can be edited.
*   At order entry and item entry you can select existing text modules or enter order-, item-, or product-related text.

#### Spacer text
You can enter special spacer text for every IG unit, and allocate them to the product.

There are two types:
*   Variables (wildcards) are entered in the standard text so that the spacer text is created from the entries in the document.
    Text based on those variables can consist of up to 80 characters.
    This option requires that the spacer bender permits the transfer of text.
*   A fixed number is transferred to the spacer bender for every IG unit. In this case, the standard text includes only the spacer number for the spacer bender. This number is allocated to the product. Based on this number, the spacer bender will automatically insert the right text.

#### Reminder text
The spacer text can only define how the customer shall be reminded, e. g. without reminder text, normal, severely, etc. The code is transferred to financial accounting.

#### Quality text
The requirements regarding quality text vary from country to country. This text is entered with the necessary details.
If you enter an IG unit in an order, the product, gas, and product type or product group will be checked. Based on the the country code in the delivery address, the appropriate quality text will be added to the spacer text.
If an IG unit includes two lites for which quality text has been entered, the priority defined will decide which of them shall be printed on the spacer.

#### CEKAL
In France, CEKAL-certified IG units have to meet certain quality criteria.
To be able to adjust the CEKAL standards in case of changes, the current CEKAL standards are not fixed in A+W Business. They can be defined at random.
When you enter an IG unit, the CEKAL text will be created based on the defined rules. It can be changed in the order. This text can be used in the following way:
*   Print CEKAL text on forms, labels, and work orders.
*   Transfer CEKAL text to production for the spacer bender.

### Text codes and standard text
Standard text is distinguished by means of text codes, e. g. text code Q for quotations, P for production, D for delivery note. Text codes can be entered according to your company's requirements.

**Examples**
*   **Info text (text code /):**
    Shall be printed on all documents, e.g. to announce company holidays.
*   **Delivery note text (text code D):**
    To be printed only on delivery notes, e.g. deadlines for complaints.
*   **Quotation text (text code O):**
    This text shall only be printed on quotations, e. g. validity of the quotation.

Text codes are not only used for grouping your standard text. The text code defines which text shall be printed on the individual documents or shall be transferred to production.

**Example**
Production text (text code P) shall not be printed on delivery notes. In management of forms you can define - for every form - the text codes that shall not be printed.
This function is described in a separate chapter.
⇨ "Form management" on page B-546

When you select the text by hand in a document, the code can be used as a filter criterion.

| | |
| :--- | :--- |
| **A** | Text numbers |
| **B** | Text identifier |
| **C** | Defined text |
| **D** | List of standard text for quotes |

*Fig. B-291: Default texts*

For every text code (B) you can enter any number of text modules (D). Each text is marked by a special number (A).

Allocate the text numbers in blocks based on the text codes, e.g. numbers 1 to 199 for code O, 200 to 299 for code I, 300 to 399 for code P.

The text modules can be inserted in documents and can then be edited. Blanks will be added by hand or will be filled by variables.

| | |
| :--- | :--- |
| **A** | Selected text |
| **B** | Defined text |

*Fig. B-292: Standard text in the quote*

In this example, the date has to be added by hand in the text of the quotation.

Text can be entered in the following dialogs:
*   `Partner management` > tab `Text`
*   `Product management` > tab `Text`
*   `Document management` > tab `Text`
*   `Items` > tab `Text`

## Variables

General text and system text can be entered with variables. These serve to enter the appropriate data when the document is issued.

**Example**
The date is usually represented by a wildcard. It is loaded from the system date and entered when the document or file is issued.
Variable `<d1>` is automatically replaced in the document by the date `Valid from` and variable `<d2>`, by the date `Valid until`.

| | |
| :--- | :--- |
| **A** | Text with variables |
| **B** | Variable |

*Fig. B-293: System text*

Variables are used in connection with:
*   Processing text
*   Product definition
*   Spacer text, CEKAL text
*   Export files

## Formulas

In the text, variables can be combined in formulas where a parameter is determined by means of the details in document.

*Fig. B-294: Text and formula in product definition*

This example shows the formula for determining the edge length. This formula should be read as follows:
*   `<%"`: number of edges
*   `<§>`: edge numbers
*   `<=>`: total length

For a lite of the size 1200 x 1800 mm this means: 4 edges = 6000 mm total length to be processed.

Based on the number of edges, the following text will appear in the order:

*Fig. B-295: Example order item (2 or 4 edges arrissed)*

The total length depends on the edges to be processed.

The definition of such a formula is supported by explanations which also point out the valid variables.

| | |
| :--- | :--- |
| **A** | Represents the symbol `=` |
| **B** | Represents the symbol `§` |
| **C** | Represents the symbol `%` |
| **D** | Formula |

*Fig. B-296: Formula and parameters for the processing step 'arrissing'*

This example for the processing step Arrissing shows the available variables (A to C). The text (D) between the variables (in pointed brackets) can be entered at random.
The formula is: (number of edges) * (edge length) = (total length)

Only the parameters valid for the corresponding processing step(s) will be listed.
⇨ "Available variables (wildcards)" on page B-597
⇨ Software Reference, "System Text" on page B-1064

## File Attachment

You can also attach files to an order, e. g. with details on the calculation or regarding shapes. Codes are used to define the file attachments to be passed on, e.g. to production.

File attachments will be passed on in the following cases:
*   **Transfer to production**:
    File attachments for transfer in OrderXML, e. g. product information.
*   **Copy documents**:
    Quotation to order, e.g. calculation information.
*   **P.O. transfer**:
    e.g. product information.

| Code | Name |
| :--- | :--- |
| A | All |
| P | Production |

*Fig. B-297: File attachment types*

Standard code A shows that all file attachments will be transferred. The only exception is P.O. transfer.

As for text codes, the codes for these file attachments can be defined, e.g. P for production, O for quotes.

The settings for the transfer of file attachments are described in the sections Sales and Production.

## Text input

You can enter standard texts to be offered for selection, e.g. at order entry.

For instructions on this subject, please see:
*   "How to enter standard text" on page B-543
*   "How to enter customised text" on page B-132

> **Prerequisite**
> Text can be entered completely only if the text codes have been defined. These are entered in dialog Text codes as described in Tutorial 1 for basic tables.

### How to enter standard text

1.  Go to menu `Master Data` > `Text` > `Text`
    The dialog for entering standard text appears.
2.  Go to the menu `Start` > `New` to switch to the input mode.

| | |
| :--- | :--- |
| **A** | Freely-selectable number |
| **B** | Matchcode |
| **C** | Text identifier |
| **D** | Text input |

*Fig. B-298: Fields for new text are accessible*

⇨ Software Reference, "Text" on page B-1064

3.  Enter the number (A).
    Please stick to the number blocks you have reserved for the codes.
4.  Enter the matchcode (B).
    The matchcode should include a catchword from the text.
5.  Select the text code (C), e.g. `I Info text`.

The text code defines the documents in which the text can be selected and printed.

6.  Enter the desired text in the input field (D).
    The settings for the fonts and the type size only apply to the display on screen. They will not be used for printing.
7.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved. The text can now be allocated in documents, partner management, and product management.

> **Foreign-language texts**
> Add the translations in the corresponding languages in the same way. To avoid mix-ups you should choose the same text number as for the original text.

### Additional information
⇨ Software Reference, “Product Management - Text" on page B-693
⇨ Software Reference, "Partner Management - Text" on page B-819
⇨ Software Reference, "Text" on page B-1064

## Forms

### Objectives
*   Introducing the function of forms.
*   Checking the settings for printing prices and sketches.
*   Adjusting the settings for printing forms.
*   Defining direct printing and print jobs.

### Benefits
*   Documents are printed on forms in different formats.
*   The printouts can be adjusted to a certain extent.

### Please note
*   **Print item**: Print points are points in the program at which a document can be printed.
*   **Status**: Printing a document will raise its status. The document can reach the 'original printout' status just once. After that, printing can just be repeated.
*   **Form**: Forms are fixed files adapted to the company's layout. Documents can be printed only if at least one form has been defined for the print points. You can define several forms for every print point.
*   **Direct Printing**: Different settings can be made for the five document types; these can be used for printing a document without opening the dialog `Printing of forms/labels`.
*   **Print Job**: If printing is started from a central print server, print jobs can be defined for automatic printing.

## Form management

Documents are printed on forms. The forms for printing order confirmations, invoices, etc. are created with your company's standard layout and are available in different languages. Apart from the forms for the documents, forms for printing labels and for exporting data are defined. These two functions are described in detail in section Sales.

### Print item

Print points are points in the program at which a document can be printed. These print points are matched by a status (point) each to which the printed document is set. We distinguish the output via printer, fax, or email.

Print points are defined for the original printout and repeated printing. This means that just one original copy can be printed per document and print point. Repeated printing can be repeated as the term implies.

**Examples**

| Code | Type | Name |
| :--- | :--- | :--- |
| 100 | 2 (order) | Print order confirmation |
| 101 | 1 (quotation) | Print quotations |
| 102 | 2 | Print delivery note |
| 103 | 2 | Print invoice |
| 104 | 3 (credit note) | Print credit note |
| 105 | 2 | Print complaint |
| 106 | 5 (P.O.) | Print P.O. |
| 107 | 4 (inquiry) | Print inquiry |
| 108 | 2 | Print work order |
| ... | | |
| 200 | 2 | Repeat printing of order confirmation |
| 201 | 1 | Repeat printing of quotation |
| 202 | 2 | Repeat printing of delivery note |
| 203 | 2 | Repeat printing of invoice |
| 300 | 2 | Print fax order confirmation |
| 350 | 2 | Print email order confirmation |
| 400 | 2 | Repeat printing of fax order confirmation |
| 450 | 2 | Repeat printing of email order confirmation |

This list shows some of the print points. For every document type, print points are defined which allow printing of the original and repetitions in the different output formats.

Each print point must be allocated to at least one form.

### Allocation of forms

A print point can be allocated to any number of forms. These allocations are made when the program is installed and usually require no changes. You can allocate further forms however. These forms have to be saved as template files in `*.qrp` format.

| | |
| :--- | :--- |
| **A** | Flag for the standard form |
| **B** | Actual print point |
| **C** | Number of copies |
| **D** | File name of the form |
| **E** | Status diversion, e. g. cash sale |
| **F** | List of allocated forms |

*Fig. B-299: Allocation of forms*

This example shows the forms (F) allocated to print point `Print OC` (B). The selected form is the standard form (A) of which one copy (C) is printed.

Each form can be allocated a different status point (E). This allocation is usually only necessary for a cash sale form. Select the alternative status point `Cash sale`. If no different status point is entered, printing will change the document status to the status matching the print point.

### Printing

When printing forms, only the forms allocated to the document type in question will be offered for selection.

| | |
| :--- | :--- |
| **A** | Select the form |
| **B** | Document status after printing |
| **C** | Select the print mode |

*Fig. B-300: Print order from number manager*

The documents of a number manager are printed according to the settings for the print mode (C) and the form (A).

You can set the following print methods:
*   Direct Printing
*   Print jobs

These methods are described in separate chapters.
⇨ "Direct printing" on page B-557
⇨ "Print jobs" on page B-558

### Output format

All documents can be printed in different formats on the defined forms:
*   Print on paper
*   PDF
*   RTF
*   E-mail
*   Fax
*   XML

The format you choose depends on the purpose for which the document shall be printed.

For all documents you want to send electronically you have to make sure that the recipient will be able to read them.

**Example**
Emailing a PDF file requires that the recipient has installed a so-called viewer that allows to open and read the document, e.g. Acrobat Reader. This document format is best suited if you want to include shape sketches or grills in the document.

### Adjust the printout

The printout can be adjusted to a certain extent. Apart from the headers and footers you can adapt e. g.:
*   Printing of sketches, prices, product names, etc.
*   Text codes for text not to be printed.
*   Paging
*   Default printer

The settings for printing sketches and prices are made in different dialogs. These settings are describe in separate chapters.
⇨ "Printing prices" on page B-550
⇨ "Printing sketches" on page B-552

## Printing prices

Printing of prices on forms is defined at different points which may influence each other:
*   **Management of forms**: The settings are generally applicable and define whether the definition shall be adopted from the document.
*   **Partner management**: The settings define how detailed the prices shall be printed. These settings can be changed in the document.
*   **Product management**: These settings define whether the prices shall be shown implicitly or explicitly, e. g. for BOM elements.
*   **Document management (order)**: The settings define how detailed the prices shall be printed. The settings will be adopted only if the settings in management of forms permit this.

### Management of forms: Settings for printing prices

Management of forms settings offers the following options:
*   **0 - Standard** or **2 - Print prices always (totals mode)**:
    Printing of forms will use the details defined in the document:
    *   **0 - No printing**: Prices will not be printed.
    *   **1 - All prices**: Prices are printed per order item.
    *   **2 - Totals only**: Only item totals will be printed.
*   **1 - Always print prices**: The settings made in the document will be ignored. Prices will be printed per order item.

| | |
| :--- | :--- |
| **A** | Tab Options 1 |
| **B** | Printing of prices |

*Fig. B-301: Settings for printing prices*

### Printing of item prices and totals

Printing of prices is controlled by management of forms and the document settings.

| Settings | | Printing | |
| :--- | :--- | :--- | :--- |
| **Document** | **Management of forms** | **Item prices** | **Totals** |
| 0 | 0 | - | - |
| 1 | 0 | X | X |
| 2 | 0 | - | X |
| 0 | 1 | X | X |
| 1 | 1 | X | X |
| 2 | 1 | X | X |
| 0 | 2 | - | X |
| 1 | 2 | - | X |
| 2 | 2 | - | X |

**Legend:**
*   **Documents**
    *   0 = no printing
    *   1 = all prices
    *   2 = only totals
*   **Management of forms**
    *   0 = Standard (document decides)
    *   1 = Print prices always
    *   2 = Print prices always (totals mode)
*   - = no printing, X = print

**Example**
If `Print totals (2)` is set in the document and `Standard (0)` in management of forms, only totals will be printed, no item prices.

## Printing sketches

When printing sketches, shape and grill sketches are distinguished. The display and printing of sketches are defined in different dialogs:
*   **Company data**: The settings define how grill sketches shall be printed by default.
*   **Management of forms**: The settings define details for printing sketches of shapes and grill patterns.
*   **Product management**: These settings define for shapes and grill patterns whether sketches shall be printed. You can choose between true-to-scale and schematic display.
*   **Item entry**: The settings are made separately for shapes and grill patterns and define whether and how sketches shall be printed. You can choose between true-to-scale and schematic display per item.

| | |
| :--- | :--- |
| **A** | Print mode (shapes, grills) |
| **B** | Display size |
| **C** | Text size on shape sketches |
| **D** | Scale for grill sketches |

*Fig. B-302: Management of forms – Settings for printing sketches*

In management of forms you can enter the settings for printing shape and grill sketches. This can be differentiated further by choosing true-to-scale or schematic display (A). You can also define the size of the printed sketch (B).

If shape sketches are printed true to scale, the sizes are also shown on the sketch. The position of the sizes on the sketch can be edited in the pattern so that these will be clearly legible on the printout.

> **Curved glass**
> The curvature of curved glass will always only be shown schematically.

### Printing of grill sketches (rectangular lites)

| | Settings in management of forms | | |
| :--- | :--- | :--- | :--- |
| | **no printing** | **schematic** | **true to scale** |
| **Item settings** | **true-to-scale grill** | no printing | no printing | true-to-scale grill |
| | **schematic grill** | no printing | schematic | schematic grill |
| | **no printing** | no printing | no printing | no printing |

### Print sketches of shapes

| | Settings in management of forms | | |
| :--- | :--- | :--- | :--- |
| | **no printing** | **schematic** | **true to scale** |
| **Item settings** | **true-to-scale shape** | no printing | schematic | true to scale |
| | **schematic shape** | no printing | schematic | schematic |
| | **no printing** | no printing | no printing | no printing |
| | **true-to-scale grill** | no printing | no printing | no printing |
| | **schematic grill** | no printing | no printing | no printing |

These tables show that grills on a rectangular lite will be printed true to scale only if true-to-scale printing has been set both in the document and in management of forms.

For printing grill patterns you have to enable the function `Extended grill sketch` for printing of forms in company data.

This table shows that shapes will be printed true to scale only if true-to-scale printing is set in the document as well as in management of forms.

Printing of shape sketches is enabled or disabled in general in management of forms, tab `Options 1`.

Shape sketches will always be printed on a separate page.

### Print dimensioned sketch

Module Documents allows printing dimensioned sketches. You can select the function `Extended shape sketch` to print true-to-scale sketches of shapes and grills on a separate page.

Dimensioned sketches can only be used if this function is enabled in company data.

*Fig. B-303: Company data – Print tab (Shows `Extended Georgian bar sketch on printed forms` checkbox)*

The dialog `Print dimensioned sketch` only shows those items for which printing of sketches for shapes and grills has been set to true to scale.

| | |
| :--- | :--- |
| **A** | Select items with grills |
| **B** | Select items with shapes |
| **C** | Grill details |
| **D** | Product sketch |

*Fig. B-304: Print true-to-scale sketches*

The buttons (A) and (B) can be used for selecting the items which include grills (A) or shapes (B).
If you have enabled the details for grills (C), the bill of material and details on the grills will also be printed.

| | |
| :--- | :--- |
| **A** | Grill sketch |
| **B** | Grill cutting list |
| **C** | Shape sketch |

*Fig. B-305: Examples for the printing of dimensioned sketches*

The product sketch is attached as a file to the product. In product management, you can attach one image to every product as an attachment. This image can only be printed if the checkbox `Print on form` is ticked in product management.

*Fig. B-306: Product management - example for article sketch*

This image shows the product itself. It shows neither the shape nor any fitted grills. It is therefore only useful for rare patterned glass types.

The image can also be printed on forms. For this purpose, the checkbox must be ticked.

## Direct printing

When printing individual documents you can define settings for the so-called direct printing. All settings for direct printing are fixed so that no intervention is required.

| | |
| :--- | :--- |
| **A** | Standard print functions |
| **B** | Direct Printing |

*Fig. B-307: Direct printing in the order*

The settings are made in the `Order forms` dialog.

| | |
| :--- | :--- |
| **A** | Document type for which direct printing has been defined |
| **B** | Print point started by direct printing |
| **C** | Form |
| **D** | Check before printing |
| **E** | List of defined direct printouts |

*Fig. B-308: Allocations for direct printing*

This example shows that several allocations (E) for direct printing can be made for the same document type (A). When printing right from the document, manual entries are not required. If printing is started without checking (D), dialog `Printing of forms/labels` does not appear. The print job is transferred to the selected printer right away.

Allocations for direct printing can be defined for the following document types:
*   Quotation
*   Order including order confirmation, delivery note, invoice, complaints, etc.
*   Credit note
*   Purchase order request
*   P.O.

## Print jobs

You can define print jobs is you are using a central print server. One or more documents can be allocated to a print job. The print server will process these print jobs in the sequence shown on the list, e.g.:
*   Printing order confirmations for internal purposes.
*   Faxing of order confirmations as repeat printout.
*   Repeated emailing of order confirmations to the salesman.

| | |
| :--- | :--- |
| **A** | Name of the print job, document type |
| **B** | List of print jobs |
| **C** | Settings for collective printing |
| **D** | Settings for dispatch |

*Fig. B-309: Print job*

Every print job refers to a certain document type and can only be started for this type. The fields for the print settings (D) are released according to the form.

After each print run, the document status is raised. The sequence (B) of print runs therefore has to match the allocated status. If e.g. invoices can only be printed after the delivery note has been printed, the print run for the delivery note has to precede the print run for the invoice.

If collective printing (C) of invoices is defined in the print job, the option `Collective printing` must be enabled in customer master data. A collective invoice includes all orders from a customer for which the corresponding code has been set. Printing can be defined further:
*   **Always**:
    This setting overrides the collective printout setting made in the master data.
*   **By P.O. text 1**:
    All documents for a customer are filtered by P.O. text 1 and combined. If there are 10 orders from a customer, for example, five of which have the same P.O. text 1, six order confirmations will be printed.
*   **By shipping address**:
    All documents with the same shipping address will be combined.
*   **Standard**:
    All documents for the same customer or supplier are combined if the code for collective printout has been set.

The printing of collective invoices is described in detail in section Sales.
⇨ Sales, "Printing of collective invoices" on page C-1149

> **Printer name must be known**
> When defining print jobs, the printer must be available on the server. It has to be installed on the client as well.

## Definition of direct printing

Settings for direct printing can be made for every document type.

### How to define direct printing

1.  Go to menu `Master Data` > `Forms` > `Order forms`.

| | |
| :--- | :--- |
| **A** | Name of direct print job |
| **B** | Document type, print point |
| **C** | Printer |
| **D** | Form for direct printing. |
| **E** | Show print dialog |

*Fig. B-310: Fields for new direct print job accessible*

⇨ Software Reference, "Order Forms" on page B-1083

2.  Go to the menu `Start` > `New` to switch to the input mode.
    The fields are preset by the selected direct print job.
3.  Enter the name (A).
    Enter the name so that it is clear to see whether this is the first printout or a repeated printout, e. g. `quotation (RP)` for the repeated printing of quotations.
4.  Choose the document type and the print point (B) for which the direct print job shall be used.
    Make sure that the print point matches the selected document type. Should you choose the wrong print point by mistake, the document cannot be printed.
5.  Choose the printer (C) for the direct print job.
    The selection shows all printers installed on the computer in question. If the server printer is not listed you will have to install it, or have it installed.
6.  If necessary, choose the form (D) for the print point.
    This selection has to be made only if several forms are allocated to the print point.
7.  Tick the checkbox (E) if required.
    When the checkbox is ticked, the dialog `Printing of forms/labels` also appears when you call direct printing.

*Fig. B-311: Settings for direct printing have been made*

8.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved and the list is updated. This direct print job is now available in the quotation.

## Entering a Print Job

A print job includes several print runs. When sorting the print runs, you have to obey the sequence of status allocation. The delivery note for example can also be printed after the order confirmation on the print server.

For instructions on this subject, please see:
*   "How to enter a print job" on page B-562
*   "How to add print runs" on page B-564

Most of the following settings for printing via server cannot be changed while printing.

### How to enter a print job

1.  Go to menu `Master Data` > `Forms` > `Print jobs`.
    Dialog `Print jobs` appears.
2.  Go to the menu `Start` > `New` to switch to the input mode.

| | |
| :--- | :--- |
| **A** | Name of the print job |
| **B** | Document type |

*Fig. B-312: Fields for the new print job are accessible*

⇨ Software Reference, "Print Jobs" on page B-1083

3.  Enter the name (A).
    Choose the name so that the use of the print job becomes quite clear. In this example, a print job for repeated printing of delivery notes and invoices is defined.
4.  Choose the document type (B).
    In this document, `Order` is selected.
5.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved. You can now add print runs and make the settings for printing.

> **Selecting a print job**
> From the list of `Print jobs` you can select the print job to be edited. If the new print job is not displayed yet, just close the dialog and open it again so that the new data can be loaded.

### How to add print runs

1.  Select the print job to which a print run shall be added.

| | |
| :--- | :--- |
| **A** | Select the form |
| **B** | Select the printer |
| **C** | Select print jobs |
| **D** | Forms in the print run |
| **E** | Add a print run |
| **F** | Delete the print run |

*Fig. B-313: Fields for new print runs are accessible*

2.  Click on `[Add]` (E).
    The fields in section `Form selection` are accessible.
3.  Choose the form (A), e.g. `OC RepPrint`.
    The form appears on the list (D).
4.  Choose the printer (B).
    Make sure to choose the right network printer.
5.  Repeat steps 2 to 4 to add more print runs.

| | |
| :--- | :--- |
| **A** | Setting for the document number |
| **B** | Settings for printing |
| **C** | Sort print runs |
| **D** | List of print runs in the print job |

*Fig. B-314: Collect print jobs*

6.  Use the arrow keys to sort the print runs on the list (C) in the sequence matching the status allocation.
7.  If required define the details (B) for printing per form.
    The available settings for the print job depend on the selected form. They are valid only for this form.
    The number (A) for the documents can be loaded from the number ranges of the order areas or from that of the clients.
8.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved.

### Additional information
⇨ Software Reference, "Shape sketch, grill sketch" on page B-676
⇨ Software Reference, "Company Data > Documents" on page B-952
⇨ Software Reference, "Company Data - Print" on page B-1005
⇨ Software Reference, "Forms" on page B-1068
⇨ Software Reference, "Form Management" on page B-1068
⇨ Software Reference, "Order Forms" on page B-1083
⇨ Software Reference, "Print Jobs" on page B-1083
⇨ Sales, "Print" on page C-1311

## Complex Exercise

The following tasks are based on the sessions in Tutorial 1 and Tutorial 2.
*   Create a new calendar for the following year.
*   Enter two new price keys with a validity of 90 days, one for sales and one for purchasing.
    You are going to use them as rates for the following tasks!
*   Enter a laminated glass product with the processing step `Grinding`.
    Please check for which of the BOM elements the processing step has been defined.
*   Enter an IG product in which the formerly defined laminated lite is one of the lites.
    Please make sure that the procurement type for this glass is correct.
*   Enter the price tables for calculating the purchase and sales prices of the new products. Define them for your new rate.
*   Enter a customer with the following data:
    *   Route
    *   Payment conditions
    *   Lorry and driver
*   Enter a project for this customer.
    In this rate, enter a new price list for this project and allocate it to the customer.
*   Enter an order with your IG unit.
    The order has to refer to the project and should automatically show the appropriate price.
*   Check the project status in master data.
*   Enter a new employee. He shall be entitled to enter orders and transfer them to production.

## Additional Information

This section provides additional information on Tutorial 1 and 2. These are mainly technical details regarding calculations and lists of fixed settings.

*   "Project/invoice management" on page B-568
*   "Available document types" on page B-592
*   "Available limit types" on page B-593
*   "Available system text" on page B-596
*   "Available variables (wildcards)" on page B-597
*   "Patterns for leaded designs" on page B-600
*   "Monitoring of changes" on page B-601
*   "A+W Production" on page B-604
*   "Mixed calculation" on page B-607
*   "French pricing" on page B-608
*   "Calculation" on page B-609

## Project/invoice management

### Objectives
*   Introducing versions of project management.
*   Working with projects.

### Benefits
*   Special project conditions will be used automatically for the term of the project.
*   Several orders can be issued for a blanket order until the agreed surface, quantity, or total is reached.

### Please note
*   **Object**: A project is a specific building project in which several customers and suppliers can be involved. For every building project, a project is defined and allocated to the partners involved.
*   **Customer project**: A project can be mentioned in an order only if it has been allocated to the customer in question. Different sales representatives and payment terms can be stated in the customer project. Once marked as completed, a project cannot be used any longer.
*   **Blanket order**: A blanket order refers to a customer who places on call orders from an agreed total quantity and/or total.
*   **Partial invoice**: Work orders and partial invoices can be issued for blanket orders.
*   **Invoice management**: In the course of invoice management you can enter claims, hours required and purchase requirements which are allocated to an order. Projects cannot be used in connection with invoice management.
*   **Default settings**: Company data: Tab `Documents` > `Project Management`.

> **Previous knowledge**
> Please note that the sequence of necessary steps is described only in brief here for those steps that have been described in closer detail in other parts of the A+W Business documentation.

### Versions of project-/invoice management
There are different modes of working with projects and invoicing orders and purchase orders.
*   Projects are specific building projects for which special terms are valid for orders and/or purchase orders.
*   Blanket orders can be managed independent of building projects. The general terms for this are defined in a blanket order. Individual work orders can be issued for a blanket order until the totals defined in the blanket order are reached. The individual work orders are settled by means of partial invoices.

The required invoice management (project management) version must be enabled in company data.

The different modes offer the following functions:
*   **Standard project management**: In this mode, a project can be allocated to a business partner. When the project is mentioned in the document, the terms allocated to this project will be used for pricing.
*   **Extended project management**: Extended project management allows entering additional details on the salesman and the payment terms. These details will be used for the order if the project is allocated to this order.
*   **Standard project management + invoice management with allocated orders**: This mode links project management and invoice management with allocated orders so that both modes can be used simultaneously.
*   **Invoice management with allocated orders**: In this mode, you enter a blanket order based on which you can create partial invoices and the corresponding orders.
*   **Invoice management**: In this mode, partial invoices for working hours performed and for purchased elements can be issued and allocated to an order as a claim.

When invoice management is active, the dialogs for general projects are locked in master data for allocating customers and suppliers. Module Documents shows the invoice management dialogs if one of the invoice management versions is has been enabled.

The actual projects are defined as such before they are assigned to customers and suppliers. A project can be allocated to one or several customer(s) or supplier(s).

A blanket order is assigned to just one customer however.

### Estimated quantities
Maximum quantities for a project can be defined for a product or a product group. These can refer to the net turnover, the quantity, or the surface:
*   Defining the net turnover is useful for example if lites of different sizes and/or glass types are going to be delivered.
*   Defining the quantity is useful if a certain product of a fixed size shall be delivered.
*   Defining the surface is useful if different sizes of the same product shall be delivered.

> **Quantities for a product or a product group?**
> If you plan to offer quite different products for the same project it is advisable to enter a maximum value for a product group.
> If certain products have been agreed, the maximum quantity depends on the size. A quantity should be used for fixed sizes while otherwise, the surface should be defined.

### Project management settings
Project management requires that one of the following settings is made in company data:
*   Standard project management
*   Extended project management
*   Standard project management + invoice management with allocated orders

One of the following settings must be selected in company data for the invoicing of blanket orders:
*   Invoice management with allocated orders
*   Standard project management + invoice management with allocated orders

> **Previous knowledge**
> Please note that the sequence of necessary steps is described only in brief here for those steps that have been described in closer detail in other parts of the A+W Business documentation.

### How to define the settings for project management

1.  Please make sure that the right mode has been enabled in company data, e.g. `Standard project management`.

| | |
| :--- | :--- |
| **A** | Company data - Documents tab |
| **B** | Project management mode |

*Fig. B-315: Enable project management*

2.  Enter a project.
3.  Define the terms to be used for pricing, e. g. rate, price, discount.
4.  Allocate the project to the customers and suppliers involved.

If a project is assigned to several customers, the settings for maximum values and the validity are saved separately. You can draw up a list of orders for a customer at a time.

These steps are described in detail in Tutorial 1.
*   Tutorial 1, "Definition and Allocation of Projects" on page B-186
*   Tutorial 1, "Input of Unit Prices" on page B-301
*   Tutorial 1, "Defining a discount" on page B-424

## Standard project management

Use standard project management to enter an order and define the project to which the order refers.

First, make sure that `Standard project management` has been enabled in company data.
⇨ "Project management settings" on page B-570

> **Previous knowledge**
> Please note that the sequence of necessary steps is described only in brief here for those steps that have been described in closer detail in other parts of the A+W Business documentation.

You have to execute the following steps before entering an order for a project:
*   Enter a project
*   Allocate the project to the customer
*   Enter a price for the customer and the project (optional)
*   Enter a discount for the project (optional)

| | |
| :--- | :--- |
| **A** | Validity of the project |
| **B** | Agreed maximum values for the project |

*Fig. B-316: Project arrangements (standard project management)*

For every customer and supplier you can defined the period (A) in which orders or purchase orders can be entered for the project. You can also enter the maximum amount, surface, and/or quantity (B).

### Enter an order for a standard project

The project-related prices and discounts are taken into account for invoicing an order if the customer and the project have been defined.

#### How to enter an order for a project
1.  Go to `Documents` > `Order` > `Order`.
2.  Fill in the header on tab `Document`.
3.  Go to the `Terms` tab.

| | |
| :--- | :--- |
| **A** | Customer project |
| **B** | Supplier project |

*Fig. B-317: Customer order - Project (tab Terms)*

4.  Go to section `Terms / order volume` and enter the number of the customer project (A).
    You cannot enter the number if the project's validity has expired or if the project status is completed and it has been closed.
5.  Open the item entry and enter the order items.
    Since no products or product groups are defined for a standard project, you can enter a product at random.
6.  Select in the menu `Start` > `Save` to save the data.
    The data will be saved. The prices will be calculated and the price views are updated.
7.  Close item entry.
    You can display a list of the orders that have been entered for this project so far.
8.  Go to tab `Terms` and click on the zoom icon right next to the project name.

| | |
| :--- | :--- |
| **A** | Orders entered for the project so far |
| **B** | Total for the entered orders |
| **C** | Maximum values acc. to project definition |

*Fig. B-318: Customer orders for the project*

This view only shows the orders of the present customer.

## Extended project management

Extended project management can be used for defining additional terms for the projects, e. g. payment terms.

First, make sure that `Extended project management` has been enabled in company data.
⇨ "Project management settings" on page B-570

> **Previous knowledge**
> Please note that the sequence of necessary steps is described only in brief here for those steps that have been described in closer detail in other parts of the A+W Business documentation.

You have to execute the following steps before entering an order for a project:
*   Enter a project
*   Allocate the project to the customer
*   Enter a price for the customer and the project (optional)
*   Enter a discount for the project (optional)

### Working with extended projects

For instructions on this subject, please see:
*   "How to define a project" on page B-575
*   "How to check the accumulated totals" on page B-578

#### How to define a project
1.  Enter a project.
2.  Allocate the project to the customer.

| | |
| :--- | :--- |
| **A** | Period for order entry |
| **B** | Salesman for commission calculation |
| **C** | Different payment terms |
| **D** | Status |

*Fig. B-319: Extended project settings*

3.  Define the validity (A) if orders shall be entered for this project only up to a certain date.
    If the project is completed earlier you can change the status (D) to `completed`.
4.  Enter an alternative salesman (B) and/or different payment terms (C).
    At order entry, this information will be adopted for the order if the order is allocated to the project.
5.  Go to tab `Estimated quantities`.

| | |
| :--- | :--- |
| **A** | Selection of the product |
| **B** | Select the product group |
| **C** | Input fields for quantities |
| **D** | Release input fields |

*Fig. B-320: Extended project settings - estimated quantities*

6.  Click on button (D) to release the input fields.
7.  Choose the option for which you are going to enter values, i.e. `Product` (A) or `PGR` (B).
8.  Enter the estimated quantities (C).

9.  Select in the menu `Start` > `Save` to save the data.
    You can now enter orders for the customer and also define the project. The accumulated totals for a project are updated whenever an order item is saved.
    If the project status is set to `completed`, no further orders can be entered for this project. You can thus lock the project even before its validity has expired. The project will be locked automatically when the 'valid until' date has been reached.

### How to check the accumulated totals

1.  Go to dialog `Invoices` > `Totals`.
    This tab shows the totals for the present customer.

| | |
| :--- | :--- |
| **A** | Product for which quantities have been entered |
| **B** | Product groups of the products entered in the orders |

*Fig. B-321: Accumulated totals*

You can see if the project limits defined on tab `Estimated quantities` have been reached for product (A).

| | |
| :--- | :--- |
| **A** | Products for which no quantity has been agreed |
| **B** | Estimated turnover achieved |

*Fig. B-322: Accumulated totals*

When the limit of a product or product group has been reached or even exceeded, the appropriate entries will appear in red (B) at the top of the list.

Products for which no quantities have been entered, will be listed as well. The corresponding product groups will also be shown for these products. The quantities are only taken into account for the total price however.

The information shown on tabs `Estimated quantities` and `Totals` can be printed.
2.  Go to menu `Print` > `Screen` > `Print by product` to view the list.
3.  Acknowledge the printer settings to start printing.
    In the same way you can send the list to the printer straight away.

*Fig. B-323: Accumulated totals for all customers involved*

The printout shows all projects and customers.
To get an overview of the totals in a project, select the project and start printing.

## Invoice management with allocated orders

A blanket order can be allocated to a project in this mode. In the blanket order, enter products without details on the product structure for the individual items, e. g. an IG product without details on processing, grills, or shapes.

Based on this blanket order, create claims in which you define the percentage, quantity or amount of the original blanket order to be delivered. When you create a claim, an order of the type `Claim` will be issued automatically.

No invoices will be issued for these claims. They are transferred to financial accounting in a special mode. When the blanket order is fulfilled and thus completed, the (whole) blanket order will be invoiced.

For production and delivery to the customer, issue work orders and allocate them to the (invoice) project. You can even issue purchase orders for these work orders which are also allocated to the project. These purchase orders can be created manually, or via automatic transfer to purchasing. Both types of purchase orders can be listed separately. No invoices will be issued for work orders.

*Fig. B-324: Invoice management with allocated orders (Diagram shows flow from Blanket Order to Partial Invoices, Production Orders, and Purchase Orders, all feeding into a final Total Account)*

Once a project has been marked as completed, no further orders can be entered for it. This status is set automatically when the quantities from the partial invoices have reached the quantities defined in the blanket order.

## Invoicing of blanket orders

You can enter prices and discounts for the customer for whom the blanket orders are entered. If special terms shall apply to the blanket order, the appropriate prices, discounts, or surcharges have to be defined for the customer.

One of the following settings must be selected in company data for the invoicing of blanket orders:
*   Invoice management with allocated orders
*   Standard project management + invoice management with allocated orders

For instructions on this subject, please see:
*   "How to enter a blanket order" on page B-583
*   "How to enter an order for a blanket order" on page B-586
*   "How to issue a partial invoice" on page B-588
*   "How to complete a blanket order" on page B-591

> **Previous knowledge**
> Please note that the sequence of necessary steps is described only in brief here for those steps that have been described in closer detail in other parts of the A+W Business documentation.

### How to enter a blanket order

1.  At order entry, enter a blanket order of the document type `Blanket order`.

| | |
| :--- | :--- |
| **A** | Document type Blanket Order |

*Fig. B-325: Blanket order*

2.  Enter the products to be invoiced by means of this blanket order.
    Entering e.g. an IG product without details on grills, shapes, or processing is quite sufficient.
3.  Save the order and close order entry.
4.  Go to `Documents` > `Project invoicing` > `Invoicing`.
    Dialog `Invoices` appears.
5.  Go to the menu `Start` > `New` to switch to the input mode.
    The input fields are enabled.

| | |
| :--- | :--- |
| **A** | Reference to quotation or customer order |
| **B** | Invoice number |
| **C** | Customer number |
| **D** | Blanket order number |
| **E** | Status |

*Fig. B-326: Enter an invoicing project for a blanket order*

6.  Enter the following data:
    *   Invoice number (B)
    *   Customer number (C)
    *   Blanket order number (D)
    As a reference (A) you can enter the number of the quotation and/or of the order placed by the customer.
    If the orders are to be shipped to another address, enter the corresponding details, e. g. one of the customer's subsidiaries.
7.  Select in the menu `Start` > `Save` to save the data.
    Now you have created an invoicing project for your blanket order.
    You can switch to tab `Blanket order` to view the items of the blanket order. If the data do not appear right away please reload the blanket order in selection mode.

*Fig. B-327: Items of the blanket order*

The preparations for invoicing are thus completed. You can now enter partial invoices and the corresponding work orders.

### How to enter an order for a blanket order

1.  Go to `Documents` > `Order` > `Order`.
2.  Select menu `Edit` > `New`.
3.  Fill in the header on tab `Document`.

| | |
| :--- | :--- |
| **A** | Document type Work Order |
| **B** | Invoice number |

*Fig. B-328: Work order for a blanket order*

4.  Choose the document type (A) `Work order`.
5.  Enter the invoice number (B).
    The invoice number is no longer available after the estimated quantity defined in the blanket order has been used up.
6.  Select in the menu `Start` > `Save` to save the data.
7.  Go to tab `Items` and enter the items and quantities to be produced and shipped.
    You can now enter shapes, grills, and processing steps for the items.
8.  Edit the order, e.g. by transferring it to production and/or purchasing.
    Dialog `Invoices` can be used to view the orders entered so far and the quantities that are still open.

*Fig. B-329: Assigned orders*

### How to issue a partial invoice

1.  Go to `Documents` > `Project invoicing` > `Invoicing`.
    Dialog `Invoices` appears.
2.  View the invoice for which a partial invoice shall be issued.
3.  Go to menu `Functions` > `Issue partial invoice`.

| | |
| :--- | :--- |
| **A** | Quantity to be invoiced |
| **B** | Quantity unit |

*Fig. B-330: Partial invoice*

4.  Enter the quantity (A) and the quantity unit (B) to be invoiced, e.g. 25 units.
    For the individual items you can choose quantity, per cent, or amount. The unit chosen for the first partial invoice for an item has to be kept for the following invoice.
5.  Click on `[OK]` to save the data.
    The data will be saved. The dialog closes; dialog `Invoices` reappears. On tab `Blanket order`, the entries in the appropriate columns will be updated.

An order of the type `Claim` is created in document management.

| | |
| :--- | :--- |
| **A** | Document type 'Claim' |
| **B** | Invoice number |

*Fig. B-331: Document 'Claim'*

The type `Claim` (A) and the invoice number (B) are set automatically.

6.  Go to item entry and check the items.
    You cannot print an invoice for this order. The following message appears when you start printing invoices:
    > **Question [3483]**
    > ? 1 unprocessed documents! Start printout nevertheless?

7.  Start the printing of invoices nonetheless so that the order status is changed.
    When this is completed, success of processing will be reported.
    No invoice is issued though.

| | |
| :--- | :--- |
| **A** | Status |
| **B** | Invoice number |

*Fig. B-332: No invoice for partial orders*

The fields for the invoice number and the invoice amount both show an entry of 0. The document status will still be set to `printed`.

### How to complete a blanket order

The claim can now be transferred to financial accounting, and then closed.
1.  Go to `Documents` > `Project invoicing` > `Invoicing`.
    Dialog `Invoices` appears.
2.  Display the (invoicing) project to be completed.
    When all quantities have been met, the project status is set to `complete`.
3.  Tab `Blanket order` shows whether all invoiced quantities have been set to 100%.

*Fig. B-333: Blanket order completed*

4.  Open the blanket order in document management and close it by printing the invoice and transferring it to financial accounting.

## Available document types

We distinguish the following document types:

| Type | Description |
| :--- | :--- |
| **Down payment** | This document type is automatically set for deposits. |
| **In-house production** | This document type is set when an order (work order) is entered. |
| **Receivables** | This document type is automatically set when an invoice is issued. Module: Project invoice management. |
| **Internal charging** | This document type is automatically set at transfer to purchasing. Module: Profit center invoicing. |
| **Internal order** | This document type is automatically set at transfer to purchasing. Module: Internal orders (multi-stepped production). |
| **Customer material** | This code has to be set manually. As a result, all items will be automatically set to supply type Customer's own glass. |
| **Stock P.O.** | This document type is set for stock P.O.s. The code can also be set manually for a P.O. |
| **Complaint** | This document type is automatically set when a complaint is entered. The code can also be set manually for an order. |
| **Partial Del.** | This document type is automatically set when partial shipments are entered. |
| **Value booking** | This document type is automatically set when a credit note is issued. Quantities like piece, square meter and linear meter are not transferred to statistics as a result. |

*Tab. B-25: Document types*
⇨ Software Reference, "Company Data > Archives" on page B-989

## Available limit types

The limits are fixed and cannot be changed. If you need more limit types please contact A+W Software GmbH.

**Tab. B-26: Limit types for price definition (Section 1 of 3)**

| Limit type | Description | Example |
| :--- | :--- | :--- |
| **1 x width+height** | Sum of width and height. | 600 + 800 = 1400 mm |
| **Number of fields** | Only for grills. | |
| **Number of intersections** | Only for grills. | |
| **Processing Index** | 'up to' value. ⇨ "Processing Index" on page B-317 | Up to including 100. This value is defined with a reference to glass thickness and product type. |
| **Exact processing index** | Exact value. | 101 for doors. |
| **Width** | 'up to' value for the width. | Up to 1800 mm of a lite. |
| **Width (proc.)** | Maximum value for processing (length of processing). | 450 mm for notches. |
| **Exact width** | Exact value. | 1200 mm for doors. |
| **Width/Height** | Aspect ratio of width and height. | 1:2 |
| **Thickness** | On main item level: Item thickness. On BOM level, the system will search for the main glass: If the main glass is found: Glass thickness. If no main glass is found: Item thickness. | |
| **Thickness (additive, glass only)** | Thickness of all lites of the BOM. | Main laminated glass item + BOM element 1 float = 4 mm + Film 0.75 + BOM element 2 float = 4 mm = Total thickness of all lites = 8 mm |
| **Thickness (glass only)** | Thickness of the individual BOM lite. | 26 mm |
| **Thickness (BOM)** | On main item level: Total item thickness. On BOM level: Thickness of the BOM element. | Film, glass (for BOM elements) |
| **Thickness (parent product)** | On main item level: Total item thickness. On BOM level: Thickness of the parent product. | IG - toughened glass - processing. The parent product in this case is toughened glass. |
| **Diameter** | Drilling diameter. | 12 mm |

**Tab. B-26: Limit types for price definition (Section 2 of 3)**

| Limit type | Description | Example |
| :--- | :--- | :--- |
| **Assembly position** | Glass price graduated by fitting position | Example 1: Main item: IG. Fitting position 1: single annealed, Fitting position 2: Airspace, etc. Example 2: Main item IG. Fitting position 1: LG, etc. |
| **Distance** | Surcharge calculation for transport/toll per kilometer. | 130 km |
| **Main product no.** | Product number of the main item. | |
| **Height** | 'up to' value for the height. | Up to 5800 mm of a lite. |
| **Height (proc.)** | 'up to' value for processing (length of processing). | 950 mm for notches. |
| **Exact height** | Exact value. | 2100 mm for doors. |
| **Edgework size** | Processing steps such as bevelling or mitres. For bevelling = bevelling width. | |
| **Edge length (longest/shortest)** | 'up to' value on main item level. | |
| **kg/lbs** | Unit weight. | Surcharge for transport/toll. |
| **kg/lbs per item** | Total item weight. | Surcharge for transport/toll. |
| **Linear meters** | Linear meters of this unit. | Grills. |
| **Linear meters (proc.)** | Linear meters of processing. | Edge polishing. |
| **Lin.m. (rounded)** | Linear meters, rounded. ⇨"Size calculation" on page B-211 | |
| **Lin.m. order Product/PGR/MPG/SPG** | Total linear meters of a product or a product group in an order. | Example product: Item 1: 5 lin.m, Item 2: 10 lin.m. Quantity limit: up to 10 lin.m = 5 Euro/lin.m, up to 99 lin.m = 4 Euro/lin.m. Total lin.m. per order: Product 1001 = 15 lin.m = 4 Euro/lin.m |
| **Lin.m. item** | Total linear meters of the item | |

**Tab. B-26: Limit types for price definition (Section 3 of 3)**

| Limit type | Description | Example |
| :--- | :--- | :--- |
| **Net value (delivery date)** | Total order value for a customer per delivery date. | Module Shipping fee: The shipping fee is calculated when the invoice is issued. |
| **Product type / Product group** | Product type/group of a glass on main item level or BOM level. | |
| **Sqm** | Square meters for this item. | Glass, coating. |
| **sqm (rounded)** | Square meters, rounded. | Glass |
| **sqm (delivery date)** | Total square meters for a customer's order per delivery date. | Module Shipping fee: The shipping fee is calculated when the invoice is issued. |
| **sqm order Product/PGR/MPG/WOG** | See lin.m. order product. | |
| **sqm item** | Total square meters of main item. | Glass, coating |
| **sqm item (rounded)** | Square meters of main item, rounded. | Glass |
| **Sqm rectangle** | Surrounding rectangle (for shapes). | Limit type is irrelevant for pricing. |
| **Radius rounded corner (proc.)** | Radius of rounded corners. | |
| **Grills** | See lin.m. order product. | Limit type is irrelevant for pricing. |
| **Pcs. order product/PGR/MPG/SPG** | See lin.m. order product. | |
| **Pcs. item** | Total item quantity. | |
| **Pieces** | Item quantity. | |
| **Pcs. (proc.)** | Number of processing steps. | |
| **AIR** | Spacer thickness. | |
| **Spacer (biggest)** | Biggest spacer in an IG unit. | |
| **PGR external key / key exact** | The external key can be used to calculate prices by product group. | Example: Processing of toughened and laminated glass. |
| **Net surcharge basis** | Proportional energy surcharge on glass. The basis for the energy surcharge is the total net price of all lites of an order. The surcharge is automatically added as order item 900. | Example: up to 1000.00 = 5% surcharge, over 1000.00 = 2% surcharge |

## Available system text

**Tab. B-27: System text**

| No. | Text | Context |
| :--- | :--- | :--- |
| 1 | Shape | |
| 2 | ;bottom:;right:;top:;left:;Sheet; S | Step dimensions |
| 3 | Glass is included in the shipment! | |
| 50 | Invoice <ar> dated <ard> for deposit dated <ad> | Down Payments |
| 51 | Down payment of <ad> for order <aa> of <aad> | Down Payments |
| 100 | Original invoice total %X1 | DMS project management |
| 101 | Previous changes %X2 | DMS project management |
| 102 | Changes effected with this invoice %X3 | DMS project management |
| 103 | Total changes %X4 | DMS project management |
| 104 | New invoice total %X5 | DMS project management |
| 105 | - incomplete work %X6 | DMS project management |
| 106 | Value of work completed %X7 | DMS project management |
| 107 | - previous invoice %X8 | DMS project management |
| 108 | TODAY'S INVOICE NO.%X9%X10 | DMS project management |
| 110 | Ug value in W/sqm | Tech. IG parameter |
| 111 | Ug value according to DIN 4108-4 | Tech. IG parameter |
| 112 | Light transm. in % | Tech. IG parameter |
| 113 | g value in % | Tech. IG parameter |
| 114 | b factor | Tech. IG parameter |
| 115 | Sound insulation factor in dB | Techn. IG parameters |
| 116 | Thickn.tolerance in mm | Tech. IG parameter |
| 117 | Size tolerance mm (<200 cm) | Tech. IG parameter |
| 118 | Size tolerance in mm (<200 cm) | Tech. IG parameter |
| 119 | Airspace bars, single | Insurance price list |
| 120 | Airspace bars, several | Insurance price list |

⇨ Software Reference, "System Text" on page B-1064
⇨ Tutorial 2, "Text input" on page B-543

## Available variables (wildcards)

You can enter text variables which will be filled in in the actual document.

### Formula
`<@Formula number@>` = execute a formula with number (nn)
⇨ "Variables" on page B-539

### General

**Tab. B-28: Variables**

| Section | Variable | Meaning |
| :--- | :--- | :--- |
| **General** | `%X1, %X2, %X3, etc.` | A+W Business will fill the variables with the appropriate values. ⇨ Software Reference, "System Text" on page B-1064 |
| **Down payment** | `<aa>` | Deposit order number |
| **Down payment** | `<aad>` | Deposit order date |
| **Down payment** | `<ad>` | Deposit date |
| **Down payment** | `<ar>` | Deposit invoice number |
| **Down payment** | `<ard>` | Deposit invoice date |
| **CEKAL** | `<h>` | Company number as per company data |
| **CEKAL** | `<jj>` | Year and quarter in format YYYY-QQ |
| **CEKAL** | `<p1>` | Description 1 |

### Processings

| Variable | Meaning |
| :--- | :--- |
| `<%>` | Quantity (edges, drilled holes, corner cut-outs, ...) |
| `<$>` | Main parameters (diameter, radius, width, height) |
| `<§>` | Additional parameters (edges involved, corners or x, y, d for drill holes) |
| `<=>` | Calculated lin.m. |
| `<?`>` | Calculated sqm |

| Name 3 in product management | Processing dialog, item entry |
| :--- | :--- |
| `<%>` edges [`<§>`] with miter 45° polished (`<=>` lin.m.) | 2 edges [2/3] with miter 45° polished (2.45 lin.m.) |
| Sawing of `<%>` edges `*<§>*` | Sawing of 3 edges *2/3/4* |
| `<%>` holes, d = `<$>` mm | 2 holes with d = 20 mm |
| `<%>` hole(s) d=`<$>`mm X, Y [`<§>`] | 2 holes d = 20 mm X, Y [100, 100] |
| `<%>` x `<$>` mm rounded corner [`<§>`] | 4 x 15 mm rounded corner [1/2/3/4] |
| `<$>` corner cut-outs / `<%>` pieces / [`<§>`] | 100 x 75 corner cut-outs / 2 pcs. / [3/4] |

### Spacer text

The spacer text can be entered in the product, and refers to the standard text. If only a number shall be transferred for the customer, the number must be entered in the standard text. The whole text can be transferred with variables.

**Tab. B-29: Variables for spacer text**

| Variable | Meaning |
| :--- | :--- |
| `<ab>` | Spacer name, short |
| `<sc>` | Spacer code |
| `<an>` | Order number without leading zero or blanks |
| `<br>` | Width, without leading zeros or blanks |
| `<c1>` | Customer name 1 |
| `<cn>` | Customer number |
| `<esg>` | Toughened glass, short name |
| `<g>` | Gas |
| `<gt>` | Quality Text |
| `<ho>` | Height, without leading zero or blanks |
| `<kp>` | Customer item |
| `<no>` | Order number/item |
| `<p1>` | Product name 1 |
| `<p2>` | Lite structure |
| `<pd>` | Production date |
| `<pn>` | Product number |
| `<po>` | Item number with leading zeros, 3-digit |
| `<ps>` | Item number, without leading zero or blanks |
| `<sn>` | Key number |
| `<vs>` | Laminated glass name |
| `<vsg>` | Laminated glass name, short |
| `<wh>` | Item sizes |
| `<kk>` | Transfer to purchasing: Customer consignment |

**Example**
*   **Entry**: `<c1> <p1> <p2> <wh> <no>`
*   **Output**: John+Partner Standard IG FL4/18/ORN528 540x1030 109384/001

## Patterns for leaded designs

The following patterns are defined by default for leaded designs:

*Fig. B-334: Leaded design patterns*

| Type | Name | Type | Name |
| :--- | :--- | :--- | :--- |
| Type 1 | Gothic | Type 2 | Stuart |
| Type 3 | Diamonds | Type 4 | Cumberland |
| Type 5 | Hanover | Type 6 | Jacobean |
| Type 7 | Northumberland | Type 8 | Queen Anne |
| Type 9 | Queen Caroline | Type 10 | Rectangles |
| Type 11 | Square Gothic | Type 12 | Diamond Pillar |
| Type 13 | Westmorland | Type 14 | Windsor |
