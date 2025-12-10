---
title: "EN-UM-AWEnterprise_21"
source: "EN-UM-AWEnterprise_21.pdf"
tags: ["Dispatch Control", "A+W Enterprise", "Software Manual", "Logistics", "Racks", "Finished Goods", "Printing", "Workflow", "Help Cards", "Index"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A comprehensive software reference manual for the A+W Enterprise Dispatch Control module. This document details functionalities for managing logistics, including filtering data, handling finished goods stock, and executing various printing tasks. It also provides step-by-step 'Help Cards' for common operational workflows."
long_description: "This document serves as a detailed software reference guide for the A+W Enterprise Dispatch Control module, designed for users involved in logistics and dispatch management. The manual is divided into two primary parts: a Software Reference section and a Help Cards section. The Software Reference section provides in-depth information on core functionalities. It begins by explaining how to use filter conditions for searching data and details the various fields displayed in hit dialogs, such as delivery dates, routes, and order information, complete with technical database field names. It then covers advanced topics like the management of Finished Goods Stock, including procedures for search, overview, inventory management (starting and closing), and viewing booking logs. Another significant part of this section is dedicated to 'Print' functions, outlining the processes for printing loading lists, preliminary and final delivery notes, and other user-defined lists. The second part of the manual consists of 'Help Cards,' which offer practical, step-by-step instructions for performing common tasks. These cards are structured to guide users through workflows such as using the Dispatch Explorer (with and without DC Explorer), editing tours (moving entire tours, orders, or individual items), preparing for dispatch (checking missing quantities, correcting packed quantities, changing addresses, creating delivery notes), and canceling documents. The guide is rich with technical details, including navigation paths, keyboard shortcuts, and database field information, making it an essential tool for both daily operations and system configuration."
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

