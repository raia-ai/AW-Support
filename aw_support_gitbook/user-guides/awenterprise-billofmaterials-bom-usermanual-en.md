---
title: "EN-UM-AW_Enterprise-Sales_4_5"
source: "EN-UM-AW_Enterprise-Sales_4_5.pdf"
tags: ["A+W Enterprise Sales", "Bill of Materials", "BOM", "Software Reference", "Muntin Entry", "Packaging Planning", "Product Structure", "Order Entry", "Sales Module", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the Bill of Materials (BOM) module within the A+W Enterprise Sales software, version 4.00. It details the functionalities for viewing, creating, and managing BOMs, including product structures, production sketches, and processing parameters."
long_description: "This comprehensive software reference manual provides an in-depth guide to the Bill of Materials (BOM) section of the A+W Enterprise Sales application, version 4.00. The document systematically walks users through the various dialogs, tabs, and fields related to BOM management. Key areas covered include the BOM View, which allows for examination of product structures and production sketches, and the Current BOM Level tab for editing individual articles and their properties. It provides detailed explanations of parameters for numerous processing types, such as edge work, drilling, tempering, and surface treatments like silk-screening. The guide also covers specialized functionalities like Muntin Entry for defining muntin patterns in insulated glass units, Stepped Entry for managing stepped glass, and Edge Allocation for shaped lites. Furthermore, a significant portion is dedicated to Packaging Planning, detailing how to specify sorting algorithms, rack types, and loading parameters to generate an optimized packaging plan. The final sections describe how to manage internal notes associated with documents, articles, projects, and market partners. Each function is explained with its corresponding navigation path, keyboard shortcuts, and technical database field information, making it an essential resource for advanced users, system administrators, and technical support staff."
---

# Bill of Materials (BOM)

---
## Software Reference

-   **BOM**: Opens the *Current BOM Level* tab on the selected BOM level and displays a list of all articles on this BOM level. Alternatively, you can use `<F5>` to open the *Current BOM Level* tab for the selected BOM level.
    ⇨ "BOM View – Current BOM Level" on page D-205
-   **OK**: Closes the BOM View dialog.

---

## BOM View – Product Structure

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > <F3> > Product Structure tab`

**Fig. D-80:** Product Structure

This tab displays the preview for the product structure in cross-section.

In the BOM view, the BOM is on the left side of the dialog and the *Product Structure* and *Production Sketch* are displayed on the right side of the dialog.

Use `<Shift>+<F2>` to change to the *Production Sketch* tab.
⇨ "BOM View – Production Sketch" on page D-203

The side with the sun indicates the outside of the product structure. On the right, the lites, spacers, foils, etc. are displayed. The numbering of the installation position is always counted from left to right, that is, the lite by the sun always has the installation position 1 or 2.
⇨ "Product Structure" on page D-200

### Footer

The buttons in the footer are described for the *BOM View - BOM Structure* dialog.
⇨ "BOM View – BOM Structure" on page D-199

---

## BOM View – Production Sketch

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > <F3> > Production Sketch tab`

**Fig. D-81:** Production Sketch

This tab displays the dimensioned product sketch for the item. Using this SN-Live sketch, you can check the correctness of the items entered and their processings.

In the BOM view, the BOM is on the left side of the dialog and the *Product Structure* and *Production Sketch* are displayed on the right side of the dialog.

Use `<Shift>+<F2>` to change to the *Product Structure* tab.
⇨ "BOM View – Product Structure" on page D-202

---

## Production Sketch tab

The production sketch displays the dimensioned sketch of the item with the processings. With a click on the sketch, you open an enlarged view of the sketch on the *SNLive Zoom* dialog. On this dialog, you can zoom in on parts of the sketch.

Depending on the configuration of A+W CAD Designer (Shapes), arrows are shown on the sketch that indicate the direction of the product structure in the cross-sections.

The descriptions and markings indicate the positioning and processing type, e.g. which edges of a lite are processed and whether the edges are ground or polished, etc. The markings of the processing that is selected on the *Parameters* tab are highlighted in red on the top-view sketch.

-   **H, H(n)**: Height of the lite. Depending on the shape, there are different specifications for the lite sides. The letter H means the total height and the letter H(n) means the partial height of H. The parameters are numbered consecutively. The number in the square brackets specifies the height of the lite side in millimeters.

-   **W, W(n)**: Width of the lite. Depending on the shape, there are different specifications for the lite sides. The letter W means the total width and the letter W(n) means the partial width of W. The parameters are numbered consecutively. The number in square brackets specifies the width of the lite side in millimeters.

### Footer

The buttons in the footer are described for the *BOM View - BOM Structure* dialog.
⇨ "BOM View – BOM Structure" on page D-199

---

## BOM View - Current BOM Level

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > <F5>`

**Fig. D-82:** Current BOM Level

This tab displays the individual articles of the selected BOM level. Particular information about the articles is displayed, e.g. installation position, quantity, type. You can edit the articles and the associated information. The system adjusts the field display to the requirements of the article. For muntins, for example, instead of the quantity of widths and heights, the quantity of horizontal and vertical muntins is displayed.

If you mark an article in the table, the corresponding article in the BOM tree is highlighted with a light blue spacer.

-   Use `<F6>` to attach an additional article to the BOM.
-   Use `<F3>` to open the next deeper BOM level.
-   Use `<F5>` to open the *All Parameters/Sketch* tab.

When you enter processings in the BOM, you can specify the parameters for the processing on the *All parameters/Sketch* tab.
⇨ "BOM View – All Parameters/Sketch" on page D-212

At the top of the dialog, the *Product Structure* and *Production Sketch* tabs are displayed.
⇨ "BOM View – Product Structure" on page D-202
⇨ "BOM View – Production Sketch" on page D-203

On the *Product Structure* tab, the `Change Product View` button is also displayed.

---

### Change Product View

Turns the installation position of the header article. This mirrors all installation positions of the product structure. The turn is displayed in the cross-section sketch on the *Product Structure* tab.

Use `<Shift>+<F2>` to change between the *Product Structure* and *Production Sketch* tabs.

### Current BOM Level Fields

-   **Article, Description**: Product code and description of the item. This description can be changed.
    *Technical info: mandatory field, numeric field, alphanumeric field, DB field: austrukt.artnr, aufstrukt.artbez1*

-   **IP**: Installation position of the lites and spacers. The position is important for the arrangement and orientation of the lites.
    ⇨ "BOM View – Product Structure" on page D-202
    *Technical info: numeric field, DB field: aufstrukt.einbaupos*

-   **Strct**: Sense of pattern of the ornamental glass. The sense of pattern can be oriented in different directions. The specification of the direction is required for cutting. The column is only enabled for patterned glass.
    -   `vert`: Vertical sense of pattern.
    -   `horiz`: Horizontal sense of pattern.
    -   `diag`: Diagonal sense of pattern.
    *Technical info: toggle field, DB field: aufstrukt.strukthb*

-   **Qty1, Qty2**: Quantity of the selected articles in the BOM, e.g. processings.

    **Example of drilling**
    `Qty1=3` - the lite has 3 drillings.
    The quantity can be changed in the quotation for the price calculation. In the order, each drilling must be entered individually and dimensioned.

    **Example of edge processing**
    `Qty1=2` - in the width, 2 edges are processed.
    `Qty1=1` - in the height, 1 edge is processed.
    *Technical info: numeric fields, DB fields: aufstrukt.anzahl1, aufstrukt.anzahl2*

-   **Wi, He**: Number of widths and heights of the lite that are processed. The fields are displayed for edge processings as alternatives to the fields `Qty1`, `Qty2` or `horiz`, `vert`. If you have entered a shaped lite, it may not be possible for the system to detect the edges as width or height since it may have more than four edges, for example. You have to specify the edge assignment for these shaped lites in the master data. In the master data you can define which edge is calculated as height or width.
    ⇨ Stammdaten, "Kantenzuordnung" auf Seite J-185
    *Technical info: numeric fields, DB fields: aufstrukt.anzahl1, aufstrukt.anzahl2*

-   **ho, ve**: Number of the horizontal and vertical muntins. For muntin processings, the fields are displayed as alternatives to the fields `Wi`, `He` or `Qty1`, `Qty2`.
    *Technical info: numeric fields, DB fields: aufstrukt.anzahl1, aufstrukt.anzahl2*

-   **R/A**: Replacement or additional indicator.
    -   `R`: Replacement indicator. The article was replaced in the BOM.
    -   `A`: Additional indicator. The article was added to the BOM.
    -   `Empty field`: The article is taken over from the master data into the BOM.
    *Technical info: toggle field, DB field: aufstrukt.zusatz*

-   **Offs.**: Step reduction. Depending on whether you enter a step in the item, the specification is set automatically using formulas in the master data.
    -   `Y`: Yes, the article has a step. The step reduction dimension is deducted from the lite dimensions.
    -   `N`: No, no step is assigned to the article. The lite dimensions remain unchanged.
    *Technical info: toggle field*

-   **Supplier**: Supplier number for ordered article. If a supplier is entered, `4 – Ordered` is specified automatically as type.
    *Technical info: numeric field, DB field: aufstrukt.linr*

-   **Field without name**: Number and description of the type of the article. The type of the article can deviate from the type of the item.
    -   `0 = none`: No deviating replacement or additional type selected.
    -   `1 = order before EDI`: The subpart is ordered internally before the head part is transferred to the corresponding producing site. The supplier is notified that the subpart is included in the delivery.
    -   `2 = stock withdrawal before EDI`: The subpart is taken from the stock before the head part is transferred to the corresponding producing site. The supplier is notified that the subpart is included in the delivery.
    -   `3 = produce before EDI`: The subpart is produced internally before the head part is transferred to the corresponding producing site. The supplier is notified that the subpart is included in the delivery.
    -   `4 = P.O.`: Subpart must be ordered from the supplier.
    -   `5 = stock withdrawal`: Subpart is withdrawn from the stock.
    -   `6 = production`: Subpart is produced internally.
    -   `7 = incl. in delivery`: Subpart will be included in the delivery to the supplier by the customer.
    -   `8 = not available`: The subpart is not available.
    -   `9 = included in delivery before EDI`: The type is evaluated before the subpart is ordered via EDI from a different site and is included in their delivery.
    *Technical info: numeric field, DB field: aufstrukt.bestellkzdd*

-   **Print**: Print option for the documents.
    -   `Y`: Print the article breakdown on the customer documents.
    -   `N`: Do not print the article breakdown on the customer documents.
    -   `S`: The article is only output on sales forms, e.g. order confirmations, delivery notes, invoices.
    -   `P`: The article is only output on production papers, e.g. cutting lists.
    *Technical info: toggle field, DB field: aufstrukt.druckkz*

### Footer Buttons (Current BOM Level)

The buttons in the footer are described for the *BOM View - BOM Structure* dialog.
⇨ "BOM View – BOM Structure" on page D-199

In addition, the following buttons are displayed:

-   **Double**: Doublicates the selected article and the associated parameters and inserts it in front of the selected article.
-   **New**: Creates a new line for an article after the last article on the selected BOM level.
-   **Copy**: Copies the selected article and the associated parameters.
-   **Add**: Inserts the copied article into the selected item and overwrites the existing parameters. This way, you can insert the copied article in a new item or overwrite the parameters of an article of the same type. The button is only enabled if an article has already been copied.
-   **Del.**: Removes the selected article from the BOM. The button is only enabled for additional articles.
-   **Find A**: Opens the *Find-A* dialog for article search using the processing or article type. The button is only enabled if you enter a new article and the cursor is in the *Article* field.
    ⇨ "Find Article by Types" on page D-61
-   **Params**: Opens the *All Parameters/Sketch* tab for editing the parameters for the selected article. The button is only enabled if parameters can be specified for the selected article.
    ⇨ "BOM View – All Parameters/Sketch" on page D-212
-   **BOM**: Opens the next BOM level down and displays a list of all articles on this BOM level. The button is only enabled if additional articles are attached to the selected article.
-   **OK**: The function depends on the selected BOM level:
    -   The first level of the BOM is open: All changes are saved and the *Current BOM Level* tab is closed.
    -   A deeper level of the BOM is open: All changes are saved and the next higher level of the BOM is displayed.

---

## BOM View – Processing Param. (short)

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > <F5> > ProcessingParam. (short) tab`

**Fig. D-83:** Processing Param. (short)

This tab lists the individual articles with a selection of associated parameters. You can edit the parameters. The system adjusts the field display to the requirements of the article. For surface processings, the dimension type, size, and position of the area processing are displayed.

If you mark an article in the table, the corresponding article in the BOM tree is highlighted with a light blue spacer.

### Processing param. (short) tab

The display of the fields varies depending on the processing and in some cases does not display all parameters for the processing article. Use `<F5>` to display the *All Parameters/Sketch* tab, on which all processing parameters for the selected article are displayed. The parameters are described in detail for the *All Parameters/Sketch* tab.
⇨ "BOM View – All Parameters/Sketch" on page D-212

The following fields are always displayed:

-   **Article, Description**: Product code and description of the item.
    *Technical info: mandatory field, numeric field, alphanumeric field, DB field: austrukt.artnr, aufstrukt.artbez1*
-   **Additional text**: Text field for additional information. You can specify in the master data whether the field is enabled.
    ⇨ Stammdaten, "Artikel-Vermaßung – Texte" auf Seite J-331
    *Technical info: alphanumeric field, DB field: aufstrukt.zusatz*

### Footer

The buttons in the footer are described for the *Current BOM Level* tab.
⇨ "BOM View - Current BOM Level" on page D-205

In addition, the following button is displayed:

-   **OK**: Saves all changes and changes to the *Current BOM Level* tab.

---

## BOM View – Addresses

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > <F5> > Addresses tab`

**Fig. D-84:** Addresses

This tab displays address information about the suppliers of the individual items in the BOM.

The tab is only enabled customer-specifically.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

---

## BOM View – All Parameters/Sketch

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > <F5> >Select Processing article > <F5>`

**Fig. D-85:** All Parameters/Sketch

On this tab, the parameters for the selected processing article are entered. The fields differ depending on the processing.

Depending on the configuration, the production sketch or BOM structure of the item is displayed on the left side of the dialog. You can change the view with the buttons in the footer.

### All Parameters/Sketch tab

The parameters displayed are drawn from the processing catalog that is stored in the master data. The parameters differ depending on which processing is selected. The description of the individual parameters can be adjusted customer-specifically. You can edit the processing parameters. The following parameters are simply examples. All parameters are described that can be displayed for the various processings. The descriptions can differ depending on customer-specific configuration.

> **Database reference on the All Parameters/Sketch tab**
> There is a complete description of the database references for the individual parameters in the A+W processing catalog.

-   **Article**: Display of the number and description of the processing article.
    *Technical info: display fields, DB fields: poszu.artnr*
-   **Color/Thick**: Display of the color and thickness of the article. The identifier of the color is in the first field; the thickness in millimeters is in the second field.
    *Technical info: display fields, DB fields: poszu.farbe*

-   **A+W Proc. Type**: Display of the number and description of the pre-defined A+W processing types. The processing types are described in the normal A+W processing catalog.
    *Technical info: display fields, DB fields: poszu.awtyp*

-   **Dimension Type**: Interpretation of the dimension entered. In the *Sketches* area, a graphic is displayed from which you can see how the dimensions must be specified.
    -   **Absolute**: With this setting, you select a reference corner from which measurement will be started. The reference corners refer to the circumscribed rectangle of the shaped lite.
    -   **Distance from 2 edges**: With this setting you select the two reference edges from which measuring will be started.
    -   **Corner+edge**: With this setting you select the reference corner and edge from which measuring will be started.
    *Technical info: toggle field, DB field: poszu.mtyp*

-   **Text**: Information text pertaining to the processing step.
    *Technical info: alphanumeric field, DB field: poszu.txt*

-   **Qty Wi/He**: Display of the number of widths and heights of the glass sides to be processed that are listed with width and height information. The field is filled automatically if the edges/corners to be processed are selected in the *Edges/Corners Information* area. Alternatively, the field `Quantity` is displayed.
    *Technical info: display fields, DB fields: poszu.panz1, poszu.panz2*

-   **Quantity**: Display of the quantity of processings on the glass, quantity of rounded corners. The field is filled automatically if the edges/corners to be processed are selected in the *Edges/Corners Information* area. Alternatively, the `Quantity Wi/He` field is displayed.
    *Technical info: display field, DB field: poszu.pme*

-   **Motif (file)**: Name of motif file. Use `<F9>` to open the Explorer for file selection. The field is only displayed if as processing Stamp, Coloring, Etching, Sand blasting, Logo or Silk Screen is selected with motif reference.
    *Technical info: mandatory field, alphanumeric field, DB field: poszu.macronameSilk Scree*

### Edge/Corner Information

The display of the parameters depends on the dimension type.

-   **Proc. Edges**: Selection of the edges to be processed. The field is displayed for edgework.
    -   ☑ Edge will be processed.
    -   ☐ Edge will not be processed.
    *Technical info: mandatory field, checkbox, DB field: poszu.bearbvek*

-   **Proc. Corners**: Selection of the corners to be processed. The field is displayed for corner processings.
    -   ☑ The corner will be processed.
    -   ☐ The corner will not be processed.
    *Technical info: mandatory field, checkbox, DB field: poszu.bearbvek*

-   **Ref. Edges**: Selection of the edge that serves as reference edge for the dimensioning of the processing. If the dimension type *Corner+Edge* is selected, you can only select an edge; if the dimension type *from 2 edges* is selected, you have to select two edges next to one another.
    -   ☑ The edge is used as reference edge.
    -   ☐ The edge is not a reference edge.
    *Technical info: mandatory field, checkbox, DB field: poszu.bearbvek*

-   **Ref. Corner**: Selection of the corner that serves as reference point for the dimensioning of the processing. You can only select a corner as reference corner.
    -   ☑ The corner is used as reference corner.
    -   ☐ The corner is not a reference corner.
    *Technical info: mandatory field, checkbox, DB field: poszu.ecknr*

### Sketches

In the Sketches display you can view the allocations of the edges and corners for the processing of the glass lite and the selected dimension type.

In the graphic, depending on the processing, the interpretation of the respective values are displayed, e.g. for drillings:

**Drilling types**
- Simple drilling
- Countersunk hole
- Stepped drilling

In addition, depending on the processing, the following fields can be displayed:

-   **Distance A**: Distance A for all corner cut-offs and corner cut-outs in millimeters. In the production sketch and in the *Sketches* area, it is displayed from which edge the distance is measured.
    *Technical info: mandatory field, numeric field, DB field: poszudmess1*

-   **Distance B**: Distance B for all corner cut-offs and corner cut-outs in millimeters. In the production sketch and in the *Sketches* area, it is displayed from which edge the distance is measured.
    *Technical info: mandatory field, numeric field, DB field: poszudmess2*

-   **Dist. corner (X)**: Distance from the reference corner in direction of the lite center in millimeters. This field is only displayed for the dimension type *Corner+Edge*.
    *Technical info: numeric field, DB field: poszu.mass1*

-   **DstEdge (Y)**: Distance from the reference corner in direction of the lite center in millimeters. This field is only displayed for the dimension type *Corner+Edge*.
    *Technical info: numeric field, DB field: poszu.mass2*

-   **DstEdge1 (X)**: Distance from the 1st reference edge in direction of the lite center in millimeters. The 1st reference edge is always the numerically smallest reference edge. This field is only displayed for the dimension type *from 2 edges*.
    *Technical info: numeric field, DB field: poszu.mass1*

-   **DstEdge2 (Y)**: Distance from the 2nd reference edge in direction of the lite center in millimeters. The 2nd reference edge is always the numerically larger reference edge. This field is only displayed for the dimension type *from 2 edges*.
    *Technical info: numeric field, DB field: poszu.mass2*

-   **Exp.Para. (W), (W)/(B)**: Width of the parallel area (W) or of the parallel cut-out (W)/(B) in millimeters.
    *Technical info: numeric field, DB field: poszu.dmess1*

-   **Exp.Vert. (H), (H)/(A)**: Height of the vertical area (H) or of the vertical cut-out in millimeters.
    *Technical info: numeric field, DB field: poszu.dmess2*

-   **Rot.Angle**: Angle (in degrees) of the cut-out, motif or area macro for the reference edge. The cut-out, motif or area macro is rotated counter-clockwise.
    *Technical info: numeric field, DB field: poszu.dmeess5, poszu.dmess7*

-   **Diamet. (D)**: Diameter of the drilling in millimeters. For the processing *Stepped drilling* or *Countersunk drilling*, D corresponds to the middle or smallest diameter for the drilling.
    *Technical info: mandatory field, numeric field, DB field: poszu.dmess1 (drilling, countersunk drilling), postzu.dmess2 (stepped drilling).*

-   **Diamet. (D1)**: Diameter of the stepped drilling in the second lite in millimeters. This field is only displayed for the processing *Stepped drilling*.
    *Technical info: numeric field, DB field: poszu.dmess3*

-   **Diamet. (D2)**: Diameter of the stepped drilling in the third lite in millimeters. You can enter a maximum of three diameters for a stepped drilling. This field is only displayed for the processing *Stepped drilling*.
    *Technical info: numeric field, DB field: poszu.dmess4*

-   **Diam.Top (D1)**: Diameter of the counterbore on the outside of the lite (top) in millimeters. This field is only displayed for the processing *Countersunk drilling*.
    *Technical info: numeric field, DB field: poszu.dmess2*

-   **Diam. Btm (D2)**: Diameter of the counterbore on the inside of the lite (bottom) in millimeters. This field is only displayed for the processing *Countersunk drilling*.
    *Technical info: numeric field, DB field: poszu.dmess5*

-   **Level**: Processing side of the lite. The view is always from the outside (top) to the inside (bottom).
    -   **top**: The processing is done on the top side of the lite.
    -   **bottom**: The processing is done on the bottom side of the lite.
    -   **both**: The processing is done on both sides of the lite.
    *Technical info: toggle field, DB field: poszu.ebene*
    **Processing sides (example: double IG)**: `top` `bottom` `top` `bottom`

-   **Corner (C)**: Corner of the lite that serves as reference point for the processing. Alternatively, you can select the reference corner in the *Edges/Corners Information* area. This field is only displayed for the dimension types *Absolute coordinates* and *Corner+Edge*.
    ⇨ "Edge/Corner Information" on page D-214
    *Technical info: numeric field, DB field: poszu.ecknr*

-   **Relie.Cut**: Relief cut. For drillings and counterdrillings, a relief cut can be set so that the lite does not break during drilling, e.g. if the drilling is very close to the edge.
    -   ☑ A relief cut is made.
    -   ☐ A relief cut is not made.
    *Technical info: checkbox*

-   **Edge qual.**: Quality of the edges, e.g. polishing, arrissing. Use `<F9>` to open the dialog for selecting the edge processing.
    *Technical info: mandatory field, numeric field, DB field: poszu.kantenqual*

-   **Logo No., Stamp No., Screen No.**: Number of the logo, stamp or screen that is transferred to production. You can store the numbers for the motif files in the master data.
    ⇨ Stammdaten, "Motivzuordnung" auf Seite J-266
    *Technical info: numeric fields, DB field: xsiebnr.siebnr*

-   **Macro name**: File name of the selected SN macro. The field is only edited if the system is configured appropriately. The macro file is drawn from the master data.
    *Technical info: alphanumeric field, DB field: poszu.dateiname*

-   **Ori.1.Edge**: Orientation of the 1st edge for cut-outs, e.g. corner and edge cut-outs.
    -   **vertical**: The edge is vertical to reference edge A.
    -   **parallel**: The edge is parallel to reference edge B.
    *Technical info: toggle field, DB field: poszu.dmess3*

-   **Ori.2.Edge**: Orientation of the 2nd edge for cut-outs, e.g. corner and edge cut-outs.
    -   **vertical**: The edge is vertical to reference edge B.
    -   **parallel**: The edge is parallel to reference edge B.
    *Technical info: toggle field, DB field: poszu.dmess4*

-   **Radius (R)**: Radius for the rounded corner. It is measured from the center point of the lite. If you want to assign the round corners different radiuses, you have to enter a separate processing step for every round corner.
    *Technical info: mandatory field, numeric field, DB field: poszudmess1*

-   **Radius ou.**: Outside radius for the cut-out, e.g. corner or edge cut-out.
    *Technical info: numeric field, DB field: poszudmess4, poszudmess6*

-   **Radius in., R**: Inside radius for the cut-out, e.g. corner or edge cut-out.
    *Technical info: numeric field, DB field: poszudmess3, poszu.dmess4, poszu.dmess5*

-   **Ref.Edge**: Reference edge of the lite. If you have not selected an edge, edge 1 is used as the reference edge.
    *Technical info: numeric field, DB field: poszu.bearbvek*

-   **Ref.Point**: Selection of the reference point for the cut-out or the motif. You can select any corner of the cut-out or motif or the center point (9=center point) as the reference point. The reference point specifies which point of the cut-out or motif refers to the insertion point of the dimension type. By default, corner 1 is selected as the reference point.
    *Technical info: mandatory field, numeric field, DB field: poszu.dmess3-5*

-   **Saturation**: Intensity of the surface processing in percent.
    *Technical info: numeric field, DB field: poszu.dmess4*

-   **Coat.No.**: Number that is transferred to production. This specification is optional. You can only specify a coating number if you have selected a surface processing with motif. If you specify the coating number, the assigned motif file is displayed in the *Motif(File)* field.
    ⇨ Stammdaten, "Motivzuordnung" auf Seite J-266
    *Technical info: numeric field, DB field: poszu.dmess1*

-   **Scale**: Scaling of the motif. The scaling is only enabled for motifs with the dimension type *Absolute coordinates*.
    -   **freely scalable**: You can specify the height and width of the motif at will. The motif will not be scaled proportionally. If you do not specify any dimensions, the motif will be adjusted to the total height and total width of the lite. This scaling is selected by default.
    -   **proport. (W)**: You can specify the height and width of the motif at will. The height of the motif is adjusted proportionally to the width. If you do not specify any dimensions, the motif is adjusted proportionally to the total width of the lite.
    -   **proport. (H)**: You can specify the height and width of the motif at will. The height of the motif is adjusted proportionally to the height. If you do not specify any dimensions, the motif is adjusted proportionally to the total height of the lite.
    -   **not scalable**: This mode only makes sense with specification of a coating number. With specification of a coating number, this mode is pre-set. You can specify the height and width of the motif within the dimensions from the master data at will. The motif will be cut.
    *Technical info: toggle field*

-   **Mirror**: You can mirror the motif horizontally.
    -   ☑ The motif will be mirrored.
    -   ☐ The motif will not be mirrored.
    *Technical info: checkbox, DB field: poszu.dmess9*

-   **Depth**: Depth of the edgework, e.g. facet grinding, edge screen printing.
    *Technical info: mandatory field, numeric field, DB field: poszu.dmess2*

-   **Depth T.**: Depth of the counterbore on the outside of the lite (top) in millimeters. This field is only displayed for the processing *Countersunk drilling*.
    *Technical info: numeric field, DB field: poszu.dmess3.*

-   **Depth B.**: Depth of the counterbore on the inside of the lite (bottom) in millimeters. This field is only displayed for the processing *Countersunk drilling*.
    *Technical info: numeric field, DB field: poszu.dmess6*

-   **Turn**: You can turn the macro. In the process, the macro is mirrored horizontally and vertically. This field is only displayed for the processing *Surface macros*.
    -   ☑ The macro is turned.
    -   ☐ The macro is not turned.
    *Technical info: checkbox*

-   **Angle**: Angle in degrees for the grinding of the edgework.
    *Technical info: mandatory field, numeric field, DB field: poszu.dmess1*

-   **Angle Top (<1)**: Opening angle of the counterbore on the outside of the lite (top) in degrees. By default, 60 degrees is specified for the opening angle. This field is only displayed for the processing *Countersunk drilling*.
    *Technical info: numeric field, DB field: poszu.dmess4*

-   **Angle B. (<2)**: Opening angle of the counterbore on the inside of the lite (bottom) in degrees. By default, 60 degrees is specified for the opening angle. This field is only displayed for the processing *Countersunk drilling*.
    *Technical info: numeric field, DB field: poszu.dmess7*

-   **WR**: Width of the cut-out from the reference corner along the reference edge in direction of the lite center in millimeters.
    *Technical info: mandatory field, numeric field, DB field: poszu.dmess1*

-   **X Dim. (X)**: Horizontal shift from the reference point in direction of the lite center in millimeters. This field is only displayed for the dimension type *Absolute coordinates*.
    *Technical info: numeric field, DB field: poszu.mass1*

-   **Y Dim. (Y)**: Vertical shift from the reference point in direction of the lite center in millimeters. This field is only displayed for the dimension type *Absolute coordinates*.
    *Technical info: numeric field, DB field: poszu.mass2*

### Footer (All Parameters/Sketch)

The display and function of the buttons depends on whether the left side of the dialog displays the BOM structure or the production sketch of the item.

-   **Production sketch is displayed**:
    -   **Sketch**: Opens the *SNLive Zoom* dialog for display of and zooming in on the production sketch.
-   **BOM structure is displayed**:
    -   **Sketch**: Changes the view and displays the production sketch of the item on the left side of the dialog.
-   **BOM**: Changes the view and displays the BOM structure of the item on the left side of the dialog. This button is only displayed if the production sketch is displayed on the left side of the dialog.
-   **Edges**: Opens the *Edge assignment* dialog. The button is only enabled for edge processings or processings to which the dimension type *2 edges* or *Corner+Edge* is assigned.
    ⇨ "Edge Allocation" on page D-220
-   **OK**: Saves all changes and closes the *All Parameters/Sketch* tab.

---

## Edge Allocation

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > Select Edge processing > <F5>`

**Fig. D-86:** Edge Allocation

On this dialog, you specify which edge(s) of a lite will be processed. The number of edge processings is displayed in the fields `Qty1` and `Qty2`.

The shape number is shown in the center of the shape sketch. A number and a checkbox are displayed for each edge.

-   **1, 2, 3, 4, 5, ..., x**: Edge allocation in shape. If edgework is allocated, any edge can be selected.
    -   ☑ The edge is used as reference edge.
    -   ☐ The edge is not a reference edge.
    *Technical info: checkbox, DB field: poszu.bearbvek*

> **Edge allocation for reference edges**
> The *Edge Allocation* dialog is also displayed if you have selected a processing with the dimension type *Corner+Edge* or *2 edges* and want to allocate the reference edges.
> Depending on the dimension type, you can select a reference edge or two reference edges:
> -   **Corner+Edge**: You can select an edge. The reference corner must be on the selected edge.
> -   **2 edges**: You can select two edges. The reference edges must be next to one another.

---

## Item Processing

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > <Ctrl> + <F8>`

Use this dialog to manage the processing operations for individual items. The item number is shown in the dialog title.

The fields on the *Item Processings* dialog are largely analogous to the fields on the *BOM View* dialog.
⇨ “BOM View" on page D-198

---

## Dimensions of Individual BOM Elements

**Navigation**: `Sales > Order Entry > Items tab > General tab > Price field > <F3>`

**Fig. D-87:** Dimensions of the individual BOM elements

Check the dimensions of the BOM elements for the selected item on this dialog. The data serves only informational purposes. You cannot edit the entries.

-   Using `<F3>` or the plus and minus signs in front of the lines, you can open and close the selected component in the Item column.
-   Use `<F5>` to open the *Shape Dimensions* dialog.
    ⇨ "Shape - Dimensions" on page D-180

### Dimensions of the individual BOM elements

-   **Article**: Display of the article number and description. Next to the description of glass and airspaces, the installation position is also specified, e.g. `EP: 2`.
    *Technical info: display field, DB fields: posbemass.artnr, artikel.artbez1*

-   **Shp**: Display of the shape number from the shape catalog.
    *Technical info: display field: DB field: kmodparam.modnr*

-   **Field without name**: Display of the step marking.
    -   `N`: No step is entered for the glass.
    -   `R`: The glass is the reference glass of the article.
    -   `Y`: A step is entered for the glass.
    -   `A`: A step is entered for the glass automatically. The automatic step is specified by the system and cannot be edited.
    The entry of steps is described in detail for the Step Entry dialog:
    ⇨ "Stepped Entry (Relevant Parts)" on page D-226
    *Technical info: display field*

-   **Qy1, Qy2**: Quantity of selected articles in the BOM, e.g. processings. The display depends on the processing selected, e.g. quantity of drillings, quantity of edge processings, etc.
    *Technical info: numeric fields, DB fields: aufstrukt.anzahl1, aufstrukt.anzahl2*

-   **Dim.1**: Display of the width in millimeters.
    *Technical info: display field, DB field: posbemass.mass1*

-   **Dim.2**: Display of the height in millimeters.
    *Technical info: display field, DB field: posbemass.mass2*

-   **Dim. 3**: Dimension of the spacer in millimeters.
    *Technical info: display field, DB field: posbemass.mass3*

-   **Tnr**: Display of the article part number in the BOM.
    *Technical info: display field, DB field: aufstrukt.tnr*

### Footer

-   **Shape**: Opens the *Shape Dimensions* dialog. The dimensions serve only informational purposes. You cannot edit the entries. The button is only enabled if a shape is assigned to the selected item.
    ⇨ "Shape - Dimensions" on page D-180
-   **Spac. Offset**: Opens the *Edge Clearance* dialog. The button is only displayed if a spacer article is marked in the BOM.
    ⇨ "Spac. Offset" on page D-224
-   **Sealing**: Opens the *Sealing Depth* dialog. The button is only displayed if an outer sealing article is marked in the BOM.
    ⇨ "Sealing Depths" on page D-225

---

## Spac. Offset

**Navigation**: `Sales > Order Entry > Items tab > General tab > Price field > <F3> > Select spacer article > [Spacer Offset]`

**Fig. D-88:** Spac. Offset

On this dialog, you define the dimensions for the spacer offset.

The spacer offset for an IG lite is the distance from the glass outer edge to the spacer outer edge. If you have entered stepped IG, the distance from the smaller glass outer edge of the smaller lite to the spacer outer edge is the spacer offset.

Generally, the spacer offset is the same on all edges of a lite. However, you can also enter an edge-specific spacer offset.

The edge clearance is calculated from `Cutback - spacer thickness`.

Most fields are described in the following location:
⇨ "Shape - Dimensions" on page D-180

In addition, the following fields are displayed:

-   **(Fields in the lite)**: Cutback per lite edge in millimeters. The cutback for an IG lite is the distance from the outer edge of the glass to the inner edge of the spacer. For a stepped IG lite, the smaller lite counts. Generally, the cutback on all edges is the same. However, you can also enter an edge-specific cutback.
    *Technical info: mandatory fields, alphanumeric fields, DB fields: kstufen-param.dmass1, kstufenparam.dmass2, ..., kstufenparam.dmass10*

---

## Sealing Depths

**Navigation**: `Sales > Order Entry > Items tab > General tab > Price field > <F3> > Select Sealing > [Sealing]`

**Fig. D-89:** Sealing Depths

Use this dialog to define the sealing depth.

Most fields are described in the following location:
⇨ "Shape - Dimensions" on page D-180

In addition, the following fields are displayed:

-   **(Fields in the lite)**: Sealing depth per lite edge in millimeters.
    *Technical info: mandatory fields, alphanumeric fields, DB fields: kstuf-param.dmass1-10*

---

## Stepped Entry (Relevant Parts)

**Navigation**: `Sales > Order Entry > Items tab > General tab > Quantity field > <Ctrl> + <F10>`

**Fig. D-90:** Stepped Entry (Relevant Parts)

On this dialog, you specify a step by specifying the dimensions of the glass to be stepped. The reference glass and the glass to be stepped are specified according to the formulas from the master data and assigned automatically by the system. You can edit the assignment under circumstances. You need the reference glass for the dimension calculation of the glass to be stepped.

-   Use `<Shift>+<F5>` to specify the marked glass as reference glass.
-   Use `<F5>` to open the *Shape Dimensions* dialog to specify the dimensions of the reference glass. The selected article has to be the reference glass.
    ⇨ "Shape - Dimensions" on page D-180
-   Use `<F3>` to assign the *Step Reductions* dialog to specify the step dimension. A step has to be assigned to the selected article (S=Y). If you have selected the reference glass, use `<F3>` to open the *Shape Dimensions* dialog.
    ⇨ "Step Reductions" on page D-228

If the item for which you want to enter a step is assigned a shaped lite, the identifier `M` is in the fields next to the article number.
If the data for the step for the item is not yet entered completely or it has to be entered, there is a question mark in the fields next to the article number for the corresponding lites.

### Stepped Entry Fields

-   **Article**: Article number and description of the article. The installation position of the glass is specified in the brackets, e.g. `EP: 1`. The reference glass has the suffix `*REFERENCEGLASS*`.
    *Technical info: display field, DB field: aufstrukt.artnr*

-   **C**: Marking of the step. The reference glass is required for calculation of the step deduction for the glass to be stepped. The following information is displayed:
    -   `N`: No step is entered for the glass.
    -   `R`: The glass is the reference glass of the article.
    -   `Y`: A step is entered for the glass.
    -   `A`: An automatic step is entered for the glass. The automatic step is specified by the system. You cannot edit it.
    *Technical info: toggle field, DB field: kstufparam.art*

-   **Shape**: Shape number of the glass. You can edit the shape or replace it with a new shape. If the lite is not yet assigned a shape, you can assign a shape to the reference glass. Use `<F9>` to open the shape catalog and select a shape. Alternatively, you can enter the shape number directly. If you assign a new shape, the *Shape Dimensions* dialog opens automatically before the step entry.
    ⇨ "Shape - Dimensions" on page D-180
    *Technical info: display field, DB field: kstufparam.modnr*

-   **Sketch**: View of the article in cross section.

### Footer

-   **Delete**: Deletes the step from the item. This field is only enabled if you have last marked an item with steps and you are entering a new item. The BOM of the last marked item including the step is taken over into the new item. If you have specified the quantity for the item, the *Step Entry (relevant parts)* dialog opens automatically. Use `[Delete]` to remove the step from the BOM header of the item and close the dialog.
-   **Replacement**: Enables the field for the selected lite. You can specify a new item number as replacement article.
-   **Matchcode**: Opens the *Find Article* dialog with the cursor in the *Matchcode* field. The button is only displayed if a lite is being replaced.
    ⇨ "Find Article" on page D-51
-   **Selo**: Opens the *Find Article* dialog with the cursor in the *From Number* field. The button is only displayed if a lite is being replaced.
    ⇨ "Find Article" on page D-51
-   **OK**:
    -   If you have specified the dimensions for reference glass and stepped article: saves all details and closes the dialog.
    -   If you have not yet entered dimensions for reference glass and stepped articles: First opens the *Shape Dimensions* dialog to specify the dimensions of the reference lite. Then opens the *Step Reductions* dialog to specify the step dimension.
        ⇨ "Shape - Dimensions" on page D-180
        ⇨ "Step Reductions" on page D-228

---

## Step Reductions

**Navigation**: `Sales > Order Entry > Items tab > General tab > Quantity field> > <Ctrl> + <F10> > Stepped glass > <F3>`

**Fig. D-91:** Step Reductions

Enter the step reduction per lite edge on this dialog. The fields and sketches on the dialog vary depending on the shape number of the lite. You have to specify at least one step reduction per lite.

The system can be configured so that two previews of the shaped lite are displayed on the right side of the dialog. The top view displays a preview of the shaped lite without step. The lower view displays a preview of the shaped lite after deduction of the step. If you change the dimension of the shaped lite or the reduction dimension, the respective preview of the lite is updated.

Most fields are described in the following location:
⇨ "Shape - Dimensions" on page D-180

In addition, the following fields are displayed:

-   **(Fields in the lite)**: Step reduction per edge of the glass to be stepped in millimeters.
    *Technical info: mandatory fields, numeric fields, DB fields: kstufen-param.dmass1, kstufenparam.dmass2, ..., kstufenparam.dmass10*

---

## Muntin Entry

**Navigation**: `Sales > Order Entry > Items tab > General tab > AIR field > <Shift> + <F8>`

Use this dialog to enter a muntin pattern for an IG article.

This dialog contains the following tabs:
-   "Muntin Entry – Muntins" on page D-229
-   "Muntin Entry - Add. Info" on page D-232

### Muntin Entry – Muntins

**Navigation**: `Sales > Order Entry > Items tab > General tab > AIR field > <Shift> + <F8>`

**Fig. D-92:** Muntin Entry – Muntins

Use this tab to enter muntins. The sketch displays the muntin pattern that is entered in the selected inner spacer. The muntins are only displayed in the sketch after entry.

The sketch shows the height and width of the glass, as well as of the individual muntins. The thickness of the airspace is listed at the edge of the lite. All dimensions are given in the specified measurement unit, millimeters or inches.

In addition, the thickness and colors of the muntins are also displayed schematically.

If the selected muntins cannot be displayed in the sketch, e.g. for muntin patterns in two different spacers, a red exclamation point appears in the sketch.

You can edit the muntin pattern on the *Muntin Editor* dialog.
⇨ "Muntin Editor" on page D-234

#### Muntins tab

-   **Muntins, Description**: Article number and description of the muntin. You can only enter two different muntin articles on a lite.
    *Technical info: mandatory field, numeric field, alphanumeric field, DB fields: kspross.artnr, artikel.artbez1*
-   **ho, ve**: Number of the horizontal and vertical muntins. You can enter a maximum of 12 muntins on a lite.
    *Technical info: mandatory fields, numeric fields, DB field: kspross.anzahl1, kspross.anzahl2*
-   **Symmetry**: Arrangement of the muntins. If you select the setting `(+E)` under Symmetry, then you can edit the muntin pattern in the muntin editor.
    -   `F-Sym = Field-symmetrical`: The drill points are calculated automatically. They will be made so that all interior fields are the same size. The distances of the drill points depend on the muntin type from the master data and take the width of the muntins into consideration. Therefore, they are different sizes.
    -   `F-Sym+E = Field-symmetrical with editor`: The drill points are calculated automatically. They can be edited in the *Muntin Editor*. You have to select this setting if, for example, you want to define auxiliary muntins.
    -   `D-Sym = Drilling point-symmetrical`: The drill points are calculated automatically. They will be arranged symmetrically in the spacer. If there are more than one muntin per direction, the fields will be different sizes. The difference is plain to see if the muntins are very wide.
    -   `D-Sym+E = Drilling point-symmetrical with editor`: The drill points are calculated automatically. They can be edited in the *Muntin Editor*. You have to choose this setting if certain requirements for the drill holes have to be met.
    -   `Asym-E = asymmetrical without editor`: Glass areas are arranged asymmetrically. This cannot be edited with the *Muntin editor*.
    *Technical info: toggle field, DB field: kspross.symkz*
-   **Color, Description**: Number and designation of the color if the muntin is defined as color variant.
    *Technical info: numeric field, alphanumeric field, DB field: kspross.farbe*
-   **Supplier**: ID of the supplier of the muntins.
    *Technical info: numeric field, DB field: kspross.linr*
-   **IF**: Number of the inner spacer for multiple IG. You have to specify in which spacer the muntins are installed. If you edit the muntins in the editor, the *Muntin Editor* dialog appears for each inner spacer.
    ⇨ "BOM View" on page D-198
    ⇨ "Muntin Editor" on page D-234
    *Technical info: numeric field, DB field: kspross.rahmenst*

#### Footer

-   **Editor**: Opens the *Muntin Editor* dialog for editing the muntin pattern.
    ⇨ "Muntin Editor" on page D-234
-   **BOM**: Opens the *Muntin Article* dialog for selection of a muntin color.
-   **OK**: Saves the muntin pattern and closes the *Muntin Entry* dialog. If you have selected an option with editor on the *Muntins* tab in the *Symmetry* column, the *Muntin Editor* dialog opens automatically to edit the muntin pattern.

---

### Muntin Entry – Add. Info

**Navigation**: `Sales > Order Entry > Items tab > General tab > AIR field > <Shift> + <F8> > Add. Info tab`

**Fig. D-93:** Muntin Entry – Additional Info

Use this tab to enter additional information about the muntin pattern or to edit the default values.

The sketch is described for the *Muntin Entry* dialog:
⇨ "Muntin Entry" on page D-229

#### Add.info tab

This tab displays the additional information about the mullion construction.
The columns are described for the *Muntin Entry - Muntins* tab.
⇨ "Muntin Entry" on page D-229

In addition, the following columns are displayed:

-   **SType**: Number of the type.
    *Technical info: numeric field, DB field: kspross.beschaffart*
-   **GI**: Number of the lite. The field can only be edited if you have selected a muntin with appropriately pre-defined muntin type (lead muntins). For a multiple IG, you can specify with the glass number on which glass the muntins should be glued.
    *Technische Info: numeric field, DB field: kspross.rahmenst*
-   **mm**: Display of the total muntin length in millimeters. The muntin length is calculated by the system.
    *Technical info: display field, DB field: kspross.Ifdm*
-   **Light Shade**: Width of the light shade in millimeters. This field is only configured customer-specifically.
    *Technical info: numeric field, DB field: kspross.offset*

#### Footer

The footer area is described for the *Muntin Entry* dialog:
⇨ "Muntin Product - Product Number" on page D-233

---

## Muntin Product – Product Number

**Navigation**: `Sales > Order Entry > Items tab > General tab > PType field > <Shift> + <F8> > Insert Muntin > <F3>`

**Fig. D-94:** Muntin Product

Select the color variant for a muntin article in this dialog.

-   **Article, Description**: Article number and description of the muntins.
    *Technical info: display fields, DB fields: kspross.artnr, artikel.artbez1*
-   **Color, Description**: Number and designation of the color variant of the muntin. Use `<F9>` to open the *Color/Thickn.* dialog.
    *Technical info: numeric field, display field, DB field: kspross.farbe*

---

## Muntin Editor

**Navigation**: `Sales > Order Entry > Items tab > General tab > AIR field > <Shift> + <F8> > Insert Muntin > [Editor]`

**Fig. D-95:** Item Inner spacers

Use this dialog to edit the muntin pattern and specify the muntin space dimensions. The muntin pattern is displayed per inner spacer.

If you have selected a multiple IG and the muntins are installed in different inner spacers, the editor opens for each inner spacer with muntins. The title line of the dialog is displayed for the spacer in which you are editing the muntin pattern.

You can shift horizontal and vertical muntin sections to different drill point positions and remove or add them back by clicking.

-   Use `<Shift>+<F11>` to open the *Muntin Sections* dialog.
    ⇨ "Muntin Sections" on page D-236
-   Use `<Shift>+<F5>` to open the *Muntin Pattern* dialog.
    ⇨ "Grid Pattern" on page D-237
-   Use `<F5>` to select individual muntin sections and edit these. The selected muntin section is highlighted in red in the editor. Use `<1>` or `<2>` to insert the selected muntin section or remove it. Use `<3>` to end the editing.
-   Use `<F3>` to delete all changes to the muntin pattern and arrange the muntins symmetrically. The muntin pattern is only reorganized if you confirm the message with [Yes].

If you enter several muntin articles on a spacer, they are numbered sequentially. The numbers of the muntins are displayed at the edge connection points and listed in the *Muntin Information* field. Move the muntins over the drill points by clicking on a glass surface and specifying the new alignment of the drill points. Drill points that are too close to one another, or overlapping, can vanish from the view. You can also move the drill points on the *Muntin Sections* dialog.

### Muntin information

This area lists the numbers and descriptions of the muntins used.

### Drill Points from Edge

This area lists the horizontal and vertical drill points.

-   Use `<Shift>+<F12>` to open the *Drill Point* dialog.
    ⇨ "Drill Point" on page D-235
-   Use `<Shift>+<F8>` to open the *Clear Field* dialog.
    ⇨ "Clear Field" on page D-235

### Footer

-   **New Pattern**: Deletes the specified muntin pattern and arranges the muntins in the editor symmetrically. The muntin pattern is only reorganized if you confirm the message with [Yes].
-   **OK**: Saves the muntin pattern and closes the *Inner Spacer Item* dialog.

---

### Drill Point

**Navigation**: `Sales > Order Entry > Items tab > General tab > AIR field > <Shift> + <F8> > Insert Muntin > [Editor] > <Shift> + <F12>`

**Fig. D-96:** Drill Point

Use this dialog to edit the drill point items of the muntins.

-   **Drill Point**: Position of the drilled hole in the lite. If you change the drilled hole position, you also shift the muntins. Use `<Page Down>` to change between the drilled holes and edit these. In addition to the selected drilled hole, an arrow tip `>` is displayed in the preview.
    *Technical info: mandatory field, numeric field, DB field: ksprpar.bohrp*

### Clear Field

**Navigation**: `Sales > Order Entry > Items tab > General tab > AIR field > <Shift> + <F8> > Insert Muntin > [Editor] > <Shift> + <F8>`

**Fig. D-97:** Clear Field

Use this dialog to edit the height of the clear fields.

-   **Input**: Height of the clear field on the lite. If you change the height of the clear field, you shift the muntins. Use `<Page Down>` to change between the fields and edit their height. In addition to the selected field, an arrow tip `>` is displayed in the preview.
    *Technical info: mandatory field, numeric field, DB field: ksprpar.laenge*

---

## Muntin Sections

**Navigation**: `Sales > Order Entry > Items tab > General tab > AIR field > <Shift> + <F8> > Insert Muntins > [Editor] > <Shift> + <F11>`

**Fig. D-98:** Muntin Sections

The details for all muntin sections are shown on this dialog.

-   **Article, Article Descript.**: Article number and description of the muntin. You can adjust individual muntin sections if you change the article number of the muntin. For this, you have to have entered different muntins on the same inner spacer. You can only use the article numbers of the muntins entered for the changes.
    *Technical info: mandatory field, numeric field, display field, DB fields: kspross.artnr, artikel.artbez1*
-   **Assy. Type**: Specifies how the muntin will be installed.
    -   horizontal
    -   vertical
    *Technical info: display field, DB field: ksprpar.swflag*
-   **Ser**: Serial number of the muntin that is shown in the item overview at the edge connection points.
    *Technical info: display field, DB field: ksprpar.Ifdnr*
    ⇨ "Muntin Editor" on page D-234
-   **Length**: Length of the muntin section.
    *Technical info: display field, DB field: ksprpar.laenge*
-   **Drill Point**: Position of the drilled hole of the muntin. Reference point for the measurement is the lower left corner of the glass.
    *Technical info: mandatory field, numeric field, DB field: ksprpar.bohrp*
-   **Set**: Identifier to show whether the muntin section will be installed.
    -   `Y`: This muntin section will be installed.
    -   `N`: This muntin section will not be installed.
    *Technical info: numeric field, DB field: ksprpar.gesetzt*

---

## Grid Pattern

**Navigation**: `Sales > Order Entry > Items tab > General tab > AIR field > <Shift> + <F8> > Insert Muntins > [Editor] > <Shift> + <F5>`

**Fig. D-99:** Muntin Pattern

Use this dialog to enter the spacing dimensions of the muntins to the glass edges and one another.

This dialog is enabled for individual customers only.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

-   **Glass Edge -> Lower Edge**: Dimension from the bottom glass edge to the bottom edge of the marked muntin.
-   **Glass Edge -> Center**: Dimension from the bottom glass edge to the middle of the marked muntin.
-   **Glass Edge -> Upper Edge**: Dimension from the bottom glass edge to the top edge of the marked muntin.
-   **Loser Edge -> Lower Edge**: Dimension from the bottom glass edge of the marked muntin to the bottom edge of the next muntin.
-   **Loser Edge -> Center**: Dimension from the bottom glass edge of the marked muntin to the middle of the next muntin.
-   **Loser Edge -> Upper Edge**: Dimension from the bottom edge of the marked muntin to the top edge of the next muntin. If the last muntin is marked, the dimension from the bottom edge of the marked muntin to the top glass edge is specified.
-   **Center -> Lower Edge**: Dimension from the middle of the marked muntin to the bottom edge of the next muntin.
-   **Center -> Center**: Dimension from the middle of the marked muntin to the middle of the next muntin.
-   **Center -> Upper Edge**: Dimension from the middle of the marked muntin to the top edge of the next muntin. If the last muntin is marked, the dimension from the middle of the marked muntin to the top glass edge is specified.
-   **Upper Edge -> Lower Edge**: Dimension from the top edge of the marked muntin to the bottom edge of the next muntin.
-   **Upper Edge -> Center**: Dimension from the top edge of the marked muntin to the middle of the next muntin.
-   **Upper Edge -> Upper Edge**: Dimension from the top edge of the marked muntin to the top edge of the next muntin. If the last muntin is marked, the dimension from the top edge of the marked muntin to the top glass edge is specified.

---

# Packaging Planning

You can use packaging planning to plan which and how many forms of packaging you need for the order. The system creates the planning automatically according to your specifications.

Generally lites are packed on racks. Therefore, the terms packaging form and rack are used synonymously for the field and column designations on the dialogs.

You can select different sorting algorithms that specify the item quantities on the racks. In addition you can, depending on the sorting algorithm selected, make your own specifications for the racks, e.g. the number of lites that should be loaded on the rack.

Rack planning depends on the particular system configuration and the settings in the master data.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

This section describes the following dialogs:
-   "Specs. Packaging Planning" on page D-239
-   "Rack Planning" on page D-245

## Specs. Packaging Planning

**Navigation**: `Sales > Order Entry > Items tab > General tab > Price field > <End> > Discount field > <Ctrl> + <G>`

**Fig. D-100:** Specs. Packaging Planning

Use this dialog to make the specifications with which the system should plan the racks that are required for the order. After you have made the specifications, you can start the rack planning. The result is displayed on the *Rack Planning* dialog.
⇨ "Rack Planning" on page D-245

By selecting various sorting algorithms, you can decide which of the specifications you would like to make yourself and which should be made by the system automatically.

The rack planning is configured customer-specifically with one of the following two sets of sorting algorithms:
-   Combination of the sorting algorithms FA, TA, M, and EA
-   Combination of the sorting algorithms PA, PO, and PV

It is not possible to use the sorting algorithms from the various sets together or to combine individual ones.

### Specifications in the sorting algorithms GA, TA, M, and EA

In the overview, you can see which specifications are required, optional or cannot be made depending on whether the sorting algorithm GA, TA, M or EA was specified:

| Sort | Required specification | Optional specification | Specification cannot be made |
| :--- | :--- | :--- | :--- |
| GA | Rack type or rack main group. | - Intermediate padding<br>- Number of lites per padding | - Number of lites<br>- Grouping<br>- Number of lites next to one another<br>- Number of lites across from one another |
| TA | Rack type or rack main group. | - Number of lites<br>- Grouping<br>- Intermediate padding<br>- Number of lites per padding<br>- Number of lites next to one another<br>- Number of lites across from one another | |
| M | - Rack Type<br>- Number of lites<br>- Grouping | - Rack main group<br>- Intermediate padding<br>- Number of lites per padding<br>- Number of lites next to one another<br>- Number of lites across from one another | |
| EA | Rack type or rack main group | - Number of lites<br>- Intermediate padding<br>- Number of lites per padding | - Grouping<br>- Number of lites next to one another<br>- Number of lites across from one another |

### Specifications in the sorting algorithms PA, PO, and PV

In the overview, you can see how the specifications in the sorting algorithms PA, PO, and PV are made:

| Sort | Specifications |
| :--- | :--- |
| PA | The specifications for the sorting algorithm are made via priority lists. |
| PO | The specifications are made via the Rack optimization (PMO). |
| PV | The specifications are made via the Rack optimization (PMO) and the rack loading displayed with the PackView. |

The system calculates whether dimension restrictions are violated by the specifications. For this, rack information stored in the rack management is used, e.g. the rack width. If dimension restrictions are violated, then a message is displayed indicating which specification has to be edited.

Rack management, the Rack optimization and PackView are described in separate documents. For additional information about this module, contact your A+W Software GmbH contact person.

-   Use `<F5>` to change to the header of the dialog in order to change the values for the rack type depending on the document. The header area works like an individual dialog and can be exited again with `<F5>`.
-   Use `<F3>` to start the rack planning. The *Rack Planning* dialog opens.
    ⇨ "Rack Planning" on page D-245
-   Use `<Ctrl>+<F10>` to display an existing rack planning. If there is no rack planning available, a corresponding message is displayed.
-   Use `<Shift>+<F8>` to discard the rack planning specifications. If you confirm the query, all entries will be deleted.
-   Use `<End>` to exit the dialog. The rack planning specifications will be applied.

Depending on the system configuration, when exiting the order entry, there is a branching to the specifications for rack planning. The dialog opens if you confirm the query or if you have changed an existing order.

> **Rack planning in the background process**
> If when saving the order, you respond no to the query about whether you would like to branch into the Rack Planning Specifications, you will be asked whether the rack planning should be conducted in the background process. The execution in the background process can make sense for larger orders if you don't want to wait for the calculation of the rack planning.

The specifications for the rack planning are deleted for the item in question if after saving the rack specifications, you change the value of an item in the order entry, e.g. the quantity.

If after saving the rack specifications you change the composition in a BOM, you will be asked whether you would like to delete the specifications for the rack planning for this BOM. If you confirm the query, all specifications for all items will be deleted that contain the BOM.

### Header

The header area displays the information about the rack type that was specified for the item.

-   **Rack**: Rack type short name and rack type name, e.g. multi-use rack or wooden box. If a rack main group was specified for the item, then the rack main group short name and the rack main group are also displayed. The rack main group is stored in the master data.
    ⇨ "Gestellgruppenbezeichnungen" auf Seite J-203
    *Technical info: display field, DB field: kposgpl.gtypnr*

-   **Maximum/Minimum Weight**: Maximum and minimum weight of the rack type. The maximum weight cannot be changed.
    *Technical info: display field, DB field: kposgpl.maxb, kposgpl.minb*

-   **Maximum/minimum width**: Maximum and minimum width of the rack type.
    *Technical info: numeric field, DB field: kposgpl.maxb, kposgpl.minb*

-   **Maximum/minimum height**: Maximum and minimum height of the rack type.
    *Technical info: numeric field, DB field: kposgpl.maxh, kposgpl.minh*

-   **Minimum/maximum depth**: Maximum and minimum depth of the rack type.
    *Technical info: numeric field, DB field: kposgpl.maxt, kposgpl.mint*

-   **Padding in mm top, bottom, left, right, front, back**: Side padding for variable boxes. The padding can only be edited if a variable box was specified as rack type for the position.
    *Technical info: numeric fields, DB field: kposgpl.foben, kposgpl.funten, kposgpl.flinks, kposgpl.frechts, kposgpl.fvorne, kposgpl.fhinten*

-   **Own weight**: Own weight of the rack type. The own weight cannot be changed.
    *Technical info: display field, DB field: gtyp.eiggew*

-   **Distance in mm crosswise**: Distance between the lites placed next to one another. The distance can only be changed if packing next to one another is allowed for the rack type.
    *Technical info: numeric fields, DB field: kposgpl.absquer*

-   **Distance in mm high**: Distance between the lites placed next to one another. The distance can only be changed if packing above one another is allowed for the rack type.
    *Technical info: numeric fields, DB field: kposgpl.abshoch*

-   **Pltm**: Position number of the selected position in the overview.
    *Technical info: display field, DB field: kposgpl.posnr*

### Overview of specifications for rack planning

-   **Itm**: Item number.
    *Technical info: display field, DB field: kposgest.posnr*
-   **Qty**: Quantity of the item.
    *Technical info: display field, DB field: kpos.menge*
-   **Sort**: Sorting algorithm. If you change the sorting algorithm for an item, then you are asked if you would like to specify it for all items. If you confirm the query, the sorting algorithm is taken over for all items. You can also combine the sorting algorithms.
    -   **TA**: Total algorithm. You have to specify the rack type or the rack main group. The item quantities are distributed automatically by the system on the rack. You cannot specify the number of lites on the rack and the grouping. With the selection of the total algorithm for an item, it is automatically specified for all other items. If you want to combine the total algorithm with other sorting algorithms, then you must first specify the total algorithm and then the other sorting algorithms for individual items. The total algorithm is selected by default.
    -   **PA**: Partial algorithm. You have to specify the rack type or the rack main group. You can also specify the number of lites and the grouping.
    -   **M**: Manual sorting. You have to specify the rack type, number of lites, and the grouping. You can also specify the rack main group.
    -   **PA**: Priority-controlled algorithm. The item quantities are distributed automatically by the system across the rack type with the highest priority. If the item articles cannot be distributed across the rack type with the highest priority because restrictions are violated, then the next rack type in the priority list is used. You can only select the priority-controlled algorithm if a priority list for rack types was stored in the rack management.
    -   **PO**: Rack planning with the Rack optimization (PMO) via a customer-specific interface.
    -   **PV**: Rack planning with the PackView. The racks are planned via a customer-specific interface with the Rack optimization (PMO) and a 3D packing view of the rack loading can be displayed with the PackView.
    -   **EA**: Even algorithm. You have to specify the rack type or the rack main group. For the number of lites, you can only specify an even number. The quantities in all items also have to be even numbers. The group is specified by the system automatically. If you specify the even algorithm for an item, then it is automatically specified for all other items. If you want to combine the even algorithm with other sorting algorithms, then you must first specify the even algorithm and then the other sorting algorithms for individual items.
    *Technical info: toggle field, DB field: kposgpl.belart*
-   **Rtyp**: Number of the rack type. Use `<F9>` to open the rack type search. Only a rack type can be selected that is permitted for the customer. It is stored in the master data which rack types are permitted for a customer.
    ⇨ "Gestelltypen" auf Seite J-103
    *Technical info: numeric field, DB field: kposgpl.gtypnr*
-   **Ghgr**: Number of the rack main group. Use `<F9>` to open the rack main group search. Only a rack main group can be selected that is permitted for the customer. The rack main groups and their assignment to customers are stored in the master data.
    ⇨ "Gestellgruppenbezeichnungen" auf Seite J-203
    ⇨ "Gestelltypen" auf Seite J-103
    *Technical info: numeric field, DB field: kposgpl.ghgrnr*
-   **Quantity**: Number of lites on the rack/in the box. If a value is entered that is smaller than the item quantity, then another line is inserted for the item automatically. The remaining quantity is shifted to the next line.
    *Technical info: numeric field, DB field: kposgpl.gesanz*
-   **Group**: Grouping of items. Item articles from different items can be planned on one rack. With the Quantity you specify how many of the item articles should be assigned to the group.
    *Technical info: numeric field, DB field: kposgpl.gruppe*
-   **Airspace**: Padding in the airspace. The thickness of the padding between the lites in mm.
    *Technical info: numeric field, DB field: kposgpl.zwraum*
-   **Qty**: Number of lites per padding. For example, padding should be inserted between every five sheets.
    *Technical info: numeric field, DB field: kposgpl.zwabs*
-   **Cross**: Number of lites next to one another. The number can only be changed if packing next to one another is allowed for the rack type. If for the item the total algorithm or a grouping was specified, then the number cannot be edited.
    *Technical info: numeric field, DB field: kposgpl.zwabs*
    *Technical info: numeric field, DB field: kposgpl.anzquer*
-   **High**: Number of lites on top of one another. The number can only be changed if packing one on top of another is allowed for the rack type. If for the item the total algorithm or a grouping was specified, then the number cannot be edited.
    *Technical info: numeric field, DB field: kposgpl.anzhoch*

### Footer

In the footer, the article number, article main description, and the width and height of the article for the selected item are displayed.

---

## Rack Planning

**Navigation**: `Sales > Order Entry > Footer area > Discount field > <Ctrl> + <G> > Packaging Planning Settings > <F3>`

**Fig. D-101:** Rack Planning

This dialog displays the result of the rack planning. In the overview, you see the planned requirement for racks and their loading. The rack planning is calculated by the system. You cannot edit the results of the rack planning. If you would like to change the rack planning because you see, for example, that the rack is not optimally utilized, then you can change to the *Specs. Packaging Planning* dialog. On this dialog, you can change the specifications that the system uses for the calculation and restart the rack planning.
⇨ "Specs. Packaging Planning" on page D-239

You cannot close the *Rack Planning* dialog. If you want to exit the dialog, change to the *Specs. Packaging Planning* dialog.

-   Use `<Ctrl>+<F10>` to change to the *Specs. Packaging Planning* dialog.
-   Use `<F2>` to store up to four texts for each rack. By selecting `Y` for yes and `N` for no in the *Orders* column, you can decide for each text whether it should be printed on the order documents.
-   The storage of texts for the racks depends on the settings in the master data and the system configuration in question.

The following views are enabled only customer-specifically:
-   Use `<F5>` to change to the *Box Dimensions* view.
-   Use `<Shift>+<F5>` to change to the *BoxInfo* view.

### Header

The fields in the header area are described for the *Rack Planning Specifications* dialog:
⇨ "Specs. Packaging Planning" on page D-239

### Rack planning overview

The columns are described for the *Specs. Packaging Planning* dialog:
⇨ "Specs. Packaging Planning" on page D-239

In addition, the following columns are displayed:

-   **Rack No.**: Rack number. The rack number is assigned by the system.
    *Technical info: display field, DB field: kposgest.vsgnr*
-   **Ser.**: Serial numbering of the rack.
    *Technical info: display field, DB field: kposgest.Iftpos*
-   **Width**: Width of the lite.
    *Technical info: display field, DB field: kpos.laenge*
-   **Height**: Height of the lite.
    *Technical info: display field, DB field: kpos.breite*
-   **Depth**: Depth of the loading. The loading depth, calculated from the thickness of all lites and the padding.
    *Technical info: display field*
-   **Weight**: Total weight of the lites on the rack.
    *Technical info: display field*

### Footer

The following rack information about the selected item is displayed:

-   **Rack**: Rack number.
-   **TotNo**: Number of articles that are loaded on the rack.
-   **TotDepth**: The article loading depth, calculated from the number of articles, but without the padding.
-   **TotWeight**: The total of the rack's own weight and the weight of the articles.

---

# Notes

Notes are internal information that is not output on forms. Depending on the configuration, they may be displayed automatically or they can be called up manually.

You can enter several lines of text in a note. For each text line, you can set an individual priority and an info location.

The market partner, article, and object notes can be stored in the master data. The document notes are only stored in the respective document and not in the master data.

> **Database reference in the note texts**
> The notes are stored in the database table `memo`. The type of note is specified by the corresponding entries `memp.typ`, `memo.key1-3` and `memp.flag1-3`.

| Priority | Meaning |
| :--- | :--- |
| **Low** | Notes can be viewed for the respective notes type via the Info menu, but they are not displayed automatically. |
| **Medium** | Notes can be viewed for the respective notes type via the Info menu, but they are not displayed automatically. |
| **High** | Notes for the note type in question are displayed automatically if the market partner, the document, the object or the article for which the note was entered is called up. If the note is displayed, the complete note text is displayed, that is, even all text lines with the priority Low or Medium are displayed. |
| **Block for reference** | No reference can be made to documents with notes of this priority. The stored information text is displayed automatically if the document should be used as reference document or the document is opened. This priority can only be selected for document notes. |

**Tab. D-8:** Priority levels

Depending on the note type, the note text is displayed automatically for the corresponding processing step if its priority is set to high:

-   **Document notes**: These note texts are displayed as soon as the document is opened.
-   **Market partner notes**: These note texts are displayed as soon as the market partner is selected. The note refers to the selected market partner, e.g. to the customer or supplier.
-   **Project note**: These note texts are displayed as soon as the project is selected. You can only store notes for a project if you have selected a project for the order.
-   **Article notes**: These note texts are displayed as soon as the article is selected.
-   **Customer notes**: These note texts are displayed as soon as the customer is selected.
-   **Customer-article notes**: These note texts are displayed as soon as an article for this customer is selected.
-   **Project-article notes**: These note texts are displayed as soon as the article for this project is selected.
-   **Supplier notes**: These note texts are displayed as soon as the supplier is selected.
-   **Supplier-article notes**: These note texts are displayed as soon as the article for this supplier is selected.

You can display and edit notes for documents, market partner, articles, project, and various combinations of these types, e.g. project-article notes.

-   "Document Notes" on page D-249
-   "Market Partner, Project, Article Notes" on page D-250
-   "Customer Article, Supplier Article, Project Article Notes" on page D-253

## Document Notes

**Navigation**:
- `Sales > Order Entry > Header, Footer area > <Shift> + <F4> > Document Notes`
- `Sales > Order Entry > Item level > <Shift> + <F4> > Notes > Document Notes`

**Fig. D-102:** Document Notes

Use this dialog to store notes about the open document. You can enter the document notes in the header and on the item level of a document. You can only store the notes for the current document. They are not stored in the master data.

### Body

-   **(Entry lines for text)**: Note text for the open document. Use `<Enter>` to change to the next text line. Each text line is configured individually; that is, you can specify the priority for each line.
    *Technical info: alphanumeric fields, DB fields: infokauf.atxt*

### Footer

-   The priority for the current note is displayed in the footer.
-   **Priority**: Changes the priority for the selected text line. Alternatively, you can change the priority with `<Shift>+<F10>`.

## Market Partner, Project, Article Notes

**Navigation**:
- `Sales > Order Entry > Header, Footer area > <Shift> + <F4> > Market Partner, Project, Article Notes`
- `Sales > Order Entry > Header, Footer area > <Shift> + <F4> >Notes > Customer, Supplier, Project, Article Notes`

**Fig. D-103:** Market Partner, Project, Article Notes

These dialogs display notes about the market partner, the project or the article. The dialogs are structured the same way. Differences will be described explicitly below.

The note texts are generally created in the master data. If you edit the note texts and add new ones, store them with `<F3>`. The changes are taken over into the master data and the dialog closes.

In sales documents, the customer notes are displayed and in purchasing documents the supplier notes.
