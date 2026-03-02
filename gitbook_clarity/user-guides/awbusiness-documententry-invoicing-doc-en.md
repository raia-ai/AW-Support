---
description: "EN_AWBusiness_Sales_4_2-2"
---


# Comprehensive Document Entry up to the Invoicing Stage: Tutorial

*Fig. C-63 Pattern preview with proportional scaling*

5. Select in the menu **Start > Save** to save the data.

---
## Enter a Surcharge for Special Services

You can define several surcharges per item in case the product structure requires special work steps or services. A special service may be e.g. the changing of the pattern or coating level for an IG unit.

> **Prerequisite**
> Services must be entered as products in the master data. They are listed in the Services product group.

### How to enter a surcharge for special services

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
    You should start entering services only after all order items have been completely entered and saved. Go to the tab **Item** if required.
2.  Go to the tab **Services**.

*(Image: Fig. C-64 Service entry - Example: Packing surcharge, showing the services tab with item references (A) and a product number input for the service (B). The section Item reference shows all order items.)*

*   **A**: Select the item
*   **B**: Product number of service

3.  Select the service by means of the search function, or enter the product number (B) directly in the input line.
    The fields are completed with the values from the master data.
4.  Check the values, e. g. price or display.
    The price for the service can be printed the same as for every BOM component.
    ⇨ "Calculation settings" on page C-138
5.  Select the item(s) (A) for which this service shall be calculated.
    Use **[All]** to tick all order items or **[None]** to remove all checkmarks. The value for the service will be updated in the input line.
6.  Go to the menu **Start > Save** to adopt the data.
    The prices for the service will be updated. The service will be entered in the BOM of all ticked items.
7.  Go to the menu **Start > New** and repeat the steps 3 to 6 in order to enter additional services.
    The prices for the service will be updated. The service will be entered in the BOM of all ticked items.
8.  Go to the menu **Start > Save** to save the data.
    The data will be saved; price fields will be updated.

> **Delete a service**
> Services cannot be deleted from the BOM by means of the context menu. To remove a service, you have to remove the item allocation or the entire service in the Service tab.

## Edit BOM Structure

You can amend any BOM structure to your customer's requirements. Please note the following:
*   Gas is always added to the spacer as a component.
*   A film layer can be added before or after an individual sheet in a laminated unit.
*   Grills, shapes, processing steps and services can only be attached via the corresponding tabs.
    *   ⇨ "Enter Grills" on page C-105
    *   ⇨ "Enter Shape" on page C-110
    *   ⇨ "Enter Processing Step" on page C-115

The following instructions exist for this training module:
*   "How to edit the BOM structure" on page C-129
*   "How to delete a BOM component" on page C-130

### How to edit the BOM structure

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Select the component on the BOM before or after which you want to add a component.
3.  Open the context menu (right mouse button) and select the required command.

*(Image: Fig. C-65 Open the context menu on the BOM. The screenshot shows a context menu with options like "Add element", "Insert element (before)", "Insert element (after)", and "Delete element".)*

The display changes to the BOM tab. The field for the product number is enabled.

*(Image: Fig. C-66 Enter product number of new component. The screenshot shows an empty input field ready for a new product number.)*

4.  Enter the product number and select the requested product, e. g. a filling.

*(Image: Fig. C-67 Enter product number of new component. The screenshot shows the product number "12530" for "Wärmedämmgas Krypton" being added to the BOM.)*

5.  Go to the menu **Start > Save** to save the new component.
    The data will be saved.

### How to delete a BOM component

1.  In the section BOM, select the component you want to delete.
2.  Open the context menu and select the command **Delete component**.
    The component is removed from the BOM.
3.  Click on **[Save]** to save the changes.
    The data will be saved.

> **Delete a service**
> Services cannot be deleted from the BOM by means of the context menu. To delete a service, you have to remove the item allocation in the Service entry dialog.
> ⇨ "Enter a Surcharge for Special Services" on page C-127

## Edit or Add an Order Item

You can edit any order after saving it. Please note that P.O. items or cut items may have been transferred to the corresponding interfaces already.

