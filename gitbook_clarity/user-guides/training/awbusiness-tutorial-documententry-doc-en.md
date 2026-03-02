---
description: "EN_AWBusiness_Sales_4_2-1"
---


---
## Comprehensive Document Entry up to the Invoicing Stage

### Save Quick Inquiry

*Figure: Save quick inquiry dialog*
```
Save as
- Client: Quotation
- Area: Order
- Number Manager: Mandant 1, <k.A.>, Documentation
```

6. Choose in the **Save quick inquiry** dialog whether you would like to save the data as a quotation or as an order.
7. Select the corresponding OM area and number manager.
8. Click on **[OK]** to save the data.
   Quick inquiry closes. The system returns to the item entry in the document you have been editing last.

---

## Checking the Availability of Products

If the report on stock shortfall has been enabled in the Options menu, the system will issue an appropriate report when you try to save an order where this is the case. Right at item entry you can check the stock on hand and the future stock on hand and amend the delivery dates of the current order as required.

### Checking the availability of a product

1.  Select the item for which you require details.
2.  Click on **[Info]**.
    The dialog opens. In the following example, the delivery date is at risk due to a stock shortfall for one of the BOM components.

    *Fig. C-43: Stock shortfall for one of the BOM components*

    One of the components is shown in red letters on the BOM. This is the component that jeopardizes the delivery date.

3.  Click on **[End]** to close the dialog.
    The **Article info** dialog closes.

4.  Go to the menu **Start > Stock search** to switch to the search mode.
    If the components are not kept as stock articles, you must enter the product number of the critical component and start searching.
    In the following example, the components are kept as stock articles.

    *Fig. C-44: Stock info*
    *   **A**: The present stock on hand falls short of the minimum stock required
    *   **B**: Reserved quantity
    *   **C**: Ordered quantity

    The stock on hand of this component falls short of the minimum stock. Reservations exceed the currently open purchase orders by far. You can infer that the production date will have to be postponed.

5.  Switch to the **Future stock on hand** tab to check how you can adjust the dates for this order.

    *Fig. C-45: Future stock on hand*
    *   **A**: Inquired product: current stock
    *   **B**: Stock on hand and reservations for the next 14 days
    *   **C**: Total stock for the period displayed (only stock articles in the same stock management mode)

    Display of the future stock on hand takes into account a period of up to 14 days in advance. This tells you when the stock on hand will permit to produce the order in question.

6.  Click on **[End]** to close the dialog.
    Item input is shown again. Now you can change the product or the dates in the order header.

---

## Enter Grills

For every insulating glass unit, you can enter grill patterns for all spaces between sheets. They always apply to the entire item.

The following instructions exist for this training module:
*   "How to enter a common grill pattern" on page C-105
*   "How to enter an irregular grill pattern" on page C-108

### How to enter a common grill pattern

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Enter a new item or select the item for which you want to enter grills in the **Items** section.
3.  Go to the **Grills** tab.

    *Fig. C-46: Fields for grills are enabled*
    *   **A**: Grill pattern selection
    *   **B**: In the case of multiple IG: Select the spacer
    *   **C**: Selection of grills
    *   **D**: Calculation type

4.  Select the grill pattern by means of the corresponding icon (A).
5.  Choose the grills (C) and enter the quantity.
    If you have entered a multiple IG unit, you must select the spacer (B) to which the grills shall be attached.
    The graphics and the fields are updated. You can choose different products and/or variants for the horizontal and vertical grills.
    Use the `++` button to adopt the grills for the second spacer.
    However, you can also design the grill grids differently in the gaps, e. g. position the horizontal grills in the first gap and the vertical ones in the second.

    *Fig. C-47: Grill pattern with different grills*
    *   **A**: Drill sizes
    *   **B**: Reference point for dimensions
    *   **C**: Indicator for grill pads
    *   **D**: Calculation type
    *   **E**: Cutback

6.  Define the calculation type (D) and enter the drilling sizes (A) if necessary.
    The fields for the drilling sizes are only enabled for asymmetrical calculation types.
    (See "Grill pattern" on page C-69)
7.  Check the size of the cutback (E) and define whether or not grill pads (C) shall be fitted.
    If the cutback is supposed to be in different sizes at the edges, you must open the **Cutback** dialog by clicking on button (E). Then enter the cutback size for each edge.
