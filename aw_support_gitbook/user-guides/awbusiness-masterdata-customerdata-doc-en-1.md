---
description: "EN_AWBusiness_Master_Data_9_1-4"
---


# Customer Data

**Related Topics:**
- "How to allocate an alpha-numerical value" on page B-76
- "How to allocate a numerical value" on page B-78

---
## How to allocate an alpha-numerical value

1.  Go to menu **Master data > Partners > Customer > Customers > tab Classifiers**.

    *Fig. B-33 Allocate classifier value: This image shows the 'Classifiers' tab in the customer master data screen. It highlights the 'Classifier type' column (A) and the 'Allocated value' column (B).*

2.  Mark a classifier (A) with code A (alpha-numerical). The entire line is selected.
3.  Go to menu **Functions > Classifiers group > Classifier values**.
    You can also double-click on the **Value (B)** field of the selected classifier. The dialog **Classifier value allocation** appears.

    *Fig. B-34 Enter a classifier value: This dialog shows an input line (A) for a new value, a 'New' button (B) to release the input line, and an 'Adopt' button (C) to adopt the value.*

4.  Click on **[New]** (B) to get access to the next line. The next line is released.
5.  Enter the new value, e.g., `Area South 1` for an alpha-numerical classifier for the turnover.
6.  Click on **[OK]** to save the data. The data will be saved. You can enter further classifiers by repeating the steps 4 to 6. These classifier values will not be automatically adopted for the current partner.
7.  Select the line with this value and click on **[Adopt]** to assign this value to the partner. The dialog **Classifier value allocation** is closed and the dialog **Partner management** reappears in the foreground.

    *Fig. B-35 Adopted classifier value: This image shows the 'Classifiers' tab with the value "South 1" now assigned to the 'Key group' classifier.*

8.  Select in the menu **Start > Save** to save the data. The data will be saved. They can be used now for analysis.

## How to allocate a numerical value

1.  Go to menu **Master data > Partners > Customer > Customers > tab Classifiers**.
2.  Position the cursor in section **Classifiers** on the field **Value** for an entry with code N (numerical) or D (Date).
3.  In the context menu, select **Insert**. Open the context menu with the right mouse key.
4.  Enter the values as defined:
    - **N (numerical)**, e.g. `600000` (turnover)
    - **D (date)**, e.g. `23.02.2012` (birthday gift for the head of department)
    Use `<Tab>` to go to the next line to enter another value.

    *Fig. B-36 Numerical value: The image displays the 'Classifiers' tab where a numerical value '600000' has been entered for the 'Group turnover' classifier.*

5.  Select in the menu **Start > Save** to save the data. The data will be saved.

## Exercises

The exercises are based on each other. The data you have entered for exercise purposes will therefore be needed again. Mark these data so that they are easy to distinguish, e.g., by the supplement 'training' or 'demo'.

-   Enter at least one new customer.
-   Enter routes for your district, for collection, and for a forwarder.
-   Enter a customer group called Training.
-   Allocate your customer to one of the groups.
-   Allocate the customer to another customer group when a toughened glass order is entered for him.
-   Standard rounding
-   Invoicing mode
-   Partial shipment and partial invoice permitted
-   Enter an alternative invoice address.
-   Define one of the addresses as the standard shipping address.
-   Enter text for your training customer which is valid only for him, and shall be printed on production papers.
-   Enter three classifiers with different properties (numerical, alpha-numerical, date).
-   Allocate to your training customer a value for each of the classifiers.

### Locking of demo data

> If you do your exercises during actual operation you should lock the demo data for further use as soon as you have made your tests.

## Finances and Balance

### Objectives

-   Knowing the terms for invoices and payments.
-   Defining a calendar and a change of payment date.
-   Setting the credit limit check.

### Benefit

-   Customer invoices are issued based on the settings made in customer master data.
-   Balance and credit limit are shown at order entry so that the actual orders and receivables can be taken into account.

### Note

**Due date**
: Due dates are calculated automatically. Enter the required mode and the invoicing dates.

**Credit term**
: The document date and the invoicing date form the first reference date. This is the basis for calculating the credit term.

**Payment day postponement**
: To make sure that no invoices are due for payment during the customer's company holidays you can define the period in question in the customer's calendar.