> **Change ordered item**
> If P.O. items have been transferred already, input fields will be locked. They can be enabled via the menu **Functions > Item group > Change locked item**.

### Copy order item

You can copy any existing and saved item and add it as a new item. The data of the new item can be amended later, e. g. by replacing a sheet. This function is useful for entering complex BOM structures for which no product or macro has been defined.

**How to copy an order item**

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Select the item you want to copy from the list.
3.  Go to the menu **Start > New**.
    The new item is added, showing the data of the copied item.
4.  Edit the data, e. g. the sizes.
5.  Go to the menu **Start > Save** to save the data.
    The new item is saved. The fields in the **Totals** tab are updated.

> **Alternative copy function**
> If you have entered a large number of items, you can find the requested item more easily by using the function **Copy from item ...** For this function, go to the menu **Functions > Item group**.

### Deleting an order item

You can remove items from any saved order. However, please note that P.O. items or cut items may have been transferred to the corresponding interfaces already.

**How to delete an order item**

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  In the section **Items**, select the line you want to delete.
3.  Go to the menu **Start > Delete**.
    The item is removed from the list and from the order. The fields in the **Totals** tab are updated.

## Exercises

### Enter items

Open your order and enter the following items:
*   IG units with single annealed float 5 mm
    *   10 pcs. of 600 x 800 mm
    *   10 pcs. of 1000 x 1000 mm
*   Save the items and check whether automatic surcharges have been added.

### Editing items

Change the following item details:
*   Copy an item so that you have entered 3 items in total now.
*   Add a simple grill pattern for one of the items.
*   Replace the outside sheet by a patterned glass sheet for one of the items.
*   Add steps to a simple shape.
*   Define additional services for this shape.

### Answering quick inquiries

Enter a quick inquiry:
*   Save all changes in the current order.
*   Start the quick inquiry function and select another customer.
*   Enter an IG unit including laminated glass, part of which is to be purchased.
*   Enter a tempered glass sheet to be purchased completely.
*   Save the quick inquiry in the form of a new order.

### Enter an item via quick input

Enter an item via quick input.
*   Enable the option **Dynamic product field**.
*   Enter the following values:
    **215,8003-1000-500-1000-800**
*   Enter another item with the following values:
    **150000,8001-1000-1000-120,8260-2-2**
*   Check whether the bill of material, the shape and the grills have been entered correctly.

### Entering patterns

Enter a pattern:
*   Create a pattern in the master data.
*   Select an existing item and add a pattern with the screen number created.
*   Enter a new item and add a pattern without screen number.
*   Enter a pattern with proportional scaling and adjust the parameters so that the pattern is not cut off.

**Additional information**
*   ⇨ Master Data, "Company Data - Parameters" on page B-934
*   ⇨ Master Data, "Company Data > Price Calculation" on page B-944
*   ⇨ "Enter Grills" on page C-105
*   ⇨ "Enter Shape" on page C-110
*   ⇨ "Enter a Surcharge for Special Services" on page C-127
*   ⇨ "Edit BOM Structure" on page C-128
*   ⇨ "Enter Patterns" on page C-118

## Prices

**Objectives**
*   Getting familiar with pricing in A+W Business (prices, surcharges, discounts).
*   Getting familiar with the price display.
*   Editing prices in an order.

**Benefits**
*   If pricing is done by means of predefined prices, discounts and surcharges, there is usually no need for manual intervention.
*   Knowing the context and overall scheme of pricing allows you to make individual price adjustments.

> **Note:**
> Prices must be enabled for the product. Prices can be adopted from the master data only if the price-relevant code has been set in product management.

| Term | Description |
| :--- | :--- |
| **Manual changes** | Prices and surcharges can be entered manually for every item; however, definitions in the master data are also useful for this purpose. |
| **Reset price changes** | Item input allows you to undo manual price amendments in general. The menu **Functions > Delete preset item prices** is used to delete manual price amendments for an item. The menu **Functions > Delete item settings** resets the changes to the master data entries. |
| **Prevent price changes** | Manual amendment of prices in the order can be protected by a password. |
| **Default settings** | **Master data:** Surcharges, Roundings. **Company data:** Documents tab (minimum price not met), Pricing tab. |

