---
title: "A+W Enterprise Sales Software Reference - Notes, Texts, Prices, Conditions, and Release"
source: "EN-UM-AWEnterprise_14.pdf"
tags: ["software reference", "A+W Enterprise", "sales module", "order entry", "pricing", "notes management", "technical writing", "user manual", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a detailed software reference guide for the A+W Enterprise Sales module, covering functionalities related to Notes, Texts, Prices and Conditions, and Order Release. It provides step-by-step instructions and technical details for managing customer, article, and project-specific information within the system."
long_description: "This comprehensive software reference manual details various features within the A+W Enterprise Sales application, specifically focusing on the management of supplemental information and pricing structures. The 'Notes' section explains how to create, display, and edit different types of notes, such as customer notes, article notes, project notes, and document notes, detailing when and how they are displayed to the user. The 'Texts' section covers the management of additional document information, including header/footer texts, article/item texts, special texts (like spacer, product code, logo), and phrases, explaining how these are generated, edited, and printed on various forms. The 'Prices and Conditions' section provides an in-depth look at the price calculation engine, describing how to manage order-specific conditions, various price types (order prices, muntin prices, exchange prices, sub-part prices), and conditions for PCD (Price Code Determination) processing for different glass and article types. Finally, the 'Release' section outlines the process for manually releasing orders that were not automatically processed due to system constraints, such as exceeding credit limits, and the authorization procedures required. The guide includes navigation paths, field descriptions with technical database information, and explanations of system dialogs and configurations."
---

# Software Reference

---
## Notes

You can display and edit notes for documents, market partner, articles, project, and various combinations of these types, e.g. project-article notes.

-   **Customer notes:** These note texts are displayed as soon as the customer is selected.
-   **Customer-article notes:** These note texts are displayed as soon as an article for this customer is selected.
-   **Project-article notes:** These note texts are displayed as soon as the article for this project is selected.
-   **Supplier notes:** These note texts are displayed as soon as the supplier is selected.
-   **Supplier-article notes:** These note texts are displayed as soon as the article for this supplier is selected.

-   "Document notes" on page D-1302
-   "Market partner, project, article notes" on page D-1303
-   "Market partner article notes" on page D-1305

---
*A+W Enterprise Sales*
*D-1301*

---

## Document notes

**Sales > Order Entry > Header, Footer area > <Shift> + <F4> > Document Notes**
**Sales > Order Entry > Item level > <Shift> + <F4> > Notes > Document Notes**

*Fig. D-108 Document notes*

Use this dialog to store notes about the open document. You can enter the document notes in the header and on the item level of a document. You can only store the notes for the current document. They are not stored in the master data.

### Body

**(Entry lines for text)** Note text for the open document. Use `<Enter>` to change to the next text line. Each text line is configured individually; that is, you can specify the priority for each line.
**Technical info:** alphanumeric fields, DB fields: infokauf.atxt

### Footer

The priority for the current note is displayed in the footer.

**Priority**
Changes the priority for the selected text line.
Alternatively, you can change the priority with `<Shift>+<F10>`.

---
*A+W Enterprise Sales*
*D-1302*

---

## Market partner, project, article notes

**Sales > Order Entry > Header, Footer area > <Shift> + <F4> > Market Partner, Project, Article Notes**
**Sales > Order Entry > Header, Footer area > <Shift> + <F4> >Notes > Customer, Supplier, Project, Article Notes**

*Fig. D-109 Market partner, project, article notes*

These dialogs display notes about the market partner, the project or the article. The dialogs are structured the same way. Differences will be described explicitly below.

The note texts are generally created in the master data. If you edit the note texts and add new ones, store them with `<F3>`. The changes are taken over into the master data and the dialog closes.

In sales documents, the customer notes are displayed and in purchasing documents the supplier notes.

On the item level, you can only open the supplier notes in sales if the marked item has the supply type PO and a supplier is assigned.

You can only edit project notes if a project is assigned to the current document. You can edit the notes in the header and on the item level of a document.

Edit article notes for the current article. You can only edit the article notes on the item level for the selected item.

---
*A+W Enterprise Sales*
*D-1303*

---

### Header

These dialogs display only the fields that are relevant for the respective note type.

**Customer** Customer number.
**Technical info:** display field, DB field: memo.key1

**Supplier** Supplier number.
**Technical info:** display field, DB field: memo.key1

**Project** Project.
**Technical info:** display field, DB field: memo.key1

**Article** Article number.
**Technical info:** display field, DB field: memo.key2

### Body

**(Entry lines for text)** Note text for the selected market partner. Use `<Enter>` to change to the next text line. Each text line is configured individually, that is, you can specify the priority and the info location for each line.
**Technical info:** alphanumeric fields, DB fields: memo.text

### Footer

The priority and info location for the current note are displayed in the footer.

The Priority button is described in detail for the Document Notes dialog:
⇨ "Document notes" on page D-1302

Use `<Shift>+<F9>` to change to the info location:

| Info location | Meaning |
| :--- | :--- |
| **Everywhere** | Information is displayed in the master data, the sales and purchasing documents. |
| **Sales order** | Information is displayed in the master data and the sales documents. |
| **Purchase order** | Information is displayed in all purchasing documents and the master data. |
| **Master data** | Information is only displayed in the master data. |

*Tab. D-9 Settings for the info location*

---
*A+W Enterprise Sales*
*D-1304*

---

## Market partner article notes

**Sales > Order Entry > Item level > <Shift> + <F4> >Notes > Customer, Supplier, Project, Article Notes**

*Fig. D-110 Notes about the customer, supplier or project with a particular article*

These dialogs display the notes about the current article for the selected customer, supplier or project. These notes can only be displayed on the item level for the selected item.

The note texts are generally created in the master data. If you edit the note texts and add new ones, store them with `<F3>`. The changes are taken over into the master data and the dialog closes.

Supplier-article notes in sales are only displayed if the marked item has the supply type PO and a supplier is assigned.

Project-article notes are only displayed if a project is assigned to the current document.

### Header

The fields in the header area are described in detail for the Market Partner, Project, and Article Notes dialogs:
⇨ "Market partner, project, article notes" on page D-1303

---
*A+W Enterprise Sales*
*D-1305*

---

### Body

**(Entry lines for text)** Note text about the selected article for the current customer. Use `<Enter>` to change to the next text line. Each text line is configured individually; that is, you can specify the priority and info location for each line.
**Technical info:** alphanumeric field, DB fields: memor.txt

### Footer

The fields and buttons in the footer area are described in detail for the Market Partner, Project, and Article Notes dialogs:
⇨ "Market partner, project, article notes" on page D-1303

---
*A+W Enterprise Sales*
*D-1306*

---

## Texts

Use texts to display additional information about document. The texts are, depending on the text type, either generated by the system according to specifications from the master data and the transaction data or entered manually. You can print out texts with information for customers on different forms. Texts with internal information can be displayed automatically when calling up a document.

Text management depends on the settings in the master data and the respective system configuration.

**For customer-specific adjustments, contact your contact person at A+W Software GmbH.**

The following dialogs are described in this section:

-   "Header and footer texts" on page D-1308
-   "Article and item texts" on page D-1311
-   "Special texts" on page D-1312
-   "Phrases" on page D-1314
-   "External information" on page D-1316
-   "Box signature" on page D-1317

---
*A+W Enterprise Sales*
*D-1307*

---

## Header and footer texts

**Sales > Order Entry > Header, Footer area > <F4> > Texts > Header, Footer Text**
**Sales > Order Entry > Item level > <F4> > Texts > Header, Footer Text**

*Fig. D-111 Header and footer texts*

This dialog displays texts with additional information about the document header or footer. The texts are generated from the master data using the text management. The text management is described for the Master Data part:
⇨ Master Data, "Text Management" on page B-506

You can edit the texts with reference to documents and add set phrases.

The texts can be printed out on different forms. You can change the selection of the appropriate forms on the right side of the Texts dialog in the Forms area.

### Header text tab

**(Entry lines for text)** Information text about the header area. Use `<Enter>` to change to the next text line.
**Technical info:** alphanumeric fields, DB fields: auftxt.txt

### Footer tab

**(Entry lines for text)** Information text about the footer area. Use `<Enter>` to change to the next text line.
**Technical info:** alphanumeric fields, DB fields: auftxt.txt

---
*A+W Enterprise Sales*
*D-1308*

---

### Forms

In the forms area, you specify on which form types the information text is output.
☑ The information text is printed on the selected form. In the database, the value 1 is assigned.
☐ No information text is printed on the form. In the database, the value 0 is assigned.
**Technical info:** checkboxes, DB fields: auftxt.formular

> **Database reference for forms**
> In the database, all entries are saved per form in a form vector. All forms are specified in the sequence indicated under the corresponding number in the form vector (no. in the form types table).
> If a 1 is assigned to a form, then it is printed. If a 0 is assigned, the form will not be printed.

| No | Field contents | Meaning |
| :-- | :--- | :--- |
| 1 | Quotat. | Text will be printed on the quotation. |
| 2 | OC | Text will be printed on the order confirmation. |
| 3 | Inquiry | Text will be printed on the request for quotation to the supplier. |
| 4 | Invoice | Text will be printed on the invoice. |
| 5 | Credit Nte | Text will be printed on the credit note. |
| 6 | Manual cutting list | Text will be printed on the manual cutting list. |
| 7 | Deliv. Note | Text will be printed on the delivery note. |
| 8 | Production | Text will be printed on the production paperwork. |
| 9 | P.O. | Text will be printed on the P.O. |
| 10 | Muntins Doc. | Text will be printed on the muntin documents. |
| 11 | Work order | Text will be printed on the work order. |
| 12 | Label | Text will be printed on the labels. |
| | Spacer text | Text will be printed on the production paperwork. |

*Tab. D-10 Form types*

---
*A+W Enterprise Sales*
*D-1309*

---

### Footer

**Phrases**
Opens the Phrases dialog to select existing set phrases.
⇨ "Phrases" on page D-1314

**New Phrases**
Opens the New Phrases dialog on which you create your own phrases.
⇨ "Phrases" on page D-1314

---
*A+W Enterprise Sales*
*D-1310*

---

## Article and item texts

**Sales > Order Entry > Item level > <F4> > Texts > Article Text, Item Text**

*Fig. D-112 Article and item texts*

This dialog displays texts with additional information about the articles or items of a document.

The texts are generated from the master data and according to the system settings. The text management is configured customer-specifically and is described in the Master Data part:
⇨ Master Data, "Text Management" on page B-506

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

You can edit the texts with reference to documents and add set phrases. If you have selected phrases for the article or item text, you can edit these document-specifically.

The texts can be printed out on different forms. You can change the selection of the appropriate forms on the right side of the dialog in the Forms area.

---
*A+W Enterprise Sales*
*D-1311*

---

### Article Text tab

**(Entry line for text)** Information text about the selected article. Use `<Enter>` to change to the next text line.
**Technical info:** alphanumeric fields, DB fields: auftxt.txt

### Item Text tab

**(Entry line for text)** Information text about the selected item. Use `<Enter>` to change to the next text line.
**Technical info:** alphanumeric fields, DB fields: auftxt.txt

### Forms

This area is described in detail for the Header and Footer Texts dialog.
⇨ "Header and footer texts" on page D-1308

### Footer

This area is described in detail for the Header and Footer Texts dialog.
⇨ "Header and footer texts" on page D-1308

## Special texts

**Sales > Order Entry > Item level > <F4> > Texts > Special Texts > Spacer Text, Product Code, Shape Text, Logo Text**

*Fig. D-113 Special texts*

These dialogs display special texts about the individual articles. The special texts are generated by the system using the master data. The text management depends on the settings in the master data and the respective system configuration. Depending on the configuration, you can edit the texts document-related.

---
*A+W Enterprise Sales*
*D-1312*

---

The dialogs are only enabled customer-specifically.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

A text number is assigned to each text. Under some circumstances, the text number is transferred to production if it is needed there.

| Text type | Description | Text number |
| :--- | :--- | :--- |
| **Spacer Text** | Additional information about the frame text that is printed on the frame. | 1000 |
| **Product code** | Additional information about the product code, e.g. CEKAL certification mark. | 1003 |
| **Shape text** | Additional information about the shape. The parameters of the shape are displayed as text for each item.<br>You can enter a shape text only for items with shaped lite. | 1002 |
| **Logo text** | Additional information about the logo. You can enter a logo text only for items with a processing with logo. | 1010 |
| **Box signature texts** | Box signature for dispatch.<br>⇨ "Box signature" on page D-1317 | Starting with 5000 |

*Tab. D-11 Special texts*

---
*A+W Enterprise Sales*
*D-1313*

---

## Phrases

**Sales > Order Entry > Item level > <F4> > Texts > Header, Footer Text, Article Text, Item Text > [New Phrases]**

*Fig. D-114 Phrases*

Use this dialog to create or edit phrases. Phrases are default texts that are stored in the master data.

Phrases can be used in the header, footer, article, item texts, and the special texts as pre-formulated text modules.

On the right side of the dialog, you select the types of forms on which the phrases should be printed.
**Technical info:** alphanumeric fields, DB field: floskel.code, floskel.txt
⇨ "Forms" on page D-1309

**Code** Code and description of the phrase. If you enter the code for an existing phrase, the description will be displayed in plain text.
**Technical info:** alphanumeric fields, DB field: floskel.code, floskel.txt

**(Entry line for text)** Default text that is assigned to the phrase.
**Technical info:** alphanumeric fields, DB fields: floskel.txt

> **Editing existing phrases**
> If you enter the code for an existing phrase, you can edit and then take over this phrase.

If you click on [Phrases] in the footer area of the text dialogs, a search dialog opens on which you can search for existing phrases.

---
*A+W Enterprise Sales*
*D-1314*

---

*Fig. D-115 Selection of the phrases*

**Code** Code of the phrase. Use [Search] to display all existing phrases on a separate dialog. If you select a phrase, the phrase text is displayed in the entry lines of the current text dialog.
**Technical info:** alphanumeric field, DB field: floskel.code

---
*A+W Enterprise Sales*
*D-1315*

---

## External information

**Sales > Order Entry > Header, Footer area, Item level > <F4> > Texts > External Information**

*Fig. D-116 External information*

Use this dialog to store external information. External information is information about the further document processing that should be transmitted internally to various departments.

**External no.** Customer-side document description under which the customer keeps this document. The entry is taken over into the Cust.PONo. field. With the Cust.PONo. you can search for orders.
**Technical info:** alphanumeric field, DB field: kauf.exaufnr

> **Open document via the external no.**
> If you want to open a document via the external number, in the order entry you can change to the Document No. field with `<F5>` to the Cust.PONO. field. If you enter the external number and confirm with `<Enter>`, all documents with this external number are displayed. If you select an entry, the corresponding document opens.

**Purch. info** Information text that is transferred to the Purchasing department. The information can be displayed in the order pool. Use `<End>` to save the data and close the dialog.
**Technical info:** alphanumeric field, DB field: kauf.exbez1

**Dispatch info** Information text that is transferred to dispatch control. The dispatch info is displayed in the dispatch control on the item level. Use `<End>` to save the data and close the dialog.
**Technical info:** alphanumeric field, DB field: kauf.exbez2

---
*A+W Enterprise Sales*
*D-1316*

---

## Box signature

**Sales > Order Entry > Header, Footer area, Item level > <Shift> + <F4> > Box Signature**

*Fig. D-117 Box signature*

This dialog displays the box signature for dispatch. The box signature is required for dispatch control and is generated automatically.

The functions depend on the settings in the master data and the respective system configuration. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

On the dialog, each box side can be assigned texts. The texts are generated from the master data using text formulas.

The Text Formulas dialog is described in the Master Data section:
⇨ Master Data, "Text formulas" on page B-514

The assignment of the box signature is stored in the master data.

The Descriptions of Box Signature dialog is described in the Master Data section:
⇨ Master Data, "Descriptions for box signature" on page B-355

Use `<F3>` to generate the box signature. Here the data is drawn from the master data. If the box signature in the master data has changed, the data in the document entry is updated accordingly.

---
*A+W Enterprise Sales*
*D-1317*

---

You can edit the box signature order by order.

-   **Arrang.:**
    Print position of the signature on the box:
    -   front
    -   back
    -   top
    -   bottom
    -   left
    -   right
    **Technical info:** alphanumeric field, DB field: artkennfrm.formelbez
-   **Seq.:**
    Sequence number. On each box side, several texts can be printed, each on their own line. The sequence number determines the sequence in which the texts are printed. The text with the sequence number 1 is printed in the first line, the text with the sequence number 2 in the second line, etc.
    **Technical info:** numeric field, DB field: infokauf.seqnr
-   **Text:**
    Labeling text for box signature. If you have stored the box signatures in the master data, the text is displayed automatically. You can overwrite the text from the master data.
    **Technical info:** alphanumeric field, DB field: infokauf.atxt

---
*A+W Enterprise Sales*
*D-1318*

---

## Prices and Conditions

For the price calculation in the document, the article prices and market partner conditions from the master data are used. Individual prices and conditions can be edited with reference to a document.

For a detailed description, see the Prices and Conditions section.

The following dialogs are described in this section:

-   "Order conditions" on page D-1320
-   "Order prices" on page D-1325
-   "Order muntin prices" on page D-1327
-   "Order exchange prices" on page D-1330
-   "Order sub-part prices" on page D-1332
-   "Post calculation" on page D-1334
-   "Step prices" on page D-1337
-   "Conditions for PCD processing" on page D-1338
-   "Production cost calculation" on page D-1371
-   "Price calculation" on page D-1378

---
*A+W Enterprise Sales*
*D-1319*

---

## Order conditions

**Sales > Order Entry > Item level > `<F4>` > Price Info > Order Conditions**
**Sales > Order Entry > Header, Footer area > `<F4>` > Price Info > Document Conditions**

*Fig. D-118 Order conditions*

Use this dialog to store order-related prices and conditions. You can specify various criteria for price calculation for the following components:

-   Glass types
-   Muntins
-   Colored products
-   Accessories
-   Processings
-   Glazing

Enter the values for the sales and purchase prices separately. The Sales and Purchasing tabs are structured similarly. Differences will be described explicitly below.

### Header

**Order** Number of the selected order.
**Technical info:** display field, DB field: kauf.auftrnr

**Condit.debtor** Customer ID of the customer to whom the conditions apply. If you want to work without condition debitor, you have to confirm the message that appears when you exit the field with [Yes]. The field is only displayed if the Sales tab is open.
**Technical info:** numeric field, DB field: aufkond.kalkkunr

### Sales and purchasing

This tab displays the sales or purchasing prices for the various price methods.

**IG, Tmp, LAM, Bas.Glass, Processing, Col.Product, Prices-gen.** These values apply to the articles to which the price method in question is assigned.
⇨ Prices and Conditions, "Pricing methods" on page C-559

**Muntins** These values apply to the articles to which the price method muntin prices is assigned. No scaled stages can be specified for muntins.

You can specify different calculation criteria for each article group:

-   **PCD:**Price code with which the prices are determined. The PCD refers to a price list in which the prices for the articles with the price methods in question are defined.
    **Technical info:** numeric fields, DB fields: aufkond.isopkz, aufkond.pkzesgp-kz, aufkond.pkzvsgpkz, aufkond.pkzbaspkz, aufkond.pkzverpkz, aufkond.pkzfarbpkz, aufkond.pkzallpkz, aufkond.sprospkz
-   **SC:** Surcharge in percent. The surcharge is assessed on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is calculated.
    **Technical info:** numeric fields, DB fields: aufkond.isotz, aufkond.pkzesgtz, aufkond.pkzvsgtz, aufkond.pkzbastz, aufkond.pkzvertz, aufkond.pkzfarbtz, aufkond.pkzalltz, aufkond.vksprtz
-   **Factor:** Factor of the surcharge. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
    **Technical info:** numeric fields, DB fields: aufkond.isofaktor, aufkond.pkz-esgfakt, aufkond.pkzvsgfakt, aufkond.pkzbasfakt, aufkond.pkzverfakt, aufkond.pkzfarbfakt, aufkond.pkzallfakt, aufkond.sprosfakt
-   **Offs.:** Specification of the price scale level from which the price for the glass type or price method in question is determined.
    **Technical info:** numeric fields, DB fields: aufkond.pkzesgstaff, aufkond.pkzvsgstaff, aufkond.pkzbasstaff, aufkond.pkzverstaff, aufkond.pkzfarbstaff, aufkond.pkzallstaff
-   **Tpe:** Selection of the calculation type according to which the muntin prices are calculated. The calculation types are described for the Item Conditions – Muntin Prices tab:
    ⇨ "Item conditions - muntin prices" on page D-1368
    **Technical info:** numeric field, DB field: aufkond.sprosart
-   **Special surch.:** Price surcharge for special orders. In the second field, you specify the price type. The price type determines to what the price refers:
    -   **CU/piece:** The price applies per piece.
    -   **CU/m2:** The price applies per square meter.
    -   **Percent:** The price is calculated as percentage on the base price.
    These fields are only displayed on the Sales tab.
    **Technical info:** numeric field, toggle field, DB fields: aufkond.isosonderzu, aufkond.isosonderzutyp
-   **Tot.surch.:** Percentage surcharge that is charged on the total price. This field is only displayed on the Sales tab.
    **Technische Info:** numerische Felder, DB-Felder: aufkond.isozuschlag, aufkond.pkzesggeszu, aufkond.pkzvsggeszu, aufkond.pkzbastgeszu, aufkond.pkzvergeszu, aufkond.pkzfarbgeszu, aufkond.pkzallgeszu

### Surcharge and factor

Additionally, you can specify surcharges and factors for individual components. Enter the surcharge in the first field and the factor in the second field.

**Accessory SC factor** Percentage surcharge and factor for accessory articles. The fields are display on the Sales and Purchasing tabs.
**Technical info:** numeric fields, DB fields: aufkond.zubetz, aukond.zubef, aufkond.ekzubetz, aukond.ekzubef

### Processings (sales tab)

On the Sales tab, for surcharge and factor, you can specify different values for the respective corner, edge or surface processing of TG and basis glass.

**TG SC factor** Surcharge and factor for processing on single-lite safety glass.

**Bas.glass SC factor** Surcharge and factor for processings on basis glass.
You can specify the surcharge and factor for various processing. The surcharge is taken into consideration in the price calculation.

-   **Corners:** Corner processings, e.g. corner cut-off.
    **Technical info:** numeric fields, DB fields: aufkond.esgbecktz, esgbeckf, verbecktz, verbeckf
-   **Edges:** Edge processings, e.g. polishing.
    **Technical info:** numeric fields, DB fields: aufkond.esgbkantz, esgbkanf, verbkantz, verbkanf
-   **Area:** Edge processings, e.g. coating.
    **Technical info:** numeric fields, DB fields: aufkond.esgbflatz, esgbflaf, verbflatz, verbflaf

### Processings (purchasing tab)

On the Purchasing tab, for surcharge and factor, you can specify different values for the processing of TG and basis glass.

**TG SC factor** Surcharge and factor for processing on single-lite safety glass.
**Technical info:** numeric fields, DB fields: aufkond.ekesgbtz, ekesgbfakt

**Bas.glass SC factor** Surcharge and factor for processings on basis glass.
**Technical info:** numeric fields, DB fields: aufkond.ekeverbtz, ekverbfakt

### Special costs

**Glazing price** Price of the glazing work in currency unit.
**Technical info:** numeric field, DB field: aufkond.verglaseins, aufkond.verglaseinsek

**Sealing price** Price of the sealing work in the currency unit.
**Technical info:** numeric field, DB field: aufkond.verglasversieg, aufkond.verglasversiegek

**Enter minim. price** Minimum price of the glazing or sealing work.
**Technical info:** numeric field, DB field: aufkond.verglasmineins, aufkond.verglasmineinsek

**Round price/pc.** Specification of how the piece price should be rounded.
-   If 100 is specified, the price is rounded to the next full currency amount.
-   If 10 is specified, the price is rounded to the next tenth currency amount.
**Technical info:** numeric fields, DB fields: aufkond.stkprsrund, aufkond.ekstk-prsrund

**AIR surch.** Specification of whether a surcharge should be calculated for the airspace.
-   **Y:** The AIR surcharge will be charged if the AIR underruns the millimeter levels specified in the assigned IG article.
    ⇨ Prices and Conditions, "AIR surcharges" on page C-736
-   **N:** The AIR surcharge will not be charged.
This field is only displayed on the Sales tab. **Technical info:** toggle field, DB field: aufkond.szrflag

**Step surcharge** Price surcharge for step processing. In the second field you specify the surcharge type. The surcharge type specifies to what the surcharge relates:
-   **CU/pc ne:** The step surcharge is charged according to calculation of the factor as fixed net amount per step.
-   **CU/pc gr:** The step surcharge is charged as gross amount per step before calculation of the factor.
-   **Percent:** The step surcharge is charged as a percent of the glass quantity unit price and the replacement prices.
-   **%/piece:** The step surcharge is charged per step as a percent of the glass quantity unit price and the replacement prices.
**Technical info:** numeric field, toggle field, DB fields: aufkond.stufzuvk, aufkond.stufzutypvk, aufkond.stufzuek, aufkond.stufzutypek

**MinCal TSG/LSG in IG** Minimum calculation for TSG or LSG in IG panes. The value for the TG is entered in the first field, the value for LAMI in the second field. This field is only displayed on the Sales tab.
**Technical info:** numeric fields, DB fields: aufkond.minesginiso, aufkond.minvsginiso

**Min.for calcul.** Number of quantity units in pieces, square meters, etc. for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is calculated. This field is only displayed on the Sales tab.
**Technical info:** numeric field, DB field: aufkond.minber

**Round. size** Specification of the dimension rounding in millimeters for price calculation of the article. The edge lengths in the order item will be rounded to the next higher value in millimeters that is divisible by the specified dimension rounding for the price calculation. This information is not considered in production. This field is only displayed on the Sales tab.
**Technical info:** numeric field, DB field: aufkond.massrund

---
*A+W Enterprise Sales*
*D-1320, D-1321, D-1322, D-1323, D-1324*

---

## Order prices

**Sales > Order Entry > Header, Footer area, Item level > `<F4>` > Price Info > Order Prices > Article Prices**

*Fig. D-119 Order prices*

Use this dialog to store or change the article prices depending on the order. If, for example, if you purchase an article more cheaply due to a quantity discount than at the prices stored in the master data, the prices have to be changed manually for the order so that the correct profit margin can be calculated.

-   **Condit. type:** Type of the granted special condition.
    -   **Customer:** The price for the selected article is calculated according to customer-specific conditions.
    -   **Material costs:** The specified material costs will be calculated on the selected article.
    **Technical info:** mandatory field, toggle field, DB field: aufpreise.kondkz
-   **Article, Description:** Article and description of the article for which the special condition applies.
    **Technical info:** mandatory field, numeric field, alphanumeric field, DB fields: aufpreise.artnr, artikel.artbez1
-   **Price:** Price of the article.
    **Technical info:** numeric field, DB field: aufpreise.preis
-   **Price type:** Specification of to what the price refers:
    -   **CU/piece:** Price that is calculated per piece.
    -   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
    **Technical info:** toggle field, DB field: aufpreise.preistyp
-   **Factor:** Factor of the surcharge in percent. Generally a discount is granted with a factor.
    **Technical info:** numeric field, DB field: aufpreise.faktor

Switch to the Detail view using `<F2>`.

Most fields in the detail view correspond to columns in the overview. In addition, the following fields are displayed:

**Min.for calcul.** Number of quantity units in pieces, square meters, etc. for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is calculated.
**Technical info:** numeric field, DB field: aufpreise.minber

**Round size** Specification of the dimension rounding in millimeters for price calculation of the article. The edge lengths in the order item will be rounded to the next higher value in millimeters that is divisible by the specified dimension rounding for the price calculation. This information is not considered in production.
**Technical info:** numeric field, DB field: aufpreise.massrund

**Min.edge length** Specification of the edge length in millimeters for the price calculation. This size is used if the height or width of the glass in the order item is smaller than this minimum edge length.
**Technical info:** numeric field, DB field: aufpreise.minkant

The article prices are described in detail in the Prices and Conditions section:
⇨ Prices and Conditions, "Article prices" on page C-899

---
*A+W Enterprise Sales*
*D-1325, D-1326*

---

## Order muntin prices

**Sales > Order Entry > Header, Footer area, Item level > `<F4>` > Price Info > Order Prices > Muntin Prices**

*Fig. D-120 Order muntin prices*

Use this dialog to store or change the muntin prices depending on the order.

-   **Article:** Article number.
    **Technical info:** numeric field, DB field: aufspropr.artnr
-   **Calc. Type:** Selection of the calculation type according to which the muntin prices are calculated:
    -   **1 - Fields:** The price is calculated per field.
    -   **2 - LM+C+E:** The price is calculated per linear meter, per crossing, and per edge connection.
    -   **3 - LM:** The price is calculated per linear meter.
    -   **4 - LM+C:** The price is calculated per linear meter and per crossing.
    -   **5 - LM+E:** The price is calculated per linear meter and per edge connection.
    -   **6 - C:** The price is calculated per crossing.
    -   **7 - C+E:** The price is calculated per crossing and per edge connection.
    -   **8 - E:** The price is calculated per edge connection.
    -   **9 - Special:** This form of calculation is configured customer-specifically.
    -   **10 - Percent:** The price is calculated as a percentage from the base price of the head article. The percentage is specified in the detail view in the Percent field.
    -   **11 - sqm price:** The price is calculated per square meter of the glass. The price is specified in the Sq m price field.
    -   **12 - field+LM:** The price is calculated per linear meter and per crossing.
    -   **13 - piece:** A total price is calculated for the muntin pattern. The price is specified in the detail view in the Piece price field.
    -   **14 - C or LM:** The price is calculated per crossing or per linear meter.
        -   If crossing points arise on the muntin pattern, the muntins are calculated according to the number of crossings.
        -   If there are no crossing points, the muntins are calculated based on linear meters.
    -   **15 - field+C+E:** The price is calculated field, per crossing, and per edge connection.
    **Technical info:** mandatory field, numeric field, DB field: aufspropr.berart

The following fields are only considered per calculation type:

-   **Lin.meter:** Specification of the price per linear meter. The price is evaluated for the calculation types LM, LM+C+E, LM+C, LM+E, field+LM, and Special.
    **Technical info:** numeric field, DB field: aufspropr.plm
-   **Cross:** Specification of the price per crossing point. The price is evaluated for the calculation types C, C+E, LM+C, LM+C+E, C or LM, field+C+R, and Special.
    **Technical info:** numeric field, DB field: aufspropr.pkr
-   **Edge:** Specification of the price per edge connection. The price is evaluated for the calculation types E, LM+C+E, LM+E, C+E, field+C+E, and Special.
    **Technical info:** numeric field, DB field: aufspropr.pra
-   **Fields:** Specification of the price per field. The price is evaluated for the calculation types Fields, Field+LM, Field+C+E, and Special.
    **Technical info:** numeric field, DB field: aufspropr.pfe

Switch to the Detail view using `<F2>`.

Most fields in the detail view correspond to columns in the overview. In addition, the following fields are displayed:

**Fields2** Specification of the price per field if there are crossing points in the muntin pattern. The price is calculated with the calculation type Special.
**Technical info:** numeric field, DB field: auspropr.pfe2

**Percent** Specification of the percentage. The price is evaluated with the calculation types percent and special.
**Technical info:** numeric field, DB field: auspropr.prozent

**Square meter** Specification of the square meter price. The price is evaluated with the calculation type sqm price.
**Technical info:** numeric field, DB field: aufspropr.qmpreis

**Item price** Specification of the item price. The price is evaluated with the calculation type Piece.
**Technical info:** numeric field, DB field: auspropr.stckpreis

**Min. lin. meter** Specification of the muntin length in meters, for which the price is calculated at a minimum. The price is evaluated with the calculation type LM.
**Technical info:** numeric field, DB field: aufspropr.minlm

**Min. no. of fields** Specification of muntin fields for which the price is calculated. The price is evaluated with the calculation type fields.
**Technical info:** numeric field, DB field: auspropr.minfeld

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: aufspropr.faktor

For a detailed description of the muntin prices, see the Prices and Conditions section.
⇨ Prices and Conditions, "Muntin prices" on page C-918

---
*A+W Enterprise Sales*
*D-1327, D-1328, D-1329*

---

## Order exchange prices

**Sales > Order Entry > Header, Footer area, Item level > `<F4>` > Price Info > Order Prices > Exchange Prices**

*Fig. D-121 Order exchange prices*

On this dialog, you store or edit the prices for an order article by article, which are exchanged or added within the BOM.

-   **Type:** Product of the article whose price is exchanged.
    -   **IG exchange:** The exchange price is used if the article in an IG is exchanged.
    -   **LAMI exch./addition:** The exchange price is used if the article in a LAMI safety glass is exchanged or entered.
    -   **LAMI exchange:** The exchange price is used if the article in laminated safety glass is exchanged.
    -   **LAMI addition:** The exchange price is used if the article in a LAMI safety glass is added.
    **Technical info:** toggle field, DB field: aufaustpr.austkz
-   **Article, Designation:** Number and description of the article. If you specify a number, the description is displayed in plain text.
    **Technical info:** mandatory field, numeric field, display field, DB fields: aufaustpr.artnr, artikel.artbez1
-   **Price:** Price for the exchange glass.
    **Technical info:** numeric field, DB field: aufaustrpr.preis
-   **Price type:** Specification of to what the price refers.
    -   **CU/m2:** The price applies per square meter.
    -   **Percentage:** The surcharge is calculated as a percentage of the basic glass price.
    **Technical info:** toggle field, DB field: aufaustpr.preistyp

Switch to the Detail view using `<F2>`.

Most fields in the detail view correspond to columns in the overview. In addition, the following fields are displayed:

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: aufaustrpr.faktor

**Min.for calcul.** Specification of the minimum surface in square meters for which the price is calculated. If the area of the exchange glass is smaller than the minimum calculation area, the price for this minimum calculation area is used.
**Technical info:** numeric field, DB field: aufaustpr.minber

**Round size** Specification of the dimension rounding in millimeters for price calculation of the article. The edge lengths in the order item will be rounded to the next higher value in millimeters that is divisible by the specified dimension rounding for the price calculation. This information is not considered in production.
**Technical info:** numeric field, DB field: aufaustrpr.massrund

For a detailed description of the exchange and additional prices, see the Prices and Conditions section.
⇨ Prices and Conditions, "IG exchange prices" on page C-930
⇨ Prices and Conditions, "LAMI exchange/additional prices" on page C-963

---
*A+W Enterprise Sales*
*D-1330, D-1331*

---

## Order sub-part prices

**Sales > Order Entry > Header, Footer area, Item level > `<F4>` > Price Info > Order Prices > Sub-Part Prices**

*Fig. D-122 Order sub-part prices*

Use this dialog to store or change the prices for sub-parts depending on the order.

-   **Article, Designation:** Number and description of the article.
    **Technical info:** mandatory field, numeric field, display field, DB fields: kspross.artnr, artikel.artbez1
-   **Price:** Price of the sub-part.
    **Technical info:** numeric field, DB field: aufuteilpr.preis
-   **Type:** Specification of to what the price refers.
    -   **CU/piece:** The price applies per piece.
    -   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
    **Technical info:** toggle field, DB field: aufuteilpr.preistyp

Switch to the Detail view using `<F2>`.

Most fields in the detail view correspond to columns in the overview. In addition, the following fields are displayed:

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: aufuteilpr.faktor

**Minim. calcul.** Number of quantity units in pieces, square meters, etc. for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is calculated.
**Technical info:** numeric field, DB field: aufuteilpr.minber

**Round size** Specification of the dimension rounding in millimeters for price calculation of the article. The edge lengths in the order item will be rounded to the next higher value in millimeters that is divisible by the specified dimension rounding for the price calculation. This information is not considered in production.
**Technical info:** numeric field, DB field: aufuteilpr.massrund

---
*A+W Enterprise Sales*
*D-1332, D-1333*

---

## Post calculation

**Sales > Order Entry > Header, Footer area, Item level > `<F4>` > Price Info > Post Calculation**

*Fig. D-123 Post calculation*

Use this dialog to store order-related conditions for the sales and purchasing prices.

-   Use `<F3>` to calculate the prices with the new conditions. The values of the recalculation will be taken over into the item conditions.

If you edit the value, they are taken over into the corresponding price conditions. The technical information and database reference of the fields correspond to the respective price conditions.
⇨ "Conditions for PCD processing" on page D-1338

### Header

**Bill of material (BOM)** Number of the BOM for which the conditions should be specified.
**Technical info:** numeric field, DB field: kpos.poskonr

**Download conditions** Specification whether the conditions for price determination should be drawn from the master data.
-   **Y:** The conditions from the master data are used for price determination. The specified values in the body are overwritten by the values from the master data if the corresponding value was stored in the master data.
-   **N:** The conditions from the master data are not used. You can specify the conditions order-related in the body.
**Technical info:** toggle field

### Sales and purchase

You can specify a value apiece for Sales and for Purchasing for the following fields.

**Basic price** Basic price of the article. In the second field, you specify the price type. The price type determines to what the price refers:
-   **CU/piece:** The price applies per piece.
-   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
**Technical info:** numeric field

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric field

**SC** Surcharge in percent. The surcharge is assessed on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is calculated.
**Technical info:** numeric field

**Processing factor** Factor for processings in percent.
**Technical info:** numeric field

**Processing surcharge** Surcharge for processings in percent.
**Technical info:** numeric field

**Accessory factor** Factor for accessory items in percent.
**Technical info:** numeric field

**Accessory SC** Surcharge for accessory articles in percent.
**Technical info:** numeric field

**Muntins SC** Surcharge for muntin articles in percent.
**Technical info:** numeric field

**Muntin calcul. type** Selection of the calculation type according to which the muntin prices are calculated.
The calculation types are described for the Item Conditions – Muntin Prices tab.
⇨ "Item conditions - muntin prices" on page D-1368
**Technical info:** numeric field

**Glazing price** Price of the glazing per square meter.
**Technical info:** numeric field

**Min. price glazing** Minimum price that is calculated for the glazing. If in the order the price of the glazing for an article is less than the specified minimum price, the minimum price will be charged.
**Technical info:** numeric field

**Sealing price** Price for sealing per square meter.
**Technical info:** numeric field

**Min. price sealing** Minimum price that is calculated for the sealing. If in the order the price of the sealing for an article is less than the specified minimum price, the minimum price will be charged.
**Technical info:** numeric field

### Exchange

-   **IG_Exchange, Description:** Number and description of the exchange article.
    **Technical info:** mandatory field, numeric field, display field
-   **Sales fact:** Factor for the sales price of the surcharge in percent.
    **Technical info:** numeric field
-   **SalesPrc:** Sales price of the article in percent.
    **Technical info:** numeric field
-   **PU factor:** Purchase price factor of the surcharge in percent.
    **Technical info:** numeric field
-   **Pu. Price:** Purchase price of the article. **Technical info:** numeric field

---
*A+W Enterprise Sales*
*D-1334, D-1335, D-1336*

---

## Step prices

**Sales > Order Entry > Items tab > Enter stepped article > Price field > `<Shift>` + `<F9>` > `<F8>`**

*Fig. D-124 Step prices*

Enter scaled prices for stepped articles on this dialog, e.g. for IG articles.

-   **SA/PU:** These entries are intended for Purchasing or Sales.
-   **from step width (mm):** Value of the step width in millimeters, e.g. €3.50 from a step width of 100 mm and €7.80 from a step width of 200 mm.
-   **Pieces:** Number of steps for calculation.
-   **Surch.:** Value of the step surcharge in currency units, e.g. in euros.
-   **Surch. type:** Calculation type of the scaled surcharge for steps.
    -   **CU/m2 =** Price (currency unit) for scaling the step width is multiplied by the number of steps and the value of the Surcharge field. This value is added to the glass price.
    -   **CU/piece/m2 net:** Scaling of the step width is multiplied by the number of steps and the value of the Surcharge field. The result is multiplied by the area of the surrounded rectangle of the article and added to the unit price.

---
*A+W Enterprise Sales*
*D-1337*

---

## Conditions for PCD processing

**Sales > Order Entry > Items tab > Price field > `<Shift>` + `<F9>`**

These dialogs display the price conditions of an item article.

The dialogs are divided into two tabs or areas, which display the price conditions for sales and purchasing. The Purchasing tab is only enabled if the supply type PO or Included is selected for the item. The structure of the tabs and areas differs depending on which price method is assigned to the item article. The values are displayed that are relevant for the price calculation.

The individual price methods are described in detail in the Prices and Conditions section:
⇨ Prices and Conditions, "Pricing methods" on page C-559

You can edit the values for the price conditions. If you would like to recalculate the price, close the dialog. A query is displayed asking whether you would like to recalculate the price. If you confirm the query, the prices will be calculated with the document-related item conditions.

The following dialogs are described in this section:

-   "Conditions for PCD, PCD BASIC GLASS processing" on page D-1339
-   "Conditions for PCD BASIC GLASS" on page D-1343
-   "Conditions IG" on page D-1345
-   "Conditions IG (SWITZERLAND)” on page D-1350
-   "Conditions for PCD COLORED ARTICLE” on page D-1354
-   "Conditions for PCD PRICES GENERAL" on page D-1356
-   "Conditions for PCD GLASS DOORS" on page D-1358
-   "Conditions for manual prices" on page D-1361
-   "LAMI exchange/additional prices" on page D-1363

Depending on which price-relevant processings are included in the item's BOM, the Processing Prices (SA), (PU) and Muntin Prices tabs are enabled. The price properties for processing prices are specified in the master data.
⇨ Master Data, "Price characteristics" on page B-444

The Processing Prices (SA), (PU) and Muntin Prices tabs will be described separately.

The following tabs are also described in this section:

-   "Item conditions - processing prices" on page D-1365
-   "Item conditions - muntin prices" on page D-1368

---
*A+W Enterprise Sales*
*D-1338*

---

### Conditions for PCD, PCD BASIC GLASS processing

**Sales > Order Entry > Items tab > Price field of item article with price method PCD basic glass, PCD Processing > `<Shift>` + `<F9>`**

*Fig. D-125 Conditions for PCD, PCD BASIC GLASS processing*

This dialog displays the price conditions for an item article to which the price method PCD Basic Glass or PCD Processing is assigned. You can edit the price conditions.

On the Conditions for PCD BASIC GLASS and Conditions for PCD Processing dialogs, the Sales and Purchasing dialogs are largely the same. The Total Surcharge field is not displayed on the Purchasing tab.

If additional processing are included in the item's BOM, then the Processing Prices (SA), (PU) tabs are enabled:
⇨ "Item conditions - processing prices" on page D-1365

If muntins are included in the item's BOM, then the Muntin Prices tab is enabled:
⇨ "Item conditions - muntin prices" on page D-1368

#### Header

**SA PCD** Price code for the pre-defined price list for sales.
**Technical info:** mandatory field, numeric field, DB field: pokokon.pkz

**PU PCD** Price code for the pre-defined price list for purchasing.
**Technical info:** mandatory field, numeric field, DB field: pokokon.ekpkz

**Vector** Number of the vector from which the price should be drawn.
**Technical info:** mandatory field, numeric field, DB field: pokokon.matnr

#### Sales, purchasing tabs

**Price type** Type of pricing. By default, the price type Single Price is selected. The field is a display field. If you change the glass or basic price or enter the price in the item without performing a price calculation, then Manual Price is displayed as price type.
**Technical info:** display field, DB field: pokokon.flag6

**Scal. level** Price level from which the price is used. The field is only evaluated by the price calculation if the price type 2 - Scaling Level is specified for the relevant article price vector.
**Technical info:** numeric field, DB field: pokokon.flag1, pokokon.ekflag1

**Price type** Indication of what the specified price refers to.
-   **CU/piece:** The price applies per piece.
-   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
**Technical info:** toggle field, display field

**Glass price** Basic price of a glass lite. The price type is drawn from the previous field.
**Technical info:** numeric field, DB field: pokokon.zu1, pokokon.zuk1

**Shape surch.** Price surcharge that is charged for shapes. You can specify the value in percent or as amount with currency unit. The higher amount is always used as surcharge.
**Technical info:** numeric fields, DB fields: pokokonzu2, pokokon.zuk2

**SC** Percentage surcharge that is assessed on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is calculated.
**Technical info:** numeric field, DB field: pokokon.zu3, pokokon.zuk3

**Factor** Factor of the surcharge in percent.
**Technical info:** numeric field, DB field: pokokon.zu4, pokokon.zuk4

**Total surcharge** Price surcharge for the item in percent.
**Technical info:** numeric field, DB field: pokokon.zu26, pokokon.zuk26

**Round size** Dimension rounding in millimeters. **Technical info:** numeric field, DB field: pokokon.zu5, pokokonzuk5

**Minim. calculat.** Minimum surface in square meters.
**Technical info:** numeric field, DB field: pokokon.zu6, pokokon.zuk6

**Size of bundle** Capacity of the package in quantity units.
**Technical info:** numeric field, DB field: pokokon.zu8, pokokonzuk8

**Round price/pc.** Rounding down or rounding up for unit price of an item.
**Technical info:** numeric field, DB field: pokokonp.vkstkprsrund, pokokonp.ek-stkprsrund

**Surcharge type** The surcharge type specifies according to what the surcharge is scaled and how the surcharge is determined:
-   **Surface:** The surcharge applies starting with the specified surfaces.
-   **Longer edge:** The surface applies for the longer edge.
-   **Side ratio:** The surcharge applies starting with the specified side ratio.
-   **Oversize surcharge:** The surcharge applies starting with the specified size, e.g. edge length.
**Technical info:** toggle field, display field

**Surcharge** Surcharge that is charged on the price. It depends on the configuration whether the surcharge is charged on the glass basis, the basic quantity or unit price basis.
**Technical info:** numeric field, DB field: pokokon.zu24, pokokon.zuk24

**Discount/piece** Specification of the discount.
**Technical info:** numeric field, DB field: pokokon.zu25, plkokon.zuk25

**Min. price** Minimum price for the lite.
**Technical info:** numeric field, DB field: pokokon.zu20, pokokon.zuk20

#### Size surcharges

This area displays the values for price surcharges and the surcharge type. You can edit the values. The surcharge type specifies to what the surcharge refers:

-   **CU value:** The surcharge or discount is calculated as fixed amount on the article price. If the surcharge on the order is charged as a fixed amount, the currency of the PLCd determined for the header article applies. The currency is not converted.
-   **Percent:** The surcharge is calculated as a percentage of the base price of the header article. This surcharge type is only selected for exchange articles and processings.

**Small glass surcharge** Price surcharge for small glass if the area of the glass is smaller than the specified limit value. In the second field, you select the surcharge type.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu10, pokokon.zuk10

**Overlength surcharge** Price surcharge for overlengths if an edge length is longer than the specified limit value. In the second field, you select the surcharge type.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu11, pokokon.zuk11

**Oversize surcharge** Surcharge for oversizes if both glass edges exceed a specified length. In the second field, you select the surcharge type.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu12, pokokon.zuk12

#### Glazing

This area displays the values for glazing and sealing. You can edit the values.

**Enter minim. price** Minimum price that applies for glazing and/or sealing.
**Technical info:** numeric field, DB field: pokokon.zu21, pokokon.zuk21

**Glazing price** Price for glazing.
**Technical info:** numeric field, DB field: pokokon.zu22, pokokon.zuk22

**Sealing price** Price for sealing.
**Technical info:** numeric field, DB field: pokokon.zu23, pokokon.zuk23

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1339, D-1340, D-1341, D-1342*

---

### Conditions for PCD BASIC GLASS (LAMI/TG)

**Sales > Order Entry > Items tab > Price field of item article with price method PCD LAMI or PCD TG > `<Shift>` + `<F9>`**

*Fig. D-126 Conditions for PCD LAMI, TG*

This dialog displays the price conditions for an item article to which the price method PCD LAMI or PCD TG is assigned. You can edit the price conditions.

On the Conditions for PCD LAMI and Conditions for PCD TG dialogs, the Sales and Purchasing dialogs are largely the same. The Total Surcharge field is not displayed on the Purchasing tab.

If additional processing are included in the item's BOM, then the Processing Prices (SA), (PU) tabs are enabled:
⇨ "Item conditions - processing prices" on page D-1365

If muntins are included in the item's BOM, then the Muntin Prices tab is enabled:
⇨ "Item conditions - muntin prices" on page D-1368

If you have entered a LAMI article, use `<Shift>+<F10>` to display the conditions for the exchange and additional prices for the individual lites in the LAMI article on a separate dialog.
⇨ "Production cost calculation" on page D-1371

#### Header

The fields are described for the Conditions for PCD BASIC GLASS, PCD Processing dialog:
⇨ "Conditions for PCD, PCD BASIC GLASS processing" on page D-1339

#### Sales, purchasing tabs

Most fields are described for the Conditions for PCD BASIC GLASS, PCD Processing dialog:
⇨ "Conditions for PCD, PCD BASIC GLASS processing" on page D-1339

#### Size surcharges

Most fields are described for the Conditions for PCD BASIC GLASS, PCD Processing dialog:
⇨ "Conditions for PCD, PCD BASIC GLASS processing" on page D-1339

In addition, the following fields are displayed on the Sales tab:

**Aspect ratio** Surcharge for certain aspect ratios. In the second field, you select the surcharge type. The field is only displayed on the Conditions for PCD TGH dialog.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu28, plkokon.zuk28

#### Glazing

The fields are described for the Conditions for PCD BASIC GLASS, PCD Processing dialog:
⇨ "Conditions for PCD, PCD BASIC GLASS processing" on page D-1339

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1343, D-1344*

---

### Conditions IG

**Sales > Order Entry > Items tab > Price field of item article with price method IG > `<Shift>` + `<F9>`**

*Fig. D-127 Conditions IG*

This dialog displays the price conditions for an item article to which the price method IG is assigned. You can edit the price conditions.

The Sales and Purchasing tabs on the Conditions IG dialog are similarly structured.

If additional processing are included in the item's BOM, then the Processing Prices (SA), (PU) tabs are enabled:
⇨ "Item conditions – processing prices" on page D-1365

If muntins are included in the item's BOM, then the Muntin Prices tab is enabled:
⇨ "Item conditions - muntin prices" on page D-1368

#### Header

**PCD** Price code for the pre-defined price list.
**Technical info:** numeric field, DB field: pokokon.pkz, pokokon.ekpkz

**PLCD** The price list code is the unique numbering for regional, national and foreign price lists.
**Technical info:** numeric field

#### Sales, purchasing tabs

**Price type** Type of pricing.
-   **Matrix:** The price is calculated from the assigned price matrix. In the price matrix, the prices are scaled according to the height and width of the glass.
-   **Vector:** The price is calculated from the assigned vector. In a vector, prices can be scaled by size.
-   **Individual lites:** The price is calculated from the individual prices of the glass from which the lite is made.
-   **Prs/sqm:** The price is calculated per square meter. This price type is selected automatically if you edit the base price or an exchange price in the conditions.
**Technical info:** toggle field

**Matrix / vector** Number of the matrix or vector. The matrix is a two-dimensional price table with two reference values for the scaling, e.g. width and height. The vector is a one-dimensional price table with a reference value for the scaling, e.g. area. If you have selected a matrix or a vector, the name of the matrix or vector is displayed in plain text.
**Technical info:** numeric field, DB field: pokokon.matnr, pokokon.ekmatnr

**Basic price** Basic price of a glass lite. The basic price depends on the selected price type. In the second field, you select the price type. The price type determines to what the price refers:
-   **CU/piece:** The price applies per piece.
-   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu1, pokokon.zuk1

**Surcharge** Price surcharge that is charged on the basic price.
**Technical info:** numeric field, DB field: pokokon.zu20, pokokon.zuk20

**1. Exchange, 2. Exchange, 3. Exchange** Exchange sub-parts of the item. You can specify the following values in the fields:
-   **First field:** Number of the exchange list.
    **Technical info:** numeric fields, alphanumeric fields, DB fields: pokokon.at-mat1, pokokon.atmat2, pokokon.atmat3
-   **Second field:** Exchange code E (exchange) or A (addition).
    **Technical info:** numeric fields, alphanumeric fields, DB fields: pokokon.at-kz1, pokokon.atkz2, pokokon.atkz3
-   **Third field:** Price of the exchange article.
    **Technical info:** numeric fields, alphanumeric fields, DB fields: pokokon.atp1, pokokon.atp2, pokokon.atp3
-   **Fourth field:** Price surcharge of the exchange article in percent.
    **Technical info:** numeric fields, alphanumeric fields, DB fields: pokokon.zu11, pokokon.zu12, pokokon.zu13, pokokon.zu14, pokokon.zu15, pokokon.zu16

**Shape surch.** Price surcharge that is charged for shapes. You can specify the value in percent or as amount with currency unit. The higher amount is always used as surcharge.
**Technical info:** numeric fields, DB fields: pokokonzu2, pokokon.zuk2

**Surcharge** Percentage surcharge that is assessed on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is calculated.
**Technical info:** numeric field, DB field: pokokon.zu3, pokokon.zuk3

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: pokokon.zu4, pokokon.zuk4

**Round size** Specification of the dimension rounding in millimeters for price calculation of the article. The edge lengths in the order item will be rounded to the next higher value in millimeters that is divisible by the specified dimension rounding for the price calculation. This information is not considered in production. This field is only displayed on the Sales tab.
**Technical info:** numeric field, DB field: pokokon.zu5, pokokon.zuk5

**Minim. calculat.** Specification of the minimum area in square meters for which the price is calculated. If the area in the order item is smaller than the minimum calculation area, the price for this area will be calculated. This field is only displayed on the Sales tab.
**Technical info:** numeric field, DB field: pokokon.zu6, plkokon.zuk6

**Minimum edge length** Specification of the edge length in millimeters for the price calculation. This size is used if the height or width of the glass in the order item is smaller than this minimum edge length. The field is only displayed on the Conditions IG dialog.
**Technical info:** numeric field, DB field: pokokon.zu7, plkokon.zuk7

**AIR surch.** Price surcharge for the airspace. You specify the surcharge type in the second field. The surcharge type specifies to what the surcharge refers:
-   **CU/unit:** The surcharge is charged as fixed amount on the unit price of the item.
-   **CU/sqm:** The surcharge is charged per square meter of the airspace
-   **Percentage:** The surcharge is calculated per airspace as a percentage of the basic glass price.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu8, pokokon.zuk8

**Step surcharge** Price surcharge for glass with a step. You specify the surcharge type in the second field. The surcharge type specifies to what the surcharge refers:
-   **CU/pc ne:** The step surcharge is charged according to calculation of the factor as fixed net amount per step.
-   **CU/pc gr:** The step surcharge is charged as gross amount per step before calculation of the factor.
-   **Percent:** The step surcharge is charged as a percent of the glass quantity unit price and the exchange prices.
-   **%/piece:** The step surcharge is charged per step as a percent of the glass quantity unit price and the exchange prices.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu9, pokokon.zuk9

**Decor. glazing** Price surcharge for decorative glazing in percent if a Decorative glazing article type is attached in the BOM.
**Technical info:** numeric field, DB field: pokokon.zu28, plkokon.zuk28

**Excess length surch.** Price surcharge for excess lengths in percent if an Edge length is longer than the specified limit value.
**Technical info:** numeric field, DB field: pokokon.zu19, pokokon.zuk19

**Special surch.** Price surcharge for special orders. You specify the surcharge type in the second field. The surcharge type specifies to what the surcharge refers:
-   **CU/unit:** The surcharge is charged as fixed amount on the unit price of the item.
-   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
-   **Percentage:** The surcharge is calculated as a percentage of the basic glass price.
**Technical info:** numeric field, DB field: pokokon.zu25, plkokon.zuk25

**Total surcharge** Price surcharge for the item in percent.
**Technical info:** numeric field, DB field: pokokon.zu26, pokokon.zuk26

**Min. price** Minimum price for the item.
**Technical info:** numeric field, DB field: pokokon.zu18, pokokon.zuk18

**Round price/pc.** Rounding down or rounding up for unit price of an item.
**Technical info:** numeric field, DB field: pokokonp.vkstkprsrund, pokokonp.ek-stkprsrund

#### Size surcharges

Most fields are described for the Conditions for PCD BASIC GLASS, PCD Processing dialog:
⇨ "Conditions for PCD, PCD BASIC GLASS processing" on page D-1339

In addition, the following fields are displayed:

**Side ratio** Price surcharge for certain aspect ratios. You select the surcharge type in the second field.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu28

**Surface surcharge** Price surcharge for particular areas. You select the surcharge type in the second field. The field is only displayed on the Conditions IG dialog.
**Technical info:** numeric field, toggle field, DB fields: pokokon.zu9

#### Glazing

**Glazing price** Price for glazing.
**Technical info:** numeric field, DB field: pokokon.zu21, pokokon.zuk21

**Sealing price** Price for sealing.
**Technical info:** numeric field, DB field: pokokon.zu22, pokokon.zuk22

**Minimum price glazing** Minimum price for glazing.
**Technical info:** numeric field, DB field: pokokon.zu23, pokokon.zuk23

**Minimum price sealing** Minimum price for sealing.
**Technical info:** numeric field, DB field: pokokon.zu24, pokokon.zuk24

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1345, D-1346, D-1347, D-1348, D-1349*

---

### Conditions IG (SWITZERLAND)

**Sales > Order Entry > Items tab > Price field of item article with price method IG Switzerland > `<Shift>` + `<F9>`**

*Fig. D-128 Conditions IG (SWITZERLAND)*

This dialog displays the price conditions for an item article to which the price method IG Switzerland is assigned. You can edit the price conditions.

On the Conditions IG (SWITZERLAND) dialog there is a Sales tab, but no Purchasing tab.

If additional processing are included in the item's BOM, then the Processing Prices (SA), (PU) tabs are enabled:
⇨ "Item conditions - processing prices" on page D-1365

If muntins are included in the item's BOM, then the Muntin Prices tab is enabled:
⇨ "Item conditions – muntin prices" on page D-1368

#### Sales tab

**SA PCD** Price code for the pre-defined price list for sales.
**Technical info:** mandatory field, numeric field, DB field: pokokon.pkz

**Vector** Number of the vector from which the price should be drawn.
**Technical info:** mandatory field, numeric field, DB field: pokokon.matnr

**Basic glass price** Display of the minimum price for the basic glass price. The basic glass price is specified by the factor and can be edited document by document:
-   **Basic glass price:** Basic glass price in currency unit. **Technical info:** numeric field, DB field: pokokon.zu1
-   **(PType):** Specification of to what the basic glass price refers.
    -   **CU/piece:** The price applies per piece.
    -   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
    **Technical info:** toggle field, DB field: pokokon.flag2
-   **Minimum prices (in lines basic glass price):** Minimum price for the basic glass price. This price is specified if the calculated price in the order item is lower than the specified minimum price. **Technical info:** numeric field, DB field: pokokon.zu20

**Quantity scale discount 1** Discount on the basic glass price in percent. The discount applies starting with the quantity that is specified for the customer.
**Technical info:** numeric field, DB field: pokokon.zu2

**Basic gas price** Basic price for the gas filling of IG articles. You can enter the following values in the fields:
-   **Basic gas price:** Basic gas price per square meter.
    **Technical info:** numeric field, DB field: pokokon.zu3
-   **Minimum prices (in lines basic gas price):** Minimum price for the basic gas price. The price that is specified if the calculated price in the order item is lower than the specified minimum price.
    **Technische Info:** numeric field, DB field: pokokon.zu21

**1. Exchange, 2. Exchange, 3. Exchange** In the fields, you enter the prices for the exchange articles in the BOM. You can specify max. three exchange prices:
-   **1. Exchange, 2. Exchange, 3. Exchange:** Number of the exchange list.
    **Technical info:** numeric fields, DB fields: pokokon.atmat1, pokokon.atmat2, pokokon.atmat3
-   **PG:** Price group.
    **Technical info:** display fields, DB fields
-   **(article price):** Price of the exchange article per square meter.
    **Technical info:** numeric fields, alphanumeric fields, DB fields: pokokon.atp1, pokokon.atp2, pokokon.atp3.
-   **Minimum prices (in line 1. Exchange, 2. Exchange, 3. Exchange):** Minimum price for the exchange. The price that is specified if the calculated price in the order item is lower than the specified minimum price.
    **Technical info:** numeric fields, DB fields: pokokon.zu22, pokokon.zu23, pokokon.zu25

**Quantity scale discount 2** Discount on the exchange price in percent. The discount applies starting with the quantity that is specified for the customer.
**Technical info:** numeric field, DB field: pokokon.zu4

#### Surcharges

**Surcharge** Percentage surcharge that is assessed on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is calculated.
**Technical info:** numeric field, DB field: pokokon.zu5

**Pressure compensation** Surcharge for pressure compensation in percent. **Technical info:** numeric field, DB field: pokokon.zu6

**Series discount** Discount on the glass price in percent. The discount applies starting with the number of lites that is specified for the customer.
**Technical info:** numeric field, DB field: pokokon.zu7

**Product code factor** Factor that is considered for the product code with reaching of the limit quantity. If you specify a factor < 100%, it is used as discount and reduces the price.
**Technical info:** numeric field, DB field: pokokon.zu8

**Shape surch.** Price surcharge in percent that is charged for shapes.
**Technical info:** numeric field, DB field: pokokon.zu9

**Minimum shape surch.** Minimum price surcharge that is charged for shapes. If the calculated shape surcharge in the order is smaller than the defined minimum shape surcharge, this minimum surcharge is used.
**Technical info:** numeric field, DB field: pokokon.zu10

**Single shape surcharge** Price surcharge in percent for particular shapes.
**Technical info:** numeric field, DB field: pokokon.zu11

**Step surcharge** Price surcharge for step processing per piece.
**Technical info:** numeric field, DB field: pokokon.zu19

**Transport surcharge** Price surcharge for the transport in the currency unit.
**Technical info:** numeric field, DB field: pokokon.zu12

**Total surcharge** Price surcharge for the item in percent.
**Technical info:** numeric field, DB field: pokokon.zu13

**Glazing** Price surcharge for the glazing in currency unit per square meter.
**Technical info:** numeric field, DB field: pokokon.zu14

**Sealing** Price surcharge for the sealing in the currency unit per linear meter.
**Technical info:** numeric field, DB field: pokokon.zu15

**UV protection** Price surcharge for the UV protection per linear meter.
**Technical info:** numeric field, DB field: pokokon.zu24

#### (Area without description)

**Round size** Dimension rounding in millimeters.
**Technical info:** numeric field, DB field: pokokon.zu16

**Minim. calculation** Minimum number of quantity units for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is calculated.
**Technical info:** numeric field, DB field: pokokon.zu17

**Min. edge** Minimum edge length in millimeters.
**Technical info:** numeric field, DB field: pokokon.zu18

#### Processings

**Corner SC, Corner factor** Surcharge and factor for the price surcharge in percent for corner processings, e.g. corner cut-off.
**Technical info:** numeric fields, DB field: pokokon.zu26

**Edge SC, Edge factor** Surcharge and factor of the price surcharge in percent for edge processings, e.g. polishing. **Technical info:** numeric fields, DB field: pokokon.zu27, pokokon.zu28

**Area SC, Area factor** Surcharge and factor of the price surcharge in percent for surface processings, e.g. coating.
**Technical info:** numeric fields, DB field: pokokon.zu29, pokokon.zu30

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1350, D-1351, D-1352, D-1353*

---

### Conditions for PCD COLORED ARTICLE

**Sales > Order Entry > Items tab > Price field of item article with price method PCD colored article > `<Shift>` + `<F9>`**

*Fig. D-129 Conditions for PCD COLORED ARTICLE*

This dialog displays the price conditions for an item article to which the price method PCD Colored Article is assigned. You can edit the conditions.

The Sales and Purchasing tabs on the Conditions PCD COLORED ARTICLE dialog are similarly structured.

If additional processing are included in the item's BOM, then the Processing Prices (SA), (PU) tabs are enabled:
⇨ "Item conditions - processing prices" on page D-1365

#### Header

**SA PCD** Price code for the pre-defined price list for sales.
**Technical info:** mandatory field, numeric field, DB field: pokokon.pkz

**PU PCD** Price code for the pre-defined price list for purchasing.
**Technical info:** mandatory field, numeric field, DB field: pokokon.ekpkz

#### Conditions tab

Most fields are described for the Conditions for PCD BASIC GLASS, PCD Processing dialog:
⇨ "Conditions for PCD, PCD BASIC GLASS processing" on page D-1339

In addition, the following fields are displayed:

**Basic price** Basic price of the article. The price type determines to what the price refers:
-   **CU/piece:** The price applies per piece.
-   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
**Technical info:** numeric field, DB field: pokokon.flag2

**Minim. calculat.** Minimum number of quantity units for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is charged.
**Technical info:** numeric field, DB field: pokokon.zu6, pokokon.zuk6

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1354, D-1355*

---

### Conditions for PCD PRICES GENERAL

**Sales > Order Entry > Items tab > Price field of item article with price method PCD prices - general > `<Shift>` + `<F9>`**

*Fig. D-130 Conditions for PCD PRICES GENERAL*

This dialog displays the price conditions for an item article to which the price method PCD prices general is assigned. You can edit the price conditions.

The Sales and Purchasing tabs on the Conditions for PCD PRICES GENERAL dialog are similarly structured. The Total Surcharge field is not displayed in the Purchasing area.

If additional processing are included in the item's BOM, then the Processing Prices (SA), (PU) tabs are enabled:
⇨ "Item conditions - processing prices" on page D-1365

#### Header

**SA PCD** Price code for the pre-defined price list for sales.
**Technical info:** mandatory field, numeric field, DB field: pokokon.pkz

**PU PCD** Price code for the pre-defined price list for purchasing.
**Technical info:** mandatory field, numeric field, DB field: pokokon.ekpkz

**Vector** Number of the vector from which the price should be drawn.
**Technical info:** mandatory field, numeric field, DB field: pokokon.matnr

#### Conditions tab

Most fields are described for the Conditions for PCD BASIC GLASS, PCD Processing dialog:
⇨ "Conditions for PCD, PCD BASIC GLASS processing" on page D-1339

In addition, the following fields are displayed:

**Basic price** Basic price of the article. The price type determines to what the price refers:
-   **CU/piece:** The price applies per piece.
-   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
**Technical info:** toggle field, DB field: pokokon.flag2

**Minim. calculat.** Minimum number of quantity units for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is charged.
**Technical info:** numeric field, DB field: pokokon.zu6, pokokon.zuk6

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1356, D-1357*

---

### Conditions for PCD GLASS DOORS

**Sales > Order Entry > Items tab > Price field of item article with price method PCD glass doors > `<Shift>` + `<F9>`**

*Fig. D-131 Conditions for PCD GLASS DOORS*

This dialog displays the price conditions for an item article to which the price method PCD Glass Doors is assigned. You can edit the price conditions.

The Sales and Purchasing areas display mainly the same fields. In the Sales area, you specify the sales prices; in the Purchasing area the purchasing prices.

#### Header

**SA PCD** Price code for the pre-defined price list for sales.
**Technical info:** mandatory field, numeric field, DB field: pokokon.pkz

**PU PCD** Price code for the pre-defined price list for purchasing.
**Technical info:** mandatory field, numeric field, DB field: pokokon.ekpkz

**(Area without description)**
**Lite 1, 2, ... 7** Area of the lites in the glass door system. In the adjacent fields in the Sales and Purchasing areas, the square meter price for the lite in question is displayed.
**Technical info:** numeric fields, DB fields: pokokon.zu5, pokokon.zu7, pokokon.zu9, pokokon.zu11, pokokon.zu13, pokokon.zu15, pokokon.zu17

#### Sales and purchasing

**Scal. level** Price level from which the price is used. The field is only evaluated by the price calculation if the price type 2 - Scaling Level is specified for the relevant article price vector.
**Technical info:** numeric fields, DB fields: pokokon.flag1, pokokon.ekflag1

**SC** Surcharge in percent. The surcharge is charged on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is charged.
**Technical info:** numeric fields, DB fields: pokokon.zu3, pokokon.zuk3

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric fields, DB fields: pokokon.zu4, pokokon.zuk4

**Lite ... €/sqm** Price per square meter for the lite in question.
-   **Sales:** Price per square meter for the adjacent lite.
    **Technical info:** numeric fields, DB fields: pokokon.zu6, pokokon.zu8, pokokon.zu10, pokokon.zu12, pokokon.zu14, pokokon.zu16, pokokon.zu18
-   **Purchasing:** Purchase price per square meter for the adjacent lite.
    **Technical info:** numeric fields, DB fields: pokokon.zuk6, pokokon.zuk8, pokokon.zuk10, pokokon.zuk12, pokokon.zuk14, pokokon.zuk16, pokokon.zuk18

**Surcharge** Surcharge that is charged on the price. You specify the surcharge type in the second field. The surcharge type specifies to what the surcharge refers:
-   **CU/unit:** The surcharge is charged as fixed amount on the unit price of the item.
-   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
-   **Percentage:** The surcharge is calculated as a percentage of the basic glass price.
This field is only displayed in the Sales area.
**Technical info:** numeric field, toggle field, DB fields: plkokon.zu19

**SA edge processings/SC** Surcharge for edge processings on the sales price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
**Technical info:** numeric field, DB field: pokokon.zu20

**SA edge processings/factor** Factor for edge processings on the sales price in percent. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: pokokon.zuk20

**SA corner processings/SC** Surcharge for corner processings on the sales price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
**Technische Info:** numeric field, DB field: pokokon.zu21

**SA corner processings/Factor** Factor for corner processings on the sales price in percent. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: pokokon.zuk21

**SA surface processings/SC** Surcharge for surface processings on the sales price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
**Technical info:** numeric field, DB field: pokokon.zu22

**SA surface processings/factor** Factor for surface processings on the sales price in percent. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: pokokon.zuk22

**PU all processings/SC** Surcharge for all processings on the purchasing price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
**Technical info:** numeric field, DB field: pokokon.zu23

**PU all processings/factor** Factor for all processings on the purchasing price in percent. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: pokokon.zuk23

**Accessory/SC** Surcharge for accessory articles on the purchasing and/or sales price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
**Technical info:** numeric fields, DB fields: pokokon.zu24, pokokon.zuk24

**Accessory/Factor** Factor for accessory articles on the purchasing and/or sales price in percent. Generally a discount is granted with a factor.
**Technical info:** numeric fields, DB fields: pokokon.zu25, pokokon.zuk25

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1358, D-1359, D-1360*

---

### Conditions for manual prices

**Sales > Order Entry > Items tab > Price field of item article with price method Manual Prices > `<Shift>` + `<F9>`**

*Fig. D-132 Item conditions – conditions for manual prices*

This dialog displays the price conditions for an item article to which the price method Manual Prices is assigned in the master data. You can edit the price conditions.

> **Automatic price method change**
> You can also specify a price manually for item articles with a different price method. The price method for this item article is then changed automatically to manual prices.

-   **Price type** Specification of to what the price refers.
    -   **CU/piece:** The price applies per piece.
    -   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
    **Technical info:** toggle field, DB field: pokokon.flag2

You enter the following values for sales and purchasing prices separately.

**Price** Basic price of a glass lite. The price type is drawn from the previous field.
**Technical info:** numeric fields, DB fields: pokokonzu1, pokokon.zuk1

**SC** Surcharge in percent. The surcharge is charged on the quantity unit price.
**Technical info:** numeric fields, DB fields: pokokonzu2, pokokon.zuk2

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric fields, DB fields: pokokonzu3, pokokon.zuk3

**Round size** Specification of the dimension rounding in millimeters for price calculation of the article. The edge lengths in the order item will be rounded to the next higher value in millimeters that is divisible by the specified dimension rounding for the price calculation. This information is not considered in production.
**Technical info:** numeric fields, DB fields: pokokonzu5, pokokon.zuk5

**Minim. calculat.** If the value in the order item is smaller than the minimum calculation quantity, the price for this value is charged. For an article that is specified as area, the minimum area in square meters is specified as minimum calculation value. **Technical info:** numeric fields, DB fields: pokokon.zu5, pokokon.zuk5

---
*A+W Enterprise Sales*
*D-1361, D-1362*

---

### LAMI exchange/additional prices

**Sales > Order Entry > Items tab > Price field of LAMI article > `<Shift>` + `<F9>` > `<Shift>` + `<F10>`**

*Fig. D-133 LAMI exchange/additional prices*

This dialog displays the conditions for the exchange and additional prices for the individual lites in a LAMI article. You can edit the price conditions.

The values for sales, purchasing, and the detail view of the exchange and additional prices are each displayed in their own view.

-   Use `<F2>` to change between the views for sales, purchasing, and the detail view.

The dialog is only enabled if LAMI articles are included in the selected item.

#### Sales and purchasing

-   **Article:** Article number.
    **Technical info:** display field, numeric field, DB field: pokoaust.artnr
-   **Exchange/Additional list, Description:** Number of the exchange list. If a number is specified, the description is displayed in plain text.
    **Technical info:** numeric field, display field, DB fields: pokoaust.vkatlnr, pokoaust.ekatinr, xatl.bez
-   **Min.calc.:** Minimum calculation. Specification of the minimum area in square meters for which the price is calculated. If the area of the exchange glass in the order item is smaller than the minimum calculation area, the price for this minimum calculation area is used.
    **Technical info:** numeric field, display field, DB fields: pokoaust.vkminber, pokoaust.ekminber
-   **Factor:** Factor of the surcharge in percent.
    **Technical info:** numeric field, display field, DB fields: pokoaust.vkfaktor, pokoaust.ekfaktor
-   **SA price, PU price:** Sales or purchasing price of the exchange glass.
    **Technical info:** numeric field, DB field: pokoaust.vkmepreis, pokoaust.ekmepreis
-   **Type:** Specification of to what the price refers.
    -   **CU/m2:** The price applies per square meter.
    -   **Percentage:** The surcharge is calculated as a percentage of the basic glass price.
    **Technical info:** toggle field, DB field: pokoaust.vkpreistyp, pokoaust.ekpre-istyp

#### Detailed view

The fields in the detail view correspond to columns in sales and purchasing. In addition, the fields for the size surcharges for sales and purchasing are displayed. The surcharge type specifies to what the surcharge refers:

-   **CU value:** The surcharge or discount is calculated as fixed amount on the sales/purchasing price.
-   **Percent:** The surcharge is calculated as a percentage of the sales/purchasing price.

**Small glass surcharge** Price surcharge for small glass if the area of the glass is smaller than the specified limit value. You select the surcharge type in the second field.
**Technical info:** numeric field, toggle field, DB fields: pokoaust.vkklzuschlag, pokoaust.vkklzutyp, pokoaust.ekklzuschlag, pokoaust.ekklzutyp

**Overlength surcharge** Price surcharge for overlengths if an edge length is longer than the specified limit value. You select the surcharge type in the second field. **Technical info:** numeric field, toggle field, DB fields: pokoaust.vkueb-zuschlag, pokoaust.vkuebzutyp, pokoaust.ekuebzuschlag, pokoaust.ekuebzutyp

**Oversize surcharge** Surcharge for oversizes if both glass edges exceed a specified length. In the second field, you select the surcharge type.
**Technical info:** numeric field, toggle field, DB fields: pokoaust.vkuebzuschlag, pokoaust.vkuebgrzutyp, pokoaust.ekuebgrzuschlag, pokoaust.ekuebgrzutyp

---
*A+W Enterprise Sales*
*D-1363, D-1364*

---

### Item conditions – processing prices

**Sales > Order Entry > Items tab > Select price field of item article including additional processing steps > `<Shift>` + `<F9>`**

*Fig. D-134 Item conditions – processing Prices (SA), (PU), detail view*

These tabs display the price conditions for a price-relevant processing depending on whether it is included in the item BOM. You can edit the price conditions.

The processing prices are divided into Sales and Purchasing. Furthermore, there is a detail view that is the same for both tabs. The detail view displays more values of the processing prices for the individual processing.

-   Switch to the Detail view using `<F5>`.

The tabs are only enabled if additional processings are entered in the selected item. The **Processing Prices (Sls)** tab is only enabled if the supply type PO or Included is selected for the item.

#### Processing prices (SA) tab

-   **Article:** Description of the processing.
    **Technical info:** display field, DB field: aufstrukt.artnr
-   **Wd., Hgh:** Number of processed widths and heights of the lite.
    **Technical info:** numeric fields, DB fields: poszu.panz1, poszu.panz2
-   **Price type:** Specification of to what the price refers.
    -   **CU/piece:** The price applies per piece.
    -   **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
    -   **Percent:** The price is calculated as a percentage from the base price of the head article.
    -   **CU/m2:** The price applies per square meter.
    -   **CU/linm:** The price applies per linear meter.
    **Technical info:** toggle field, DB field: poszu.part
-   **Qty:** Quantity of the processing per basic quantity unit.
    **Technical info:** numeric field, DB field: poszu.pme
-   **Factor:** Sales price factor of the processing price surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
    **Technical info:** numeric field, DB field: poszu.vkfaktor
-   **SC:** Sales price surcharge for the processing in percent. The surcharge is charged on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is charged.
    **Technical info:** numeric field, DB field: poszu.vktz
-   **ShpSrch:** Shape surcharge in percent.
    **Technical info:** numeric field, DB field: poszu.vkmodzusch
-   **SalesPrc:** Sales price of the processing.
    **Technical info:** numeric field, DB field: poszu.ppme
-   **Grp:** Number of the grouping. The processings can be grouped under a number.
    **Technical info:** numeric field, DB field: poszu.masflag

#### Processing prices (PU) tab

Most of the columns are described for the Purchasing Prices (Sls) tab.
⇨ "Processing prices (SA) tab" on page D-1366

In addition, the following columns are displayed:

-   **PU Factor:** Purchasing price factor of the processing price surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
    **Technical info:** numeric field, DB field: poszu.ekfaktor
-   **PuSC:** Purchase price surcharge for the processing in percent. The surcharge is charged on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is charged.
    **Technical info:** numeric field, DB field: poszu.ektz
-   **PuShSur:** Purchase price shape surcharge in percent.
    **Technical info:** numeric field, DB field: poszu.ekmodzusch
-   **PU price:** Purchasing price of the processing.
    **Technical info:** numeric field, DB field: poszu.ppmeek

#### Processing prices detail view

Most of the fields in the detail view are described for the Purchasing Prices (Sls) tab.
⇨ "Processing prices (SA) tab" on page D-1366

In addition, the following fields are displayed:

**Round size** Dimension rounding per processing in quantity unit.
**Technical info:** display field, DB field: poszu.massrund

**Minim. calculat.** Specification of the minimum calculated quantity unit of the processing.
**Technical info:** display field, DB field: poszu.minber, poszu.minberek

**Basic price** Basic price of a price-relevant processing for sales and purchasing. The basic price for sales corresponds to the value in the SA Price field on the Processing Prices (Sls) tab, the basic price for purchasing to the value in the PU Price field on the Processing Prices (Purch) tab.
**Technical info:** numeric fields, DB fields: poszu.ppme, poszu.ppmeek

**Min. price** Minimum price for the processing.
**Technical info:** numeric field, DB field: poszu.minpreis

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1365, D-1366, D-1367*

---

### Item conditions – muntin prices

**Sales > Order Entry > Items tab > Price field of item article including muntins > `<Shift>` + `<F9>`**

*Fig. D-135 Item conditions – muntin prices*

This tab displays the price conditions for muntin prices of an item article. You can edit the price conditions.

The tab is only enabled if muntins are entered in the selected item. The values for sales and purchasing prices are displayed in two individual areas.

#### Sales and purchasing

**Muntin PCD** Muntin price code from the pre-defined price list for muntin calculation.
**Technical info:** numeric field, DB field: pokospro.vkpkz, pokospro.ekpkz

**Muntins calcul. type** Calculation type of the muntins. The muntin calculation types are described in detail elsewhere:
⇨ "Order muntin prices" on page D-1327
**Technical info:** numeric field, DB field: pokospro.vkberart, pokospro.ekberart

**Muntins factor** Factor for the muntin surcharge in percent. Using the factor, you can change the price calculation for the item without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: pokospro.vkfaktor, pokospro.ekfaktor

**Muntins SC** Muntin surcharge in percent. The surcharge is charged on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is charged.
**Technical info:** numeric field, DB field: pokospro.vktz, pokospro.ektz

**Price per field** Muntin price by number of fields if there are crossing points in the muntin pattern. If, for example, two vertical and two horizontal muntins divide the window into nine fields, the price is calculated nine times. The price is evaluated for the calculation types Fields, Field+LM, Field+E+C and Special.
**Technical info:** numeric field, DB field: pokospro.vkfeld, pokospro.ekfeld

**Price per field 2** Muntin price by number of fields if there are no crossing points in the muntin pattern. If, for example, four vertical and no horizontal muntins divide the window into five fields, the price is calculated five times. The price is evaluated for the calculation types Fields, Field+LM, Field+E+C and Special.
**Technical info:** numeric field, DB field: pokospro.vk2feld, pokospro.ek2feld

**Price per Inch** Price per inch for the muntin. The price is evaluated for the calculation types LM, LM+C+E, LM+C, LM+E, field+LM, and Special.
**Technical info:** numeric field, DB field: pokospro.vklaufm, pokospro.eklaufm

**Price per edge** Price per edge connection. The price is evaluated for the calculation types E, LM+C+E, LM+E, C+E, field+C+E, and Special.
**Technical info:** numeric field, DB field: pokospro.vkrand, pokospro.ekrand

**Price per cross** Price per crossing point. The price is evaluated for the calculation types C, C+E, LM+C, LM+C+E, C or LM, field+C+R, and Special.
**Technical info:** numeric field, DB field: pokospro.vkkreuz, pokospro.ekkreuz

**Percent** Price as percentage on the price of the head article. The price is evaluated for the calculation type Percent.
**Technical info:** numeric field, DB field: pokospro.vkprozent, pokospro.ekproz-ent

**Price/Sqft** Price per square foot. The price is evaluated with the calculation type sqm price.
**Technical info:** numeric field, DB field: pokospro.vkqmpreis, pokospro.ekqm-preis

**Price/Pc.** Price per muntin pattern. The price is evaluated for the calculation type Piece.
**Technical info:** numeric field, DB field: pokospro.vkstueckprs, pokospro.ek-stueckprs

**Min. lin. meter** Minimum length of the muntins in meters, which will be calculated for the price. If the muntin measures fewer linear meters than the minimum linear meters, then the price for the minimum linear meters will be calculated. The price is evaluated with the calculation type LM.
**Technical info:** numeric field, DB field: pokospro.vkminlm, pokospro.ekminlm

**Min. no. of fields** Minimum number of muntin fields for which the price will be calculated. The price is evaluated with the calculation type Fields.
**Technical info:** numeric field, DB field: pokospro.vkminfeld, pokospro.ekmin-feld

**Muntins factor 2** Factor for the muntin surcharge in percent for the second muntin. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
**Technical info:** numeric field, DB field: pokospro.vkfaktor2, pokospro.ekfaktor2

**Price per field (2nd muntin)** Muntin price by number of fields for the second muntin if there are crossing points in the muntin pattern. The price is evaluated for the calculation types Fields, Field+LM, Field+E+C and Special.
**Technical info:** numeric field, DB field: pokospro.vkfeld2, pokospro.ekfeld2

**Price per field 2 (2nd muntin)** Muntin price by number of fields for the second muntin if there are no crossing points in the muntin pattern. The price is evaluated for the calculation types Fields, Field+LM, Field+E+C and Special.
**Technical info:** numeric field, DB field: pokospro.vk2feld2, pokospro.ek2feld2

**Price per Inch (2nd muntin)** Price per inch for the second muntin. The price is evaluated for the calculation types LM, LM+C+E, LM+C, LM+E, field+LM, and Special.
**Technical info:** numeric field, DB field: pokospro.vklaufm2, pokospro.eklaufm2

**Price per edge (2nd muntin)** Price per edge connection for the second muntin. The price is evaluated for the calculation types E, LM+C+E, LM+E, C+E, field+C+E, and Special.
**Technical info:** numeric field, DB field: pokospro.vkrand2, pokospro.ekrand2

**Min. lin. meter (2nd muntin)** Minimum length of the second muntin in meters, which will be calculated for the price. If the muntin measures fewer linear meters than the minimum linear meters, then the price for the minimum linear meters will be calculated. The price is evaluated with the calculation type LM.
**Technical info:** numeric field, DB field: pokospro.vkminlm2, pokospro.ekmin-lm2

#### Footer

This area displays the description of the article and the code for the article's product group.

---
*A+W Enterprise Sales*
*D-1368, D-1369, D-1370*

---

## Production cost calculation

**Sales > Order Entry > Items tab > Price field > `<Ctrl>` + `<F10>`**

This dialog displays the results of the cost calculation. You can edit some of the values.

In the document entry, first only the material costs are displayed. The machine and personnel costs are only displayed if the document has been scheduled in a production system.

This dialog offers the following tabs:

-   "Production cost calculation – overview” on page D-1372
-   "Production cost calculation – details" on page D-1374

### Production cost calculation – overview

**Sales > Order Entry > Items tab > Price field > `<Ctrl>` + `<F10>` > Overview**

*Fig. D-136 Production cost calculation – overview*

This tab displays the production costs for the selected item. You can edit the calculated quantity and unit price of the items.

If for a processing article machines or personnel costs are calculated, then the corresponding article number and description for the item article are displayed via the table in the tab heading.

Use `<F2>` to change to the detail view where you can edit additional data.

> **Calculation only after transfer to production**
> Depending on the system configuration, the production costs are only displayed if you have already transferred an order to production. If you have not yet transferred the order to production, only the material costs are displayed.

#### Overview Fields

-   **Cost type:** Display of the type of the production costs.
    -   Material costs
    -   Internal contribution margin
    -   Assembly costs
    -   Machinery costs
    -   Personnel costs
    -   Fixed Costs
    -   Purchased
    **Technical info:** display field, DB field: poskost.satztyp
-   **Article:** Display of the article number.
    **Technical info:** display field, DB field: poskost.artnr
-   **Cost center:** Cost center name for statistical evaluations.
    **Technical info:** alphanumeric field, DB field: poskost.kostenst
-   **Phys. Qty:** Display of the physical item quantity (actual quantity), e.g. glass area.
    **Technical info:** display field, DB field: poskost.phymenge
-   **Calcul. Qty:** Display of the calculated item quantity, e.g. glass area + waste.
    **Technical info:** display field, DB field: poskost.pme
-   **Price/QU:** Display of the price per quantity unit of the item.
    **Technical info:** display field, DB field: poskost.ppme
-   **Price/pc.:** Price per piece of the item.
    **Technical info:** numerical field, DB field: poskost.stprs

#### Footer

Sums from the corresponding rate types. The following abbreviations are shown:

-   **Mat.:** Material costs.
-   **IntDB:** Internal contribution margin.
-   **Assy.:** Assembly costs.
-   **Mach.:** Machine costs.
-   **Pers.:** Personnel costs.

### Production cost calculation – details

**Sales > Order Entry > Items tab > Price field > `<Ctrl>` + `<F10>` > Details tab**

*Fig. D-137 Production cost calculation – details*

This tab displays the detail data for the production costs determined. You can edit the selected item and thus recalculate the production costs.

Use `<Page Up>` and `<Page Down>` to navigate between the individual costs of the current item.

If for a processing article machines or personnel costs are calculated, then the corresponding article number and description for the item article are displayed via the table in the tab heading.

#### Details

Depending on the cost type, different fields are displayed:

**Production item** Production item number for production costs. For ordered processings, the corresponding item number for the order is displayed in which the subparts are ordered.
**Technical info:** display field, DB field: poskost.plfdpos

**Cost type** Display of the type of the production costs.
**Technical info:** display field, DB field: poskost.satztyp

**Manual modification** Specification whether the values were overwritten. If the production costs are changed, Manual will be displayed in the field. You cannot edit the content in the field.
**Technical info:** display field, DB field: poskost.manuell

**Supply type** Display of the supply type of the selected article. The value can only be edited for the record types Machine Costs and Personnel Costs.
-   **None:** No supply type, e.g. for services.
-   **P.O.:** Article has to be ordered from the supplier.
-   **Stock:** Article will be taken from stock.
-   **Production:** Article will be produced.
-   **Acc.:** Article is delivered by the customer, e.g. for further processing.
-   **not avail:** The article is not available.
**Technical info:** toggle field, DB field: poskost.beschaffart

**Quantity** Article quantity in the BOM of the item. For the production costs, the quantity is always 1. For machine costs, generally no quantity is displayed.
**Technical info:** display field, DB field: poskost.menge

**Article** Number of the article for which the costs are determined.
**Technical info:** display field, DB field: postkost.artnr

**Header prod.** Article to which the selected article is attached as subpart. If the article is itself the header article, the field remains empty.
**Technical info:** display field, DB field: poskost.refartnr

**Production sub no.** Personnel number. You cannot edit the value. This field is only displayed for the record type Machine Costs.
**Technical info:** numeric field, DB field: poskost.psbmnr

**Machine no.** Number of the machine that is used for the calculation. With connection to A+W Production, the machine ID and name are shown here. This field is only displayed for record types Machine costs and Personnel costs.
**Technical info:** numeric field, DB field: poskost.bmnr

**Logical machine** Logical machine number. With connection to A+W Production, the ID of the logical machine and its name are displayed here. This field is only displayed for record types Machine costs.
**Technical info:** numeric field, DB field: poskost.psbmnr

**Process class** Number of the process class for the production planning. Several work processes can be summarized in a process class. This field is only displayed for the record types Machine Costs and Personnel Costs.
**Technical info:** numeric field, DB field: poskost.agknr

**Work process** Number of the work process for the production planning. This field is only displayed for the record types Machine Costs and Personnel Costs.
**Technical info:** numeric field, DB field: poskost.agnr

**Staff ID** Personnel class number. You cannot edit the value. This field is only displayed for record types Personnel Costs.
**Technical info:** numeric field, DB field: poskost.pknr

**Cost center** Cost center name for statistical evaluations.
**Technical info:** alphanumeric field, DB field: poskost.kostenst

**Basic unit of qty** Basic quantity unit that was assigned to the article in the master data, e.g. square meter, piece. The value is used for calculation of the piece price for the record types Machine Costs and Personnel Costs. You cannot edit the value. This field is only displayed for the record types Machine Costs and Personnel Costs.
**Technical info:** numeric field, DB field: poskost.lugme

**Variant** Display of the variant number of the article.
**Technical info:** numeric field, DB field: poskost.variante

**Qty (physical)** Physical quantity of the item (actual quantity), e.g. glass area, duration of work. The physical quantity is used as calculation basis for the calculational quantity and unit price. The field corresponds to the Phy. Qty column on the Overview tab.
**Technical info:** numeric field, DB field: poskost.phymenge

**Loss** Percentage loss of the item, e.g. material loss, time loss. The percentage of the loss is calculated on the calculated quantity. If you specify a negative loss, the calculated loss gets smaller.
**Technical info:** numeric field, DB field: poskost.verlust

**Quantity (calculation)** Calculated quantity of the item, e.g. glass area + waste. The calculated quantity is calculated from the physical quantity including loss.
Physical quantity + loss/100xphysical quantity The field corresponds to the Calc. Qty column on the Overview tab.
**Technical info:** numeric field, DB field: poskost.pme

**Price/QU** Price per basic quantity unit of the item. The quantity unit price is used for calculation of the unit price. The field corresponds to the Qty Price column on the Overview tab.
**Technical info:** numeric field, DB field: poskost.ppme

**Price/pc.** Price per unit of item. The unit price is calculated from the quantity unit price and the calculated quantities: Quantity unit price x calculated quantity
For the record types Machine Costs and Personnel Costs, the basic quantity unit is also used for calculation of the unit price.
Quantity unit price x calculated quantity / basic quantity unit
**Technical info:** numeric field, DB field: poskost.stkprs

**Date** Entry date of the item.
**Technical info:** date field, DB field: poskost.datum

**Price per quantity unit / complet. report** Price per quantity unit with completion report.
**Technical info:** numeric field, DB field: poskost.fppme

**Price/pc. / completion report** Item price with completion report in own currency.
**Technical info:** numeric field, DB field: poskost.fstprs

**(Price/pc.) in foreign currency** Price/Pc. in foreign currency.
**Technical info:** numeric field, DB field: poskost.stkprsfw

**(Price/pc./complet. report in foreign currency)** Price/Pc. with completion report in foreign currency.
**Technical info:** numeric field, DB field: poskost.fstprsfw

#### Footer

The footer is described for the Overview tab:
⇨ "Footer" on page D-1373

---
*A+W Enterprise Sales*
*D-1371, D-1372, D-1373, D-1374, D-1375, D-1376, D-1377*

---

## Price calculation

**Sales > Pricing**

*Fig. D-138 Price calculation*

Use this dialog to calculate the sales prices based on the defined conditions. The calculated price is only for your information and will not be saved.

The control elements are described for the Order Entry dialog:
⇨ "Order entry" on page D-1133

---
*A+W Enterprise Sales*
*D-1378*

---

## Release

Depending on the system configuration, orders are not released during entry, e.g. if the operator does not have sufficient rights, the contribution margin is underrun or the company limit is exceeded. These orders have to be released manually for further processing in order to transfer them later to the system; that is, to production, purchasing, dispatch, and the warehouse.

The following dialogs are described in this section:

-   "Order release" on page D-1379
-   "Authorization" on page D-1382

### Order release

**Sales > Order Release > Release**

*Fig. D-139 Order release*

On these dialogs, you search for and release an order for further processing. You can only release an order if you have the appropriate rights. Depending on the reason for the order block, different rights are required for the order release.

On the **Order Release** search dialog, you can filter the search for release:

-   **Enter search criteria > [Start]:**
    You can select department or operator and/or reason in the specified company. All orders are displayed that fulfill the criteria. If you don't enter any criteria, all orders not yet released are displayed in the hit list.
-   **[Individual] > Enter reason > Specify company, operator > [OK]:**
    First you have to enter a reason and then you can select the company and/or the operator on the Release dialog.

On the order release dialog, all orders are displayed that fulfill the search criteria.

-   Use `<Shift>+<F5>` to open the marked order in the order entry.
-   Use `<Ctrl>+<F9>` to release all orders.
-   Use `<Shift>+<F9>` to release all orders starting with the marked order.
-   Use `<Shift>+<F12>` to open the **Blockage reasons for unsuccessful release** dialog. This dialog displays the reasons for the block of the order. The dialog is only displayed if an order is blocked for more than one reason.
-   Use `<F3>` to release the selected orders.

#### Header

This area displays the search criteria that you have specified. You cannot edit the search criteria after the fact. For a new search, you have to close the dialog and open it again.

#### Overview

This area displays the orders that fulfill the search criteria and can be released. You can only edit the values in the **Free** and **LL** columns. The other columns are only for your information.

-   **Order:** Number of the order that is not yet released.
    **Technical info:** display field, DB field: kauf.auftrnr
-   **Free:** Information about releasing the order. If the field is grayed out, then the release is not possible for data-technical reasons or you do not have the appropriate rights for the release.
    -   **NO:** order will not yet be released.
    -   **YES:** order will now be released.
    -   **NEVER:** order will never be released.
    -   **SC:** transfer order to shipping control only.
    **Technical info:** toggle field, DB field: kauf.tekap.kz
-   **Customer, Name:** Number and name of the customer in this order.
    **Technical info:** display fields, DB fields: kauf.kunr, mp.name
-   **Req. On:** Planned delivery date.
    **Technical info:** display field, DB field: kauf.ltideal
-   **Call:**
    -   **Y:** The order will only be shipped on the customer's request.
    -   **N:** The order will be delivered by default.
    **Technical info:** display field, DB field: kauf.abrufkz
-   **User, DptNo:** Number and department number of the order operator.
    **Technical info:** display fields, DB fields: kauf.eusr, kauf.abtnr
-   **Entered:** Date on which the order was entered.
    **Technical info:** display field, DB field: kauf.edat
-   **Site:** Site number that is assigned to the order.
    **Technical info:** display field, DB field: kauf.hausnr
-   **LL:** Limit lock. Specification whether the order is locked. You can only release orders if you have the appropriate rights. You require special rights if you want to release orders that have exceeded the company limit or the general credit insurance limit.
    -   **Y:** The limit lock is active. The Free field is locked and the value set automatically to NO.
    -   **N:** The limit lock is disabled. The order can be released.
    **Technical info:** toggle field, DB field: kauf.limsperre
-   **Remark:** Additional information on the order.
    **Technical info:** display field, DB field: kauf.luspermodus
-   **Info:** Indication whether order information is stored. If an I appears in the column, information is stored for the order. Use `<F5>` to open the Remark dialog with the stored information.
    **Technical info:** display field

> **Status display**
> On the Order entry dialog in the order that was not released directly by local settings or not suitable data, the status display (top right) is output that the order was not released.

---
*A+W Enterprise Sales*
*D-1379, D-1380, D-1381*

---

### Authorization

**Sales > Order Release > Authorization**

*Fig. D-140 Authorization*

On this dialog, you can authorize an employee to release an order, even if this order exceeds the credit limit. You specify the maximum amount of the overage by specifying the new value accordingly or entering a value in the Maximum Increase in Value field.

The functions depend on the settings in the master data and the respective system configuration. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

**Document** Number and type of the document. If you have specified a number, the document type is displayed in plain text.
**Technical info:** mandatory field, numeric field, DB field: kauffrei.auftrnr

**Serial amendment no.** Number of the amendment process. The current amendment number is entered automatically. You can specify a smaller amendment number to view the corresponding amendment state.
**Technical info:** numeric field, DB field: kauffrei.aendernr

> **Increase the amendment number**
> You can only edit the last amendment state without increasing the amendment number. If you call up an amendment state that is farther back and edit it, the amendments are stored under a new amendment number.

**Customer** Customer name from the document. If you have specified the document number, the customer is displayed in plain text.
**Technical info:** display field, DB field: kauf.kunr

**Authorized employee** Number and name of the employee for whom the authorization is created. If you have specified a number, the name of the employee is displayed in plain text.
**Technical info:** numeric field, DB field: kauffrei.aendmanr

**Old value** Old net total value of the document. As value, the current net total value of the document is used.
**Technical info:** numeric field

**New value** Upper limit for the new net total value of the document. The value has to be higher than the old net total value. The value depends on the Maximum Increase in Value field:
-   If the Maximum Increase in Value field is empty and you specify a new net total value, the difference between the old and new net total value is displayed automatically in the Maximum Increase in Value field.
-   If there is already a value in the Maximum Increase in Value field and you specify a new net total value, the value in the Maximum Increase in Value field is adjusted automatically to the new value.
**Technical info:** numeric field

**Maximum increase in value** Maximum increase of costs that exceed the old net total value of the order. The value depends on the New Value field:
-   If the New Value field is empty and you specify a new maximum value, the difference between the old and new net total value is displayed automatically in the New Value field.
-   If there is already a value in the New Value field and you specify a new maximum value, the value in the New Value field is adjusted automatically to the new value.
**Technical info:** numeric field, DB field: kauffrei.maxpreisdiff

#### Footer

**Employee** Display of the name of the authorizing employee.
**Technical info:** display field, DB field: kauffrei.automanr

**Date** Display of the date on which the authorization was released. By default, the current date is displayed.
**Technical info:** display field

---
*A+W Enterprise Sales*
*D-1382, D-1383*

---

## Delivery

By default, delivery notes are entered and managed in the Shipping Control module because the bookings of packed and finished products from other modules and programs are forwarded automatically to the dispatch control. If the Shipping Control module is not configured, you can create delivery notes in the Sales module.

Depending on the configuration, you can create a delivery plan for an order. In the delivery plan, you can break up the order into partial deliveries. A delivery note is created for each (partial) delivery of an order. The delivery note serves as proof of the order processing for logistics and transportation and for the customer's information. Depending on the type of deliveries, the system distinguishes between complete and partial delivery notes. You can create and edit delivery notes automatically or manually.

The functions depend on the settings in the master data and the respective system configuration.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

The following dialogs are described in this section:

-   "Delivery plan" on page D-1385
-   "Delivery information – delivery details" on page D-1387
-   "Delivery notes (automatic)" on page D-1391
-   "Delivery notes (manual)" on page D-1393
-   "Delivery notes log" on page D-1395

---
*A+W Enterprise Sales*
*D-1384*

---

### Delivery plan

**Sales > Order Entry > Item level > `<F4>` > Delivery Plan**

*Fig. D-141 Delivery plan*

On this dialog, you enter the delivery plan. You can specify several partial deliveries for an order. If you create a delivery note, the data is drawn from the delivery plan and evaluated. You can only create a delivery note for an order when the entry of the items is complete.

#### Overview

-   **Itm:** Number of the item from the order.
    **Technical info:** display field, DB field: lieferplan.posnr
-   **Shipm.:** Number of the (partial) delivery.
    **Technical info:** mandatory field, numeric field, DB field: liefplan.subnr
-   **Deliv.date:** Estimated date for the (partial) delivery.
    **Technical info:** date field, DB field: liefplan.ltplan
-   **ArrivalDay:** Estimated arrival date for the (partial) delivery.
    **Technical info:** display field, DB field: liefplan.ankunft
-   **Article:** Name/description of the article.
    **Technical info:** display field, DB field: liefplan.artbez1
-   **Route:** Number of the route for the (partial) delivery.
    **Technical info:** mandatory field, numeric field, DB field: liefplan.route
-   **Total:** Total number of pieces of the ordered item from the order.
    **Technical info:** numeric field, DB field: liefplan.geslief
-   **Deliv.:** Already delivered item of the order.
    **Technical info:** numeric field, DB field: liefplan.geliefert
-   **Packed:** Quantity of packed items for the order.
    **Technical info:** numeric field, DB field: liefplan.gespack
-   **Scheduled:** Scheduled number of pieces of the item that will be delivered in this (partial) delivery.
    **Technical info:** mandatory field, numeric field, DB field: liefplan.zuliefern

#### Details

The Details tab is currently not used.

---
*A+W Enterprise Sales*
*D-1385, D-1386*

---

### Delivery information – delivery details

**Sales > Order Entry > Item level > `<F4>` > Shipping Information**

*Fig. D-142 Delivery details*

On this dialog, the details of the delivery are displayed, e.g. the route and planned delivery date. The differing delivery information is especially important if there is a distinction between production and delivery site.

Some fields in the Producing and Shipping Site areas can only be pre-populated if you are working with internal site separation and the via site logic is active.

The fields on this dialog are pre-populated by the system. Generally you do not have to edit the fields.

#### Producing site

**Delivery addr. code** Code and name of the saved delivery address of the producing site.
**Technical info:** alphanumeric fields, DB fields: kauf.lort, kauf.lort

**Disp. type** Number and description of the dispatch type. If a number is specified, the description of the dispatch type is displayed in plain text.
**Technical info:** numeric field, display field, DB field: kauf.versandartvia

**Sched. delivery date** Date of the planned delivery to the producing site. The date specifies the day on which the delivery will probably leave the producing site.
**Technical info:** date field, DB field: kauf.ltplan

**Route** Number of the route for delivery.
**Technical info:** mandatory field, numeric field, DB field: kauf.routenr

**Travel time** Probable duration to the delivery site. If a route is specified for which a travel time is stored, the travel time is displayed in plain text. It can affect the delivery date.
**Technical info:** display field

**Route days** Display of the days of the week on which the route is driven. If a route is specified, the associated days of the week are drawn from the master data and displayed in plain text.
**Technical info:** display field

**Area** Display of the dispatch region. Several delivery routes can be combined into a dispatch region if the system is configured appropriately. The dispatch region is drawn from the master data for the appropriate via route. The field is pre-populated if the regional routes module is configured and a dispatch region is assigned to the current route. In addition, you have to work with internal site separation and the via site logic must be active.
**Technical info:** display field, DB field: route.region

**Via site** Number of the delivering site via which the delivery will be sent. You specify the via site in the header in the Route field with `<F5>`.
**Technical info:** display field, DB field: kauf.vsvia

**Site** Display of the site number (company number) in which the order is created.
**Technical info:** display field, DB field: kauf.hausnr

**Tonnage** Display of the load capacity of the vehicle in kilograms. This field can be configured at will.
**Technical info:** display field

**Calendar** Indication whether the calendar will be used for the delivery date determination. You can specify in the route master data for each route whether the calendar will be evaluated.
☑ The calendar will be used for the delivery date determination.
☐ The calendar will not be used for the delivery date determination.
**Technical info:** checkbox

#### Delivery site

This area is only displayed if you are working with internal site separation and the via site logic is active.

**Delivery addr. code, delivery addr. name** Code and name of the delivery address of the delivery site.
**Technical info:** alphanumeric fields, DB fields: kauf.lort, kauf.lort

**Disp. type** Number of the dispatch type, e.g. truck. If a number is selected, the description of the dispatch type is displayed in plain text.
**Technical info:** display field, DB field: kauf.versandartvia

**Arrival at via site** Date on which the delivery will probably reach the via site. **Technical info:** display field

**Handling time** Handling time for loading or unloading in the delivery site.
**Technical info:** numeric field

**Route** Number of the route via which delivery is made to the customer. The route has to be created in the master data as via route for the delivery site:
⇨ Master Data, "Routes" on page B-259
**Technical info:** mandatory field, numeric field, DB field: kauf.routenr

**Travel time** Display of the duration to the delivery site. If a route is specified for which a travel time is stored, the travel time is displayed in plain text.
**Technical info:** display field

**Route days** Display of the days of the week on which the route is driven. If a route is specified, the associated days of the week are drawn from the master data and displayed in plain text.
**Technical info:** display field

**Area** Indication of the country code with naming of the dispatch region.
**Technical info:** display field

**Tonnage** Display of the load capacity of the vehicle in kilograms. This field can be configured at will.
**Technical info:** display field

**Requested del. date** Planned delivery date from the delivery site to the customer.
**Technical info:** display field, DB field: kauf.ltplan

**Calendar** Indication whether the calendar will be used for the delivery date determination. You can specify in the route master data for each route whether the calendar will be evaluated.
☑ The calendar will be used for the delivery date determination.
☐ The calendar will not be used for the delivery date determination.
**Technical info:** checkbox

#### Customer

**Requested del. date** Date of delivery requested by the customer.
**Technical info:** Date field, DB field: kauf.ltideal

**Arrival date** Date on which the delivery will probably reach the customer. The arrival date is calculated using the delivery date, the travel time, and the route days.
**Technical info:** display field

**Date status** Status indicator whether the customer's requested date and the calculated arrival date of the delivery match.
**Technical info:** display field

| Symbol | Status indicator | Meaning |
| :--- | :--- | :--- |
| ● | green | The probable delivery date corresponds precisely to the customer's requested date. |
| ● | yellow | The probable delivery date is before the customer's requested date. |
| ● | red | The probable delivery date is after the customer's requested date. |

*Tab. D-12 Date Status*

#### Calendar section

The calendar section displays a section of three weeks around the customer's requested date. All dates, e.g. planned delivery date, customer's requested date, delivery date in the producing site, etc. that are in this period are displayed on the corresponding days. You can display information about the date in question as a tool tip.

---
*A+W Enterprise Sales*
*D-1387, D-1388, D-1389, D-1390*

---

### Delivery notes (automatic)

**Sales > Delivery Notes > Automatic Release**

*Fig. D-143 Delivery notes (automatic)*

On this dialog, you generate delivery notes as accompanying documents for order delivery. On this dialog you can also generate invoices and complete documents.

If the Shipping Control module is configured in your system, you should only create delivery notes in the Shipping Control module. By default, the system is not configured to create delivery notes in the Sales module.

> **Inconsistencies with shipping control**
> Creating delivery notes in Sales can cause inconsistencies with Shipping Control since the status bookings, e.g. quantities packed or reported complete are only up-to-date in the Shipping Control. For customer-specific adjustment, please contact your partner at A+W Software GmbH.

-   **Release:** Specification of the release type for the selected document.
    -   **Delivery note:** A delivery note will be generated for the selected document.
    -   **Invoice:** An invoice will be generated for the selected document. You can only generate an invoice for documents for which a delivery note exists.
    -   **DN + Invoice:** A delivery note and invoice will be generated for the selected document.
    -   **Complete document:** The selected document is completed. Changes to the document will no longer be forwarded to the system.
-   **Site:** Site number.
-   **Document:** Document number. For delivery note generation, you specify the number of the order, for invoice generation the number of the delivery note. The order and delivery note number are identical. For the delivery note, you can also specify the subnumber for partial deliveries.
-   **SubNo:** Subnumber of the document, e.g. of the partial delivery note. The subnumber must be specified to generate a delivery note.
-   **Grp:** Dispatch group. Delivery notes can be assigned to a dispatch group in the dispatch planning. The dispatch groups are stored in the system master data. The dispatch group serves as additional identifier for the route locking.
-   **Deliv. note:** Information as to whether a delivery note or partial delivery note exists. If there is already a delivery note, then this field will show exists.
-   **Invoice:** Invoice number.
-   **Cust. no.:** Customer number.
-   **Cust.:** Customer name.
-   **Date:** Date of the document entry.
-   **Val.date:** Period until the value date in days.
-   **Cr.:** Create. Indication of whether the delivery notes and/or invoices should be generated.
    -   ☑ Yes, generate.
    -   ☐ Do not generate.

#### Footer

Customer name and the total net amount are shown.
Use `<F2>` to display the following fields:

-   **Amount:** Total net amount.
-   **Emp.:** Employee number of the person who entered the document.
-   **Entered by:** Name of the person who entered the document.
-   **Document date:** Corresponds to the Date field.

---
*A+W Enterprise Sales*
*D-1391, D-1392*

---

### Delivery notes (manual)

**Sales > Delivery Notes > Manual Delivery Notes**

*Fig. D-144 Delivery notes (manual)*

Use this dialog to manually generate and edit delivery notes. You only generate delivery notes manually if you have to correct the order data, e.g. in case of a different delivery quantity.

If the Shipping Control module is configured in your system, you should only create delivery notes in the Shipping Control module. By default, the system is not configured to create delivery notes in the Sales module.

> **Inconsistencies with shipping control**
> Creating delivery notes in Sales can cause inconsistencies with Shipping Control since the status bookings, e.g. quantities packed or reported complete are only up-to-date in the Shipping Control.
> For customer-specific adjustment, please contact your partner at A+W Software GmbH.

The fields and tabs are described for the Order Entry dialog:
⇨ "Order entry" on page D-1133

In addition, the following fields are displayed.

#### Header

**Order** Number of the order and subnumber. You assign subnumbers for partial delivery notes. Use `<TAB>` to assign the next free subnumber automatically. If delivery notes are already entered for an order, you can enter the subnumber and call up the already created delivery note.

#### General tab

**Received** Item quantity that has already been delivered with the previous delivery note.

**Deliv.** Quantity of the article that are being delivered with the selected delivery note.

---
*A+W Enterprise Sales*
*D-1393, D-1394*

---

### Delivery notes log

**Sales > Delivery Notes > Log**

*Fig. D-145 Delivery notes log*

This dialog displays the delivery notes log. All documents for the delivery notes are noted with the specification of the date and the time.

If you are working with internal site separation, first a dialog opens where you can specify the site number. The log displays only the documents for the selected site.

> **Delivery note log for the current day**
> A delivery note log is generated for the current day. If the error message is displayed that the file is empty or cannot be read, then no delivery note has been generated on this day.

---
*A+W Enterprise Sales*
*D-1395*

---

## Invoices

To account for customer orders, invoices are generated an sent to the financial accounting (FinAc).
You can create the invoices automatically or manually. An invoice can only be created if a delivery note exists.

The following dialogs are described in this section:

-   "Invoices (automatic)" on page D-1397
-   "Item info" on page D-1400
-   "Invoices (manual)" on page D-1402
-   "Cash transaction" on page D-1404
-   "Booking of invoices" on page D-1405
-   "Partial invoice (automatic)" on page D-1407
-   "Partial invoice (manual)" on page D-1409
-   "Final invoices (automatic)" on page D-1410
-   "Final invoices (manual)" on page D-1412
-   "Invoice log" on page D-1413

---
*A+W Enterprise Sales*
*D-1396*

---

### Invoices (automatic)

**Sales > Invoices -> Automatic Release**

*Fig. D-146 Invoices (automatic)*

Use this dialog to create invoices for documents and send them to Financial Accounting. You can import the documents for which invoices can be generated or you can specify the document numbers manually.

Use `<Ctrl>+<F8>` to import the data for all documents for which an invoice can be generated. The data is imported via a freely configurable SQL query. The amount of data to be imported depends on the SQL query in question. You can use the query that is configured by A+W by default or specify a customer-specific SQL query for the data import.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

The footer displays the customer name and total amount from the order for which an invoice is being created.

If you have not yet booked an invoice, you can view additional information on the Invoices dialog and edit the invoice, e.g. to correct it.
⇨ "Invoices (manual)" on page D-1402

On this dialog, you can also generate the delivery note together with the invoice or complete the document.

Use `<F3>` to have the system generate the invoices for the selected orders.

#### Information on document tab

-   **Release:** Specification of which documents you are releasing for the document that is specified in the Document field.
    -   **Invoice:** An invoice will be generated for the document.
    -   **DN + Invoice:** A delivery note and invoice will be generated for the document.
    -   **Complete document:** The selected document will be completed, that is, it can no longer be edited.
    -   **Delivery note:** A delivery note will be generated for the document.
    **Technical info:** toggle field, DB field: kauf.vorgang
-   **Site:** Display of the site number.
    **Technical info:** display field, DB field: kauf.hausnr
-   **Document:** Document number.
    **Technical info:** mandatory field, numeric field, DB field: kauf.auftrnr
-   **SubNo:** Number of the partial delivery note. If the document is generated for a complete delivery, a 1 is displayed.
    **Technical info:** numeric field, DB field: kauf.subnr
-   **Grp:** Dispatch group. Delivery notes can be assigned to a dispatch group in the dispatch planning. The dispatch groups are stored in the system master data. The dispatch group serves as additional identifier for the route locking.
    **Technical info:** numeric field, DB field: lapool.vsgruppe
-   **Deliv. note:** Indication as to whether a delivery note or partial delivery note exists. If there is already a delivery note, then this field will show the entry `exists`.
    **Technical info:** display field
-   **Invoice:** Number of the invoice if an invoice exists.
    **Technical info:** display field
-   **Cust. No.:** Customer number.
    **Technical info:** display field, DB field: kauf.kunr
-   **Cust.:** Display of the customer name.
    **Technical info:** display field, DB field: mp.name
-   **Document date:** Date of the invoice creation or invoice booking. By default, the field is prepopulated with the current date. For invoices and delivery notes, you can change between document and booking date with `<Ctrl>+<B>`. Via the column header, it is indicated which date is currently displayed.
    **Technical info:** mandatory field, date field, DB field: kauf.edat
-   **Val. date:** Period until the value date in days up to a maximum of 99 days.
    **Technical info:** display field, DB field: kauf.valuta
-   **Cr.:** Create. Indication of whether the selected documents should be generated.
    -   ☑ Yes, generate.
    -   ☐ Do not generate.
    **Technical info:** checkbox

Use `<F2>` to change to the Information on Document tab.

#### Information on document tab (alternative view)

The columns are described for the Documents tab:
⇨ "Information on document tab" on page D-1398

In addition, the following columns are displayed:

-   **Amount:** Indication of the invoice amount.
    **Technical info:** display field, DB field: kauf.nettototal
-   **Rec., operator:** Display of the operator number and name.
    **Technical info:** display fields, DB fields: kauf.eust, mitarb.maname

#### Footer

The footer displays the customer name and invoice amount from the document.
Use `<F5>` to open the **Items** dialog on which additional details about the invoice items are displayed.
⇨ "Item info" on page D-1400

---
*A+W Enterprise Sales*
*D-1397, D-1398, D-1399*

---

### Item info

**Sales > Invoices -> Automatic Release > Enter values > `<F5>`**
**Sales > Invoices > Partial Invoice, Final Invoice > Automatic Release > Enter values > `<F5>`**
**Sales > Credit Notes > Book Credit Notes > Enter values > `<F5>`**

*Fig. D-147 Items info*

This dialog displays the details of the individual items from the automatic invoice or credit creation.

#### Item info I tab

-   **Docum.:** Document number.
    **Technical info:** numeric field, DB field: kauf.auftrnr
-   **Itm:** Number of the item in the document.
    **Technical info:** numeric field, DB field: kpos.lfdpos
-   **Article, Designation:** Number and description of the article.
    **Technical info:** numeric field, alphanumeric field, DB fields: kpos.artnr, kpos.artbez1
-   **I:** Indication of whether the item has been invoiced.
    **Technical info:** display field, DB field: kauf.fakturakz

---
*A+W Enterprise Sales*
*D-1400*