**Payment terms**
: Each payment term can take into account several levels of due dates and percentages for the cash discount.

**Acct. No.**
: The customer number is used as the main account and is transferred to financial accounting. The customer number of one of the customer's subsidiaries can be used as the main debtor to whom invoices and credit notes are addressed.

**Credit limit**
: You can define the insured credit limit and the internal (uninsured) credit limit for every customer. The credit limit can be automatically checked when new orders are entered.

**Taxes**
: Taxes can be calculated only if they have been defined as tax rates and allocated to the customer.

**Currencies**
: Prices can be kept in different currencies. Orders can be entered in national currency or foreign currency. The national currency will always be used for statistical purposes. A+W Business will convert the amounts accordingly.

## Payment Settings

Invoice settings can be made for every customer on tab **Finances**.

*Fig. B-37 Customer master data - tab Finances: This screenshot displays the 'Finances' tab within the customer master data, showing various fields for financial settings. Key areas highlighted are:*
-   *A: Bank account details.*
-   *B: Due date calculation settings.*
-   *C: Invoicing details like due days and payment days.*
-   *D: Payment terms.*
-   *E: Main account or alternative invoice address.*
-   *F: Valid tax rate selection.*

The customer's bank details (A) are entered e.g. in order to use them for credit notes or printing receipts.

For the customer invoices, enter:
-   Due day calculation mode (B)
-   Accounting date (C)
-   Payment terms (D)
-   Valid tax rate (F): You can enable up to five different tax rates.

The tax rates are defined in **Finances > Tax**. You can also enter (in company data) whether the tax shall be calculated per item or per BOM element. This entry is valid for all customers. The settings in company data are described in the software reference.

## Due Date Calculation

Due dates are calculated automatically. Enter the required mode and the invoicing dates:
-   Accounting date, e. g. if the invoice date is not decisive.
-   Due days (gross days)
-   Payment days

| Mode | Text |
| :--- | :--- |
| **0** | 1st Reference date |
| **1** | 1st Reference date + Days gross |
| **2** | 1st Reference date + Days gross + Rounding up to 1st day of settlement or end of month |
| **3** | 1st Reference date + Days gross + Rounding up to the 15th or end of month |
| **4** | 1st Reference date + Days gross + Rounding up to the 10th, 20th or end of month |
| **5** | 1. Reference date rounded to end of month + gross days (0/30/60/90). The calculated term of payment is always rounded to the month's end. **Attention:** For flag 5 and 6, the entry in field Gross days must be divisible by 30. 30 days = 1 month, 60 days = 2 months, 90 days = 3 months by which the first reference date is increased. |
| **6** | 1. Reference date is rounded to the month's end + gross days (0/30/60/90) + date of settlement |
| **7** | 1st Reference date + Days gross + rounded up to 1st, 2nd or 3rd day of settlement |
| **8** | 1st Reference date + Days gross + rounded up to 1. Or 3rd day of settlement in dependence on 2nd day of settlement |
| **11** | Maturity date = shipping date + payment term |

Examples for calculating due dates are available in section Sales.
⇨ Sales, "Due date calculation" on page C-208

## Accounting

The document date and the accounting date form the first reference date. This is the basis for calculating the payment term.

-   **Accounting date = 0:** The first reference date matches the document date.
-   **Accounting date ≠ 0:** The document date is rounded to the accounting date and forms the first reference date.

**Examples**
*(ACD = accounting date)*

| Document date | ACD | 1st reference date | Note |
| :--- | :-- | :--- | :--- |
| 13.03. | 0 | 13.03. | 1st Reference date = Document date |
| 13.03. | 25 | 25.03. | The document date is rounded to the 25th of the same month |
| 27.03. | 25 | 25.04. | Since the invoicing date is less than the document date, the document date is rounded to the 25th of the following month |

These examples show how the first reference date is calculated from the document date and the accounting date.

## Payment Day Postponement

You can define that the calculation of the payment date shall be postponed, e.g., to make sure that invoices do not become due during the customer's works holidays. The time of the postponement is set in the customer calendar.

Calculation always refers to the entries in the customer calendar. The type of postponement is valid irrespective of the days defined in the customer calendar.

⇨ "Editing Customer's Calendars" on page B-103