## Display of Prices in the Dialog

When you enter a product in the document, the prices will be adopted from the master data.

*(Image: Fig. C-68 Item prices display, showing an annotated screenshot of the item entry screen.)*

*   **A** Total order price
*   **B** Price and price unit per component
*   **C** Item price per unit in purchasing
*   **D** Item price in sales
*   **E** Item price per item (only main product), including discount
*   **F** Discount applied to price per piece
*   **G** Unit price per item
*   **H** Price per price unit

This example shows how the current prices are calculated and displayed at item entry:

*   The item price of the main product (G) is based on the calculated quantity (surface), the unit price (H) and the discount (F).
*   The unit price (G) per item consists of the item price for the main product (E), the price for additional components, e. g. grills, shape, processing and, if applicable, the replacement surcharge (B).
*   The replacement surcharge (B) shows the amount per calculated quantity.

### The order value is displayed in the Totals tab.

*(Image: Fig. C-69 Display of prices, showing an annotated screenshot of the Totals tab.)*

*   **A** Total of orders for this customer
*   **B** Order total in the national currency + foreign currency
*   **C** Manual setting for fixed price and discount
*   **D** Tax amount
*   **E** Gross amount
*   **F** Down payment amount
*   **G** Enter down payment
*   **H** Costs (after feedback from capacity planning or production)

## Prices and Price Calculation

Prices, surcharges and discounts are adopted from the master data and can be changed per item and order manually. Order total and item totals are updated automatically. Manually amended entries are shown in red.
Prices can be printed as net or gross prices.

> **Adopt prices from the master data**
> Basically, prices can be adopted from the master data only if the code **price-relevant** has been set in product management.

### Manual change of price

The price change of an item always refers to the main product. If you change the price of a BOM component, the new price will be added to the main product.

Predefined prices can be changed on the following levels:
*   Price year and price key
*   Price per price unit
*   Fixed price for one piece of the item
*   Fixed price for the entire item
*   Fixed price for a group of items
*   Fixed price for the entire order
*   Price of a BOM component
*   Discounts

To show the item price without discounts and individual prices, the option **Extended pricing** must be set in the company data. The displayed data will not be processed further. This field only serves for report analysis.

## Calculation settings

Various settings can be made for price calculations. Pricing parameters are generally defined in the company data and can be changed for each individual order.
In addition, you define in the product and BOM in the order how the individual prices should be displayed in the calculation:
*   **Implicit:** The main item's price includes all prices of the BOM components; i.e. this includes shape and replacement surcharges as well as processing.
*   **Explicit:** The price will be shown separately.
*   **Implicit, price per quantity unit:** The prices of the BOM components are converted to the main product's price unit. This total price of the price unit is shown in the document, but only if all BOM components of the item have been assigned with the same display type.

**Example: Show implicit price in price per QU**
In this example, a float sheet of 5 mm, 1000 x 2000 mm with two drill holes has been entered. The glass price is €10/sqm. For the drill holes, €5 /pcs. are calculated; the price code is set to implicit.
This results in the following calculation:

| Description | Calculation | Result |
| :--- | :--- | :--- |
| Total price for glass | | € 20 |
| Total price for drill hole | | € 10 |
| **Total price** | €20 + €10 | **€ 30** |
| ÷ Total sqm | | ÷ 2 |
| **Price/sqm** | €30 / 2 | **€ 15** |
| **Total price per sqm** | | **€ 15** |

The price for drilling is included in the price/price unit of the main product (in this case, glass -> sqm) (implicit).

## Fix prices

If orders are handled by different persons in your company, you can fix the prices for an order. They will then be locked for further editing. The order itself can still be edited. You can also fix entire order items.

### Updating order totals

Item totals can be updated right away or when the order is saved.
If prices are changed, totals have to be recalculated. Since this is not done automatically based on the set flag, recalculation must be enabled via the function **Force recalculation of totals**.

