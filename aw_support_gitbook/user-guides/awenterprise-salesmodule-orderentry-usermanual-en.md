---
title: "EN-UM-AW_Enterprise-Sales_4_6"
source: "EN-UM-AW_Enterprise-Sales_4_6.pdf"
tags: ["A+W Enterprise", "Sales Module", "Software Reference", "Order Entry", "Pricing", "Conditions", "Technical Manual", "ERP", "Notes", "Texts"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical software reference guide for the A+W Enterprise Sales module. This document details the various dialogs, fields, and functionalities related to order entry, including managing notes, texts, prices, and conditions for customers, suppliers, articles, and projects."
long_description: "This document is a comprehensive software reference manual for the A+W Enterprise Sales module, version 4.00/03-2020. It provides detailed descriptions of the user interface, focusing on the 'Sales > Order Entry' workflow. The manual is organized into major sections such as 'Notes,' 'Texts,' and 'Prices and Conditions.' Each section breaks down specific dialogs and their components, including header, body, and footer areas. It explains how to manage various types of notes (Customer, Supplier, Project, Article), handle different text types (Header, Footer, Item, Special Texts), and configure complex pricing structures through 'Order Conditions,' 'Order Prices,' and 'Conditions for PCD Processing.' The guide includes navigation paths, technical information about database fields (DB fields), and explanations of specific functionalities like creating phrases, setting up form outputs, and managing post-calculations. It is intended for users and administrators who need to understand the detailed workings of the A+W Enterprise Sales system to configure and operate it effectively."
---

# Software Reference

---
## Notes

On the item level, you can only open the supplier notes in sales if the marked item has the type PO and a supplier is assigned.

You can only edit project notes if a project is assigned to the current document. You can edit the notes in the header and on the item level of a document.

Edit article notes for the current article. You can only edit the article notes on the item level for the selected item.

### Header

These dialogs display only the fields that are relevant for the respective note type.

**Customer** Customer number.
Technical info: display field, DB field: memo.key1

**Supplier** Supplier number.
Technical info: display field, DB field: memo.key1

**Project** Project.
Technical info: display field, DB field: memo.key1

**Article** Article number.
Technical info: display field, DB field: memo.key2

### Body

**(Entry lines for text)** Note text for the selected market partner. Use <Enter> to change to the next text line. Each text line is configured individually, that is, you can specify the priority and the info location for each line.
Technical info: alphanumeric fields, DB fields: memo.text

### Footer

The priority and info location for the current note are displayed in the footer.
The Priority button is described in detail for the Document Notes dialog:
⇨ "Document Notes" on page D-249

Use <Shift>+<F9> to change to the info location:

| Info location | Meaning |
| :--- | :--- |
| **Everywhere** | Information is displayed in the master data, the sales and purchasing documents. |
| **Sales order** | Information is displayed in the master data and the sales documents. |
| **Purchase order** | Information is displayed in all purchasing documents and the master data. |
| **Master data** | Information is only displayed in the master data. |

**Tab. D-9** Settings for the info location

## Customer Article, Supplier Article, Project Article Notes

**Sales > Order Entry > Item level > <Shift> + <F4> >Notes > Customer, Supplier, Project, Article Notes**

*Fig. D-104 Notes about the customer, supplier or project with a particular article*