| Option | Type of postponement |
| :--- | :--- |
| **0** | No postponement |
| **1** | **50:50 split** - due dates are split into half: One half of the amount becomes due within a certain period before the original due date. The other half is due within a certain period after the original due date. |
| **2** | **Shift by period** – due dates will be postponed by a certain period. |
| **3** | **Same as option 2 plus surcharge.** An appropriate surcharge must have been defined if you choose this option. |

## Examples

**Starting position:**
-   **Invoice amount:** 300 Euros
-   **Invoice date:** 10.07.
-   **Customer accepts no due dates in August (01.08. - 31.08.)**

### Example 1

**Credit term 30 days = Due date 10.08.**

-   **Option 1: 50:50 split**
    -   Due date 1: 10.07. = 150 €
    -   Due date 2: 10.09. = 150 €
    -   Half of the invoice amount is due before the company holidays and the other half, afterwards.
-   **Option 2: Postponement by period**
    -   Due date: 10.09. = 300 €
    -   The entire amount becomes due after the company holidays.
-   **Option 3: Like option 2 + surcharge**
    -   Due date: 10.09. = 303 € (300 € + 1 %)
    -   The entire amount is due after the company holidays. An additional surcharge will be applied.

### Example 2

**Credit terms 30, 60 days**
-   **Due date 1:** 10.08. = 150 €
-   **Due date 2:** 10.09. = 150 €

-   **Option 1: 50:50 split**
    -   Due date 1: 10.07. = 75 €
    -   Due date 2: 10.09. = 225 €
    -   150 € are due on the first due date. This amount will be split into halves so that 75 € are due on the moved up first due date. The remaining 75 € are due on the second due date so that 150 € + 75 € are due at that time.
-   **Option 2: Postponement by period**
    -   Due date: 10.09. = 300 €
    -   150 € are due on the first due date. This amount is due on the second due date so that at that time, 300 € are due.
-   **Option 3: Like option 2 + surcharge**
    -   Due date: 10.09. = 303 € (300 € + 1 %)
    -   The whole invoice amount is moved to the second due date. An additional surcharge is applied.

### Example 3

**Credit terms 30, 60, 90 days**
-   **Due date 1:** 10.08. = 100 €
-   **Due date 2:** 10.09. = 100 €
-   **Due date 3:** 10.10. = 100 €

-   **Option 1: 50:50 split**
    -   Due date 1: 10.07. = 50 €
    -   Due date 2: 10.09. = 150 €
    -   Due date 3: 10.10. = 100 €
    -   In this example, only the first due date is affected at which point 100 € would be due. This amount is split so that the first half (50 €) is due before the original date. The second half is due on the second due date together with the original (third) amount (50 € + 100 €).
-   **Option 2: Postponement by period**
    -   Due date 1: 10.09. = 200 €
    -   Due date 2: 10.10. = 100 €
    -   In this example, the amount is moved from the first due date to the second.
-   **Option 3: Like option 2 + surcharge**
    -   Due date 1: 10.09. = 201 € (200 € + 1 %)
    -   Due date 2: 10.10. = 100 € (100 €)
    -   In this example, the amount is moved from the first due date to the second, and a surcharge is applied to the postponed amount.

The customer calendar is described in a separate session.
⇨ "Editing Customer's Calendars" on page B-103

## Calendar

The current year must be defined in the general calendar in order to enter documents. Daily working hours have to be defined so that dates can be calculated at order entry, e.g. delivery dates. Weekends and public holidays (without working hours) have to be entered for these calculations.

You can also enter the company holidays by setting the daily working hours to zero for that time. These days will be taken into account when determining delivery dates.

*Fig. B-38 General calendar: This image shows the general calendar setup screen. It displays a list of dates with their corresponding working hours (A), and controls to apply changes to a week or year (B).*

The customer calendar is based on the general calendar. It mainly serves to enter the days for the due date postponement for every customer.

## Payment Terms

The payment terms for every customer are entered in customer master data on tab **Finances**. In the order header, the payment terms are loaded from customer data and can be changed if required. The settings for calculating the cash discount are made in dialog **Payment terms**.

*Fig. B-39 Payment terms: This screenshot shows the Payment Conditions dialog. It highlights the cash discount definition with rates and days (A) and the credit term definition (B).*