8.  Check the sales prices and the printer settings.
9.  Go to the menu **Start > Save** to adopt the data.
    The view changes to the **Item** tab. In the BOM, a component has been entered for the horizontal grills, as well as for the vertical grills.
10. Go to the menu **Start > Save** to save the item.
    The data will be saved; price fields will be updated.

### How to enter an irregular grill pattern

1.  Enter the grills as described in steps 1 to 6 above.
    Please make sure that the number of bars permits an asymmetrical pattern.

    *Fig. C-48: Basic grill pattern*
    *   **A**: Selection of horizontal grills
    *   **B**: Selection of vertical grills
    *   **C**: Selection of diagonal grills
    *   **D**: Auxiliary bars tab

2.  To fit V bars, go to the tab **Auxiliary bars** (D).
    Special grill patterns such as sun or moon are also possible. These are the subject of a separate training session on **A+W CAD Designer**.
3.  Disable the checkboxes for all grid sections that are not required, e. g. the vertical bars in the top third (B).
4.  Enable the checkboxes for diagonal bars (C).

    *Fig. C-49: Irregular grill pattern*

5.  Go to the **Prices** tab to check the sales prices.
6.  Go to the menu **Start > Save** to adopt the grill data.
    The display changes to the **Item** tab. The BOM shows the grills and the corresponding prices.
7.  Go to the menu **Start > Save** to save the item.
    The data will be saved; price fields will be updated.

> **Saving frequently required product structures as macros**
> When you have entered a product structure that you will be using frequently, for this particular customer or in general, you can save it as a macro and load it when you enter the next order.

---

## Enter Shape

You can enter a shape for every item. It will apply to the entire item. The entered shape can be printed on the order confirmation. You have to define the print parameters for this purpose. (See "Printing Sketches" on page C-192)

> **Change shape**
> If you change the shape during input, the shape parameters will be kept. This refers to reflected shapes only. However, if the parameters change, you have to enter new values.
>
> **Enter processing**
> You should enter the shape with all its edges and lengths first. Only then will the system display all existing edges which you can select for processing. (See "Enter Processing Step" on page C-115)

### How to enter a shape

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Enter a new item or select in the section **Items** the item for which you want to enter a shape.
    For the dimensions, you must enter the size of the surrounding rectangle. If you have entered the dimensions on the Shapes tab, the values are updated in the item and can no longer be changed there.
3.  Switch to the **Shapes/processing** tab.
4.  Select by using the icon **Shapes**.
    The fields to enter the values are displayed.
5.  Select the shape by entering the shape or product number, or by means of the corresponding icon (B).
    The section Display shows a sketch of the shape; the fields for the corresponding sizes are enabled.

    *Fig. C-50: Enter shape*
    *   **A**: Enter sizes
    *   **B**: Select a shape
    *   **C**: Dimensions for price calculation

6.  Enter the sizes for the edges (A).
    Please observe the corresponding notifications, W1+W2<=W for example means that the total of the entries for edges W1 and W2 must not exceed the size of edge W.
    When you have made all entries, the size of the surrounding rectangle is shown which is used for price calculation by default.

    *Fig. C-51: Shape entered*

7.  Go to the menu **Start > Save** to adopt the shape data.
    The data will be saved.
8.  Go to the menu **Start > Save** to save the item.
    The data will be saved; price fields will be updated.
    You can add processing steps now if required. (See "How to enter a processing step" on page C-115)

---

## Enter Steps

You can enter a step for every IG item. It will always apply to the entire item.

### How to enter a step

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Enter a new item or select in section **Items** the IG item for which you want to enter a step.
3.  Switch to the **Shapes/processing** tab.
4.  Select the step by entering the product number, or by means of the corresponding icon.
    The fields to enter the values are displayed.

    *Fig. C-52: Define step*
    *   **A**: Select the sheet for which the step shall be defined: 1 = Outside sheet, 2= Inside sheet
    *   **B**: Enter the values per edge: Positive entries will scale down the selected sheet. Negative entries will enlarge the sheet.

5.  Enter all necessary sizes.
    The fields for the sizes are now enabled. If no shape has been entered, a rectangular sheet will be displayed automatically.
    In the section **Parameter**, 1 represents the outside sheet and 2 the inside sheet.
    Please make sure to tick checkbox 2 (A) for the inside sheet. You will then have to enter positive values for this sheet in the fields, e. g. 15.
    If you enter negative sizes (-15), a larger sheet will be cut. This would mean that sheet 2 (inside) would be bigger than the outside sheet.
    The sheet view is updated.

