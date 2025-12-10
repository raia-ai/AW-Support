---
title: "Business_-_Minimum_Invoice_Amount"
source: "Business_-_Minimum_Invoice_Amount.docx"
tags: ["A+W Business", "Minimum Invoice Amount", "Invoicing", "Surcharge", "Billing Policy", "Order Entry", "Customer Account Setup", "ERP", "GST"]
version: "1.0"
last_updated: "2025-10-03"
short_description: |
  This document provides step-by-step guidance for configuring a minimum invoice amount in A+W Business. It explains where to set the invoicing surcharge/minimum value on the customer record, how the system applies a surcharge when orders fall below the defined threshold, and how the resulting amounts appear during order entry and on the final invoice. Examples illustrate the configuration using a before-GST minimum value and show how the surcharge bridges any shortfall to reach the minimum invoice amount. A reference to internal ticket AW-214264 is included for further information.
long_description: |
  This guide explains how to set up and apply a minimum invoice amount in A+W Business so that small orders are automatically brought up to a defined threshold. It is intended for billing administrators, finance users, and customer account managers who configure customer-specific invoicing rules.
  
  The process begins on the customer master data, specifically the 2. Order tab, where the Invoicing surcharge / minimum value field is maintained. In this configuration, you select the appropriate mode and enter the minimum amount that should be enforced before GST. The example uses the mode “Min Value (in one item)” with a value of 36.37 set before GST. This ensures that if the sum of order lines does not reach the stated minimum, the system will automatically calculate and add a surcharge to bridge the difference.
  
  During order entry, the system inserts an additional line to represent the shortfall against the minimum. This line is clearly visible on the order, allowing users to verify that the surcharge is applied precisely to meet (but not exceed) the configured minimum invoice amount. The document references screenshots where the surcharge is highlighted in red to illustrate how the shortfall is shown within the order workspace.
  
  On the invoice printout, the surcharge appears as a distinct item (e.g., “Surcharge for bill”) that, when combined with the order items total, reaches the configured minimum. In the worked example, a surcharge of 12.88 is added to an order items total of 23.49, resulting in a final amount of 36.37, which matches the minimum defined in the customer setup. This makes the enforcement transparent to customers and auditors, and it simplifies adherence to minimum billing policies without manual adjustments.
  
  While the examples reference before-GST values, organizations should ensure the mode and value align with their tax treatment and commercial policy. For more background and internal notes, see reference AW-214264. Implementing this setting helps standardize billing practices, reduce manual intervention for low-value orders, and maintain profitability by covering fixed processing costs associated with invoicing.
  
  Key configuration elements covered include:
  - Selecting the correct surcharge mode to determine how the minimum is enforced.
  - Entering the minimum value as a before-GST amount, if applicable to your policy.
  - Verifying during order entry that the shortfall line is created and calculated correctly.
  - Confirming on the invoice that the surcharge is itemized and the final total meets the minimum.
  
  When adopting this policy, communicate the minimum invoice amount to customers in advance and ensure your terms and conditions reflect the surcharge practice. Additionally, test the configuration in a non-production environment to validate rounding behavior, tax handling, and pricing interactions with discounts or promotions. These checks help avoid discrepancies and ensure a smooth billing experience for both staff and customers.
---

# A+W BUSINESS – SETTING UP A MINIMUM INVOICE AMOUNT

> More Information - [AW-214264]

## Customer Account Setup
On a customer record on the 2. Order tab change the Invoicing surcharge / minimum value.
Notice the mode in the image below and have the value as before GST.

- Mode = Min Value (in one item)
- Value = 36.37 (before GST)

## Order Entry
In this instance the system will add a new entry on the order which calculate the shortfall in the order amount.
See red amount in the image below.

## Invoice Example
Finally we can see a print out of the invoice showing a Surcharge for bill of 12.88.
Adding this to the order item amount of 23.49 we have a total of 36.37.
The total of 36.37 was the previous value that was entered against the previous customer setup.