You can set up several steps for a payment term, in complete records of up to five credit terms (B) and three percentages (A) for cash discount. Moreover, you can enter any number of conditions which only refer to the cash discount.

**Example**

| Cash discount | Rate 1 | Days 1 | Rate 2 | Days 2 | Due days 1 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| | 3.00 % | 10 | 1.5 % | 20 | 30 |

This example shows that the customer can deduct a cash discount of 3% within the first 10 days but only 1.5% within the following 10 days. After 30 days, the invoice is due without deductions.

## Payment Modes, Solvency

Payment modes and solvency serve for information only. These entries are made in simple, basic tables. They can be extended at random.

*Fig. B-40 Payment Modes, Solvency: The image displays two simple table-based dialogs for defining Payment Modes (e.g., Bank, Check, Cash) and Solvency levels (e.g., Very good, OK, Bad).*

## Main Account or Alternative Invoice Address

You can enter the customer number of the main debtor (subsidiary) who shall receive invoices and credit notes. Prerequisite is that this has been defined as a subsidiary of the customer. The main account is thus the main debtor's customer number. If this field is blank, the number of the current customer will be automatically used as the main account.

## Banks

Enter the bank data for payments from and to your customers and suppliers.

*Fig. B-41 Bank data: This image shows a list of banks with their details. It highlights the 'Bank code' (A) necessary for IBAN, the 'BIC' (B) for international payments, and the 'Country code' (C) also necessary for IBAN.*

Banks are allocated to the partners in partner management, tab Finances. In partner management, you can have the IBAN determined by the system if at least the following data have been entered for the bank: bank code (A), country code (C), and account number (in customer master data). This function is started in partner management via menu **Functions**.

> ### Bank for the company and clients
> The bank accounts for your company and clients are entered in menu **Master data > Company > Banks**. You also access the bank data entered in **Finances**.

## Credit Limit for Customers

You can enter two different values for the credit limit for every customer, which can be automatically checked when a new order is entered. Credit limit 2 can be used as an internal, uninsured credit limit.

To check the credit limit you have to make the following decisions:
-   Define the credit limit for every customer in customer data.
    -   **Credit limit 1:** This entry defines the insured credit limit.
    -   **Credit limit 2:** This entry is an internal (uninsured) credit limit granted to the customer because of his credit standing.
-   Define the reaction in case the credit limit is exceeded:
    -   Normally, the status will be raised. If the credit limit is exceeded, new orders will be set to a defined status and will be locked for processing. This status can be reset by hand to release the orders for processing.
    -   New orders can be entered and saved. There is a message however pointing out that the credit limit is overdrawn. It is up to the user to decide whether the order shall be processed or rejected.

### Type of check

The appropriate code for every customer or subsidiary is set in partner management.

-   No credit limit check
-   Limit 1 + Message Limit 2
-   Limit 2 + Message Limit 1
-   Check of credit limit 1
-   Check limit 1 and 2
-   Check credit limit 2
-   Advance payment

If you are working with subsidiaries, the credit limit can be checked on two levels:
-   Checking the site's credit limit.
-   Check the main customer's credit limit:
    -   Check via subsidiary code
    -   Check via input in field **Main account**: The subsidiary's credit limit will be ignored.

*Fig. B-42 Partner management - Settings for checking the credit limit: This image shows credit limit settings, highlighting options for comprehensive checks by subsidiaries (A) and the dropdown for the type of check (B).*

## Show current order volume

The order header shows the credit limit and the receivables. This allows to check every order and discuss with the customer whether a new order can be accepted. In this area, data will be updated after transfer to accounting and after every report.

*Fig. B-43 Credit limit and balance: This image shows two panels. The top panel displays the credit limit and receivables within an order. The bottom panel shows the financial values in the master data, highlighting the credit limit (A) and the resulting balance (B).*

### No credit limit check

If the credit limit is not checked, the actual amounts will only be displayed. When the credit limit is exceeded and in case of cash in advance, orders can generally be processed. Quotations can be entered irrespective of the credit limit and possible locks.

### Receivables Reports

In connection with a financial accounting program (FinAcc) which reports the receivables, you will get an expressive overview of the customer's present financial status. If you do not use receivables reports, the check will include all orders which have not been transferred to financial accounting yet.