6.  Go to the menu **Start > Save** to adopt the stepping data.
    The data will be saved.
7.  Go to the menu **Start > Save** to save the item.
    Data will be saved and the price fields updated when you enter a price for the step, or adopt it from the price lists.

---

## Enter Processing Step

You can enter several processing steps per item. First, you must enter every further processing step in the BOM as a component. Processing steps always apply to the entire item.

> **Prerequisite**
> Processing steps must be entered as products in the master data.

The following instructions exist for this training module:
*   "How to enter a processing step" on page C-115
*   "How to enter processing steps for a shape" on page C-117

### How to enter a processing step

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Enter a new item or select in the section **Items** the item for which you want to enter a processing step.
3.  Switch to the **Shapes/processing** tab.
4.  Select the processing step by entering the product number, or by means of the corresponding icon, e. g. edgework.
    Product data for this processing step is adopted. The fields for the corresponding parameters are displayed and enabled.
    For a description of the parameters per processing type, please refer to the Software Reference.

    *Fig. C-53: Processing: Example: Edge sawing*
    *   **A**: Selection of processing step
    *   **B**: Selection of the edges to be processed
    *   **C**: Reference corners, reference edges
    *   **D**: Miter angle

5.  Enter the parameters by ticking or unchecking the checkboxes (B) for the edges and enter the sizes.
    Pay attention to the reference corners or reference edges (C) and convert the sizes if necessary.

    > **Incorrect or missing processing parameters**
    > If incorrect parameters are displayed for a processing step, you have to check if the correct product type and group have been allocated to this product in product management.

6.  Go to the menu **Start > Save** to adopt the data.
    The data will be saved; price fields will be updated. The BOM shows the processing and the corresponding price.
7.  The following activity sequence describes how you can enter additional processing steps.
    Go to the menu **Start > Save** to save the item.
    The data will be saved; price fields will be updated.

### How to enter processing steps for a shape

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Enter a new item or select in the section **Items** the item for which you have entered the shape.
    These steps also apply to rectangular sheets and IG items.
3.  Switch to the **Shapes/processing** tab.
4.  Click the main product on the BOM.
    A component with product number 0 will be entered.
5.  Select the new component and select the processing step, e. g. a step.
    Proceed as described in the aforegoing steps.

---

## Enter Patterns

You can enter patterns for surface processings of the product group **Coating, Matting, Screen printing, Area enameling, Sand blasting,** and **Color**.

You can enter a pattern in two ways:
*   With screen number
*   Without screen number

The difference between the two entry methods will be shown in the following learning module.

The following instructions exist for this training module:
*   "How to create a pattern with screen number in the master data" on page C-118
*   "How to enter a pattern with screen number" on page C-120
*   "How to enter a pattern without screen number" on page C-124

> **Prerequisite**
> The pattern file must be saved in a directory so that you can enter a pattern and/or create a pattern with screen number.

### How to create a pattern with screen number in the master data

1.  Save the pattern file in the directory from which you want to insert the file.
2.  Select **Master Data > Products > Item > Patterns**.
    The **Patterns** dialog opens.
3.  Select in the menu **Start > New** to create a pattern.
    The fields in the **Pattern** area are enabled.

    *Fig. C-54: Creating a pattern with screen number*

4.  Enter a screen number (A) for the pattern.
5.  If necessary, enter a name (B) for the new pattern. It should be meaningful and unique so that you can recognize the pattern using the name.
6.  Enter the pattern file (C) with the **[Folder]** button.
    The pattern file is displayed in the preview window (D).

    *Fig. C-55: Example - Creating a pattern with screen number*
    *   **A**: Screen number
    *   **B**: Pattern name
    *   **C**: Path for the pattern file
    *   **D**: Preview for the pattern
    *   **E**: Maximum dimensions of the pattern

7.  Enter the maximum width and height (E) of the screen.
    These dimensions from the master data cannot be exceeded if you are entering a pattern with screen number and the item entry.
8.  Select in the menu **Start > Save** to save the data.
    You can enter the pattern via the screen number in the processing.

### How to enter a pattern with screen number

