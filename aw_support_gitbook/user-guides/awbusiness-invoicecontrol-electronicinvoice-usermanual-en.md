---
description: "EN-UM-AWBusiness_23"
---


# Software Reference

---
## Invoice

> i
> **Exchange rate** If you are using more than one currency, the exchange rate defined in the master data is shown here. It can be changed. If you are using only Euro as a currency, the entry in this field must be 1.

### Fix exchange rate

You can define a different exchange rate for each purchase order. This will be used automatically for price control calculations. You can only change it if it has not been fixed in the purchase order.

-> Sales, "Rate fixed for invoicing" on page C-1557

### Target Number Manager

These two fields are released only if the option Fill target NM is enabled. Invoices will be moved to the defined Number Manager after invoice control, e.g. in order to release them for payment.

-> "Options menu" on page D-2025

**Employee** Name of the employee allocated to the target Number Manager.

**Number manager** Number Manager to which the invoices shall be moved after the check.

### Purchase orders

The list shows all purchase orders included in the Number Manager. If you have used the purchase order numbers as a filter in the P.O. data section, only the corresponding purchase orders will be displayed.

The VAT and foreign currency amount columns are displayed only if a mode with VAT and/or a foreign currency has been selected.

**Total** These fields show the totals of the listed purchase orders and the total VAT amount.

### Underlying VAT record

This field shows the percentage for VAT calculation defined in the purchase order which belongs to this invoice.

-> Sales, "Tax rate" on page C-1636

## Invoice control – items

> Documents > P.O. > Invoice > Invoice control > Items tab