If the function **Individual receivables report** is active in company data, receivables can be checked for the corresponding customer at order entry and in customer management. All open invoices will be shown.

Customers whose balance has been settled after the last receivables report will be updated in customer management with a balance of 0.

### Overdrawn credit limit

The settings in company data and the status allocation define how A+W Business is going to act in case the credit limit is overdrawn:

-   A lock status is defined in status allocation beyond which further entries are impossible.
-   The status will be raised only if the option **Raise status if credit limit is overdrawn** is active in company master data.

If these two settings are combined, new orders cannot be entered once the credit limit is reached or overdrawn.

The message **Credit limit exceeded, customer locked** also appears before the document is copied. Copying will not take place. The credit limit will be checked even if the customer is changed in an existing order.

To process a new order even if the credit limit has been exceeded, the order status has to be reduced manually. After that, the status will not be raised again automatically. The change of status is described in detail in section Sales.

Customer orders can be transferred via EDI interface (electronically). If the credit limit is overdrawn by an order, it gets the status *Order locked due to credit limit*. It will be booked in capacity planning despite the lock status. This order has to be released manually by reducing the status. After that, it will be automatically transferred to production.

The status-raising functions will be explained in detail in a separate session.
⇨ Tutorial 2, "Status Administration" on page B-418

## The Process of Checking

*Fig. B-44 Checking the credit limit: This figure illustrates the workflow for checking a customer's credit limit.*

The process is as follows:
1.  **Enter order header**, which contains the Credit limit (Customer).
2.  **Is the credit check activated?**
    -   **No:** Proceed to **Enter order**.
    -   **Yes:** Proceed to the next step.
3.  **Is the limit overdrawn?**
    -   **No:** Proceed to **Enter order**.
    -   **Yes:** Proceed to **Change status**.
4.  **Change status** leads to the next check.
5.  **Is the order locked?**
    -   **No:** A **Message** is displayed, and you can proceed to **Enter order**.
    -   **Yes:** Proceed to the next step.
6.  **Reset status manually?**
    -   **No:** **Do not save order**. The process ends.
    -   **Yes:** Proceed to **Enter order**.
7.  **Enter order**.
8.  The order data can then be used for **Transfer invoice to financial accounting** and **Receivables report**.

The manual change of status can be prevented e.g. by the appropriate settings in the user rights.

## Credit Limit Analysis

Credit limit analysis can be used for evaluating the development of certain financial data for a customer or customer group within a defined period.

The system will analyse the credit limit, receivables, liability, balance 1, balance 2, and the orders on hand.

The hierarchy is:
1.  Undelivered orders
2.  Orders shipped but not yet invoiced
3.  Invoiced orders that have not been transferred to financial accounting yet
4.  Totals of 1-3

*Fig. B-45 Credit limit snapshot for a customer: This screenshot shows the Credit limit analysis screen, which provides a snapshot of a customer's financial data over time, including credit limits, receivables, liabilities, and order statuses.*

The credit limit snapshot is created by a daily task analysing the financial data. If you are going to work with formulas, please contact a member of the service team of A+W Software GmbH.

## Currencies

Prices can be shown in the orders in the currency allocated to the customer. Prerequisite for this is that currencies and exchange rates are entered and maintained accordingly.

For order entry, **A+W Business** can use two different currency settings:
-   **National (home) currency:** The currency of the country in which headquarters are located. In Europe, this is usually Euro.
-   **Foreign currency:** The currency that differs from the home currency, e.g. the currency in which prices are shown in orders for foreign customers.

For statistical comparison, your home currency will be used always. A+W Business will convert the amounts accordingly.

The options for price management and calculation in the orders are:
-   Price lists and orders are kept in national currency.
-   Price lists are kept in national currency; for foreign customers, the amounts can be shown either in national or foreign currency. For this, you have to enter and update the exchange rates for the foreign currencies.
-   Price lists are kept in foreign currency; the amounts in the orders can be shown in national or foreign currency. The exchange rate is defined for internal purposes.

The currency to be used as a basis for calculation as well as the currency in which orders are entered are both defined in company data.

*Fig. B-46 Company data – tab tax, currency settings: This image shows the currency settings in company data. It highlights the national currency used for calculation (A), the default setting for order entry (B), and the currency for displaying prices in the order (C).*

