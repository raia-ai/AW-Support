---
description: "EN-UM-AWEnterprise_21"
---


# Software Reference

---
## Racks

You can change the filter conditions in all fields as needed:

| Condition | Meaning |
| :--- | :--- |
| **=** | Search exactly for this value (e.g. market partner field = 600004 lists only documents relating to this market partner). |
| **>** | Search for larger values (e.g. market partner field > 600004 lists only documents with market partner numbers larger than 600004). |
| **p** | Search for patterns in text fields (e.g. Reference field Shape 12 lists all documents with the reference text model 12.) |
| **0** | Search for values = 0 (e.g. market partner field 0 lists only market partners with the number 0). |
| **Z** | Search all values in the range. |
| **!** | Search all values except for this value (e.g. Department field! 10 lists all departments except for the department with the number 10). |
| **<** | Search for smaller values (e.g. market partner field < 600004 lists only documents with market partner numbers smaller than 600004). |

**Tab. G-5 Meaning of the filter conditions**

After entry, use `<F3>` to trigger the search action. Insofar as the search was successful, a hit quantity is output on the same dialog. Use `<F2>` to see additional fields for selection.

The following fields are displayed on the hit dialogs:

**Del. date** Delivery date stated in the order.
Technical info: date field, DB field: lapool.ltplan

**Route** Route number.
Technical info: display field, DB field: lapool.routennr

**Order** External order number. For dispatch mode with purchasing documents, the number of the PO is always output here.
Technical info: Display field, DB info: lapool.auftrnr

**Itm** Item number from the order.
Technical info: display field, DB field: lapool.posnr

**Customer** Customer number of the order.
Technical info: Display field, DB info: lapool.kunr

**Project** Project number from the order if there is one.
Technical info: Display field, DB info: lapool.objnr

**Tot.** Total quantity of items that was entered for this order.
Technical info: Display field, DB info: lapool.gesstk

**Call** Number of items the customer has ordered for that date.
Technical info: display field, DB field: lapool.abrufstk

**Pack** Quantity packed for this item.
Technical info: display field, DB field: lapool.iststk

**Width** Height of the lite.
Technical info: display field, DB field: lapool.breite

**Height** Width of the lite.
Technical info: display field, DB field: lapool.laenge

**sqft** Item surface in square feet.
Technical info: display field, DB field: lapool.iststk

**LL** Loading list number if there is already a loading list for this order.
Technical info: Display field, DB info: lapool.llnr

**DN** Indication of whether there is already a delivery note for this order.
Technical info: Display field, DB info: lapool.Isdrukz

**Prod.description** Product description for the order item.
Technical info: Display field, DB info: lapool.artbez1

**Shape** Shape number from the order item if there is one.
Technical info: Display field, DB info: lapool.modnr

**kg** Weight per order item.
Technical info: Display field, DB info: lapool.gewicht

### Footer

The footer of the dialog displays additional information for the following fields:

-   **External customer OrderNr**
-   **Width** (largest value for lite length from the hit quantity)
-   **Height** (largest value for lite height from the hit quantity)
-   **kg** (total weight for all items displayed in the overview)
-   **qm** (total surface for all items displayed in the overview)
-   **Tot.** (total quantity of the units entered for all items displayed in the overview)
-   **Call** (total number of units requested for all items displayed in the overview)
-   **Pack.** (total quantity of packed units for all items displayed in the overview)

### Delivery date changes

Dispatch control – Order level > `<Shift>` + `<F4>` Delivery date changes