If product and price definitions are changed in the master data, the new data will not be automatically transferred to existing documents. The menu **Recalculate** offers various options for defining the data to be reloaded and the values that are to be recalculated in the corresponding documents.
The document will be checked for duplicates before recalculation. If duplicates are found, recalculation will be aborted.

> **Start recalculation after consultation**
> Please ask your contact at A+W Software GmbH for assistance before using the recalculation function for the first time.

## Price recorder

The price recorder lists the manual prices of individual order items. Within a defined period, price conditions for quotations and orders (including archived ones) will be used. When searching, the price recorder distinguishes main product and BOM level.
This way you can create a quotation based on previously granted terms.
The search result depends on the start position from which you call the price recorder:
*   **BOM components:** If you have selected a replaced, patterned glass sheet in the BOM, for example, and start the price recorder, the system will only search for this patterned glass as part of a BOM.
*   **Main product:** If you start the price recorder on tab **IG** or **Article**, the program will search for this article or IG only on the main product level.
*   **Product structure:** You can also activate a filter to take the product structure into account.

The resulting price conditions can be adopted for the current item. Manual prices and discounts must be confirmed separately.

*(Image: Fig. C-70 Price recorder, showing the price recorder dialog with various filter options.)*

*   **A** Restriction to document type
*   **B** Restriction to archive years
*   **C** Restriction to entry period

All price conditions the price recorder finds for a product can be printed. The price recorder shows the product number as well as the input date of the document, the price/PU, discount, document and item number, and the product size.

## Formulas

Price formulas can be defined in price master data. These will be applied for price calculation in the document. Formula-based pricing is used for item prices and BOM component prices.

*(Image: Fig. C-71 Price formula selection, showing the formula editor with a list of available formulas and their code.)*

**Alternatives**
The price for alternative items (in the quotation) is not part of the order total.
Calculation of alternative quotations also calculates the automatic surcharges.
Quotations will be introduced in a separate training module:
⇨ "Quotations" on page C-323

## Definition of Minimum Values

The following minimum values can be defined for calculation purposes:
*   **Minimum order value:** If a minimum order value has been defined in the customer master data, the order totals will be calculated accordingly.
*   **Minimum invoice amount:** A minimum amount per invoice can be defined in the customer master data.
*   **Invoicing surcharge:** An invoicing surcharge can be defined in the customer master data for a minimum amount per invoice.
*   **Minimum price:** If the customer's standard price is not met after manual changes have been made, the difference will be displayed. You must enter a reason for the new price. Falling short of the minimum price can be password-protected.

A change of rate is no change of price; therefore, you do not have to enter a reason for this.
Reasons can be listed in a report. After printout, you can reset the print code; the items are no longer listed on the next printout.
This function is available when extended pricing is active.

## Surcharges and Services

Automatic surcharges will be added as the last order item and will be included in the calculation of the total.
All items will be recalculated if a surcharge or discount is enabled or disabled in the document header.
Calculation of surcharges and services can be changed to rounded quantities (surface). This setting can be changed in the order if calculation shall be based on the actual surface. You must enable the option **Price unit sqm (act.)** for this.

## Changing the Item Price

You can change both the amount and the price unit in an order. These changes only apply to the selected item. This module will show you how to change the prices, discounts and surcharges for an existing item.
The following instructions exist for this training module:
*   "How to change an item's unit price” on page C-144
*   "How to change the price of a replacement sheet" on page C-146
*   "How to change the price information of a BOM component" on page C-147
*   "How to change a grill price” on page C-148

### How to change an item's unit price

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Select the item for which you want to change the price.
    The unit price of an item can be changed as follows:
    *   Amend the unit price or value in the field **Sales price** to define a fixed price.
    *   Change the key, the unit price, the unit and/or the discount in the input line.

In the following example, we will change the prices in the input line.

*(Image: Fig. C-72 Change unit price of item, showing the item list with columns for price settings.)*

*   **A** Price Year
*   **B** Price key
*   **C** Price per price unit
*   **D** Price unit
*   **E** Discount
*   **F** Unit price of item (glass)

