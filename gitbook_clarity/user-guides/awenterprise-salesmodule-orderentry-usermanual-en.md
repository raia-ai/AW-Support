---
description: "EN-UM-AW_Enterprise-Sales_4_6"
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