> **Prerequisite**
> The pattern must be created in the master data so that you can enter it via the screen number.

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
    Enter a new item or mark the item for which you want to enter the pattern in the **Items** area.
    In this example, a rectangular TG sheet with the dimensions 1100 x 2100 mm is selected.
2.  Go to the **Shapes/processing** tab.

    *Fig. C-56: Selecting coating as product group*
    *   **A**: Buttons for coating
    *   **B**: Product number

3.  Select the processing by entering the product number (B), or by clicking the appropriate button (A).

    *Fig. C-57: Buttons for the product groups for pattern entry*
    *   **A**: Coating
    *   **B**: Frosting
    *   **C**: Screen printing
    *   **D**: Surface enameling
    *   **E**: Sandblasting
    *   **F**: Coloring

    In this example, the product group **Coating** is selected as processing.
    Product data for this processing step is adopted. The fields for the corresponding parameters are displayed and enabled. For a description of the parameters per processing type, please refer to the Software Reference.

    *Fig. C-58: Entering patterns: example of coating*

    *Fig. C-59: Processing parameters with specification of a screen number*
    *   **A**: Dimension type
    *   **B**: X-value, Y-value, reference corner and reference edge for the positioning of the pattern
    *   **C**: Dimensions of the pattern
    *   **D**: Angle, reference edge, and reference point of the pattern
    *   **E**: Color variants
    *   **F**: Saturation
    *   **G**: Level to which the pattern is applied
    *   **H**: Path of the pattern file and file search
    *   **I**: Mirroring
    *   **J**: Screen number

4.  Select the dimension type (A), the reference point and the reference edge (D) and enter the angle (D).
    With the selection of the dimension type, you specify how the values entered should be interpreted.
    In the Reference field, you define which edge of the pattern (or whether the middle point of the pattern) refers to the insertion point of the dimension type.
    With the angle, you specify how the pattern should be turned with respect to the reference edge.
5.  Select the reference edge(s) and/or the reference corner (B) and enter the X-value and Y-value (B).
    With these values, you specify the horizontal and vertical distance to the reference point, the reference edge(s), and/or the reference corner of the sheet from which the pattern is positioned.
6.  Enter the maximum width and height (C) of the pattern.
    With the dimensions, you select the size of the pattern. By default, the dimensions of the sheet are displayed. Make sure that the cutout is not larger than the maximum dimension of the pattern from the master data.

    > **Pattern too large**
    > The width and height of the pattern are set to the maximum dimension from the product master data if the dimensions entered are larger than the dimensions from the master data. If necessary, repeat step 6 to adjust the size of the pattern.

7.  If necessary, select a variant (E).
8.  Enter the screen number (J) of the pattern file.
    The path of the pattern file (H) is displayed in the Pattern field. The combo box below the field is locked. The pattern is displayed in the graphic display.

    > **Access to pattern file**
    > Make sure that the pattern file is saved under the specified file path. If the file is moved, the pattern can no longer be found using the screen number.

    *Fig. C-60: Pattern preview after entering the screen number*

9.  If necessary, enter the saturation (F).
10. Select the processed side (G).
    The processed side **Level 1** corresponds to the outside of the sheet, **Level 2** to the inside of the sheet.
11. If necessary, mark the **Mirroring** check box (I).
    The pattern is mirrored.
12. Select in the menu **Start > Save** to save the data.

### How to enter a pattern without screen number

1.  Save the pattern file in the directory from which you want to insert the file.
2.  Enter the pattern as in steps 1 to 7 and 9 to 11 of the previous instructions.

    *Fig. C-61: Processing parameters without specification of a screen number*
    *   **A**: Dimensions of the pattern
    *   **B**: File search and path of the pattern file
    *   **C**: Scaling mode of the pattern

3.  Enter the pattern file with the **[Folder]** button (B).
4.  In the combo box, select (C) the scaling of the pattern. You can select the option **Freely adjustable**, **Proportional width** or **Proportional height**:
    *   **Freely adjustable**: With this setting, you can specify dimensions as you wish (A). This can distort the pattern.
    *   **Proportional width/proportional height**: With these settings, you can specify the height or the width of the pattern. In each case, the other dimension is adjusted proportionally. Here, the pattern can be cut off.

    *Fig. C-62: Pattern preview without proportional scaling*

