---
description: "EN_AWBusiness_Master_Data_9_5-3"
---


# Tutorial 2: Documents

4.  Choose the rounding point (B), e.g. VAT 1.
    You have now defined that VAT 1 shall be rounded. If a second tax rate is applicable for the customer, this will not be rounded.
5.  Choose the product type (C) and price unit (D).
    If you choose e.g. `<n.e>`, the settings will always be valid for this customer.
    In this example, the VAT rounding is specified. The price unit is therefore irrelevant.
6.  Select the rounding table you have drawn up for this customer, e.g. 0.05.
7.  Select in the menu Start > Save to save the data.
    The data will be saved. The new rounding will be applied to the selected customer. For all other rounding points, the general rounding allocation will still be valid for him.

---
## Exercises

*   Check the existing rounding settings and rounding allocations.
*   Allocate the following rounding to your training client:
    *   All glass items shall be commercially rounded to three digits.
    *   All unit prices shall be rounded to 0.05. Enter this rounding if there is no corresponding entry in dialog Roundings.
*   Allocate to your training customer a commercial rounding of VAT to 0.05.

### Additional Information
=> Software Reference, "Rounding (Customer, Supplier)" on page B-839
=> Software Reference, "Rounding for Customer/Supplier Groups" on page B-840
=> Software Reference, "Rounding" on page B-880
=> Software Reference, "Rounding Points" on page B-882
=> Software Reference, "Rounding Allocation" on page B-883

## Settings for Invoicing

Apart from the settings for pricing in the dialogs for prices, partners, discounts, and rounding, further data are required for the processing of documents, e. g. for payments and VAT calculation.

This chapter shows you how to edit the appropriate settings.

This includes the following training modules:
*   "Finance" on page B-454
*   "Automatic Surcharges" on page B-324

An invoice must include at least the following elements:
*   **Details on the issuing party**
    *   Company name and address
    *   Tax number and/or VAT ID
    These settings are made in dialog **Company Data**.
*   **Details on the recipient (customer)**
    *   Name and address
    These settings are made in dialog **Partner Management**.
*   **Details on the delivery/service**
    *   Delivery date
    *   Quantity and description of the products delivered
    *   Net amounts, broken down by tax rates if required
    *   Tax
    *   Date of issue (= invoice date)
    *   Unique invoice number
    These details are part of the order.

Apart from that you can - among other things - enter bank accounts for printing bank transfer forms and payment terms, manage currencies, and define tax rates.

## Finance

### Objectives
*   Introducing basic data dialogs for accountancy.
*   Checking and defining the settings for payment terms.

### Benefits
*   All data required for commercial accounting and for financial accounting are entered as basic data and are allocated to the partners and products. These data are therefore entered only once, and are maintained centrally.

### Please note

| Topic | Description |
| :--- | :--- |
| **Tax Rates** | Taxes can be calculated only if they have been defined as tax rates. Tax rates are allocated to the products and the partners. They can be changed in the documents. |
| **Currencies** | Prices can be kept in different currencies. Orders can be entered in national currency or foreign currency. For statistical comparison, your home currency will be used always. The amounts are converted by A+W Business for this purpose. |
| **Banks** | Based on the (complete) bank data, the IBAN can be determined in partner master data. |
| **Payment conditions** | Payment terms are allocated to the partners. They can be changed in the documents. |
| **Foreign key** | In the dialogs in which data for accounting are entered, an external key refers to the corresponding booking fields in the financial accounting program (FinAcc). The entry for the external key depends on the corresponding financial accounting system. |

## Taxes
Tax rates have to be entered for calculating the tax in documents. These tax rates are allocated to the products and partners.

