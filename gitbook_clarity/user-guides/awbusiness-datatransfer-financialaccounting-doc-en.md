---
description: "EN_AWBusiness_Sales_4_4-3"
---


# Tutorial: Data Transfer

---
## Data Transfer

A+W Business provides interfaces by means of which invoices and credit notes can be transferred to programs for financial accounting (FinAcc).

Data is transferred to FinAcc via number manager. Data transfer can only be started automatically in connection with Syska FinAcc.

**Automatic data transfer**
Data transfer can be automated. There are several options available, e. g. workflow tasks. Which option you can use depends on your system configuration. Should you have any questions regarding this topic, please contact your service contact at A+W Software GmbH.

Transfer of invoices to the FinAcc program is usually triggered manually. The criteria for data transfer are the same for all invoices.

Documents are analyzed and grouped on two levels:

*   The first level compiles all items and BOM components by their PGR combination for statistics.
*   The second level regroups the result another time. The system searches for the corresponding proceeds account. Search keys are the product group, VAT 1, VAT 2 and the document's business type. If there is no such key, a dialog is displayed in which the proceeds account can be entered.

If a key has no entry for the proceeds account, the blank proceeds account will be written in the output file.

Special discounts and surcharges of the product type Services and surcharges belonging to product group 000 will not be transferred but (re)distributed to the corresponding items or BOM components.

---

## Status allocation

In status allocation, you define the minimum status a document must have reached to be transferred to FinAcc.

*Fig. C-210: Example: status for FinAcc transfer*