3.  Select one or more of the following options from the input line:
    *   **In the field Price list (A):** By changing the price list (year), you must ensure that the selected price list has been assigned to a key.
    *   **In the field Key (B):** Changing the price key will change all related definitions.
    *   **In the field Price/PU (C):** Changing the amount only affects the main product; replacement surcharges etc. will remain unchanged.
    *   **In the field Unit (D):** Changing the price unit only affects the main product. You cannot enter fixed prices for the item this way.
    *   **In the field Discount (E):** Changing the discount rate only affects the main product; discounts on BOM components will remain unchanged by default.
        Exceptions: You can define that the discount defined in the company data shall be adopted for replacement glass and all BOM components.

*(Image: Fig. C-73 Price change of item, showing the price fields highlighted in red after being amended.)*

Amended entries are shown in red. The fields in the section **Sales prices** will be updated.

4.  Click on **[Save]** to save the data.
    The prices are saved. The values in the **Totals** tab are updated.

### How to change the price of a replacement sheet

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.

*(Image: Fig. C-74 Changing the price of a replacement sheet, showing the Sales price section for a BOM component.)*

*   **A** Price for replacement sheet
*   **B** Replacement sheet

2.  Select the replacement sheet on the BOM (B).
3.  Change the price and/or price unit (A) as required.
    Amended entries are shown in red. The fields are updated.
4.  Click on **[Save]** to save the changes.
    The prices are saved. The values in the **Totals** tab are updated.

## Edit BOM Component Price

The price change of a BOM component will be added to the main product and results in a new unit price for this item.
The following instructions exist for this training module:
*   "How to change the price information of a BOM component" on page C-147
*   "How to change a grill price" on page C-148

### How to change the price information of a BOM component

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Go to the tab **BOM**.
3.  Select the component for which you want to change the price information.

*(Image: Fig. C-75 Changing a component price, showing the BOM tab with detailed pricing information for a selected component.)*

*   **A** Price information on the selected component
*   **B** Changing the price code

4.  Change the entries in the section **Pricing (A)** as required, e. g. the price list.
    If you want to change the surcharge type, please follow the instructions and examples in the section **Master data**.

Amended entries are shown in red.
5.  Click on **[Save]** to save the data.
    The prices are saved. The values of the BOM and item prices and the values in the **Totals** tab are updated.

### How to change a grill price

1.  Select **Documents > Order > Select order > Items tab** or **<F9>**.
    Item entry opens.
2.  Enter a new item or select the item for which you have entered grills.
3.  Go to the tab **Grills**.

*(Image: Fig. C-76 Changing the grill price, showing the Grills tab interface for defining a grill pattern.)*

*   **A** Prices tab (grills)
*   **B** Price settings from product definition

The section **Prices (B)** shows the grid price for the entire grill pattern. You can change this price to define the total price (unit price) for the grid.
4.  Go to the tab **Prices (A)**.
    The default prices for the grill are displayed.

*(Image: Fig. C-77 Changing a price in the grill pattern, showing the Prices tab within the Grills section.)*

*   **A** Individual prices of the grill pattern
*   **B** Price per price unit

5.  Change the prices and price units as required.
    *   In the section **Grid**, the prices of the individual elements of the pattern. Ensure that you enter the details for horizontal and vertical grills separately.
    *   In the section **Prices**, the rate, the price unit and/or the discount.
    *   In the section **Grill article**, the price per price unit.

    Amended entries are shown in red. The fields in the section **Prices** are updated.
    You can reset the changes to the default values using the menu **Functions > Settings**.

> **Change grid price**
> The price in the section Prices refers to the entire grid. If you change this price, you need to take into account the quantity (LM) of grills.

6.  Go to the menu **Start > Save** to adopt the changes.
    The display changes to the **Item** tab.

7.  Go to the menu **Start > Save** to save the item.
    The values of the BOM and item prices and the values in the **Totals** tab are updated.

## Enter Fixed Price

In every order, the regular prices can be changed into fixed prices. A fixed price may refer to a part of an item, to the complete item or to the entire order.
The following instructions exist for this training module:
*   "How to define a fixed price for the entire order" on page C-151
*   "How to define a fixed price for an item" on page C-152
*   "How to define a common fixed price for several items" on page C-153
