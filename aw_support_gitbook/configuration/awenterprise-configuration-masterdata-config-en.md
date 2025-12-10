---
title: "EN-CONFIG-AW_Enterprise_4"
source: "EN-CONFIG-AW_Enterprise_4.pdf"
tags: ["A+W Enterprise", "Configuration", "Master Data", "BOM", "Product Exchange", "Stock Management", "Order Pool", "Dispatch", "PO Management", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical configuration guide for A+W Enterprise software. This document covers advanced settings for edge stripping, masking, master data management, product exchange, stock management, and order processing."
long_description: "This document is a comprehensive technical manual for configuring the A+W Enterprise system. It details various modules and functionalities, including internal P.O. transfers, masking processes for coated sheets, and master data setup for articles, processing, and materials. The guide provides step-by-step instructions for setting up bill of materials (BOM), handling stepped IG units, and managing product exchanges for IG, LAMI, and TG products. It also covers the configuration of stock management, including item master data, inventory evaluation (FIFO/LIFO), and triggering purchase order (PO) proposals. Additionally, the document explains settings for dispatch, order pool management, and system environment variables that control various automated behaviors within the software. It is intended for system administrators and technical writers responsible for maintaining and documenting the A+W Enterprise configuration."
---

If the entry help for the edge stripping is configured, then there is an alternative textsing for this processing analogous to the texting for the processing type masking.

The level of the processings (AW type 1025/edge stripping) is also transferred to the MEΤΑ processing of the article type edge stripping (atyp = 593).

The depths of the edge strippings are output on a separate line directly below the META article.

The texting of the individual processings is done without level, however with edge string and Ifm details.

This texting does not apply as default and is activated via an ENV switch.

The META processing may not have its own texting about article dimensioning.
(RANDENTSCHICHTEN_TEXTE_NEU = ON)

---
### 21.1.14. Internal P.O. Transfer

For internal P.O. transfer, the data is adopted as it was entered and calculated. In case of a BOM element (e.g. the smaller lite of a stepped IG unit), the processing record for edge stripping will be recalculated. Since the reference geometry is passed on from the IG to the individual element in this case, the processing parameters that took into account the IG step are no longer valid. The distances will be automatically adapted to the new reference geometry and do not have to be adapted manually.

### 21.1.15. Masking

AWD 250237 / September 2012

The aim of this extension is to simplify the input for the masking of coated sheets. As the masking depth varies for the individual edges and because a special article should be added to the BOM per depth for further processing (ALCIM, SN), this used to be a tedious affair. For stepped sheets, the user also had to take into account the steps for the parametrization of processing and add them if necessary.

Enabling this new module in connection with the appropriate master data adjustment will simplify the input considerably.

The switch MODUL_ABKLEBEN should be enabled.

### 21.1.16. Master data

In article master data, an article (AA) with article type = meta element and ALCIB type „Edgework"(270) has to be defined per level (top, bottom, both) and quantity unit. This article (AA) has to have a BOM consisting of a processing step (BB) and a material article (CC). The processing (BB) is defined with processing type "Edges" article type 592 by the AW processing type "Masking"(1960). The meta article (AA) itself does not have to have a certain quantity unit because this is only used for the text. The article name should however denote that this is about masking bottom/top/both. For the material article, a formula for calculating the quantities for cost calculation must be entered. The sizes ($1 and $2) for the formula are the dimensions of the masked sheet. The decisive criteria have to be entered for the processing step itself because these dimensions and properties will be preset at order entry.

- The dimensioning record for the processing article should have size parameter 1 with thickness and level (top/bottom/both), matching the parent article(AA). This level should be defined as "fixed".
- The quantity unit for the processing (lin.m/sqm) shall match that of the parent article (AA). It is vital to maintain the corresponding field in master data.
- The masking depth (XX) (default) should be entered in field „Thickness" on tab „Phys. properties".

Further processing articles are necessary to define the processing depth and the quantity units. Here no distinction per level bottom/top/both is required.

- Masking up to 10 mm(lin.m.): Thickness 10 mm/ QU = lin.m.
- Masking up to 50 mm(lin.m.): Thickness 50 mm/ QU = lin.m.
- Masking up to 100 mm(lin.m.): Thickness 100 mm/ QU = lin.m.
- Masking from 100 mm(lin.m.): Thickness: 9999 mm / QU = lin.m.

Corresponding articles will also be required for the quantity unit SQM. Please make sure that there is always an article with a maximum thickness per quantity unit so that the automatic search will produce results even for steps.

**Caution:** After you have created the article in the master data, you must restart the program before using it in the document entry.

### 21.1.17. Registration

Once the META element exists on the BOM (entered or adopted from the previous item), you can use `<F5>` or the button Parameter to open a dialogue for the edge-by-edge definition of the masking depth. The dialog shows the geometry of the reference sheet plus an input field on every edge for the masking depth. For new entries, these input fields are preset by the depth entered in the dimensioning master data for the processing (BB) and can be changed per edge if required. After saving and leaving the entire BOM, the BOM of the meta element will be completed. It will get a processing per masking depth. Matching edge vectors will be assigned to the different masking depths. The completed processing steps will be determined by means of the following logic, based on the defined masking depth: smallest entry in field, Thickness' is equal or bigger than the defined masking depth. The article's quantity unit (BB) defined in master data will be taken into account as well. The article level (BB) will also be adopted for all newly determined processing steps.

**Example 1:** A meta element „Masking for coating on top (SQM)" was added to the BOM. This article shows in the master BOM the processing step 'masking' (BB) with a thickness of 100 mm and level „top", and QU=SQM. The depth of all edges was changed to 12 mm by hand. The existing article (BB) is removed automatically because it does not fit the defined depth; the new article "Masking up to 50 mm (SQM)“ (BB1) was added.

**Example 1.1:** If the depth is changed to 12 mm only for one (or several) of the selected edges, two processing steps will be entered in the BOM. „Masking up to 10 mm" with the edge vector for the edges the depth of which remains unchanged and „Masking up to 50 mm" with the edge vector for the edges the depth of which was changed. As a processing parameter, the processing (BB1) shows the defined size of 12 mm.

If only the META element has been entered in the BOM without entering the depth, the depth record (table kstufparam, record type = 5) will be created automatically. A change of the masking depth may result in the allocation of a new BOM number in this case. The sub-elements of the type "Masking" cannot be changed on the BOM. They cannot be deleted or replaced because they are always determined automatically. The processing parameters of these elements cannot be changed either.

Price-relevant quantities (number of widths/heights) for shapes are defined like other edgework: If all edges are masked, the defaults apply; these are defined for processing articles in sub-menu „Price properties“ as Qty1 / Qty2. If there is no entry for the article as such or for the AW type "masking" in general, the edges will be calculated ac. to the shape.

### 21.1.18. Stepped IG

Starting with Version ALCIB 2011, a stepped IG with processing (with AWTyp) always has to be entered with the surrounding geometry as a reference - this means: without negative steps. (Reason: At present, SN cannot handle negative steps or processing dimensioned with a reference to the smaller sheet).

The processing step Masking is entered as described above, and refers to the individual sheet. On the step edges, the masking depth for the projecting sheets will be increased by the step size when the input fields are preset.

**Example 2:** An IG unit with a step of 100 mm on edge 1 consists of two coated lites. On both sheets, 10 mm shall be masked on all edges; the step shall also be masked. The entries for the larger sheet are preset automatically: Masking 110 mm on edge 1, masking 10 mm on edges 2, 3, 4, plus default for the smaller sheet: Masking 10 mm on edges 1, 2, 3, 4.

**Attention(!!)** For SN, all processing steps must be dimensioned based on the reference geometry. This is why in the processing dialog (<Ctrl> + <F8>) shows a masking depth of 110 mm for edge 1 of the smaller sheet. The entries for the masking depth cannot be changed in this dialog. The data shown in this dialog will be saved in another data structure, and processed by a program logic for SN; the masking depth of the individual sheets will not be changed.

In the above example (2), the processing „Masking up to 10 mm“ is determined for edges 2, 3 and 4 for the larger sheet, and the processing „Masking from 100 mm“ for edge 1. For the small sheet, the processing „Masking up to 10 mm“ is determined, albeit twice. Once for edges 2, 3 and 4 and once for edge 1. The reason is that SN cannot handle this processing by sheet at present. This is why edge 1 requires a special processing record which is internally diverted to the reference geometry.

If the step geometry is changed afterwards, the masking depths will be automatically adapted according to the described logic. Manual changes will be lost. The user is informed of this fact.

Since the masking depth for IG units is unpredictable, a new BOM number will be assigned whenever the item product includes a step and masking.

### 21.1.19. Different edge seal

From the list of the individual element sizes (<F3> in the price field) a dialog for adapting the sealing by edge can be opened with <Shift> + <F5> with the cursor on the BOM element 'Spacer'. As there is no defined connection between edge sealing and masking depth, the masking depth per edge cannot be automatically adapted after such a change. This amendment can however be made based on the META element, as for the amendment of the edge sealing on this list. Here, a change of depth can also result in the allocation of a new BOM.

### 21.1.20. Texting

It is essential that the meta elements as well as all processing steps of the type "Masking" are always set to Print = "YES" because the text for these elements is based on each other. The processing text for example 1.1 is created in the following way:

> " Masking for coating on top (article name META) on edges (text supplement 127) 1: 10 mm 2:10 mm 3:12 mm 4: 12 mm"
> " Masking up to 50 mm XXX lin.m. on edge 1 <Price>"
> " Masking up to 10 mm XXX lin.m. on edge 2 3 4 <Price>"

The sequence of the texting of the individual edges is done in the internal ALCIB edge sequence and not in the production edge sequence. Therefore, edge 4 comes before edge 2 if these have different masking depths.
For the processing steps, individual text can also be encoded in the dimensioning record. The texting of the META part is fixed, by contrast.

### 21.1.21. Internal transfer

For internal transfer, the data are adopted as they were entered and calculated. In case of a BOM element (e.g. the smaller sheet of a stepped IG unit), the processing record for masking will be recalculated. Since the reference geometry is passed on from the IG to the individual element in this case, the processing parameters that took into account the IG step are no longer valid. The depths will be automatically adapted to the new reference geometry and does not have to be adapted manually.

## 21.2. Modification of supply type

The adjustment of the supply type with reference is documented in the chapter "Entry with reference - supply types".

### 21.2.1. Spacer procurement like muntins

AWD #215783

If muntins are entered without using grid patterns, a special configuration allows adopting the supply type of the muntins (incl. suppliers if muntins are ordered) up to the inside spacers. (ENV switch SPROSSENLIEFERANT_AUF_RAHMEN = ON").

The following master data maintenance is mandatory for this logic.

1.  Go to Master data-> i Field configuration -> b Article field configuration and enter a new record (<F6>) of the type "ALPHANUM“, field name "Espace d'air". Please make sure to stick to this spelling because this field name is used for the linking of data.
2.  In article master data, enter the for the article 'inside spacer' (ALCIB article type 210) in menu <ShF4> -> n Configurable fields for the configurable field "Espace d'air" the thicknesses of the inside spacer to be checked when the supply type is adopted. Please enter the thicknesses separated by | and as integers, e.g. 8|10|12|14|16|18.
3.  For the inside spacer articles, "P.O." and "Production" should be defined as valid supply types in master data.

When the muntin dialog is closed after the sizes and muntins have been entered, the program will check if the inside spacer of the IG unit shows an entry in the configurable fields that matches the airspace of the current item. If there is no entry for the spacer or if the current spacer is not listed, the user will be informed that the adoption is impossible because of the spacer thickness. If the spacer matches a thickness on the list, the user will be asked whether the supply type or the supplier shall be adopted for the entire inside spacer. If this is required, the data will be adopted and if not, the inside spacer will keep the supply type defined in master data or in the existing BOM.

If more than one bar shall be added to the same inside spacer, the program also checks if all muntins have the same supply type. If not, the user is informed accordingly and can adjust this. If the supply types are not adjusted, the possible adoption will not be checked.

If muntins are entered for both spacers of a triple IG unit, each inside spacer will be checked separately.

Please note that the supply type can be adopted only in the described sequence of input. If the spacer is exchanged in the BOM afterwards, this information may be lost even if the muntins are adopted for the new inside spacer. A subsequent change of the airspace does not cause a new check. The same applies if the spacer is changed, e.g. by adopting the thickness of articles with thickness variants from the processing catalog.

### 21.2.2. Muntin supplier for the inside spacer

Via a configuration, you can set that the default supplier for the muntins is taken over not just into the grid, but also into the inside spacers. The muntin supplier is taken over for triple IGU into both spacers, even if only one spacer has the purchased muntins.

There are only two configuration possibilities:

1.  during the manual entry, a question is posed whether the procurement type or the supplier of the muntin should be taken over for the entire spacer. This variant does not apply for EDI orders.
2.  the procurement type or the supplier of the muntin should always be taken over automatically for the entire spacer. This variant also applies to EDI orders.

The configuration is done via the environment variable RAHMEN_BA_SPROSSE = 1/ON or 2.

### 21.2.3. Conversion to purchase order in case of violation of dimensional restrictions

If dimensional restrictions of the product to be produced have been violated and the user also has the right to enter the product anyway, the supply type of the item is automatically converted to "purchase order". If the "purchase order" is also active as an "alternative" supply type in the master record and the supplier is also entered, this supplier is also adopted. Otherwise, note appears to the user to enter the supplier. The supply type can be changed again later. If the measurement parameters are changed so that the restriction check takes place again, the supply type is also changed again. If the measurements are subsequently changed in such a way that the restrictions are no longer violated, no changeover takes place because the possibility of an immediate correction has already been given at the initial entry.

If the restrictions for the header article have been violated and the hint for this violation has also been output, this hint is also displayed as a tool tip in the measurement fields. However, the display only applies to the current item and only during entry or directly after the restrictions have been checked.

With reference, this automatic conversion does not take place.

DIMCONTROL_VIOLAT_PO = ON

## 21.3. Stock orders

### 21.3.1. Manual entry

See section Stock > Stock fill orders > Manual entry

## 21.4. Documentation back-up

#238503

There is always a chance of an unintentional crash of transaction recording caused by technical problems, unsuitable master data, incorrect operation, etc. The data lost this way for complicated, and even for completely normal transactions in ongoing operation frequently ensures displeasure and aggravation. This is why in the new version our goal is to offers support for this topic.

**Treatment of DB errors when saving**

In very rare cases, the transaction cannot be saved, if, e.g. a DB error occurs. Quite frequently, this is because of lacking master data input and assignments in particular and not all items. Up to now, with the occurrence of a DB error, only another attempt was offered, and if that did not work, the order was not saved. In the new version, it is detected whether the DB errors come from the item area, which according to our experience is what usually happens, and a report is made about the item in which a DB error first occurred. If possible, the error range is also located (directly from the item, from additional item dimensions, from the range of the processing data or conditions). In this case, the user is offered the opportunity to check the item. Here it is checked whether the problem can be detected on various dialogs (in case of impermissible values, the fields are filled with ***) in order to correct these values if necessary. In the extreme case, it may be necessary for you to delete the item and check the master data.

**Intermediate saving of the transactions**

Now there is an opportunity to back up an order/quotation/purchase order/supplier inquiry at runtime by saving it temporarily. On the lower part of the dialog, there is a new "Back up" button for this. The possibility for temporary saving exists in the header or the footer of the transaction if the items are already present, as well as in the item part itself. However, since the item data can only be backed up in complete form, the button is only active on an item entered up to the price. In an item that has not been entered completely, this is not possible because it may be that the data should be loaded later in precisely the backed-up state.

If a transaction has been backed up, then you should heed the further procedure for entry:

1.  **Initial entry:** for data back-up and subsequent cancellation of the entry (with <ESC> or <HOME>), the back-up is not retained.
2.  **Initial entry:** for data back-up and regular saving of the transaction, the back-up is overwritten with the last data entered.
3.  **Correction:** for orders with data back-up that are not yet released, during correction and the subsequent cancellation of the entry (with <ESC> and <HOME>) the user is informed that the transaction can only be exited in the last backed-up state and he is asked whether he would still like to exit the transaction and leave it in the system only as back-up or whether he would like to finish the change/correction.
4.  **Correction:** for transactions with data back-up that are not yet released, during correction and the subsequent cancellation of the entry (with <ESC> and <HOME>) the user is informed that exiting is no longer possible because the transaction was just backed up in an incomplete state. You can only reset the transaction to the last backed-up state and make the correction starting from this state through to the end or finish entering the current state of the correction.

If the transaction remained in the system due to a technical fault or was consciously stored as a back-up by the user (see point 3), then it is no longer available for all additional processes because the backed-up data does not necessarily correspond to a true end state of the transaction (for example, the following actions could not have executed: discount calculation and revenue distribution, determination of the further system throughput, etc.). They MUST be brought to a consistent state through correct storage in ALCIB.

The back-up state of an order is displayed as a traffic light in the lower left corner of the main dialog. Backed-up orders have a "green" light. There is no traffic light for orders that are not backed up. In addition, it is possible to make the traffic light display more "meaningful." With a switch, you can specify the quantity of production-relevant changes that are regarded as a "critical number." If the quantity of changes made (for the entry, the newly-entered fields count as a change) reaches half of the "critical number," the traffic light turns "yellow." If the number of changes reaches the "critical number," the notice appears (once) that a back-up at the next opportunity would make sense and the traffic light turns "red." After the successful back-up, the traffic light turns "green" again and the changes are counted again from the start.

When starting the order entry, first there is always a check whether backed-up orders from this user are still in the system. These are offered for selection first. If these are orders that are not yet released, then they appear with the status "green." These orders are not critical and you can re-enter them at a later point in time. In this case, it is permissible to exit the selection dialog with cancel. If a back-up of the order is found that was already released, then the status changes to "red" in order to show that there is an urgent need to act here. The user can not exit the selection dialog and discard changes in this situation.

If the intermediate saving encounters a DB error, then the back-up is canceled and the system behaves as it does during final saving. (see above "Treatment of DB errors when saving").

For the expanded traffic light, you should activate the switch SICHERUNGSSCHRITT = xx.

## 21.5. Dispatch type vs. Route

Starting in May 2025 this also affects A+W iQuote (documentservice.hotfix - 13.04.7673)

### 21.5.1. Automatic changing of the dispatch type in case of route change (dispatch type - route)

With this configuration, each dispatch type can be assigned **only precisely** one route and each route **only precisely** one dispatch type. With a change of the route, there is an adjustment of the dispatch type, but with a change of the dispatch type, there is no adjustment of the route.

**VERSARTHOLEN_BEI_ROUTENAEND:** disabled or OFF

Within the master data (Master data - Keys - System - Dispatch - Dispatch type), a route can be assigned to a dispatch type. If this route is used for the order entry, the dispatch type is drawn. With the change of the route (manual, change of the delivery type, selection of the delivery address), the dispatch type is adjusted. A route change in dispatch does NOT cause a change of the dispatch type. Similarly, a change of the dispatch type does not cause a change of the route. This is the default behavior in A+W Enterprise.

### 21.5.2. Automatic changing of the dispatch type in case of route change (route - dispatch type)

With this configuration, a dispatch type can be assigned to one route, but a dispatch type can be assigned to several routes. With a change of the route, there is an adjustment of the dispatch type, but with a change of the dispatch type, there is no adjustment of the route.

**VERSARTHOLEN_BEI_ROUTENAEND:** ON or 1

The system can be configured so that within the master data of a route, a dispatch type can be assigned (Master data - Keys - System - Dispatch - Routes - Routes - Routes). This dispatch type is then taken over into the document. By default, maintenance of the dispatch type in route master data is disabled. The logic can be enabled by environment variable. If this environment variable is active, routes cannot be maintained in dispatch type master data either.

When the new logic is active, every change of route (directly or via direct shipment/collection, or change of address) will result in the dispatch type for this route being adopted if it is kept in route master data. If for the new route no dispatch type is stored, then the current one in the order will be retained. Manual changes will be dropped if the route is changed in the foreground after the fact and a dispatch type is stored for this route. There is no takeover of the dispatch type for the route assignment by the background process in the course of the client assignment after entry in the call center. Also for delivery "via plant", the data for the dispatch type is taken over from both routes (internal + route to the customer). On the document dialog ("Properties" tab), the dispatch type of the route to the customer is always displayed. Shipping information dialog (menu Shipping information) shows the data for the dispatch type "via plant" if shipping "via plant" has been selected.

Change of the route in dispatch does not cause a change of the dispatch type.

### 21.5.1. Double-sided change of route and dispatch type

With this configuration, a dispatch type can be assigned to one route, but a dispatch type can be assigned to several routes. With a change of the route, there is an adjustment of the dispatch type, but with a change of the dispatch type, there is no adjustment of the route. Furthermore, this assignment is also checked in dispatch.

**VERSARTHOLEN_BEI_ROUTENAEND: 2**
alcib 13.04.20025
lapool - 13.04.20671
documentservice - 13.04.7673

The system can be configured so that within the master data of a route, a dispatch type can be assigned (Master data - Keys - System - Dispatch - Routes - Routes - Routes). This dispatch type is then taken over into the document. By default, maintenance of the dispatch type in route master data is disabled. The logic can be enabled by environment variable. If this environment variable is active routes cannot be maintained in dispatch type master data either.

**1. Document entry**

In a document, the dispatch type is drawn first from the route determined. If a route change is made directly through manual change or indirectly through change of the object, selection of a different delivery address or change of the delivery type, the dispatch type is also determined anew.

If a route is used to which no dispatch type is assigned, then the user receives a message that the route has been assigned no dispatch type and instead, the dispatch type from the market partner master data is obtained.

If the dispatch type is changed in the order, the system checks whether there is a unique assignment to the route. If so, this route is taken over. If several routes are assigned, a selection is offered via selo. If for dispatch type no assignment is found, then the system checks whether the route and dispatch type match. Only if there is no assignment for dispatch type for the route in the master data may the combination remain.

If the dispatch type is changed by changing the route or vice-versa, the corresponding discounts will be recalculated.

**2. Entry in the call center.**

The routes and dispatch type assignment should be made in the call center. After entry, there is a fixed client assignment and the routes are replaced with client-specific routes. The routes must be configured so that the corresponding route of client X also has the appropriate dispatch type and the identical discount as the original route from the call center. After the site assignment, there is NO new discount calculation by background process intauf.

**3. Changes in dispatch**

If in dispatch the order is shifted from route 1 to route 2, then in dispatch the dispatch type is also adjusted for the orders if route 2 has a different dispatch type. There is no comparison in the order itself.

If the dispatch type is changed on the order level, then there is a check whether it fits the route and the user is informed about the deviation. The changed dispatch type can also be taken over into the order. However, there is no new calculation of the order (discounts).

**4. Change in iQuote.**

If the dispatch type is changed in A+W iQuote, there is an attempt to find a route automatically. If there is a clear assignment, this route is taken over. If there is no clear assignment, the route with the highest priority (1= highest, 9999 lowest priority) is taken. If no clear assignment is found, the first appropriate route that was found in DB for this dispatch type is used and the order includes a note that no clear route could be determined.

### 21.5.2. Configuration

**VERSARTHOLEN_BEI_ROUTENAEND (client reference: no)**

This environment variable controls the behavior of route to dispatch type and vice-versa.

-   **OFF** - route assignment to a dispatch type 1:1
-   **ON/ 1** - dispatch assignment to route 1:n
-   **2** - Dispatch assignment to routes m:n

## 22. Product exchange

### 22.1. Exchange of the BOM elements for IG and LAMI

The expanded dialog for product exchange is started via menu in the process "Product Details"-> "Product exchange" or use `<F3>` directly in the document header/footer. Therefore, it is now possible not just to enter a new product and exchange glass for existing items, but also to exchange the inner frame for IG products and films for LAMI.

**Figure 13: Product exchange: Start dialog after the quantity selection**

Important for use is the correct construction of the BOMs. The entries of the assembly positions for glass but also for frames and films are required. Furthermore, work is possible with just one film, so that in this place the META films are recommended.

After entry of the new product, in the intermediate range, the original structure according to master data(!) is displayed. The global exchange rules are not considered at this point. The glass/IF for IG products that can be marked in the process as exchange will then also be considered for the desired construction.

**Figure 14: Product exchange - details on exchange**

For the glass in the BOM, you can also turn the glass in the BOM through IP change.

With a key combination, it is also possible to implement the desired construction on original construction. (Configurable? It's being offered, not yet done 08/2021)

### 22.2. Exchange of AIR for IG exchange

If IG product is excxhanged, in addition to the familiar questions about the new price calculation and text/config fields takeover, there is a query whether AIR should be changed. If this is desired, a dialog appears where you can enter the new AIR per item.

**Figure 15: Product exchange for items**

If a double is exchanged for a triple IG, then this dialog also opens automatically and you can adjust both AIRs. (configurable, new *mfo)

### 22.3. Product exchange for TG

TGH products can be exchanged, not just on the product level, but also the glass of the 1st level. (configurable, new *mfo, ENV)

**Figure 16: Product exchange for TG**

**Configuration:** PRODAUSTAUSCH_ESG_ERWEITERT

### 22.4. Additional processings in the existing BOM

If in the original BOM on the level of the header article itself or on the level of the solid material the other elements are found (all marked with the "Z" code in the BOM), these are listed in a separate dialog. In the 1st column, there is a note about where the additional elements were found. In the "Transfer" column, there is the possibility to take these along to the new BOM during the exchange (Y) or not (N). If you are working with the helper modules for masking, the data can only be taken along in the block or not. (configurable, new *mfo)

**Figure 17: Transfer additional elements**

In this separate table, all processings that have a "Z" code are taken along. Even if these are directly in the master BOM with this code.

If you are not certain whether or not the processing should be taken over, you can use `<F5>` to look at the original BOM of the new glass.

If, e.g. a processing with "Z" in the glass was found before the product exchange, it is offered for transfer. With F5, you can see in the overview that the new glass itself already has this processing in the BOM and so you can set Übernehmen=N so that this processing does not occur twice.

**Figure 18: Transfer additional elements to BOM**

### 22.5. Extended product exchange

In order to be able to use the extended product exchange, the environment variable ERWEITERTER_PRODTAUSCH = ON has to be activated.

**Functions of the extended product exchange (#453595)**

1.  **Further BOM parts for IG/LAMI**
    In the case of an extended product exchange, not only glass but also spacers are transferred to the list of exchange parts for IG units and can thus be changed. Also in the case of LAMI, the first three glasses and two foils (1 foil per gap) can be exchanged in the new product. It is also possible to change the assembly position for single glasses. But only in the corresponding assembly position.

2.  **Additional elements in the BOM (processing steps and parts)**
    All processing steps / parts that are marked as "additional" items (Z) in the existing product on the first BOM level are taken into account when exchanging products. If IG or LAMI is used as the header product, all processing steps / parts that are marked as the suffix "Z" on the 1st BOM level of the individual glasses are taken into account when exchanging products. These additional elements are displayed in a separate dialog, in which the user is given an overview of these additional elements of the selected BOM. He can control whether these elements are to be included in the new BOM by converting the "Apply" flag.

3.  **TG stamp**
    In the case of processing of the type "stamp" (A+W type = 1250), both the additional marker (Z) and the exchange marker (A) are taken into account if this is located in the first BOM level of the product itself or in the first BOM level of the individual glasses. If the new product or the new sub-glass itself also has a processing of the A+W type = stamp, this is shown in the overview as "exchange".

4.  **Qty. stepped IG**
    Efforts are also being made to incorporate steps into the new product. If the structure of the old product and the new one is adequate (items/sequence of elements within the BOM), the steps are transferred.

5.  **META elements**
    In general, META are not taken over during product exchange, even if they are marked as an addition. An exception is made for masking and enamel strips when working with the corresponding A+W modules. It is very important that the structure of the mentioned METAs in the master corresponds exactly to the regulations. In the overview dialog, you can then only select for the META part whether these are to be included in the new BOM inclusive processing steps. These processing steps, including META, form a block that is not broken apart.

## 23. Entry with interior view

In A+W Enterprise, entries are made by default in the exterior view (header article has assembly position 1). However, you can turn the entire product structure by changing the assembly position of the header article. This happens via BOM F3 (not F5) - header article Shift+F5 or the button St.Kopfdaten.

The changing of the assembly position causes the lites of the unit to be turned. When changing the assembly position of a lite or an item in the A+W Enterprise, the positioning of processings on the lite are not changed. These still refer to the header geometry. The consequence can be that after turning, the processing is not where the user expects it, especially if whole glass structures are turned (changing of the AP of the header part).

See AWDesk #412275, #412076

See also section "Views in the SNLive sketch"

**Example:**

IG consisting of Float1 and Float2. The product structure from the outside: Float1, frame, Float2.

Float1 has sand blasting with level "top"; that means the sand blasting is applied on the outside of Float1.

Now the product structure is turned around in that the AP of the header part is changed. This produces the following product structure from the outside: Float2, frame, Float1

Now the sand blasting is positioned on Float1 to the frame, for the level is still "top" and thus the processing is applied to the outside (in the direction sun -> product structure) with regard to the overall structure.

However, the expectation could be that the surface processing is now applied away from the frame on the inside (away from the sun).

The production transfer is influenced by the following switches:

**PMEKOPF_EP**

If the variable is ON and active, the assembly position of the main part is taken into account when the routing is created; otherwise the assembly position 1 applies to the main part. This is relevant if a rotation is to take place for straight assembly positions (PMEHANDLE_GERADE_EP).
The variable is also evaluated in the direct ALCIM import.

**PMEHANDLE_GERADE_EP**

If the variable is active and greater than 0, for straight assembly positions, it has to be considered that the following BOM structure is turned. E.g. In the direct ALCIM data import, the lites are then taken over in another sequence. The same applies for the OrderXML service. Here, the switch applies by default as active. To switch it off, it has to be activated and have the value 0. !!!CAUTION: Up to Version 2011, this variable has to be set for ORDERXML- transfer!!! It is not yet activated automatically here!!!!

## 24. Bill of material in document entry

With the environment variable "ADD_DEL_BUTTON_OK, you can display the buttons "Duplic.", "New," "Copy," "Ins.," "Del.", and "A-search" on the BOM dialog. The functions are also available via key combinations.

| Button | Key Combination |
| :--- | :--- |
| Duplik. | Ctrl-A |
| Neu | F6 |
| Kopie | Ctrl+B |
| Einfg | Ctrl+O |
| Entf | F7 |
| A-Suche | Return in the empty article number field |

### 24.1. Copying several processings at once between BOM levels

alcib - 13.04.10231 // QR 2105

After the processings have been placed on a level, it is now possible to transfer them as a block to another glass in the BOM. For this, the processings in question must be marked first. This is possible directly in the BOM in the last field on the "Processing parameters(short)" tab.

After the proceessings are selected, you have to combine them for the copy process. This can be done with the "Copy" button or the key combination <Ctrl+B>. Here all parameters entered are noted. If additional processing should now be noted or there are parameter corrections, then the data must be recompiled directly after this.
If the processings are only marked and not prepared for copying, then the user will be informed when leaving the BOM because the marking applies only for the current level and if the data is not compiled for the copying, the marking will be deleted.
If the processings are dimensioned, marked, and prepared for copying, you can navigate to another glass in the BOM and use the "Insert" button or the key combination <Ctrl+0> to insert all marked processings.
Here it is important that the processings to be copied are always attached at the end of the BOM level. They cannot be inserted. Even if on the level on which they were entered they are not directly next to one another. Directly after all processings were attached on the level, there comes the query whether these should be transferred to all other glass. If not, the marked data is deleted. If so, then you can navigate to the next glass and use "Insert" or <Ctrl+0> to add the processings again.

For this multiple copy function, only simple processings or parts without their own BOM (except for product-relevant elements for glass, spacers, muntins, etc.) are suitable.
Copying META processings must be done individually as it was earlier.

For activation, the environment variable PROCESSING_MULTICOPY = ON must be set.

### 24.2. Procurement type "* before EDI"

05/22/2024 // alcib - 13.04.17741

In cooperation with "A+W Production", not all "before EDI" procurement types are allowed within the BOM. Therefore, the entry is subject to certain restrictions.

Generally, a "before EDI" procurement type is only allowed below a purchased part. (see also "EN-CONFIG-A+W Enterprise Production Interface")

To prevent mis-entry and thus errors in the further process chain, the entry of "before EDI" procurement types is not allowed in A+W Enterprise by default.

After a corresponding process analysis and advising, the entry of the procurement type "PO before EDI" can be activated via the environment variable "BA_VORDFUE = 1". If "Production before EDI" should be applied, then the value 3 must be set in the environment variables ("BA_VORDFUE = 3"). If both procurement types should be possible, then the variable must be activated as follows "BA_VORDFUE = 1|3".

**ATTENTION:** It must be noted that when using this function, there is no booking of the dispatch data for purchasing and no dependent scheduling within A+W Production. These functions are only made available in the module of the "extended workbench".

### 24.3. Environment variables

**ADD_DEL_BUTTON_OK (client reference: no)**
This environment variable activates the ADD + DEL button display in the BOM

**BA_VORDFUE (client reference: no)**
You can allow "PO before EDI" (bestellkz = 1) and "production before EDI" (bestellkz=3) in the BOM. In the variable, you can enter these "bestellkz" separated by '|' so that AWE does not reject the entry.
Please only set if it is coordinated with AWP.

**PROCESSING_MULTICOPY (client reference: no)**
Activates the possibility of copying several processings between BOM levels.

## 25. Notes on documents

Notes on documents can be entered manually in the document entry with "Shift+F4" - "Document notes".

How document notes are treated during entry with reference is documented in section "Entry with reference - document notes".

### 25.1. "Order information" menu element

In the menu element "Sales - Overview - Order information" you can use F5 or the "Notes" button to view the document notes.

If the environment variable KAUFINFO_AUS_STATUS=2 is active, then you can use this menu element to enter or change notes. If the order is edited by the system or an employee, there is an appropriate notice here and the notes are displayed in read mode.

If an employee with active environment configuration has opened the dialog for the "document notes" via the "Order information" menu element, the order is locked for other employees and the system for processing.

If the document notes are exited with saving, then there is a security query asking whether the information should actually be saved. If you answer "yes" to the query, then the document notes will be saved. However, the order will NOT be transferred to the background process "intauf" and the customizing script "vorgangs_sql" will also not be called.

This way, document notes can be corrected and added without otherwise changing the order or system load by causing all of the processing through the background processes.

The environment variable can be activated employee-specifically.

## 26. Order pool (Order pool)

### 26.1. Access

With appropriate configuration, now it is possible to input order numbers on the start screen of the "Generate POs" program or to select them via selo (plus expanded search).

If no order numbers are entered or selected, the program "Generate POs" proceeds as previously; that is, all PO suggestions that are not locked by other users are loaded for PO generation.

If on the start screen a valid order number was entered or selected, then only the PO suggestions for these orders are loaded as PO generation unless they are locked by other users.

The environment variable ABTONLY must have the value "7".
The environment variable MODUL_EINKAUF must have the value "3".

### 26.2. Grouping

Within the PO pool, you can mark individual items to be ordered and POs. Which PO items are combined into a PO depends on the items' data. It can be defined via environment variable whether all items should be combined into a PO or if one PO per supplier should be generated. If the environment variable is set to 0 (or not activated at all), then all marked items are ordered from the supplier on which the cursor is currently.

**BESTPOOL_GRUPPIEREN**

Controls how the PO pool records are grouped by default:
-   **0** = by selected items
-   **1** = by supplier

In addition, there are other permanently defined criteria in the program:
-   Change if the delivery address changes (e.g. in case of direct shipment)

### 26.3. Breakage

Within the PO pool, on the "Details" tab, it is possible to enter a breakage reason and a breakage location (release February 2021). If a breakage remake is being processed with A+W Production, the breakage location and/or breakage location is transferred from production.

The breakage reasons are maintained in the table pmsbg gepflegt. The breakage locations in xbruchorte. There is no maintenance dialog for both tables. They are filled appropriately during the reporting of the breakage reorders from production.

### 26.4. Delivery date

If in the default PO pool order items with different delivery dates are grouped for a PO, then the earliest delivery date for the entire PO is taken over for the entire PO.

If in the course of the "Extended workbench" several processings with different delivery times are ordered at the same time from the same supplier, it can still be necessary that not the earliest but the latest delivery date should be taken over in the PO.

Now the PO pool can be configured precisely this way (environment variable BESTPOOL_LATE_PROCESSING). If this configuration is active, a few restrictions apply. If both ordered processings and glass are marked together, processings and glass are grouped in separate POs. For the glass order, the earliest delivery date will be used as previously and for the processing PO the latest delivery date. If for processings to be ordered accessories or foils are ordered, then these are marked during the marking of the processing to be ordered. In this case, these accessories are inserted into the PO for the processings and the PO receives the latest delivery date. If these accessories and foils are marked and grouped without the associated processing, they are treated like glass and receive the earliest delivery date.

### 26.5. Purchase information/restriction display

By default, in the PO pool in the "Pu" column (purchase information), an "I" appears if in the associated order, information is entered explicitly for purchasing.

QR 2406 / alcib - 13.04.18137

Through a configuration (environment variable BESTPOOL_INFO_EXTENDED, Stored Procedure „cu_bestellpool_ekinfo“), the column "Pu"(purchase information) receives additional characteristics.

For each PO item, the customer-specific SP "cu_bestellpool_ekinfo()" is called. It can check customer-specific restrictions. If the SP returns a value = 1, then the restrictions are violated. The column looks as follows:

-   **"."** - if there is no purchase information and no restriction violation.
-   **"I"** - if there is only purchase information
-   **"R"** - if there is only a restriction violation but no purchase information
-   **"*"** - if there is both purchase information and a restriction violation.

The customer-specific SP „cu_bestellpool_ekinfo()“ is called with the following parameters :
`cu_bestellpool_ekinfo (<ext.Auftragsnummr(auftrnr)>, <interne Auftragsnummer(aufnr)>, <int.Positionsnummer(posnr)>, <Tupelnummer(tnr)>,<Breite>,<Höhe>,<Gewicht>)` and returns = 1 for following special restrictions, otherwise = 0. The transfer parameters refer to the order for which the PO should be generated.

### 26.6. POs for packaging (boxes)

The function for box orders is currently in the pilot phase
17.02.2025: Currently the documentation is in the Sharepoint `A+W Clarity R&D - Dokumente\General\Enterprise\BestellKisten.docx`
As soon as the module has been tested successfully with pilot customers, the documentation will be taken over into the Enterprise configuration notes.

### 26.7. Environment variables

**ABTONLY (client reference: no)**
The variable indicates that the current user is working with department restriction.
-   **1** = Department of the article must match Dept. entered or be 0.
-   **2** = user of the order must be equal to the user of the PO or be 0.
-   **3** = Department of the order must be equal to the Dept. entered or be 0.
-   **4** = For completely ordered item: Department of the product group of the item is compared to the department entered. If the department of the product group is 0, the department of the article is compared.
    For parts from the BOM: same logic as 1.
-   **5 and 6:** special logic for user 24.
-   **7** = Specification of order numbers possible

**BESTPOOL_GRUPPIEREN (client reference: no)**
This variable controls how the PO pool records are grouped by default:
-   **0** = by selected items
-   **1** = by supplier

**BESTPOOL_INFO_EXTENDED (client reference: no)**
If this environment variable is active, for the population of the colum "Pu" (purchase information), the stored procedure "cu_bestellpool_ekinfo" is also called.

## 27. PO management/PO entry

### 27.1. Warning in case of change in POs with order relation

QR 2503

If in a PO with order relation items are deleted or quantities are changed, the PO no longer corresponds to the order requirements. This means that reports cannot be executed completely in the order and dispatch. This has consequences for delivery note and invoicing. Thus, with appropriate configuration (LIEFERSCHEIN_CHECKER), no delivery note can be generated if the incoming goods message is missing for individual items. For this reason, there is now a warning message on the PO dialog. However, the change is not disabled.

If the message is not required, it can be removed via customizing. This is message 38513.

## 28. Dispatch notification

### 28.1. Message on PO date postponement

Note: Here, the concern is only the sending of e-mails for the manual change of the goods receipt date of a PO. The concern is not that the change of a planned goods receipt date of a PO automatically shifts the delivery dates and goods receipt dates of upstream documents. This always requires personal communication and manual adjustment.

see also document 95577: January 2005
Purchase - Dispatch Notification

If a dispatch notification is saved for a PO, an e-mail can be sent to configured employees.

For this, the environment variable AVISE_MAIL must be activated. If the environment variable is not active, no e-mail will be sent. In the environment variable, you can specify who should receive the e-mail.

Starting in Feb 2024: An employee can be specified per process notice, PO management, EDI (see below QR24/02)

-   **ON or > 4** - Inside sales employees of the order customer in the market partner master data (mp.innenmanr)
-   **1:** User (kauf.eusr)
-   **2:** Person in charge (kauf.abvertr)
-   **3:** Sales representative (kauf.vertrerloe)
-   **4:** Department employee of the customer for the order (abteilung.manr) – starting in Feb 2024) (see below QR24/02)

Per PO item, it is checked whether the PO item has an order reference. If this is the case, it is checked whether the order is on delivery type "drop shipment". Here only the delivery type of the order not that of the relevant order item is checked. If this is a "drop shipment", no e-mail will be sent.

If it is not a drop shipment, then it is checked whether the planned goods receipt date is earlier than the delivery date of the order. If the planned goods receipt date is on the same day or later than the delivery date of the order, the appropriate e-mail ID 41 is sent.

Starting on 05/23/2024 // alcib- 13.04.17743
The check with regard to the delivery date of the order has caused too many messages and was not goal-oriented. Therefore, the check has been changed. Now it is only checked whether the new goods receipt date is in the future with regard to the old goods receipt date.

With appropriate system configuration, it is also possible to activate a customer-specific logic which, prior to sending the email,
-   checks whether the e-mail should actually be sent
-   compiles an individual text for the e-mail.

For this, the stored procedure (SP) "cumailsp41" is called.

If this SP is not present or was created with the incorrect number of parameters, the default e-mail is sent. If the SP encounters a different error than SC= -674, then an error e-mail is sent to the defined employees. In the first parameter, the SP returns whether an e-mail should be sent, and in the second parameter the mail text. The mail subject is always populated in the program with text no. 31553: "Change of delivery date in the dispatch notice".

The default mail text is populated with text no. "31554: "The delivery date of the order <ordernr> must be changed!".

Starting with QR 23/10:
Text no. 38324: "The goods receipt date of the PO <PO number> has been postponed, therefore the delivery date of the order <Ordernumber> must be postponed!"

**The SP is called with the following parameters:**

-   **INTEGER:** external order number (kauf.auftrnr)
-   **SMALLINT:** internal item number in the order (kpos.posnr)
-   **INTEGER:** external number of the PO (kauf.auftrnr)
-   **SMALLINT:** item number in the PO (kpos.posnr)
-   **INTEGER:** new PO date
-   **INTEGER:** old PO date

**The SP must return the following data:**

-   **SMALLINT:** 0, if the mail should not be sent
    not equal to 0 if it should be sent
-   **CHAR(1500):** The text that should be sent in the mail.

For performance reasons, the existence of the respective SP is noted. If it is not present, there is no further unnecessary call of the SP. If the SP is deleted in ongoing operation - and even if only for a brief time, for a change - this causes an error. In both cases, A+W Enterprise must be restarted.

[AW-137151] // October 2023
The message is now also sent if the planned goods receipt date is changed manually in the PO management (Purchasing - PO Management).

If in an existing PO the date is postponed manually (PO management) or via notice, then the status 204 (WARENEINGANGSTERMIN) is reported to the PO and in the order. This status is also transferred if the PO arose from the internal transfer. This status can be seen in the PO and in the order under document information.

Furthermore, the date postponement via dispatch notice can be seen in the delivery date postponement log of teh PO and the dispatch notification itself is noted in the change log of the PO and the order.

Analogous to the date postponement via dispatch notification, for the postponement in the PO, the system message 41 is sent. Via the environment variable AVISE_MAIL, the recipients of the e-mail can be defined separately for dispatch notification and PO management. If no separate configuration is done for the PO management, the configuration of the dispatch notification applies.

The characteristic of the environment variable AVISE_MAIL has been changed, in that 2 parameters can be defined separated with "|" (pipe). The first parameter specifies the recipient for the change under dispatch notification and the second parameter for the change in the PO management. If only one parameter is specified, it applies for both.

If the status 204 - goods received date is transferred to the upstream distributor, the sending of the e-mail ID 95 can be configured there using the System menu.

For more precise information, see configuration instruction "EN-CONFIG-A+W Enterprise System" section "Messages" and section "" and "EN-CONFIG-A+W Enterprise" section "Messages".

**Starting with QR24/02 (February 2024)**

**Expanded control of the information about manual changes to the planned goods receipt dates**

The environment variable AVISE_MAIL has been expanded and the application standardized.
The environment variable can now accommodate up to 3 values separated by "|" (pipe).

The first value is used if the goods receipt date is changed on the "Notice" dialog.
The second value is used if the goods receipt date is changed via the "PO management" dialog.
The third value is used if status is transferred about a change of the goods receipt date is transferred via EDI from the production client to the trade client.

If the 2nd or 3rd value is missing, the first value is used instead.

| Value | Message Number | Default Message Recipient |
| :--- | :--- | :--- |
| 1 | 41 and 95 | user (kauf.eusr) or for eusr=-1 like 4 |
| 2 | 41 and 95 | Person in charge (kauf.abvertr) |
| 3 | 41 and 95 | Sales representative (kauf.vertrerloe) |
| 4 | 41 and 95 | Department employee of the customer for the order (abteilung.manr) |

With AVISE_MAIL = 4, the recipient is determined via the customer of the order's department (kauf.kunr -> mp.abtnr -> abteilunge.manr). If no assignment is found, then the user (kauf.eusr) is defined as recipient.

Furthermore, the determination is expanded for the variant AVISE_MAIL = 1. Thus, for all orders that have "System2 (-1)" as user (EDI, online), the recipient is also determined via the customer's department.

## 29. Finished products stock

The finished goods stock in A+W Enterprise has absolutely nothing to do with the "Stock" module. The finished goods stock is a kind of disposition stock for goods that are ready to deliver to the customer. Goods in the finished goods stock always have a relation to the customer order. The finished goods stock provides an overview of the whereabouts of the goods at all times

The functionalities of the finished goods stock are linked to many modules of A+W Enterprise (dispatch control, incoming goods). For this reason, there are overlaps with the respective module documentation.

### 29.1. Configuration

**OHNE_FERTIGWARENLAGER (client reference: no)**
Switches off the booking from the finished goods stock.

**FERTIGWARENLAGER_MIT_VLS (client reference: no)**
The booking to the finished goods stock is made via the advance delivery note. At ADN goods are booked on "trucks" and only booked out of the site. But they are in FG stock with target site=-1. Only DN books out the records with destination site=-1.
If no ADN is generated for the order, the data is output directly from house X for the DN. Source of error: Partially ADN and then completely LS not from shipping.

**LAPFERTWBPROTO_OHNE_KST (client reference: no)**
The variable deactivates the query for the missing cost center and the missing reason in the case of manual back bookings in the finished goods stock

**LAPFERTWBPROTO_WE_STORNO (client reference: no)**
(case #200332): If this environment variable is set, if the quantity of an item in an existing goods receipt is reduced, a reason for this reduction can be entered. If a reason is entered, it is stored in the finished goods stock log (lapfertwbprot.buchtext).

**WAEIN_LAPFWLAGER_DATUM (client reference: no)**
(Case: #200054): If this environment variable is set, only users with write right DIWR within the automatic and also within the manual incoming goods generation can backdate the incoming goods date into the past.
Furthermore, this date is transferred instead of the current date to the finished goods stock log (lapfertwbprot.mandatum).

**LAPOOL_VERPACKT_DATUM (client reference: no)**
If this variable is active, the functions "Check missing quantities" and "Correct packed quantities" are used in shipping to be more restrictive.

For the missing parts check, the booking date can only be changed if the user has the LAVD right, but only in the past.

For "Correct Packed Quantities", the booking date and booking text are mandatory.

### 29.2. Dispatch control

#### 29.2.1. Delivery note

For the delivery note creation, a corresponding entry was made in the finished goods stock. Here, the arrival date (LAPOOL.ANKUNFT) will always be used as the booking date.

If an order is locked during delivery note creation but the corresponding finished goods stock booking has already been made, this booking will be cancelled automatically. Now, this booking also uses the arrival date. For the finished goods stock booking that is triggered when a delivery note is cancelled by hand, the current date is used as booking date (LAPFERTWBPROT.MANDATUM).

For the delivery note creation in dispatch control, a restriction check was implemented, which checks whether the order's arrival date falls inside or outside a closed period. If the date falls within a closed period, the delivery note cannot be created. This restriction check can be enabled with an environment variable. The check is then active for both delivery note creation in the foreground, and in the background (AUTOLS).

When a delivery note is cancelled, the reason for the cancellation is transferred to the finished goods stock log (LAPFERTWBPROT.BUCHTEXT).

If an order that has already been reported complete is cancelled in dispatch either by means of order cancellation or cancellation by transfer (internal or customer cancellation), the reason for the cancellation or the transfer will be passed on to the finished goods stock log (LAPFERTWBPROT.BUCHTEXT).

The environment variables PERIODENPRUEFUNG (ON/OFF) and LAPOOL_LS_PERIODENPRUEFUNG (ON/OFF) must be enabled for the restriction check at delivery note creation.

#### 29.2.2. Packed message

Dispatch control offers two functions for passing on the 'packed' report to the finished goods stock log: *Check missing quantities*, and *Correct packed quantities*. A new environment variable can be used to enable a different behavior for bookings in the finished goods stock log. Previously, the current date was always transferred as the booking date. Generally, the booking date may not be in the future and for past dates, the user has to have write rights for the new user right LAVD.

The check for missing quantities offers a special column, Buch.datum for entering a different booking date. The date must not fall within a closed period. When the date is changed, it can be passed on to the following items. After that, the booking date is transferred to the finished goods stock log, item by item.

Function *Correct packed quantities* is available on item level. When you change the quantity in column Packed, a booking dialog appears where you can enter the booking date, the cost center, and booking text. *Booking date* and *booking text* are compulsory fields. The booking date is preset by the present date. The amended booking date must not fall within a closed period. When you quit the dialog, the entries will be transferred to the finished goods stock log.

The environment variable for enabling the logic in dispatch control is called LAPOOL_VERPACKT_DATUM. The environment variable PERIODENPRUEFUNG must be set to the end of period for this check.

Environment variable LAPFERTWBPROTO_OHNE_KST must not be set.

If data is manually reduced in the finished products stock because of a correction of packed quantities, rebooking to truck in the via plant site, or because deliveries cancelled at the via plant site, an additional menu will ask for the reason, date, and cost center for the booking. This data is visible in the booking log.

If the booking refers to several order items, the query screen will open for every item; the data will be preset with the first data entered. This logic can be disabled.

#### 29.2.3. Inventory, finished products stock

With the "Finished products inventory" menu on the shift menu, you can lock the finished products stock during inventory. During that time, all bookings are kept in the report server until the finished products stock is released again after inventory. The list of data is accessible during inventory, however. The system will only inform you that inventory is under way. The "Inventory log" shows the progress of inventory. Who has started and finished the inventory. The inventory can only be started and ended for the current site. The log shows the data for all internal sites.

### 29.3. Receipt of goods booking

A new environment variable `WAEIN_LAPFWLAGER_DATUM` can be used to enable a different behavior for bookings in the finished goods stock log after manual and automatic receipt of goods. Previously, the current date was always transferred as the booking date. With the new logic, the date entered by the user will be transferred to the finished goods stock in case of automatic receipt of goods and the customer's requested date in case of manual receipt of goods. If this logic is active, the following rules apply for the input of goods received:

-   Receipt of goods with a date higher than the present date cannot be entered.
-   The right DIWR is required to antedate the receipt of goods.
-   Antedating the receipt of goods will produce a security check.

#### 29.3.1. Manual creation or cancellation of receipt of goods

When goods received are cancelled, the reason for the cancellation is transferred to the finished goods stock log (LAPFERTWBPROT.BUCHTEXT). An environment variable LAPFERTWBPROTO_WE_STORNO can be used to enable a logic that allows you to enter the reason for the change if the item quantity of an existing receipt is changed. It is also transferred to the finished goods stock log (LAPFERTWBPROT.BUCHTEXT).

### 29.4. Stock removal bookings

In addition to the stock removal, the module "order-related stock removal" also produces a finished report for header parts and thus an associated finished goods stock receipt.

See also EN-CONFIG-A+W Enterprise Interne Mandantentrennung.pdf

## 30. Stock

### 30.1. Item master data

This is the master data in the "Stock"module and not the general article master data in the main module.

In the article master data, you can define the inventory limits and the available variants. The inventory limits are required for the automatic triggering of PO proposals (see section"Triggering PO proposals").

#### 30.1.1. Variants

The use of dimensional variants in stock is subject to some settings and relationships.
See section "Keys – Product keys – Dimensional variants"

The settings in the dimensional variants and the configuration of the document entry with regard to physical quantity directly influence the display of the inventory forecasts.

**"Variable variant"**

The variable variant is always required if an article is not removed as a piece from the stock and is also not entered or removed as piece. This is the case with colors, for example. Even if no fixed packages (e.g. 1 can with 10 liters) are kept in stock, but rather the total quantity in liters (or kilograms), the variable variant is required. It is used for incoming goods booking for stock goods, removal from production, and for cost calculation.

For this, the environment variable WLDISPO_VARIABLE must be used.
See also "Size variants in stock"

### 30.2. Room master data

Menu element "Master Data - Room" - creation of a new warehouse
Field "In-house": company for multi-site work - currently not evaluated

-   Division not required according to physical stock - logical stock possible
-   normal stock: - loose stock
-   High-rack warehouse: - Special Bamberg; transfer of a file to an external warehouse system
-   Rack stock: see „Rack-related incoming goods - rack stock"
-   Size/costs: - only information

#### 30.2.1. Box stock

Only complete boxes of an article (e.g. stock sizes) are entered in the box stock. Only complete boxes can be booked in and out. If a lite should be removed from a stock size box (opening a box), an entire box must be resolved (removed) and booked to another stock (e.g. normal stock).

For the use of automatic and semi-automatic (delivery note/manual order-related) it should not be entered as default stock in the article master data.

#### 30.2.2. Slot warehouse

For this stock type, booking of a stock slot assignment is required.

### 30.3. Booking of incoming stock

For manual incoming stock, the price from the article supplier assignment (artliefzu) is used. If a variant is booked, then from the article-variant-supplier assignment (artfarbzu, artvarzu). If you remove the supplier from the booking dialog, no price is determined.

### 30.4. Stock inventory

**How does inventory in the stock work?**

When opening an inventory, all inventories of the associated stock are copied to an inventory stock (stock number * -1)(The tables are: wls, wlx, wlsv, wlxv, wlxifo, wlfach). The inventory differences can now be recorded in this stock (negative stock number).

At the same time, incoming and removal bookings can be made in the normal stock. Here you only need to be careful that these bookings are considered when counting.

If the recording of the inventory is complete, the inventory completion can also be initiated on the inventory screen. Here, the following actions take place:

1.  The positive stock is deleted with reference to the tables named above.
2.  The negative inventory stock is copied to the positive stock number.
3.  All bookings that were made since the beginning of the inventory in the positive stock are made again now.

It is also possible to cancel an inventory. Here, the negative inventory stock is just deleted with the associated bookings.

During inventory completion or inventory cancellation a log record with "status 923 - inventory completion" or "924 - inventory cancellation" is written to the stock history (stock log).

### 30.5. Inventory evaluation

#### 30.5.1. Average price

In the stock, there is an average price. The average price is determined by dividing the total value (wlx.g_preis, wlxv.g_preis) after a booking by the total stock (wlx.g_best, wlsv.g_best) of a booking. This is done on the article level as well as on the variant/color level.

In case of negative stocks, the average price can no longer be calculated correctly. Here, the data must be corrected by an inventory.

You can prevent negative stocks with the environment variable "WL_KEINE_NEGATIVEN_BESTAENDE".

The total stock of the article (wlx.g_best) must match the total of the total stock of the associated variants (wlxv.g_best). If this is not the case, you will have different average prices for the article and the variants. To clean this up, you must also conduct an inventory.

The tookings can be made in wlh_ok and in wlprot. If you haven't done an inventory in a long time, of course it is difficult to find an incorrect booking in the quantity of bookings."

With appropriate configuration, the stock average price is used for the material cost calculation.
In addition, there is a stock evaluation according to the FIFO and LIFO method. These values are currently calculated but not used for the cost calculation.

#### 30.5.2. FIFO and LIFO values

**FIFO (first in, first out)**

Goods are received in the following sequence:

| Description | Calculation | Result |
| :--- | :--- | :--- |
| Receipt of goods dated 20.08. | + 10 pcs. at 5,- € each | 50,- € |
| Receipt of goods dated 05.09. | + 20 pcs. at 10,- € each | + 200,- € |
| **Total** | | **250,- €** |
| Outgoing stock dated 08.10. | - 10 pcs. at 5,- € each | - 50,- € |
| **Stock on hand (by FIFO)** | | **200,- €** |

**LIFO (last in, first out)**

Goods are received in the following sequence:

| Description | Calculation | Result |
| :--- | :--- | :--- |
| Receipt of goods dated 20.08. | + 10 pcs. at 5,- € each | 50,- € |
| Receipt of goods dated 05.09. | + 20 pcs. at 10,- € each | + 200,- € |
| **Total** | | **250,- €** |
| Outgoing stock dated 08.10. | - 10 pcs. at 10,- € each | - 100,- € |
| **Stock on hand (by LIFO)** | | **150,- DM** |

Of all the following methods, only LIFO is valid for tax purposes. The system records the average price, the maximum and the minimum price. Two other stock monitoring methods are LOFO (lowest in - first out) and HIFO (highest in - first out). As these methods are invalid for tax purposes, ALCIB does not support them.

The calculation of the FIFO values is done using the table wlxifo. There, on stock receipts, new records with b_menge = quantities received and FIFO + LIFO quantity = 0 are written. For stock removals, the oldest record in the table for the corresponding key (article, stock, color, variant, box) is searched for, which has the FIFO quantity < b_menge. The value found there is then used for the calculation. If the quantity removed is greater than the difference between b_menge and FIFL quantity, the next record with the same criterion is searched for.
The LIFO process runs similarly. Only that here the newest records are searched for.
The FIFO value determined using this process is then writtten to wlprot.

#### 30.5.3. Backdating of an inventory evaluation

An inventory was completed on 12/31/2022. Now, this inventory should be provided with additional values after the fact. The current inventory of articles that must be evaluated is different today.

This function is not available. A completed stock inventory cannot be reevaluated after the fact.

### 30.6. Correction of stock bookings

#### 30.6.1. WL_KORR_DURCH_GEGENBUCH

In principle, there is a distinction between whether the variable WL_KORR_DURCH_GEGENBUCH is set or not. If this variable is set, then corrections in stock bookings are made with the difference and opposite. BSP: By accident, 100 pieces were removed from stock, but only 10 were supposed to have been removed. With this process, 90 pieces are booked back in. This procedure is actually easy to implement, but it causes a falsification of the assessments according to FIFO, LIFO, and average process.

#### 30.6.2. Standard procedure

If this variable is not set, the following logic holds. In the tables wlx_m, wlxv_m, etc., cyclical inventory back-ups are created. These tables have the same structure as the original tables; only the fields savetime and savedate, where the back-up time is saved, were added. A maximum of 2 complete back-up inventories are kept. With the command wlspec 0, a generation of the back-up inventories can be initiated directly. No backups can be created if an inventory is open or if there are open bookings. Important for this procedure is that the backups are kept current and that no records from wlh_ok are deleted.

Based on these back-ups, all bookings can then be corrected, which lie between the oldest back-up state and the current date.

The correction works as follows:

-   The booking record to be corrected is written with negated booking status and with the corrected booking price and with the corrected booking quantity in the table wlh. The original time of the booking creation (field time) is retained.
-   The stock booker then processes this record and detects from the negative booking status that this is a correction.
    -   It thus shifts all data for the combination of article number, stock to the stock + 100.000 (tables wlx, wlxv, wlfach, wlgest, wlxifo, wlprot for all records with timestamp > then the backup time in the_m tables).
    -   Then the latest backup in the_m tables is determined, which is older than the backup to be corrected. From this the backup records for the article/stock combination in question are copied back. (tables wlx, wlxv, wlfach, wlgest, wlxifo, wlprot with timestamp - see above)
    -   The record to be corrected in wlh_ok is set to error -1000.
    -   Then all bookings for the article/stock combination with booking time >= backup time and error != -1000 are pulled back into the table.
    -   The corrected record is written with positive B status and new quantity or new price into the table wlh.
    -   Then the stock booker writes a final correction record with B_status 101 into the table wlh. This has as waittime the time of the last record, which was obtained from wlh_ok. In addition, it is set to error -5, so that it is processed only after the last booking re-presented. The record contains in b_menge the difference between the B_menge of the original booking and the corrected booking. Afterwards, this difference must be identical to the difference between the backed-up total quantity in stock + 100,0-00 and the total quantity that arises after executing all re-presented bookings.
-   Now all bookings are processed individually by the stock booker.
-   In the end, for the processing of the record with status 101 it is checked whether the differences mentioned above match.
    -   If yes
        -   The records with stock number + 100,000 are deleted
        -   The final correction booking is written with error -1000 to wlh_ok.
    -   If no
        -   The records in the tables wlx, wlxv, wlfach, wlgest, wlxifo and wlprot (with timestamp limitation) will be deleted for the current article/stock combination.
        -   The records backed up with stock + 100,000 are pushed back.
        -   The correction record in wlh_ok remains with error - 1000, so that it makes no sense to try making the correction again since this booking would no longer be considered.
        -   The final correction record is set to an error status.

### 30.7. Stock filling orders

#### 30.7.1. Incoming stock booking for packing notification

Until now, the incoming stock booking was always carried out for stock filling orders when the completion report was made. The logic was based on the assumption that in this case the goods produced would be placed directly to the stock without any packaging notification. Sometimes, however, it is better for organizational reasons to carry out the incoming stock booking with the packing message, then, for example, breakage messages are no longer relevant for completed lites.

Breakage reports from the shipping area of A+W Production are not taken into account by this logic.

The incoming stock booking is made using status 415 "Incoming (packing message)" and no longer via 403 "Incoming (completion report)".

**Configuration**

The WL_STOCKORDER_WHENPACKED switch can now be used to activate the incoming stock booking via the packing message. This setting is global. It affects all incoming stock bookings for stock filling orders. Presently, it cannot be set differently for individual sites of an internal multi-site system.

The variable PMVERSANDSTUUER may not be set here, since this leads to a packing message being carried out directly with the completion report

The variable AWC_IGNORE_PACKINGMESSAGE must not be set.

#### 30.7.2. Manual entry

If an order with the customer who corresponds to the current site (xhaus) is entered, now the associated order is automatically converted to "Stock order". All items entered are then changed to supply type = PRODUCTION, regardless of whether the supply type "PRODUCTION" is provided for these articles in the master data. Similarly, there is no check whether the supply type "STOCK" is defined for the article entered. Exceptions are only the items with supply type = NONE.

If in such a stock order an article is entered that is not known in production, under some circumstances, the entire order cannot be scheduled for production planning.

Also with reference to another order/quotation of another customer, both the order type and the supply type of all existing items are converted. For the determination whether the customer corresponds to the current site, the data is determined from the table xhaus. Thus, the evaluation is positive if an entry in the table exists with kunr=<Customer number from the order> and hnr <Company number from the order>. Since the evaluation depends on 2 criteria, for the change of the company number it is also checked whether this is an order for the current site. If a subsequent change of the company number makes the initial conversion to "Stock order" moot, now it is asked whether the order type = "Stock order“ should be retained. If so, the supply types of the items are retained. If not, these are determined anew according to the existing logic on request. If an order for any other customer with the reference to the "Stock order" is generated, it is also queried whether the type of the order should remain. If this is not desired, then in this case only the type is converted; the supply type in the existing items and those taken over is not determined anew. There is also no determination of the supply types if the order type has been changed manually.

LAGERAUFTRAG_ERWEITERT = ON

### 30.8. Report of stock plates

#### 30.8.1. Motivation for this function description

In A+W Enterprise, the stock plates are managed in A+W Enterprise Stock. In order to keep inventory as precise and automated as possible, the stock removal booking by production of stock plates can be done based on the cutting data.

#### 30.8.2. Configuration

See EN-CONFIG-A+W Production.docx - Reporting of stock plates

The reporting must be switched on in XOPTON.CFG:

**In A+W Enterprise**
PMXTVRLOESCHOPT

By default, in the past data from wlppms was not taken into account for the forecast and also not removed. With the new environment variable for A+W Enterprise "WL_WLPPMS_ADAT_SHIFT" it is also possible to consider data from the past. This variable is filled with a numeric value if you want to increase the starting date for selecting the stock forecast data from table wlppms (Stock > Information System > Forecast) by 1 or more days. The selection of the data from wlppms is selected with wlppms.a_datum >= today. Now the selection can be shifted with the value from the variable into the past. (wlppms.a_datum >= today - value from WL_WLPPMS_ADAT_SHIFT)

#### 30.8.3. Resolve reservations (#289178)

The reservation is canceled by adjusting the forecast data in table WLPPMS. For each XTV feedback, the corresponding records in WLPPMS are updated for all transferred BOM elements. The booked quantity and quantity are adjusted according to the transmitted data and the status is set. As long as the booked quantity (WLPPMS.A_VERBUCHT) is smaller than the expected quantity (WLPPMS.B_ANZ), the status (WLPPMS.STATUS) is set to 1 ("partially booked"). When the booked quantity has reached the value of the expected quantity, the status is set to 2 ("completely booked").

To adjust the forecast data, only the BOM element transmitted with the XTV confirmation is considered. The entire BOM below the tuple is not checked for entries in WLPPMS.

**Examples:**

-   If an item article is reported as finished (produced), the parts below are booked out of wlppms accordingly.
-   If an item article is reported packed, the parts below are only cleared from wlppms if the packed quantity is > the finished quantity.

**XTV feedback when using the A+W ERP Stock Service**

With use of the Stock Service, previously the XTV reporting had to be deactivated since otherwise removals from coupled stocks were made twice.

The XTV reporting can now be used together with the Stock Service - for the stock booker now checks the stock properties for removals with status 68 (PMS_ABGANG_EXT). If the stock from which the removal should be made is a portal stock (WLRAUM.INTERFACE = 2), no stock removal is made. In this case, the stock in question is a synchronized third-party stock that is removed by the Stock Service. A corresponding entry in the stock booker log documents that this removal is suppressed. The record is then deleted from the table wlh.

### 30.9. Size variants in stock

#### 30.9.1. Motivation for this function description

In A+W Enterprise, articles can be created as dimension, color or size variant. In order to treat articles with size variants correctly in the stock, several settings are required, which will be summarized here. The configuration will be explained using the example of the spacers.

#### 30.9.2. Item master data

Normally, spacers are defined as BOM elements in the frame. Here, the item structure of the spacer is described via the frame for the IG.

**Spacer**
In A+W Enterprise master data – item the spacer is defined as a part of item type 220 - spacer. In this configuration, the quantity unit = 3 - length (mm) and the variant is on size. Whether the quantity unit 1 linear meters or 3 millimeters is set doesn't matter at all for stock-keeping. Which of the two quantity units is used decides in which quantity unit the article is ordered. In the "Color/size variant" field, you can then use F5 to assign the size variants and their supply type (stock) (Master data - Keys - Products – Variants – Sizes). If you would also like a forecast and if necessary an automatic removal, the inventory change for the item must be entered accordingly (e.g. completion report - see master data manual).

The spacer must be saved in the article master data as follows:

-   **Identification:**
    -   Article type = 220 spacer
-   **Phys. properties:**
    -   ME = 1 length (Ifm) or 3 length (mm)
    -   Color/size variant = sizes
-   **Supply:**
    -   Supply type = 1, 4, 5 or 7
-   **Stock:**
    -   Default stock should be defined
    -   Stock change = completion report

Furthermore, for the spacer an item dimensioning (Shift + F4 - Dimensioning - Item dimensioning) must be stored. This item dimensioning is important so that the thickness (AIR) from the item is inherited by the spacer.

**Figure 19 Article dimensioning in master data**

**SPACER**

In the master data - item the spacer is defined as a part of item type 210 - IG spacer. The spacer is also defined as "Size" in the "Color/size variants" field and assigned the appropriate size variants (production) with F5 (Master Data - Keys - Products – Variants – Sizes).

In the BOM of the frame, the spacer is attached with Anz1 = 1 and Anz2 = 0 and an appropriate inheritance formula. Important here is the inheritance of $3, in which the thickness variant is inherited.

**Figure 20: Dimension conversion dialog (formula for spacer thickness)**

If for the spacer with size variants variant-dependent prices should also be calculated, then the required settings must also be made for the spacer the item dimensioning (such as spacers) and also under price details (Shift +F4 - Price details).

**IG**
In the BOM of the IG, the frame is attached with the appropriate inheritance formula.

**Figure 21: Dimension conversion dialog (formula for spacer)**

#### 30.9.3. Stock - item master data

Under Master Data - Item, for the spacer (not the frame), the appropriate inventory data for the automatic order is entered.

The variant is "variable"

**Figure 22: Article master data in stock**

### 30.10. Triggering PO proposals

Within the A+W Enterprise stock module, it is possible to trigger PO proposals for filling up the stock based on forecast quantities. Whether this happens depends on some prerequisites.

#### 30.10.1. Prerequisites

The environment variable WL_PROG_BEST controls whether PO proposals should be triggered. If the variable is active, PO proposals are triggered. The setting is database-wide and not site-specific.

**WL_PROG_BEST:**
PO proposals are triggered based on a forecast by the stock booker.

If a PO proposal should be triggered for an article, it must have the supply types Stock - Production or Stock – PO in the master data. At the same time, a default stock and a resupply time have to be entered. Whether an inventory forecast is done for an article depends on the setting of "Change in Stock" in the A+W Enterprise article master data (master data - article tab "Stock")

In the stock master data (stock module), inventory limits have to be entered (see also section "Purchase order forecast without alarm stock").

Furthermore, the PO quantity process has to be defined via the environment variable WLBMV (see section "PO quantity process").

A PO forecast based on square meters is also possible for box stock. The inventory limits in square meters are maintained per article, stock, and variant.

#### 30.10.2. PO quantity process

The PO quantity process specifies according to which method the quantities for PO proposals for filling up the stock are calculated. The PO quantity process is set database-wide, not site-specifically.

**WLBMV:**
This variable activates the warehouse PO quantities procedure:
1.  Standard quantity
2.  Quantity booked
3.  Up to maximum stock
4.  Once to maximum stock (trigger new purchase orders only when goods receipt is booked)
5.  N * Standard quantity up to maximum stock

Within the PO forecast, the forecast stock inventory on a defined date is compared to the expected stock inventory. What the expected stock inventory is defined via the environment variable WL_PROG_BEST_ALARM. By default, the minimum inventory for triggering stock filling POs is used. If, however, the environment variable WL_PROG_BEST_ALARM is activated, the alarm stock is used instead of the defined minimum inventory.

**WL_PROG_BEST_ALARM:**
The forecast PO in the warehouse refers to the alarm stock and not to the minimum stock.

#### 30.10.3. Default quantity (WLBMV=1)

In A+W Enterprise, the default quantity for re-supply is stored under Master Data – Article.

For articles that are produced via the company's own production for stock (supply type Stock - Production), they are entered on the Supply tab in the Default quantity field. With this supply type, the default quantity cannot be maintained according to the variant (#456862).

For articles whose inventory is filled up via POs to stock (supply type Stock – PO), the default quantity is maintained in the Article – Supplier allocation. With this variant, it is possible to define this variant-specifically.

The default quantity cannot be stored site-specifically

Generally, it is the case with this procedure that the default quantity determined is always used. However, if the stock again falls below the alarm stock, including an already existing purchase order proposal, the purchase order proposal is deleted and the double quantity is entered.

#### 30.10.4. Quantity removed (WLBMV=2)

Precisely the quantity of the last stock removal is ordered.

#### 30.10.5. Up to maximum stock (WLBMV=3)

The stock is filled to the maximum. After this, the difference between actual stock and maximum stock is ordered as long as the alarm stock is not underrun.

#### 30.10.6. Once up to maximum stock (WLBMV=4)

When the alarm stock is underrun, the exact quantity required to reach the maximum stock is ordered.

POs are only triggered if good receipt is booked. If, however, within the re-supply time the forecast stock including the PO triggered drops below the alarm stock, another PO proposal is triggered.

#### 30.10.7. N * default quantity up to maximum stock (WLBMV=5)

In A+W Enterprise, the default quantity for re-supply is stored under Master Data – Article.
For articles that are produced via the company's own production for stock (supply type Stock - Production), they are entered on the Supply tab in the Default quantity field.

For articles whose inventory is filled up via POs to stock (supply type Stock – PO), the default quantity is maintained in the Article – Supplier allocation. With this variant, it is possible to define this variant-specifically.

The default quantity cannot be stored site-specifically

Generally, it is the case with this procedure that the default quantity determined is always used. However, if the default quantity is not sufficient to reach the maximum stock, a multiple of the default quantity is ordered.

#### 30.10.8. Purchase order forecast without alarm stock

In addition to standard articles that you would always like to have on hand, there are also non-standard articles.
These should only be kept in stock if they have actually been used up. You won't want to maintain an alarm stock for such articles since these articles would otherwise be permanently in stock. A PO proposal should only appear if there is an actual need, that is, an order.

#456796 For articles for which no stock on hand is to be kept in the warehouse, there is now the possibility to define an alarm stock level of 0. However, a maximum stock on hand level must be specified and the switches WL_PROG_ALARMBEST_NULL and WL_PROG_BEST_ALARM must be activated.

If there is no stock on hand for the article in question, the purchase order forecast determines a negative forecast stock on hand up to the supply time. Since this stock on hand is thus smaller than the alarm stock, a purchase order request is generated according to the set procedure (WLBMV).

A maximum stock level is nevertheless required so that, on the one hand, up to this level can be replenished (WLBMV = 3, 4 or 5). On the other hand, this serves to identify the articles that are to be forecast using this method. This avoids unwanted purchase order proposals for articles for which no stock limits have been defined.

If a maximum stock is defined in sqm < 1, then only as much is ordered as is actually required. However, this is only possible across variants. The maximum stock for a specific variant is always at least 1 unit.

#### 30.10.9. Variant-precise PO forecast:

Environment variables:

**WLDISPO_VARIABEL:**
If the variable is active, the stock items in the order are transferred to table wldispo as 'variable to be debited'. This does not debit the variant (piece), but the concrete dimension!

Is the forecast stock of the variant-precise PO forecast less than the alarm stock or the minimum stock?

The forecast stock is determined based on unbooked receipts of goods and is composed of:

| Component | Description |
| :--- | :--- |
| Stock on hand | |
| + Total of all unbooked receipts of goods based on stock POs (date-dependent) | – table wldispo |
| - Total (from today up to the replacement time) of the variant-related order removals (manual or delivery note-removal) | |

> Only articles whose stock change is set to manual or delivery note-removal.

Only articles whose stock change is set to manual or delivery note-removal.

In this document, WL_PROG_BEST = ON, WL_PROG_BEST_ALARM = ON and WLDISPO_VARIABEL = ON

#### 30.10.10. Order forecast for fixed articles

[AW-127400] January 15, 2023

If for fixed articles the inventory change "AWP" or "*/AWP" was selected, it could happen that order-releated, e.g. for QM articles and the quantity in QM and not, as required for fixed articles, wlppms was stored in pieces in the table. However, since for such articles pieces are always saved in the forecast, this causes problems with the inventory forecast. This program behavior has been corrected. For fixed articles, the forecast data is always written in number of pieces with inventory change AWP.

In addition, in the stock check during import, a change was made, the effect of which is that dimensioned articles are also treated as piece articles.

For correction of old data: From our point of view, it must be sufficient for all fixed articles (article prodbemass>0) in wlppms to set the b_menge (quantity in quantity unit of the article) = the b_anz (quantity).

#### 30.10.11. PO forecast for color or thickness variants with inventory change AWP

QR2506

Articles with color or thickness variants could thus far be incorporated into the nightly PO forecast via A+W Production with use of a forecast type. For this, there was previously only one overarching forecast for the entire article, which makes no sense for different thicknesses or colors.

The program behavior has now been changed so that this is possible. In stock, these articles, e.g. spacers, are then stored and booked variably.

#### 30.10.12. Environment variables

**WL_PROG_BEST (stock reference: no)**
PO proposals are triggered based on a forecast by the stock booker.

**WLBMV (client reference: no)**
This variable activates the warehouse PO quantities procedure:
1.  Standard quantity
2.  Quantity booked
3.  Up to maximum stock
4.  Once to maximum stock (trigger new purchase orders only when goods receipt is booked)
5.  N * Standard quantity up to maximum stock

**WL_PROG_BEST_ALARM (client reference: no)**
The forecast PO in the warehouse refers to the alarm stock and not to the minimum stock.

**WL_PROG_ALARMBEST_NULL (client reference: no)**
If this variable is activated, articles with minimum or alarm stock = 0 will also be considered in the PO forecast. This can be used if, for example, stock sizes should only be ordered if there is a need (order-related). Generally, however, you do not want to have stock on hand for these articles.

### 30.11. Spacers/Thiokol in stock

#### 30.11.1. Spacer

The spacer should be removed from the stock by linear meter. The completion report in AWP triggers the stock removal. See also 18.3

The spacer must be saved in the article master data as follows:
-   **Identification:** article type = 220 spacer
-   **Phys. properties:**
    -   ME = 1 length (Ifm)
    -   Color/size variant = sizes
-   **Supply:** Supply type = 1, 4, 5 or 7
-   **Stock:**
    -   Default stock should be defined
    -   Stock change = completion report

**Figure 23: Master data: Identification tab, Phys. properties, stock and <F4>->Variant info**

For the correct calculation of the number of linear meters per variant, the formula must be defined in the BOM of the IG frame.
The spacer is a child part of the IG frame.

**Figure 24 Article master for spacers**

**IG frame BOM:**

**Figure 25: BOM for spacers**

**Article sizes:**
Thus, this article receives $1, $2 and $3 from its parent.

**Figure 26: Article dimensioning for spacers**

**Formula 233:**
Example:
Item: IG with quantity = 10, width = 1000, height = 1000 and AIR=16.
$1 = (2 * 2000) / 1000 = 4 m

**Figure 27: Spacer formula**

**Stock info system per variant:**

**Figure 28: Info stock per variant**

There are 15,504.61 m of variant 16 mm.

**Out:**
The system calculates how many meters should be removed per item. It removes the stock. Afterwards, the system checks whether stock order should be generated.

Example:
Item: IG with quantity = 10, width = 1000, height = 1000 and AIR=16.
10 x 4 m = 40 m.
For the 16mm variant 15504.61 - 40.00 = 15464.61 m
Is 15464.61 <= 1m? Yes, a stock order is generated 9see stock order).

**Stock order:**
The variant-precise stock is the forecast stock (calculated in the night) or that after a removal. The system checks each size variant.
If the variant-precise stock <= stock <= alarm stock, a stock order is generated.

Example:
For the 16 mm variant, we have minimum = 100, alarm = 500, and maximum = 1000.
The quantity in the purchase order is:
-   For WLBMV = 1 (default quantity):
    This quantity is in detail (F2) of colors/sizes (Shift+F4).
    ⇨ E.g. purchase order quantity = 2000 m

**Figure 29: Article master data, <F4> Variant info, <F2>**

-   For WLBMV = 2 (quantity removed):
    Only for removal, not stock forecast.
    Example:
    Item: IG with quantity = 10, width = 1000, height = 1000 and AIR=16.
    10 x 4 m = 40 m.
    For the 16mm variant 440.61 - 40.00 = 400.61 m
    400,51 < Alarm = 400,51 < 500? Yes.
    ⇨ Purchase order quantity = 40 m
-   For WLBMV = 3 (up to maximum stock):
    ⇨ Purchase order quantity = 1000 m
-   For WLBMV = 4 (once up to maximum stock):
    A new PO is triggered only once the goods receipt has been booked.
    The system checks whether there is a goods receipt for the 16 mm variant.
    ⇨ Yes, no PO
    ⇨ No, PO quantity = 1000 m
-   For WLBMV = 5 (N * default quantity up to maximum stock):
    Example:
    If default quantity for 16mm variant is 300, the PO quantity is:
    N * 300 >= Maximal = 3 * 300 = 1200 m.
    N = 2 is not enough.
    ⇨ Purchase order quantity = 1200 m

**Goods receipt:**
On goods receipt, the system removes the stock.

#### 30.11.2. Drying agents

Drying agents are stored in the warehouse in 25, 140, and 600 g containers.
In the article master data, the drying agents must be stored as follows:

-   **Identification:** article type = 250 drying agent
-   **Phys. properties:**
    -   ME = 8 weight (kg)
    -   Dimensional variant activated
-   **Supply:** Supply type = 1, 4, 5 or 7
-   **Stock:**
    -   Default stock should be defined
    -   Stock change should be defined, e.g. delivery note

**Figure 30: Phys. properties for drying agent**

**Figure 31: Variant info for drying agent**

For the correct calculation of the number of kilograms, the formula must be defined in the BOM of the IG spacer.

**IG spacer BOM:**