This example shows that the national currency (A) is Euro. The national currency is usually selected as the standard setting (B) for order entry. If you are using price lists in another than the national currency, select the setting **Euro** for displaying prices (C) at order entry.

## Pricing in connection with foreign currency

You can maintain sales and purchase prices in A+W Business even if they occur in different currencies.

Price calculation with foreign currencies can produce different results if prices for quantities are calculated on different levels. This setting is made in company data.

If the foreign currency amount shall result from the BOM and the quantity, the amounts can be calculated in the following ways.

-   **The item price is the item price in national currency:**

| Calculation | Operation | Result |
| :--- | :--- | :--- |
| HC price/PU | x factor | = FC price/PU |
| HC gross price/pc. | x factor | = FC gross price/pc. |
| HC net price/pc. | x factor | = FC net price/pc. |
| **HC item price** | **x factor** | **= FC item price** |
| *Note: NC = national currency, PU = price unit, FC = foreign currency* |

-   **The item price is created from the net price in foreign currency:**

| Calculation | Operation | Result |
| :--- | :--- | :--- |
| NC price/PU | x factor | = FC price/PU |
| NC gross price/pc. | x factor | = FC gross price/pc. |
| NC net price/pc. | x factor | = FC net price/pc. |
| **FC net price/pc.** | **x qty.** | **= FC item price** |
| *Note: NC = national currency, PU = price unit, FC = foreign currency* |

## Cash Discount

A+W Business distinguishes three calculation types for cash discount which are described in the following examples.

### On gross amount:

| Calculation | Calculation/basis | Value |
| :--- | :--- | :--- |
| Net 100.00 | 100.00 | 100.00 |
| VAT 19% | | 19.00 |
| Gross | 119.00 | 119.00 |
| Cash discount 2% | | 2.38 |

### On net amount (gross minus cash discount):

| Calculation | Calculation/basis | Value |
| :--- | :--- | :--- |
| Net 100,00 | 100.00 | |
| Cash discount 2% | 2.00 | 98.00 |
| VAT 19% | 98.00 | 18.62 |
| Gross | | 116.62 |

### On net amount:

| Calculation | Calculation/basis | Value |
| :--- | :--- | :--- |
| Net 100,00 | 100.00 | 100.00 |
| Cash discount 2% | 2.00 | |
| VAT 19% | 98.00 | 18.62 |
| Gross | | 118.62 |

## Settings in Company Data

If the status shall be changed when the credit limit is overdrawn, checkbox (A) must be ticked in company data, tab **Parameters**.

*Fig. B-47 Company data > Parameters: This screenshot shows the Parameters tab in the Company Data settings. It highlights the checkbox "Raise status when credit limit is exceeded" (A) and the setting for "Tax calculation on item/BOM level" (B).*

You have to define in status allocation whether order entry shall be locked when the status is raised. Status allocations are described in a separate session.
⇨Tutorial 2, "Status Administration" on page B-418

## Receivables

For receivables reports, you have to check the financial accounting program as well as the settings for updating in company data.

*Fig. B-48 Company data – tab FinAcc: This screenshot shows the FinAcc (Financial Accounting) tab in Company Data. It highlights the selection of FinAcc interfaces (A), the file paths for reports (B), the "Update after receivables report" option (C), and the "Individual check by customer" option (D).*

## Editing the Customer's Financial Data

The following instructions are based on the steps described in the previous session.

### How to edit the data for invoicing

1.  Go to menu **Master data > Partners > Customer > Customers > tab Finances**.

    *Fig. B-49 Partner management - Payment terms: This screenshot shows the 'Finances' tab for a customer. It highlights the 'Due date calculation mode' (A), the 'Activate tax calculation' checkbox (B), the tax rate selection (C), and the 'Lock customers' dropdown (D).*

2.  Check the settings for the lock code (D).
    If the new partner data shall be used at once, you have to choose the setting **not locked**.
    You should lock the data if e.g. price and payment agreements have not been finalised with the new partner. In this case, you cannot enter any documents for him, i.e. orders of purchase orders.

3.  Enter the settings for the due dates (A) agreed with this partner.

4.  Activate tax calculation (B) and choose the tax rate (C).
