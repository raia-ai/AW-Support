---
title: "EN-UM-AWEnterprise_17"
source: "EN-UM-AWEnterprise_17.pdf"
tags: ["A+W Enterprise", "Purchasing", "Stock Management", "Software Reference", "ERP", "Purchase Orders", "Receipt of Goods", "Invoicing", "Document Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A software reference manual for the A+W Enterprise system, covering the Purchasing and Stock modules. It details procedures for purchase order entry, item management, goods receipt, invoicing, and provides overviews of various system functions."
long_description: "This document is a comprehensive software reference guide for the A+W Enterprise system, specifically focusing on the Purchasing and Stock modules. The Purchasing section provides detailed instructions on managing the entire procurement lifecycle, including creating and managing purchase orders, defining totals, discounts, and surcharges. It covers the various tabs for purchase order items such as general details, properties, prices, order info, status, and evaluation. The guide also explains how to handle the receipt of goods, both automatically and manually, manage dispatch notifications, and log goods receipts. The section on Invoices and Credit Notes describes the process for invoice checking, automatic and manual invoice creation (including collective invoices), booking invoices, and managing credit notes. The document concludes the Purchasing module with overviews and search functionalities. The latter part of the document introduces the A+W Enterprise Stock module, providing a high-level overview of its menus and functions for stock bookings, master data management, inventory, evaluation, and system administration."
---

# A+W Enterprise Purchasing

## Purchase order entry - totals

**Path:** `Purchase > P.O. Management > Open Purchase Order > Items Tab > General Tab > Price Field > <End> > Net Total Field > <F2>`

*Fig. E-17 Purchase order entry (totals)*

On this dialog, you define discounts, rebates, and surcharges for the entire purchase order and you can edit various payment options.

Discounts are arranged with suppliers. You can define a generally applicable discount in the master data and allocate a supplier-specific discount to each supplier. For a purchase order with selected suppliers, the supplier-specific discount is always allocated first. If no discount has been defined for this sup-plier, the general discount is applied.

The dialog is described in detail in the Sales section.
⇨ Sales, "Order entry - totals" on page D-1155

## Purchase order entry - discounts detailed view

**Path:** `Purchasing > P.O. Management > Open Purchase Order > Items Tab > General Tab > Price Field > <End> > Net Total Field > <F2> > <F5> > <F5>`

*Fig. E-18 Discounts detailed view*

Enter the details relating to the selected discount on this dialog.

The dialog is described in detail in the Sales section.
⇨ Sales, "Order entry - detailed view discounts" on page D-1160

## Purchase order items

**Path:** `Purchasing > P.O. Management > Open Purchase Order > Items Tab – General Tab`

The Items tab offers the following tabs:
*   "Purchase order items - general" on page E-1604
*   "Purchase order items - properties" on page E-1613
*   "Purchase order items - prices" on page E-1617
*   "Purchase order items - order info" on page E-1620
*   "Purchase order items - status" on page E-1622
*   "Purchase order items - evaluation" on page E-1624

On the item level, you can enter shapes, processings, steps, and muntin anew or view and change this information in the POs created. You can also view and adjust the sales prices for the items.

The dialogs are described in detail in the Sales section.
⇨ Sales, "Muntin entry" on page D-1281
⇨ Sales, "Stepped entry (relevant parts)" on page D-1278
⇨ Sales, "BOM view" on page D-1249
⇨ Sales, "Shape - dimensions" on page D-1232
⇨ Sales, "Prices and Conditions" on page D-1319

## Purchase order items - general

**Path:** `Purchasing > P.O. Management > Open Purchase Order > Items Tab – General Tab`

*Fig. E-19 Purchase order items - general*

In this area, you enter and edit the items of a purchase order. You can select the articles, the dimensions, quantity, and supply type and assign processings to the articles.

In the event of a status change, a corresponding note regarding the purchase order status is shown at the level of the tab. In front of the Item field, the item status and if necessary the item code are displayed as traffic light.
⇨ "Explanation of symbols" on page E-1580

Order-related purchase orders and stock purchase orders are usually executed using the Create Purchase Orders dialog and can be edited in the P.О. Management if required.
⇨ "Creating purchase orders" on page E-1569

### Header
The fields in the header area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

### Items tab (left area)
In the Info area, various information about the marked item is displayed. The technical values can be edited.
⇨ "Items tab (Info area - graphic, technical values)" on page E-1607

*Fig. E-20 Items tab (info area left)*

This area displays information about the marked item. The information about the header article is always displayed. All other information is only displayed if it exists. If no information exists, the corresponding position remains empty.

**Ref.** Commission text for printing. The field can only be entered if the appropriate flag is set for the article in the master data. For the first item, you can enter the commission text directly. If you enter a new item, the commission text of the previous item is taken over automatically. Alternatively, there are the following possibilities:
*   Use `<F4>` > References > New Reference or Change Reference to create a new reference text via the supplementary menu or to change the existing reference text for the entire purchase order.
*   Use `<Shift>+<F11>` to change from the item level to the text entry for the reference in order to create a reference text for the selected item.

Use `<Enter>` to change from the Commis field to the General tab, which is in the item area in order to continue item entry.
Technical info: alphanumeric field, DB field: komm.kommtxt

> **Inheriting reference text**
> If you assign a reference text to an item with `<Shift>+<F11>`, the reference text can be taken over for all following items. For this, you have to confirm the query whether the reference should be inherited downward with [Yes]. If you click [No], the reference text is only taken over for the current item. The query is only displayed if additional items are entered after the current item. However, it is not usual to enter the reference texts in the Purchase area. In the rules, the reference texts are transferred from Sales for order-related purchase orders.

**DoP:** Declaration of performance. Description of the declaration of performance that is assigned to the article. The field is only displayed if a declaration of performance is assigned to the current article.
Technical info: display field, DB field: kposp.lbrefnr

**(CAD identifier)** Identifier that indicates whether a CAD file is assigned to the item. If a CAD file is attached, the CAD identifier is displayed. For S/N items, the S/N code is displayed in brackets next to the CAD identifier.
Technical info: display field

**(Cost center)** Designation of the cost center that is assigned to the item. If no cost center is assigned to the item, the market partner-specific cost center is used. If no cost center is assigned to the market partner, the main cost center will be used.
Technical info: display field, DB field: kpos.kostenst

**(Muntin flag)** Identifier that indicates whether muntins are entered in the item.
*   **S:** Muntins are entered in the item. The muntin structure was not edited.
*   **E:** Muntins are entered in the item. The muntin structure was edited in the editor.
*   **(no identifier):** No muntins are entered in the item.

Technical info: display field

**(Header, article)** Description of the header article. With multiple glasses, in addition to the header article, the descriptions of the individual glasses are displayed.
Technical info: display field, DB field: aufstrukt.artbez1

**(Exchange, additional article, quantity1/quantity2)** Description of the exchange and additional articles and number of articles in the BOM. Exchange articles are displayed with an A, additional articles with a Z in front of the description. Next to the article description, it is indicated how frequently the value width and how often the value height must be calculated for the article.
Technical info: display fields, DB fields: aufstrukt.artbez1, aufstrukt.anzahl1, aufstrukt.anzahl2

**(Muntin exchange, muntin additional article, quantity1/quantity2)** Description of the muntin exchange and/or muntin additional article and number of muntins in the BOM. Muntin exchange articles are marked with an A, muntin additional articles with a Z in front of the description. The quantity of horizontal and vertical muntins is displayed after the muntin description.
Technical info: display fields, DB fields: aufstrukt.artbez1, aufstrukt.anzahl1, aufstrukt.anzahl2

### Items tab (Info area - graphic, technical values)
On the right side of the Items tab, depending on the system configuration and the settings, some of the following information is displayed:
- Supply, product group and shape
- Technical details
- Hidden dimensions

The information is displayed for the marked item.

*Fig. E-21 Items tab (info area right)*

On the right, there is a schematic depiction of the product. If you have entered a shape and/or muntins in the item, a schematic product depiction is also displayed on the left.

**Customer** Customer name. The field is only displayed for order-related purchase order items.
Technical info: display field, DB field: mp.name, kauf.kunr

**ProductGrp** Product group number of the item. Articles are divided into product groups for product grouping and analysis of statistics. When you change the BOM of an item, the product group may also change.
*   Use `<Ctrl>+<F9>` to change from the item level to the input field of the product group.
*   Use `<F9>` to open the selection list for the product group. Alternatively, you can specify a product group number. A correction of the product group is only possible under certain circumstances.
Technical info: display field, DB field: kpos.wgrp

**Shape** Shape number.
*   Use `<Ctrl>+<F12>` to change from the item level to the input field for the shape number.
*   Open the Shape Catalog with `<F2>`.
*   Open a selection of shape names with `<F9>`.

Alternatively, you can enter the shape number directly in the field. After specifying a shape number, the shape entry begins. By default, the system is configured with the A+W shape catalog.
⇨ Sales, "Shape - dimensions" on page D-1232
Technical info: display field, DB field: kpos.modnr

### Technical details
Use `<F4> > Product Details > Technical Details` to select one of the following entries on the additional menu:
*   **Show Technical Details:**
    Displays the technical details of the selected item. If the selected item is already assigned a declaration of performance, the Calculated Technical Values tab opens.
    ⇨ Sales, "Calculated technical values" on page D-1242
*   **Change technical details:**
    Changes to the input fields for the technical details of the selected item. You can edit the fields.

Use `<End>` to save the changes and change back to the General tab.

**Item** Item number of the selected item. The field is only displayed if you change the technical details.
Technical info: display field, DB field: kpos.posnr

**Article code** Article code of the selected item. The field is only displayed if you change the technical details.
Technical info: display field, DB field: ktechw.artnrgen

**Total thickn.** Glass thickness for the total article of the item. The glass thickness depends on the selected facade zone and the wind load. The entry is made in millimeters. The field is only displayed if you change the technical details.
Technical info: numeric field, DB field: ktechw.dicke

**Wind load** Wind load in the installation location. Wind load (N/m²) is the pressure applied by direct winds onto the external surface of a building. The system uses this value to perform a plausibility check to determine whether the thickness group of the selected glass types suffice for the wind load defined. The field is only displayed if you change the technical details.
Technical info: numeric field, DB field: ktechw.wlast

**Section** Specification of the facade zone in which the lites will be installed. E.g. tall buildings or buildings on the outskirts are loaded with increased wind load. The field is only displayed if you change the technical details.
*   **Edge:** For buildings with increased wind load.
*   **Central:** For buildings without increased wind load.
Technical info: toggle field, DB field: ktechw.bereich

If you edit the technical details, additional fields are displayed with `<F2>`.

**U Val. DIN** Heat transmission coefficient according to DIN standard. Central dimensional unit for determining the heat loss of a component. The measurement unit is W/m²K. The lower the Ug value, the greater the heat insulation.
Technical info: numeric field, DB field: ktechw.kwert

**Ug value** Heat transmission coefficient.
Technical info: numeric field, DB field: ktechw.kbazwert

**Transmiss.** Light transmission for the percentage of rays that are allowed to pass through. The reference value of 100 % is an unglazed hole in the wall.
Technical info: numeric field, DB field: ktechw.trwert

**g value** Energy transmission coefficient (total transmittance). The variable is composed of direct solar energy transmission and secondary heat emission to the inside, as a result of slow radiation and convection.
Technical info: numeric field, DB field: ktechw.gwert

**dB value** Sound insulation value of the item in decibels.
Technical info: numeric field, DB field: ktew.dbwert

### Hidden dimensions
Use `<F4> > Product Details > Technical Details` to select one of the following entries on the additional menu:
*   **Show hidden dimensions:** Displays the hidden dimensions of the selected item next to the graphic display of the item, e.g. the spacer deduction dimension.
*   **Change hidden dimensions:** Opens the Item dimensions dialog where you can edit the various dimensions of the item.

Depending on the item selected, various parameters are listed. Use `[OK]` or `<End>` to save the changes and close the dialog.

The fields are described in detail in connection with the Article-Dimensions dialog.
⇨ Sales, "Article dimensions" on page D-1203

### Graphic display of the item
Various previews are displayed for the item:
*   **Schematic view:** Shows the lite structure as a cross-section. The sun marks the outside of the lite. The schematic structure of the item is always displayed.
*   **Top view:** Displays the lite shape and/or the muntin construction of the lite in the top view. The top view is only displayed if you have entered a shape and/or muntins in the item.

### General tab
The layout of the item level, especially on the General tab depends on the article type that you select. This way, some fields are shown or hidden, e.g.: AIR.

The following fields are available:

**Itm** Item number. Displayed in front of the Itm column, are the item status and if necessary the item code of the item in question. The item status is only displayed after saving the document.
Technical info: numeric field, DB field: kpos.lfdpos

**Supp. item** Supplier item. Specification of the item description from the supplier's item list. The field is only enabled if the entry yes is selected in the Suppl.Item field of the header area.
The item description can be printed on all customer and supplier-side documents.
⇨ "Purchase order entry - header, footer" on page E-1585
Alternatively, you can enter the article name of an existing, fixed-size article. The system then pre-populates the fields with the article data.
⇨ Sales: Software Reference, "Article details for dimensioned variants" on page D-1214
Technical info: numeric field, DB field: kpos.kuposnr

**Article** Article number. In the Article field you can enter a customer- or supplier-specific article number.
- Use `<F9>` to open the article search.
- Search for customer-specific articles with `<F10>`.
⇨ Sales: Software Reference, "Article details for dimensioned variants" on page D-1214
Technical info: mandatory field, numeric field, DB field: kpos.artnr

> **Assign original or new BOM**
> You can assign the article the original BOM or a new BOM. The BOM number is assigned accordingly. With `<F5>` in the Article field, you take over the article's original BOM. With `<Shift>+<F5>` in the Article field, you assign the article a new BOM. The article is assigned the next free BOM number by the system. In the rules, the product BOM in the Sales area is not adjusted.

**BMno** BOM number of the article. By default, the number is assigned automatically. The BOM includes all parts and processings required for manufacturing of the article. Every item in the BOM automatically gets a unique BOM number which is shown in field BOMNo. After the quantity and the dimensions of the item were specified, you can use `<F3>` to display and edit the item's BOM. The entry in this field has an influence on the price calculation. The field is locked.
⇨ Sales, "Item processing" on page D-1273
Technical info: numeric field, DB field: kpos.poskonr

**Quantity** Units of the item. For articles with stored dimension, color or thickness variants, after entry of the quantity, a dialog opens for selection of the respective variant.
⇨ Sales, "Variant and color/thickness selection" on page D-1217
Technical info: mandatory field, numeric field, DB field: kpos.menge

**Width, Height, AIR** Width, height, and airspace in the dimensional units stored for the article. For variant articles, the system takes the dimensions from the article master data using the selected variant number. If you change these dimensions, the query appears: Can the variant reference really be removed?
- Click on [No] to reset the entered sizes to the stock sizes.
- Click [Yes] to change the stock sizes. This can cause problems in the warehouse and with pricing.
Technical info: mandatory fields, numeric fields, DB fields: kpos.laenge, kpos.breite, kpos.szr

**(Columns without name)** For length, time, and piece articles, instead of width, height, and AIR, the dimension and corresponding dimension unit that are assigned to the selected article are displayed. The dimension unit of the article is drawn from the master data and cannot be edited. For installation work, for example, the dimension unit hr (hours) is displayed, for gas fillings l (liters) and for adhesive tape m (meters). You can select the dimension at will.
Technical info: mandatory field, numeric field, DB field: kpos.laenge

> **Calling up BOM of the item**
> Use `<F3>` or `<F5>` to open the BOM for the selected item. You can only open the BOM after you have specified the dimension. If you try to open the BOM before that, the system will notice this action and open the BOM automatically after specification of the dimension. In addition to the item, you will see a gray checkbox. A message with this information will also be displayed.

**SN** The checkbox indicates whether an SN file is assigned to the item.

**Comm** Commission with active representative commission. You can specify the commission key granted for each item individually. With inactive or margin-oriented commission calculation, the field is locked and will not be considered.
Technical info: numeric field, DB field: kpos.provnr

**PType** The supply type determines how an article is supplied. In purchasing, the field is pre-populated with the supply type PO and cannot be changed.
Technical info: Toggle field, database field: kpos.beschaffart

**lbs/Pc, Qty/Pc** Quantity unit in kilograms per piece, quantity unit in square meters per piece.
Use `<Ctrl>+<M>` in Price filed to change the display of the field.
Technical info: display field, DB field: kpos.gewme

**Price(field)** Net price per item. The column name varies depending on the own currency and configuration, e.g. Price/piece, Price/m2. The system calculates the total price of the item including the conditions in the selected currency. You determine the currency in the Currency/Rate field on the Miscellaneous tab.
Use `<Shift>+<F11>` to change the display of the field.
- Use `<Shift>+<F8>` to save the order in the master data as fixed dimension product.
  ⇨ Sales, "Article details for dimensioned variants" on page D-1214
- Use `<Ctrl>+<F9>` to determine the PU price with the item conditions and recalculate the price.
- Use `<F3>` to display an overview of the dimensions of the individual items.
  ⇨ Sales, "Dimensions of individual BOM elements" on page D-1274
Technical info: numerical field, DB field: kpos.nstpreis

The following columns display on the tab if you use `<F4> > Price info > Price check:`

**SA** Pre-sales price code from the transferring site.
Technical info: display field, DB field: kpos.vorvkpkz

**PCD** Pre-sales price code from the transferring site.
Technical info: display field, DB field: kpos.vorpkz

**nSA** Newly determined sales price code.
Technical info: display field, DB field: kpos.neuvkpkz

**pSF** Pre-sales price factor from the transferring site.
Technical info: display field, DB field: kpos.vorvkfaktor

**Factor** Percentage pre-sales factor from the transferring site.
Technical info: display field, DB field: kpos.vorfaktor

**nSF** Newly determined sales factor.
Technical info: display field: DB field: kpos.neuvkfaktor

**pSA-Pr.** Pre-sales price from the transferring site.
Technical info: display field, DB field: kpos.vorpreis

**nSA-Pr.** Newly determined sales price.
Technical info: display field, DB field: kpos.neuvknstpreis

With `<F4> > Stock> Stack` you can show the following field with the right system configuration.

**Stack** Stack ID of the article that is obtained from the stack warehouse.

Use `<Shift> + <F4> > Note` to display an additional field:

**Note** You can enter information about the item. The information will be displayed in OrderInfo tab.

If you select the box warehouse in the Warehouse field on the Properties tab and the system is configured appropriately, the following fields are shown:

**NB** Number of boxes.

**Lite** Number of lites per box.

**PT** ID of the packing type Box.

### Footer
The fields in the footer area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

## Purchase order items - properties

**Path:** `Purchasing > P.O. Management > Find Purchase Order > Items Tab > Properties Tab`

*Fig. E-22 Purchase order item - properties*

On this tab, you can view and edit the properties of the current item, e.g. warehouse assignment, packing type. You enter the properties individually for each item. Generally you do not have to edit the details on the Properties tab.

Use `<Page Up>` and `<Page Down>` to change to the previous and next item.

In the event of a status change, a corresponding note regarding the purchase order status is shown at the level of the tab, e.g. Ordered Local – Correction. In front of the Item column, the item status and if necessary the item code are displayed.
⇨ "Explanation of symbols" on page E-1580

### Header
The fields in the header area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

### Properties tab
The columns are described for the General tab:
⇨ "Purchase order items - general" on page E-1604

In addition, the following fields are displayed:

**Description** Description of the header article. You can edit the name. The change is only taken over purchase order-related.
Technical info: alphanumeric field, DB field: kpos.artbez1

> **Changes to the description**
> Once changed in this item, the article description will appear on all purchase order-related documents and on all purchase order-related dialogs for this document.

**Cost center** Cost center name for statistical evaluations.
Technical info: alphanumeric field, DB field: kauf.kostenst

**DOP number** Number for declaration of performance. You can select or register a new number. Use `<Ctrl>+<T>` to open the Calculated technical details tab where you can enter a new declaration of performance. You can only register a new number if the item has not yet been assigned a declaration of performance. A declaration of performance can only be entered if the system is configured appropriately.
⇨ Sales, "Calculated technical values" on page D-1242
Technical info: alphanumeric field, DB field: kpos.lbrefnr

**Warehouse** Number of the warehouse where the article is located. If you select a number, the description of the warehouse is displayed in plain text.
Technical info: numeric field, DB field: kpos.Inr

**Stack** Number of the stack warehouse where the article is located. If you select a number, the description of the stack warehouse is displayed in plain text. The stack warehouse is only enabled customer-specifically.
Technical info: numeric field, DB field: kpos.sfill1

**Box** Number of the box warehouse where the article is located. Only complete boxes of an article are entered in the box warehouse. If articles from a box are required, the remaining lites are booked to the normal stock. If you select a number, the description of the box warehouse is displayed in plain text. The box warehouse is only enabled customer-specifically.
Technical info: numerical field, DB field: bpos.kistennr

**Slot** Name of the slot warehouse where the article is located. Usually, slot warehouses are used for articles that are billed by pieces or quantities, e.g., handles, spacers. The slot warehouse is only enabled customer-specifically.
Technical info: numerical field, DB field: bpos.fach

**CE code** CE code. You can enter or change a descriptive text. The text is added to the CE code.
Technical info: alpha-numerical field, database field: kpos.steuerzu

**Account** Description of the cost center booking account.
Technical info: alphanumeric field, DB field: kposp.mankonto

**Reject reason** Number of reject reason. The number only needs to be specified if an item needs to be ordered due to glass breakage. If you specify a number, the reject name is displayed in plain text.
Technical info: numeric field, display field, DB field: bpos.bruch

**Reject place** Number and name of the reject place where the glass break happened. The number only needs to be specified if an item needs to be reordered due to glass breakage. Generally the reject place is transferred from production and taken over in this field. If needed, you can change the reject place. The reject place name is displayed in plain text in the next field.
The reject places are stored in the database table xbruchort. The values from production are taken over automatically. There is no maintenance dialog for this table in A+W Enterprise.
Technical info: numeric field, display field, DB field: bpos.bruchort

**Print sketch** Type of the sketch, e.g. SNLive. You can select none, one or several sketch types. The sketch types can be configured in the system. The sketch printing can be activated for SN Live sketches, BOMs (AWBom), sketches for muntins (AWDesign) or schematic sketches (outline). An individual sketch is printed for each sketch type.
*   Open the list of sketch types with `<F9>`.
*   Use the arrow keys to navigate between the sketch types.
*   Use `<Space>` to mark a sketch type.
Use `<End>` to close the dialog and take over the selection.
Technical info: selection field, DB field: ipos.imagedrkz.
In this field, there is a 4-digit number, in which each place indicates an appropriate sketch activation with a 1:
*   1st digit: SNLive sketch.
*   2nd digit: AWBom.
*   3rd digit: AWDesign.
*   4th digit: Outline sketch.

**Ibs/QU, Ibs/Piece, Ibs/Item, Ibs/GI** Weight of the item. The details can be displayed in the following fields:
*   kg/QU: kilogram per quantity unit
*   kg/Piece: kilogram per piece
*   kg/Item: kilogram per item
*   kg/Gl: kilogram per glass
Only the field is enabled whose weight specification is assigned in the master data of the current article.
Technical info: numeric fields, DB fields: kpos.gewme, kpos.gewst, kpos.gewpos, kpos.gewglas

**Actual QU/Pc** Physical quantity in quantity unit per piece.
Technical info: numeric field, DB field: kpos.phymestk

**Chargd. QU/Pc** Calculated quantity in quantity unit per piece.
Technical info: numeric field, DB field: kpos.qm

**Pack. type** Number of the packing type, e.g. box. If you select a number, the description is displayed in plain text.
Technical info: numeric field, DB field: kpos.verpackart

### Footer
The fields in the footer area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

## Purchase order items - prices

**Path:** `Purchase > P.O. Management > Open Purchase Order > Items Tab > Prices Tab`

*Fig. E-23 Purchase order item - prices*

This tab shows the purchase prices of the current item. The prices are displayed individually for each item.
Use `<Page Up>` and `<Page Down>` to change to the previous and next item. Usually, you do not need to open the Prices tab. If you want to edit the prices of the items, you have to edit the order and/or item conditions.

⇨ Sales, "Conditions for PCD processing" on page D-1338
⇨ Sales, "Conditions for PCD processing" on page D-1338

In the event of a status change, a corresponding note regarding the purchase order status is shown at the level of the tab, e.g. Ordered Local – Correction. In front of the Item column, the item status and if necessary, the item code are displayed.
⇨ "Explanation of symbols" on page E-1580

### Header
The fields in the header area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

### Prices tab
The columns are described for the General tab:
⇨ "Purchase order items - general" on page E-1604
In addition, the following fields are displayed:

**Price/QU** Price per quantity unit. The price is calculated from the glass price plus the surcharge.
Technical info: display field, DB field: kpos.ekbmepreis

**Gross pieces** Gross price per piece.
Technical info: display field, DB field: kpos.bmstpreis

**Factor** Factor for the price surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor. Therefore, the factor is <100%.
⇨ Sales, "Conditions for PCD processing" on page D-1338
Technical info: display field, DB field: kpos.ekfaktor

**Example**
If a supplier gives a discount of 10%, the corresponding value for the factor is 90%.

**Net pieces** Net price per piece.
Technical info: display field, DB field: kpos.eknstpreis

**Glazing/Pc.** Price per piece for glazing or installation work.
Technical info: display field, DB field: kpos.ekverglas

**Total price** Net total price of item. The total price is calculated from piece price x quantity of the article.
Technical info: display field, DB field: kpos.vorrabatt

**Minus** Minus. Individually agreed upon discount for the item. You can specify the discount in the first field as percentage or in the second field as amount. The system calculates the value for the other fields.
Technical info: numerical fields, DB fields: kpos.rabatt, kpos.nachlass

**Item price** Item price. The item price is calculated from the total price less the discount from the Discount field. You can overwrite this value, e.g. if a flat fee has been agreed upon. If you change the item price, the discount in the Discount field is adjusted automatically.
Technical info: numeric field, DB field: kpos.npospreis

**Tax rates** ID of the VAT rate per item. You can assign one VAT rate for each item.
*   Open the list of VAT rates with `<F9>`.
*   You can select a VAT rate with `<space>` (spacebar).
*   Save the VAT rate with `<End>`.
Technical info: selection field, DB field: kpos.steuerzu

### Footer
The fields in the footer area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

## Purchase order items - order info

**Path:** `Purchase > P.O. Management > Open Purchase Order > Items Tab > Order Info Tab`

*Fig. E-24 Purchase order item - order info*

This tab shows the referenced order information for the current item. The order information is displayed individually for each item.

In the event of a status change, a corresponding note regarding the purchase order status is shown at the level of the tab.
⇨ "Explanation of symbols" on page E-1580

### Header
The fields in the header area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

### Order info tab
The fields are described for the General tab.
⇨ "Purchase order items - general" on page E-1604
In addition, the following fields are displayed:

**Cust.order, Item** Order number and item number of order-related purchase orders.
Technical info: numeric fields, DB fields: bpos.vkauftrnr, bpos.vklfdpos

**Cst.project** Project number of the customer order for order-related purchase orders. If you specify a number, the description of the project is displayed in plain text.
Technical info: numeric field, display field, DB field: bpos.vkobjnr

**Orig. tupel** Parts number of the BOM item of the customer order.
Technical info: numerical field, DB field: bpos.orgtnr

**Note** Additional information on the item.
Technical info: alpha-numerical field, DB field: bpos.bemerkung

**Delivery date** Desired delivery date of the item.
Technical info: Date field, DB field: bpos.ltideal

**Sched.** Planned delivery date of the item.
Technical info: Date field, DB field: bpos.ltplan

**Confirmed** Delivery date of the item confirmed by the supplier.
Technical info: Date field, DB field: bpos.ltavis

**Confirmed qty.** Quantity of the delivery item as confirmed by the supplier. This confirmed quantity may differ from the ordered quantity.
Technical info: Date field, DB field: bpos.avismenge

**OC no.suppl.** Number of order confirmation from supplier.
Technical info: numerical field, DB field: bpos.abnr

**Sup.art.no.** Supplier's article number. If a supplier-related article number has been entered for this article in master data, this is shown here.
Technical info: alpha-numerical field, DB field: bpos.exartnr

**DN no.** Supplier's delivery note number.
Technical info: alpha-numerical field, DB field: bpos.lieferschein

**PurchDescr** Supplier-specific article description. If the article name used by the supplier has been entered for this article in the master data, it is shown here.
Technical info: alpha-numerical field, DB field: bpos.bestellbez

### Footer
The fields in the footer area are described for the Purchase Order Entry - Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

## Purchase order items - status

**Path:** `Purchase > P.O. Management > Open Purchase Order > Items Tab > Status Tab`

*Fig. E-25 Purchase order item - status*

This tab shows the status of the items, e.g. number of articles delivered and invoiced. As first item in the item overview, the item is displayed that is marked on the General tab. Generally you do not have to edit the details on the Status tab.

Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate in the item overview.

In the event of a status change, a corresponding note regarding the purchase order status is shown at the level of the tab, e.g. Ordered Local – Correction. In front of the Item column, the item status and if necessary the item code are displayed.
⇨ "Explanation of symbols" on page E-1580

### Header
The fields in the header area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

### Status tab
Some fields are described for the General tab.
⇨ "Purchase order items - general" on page E-1604
In addition, the following fields are displayed:

**Complt** Display of the units produced per item.
Technical info: display field, DB field: kpos.gesfert

**Packed** Display of the units packed and prepared for transport per item.
Technical info: display field, DB field: kpos.gespack

**Deliv.** Display of the units delivered per item.
Technical info: display field, DB field: kpos.geslief

**Calc** Display of the invoiced units per item.
Technical info: display field, DB field: kpos.gesberech

**Cancel** Display of the canceled units per item.
Technical info: display field, DB field: kpos.gesstorno

### Footer
The fields in the footer area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

## Purchase order items - evaluation

**Path:** `Purchase > P.O. Management > Open Purchase Order > Items Tab > Evaluation Tab`

*Fig. E-26 Purchase order item - evaluation*

On this tab, you display details about the delivery, e.g. how reliably the supplier delivers. You store the assessment criteria in the supplier master data. You can enter the corresponding fields for supplier assessment with `<Ctrl> + <N>` and change them if necessary.

### Header
The fields in the header area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

### Evaluation tab
Some fields are described for the General tab.
⇨ "Purchase order items - general" on page E-1604
In addition, the following fields are displayed:

**Date** Evaluation of the supplier's adherence to delivery dates for the item.
Technical info: alpha-numerical field, DB field: bpos.abnr

**Prices** Evaluation of the supplier's pricing for the item.
Technical info: alpha-numerical field, DB field: bpos.wpreis

**Quality** Evaluation of the quality of the delivered item.
Technical info: alpha-numerical field, DB field: bpos.wqual

**Qty.** Evaluation of the delivered quantity of the item.
Technical info: alpha-numerical field, DB field: bpos.wmenge

**Special** Evaluation of the supplier and the handling process.
Technical info: alpha-numerical field, DB field: bpos.wspec

### Footer
The fields in the footer area are described for the Purchase Order Entry – Header, Footer tab:
⇨ "Purchase order entry - header, footer" on page E-1585

## Pick-up address

**Path:** `Purchase > P.O. Management > Open Purchase Order > Field Entry Date > <F4> > Addresses > Pick-up Address`

*Fig. E-27 Pick-up address*

On this dialog, you enter a pick-up address. If you would like to pick up the goods yourself, you can store the pick-up address here.

**Name, 1stName** Customer's last name and first name.
Technical info: mandatory field, alphanumeric fields, DB fields: adr.adrname, adr.adrvname

**Title** Number of the customer's title. If you specify a number, the title is displayed in plain text.
Technical info: numeric field, DB field: adr.anrede

**Attn.** Contact's name.
Technical info: alphanumeric field, DB field: adr.zhd

**Additional** Additional information on the address.
Technical info: alphanumeric field, DB field: adr.branche

**Street** Street address of the pick-up address.
Technical info: alphanumeric field, DB field: adr.str

**P.O. box** Postal code and P.O. box number.
Technical info: alphanumeric fields, DB fields: adr.pfplz, adr.postfach

**PBoxCity** P.O. box code for the pick-up address (for customers outside Europe).
Technical info: alphanumeric field, DB field: adr.pfort

**Post code** Postal code of the pick-up address.
Technical info: alpha-numerical field, DB field: adr.plz

**City** City of the pick-up address.
Technical info: alpha-numerical field, DB field: adr.ort

**CCd country** International vehicle registration number of the country of destination. If you specify a code, the country name is displayed in plain text.
Technical info: alphanumeric field, DB field: adr.lfzcode

**Distance** Distance to the supplier in kilometers.
Technical info: numeric field, DB field: adr.kilometer

**Travel time** Travel time to the supplier in days.
Technical info: numeric field, DB field: adr.fahrtzeit

**Handling time** Time for loading and unloading the shipment.
Technical info: numeric field, DB field: adr.handlingszeit

**Arrival time** Requested arrival time to supplier in format hh.mm.
Technical info: alphanumeric field, DB field: adr.ankunftszeit

**Unloading point** Details of the shipping address, e.g. gate A.
Technical info: alpha-numerical field, DB field: adr.anlieferstelle

**Fax no.** Fax number of the supplier
Technical info: alphanumeric field, DB field: adr.fax

**Route** Number of the route.
Technical info: numeric field, DB field: adr.routenr

**Load.seq.** Number of the desired loading sequence. By default, the loading sequence is specified in shipping control. If you specify a number, it is transferred to shipping control and considered in route planning.
Technical info: numeric field, DB field: adr.routeposnr

**Remark** Text fields for additional information.
Technical info: alphanumeric fields, DB fields: adr.text1, adr.text2, adr.text3

## P.O. type

**Path:** `Purchase > P.O. Management > Open Purchase Order > Project Field > <Ctrl> + <F12>`

*Fig. E-28 Purchase order. types*

On this dialog, you specify the type of PO. By default, each PO has the PO type normal. If you select another PO type, it is displayed as dialog name in the header line of the dialog. Depending on the system configuration, the system may be able to change the PO type. The changed PO type will also appear as dialog name here.

*   **Normal purchase order:** Preset default for purchase order entry that also applies to stock P.O.s.
*   **Internal purchase order:** Internal purchase order between the own sites.
*   **Purchase order free-of-charge:** Purchase order with the invoice amount 0, e.g. in the event of a complaint of a purchase order. At the end of the entry, a dialog for specification of the complaint reason opens.
    ⇨ Sales, "Complaint" on page D-1211
*   **Forwarding purchase order:** This type is no longer supported!

## Allocation of document types

**Path:** `Purchase > P.O. Management > Open Purchase Order > Suppl. Item Field > <Ctrl> + <K>`
**Path:** `Purchase > P.O. Management > Open Purchase Order > Items Tab > General Tab > Prices Field > <Ctrl> + <K>`

*Fig. E-29 Allocation of document types*

On this dialog you assign files to a document or individual items. If you want to assign the file to the complete document, you have to open the dialog in the header area. If you want to assign the file to a particular item in the document, you have to open the dialog on the General tab in the document entry and open the appropriate item.

The assigned files are only displayed if you open the document type assignment for the document or the corresponding item. That is, documents that are assigned to the complete document are only displayed if the dialog is opened in the header area. Documents that are assigned to an item are only displayed if the dialog is opened in the corresponding item.

The dialog is described in detail in the Sales section.
⇨ Sales, "Allocation of document types" on page D-1223

> **Document allocation from the order**
> In the order entry, the allocated documents can be marked both on the header level and on the item level for takeover for the PO generated. For this, the checkbox Ord. activated must be enabled. This copies the allocated document to the new PO.

## Texts

Use texts to define additional information about document. The texts can be printed out on different forms. The menu items where you can view and manage the texts are the same in purchase and sales. They are described in detail in the Sales section.

⇨ Sales, "Notes" on page D-1300
⇨ Sales, "Header and footer texts" on page D-1308
⇨ Sales, "Article and item texts" on page D-1311
⇨ Sales, "Special texts" on page D-1312
⇨ Sales, "Phrases" on page D-1314
⇨ Sales, "External information" on page D-1316

### Order texts

**Path:** `Purchase > Create Purchase Orders > Select Department > <F3> > <Shift> + <F4> > Show Order Texts`

*Fig. E-30 Order texts*

On this dialog, the order texts for the PO articles are displayed. For a PO item, item and/or article texts from the associated order can be taken over. Article texts are marked with the letter A, item texts with the letter P.

On the Create POs dialog, there is an indication in the Txt column whether texts were entered for the PO item and what kind of texts are stored.
⇨ "Creating purchase orders - supplier" on page E-1570

As an alternative to the Info menu, you can call up the order texts with `<Ctrl>+<F10>` from the Create POs dialog.

You can only close the dialog via the Info menu or with `<Ctrl>+<F10>`.

## Form Printing

Use the `Printing of forms` or `Email` dialog to print purchase orders and send them to the supplier. The dialogs are described in detail in the Sales section:

⇨ Sales, "Form printing" on page D-1419
⇨ Sales, "E-mail" on page D-1423

## Purchase Order Release

**Path:** `Purchase > P.O. Release`

On this dialog, you can release, lock or cancel POs. Depending on the system configuration, the POs can also be approved directly after PO creation or PO entry.

In the change log, you can check the status of a PO. The dialog is described in detail for the Sales section:
⇨ Sales, "Amendment log" on page D-1228

This dialog contains the following views:
*   "Purchase order release - selection" on page E-1631
*   "Purchase order release – details" on page E-1633
*   "Purchase order release - additional fields" on page E-1635

### Purchase order release - selection

**Path:** `Purchase > P.O. Release`

*Fig. E-31 Purchase order release selection*

In this view, you select the PO that you want to edit.
*   Use `<F5>` to change to the Purchase order release – Details view.
    ⇨ "Purchase order release – details" on page E-1633
*   Use `<F3>` to trigger the selected function.

#### Header

**PO number** Purchase order number.
Technical info: numeric field, DB field: kauf.auftrnr

**Current** Current status of the purchase order.
*   **released:** the purchase order is released.
*   **created:** the purchase order is created but not released yet.
*   **canceled:** the purchase order has been canceled.
Technical info: display field, DB field: kaufstat.datum

**Action** Selection of the function that you want to trigger.
*   **released:** The PO is released.
*   **cancel:** The PO will be canceled and the items to be ordered placed back in the PO pool; they can be grouped into a different PO.
*   **reset:** The PO will be canceled. You can only reset POs that have the status released. Already-canceled POs cannot be reset. The reset PO remains in the system and can be released at a later point in time.
Technical info: display field

**Delivery date** Planned delivery date of the purchase order.
Technical info: display field, DB field: kauf.ltplan

**Supplier** Number and name of the supplier.
Technical info: display fields, DB fields: kauf.kunr, mp.name

**Canc. inform.** Note about cancellation. This field is only displayed if you cancel a PO and trigger the function with `<F3>`.
Technical info: alphanumeric field, DB field: kauf.exbez2

#### Footer

**Trigger**
Triggers the selected function for the current PO.

**Details**
Changes to the Purchase order release – Details view. Alternatively, you can use `<F5>` to change to the detail view.
⇨ "Purchase order release - details" on page E-1633

**End**
Closes the PO release dialog. Changes will not be saved.

### Purchase order release – details

**Path:** `Purchase > P.O. Release > Select P.O. > <F5>`

*Fig. E-32 Purchase order release - details*

In this view, the item details about the selected PO are displayed.
Use `<F2>` to change to the Purchase order release – Additional Fields view.
⇨ "Purchase order release - additional fields" on page E-1635

#### Header
The header is described for Purchase order release - Selection view:
⇨ "Purchase order release - selection" on page E-1631

#### Item overview

**Itm** Item number.
Technical info: numeric field, DB field: kpos.lfdpos

**Article** Article description.
Technical info: display field, DB field: kpos.artbez1

**Ordered** Quantity of the ordered item.
Technical info: numerical field, DB field: kpos.menge

**Width, Height** Dimensions of the item in millimeters.
Technical info: numeric fields, DB fields: kpos.laenge, kpos.breite

**Order** Order number for PO items from customer orders.
Technical info: numeric field, DB field: bpos.vkauftrnr

**Delivery** Planned delivery date of the customer order.
Technical info: date field, DB field: kauf.ltplan

#### Footer

**OK**
Closes the current view and changes to the Purchase order release – Selection view.
⇨ "Purchase order release - selection" on page E-1631

**Cancel**
Closes the current view and changes to the Purchase order release – Selection view.
⇨ "Purchase order release - selection" on page E-1631

### Purchase order release - additional fields

**Path:** `Purchase > P.O. Release > Select P.O. > <F5> > <F2>`

*Fig. E-33 Purchase order release - additional fields*

This dialog displays information about the selected purchase order item.
*   Use `<F2>` to change to the Purchase order release – Details view:
    ⇨ "Purchase order release - details" on page E-1633
*   Use `<Page Up>` and `<Page Down>` to change to the previous and next item.

#### Header
The header is described for Purchase order release - Selection view:
⇨ "Purchase order release - selection" on page E-1631

#### Purchase order details
In addition to the Purchase Order Release - Details fields, the following fields are displayed:

**Article** Number and description of the article.
Technical info: display field, DB field: kpos.artnr, kpos.artbez1

**Quantity** Quantity of the ordered item.
Technical info: display field, DB field: kpos.menge

**Confirmed** Quantity for delivery data as confirmed by the supplier.
Technical info: display field, DB field: bpos.avismenge

**SizeVar** Size variant of the ordered item for articles with variants.
Technical info: display field, DB field: kpos.var

**Lin.m.** Linear meters of the PO item. If the article is assigned the quantity unit linear meters in the master data, the actual quantity of linear meters ordered is displayed here. If the article is assigned the quantity unit area in the master data, the size of the lite ordered is noted here.
Technical info: display field, DB field: kpos.umlfdm

**Sqm** Glass area of the purchase order item in square meters.
Technical info: display field, DB field: kpos.qm

**AIR** Airspace in millimeters. The field is only preset for IG articles.
Technical info: display field, DB field: kpos.szr

**OC no.suppl.** Number of order confirmation from supplier.
Technical info: numerical field, DB field: bpos.abnr

**Item** Item number from the order in the case of order-related purchase orders.
Technical info: numerical field, DB field: bpos.vklfdpos

**Customer** Customer name of the PO items from customer orders.
Technical info: display field, DB field: kauf.kunr, mp.name

**Warehouse** Number and description of warehouse for stock articles.
Technical info: numeric field, display field, DB fields: kauf.hausnr

**Project** Number and description of the project for purchase order items from customer orders.
Technical info: numeric field, display field, DB fields: bpos.vkobjnr, mp.name

**Price/Pc.** Item price of the purchase order item.
Technical info: numerical field, DB field: kpos.nstpreis

**Item price** Total price of the purchase order item. The total price is calculated from piece price x quantity of the article.
Technical info: numeric field, DB field: kpos.npospreis

#### Footer

**OK**
Closes the current view and changes to the Purchase order release – Selection view.
⇨ "Purchase order release - selection" on page E-1631

**Cancel**
Closes the PO release dialog. Change will not be saved.

## Receipt of Goods

For deliveries, you can view the delivery plan for the purchase order and the supplier's delivery confirmation. You can advise of partial goods receipts and goods receipts and therefore check on-time goods receipt.

You can also complete the POs that should no longer be traced in the system.

The following information is available on this chapter:
*   "Dispatch notifications" on page E-1637
*   "Delivery plan" on page E-1646
*   "Receipt of goods (automatic)" on page E-1649
*   "Item info" on page E-1652
*   "Booking racks" on page E-1652
*   "Receipt of goods (manual)" on page E-1654
*   "Rack-related receipt of goods" on page E-1656
*   "Booking racks" on page E-1652
*   "Check receipt of goods" on page E-1660
*   "Missing quantities check pool" on page E-1661
*   "Receipt of goods log" on page E-1663

### Dispatch notifications

**Path:** `Purchase > Notifications`

The delivery confirmations from suppliers are managed in this dialog.
This dialog contains the following tabs and views:
*   "Notifications – overview" on page E-1638
*   "Notifications – details" on page E-1640
*   "Purchase order – overview (notification)" on page E-1642
*   "Purchase order – details (notification)" on page E-1643

#### Notifications – overview

**Path:** `Purchase > Notifications - Overview Tab`

*Fig. E-34 Notifications - overview tab*

Use this tab to enter notifications concerning receipt of goods.
*   Use `<F2>` to change to the Notification - Details tab.
    ⇨ "Notifications - details" on page E-1640
*   Use `<F5>` in the OC-No. Supplier field in the body to open the PO dialog in order to get detailed information about the items ordered.
    ⇨ "Purchase order – overview (notification)" on page E-1642

##### Header

**OC no. supplier OC Supplier:** Number of order confirmation from supplier. If you enter an order confirmation number that also includes letters, you must enter them in a case-sensitive manner.
Technical info: alpha-numerical field, DB field: bpos.abnr

**Delivery date** Planned delivery date. You can take over the delivery date for all POs. If you take over the date for all POs, the delivery date of each PO in the body is overwritten by the delivery date in the header area.
Technical info: mandatory field, date field, DB field: bpos.ltplan

**Site** Site number from the purchase order.
Technical info: display field, DB field: kauf.hausnr

**Supplier** Supplier number. If you specify a number, the name of the supplier is displayed in plain text. You can take over the supplier for all POs. If you take over the supplier for all POs, you can only select POs for this supplier for the order confirmation.
Technical info: numeric field, display field, DB field: kauf.kunr

##### Body

*   **P.O.:** Purchase order number. If you have specified a supplier, you can only specify POs for this supplier.
    Technical info: numeric field, DB field: kauf.auftrnr
*   **OC no.suppl.:** Number of order confirmation from supplier.
    Technical info: alpha-numerical field, DB field: bpos.abnr

Use `<F5>` to edit the Overview and Details of the notifications in the Supplier OC no. column.
⇨ "Purchase order – overview (notification)" on page E-1642
⇨ "Purchase order - details (notification)" on page E-1643
*   **Ordered for:** Date when the purchase order should be received. Usually the delivery date of receipt of goods or in the case of direct delivery, e.g. a construction site.
    Technical info: date field, DB field: kauf.ltplan
*   **Number:** Supplier number from purchase order.
    Technical info: display field, DB field: kauf.kunr
*   **Supplier:** Name of the supplier.
    Technical info: display field, DB field: mp.name
*   **Qty:** Quantity of the item that is delivered.
    Technical info: display field, DB field: bpos.avismenge

#### Notifications – details

**Path:** `Purchase > Notifications - Details Tab`

*Fig. E-35 Notifications - details tab*

On this tab you can view the purchase order details. You can enter changes based on the supplier confirmation.
*   Use `<F2>` to change to the Notification - Overview tab.
    ⇨ "Notifications – overview" on page E-1638
*   Use `<F5>` in field OC No. Suppl. to open the Purchase Order dialog.
    ⇨ "Purchase order – overview (notification)" on page E-1642
*   With `<Ctrl> + <L>` you can, if this possibility is configured, check the delivery address. However, the delivery address cannot be changed here.

##### Header
The header fields are described for the Notification - Overview tab:
⇨ "Notifications - overview" on page E-1638

##### Purchase information

**P.O. no.** Purchase order number.
Technical info: numeric field, DB field: kauf.auftrnr

**OC no. suppl.** Number of order confirmation from supplier.
Technical info: alpha-numerical field, DB field: bpos.abnr

**Supplier** Number and name of the supplier.
Technical info: display fields, DB fields: kauf.kunr

**Street, PCd, City** Supplier's address. The fields are pre-populated with the values from the purchase order.
Technical info: numerical field, alpha-numerical field, DB fields: kauf.orgstr, kauf.orgplz, kauf.orgort

**VAT code** ID, description and percentage of the VAT code. The percentage and the ID are determined using the number from the master data.
Technical info: display fields, DB fields: kauf.kukz

**Deliv. date** Actual delivery date of the purchase order.
Technical info: date field, DB field: kauf.ltplan

**Old** Old, planned delivery date of the purchase order.
Technical info: display field, DB field: bpos.ltplan

**Route** Number and description of the route. If you specify a number, the description of the route is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.routenr

**Net amount** Total of all item prices, including all discounts and surcharges.
Technical info: display field, DB field: kauf.nettototal

**VAT amount** Value-added tax amount of the purchase order.
Technical info: display field, DB field: kauf.mwstbetrag

**Gross amount** Gross amount of the purchase order including VAT.
Technical info: display field, DB field: kauf.gesbrutto

##### Order information
The fields are only pre-populated, if the purchase order was created from a customer order.

**Order no.** Order number for order-related purchase orders.
Technical info: display field, DB field: kauf.auftrnr

**Customer name** Customer name from the customer order.
Technical info: display field, DB field: kauf.kunr

**Delivery date** Planned delivery date of the customer order.
Technical info: display field, DB field: kauf.ltplan

**Route** Number and name of the delivery route to the customer.
Technical info: display fields, DB fields: kauf.routenr

#### Purchase order – overview (notification)

**Path:** `Purchase > Notification > Overview Tab > Column OC No. Suppl. > <F5>`
**Path:** `Purchase > Notification > Details Tab > OC No. Suppl. Field > <F5>`

*Fig. E-36 Purchase order - Overview (notification)*

Use this tab to edit the item-accurate notifications, e.g. to change the announced delivery quantity. Changes to the deliveries and partial deliveries are recorded via the notifications.

Use `<F2>` to change to Purchase Order - Details (Notification) tab.
⇨ "Purchase order – details (notification)" on page E-1643

##### Overview
*   **Itm:** Item number.
    Technical info: display field, DB field: kpos.lfdpos
*   **Article:** Article number of the item.
    Technical info: numeric field, DB field: kpos.artnr
*   **Ordered:** Quantity of the ordered item.
    Technical info: numerical field, DB field: kpos.menge
*   **OC no. suppl.:** Number of order confirmation from supplier.
    Technical info: numerical field, DB field: bpos.abnr
*   **Confirmed:** Quantity of the delivery as confirmed by the supplier. In the case of boxes, this equals the total number of lites.
    Technical info: numeric fields, DB fields: bpos.avismenge
*   **Price/Pc.:** Net price per piece of item.
    Technical info: numeric field, DB field: kpos.nstpreis
*   **Item price:** Net total price of item.
    Technical info: numeric field, DB field: kpos.npospreis
*   **Invoic.:** Invoice ID of the item. The column indicates whether the selected item has already been invoiced.
    Technical info: display field, DB field: kpos.fakturakz

#### Purchase order – details (notification)

**Path:** `Purchase > Notifications > Overview Tab > Suppl. OC No. Column > <F5> Details Tab`
**Path:** `Purchase > Notifications > Details Tab > Suppl. OC no. Column > <F5> Details Tab`

*Fig. E-37 Purchase order (notification) – details tab*

Use this tab to enter details for the delivery that has been announced by the supplier, e.g. quantity, price and delivery date. Changes to the deliveries and partial deliveries are recorded via the notifications.

Use `<F2>` to change to the Purchase Order - Overview (Notification) tab.
⇨ "Purchase order - overview (notification)" on page E-1642

**Article** Number and description of the article. If an article number is specified, the corresponding description is displayed in plain text.
Technical info: numerical field, display field, DB field: kpos.artnr, kpos.artbez1

**Note** Additional information on the item.
Technical info: alpha-numerical field, DB field: bpos.bemerkung

**Cost center** Cost center name for statistical evaluations.
Technical info: numerical field, DB field: kpos.kostenst

**Account** Description of the cost center booking account.
Technical info: alpha-numerical field, DB field: kpos.konto

**Shape** Shape number for PO items with lite shape.
Technical info: display field, DB field: kpos.modnr

**Ordered** Quantity of the ordered item.
Technical info: numerical field, DB field: kpos.menge

**Delivered** Number of delivered items.
Technical info: display field, DB field: kpos.geliefert

**Width, Height** Dimensions of the item in millimeters.
Technical info: display fields: DB fields: kpos.laenge, kpos.breite

> **One-dimensional quantity input**
> For a system configuration, in incoming goods for articles with quantity units (1,6,7,8,10), a partial quantity with regard to this quantity unit can also be reported. The field for input of the quantity kpos.laenge (e.g. a linear meter or liter specification) can be changed accordingly.

**AIR** Airspace in millimeters. The field is only preset for IG articles.
Technical info: display field, DB field: kpos.szr

**sqm piece** Surface in square meters per piece.
Technical info: numeric field, DB field: kpos.qm

**OC no.supplier** Number of order confirmation from supplier.
Technical info: alpha-numerical field, DB field: bpos.abnr

**Delivery date** Actual delivery date of the purchase item.
Technical info: Date field, DB field: bpos.ltavis

**Confirmed** Quantity of delivery as confirmed by the supplier. In the case of boxes, this equals the total number of sheets.
Technical info: numeric fields, DB fields: bpos.avismenge

**Old** Old, planned delivery date of the purchase order.
Technical info: display field, DB field: bpos.ltplan

**Order** Order number for order-related purchase orders.
Technical info: display field, DB field: kauf.auftrnr

**Item** Number of the item, in the case of order-related purchase orders.
Technical info: display field, DB field: kpos.lfdpos

**Reject reason** The number and the reject description are displayed.
Technical info: display field, DB field: bpos.bruch

**Deliv. date** Date of delivery at the customer.
Technical info: display field

**Cst. project** Project number and name of the customer order for order-related purchase orders.
Technical info: display fields, DB fields: bpos.vkobjnr.

**Stock number** Number and name of warehouse for stock articles.
Technical info: display fields, DB fields: bpos.lnr

**Sup.art.no.** Supplier's article number and ID of the supplier article. Number and ID are displayed if a supplier-specific article number is stored for the article in the master data.
Technical info: numerical field, alpha-numerical field, DB fields: bpos.exartnr, bpos.bestellbez

**Price/QU** Price per quantity unit. The price is calculated from the glass price plus the surcharge.
Technical info: numeric field, DB field: kpos.bmepreis

**Net pieces** Net price per piece.
Technical info: numerical field, DB field: kpos.nstpreis

**Item price** Net purchase price per piece.
Technical info: numeric field, DB field: kpos.npospreis

### Delivery plan

**Path:** `Purchasing > Receipt of Goods > Delivery Plan`

*Fig. E-38 Delivery plan – overview tab*

You can plan the planned deliveries on this dialog. You can determine the delivery date and delivery quantity for individual or several POs. The partial deliveries will then be used to book goods receipt.

In order to be able to work with the delivery plan in purchasing, the system must be configured appropriately.

Use `<F2>` to change to the Delivery Plan - Details tab.
⇨ "Delivery plan – details" on page E-1648

Use `<Ctrl> + <G>` to change to the Booking Racks dialog.
⇨ "Booking racks" on page E-1652

Use `<OK>` to save the delivery plan and to exit the dialog.

**Site** Site number. The field is only enabled for multi-site systems.
Technical info: display field, DB field: kauf.hausnr

**P.O.** Specification of the PO number for which the delivery plan should be created or changed.
Technical info: display field, DB field: kauf.vorgang=2

**Supplier** Displays the name of the supplier from the purchase order. The field is disabled.
Technical info: display field, DB field: kauf.kunr, mp.name

#### Overview
The Overview tab displays the following fields:
*   **Itm:** Item number.
    Technical info: display field, DB field: liefplan.lfdpos
*   **Deliv.:** Number of the delivery. The value is incremented for partial deliveries.
    Technical info: display field, DB field: liefplan.subnr
*   **Delivery date:** Delivery date for the scheduled product.
    Technical info: display field, DB field: liefplan.ltplan
*   **Article:** Article name from the purchase order.
    Technical info: display field
*   **OC no.suppl.:** Order confirmation of supplier.
    Technical item: numeric field, DB field: liefplan.abnr
*   **Total:** Total quantity of the item ordered from the PO in article quantity unit, e.g. pieces.
    Technical info: display field, DB field: liefplan.geslief
*   **Shipped:** Already shipped quantity for the ordered item in article quantity units, e.g. pieces.
    Technical info: display field, DB field: liefplan.geliefert
*   **Packed:** Already packed quantity for the ordered item in article quantity units. e.g. pieces.
    Technical info: display field, DB field: liefplan.gespack
*   **Planned:** Planned quantity for the item ordered in article quantity units that should arrive in this (partial) delivery, e.g. pieces.
    Technical info: display field, DB field: liefplan.zuliefern

### Delivery plan – details

**Path:** `Purchase > Receipt of Goods > Delivery Plan > Select Purchase Order > <F2>`

*Fig. E-39 Delivery plan – details tab*

This tab shows detailed information for the selected purchase order item.
Use `<F2>` to change to the Delivery Plan - Overview tab.
⇨ "Delivery plan" on page E-1646

Use `<Ctrl> + <G>` to change to the Booking Racks dialog.
⇨ "Booking racks" on page E-1652

Use `<OK>` to save the delivery plan and to exit the dialog.

#### Details
The fields are described on the Deliver Plan - Overview tab. In addition, the following fields are displayed on the Details tab:

**Stock** Stock number of the standard stock for stock POs. The designation of the standard stock is determined from the master data and displayed in the second field.
Technical info: display field, DB field: liefplan.lnr

**Stack** Stock number of the stack stock for stock POs insofar as the article is kept in the stack stock. The designation of the stack is determined from the master data and displayed in the second field.
Technical info: display field, DB field: liefplan.stapel, liefplan.stapelbez

**Box** Box number of the box stock for stock POs, insofar as the article is kept in the box stock.
Technical info: display field, DB field: liefplan.kistenr

**Slot** Slot designation of the slot stock for stock POs, insofar as the article is keeps in the slot stock.
Technical info: display field, DB field: liefplan.fach

### Receipt of goods (automatic)

**Path:** `Purchasing > Receipt of Goods > Automatic Receipt of Goods`

*Fig. E-40 Receipt of goods (automatic)*

Use this dialog to book received deliveries as receipt of goods. You can book individual or all loaded purchase orders of the dialog.
*   With `<Value import>` the POs in the system are uploaded to the dialog. The value import can be configured customer-specifically.
*   Use `<F9>` to select individual purchase orders that have not been booked.
*   Use `<F8>` to select purchase orders for which a delivery plan exist, that have not been booked.
*   Use `<Ctrl>+<L>` to change to the Delivery note column, where you can specify the external supplier delivery note designation.
*   Use `<F5>` to open the Item Info dialog.
    ⇨ Purchasing, “Item info” on page E-1652
*   Use `<F3>` to book the previously marked PO as goods receipt.

#### Purchase orders
The Purchase Orders tab shows the following columns:
*   **Ρ.Ο.:** Purchase order number.
    Technical info: numeric field, DB field: kauf.auftrnr
*   **1. Column without a name (subnumber):** POs without a delivery plan are booked as complete goods receipt, so this field remains empty. For POs with a delivery plan, the subnumber from the delivery plan that is announced for the current date is displayed here. If there is a delivery plan for the PO, you can use `<F9>` to select the desired partial delivery.
    Technical info: display fields, DB fields: kauf.subnr
*   **2. Column without a name (delivery plan):** Display in plan text whether there is a delivery plan for the PO.
    Technical info: display field
*   **Site:** Site number of the PO.
    Technical info: display field, DB field: kauf.hausnr
*   **Receipt:** Indication whether a goods receipt for the PO has already been received. If the goods receipt was already booked, this is indicated in the Exists column.
    Technical info: display field
*   **Invoice:** Number of the supplier's invoice if the PO has already been (partially) invoiced.
    Technical info: display field, DB field: kauf.auftrnr
*   **External no.:** Order number from purchasing if the PO was entered with reference. Display Collective PO or Stock PO
    Technical info: display field, DB field: kauf.exaufnr
*   **Date:** Date of entry for the purchase order.
    Technical info: date field, DB field: kauf.bdat
*   **Deliv. note:** Text field for the delivery note designation. Use `<Ctro> + <L>` to switch from any column to the delivery note column and enter a designation for the supplier delivery note.
    Technical info: alphanumeric field, DB field: bpos.lieferschein
*   **Chk:** Check. Checkbox whether the purchase order must be checked for completeness at receipt of goods. The function to check the receipt of goods is customer-specific.
    - The purchase order is checked at receipt of goods.
    - The purchase order is not checked.
    Use `<F4>` to set the control status for individual items starting with a particular one or all items:
    ⇨ "Receipt of goods supplementary menu" on page E-1551
    Technical info: checkbox, DB field: kauf.kontrolle
*   **Cr.:** Create. Specification whether the purchase order should be booked in receipt of goods.
    - The purchase order is booked in receipt of goods.
    - The purchase order is not booked.
    Use `<F3>` to book all selected purchase orders.
    Technical info: Checkbox

#### Footer
On the Purchase Orders tab, the name of the supplier and net amount for the marked PO are displayed.

**Items**
Opens the Item Info dialog for the marked purchase order.

**Value Import**
After specifying a time period, imports all non-booked POs with a delivery date within the specified time period.

**Create**
Books all marked POs in receipt of goods and closes the dialog.

**Cancel**
Closes the dialog without saving the purchase orders.

### Item info

**Path:** `Purchasing > Receipt of Goods > Automatic Receipt of Goods > Search for Purchase Order > <F5>`
**Path:** `Purchasing > Receipt of Goods > Complete Purchase Orders > Find Purchase Order > <F5>`

*Fig. E-41 Item overviews*

This dialog allows you to view the item overview for a purchase order. Use `<F2>` to go to the tab.

The Item Info tab is described in detail in the Sales section:
⇨ Sales, "Item info" on page D-1400

### Booking racks

**Path:** `Purchase > Automatic Receipt of Goods > Select Purchase Order > <F4> > Rack Management`

*Fig. E-42 Booking racks*

On this dialog, you can assign the lites of a PO to the rack per item.

#### Header
**Docum.** Purchase order number for which the rack is booked.
Technical info: display field, DB field: kauf.auftrnr, bcbock.auftrnr

#### Body
*   **Itm:** Number of the item on the delivered rack.
    Technical info: display field, DB field: bcbock.bposnr
*   **Quantity:** Number of lites in the item.
    Technical info: display field, DB field: bcbock.anzahl
*   **Rack, designation:** Number and designation of the rack type of the rack delivered. If you specify a number, the designation of the rack is displayed in plain text.
    Technical info: numeric field, display field, DB fields: bcbock.gnr, gest.exgnr

Use `<F2>` to display the following columns:
*   **Move:** Rack number of the delivered rack, the glass pieces of which are booked to a different rack.
    Technical info: display field, DB field: bcbock.gnr, gest.exgnr
*   **Quantity:** Quantity of glass pieces that are booked to the target rack.
    Technical info: numerical field, DB field: bcbock.anzahl
*   **Target rack:** Rack number of the target rack to which the glass is booked.
    Technical info: numeric field, DB field: bcbock.gnr, gest.exgnr

### Receipt of goods (manual)

**Path:** `Purchase > Manual Receipt of Goods > Find Purchase Order`

*Fig. E-43 Manual receipt of goods*

Use this dialog to edit and book received deliveries and partial deliveries that arrived in receipt of goods.
Use `[End]` to save your entries and to book the (partial) receipt of goods.

> **Close purchase orders in the event of partial deliveries**
> If you book a partial good receipt, you will be asked whether there will be additional goods receipt to follow. With [Yes,] only the partial goods receipt will be created and booked; the PO will not be completed. With [No], the partial goods receipt will be created and booked and the PO will be completed. Additional partial goods receipts can no longer be booked for the selected PO.

The dialog is structured the same as the Purchase Order Entry dialog.
⇨ "Purchase order entry" on page E-1584
Differences will be described explicitly below.

#### Header
**Purchase** Purchase order number and partial delivery number. For each new purchase order, the partial delivery number 1 is automatically specified. In the case of partial deliveries, you must manually enter consecutive numbers larger than 1, e.g. the partial delivery number 2 for the second partial delivery.
Technical info: mandatory field, numeric fields, DB fields: kauf.auftrnr, kauf.subnr

**Delivery note** Supplier's delivery note number.
Technical info: alpha-numerical field, DB field: kauf.lieferschein

**Check** Indication as to whether the purchase order should be checked for completeness at receipt of goods.
*   **Control:** The PO is checked in goods receipt, e.g. for completeness. The employee number and date for the check are logged.
*   **(No specification):** The PO will not be checked.
Technical info: toggle field, DB field: kauf.kontrolle

#### General tab
*   **Ordered:** Ordered item quantity in the article quantity unit.
    Technical info: numeric field, DB field: kpos.menge
*   **Alr. recei.:** Item quantity already received in the article quantity unit.
    Technical info: numeric field
*   **Received:** Already delivered item quantity in the article quantity unit. The system calculates the quantity from ordered quantity less the quantity already received.
    Technical info: numeric field, DB field: kpos.geliefert
*   **Confirm:** Supplier-side confirmed item quantity in the article quantity unit of the delivery.
    Technical info: numeric field, DB field: bpos.avismenge

### Rack-related receipt of goods

**Path:** `Purchase > Receipt of Goods > Rack-Related Receipt of Goods`

On this dialog, you enter and edit goods receipts using the rack.
There are the following views for this dialog:
*   "Rack-related receipt of goods" on page E-1656
*   "Rack load" on page E-1658

#### Rack-related receipt of goods

**Path:** `Purchase > Receipt of Goods > Rack-Related Receipt of Goods`

*Fig. E-44 Rack-related receipt of goods*

Rack-related receipt of goods are booked on this dialog.
*   Use `<F6>` to open the Rack Load dialog and create a new rack load and place the PO items on another (new) rack.
*   Use `<F5>` to open the Rack Load dialog, where you can edit the marked goods receipt.
    ⇨ "Rack load" on page E-1658

##### Overview
*   **Rack:** Rack number
    Technical info: display field, DB field: waeingestkopf.exgnr
*   **Suppl. ID:** Manually-entered ID for a delivery.
    Technical info: display field, DB field: waeingestkopf.lieferid
*   **Storage location:** Number and name of the storage location where the rack is located.
    Technical info: display field, DB field: waeingestkopf.lagerplatz
*   **Truck:** License plate number of the truck with which the PO was delivered.
    Technical info: display field, DB field: waeingestkopf.lkwkennzeichen
*   **Supplier:** Number and name of the supplier.
    Technical info: display field, DB field: kauf.kunr, mp.name
*   **Qty:** The total quantity of all lites on the rack. This quantity is calculated from all items on the rack.
    Technical info: display field, DB field: waeingestpos.menge
*   **Deliv. Date, Time:** Date and time of the delivery.
    Technical info: display field, DB field: waeingestkopf.datum. waeingst-kopf.zeit
*   **Bo.:** Specification whether the rack should be booked in goods receipt.
    - The rack is booked in goods receipt.
    - The rack is not booked.
    Use `<F3>` to start the booking of the rack.
    Technical info: checkbox, DB field: waeingestkopf.gebucht

##### Footer
**New**
Opens the Rack Load dialog where you can enter a new rack in goods receipt.
⇨ "Rack load" on page E-1658

**Correction**
Opens the Rack Load dialog where you can edit the selected rack in goods receipt.
⇨ "Rack load" on page E-1658

**Delete**
Deletes the selected rack.

**Booking**
Books the marked rack in goods receipt.

**OK**
Books the marked rack in goods receipt and closes the dialog.

**Cancel**
Closes the dialog without booking the rack.

### Rack load

**Path:** `Purchase > Receipt of Goods > Rack-Related Receipt of Goods > [New], [Correction]`

*Fig. E-45 Rack load*

In this view, you enter and edit the rack load for the goods receipt.

#### Header
You can only edit the fields in the header area if you are entering a new rack load. If you are editing an existing rack load, the header area is locked.

**Rack (no./name)** Rack number and name.
Technical info: mandatory field, numeric and alphanumeric field, DB field: waeingestkopf.gestellnr, waeingestkopf.exgnr

**Suppl.ID** Manually entered flag for a delivery.
Technical info: display field, DB field: waeingestkopf.lieferid

**Storage location** Number and designation of the storage location for the rack. If you select a number, the designation is displayed in plain text.
Technical info: mandatory field, numeric field, alphanumeric field, DB field: adr.str

**Truck plate no.** License plate number of the truck with which the rack was delivered.
Technical info: alphanumeric field, DB field: waeingestkopf.lkwkennzeichen

**Total qty.** Total quantity on all racks of the delivery. The total quantity corresponds to the total of all quantities in the Quantity column in the overview.
Technical info: display field, DB field: waeingestpos.menge

**Date** Date of delivery in the format DD.MM.YYYY.
Technical info: date field, DB field: waeingestkopf.datum

**Time** Time of delivery in the format hh:mm.
Technical info: alphanumeric field, DB field: waeingstkopf.mc

#### Body
All PO items for which goods receipt should be booked to the rack are entered and edited in the dialog body.
*   **P.O.:** Purchase order number.
    Technical info: mandatory field, numeric field, DB field: waeingestpos.auftrnr
*   **ItmNo** Item number in the purchase order.
    Technical info: mandatory field, numeric field, DB field: waeingestpos.pos-nr
*   **Supplier:** Name and number of the supplier. If you enter a purchase order number, the fields are pre-populated by the system.
    Technical info: display fields, DB fields: waeingestpos.mpnr
*   **Deliv.note:** Delivery note description of the supplier.
    Technical info: alpha-numerical field, DB field: waeingestpos.lieferschein
*   **Total:** Total quantity of the selected item.
    Technical info: display field, DB field: waeingestpos.menge
*   **Included:** Already delivered quantity of the ordered item from a partial delivery.
    Technical info: display field
*   **Qty:** Currently delivered quantity of the ordered item.
    Technical info: numeric field, DB field: waeingestpos.menge
*   **Miss. qty.:** Difference between ordered and delivered quantity.
    Technical info: numeric field, DB field: waeingestpos.fehlmenge
*   **Side:** Rack side on which the item is located:
    - 0 = not specified
    - 1 = left
    - 2 = right
    Technical info: alphanumeric field, DB field: waeingestpos.gestellseite
*   **Sequence:** The sequence in which the item is on the rack, from outside to inside.
    Technical info: numeric field, DB field: waeingestpos.reihenfolge

### Check receipt of goods

**Path:** `Purchase > Receipt of Goods > Check Receipt of Goods`

*Fig. E-46 Check receipt of goods*

On this dialog, goods receipts and purchase invoices are created automatically based on the underlying PO and an invoice received. The data is sent and received via the data transfer and it can be checked and adjusted on the Check goods received dialog.

This for-fee function must be configured explicitly. If you have questions, please contact an A+W Software GmbH service employee.

### Missing quantities check pool

**Menu:** `Purchase > Receipt of Goods > Missing Qty. Check Pool`

This dialog shows a list of items the quantity of which has been corrected.
This for-fee function must be configured explicitly. If you have questions, please contact an A+W Software GmbH service employee.

This dialog offers the following tabs:
*   "Missing quantities check pool - overview" on page E-1661
*   "Missing quantities check pool – details" on page E-1662

#### Missing quantities check pool - overview

**Path:** `Purchase > Receipt of Goods > Missing Quantity Check Pool > Overview Tab`

*Fig. E-47 Missing quantities check pool - overview*

This tab shows a list of items the quantity of which has been corrected. The data is transferred via openTrans interface.
This function description is not part of the manual and must be requested if needed.

#### Missing quantities check pool – details

**Path:** `Purchase > Receipt of Goods > Missing Quantities Check Pool > Details Tab`

*Fig. E-48 Missing quantities check pool - details*

This tab provides you with detailed information about the selected item.
This function description is not part of the manual and must be requested if needed.

### Receipt of goods log

**Path:** `Purchase > Receipt of Goods > Log`

*Fig. E-49 Receipt of goods log*

On this dialog, you can display a log about the creation and booking of goods receipts for the current day. All documents for goods receipt are logged with the specification of the date and time.

## Invoices and Credit Notes

Invoices for purchase orders are entered and booked in the program. Depending on the configuration, the internal invoice is automatically sent by the program to Financial Accounting (FinAcc).

The following information is available on this chapter:
*   "Invoice check" on page E-1664
*   "Supplier's invoice (automatic)" on page E-1671
*   "Transferred invoices" on page E-1673
*   "Supplier's invoice (manual)" on page E-1674
*   "Supplier's invoice (collective invoice)" on page E-1675
*   "Booking of invoices" on page E-1676
*   "Close purchase orders" on page E-1677
*   "Invoice log" on page E-1678
*   "Supplier's credit note" on page E-1678

The dialog Book Credit Notes is described in detail in the Sales section.
⇨ Sales, "Book credit notes" on page D-1416

### Invoice check

**Path:** `Purchase > Invoices > Invoice Check`

Use this dialog to enter and check supplier invoices, and to create and book internal invoices. The use of the invoice check in purchasing requires configuration by A+W Software GmbH.

There are the following views for this dialog:
*   "Supplier's Invoice - Purchase Overview" on page E-1665
*   "Supplier's invoice - detailed view" on page E-1668
*   "Supplier's invoice – item overview" on page E-1669
*   "Supplier's invoice - discounts" on page E-1670

#### Supplier's Invoice – Purchase Overview

**Path:** `Purchase > Invoices > Invoice Check`

*Fig. E-50 Supplier's invoice - purchase overview*

On this dialog, you enter the PO data for checking. Then you can create and book the supplier invoice for the PO checked.
*   Use `<F2>` to change to the body in the detail view.
    ⇨ "Supplier's invoice - detailed view" on page E-1668
*   Use `<F5>` in the Net amount field to change to the item detail overview.
    ⇨ "Supplier's invoice - item overview" on page E-1669
*   Use `<Ctrl>+<A>` to change to the discount overview.
    ⇨ "Supplier's invoice - discounts" on page E-1670

Use `<Enter>` to change from the body area to the footer area. With the manual entry of the invoice total, the invoice is checked in the system. You can create the invoice and book it right away or later on.
⇨ "Booking of invoices" on page E-1676

##### Header
**Document no.** Internal document number of the supplier invoice. You can specify any number (designation). If you specify a document number or select one with `<F9>` for which an invoice has already been created, you can check and if necessary edit this invoice.
Technical info: alphanumeric field, DB field: kauf.exauftrnr

**Intern (invoice/credit note)** Specification whether an invoice or a credit note was already created. If you have selected a document number for which one of these document types was already created, the associated number and document type (invoice/credit note) is displayed. The possibility of editing the credit notes via the invoice checking requires separate configuration on the part of A+W Software GmbH.
Technical info: kauf.auftrnr, kauf.vorgang

**Doc. date** Date on which the supplier invoice is entered.
Technical info: mandatory field, date field, DB field: kauf.edat

**Booking date** Date on which the supplier invoice is booked. The booking date is pre-populated by the system with the document date.
Technical info: mandatory field, date field, DB field: kauf.bdat

**Site** Site number. The field is only enabled if the internal client separation is active.
Technical info: numeric field, DB field: kauf.hausnr

**Supplier** Supplier number. If you specify a number, the name of the supplier is displayed in plain text. If you have specified a supplier, you can only select POs for this supplier in the PO overview. If you do not select a supplier, the field is pre-populated automatically with the supplier from the first PO.
Technical info: numeric field, DB field: kauf.kunr

##### Purchase order overview
*   **PO number:** Purchase order number on the supplier invoice.Use `<F5>` to change to the External No. field where you can specify the PO via the external number.Use `<Ctrl>+<L>` to change to the Deliv. Note field where you can specify the PO via the delivery note number.
    Technical info: mandatory field, alphanumeric field, DB field: kauf.auftrnr
*   **Reference doc.:** Reference document for which the internal invoice is created and booked.
    - **Goods received:** The supplier invoice refers to a goods receipt. The delivery is booked for receipt of goods.
    - **PO:** The supplier invoice refers to a PO without goods receipt. The delivery is not booked in goods receipt.
    Technical info: toggle field, DB field: kaufp.refvorgang
*   **SubNo.:** Subnumber for partial deliveries of the goods receipt. For complete deliveries, the subnumber 1 is displayed.
    Technical info: numeric field, DB field: kaufp.refsubnr
*   **Net amount:** Net amount of the supplier invoice from the PO. You can edit the amount. Depending on the configuration, only a particular deviation is permitted. If the amount entered deviates from the net amount from the PO, a message is displayed whether the total difference is acceptable.
    Technical info: numeric field, DB field: kauf.nettototal
*   **External no.:** External number that was entered on the Receipt of goods dialog, e.g. order number from sales if the PO was entered with reference.
    Technical info: numeric field, DB field: kauf.exaufnr
*   **Delivery note:** Supplier OC number that was entered on the Dispatch notification dialog.
    Technical info: numeric field, DB field: kauf.lieferschein

##### Footer
**Total amount net** Total net amount of the supplier invoice that you have to enter into the system. The system checks the invoice data by comparing the total net amount of the POs and the total net amount. The result of the invoice checking is displayed in a message:
*   **"Total amount is correct.":** The total of the invoice amounts from the Net amount matches the Total net amount. The internal invoice is created with [Yes]. In another message, you can book the invoice.
*   **"The total amount is not correct.":** The total of the invoice amounts from the Net amount column does not match the Total amount. The difference of the values is displayed as amount and percentage. In the rules, it is not possible to ignore the invoice difference. In exceptional cases, the system can be configured so that only an authorized employee may ignore the difference and create the invoice.
Technical info: numerical field, DB field: kauf.nettototal

**VAT amount** VAT amount of the POs. If you create the invoice, the field will be pre-populated by the system. You can edit the amount. Depending on the configuration, only a particular deviation is permitted. If the amount entered deviates from the VAT amount from the POs, a message is displayed. If several VAT rates are specified for a PO, the individual VAT rates are displayed. This is important for countries where different tax rates are used. The fields are only displayed if the multi-VAT module is active.
Technical info: numeric fields, DB fields: kauf.mwstbetrag1, kauf.mwstbetrag2, kauf.mwstbetrag3, kauf.mwstbetrag4

**Total amount gross** Total gross amount of the POs. The system calculate the gross amount from the total of Total net amount and VAT amount.
Technical info: numerical field, database field: kauf.gesbrutto

**Total qty** Total number of pieces of units from all purchase orders.
Technical info: display field

**Total sqft** Total area of the articles from the POs in square meters.
Technical info: display field

**Total ser.mtr.** Total length of the articles from the POs in linear meters.
Technical info: display field

#### Supplier's invoice – detailed view

**Path:** `Purchase > Invoices > Invoice Check > Find Purchase Order > <F2>`

*Fig. E-51 Supplier's invoice detailed view*

The supplier data and supplier details for the selected PO are displayed in these views.

##### Header
The header area is described for the Supplier invoice - PO overview dialog; the fields on the tabs are described in detail for the Purchase Order Entry dialog:
⇨ "Supplier's Invoice - Purchase Overview" on page E-1665
⇨ "Purchase order entry" on page E-1584

#### Supplier's invoice – item overview

**Path:** `Purchase > Invoices > Invoice Check > Net Amount Field > <F5>`

*Fig. E-52 Supplier's invoice – item overview*

In these views, the item details for the selected PO are displayed.
Use `<F2>` to change between the tabs.

The following information is displayed in plain text next to the tabs:
*   **Ρ.Ο.:** Purchase order number.
*   **(Invoice type):** Specification whether a total or partial invoice is created.
    - **Partial invoice:** A partial invoice is created for the PO.
    - **Total invoice:** A total invoice is created for the PO.

In the upper right part of the tab, the total number of items in the PO and the currently selected PO items are displayed. For example, 1 of 3 means that the currently the first item of a total of three items in the PO is selected.

##### Header
The header area is described for the Supplier's Invoice - PO Overview dialog:
⇨ "Supplier's Invoice - Purchase Overview" on page E-1665

##### Items, details tab
Use `<F2>` to change between Items and Details. The fields are described in detail with the Purchase order entry – items dialog.
⇨ "Purchase order items - general" on page E-1604

#### Supplier's invoice – discounts

**Path:** `Purchase > Invoices > Invoice Check > Net Amount Field > <Ctrl> + <A>`

*Fig. E-53 Supplier's invoice - discounts*

Use this dialog to enter and check supplier invoices, and to create and book internal invoices.

Use `<Enter>` to complete the invoice control, create and book the invoice. If you create or book an invoice, an internal invoice number will be shown. Alternatively, you can book an internal invoice subsequently.
⇨ "Booking of invoices" on page E-1676

Afterwards, the booking data for FinAcc is generated.

##### Header
The header area is described for the Supplier's Invoice - PO Overview dialog:
⇨ "Supplier's Invoice - Purchase Overview" on page E-1665

The body area is described for the Purchase Order Entry - Discounts dialog:
⇨ "Purchase order entry - discounts detailed view" on page E-1602

### Supplier's invoice (automatic)

**Path:** `Purchase > Invoices > Automatic Invoices`

*Fig. E-54 Supplier invoice (automatic)*

Use this dialog to create invoices for full deliveries. Book partial deliveries on the dialog Supplier invoice (manual) dialog. If there is already a delivery plan for a PO and part of the delivery is on the current day, the partial invoice for this delivery can also be created and booked on this dialog.

Use `<F3>` to then book the internal invoice. Alternatively, you can book the internal invoice later.
⇨ "Booking of invoices" on page E-1676

Afterwards, the booking data for FinAcc is generated.

#### Body
*   **P.O.:** Purchase order number.
*   **SubNo.:** Sub-number for deliveries. If this is a full delivery, a 1 is always shown. Partial numbers reflect the corresponding number of the partial delivery.
*   **Deliv.plan:** Specification whether the delivery plan exists.
*   **Receipt:** Delivery has already been booked as receipt of goods.
*   **Invoice:** Number of the supplier invoice.
*   **Doc. date:** Date when the supplier has created the invoice.
*   **Book. Date:** Date when the internal invoice was booked.
*   **Cre.:** Selection to create booking of the item.
    - Create booking.
    - Do not create booking.

#### Footer
Name of supplier and invoice amount of delivery.

### Transferred invoices

**Path:** `Purchase > Invoices > Booking Invoices > Transferred Invoices`

*Fig. E-55 Transferred invoices - overview*

On this tab, there is an overview of all invoices that were transferred via the open Trans interface. On the Details tab, you can see additional invoice fields for your information.

This function description is not part of the manual and must be requested if needed.

### Supplier's invoice (manual)

**Path:** `Purchase > Invoices > Manual Invoices`

*Fig. E-56 Supplier's invoice (manual)*

Use this dialog to edit and manually book internal invoices, e.g. if no prices are maintained in the system and, as a result, you cannot execute automatic invoice generation. Afterwards, the booking data for FinAcc is generated.

The fields, columns, and tabs are described with Purchase order entry dialog:
⇨ "Purchase order entry" on page E-1584

In addition, the following fields and columns are displayed:

#### Header
**Invoice no.** Invoice number of the supplier invoice.

#### General tab
**Invoice:** Quantity of the item that will be invoiced.

#### Footer
**Balance** Invoice amount including VAT.

### Supplier's invoice (collective invoice)

**Path:** `Purchase > Invoices > Collective Invoices`

*Fig. E-57 Supplier's invoice (collective invoice)*

On this dialog, you can create and book supplier invoices.

In order to create collective invoices, the purchase orders must meet certain prerequisites:
*   The supplier accepts the partial invoices. This setting is made in the master data.
*   For purchase orders, the option Collective invoice must be set in the Invoice type field.
    ⇨ "Purchase order items - properties" on page E-1613
*   The purchase orders must be booked in receipt of goods.
    ⇨ "Receipt of goods (automatic)" on page E-1649

Afterwards, the booking data for FinAcc can be generated.

The fields and the footer area are described for the Supplier's Invoice dialog:
⇨ "Supplier's invoice (automatic)" on page E-1671

### Booking of invoices

**Path:** `Purchase > Invoices > Booking of Invoices`

*Fig. E-58 Booking of invoices*

On this dialog, you can book already created but not yet booked invoices. Generally you book internal invoices on one of the following dialogs:
⇨ "Invoice check" on page E-1664
⇨ "Supplier's invoice (automatic)" on page E-1671
⇨ "Supplier's invoice (manual)" on page E-1674
⇨ "Supplier's invoice (collective invoice)" on page E-1675

Afterwards, the booking data for FinAc can be transferred.
The fields are described in Sales section.
⇨ Sales, "Booking of invoices" on page D-1405

### Close purchase orders

**Path:** `Purchase > Receipt of Goods > Close Purchase Orders`
**Path:** `Purchase > Invoices > Close Purchase Orders`

*Fig. E-59 Close purchase orders*

In this dialog, you can manually complete open purchase orders, e.g. if a purchase order has only been delivered partially and no further partial deliveries will follow.

Use `<F3>` to manually complete purchase orders.

> **Close purchase orders regularly**
> You can complete purchase orders regularly after receiving purchase orders from the supplier. You must book the purchase orders, using the two dialogs Receipt of goods and Supplier invoice so that the program can complete the purchase orders regularly.

The columns are described here:
⇨ "Receipt of goods (automatic)" on page E-1649

### Invoice log

**Path:** `Purchase > Invoices > Log`

*Fig. E-60 Invoice log*

This dialog displays the invoice log. All documents for the invoices are noted with specification of the date and time.

### Supplier's credit note

**Path:** `Purchase > Credit Notes > Enter Credit Notes`

*Fig. E-61 Supplier's credit note*

Use this dialog to enter and book credit notes that have been sent by suppliers.

The tabs and fields are described for the Purchase Order Entry dialog:
⇨ "Purchase order entry" on page E-1584
In addition, the following fields are displayed:

#### Header
**Number** Temporary number of the credit note. When saving, the final credit note number is assigned by the system at the end of entering credit notes.

**Ref.** Document number that is being referenced. You create credit notes by using a reference to a document. You must enter the following data in this order:
*   Type of reference document:
    - Purchase order.
    - Purchasing invoice.
    - Purchasing credit note.
*   Select supplier.
*   Select reference document for the supplier, e.g. purchasing invoice number.

#### Body
*   **Cred.note:** Quantity of the item that will be allocated for the credit note. However, it is possible to credit only the item number instead of the quantity.

## Overviews

There are several overviews available that allow you to check purchase order documents.
The following information is available on this chapter:
*   "Document information" on page E-1680
*   "Overview of documents" on page E-1681
*   "Purchase search" on page E-1682

### Document information

**Path:** `Purchase > Overview > P.O. Information > Open P.O.`
**Path:** `Purchase > P.O. Management > Open P.O. > Items Tab > General Tab > Quantity Column > <Shift> + <F10>`

*Fig. E-62 Purchase order information*

You can have document information displayed for all purchase orders, e.g. when the receipt of goods has been booked.

The dialog is described in detail in the Sales section.
⇨ Sales, "Order information" on page D-1428

### Overview of documents

**Path:** `Purchase > Overview > Receipt of Goods: Today, Receipt of Goods: Delayed, Receipt of Goods: From - To, Delivered - But not Invoiced, Invoiced - But not Booked, P.O.s not Transferred`

*Fig. E-63 Example for an overview dialog: Receipt of goods: from - to*

These dialogs display the overviews for the following documents:
*   Receipt of goods: today
*   Receipt of goods: delayed
*   Receipt of goods: from – to
*   Delivered - but not invoiced
*   Invoiced - but not booked
*   Purchase orders not transferred

These overview depend on the configuration and must be released separately. These dialogs can be designed customer-specifically if necessary. Please contact a service employee of A+W Software GmbH.

### Purchase search

**Path:** `Purchase > Search`

Use this dialog to search for documents. The results are displayed in a hit list.
This dialog contains the following tabs and views:
*   "Purchase search – search mode" on page E-1683
*   "Purchase search – overview" on page E-1684
*   "Purchase search – details" on page E-1686

#### Purchase search – search mode

**Path:** `Purchase > Search`

*Fig. E-64 Purchase search - search mode*

On this dialog, you enter the criteria for the document search. The results are displayed in the hit list.
Use `<F3>` to start the search.

**Site (order)** Site/client number of the orders for which the POs were created.
**Order** Order number.
**Customer** Customer number.
**Cust. route** Date of the route to the customer for direct delivery.
**Project number** Number of the project for which the goods have been ordered.
**Supplier** Supplier number.
**Site (P.O.)** Site or client number of purchase order.
**P.O.** Purchase order number.
**Ordered for** Date when the order should be received. Usually, receipt of goods or in the case of direct delivery, e.g. a construction site.
**Article** Article number.
**Complete** Code for filtering by the receipt status.
*   0 = List all purchase orders.
*   1 = List partially delivered purchase orders.
*   2 = List all completely delivered purchase orders.
**Cancel** Code for filtering by the cancellation status.
*   0 = List all purchase orders.
*   1 = List only purchase orders not canceled.
*   2 = List all canceled purchase orders.
**OC no. supplier** Number of order confirmation from supplier.
**Stock** Stock number for which the purchase order was entered.
**Input date** Date of the purchase order entry.
**Entered by** Employee who has entered the purchase order.
**Remark** Text for the item-related remark.
**External no.** Order number from Sales if the purchase order has been entered with a reference. Depending on the configuration, alternative data can be shown. The alternative data is described with the Purchase Order Entry dialog:
⇨ "Cust. order" on page E-1587
**Cost center** Cost center for which the purchase order was entered.
**Width, Height** Dimensions of the item in millimeters.

#### Purchase search – overview

**Path:** `Purchase > Search > Enter Filter Criteria > <F3>`

*Fig. E-65 Purchase search - overview*

This dialog displays the result of the search.
Switch to the Detail view using `<F5>`.

The following columns are displayed:
*   **Deliv. Date:** Date of delivery at receipt of goods or at the customer.
*   **Supplier:** Supplier number.
*   **P.O.:** Purchase order number.
*   **Itm:** Item number.
*   **Article:** Article number.
*   **Order:** Order number for which the purchase order was entered.
*   **Customer:** Customer number for which the purchase order was entered.
*   **Customer Route.:** Customer route. Date of the planned delivery of the order.
*   Display fields for the status of the purchase order:
    - Empty field = no status exists
    - C = Canceled.
    - Asterisk * = Fully delivered.
    - / = Completely invoiced.

#### Purchase search – details

**Path:** `Purchase > Search > Enter Filter Criteria > <F3> > Mark Entry > <F5>`

*Fig. E-66 Purchase search - details*

On this dialog, you can display details about an item on the hit list.
Use `<F2>` to return to the hit list.

The fields are described with the search mode and the hit list.
⇨ "Purchase search - search mode" on page E-1683
⇨ "Purchase search - overview" on page E-1684

In addition, the following fields are displayed:

**Reject reason** Reject reason in plain text, if it is present.
**Entry** Date of entry for order-related purchase order.
**Entered by** Employee name of the person who entered the order.
**Customer** Customer name and location.
**Route** Number and description of the delivery route.

---
# A+W Enterprise Stock

## Revision overview of the module

| Date | Change |
| :--- | :--- |
| 08-2023 | Update of software reference. |
| 01-2017 | Product and company names adjusted. |
| 12-2015 | Original version |

This module provides information on the following subjects:
⇨ Software Reference

## Overview

In the Stock module, you have all functions that are required for successful stock management, e.g. stock maintenance, stock bookings, inventories, as well as the planning of incoming and outgoing articles. All prices are specified as net prices in this module.

In the Stock part, you will find the following topics:
*   "Stock bookings" on page F-1700
*   "Master Data Management" on page F-1741
*   "Inventory Management" on page F-1746
*   "Evaluation" on page F-1758
*   "Information System" on page F-1765
*   "Print" on page F-1811
*   "System Administration” on page F-1813
*   "Minimum purchase price of the variant in the stock." on page F-1814

### Menus in the Stock module

You can open the Stock dialogs with the following menus:
*   "Menu overview in Bookings section" on page F-1694
*   "Menu overview in Master data section" on page F-1694
*   "Menu overview in Inventory section" on page F-1695
*   "Menu overview in Evaluation section" on page F-1695
*   "Menu overview in Info system section" on page F-1696
*   "Menu overview in Print section" on page F-1697
*   "Supplementary menu" on page F-1698

### This section provides information on the following subjects:
*   Overview
    *   Menus in the Stock module
    *   Menu overview in Bookings section
    *   Menu overview in Master data section
    *   Menu overview in Inventory section
    *   Menu overview in Evaluation section
    *   Menu overview in Info system section
    *   Menu overview in Print section
    *   Menu overview in System section
    *   Supplementary menu
*   Search Functions
*   Stock bookings
    *   Warehouse In
        *   Warehouse in – quantity tab
        *   Warehouse in – quantity tab
    *   Warehouse out
    *   Box warehouse in
        *   Box warehouse in - pieces tab
        *   Box warehouse in - quantity
        *   Single lite information
    *   Box warehouse out
    *   Slot warehouse in
        *   Slot warehouse in - Pieces
        *   Slot warehouse in – Quantity
    *   Slot warehouse out
    *   Stack warehouse in
    *   Modify stack warehouse
    *   Rack warehouse in
    *   Rack warehouse out
        *   Rack warehouse out - order related
        *   Rack warehouse out - Transfer
    *   Warehouse out (order-related)
    *   Booking correction – overview
    *   Booking correction - Details
*   Master Data Management
    *   Stockroom administration
    *   Article master data stock
*   Inventory Management
    *   Inventory - Default warehouse
    *   Inventory - box warehouse
    *   Inventory - Slot warehouse
    *   Inventory - stack warehouse
    *   Inventory - Rack warehouse
*   Evaluation
    *   Evaluation - default warehouse
    *   Evaluation - box warehouse
    *   Evaluation - slot warehouse
    *   Evaluation - stack warehouse
    *   Evaluation - rack warehouse
*   Information System
    *   Info: Stock articles
        *   Info: Stock articles - Filter dialog
        *   Info: Stock articles - Hit list
        *   Info: Stock articles - Hit list details
    *   Info: Stock variants
        *   Info: Stock variants - filter dialog
        *   Info: Stock variants - hit list
        *   Info: Stock variants - hit list details
    *   Info: Stock slots
        *   Info: Stock slots - filter dialog
        *   Info: Stock slots - hit list
        *   Info: Stock slots - hit list details
    *   Info: Stock racks
        *   Info: Stock racks - filter dialog
        *   Info: Stock racks - hit list details - general
        *   Info: Stock racks - hit list details
    *   Info: Stock stacks
        *   Info: Stock stacks - filter dialog
        *   Info: Stock stacks - hit list
        *   Info: Stock stacks - hit list details
    *   Info: Stock lites
        *   Info: Stock lites - filter dialog
        *   Info: Stock lites - hit list
    *   Info: Stock history
        *   Info: Stock history - filter dialog
        *   Info: Stock history - hit list
        *   Info: Stock history - Hit list details
    *   Orders/purchase orders
        *   Orders/purchase orders - filter dialog
        *   Orders/purchase orders - hit list
        *   Orders/purchase orders - hit list details
    *   Booking status
        *   Booking status – unbooked
        *   Booking status – error
        *   Booking status – inventory
        *   Booking status - correction
    *   Stock information - Pick list
    *   Stock information - Hit list
    *   SCC status
    *   Range - Stock forecast
    *   Range - Hit list
    *   Available stock
    *   Stock forecast
*   Print
    *   Print labels for boxes
    *   List printing
*   System Administration
    *   Delete stock log
    *   Stock price correction
    *   Stock backup

### Menu overview in Bookings section
You will find the following entries in the Booking section:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Warehouse in | ⇨ "Warehouse In" on page F-1701 |
| b | Warehouse out | ⇨ "Warehouse out" on page F-1710 |
| c | Box in | ⇨ "Box warehouse in" on page F-1711 |
| d | Box out | ⇨ "Box warehouse out" on page F-1718 |
| e | Slot in | ⇨ "Slot warehouse in" on page F-1719 |
| f | Slot out | ⇨ "Slot warehouse out" on page F-1724 |
| g | Stack management | Customer-specific functions will be explained in detail in a separate section. |
| h | Stack in | ⇨ "Stack warehouse in" on page F-1725 |
| i | Stack modification | ⇨ "Modify stack warehouse" on page F-1727 |
| j | Rack in | ⇨ "Rack warehouse in" on page F-1729 |
| k | Rack out | ⇨ "Rack warehouse out" on page F-1731 |
| l | Stack booking (doc.rel.) | Customer-specific functions will be explained in detail in a separate section. |
| m | Outg. stocks (order-rel.) | ⇨ "Warehouse out (order-related)" on page F-1735 |
| n | Correction | ⇨ "Booking correction - overview" on page F-1737 |

### Menu overview in Master data section
You will find the following entries in the Master data section:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Location | ⇨ "Stockroom administration" on page F-1741 |
| b | Article | ⇨ "Article master data stock" on page F-1743 |
| c | Slots | Customer-specific functions will be explained in detail in a separate section. |
| d | Stack types | Customer-specific functions will be explained in detail in a separate section. |

### Menu overview in Inventory section
You will find the following entries in the Inventory section:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Stock | ⇨ "Inventory - Default warehouse" on page F-1746 |
| b | Box warehouse | ⇨ "Inventory - box warehouse" on page F-1750 |
| c | Slot warehouse | ⇨ "Inventory - Slot warehouse" on page F-1752 |
| d | Stack warehouse | ⇨ "Inventory - stack warehouse" on page F-1754 |
| e | Rack warehouse | ⇨ "Inventory - Rack warehouse" on page F-1756 |

### Menu overview in Evaluation section
You will find the following entries in the Evaluation section:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Stock | ⇨ "Evaluation – default warehouse" on page F-1758 |
| b | Box warehouse | ⇨ "Evaluation – box warehouse" on page F-1761 |
| c | Slot warehouse | ⇨ "Evaluation – slot warehouse" on page F-1762 |
| d | Stack warehouse | ⇨ "Evaluation - stack warehouse" on page F-1763 |
| e | Rack warehouse | ⇨ "Evaluation – rack warehouse" on page F-1764 |

### Menu overview in Info system section
You will find the following entries in the Info section:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Article | ⇨ "Info: Stock articles - Filter dialog" on page F-1766 |
| b | Variant | ⇨ "Info: Stock variants - filter dialog" on page F-1770 |
| c | Slot | ⇨ "Info: Stock slots" on page F-1774 |
| d | Rack | ⇨ "Info: Stock stacks - filter dialog" on page F-1780 |
| e | Stack | ⇨ "Info: Stock stacks - filter dialog" on page F-1780 |
| f | Lite | ⇨ "Info: Stock lites – filter dialog" on page F-1784 |
| g | History | ⇨ "Info: Stock history - filter dialog" on page F-1787 |
| h | Orders/Purchase orders | ⇨ "Orders/purchase orders - filter dialog" on page F-1792 |
| i | Booking status | ⇨ Opens the submenu |
| ia | Booking status - Unbooked | ⇨ "Booking status - unbooked" on page F-1796 |
| ib | Booking status - Error | ⇨ "Booking status - error" on page F-1798 |
| ic | Booking status - Inventory | ⇨ "Booking status - inventory" on page F-1800 |
| j | Order list | ⇨ "Stock information - Pick list" on page F-1803 |
| k | SCC status | At present, this dialog is not used |
| l | Range | ⇨ "Range - Stock forecast" on page F-1805 |
| m | Available stock | ⇨ "Available stock" on page F-1807 |
| n | Forecast | ⇨ "Stock forecast" on page F-1809 |

### Menu overview in Print section
You will find the following entries in the Print section:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Labels | ⇨ "Print labels for boxes" on page F-1811 |
| b | List printing | The dialog is described in the Sales section. ⇨ Sales, "List printing" on page D-1427 |

### Menu overview in System section
You will find the following entries in the System section:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Delete stock log | ⇨ "Delete stock log" on page F-1813 |
| b | Price correction | ⇨ "Stock price correction" on page F-1814 |
| c | Stock backup | ⇨ |

### Supplementary menu `<F4>`
On the Booking dialogs of the Stock module, the Supplementary menu is also available. These menu entries can be reached depending on the context.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | PCd prices | In the stock ins, you can assign articles pre-defined prices via price codes. You can select the price codes from a pre-defined list. |
| b | Booking - no price | In the stock ins, you can assign articles the price = 0. |
| c | Trans.bookings | Transfer selected data record to another stock. The booking must be completed with [OK]. |
| d | Project booking | Assign selected data record to a project (e.g. construction site). |
| e | Boxes | Opens the Boxes submenu |
| ea | Boxes - book boxes | Removes the box of the current data record from the box warehouse and books the articles of the box automatically into the normal warehouse. The booking must be completed with [OK]. |
| eb | Boxes - resolve box | Removes the box of the current data record from the box warehouse and books the articles into a target warehouse. The booking must be completed with [OK]. |
| ef | Boxes - single lite information | Opens the Single lite information submenu |
| efa | Boxes - single lite information - view (<Shift> + <F2>) | ⇨ "Box warehouse in - quantity" on page F-1715 |
| efb | Boxes - single lite information - edit (<Shift> + <E>) | ⇨ "Box warehouse in - quantity" on page F-1715 |

## Search Functions

In the A+W Enterprise Stock module, you can search for information via the search functions, e.g. about articles, market partners, or orders.

These search functions are available in all A+W Enterprise modules and are operated the same way. There are descriptions in the following chapters:
⇨ Sales, "Find orders" on page D-1069
⇨ Sales, "Find market partner" on page D-1087
⇨ Sales, "Find article" on page D-1097

You can get stock-related information via the information system functions, e.g. about articles, stock types, orders, and POs.
⇨ "Information System" on page F-1765

## Stock bookings

In the Stock module, you manage the stock ins and outs of all articles in stock. You enter and edit the bookings and make booking corrections.

The following dialogs are described in this section:
*   "Warehouse In" on page F-1701
*   "Warehouse out" on page F-1710
*   "Box warehouse in" on page F-1711
*   "Box warehouse out" on page F-1718
*   "Slot warehouse in" on page F-1719
*   "Slot warehouse out" on page F-1724
*   "Stack warehouse in" on page F-1725
*   "Modify stack warehouse" on page F-1727
*   "Rack warehouse in" on page F-1729
*   "Rack warehouse out" on page F-1731
*   "Warehouse out (order-related)" on page F-1735
*   "Booking correction – overview" on page F-1737
*   "Booking correction - Details" on page F-1739
