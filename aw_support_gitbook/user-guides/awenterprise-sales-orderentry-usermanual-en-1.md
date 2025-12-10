---
title: "EN-UM-AWEnterprise_11"
source: "EN-UM-AWEnterprise_11.pdf"
tags: ["A+W Enterprise", "Sales", "Order Entry", "BOM", "ERP", "Software Tutorial", "User Manual", "Technical Documentation", "Item Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial section from the A+W Enterprise Sales user manual, focusing on entering new items, managing orders, and using various product-specific entry methods. It covers topics like item entry by customer description or article number, editing item properties, managing Bill of Materials (BOM), and handling different product types such as glass, LAMI, and IG."
long_description: "This document is a comprehensive tutorial for the A+W Enterprise Sales module, providing step-by-step instructions for managing orders and items within the system. It begins with the fundamental processes of entering new items, either by customer description or by a specific article number. The guide details how to handle various data fields like quantity, width, height, and price, and explains system prompts for features like SN-Auto (Shape and Nesting). It extensively covers the Bill of Materials (BOM), explaining how to view, edit, add, and copy articles within the BOM structure. The manual addresses particularities for different product types, including stock items with variants, float/basic glass, tempered glass, laminated glass (LAMI), and insulated glass (IG). Specialized entry procedures are also detailed, such as entering shapes, muntins, and stepped glass units (iTOE). The document also covers related sales functions like product replacement, entry without prices, creating delivery notes, invoices, and managing order releases. It serves as a practical guide for users to navigate the complexities of order creation and modification within the A+W software environment. The document is divided into a tutorial section and a software reference section, which includes a detailed table of contents and descriptions of various menus, dialogs, and functions."
---

# Tutorial: Orders

---
## Enter new items

### Here's how to enter an item by customer description

You can enter the item description defined by the customer after selecting **Item** in the header, field **Cust.Item**.

*⇨ Sales, "Cust. Item" on page D-1137*

1.  Enter the new item text in field **Cust.Itm**.
    The text can exceed the visible field length. It can be a free text.
2.  Confirm your entry with `<Enter>`.
    The cursor jumps to the **Article** field.

### Here's how to enter an item with article number

> **UI Screenshot Description:** The image shows the item entry screen in A+W Enterprise. The screen has tabs for "General", "Properties", "Prices", "Status", and "Costs". The item grid includes columns like "Itm", "Cu.ltm", "Article", "BMno", "Qty.", "Width", "Height", "SN", "Comm", "PType", "kg/Pc", "EUR/Qty", "Sender", "Qt Total", "Discount", "Net Total", "+VAT", and "Gross". Buttons at the bottom include "Attachments(0)", "Copy Item", "BOM", "Save", "OK", and "Cancel". The cursor is currently in the "Article" field.

This is where you enter the individual articles (items) of an order.

The cursor is on the **Article** field in order entry. The descriptions for fields that are not present when you enter the dialog are shown dynamically, depending on the properties of the article entered, e.g. for a double IG article, the fields are called **Width/Height/AIR**.

1.  Enter or select the article as follows:
    *   Enter the article number (if known) in field **Article**.
    *   Or press `<F9>` to search for the article number or using other criteria.
    *   Or press `<F8>` to search by matchcode.
        *⇨ Sales, "Find article" on page D-1097*
    *   Select the required article using `<arrow keys>` + `<F3>` or using the mouse.
    *   Confirm your entry with `<Enter>` or a double-click.
    *   For item entry according to particular product groups, see the following chapter:
        *⇨ Sales, "Entering items (depending on product type)" on page D-1007*
    *   Press `<Enter>` to move the cursor to the **Quantity** field.
2.  If you are using SN-Auto, the system will ask: `Do you want to have the system create the SN file for this item?`
    *   Choose **[YES]** if you want A+W Enterprise to create an SN file in the background.
    *   Choose **[NO]** if you do not need an SN file, or if you want to start SN directly from order entry.
3.  Enter the quantity in field **Quantity** and decide whether you want to change the product structure in the BOM.
    The cursor jumps to the **Width** field.
4.  If you are working with iTOE, note the following description:
    *⇨ Sales, "Stepped entry" on page D-1022*
5.  Enter width and height and confirm with `<Enter>`.
    Field **AIR** (airspace) needs to be filled in for IG.
6.  A+W Enterprise opens the **Processings** dialog if you have entered products that include processings. Alternatively, you can attach additional processings to the desired article:
    *⇨ Sales, "Complex steps in the BOM editor" on page D-1014*
    Specify the necessary processing steps in this dialog.
    You can open the **Processings** dialog anytime with `<Ctrl>` + `<F8>` in the fields **Width**, **Height** or **Price/pc**.
7.  For muntin entry, see the following chapter:
    *⇨ Sales, "Muntin entry" on page D-1018*
8.  For step entry, see the following chapter:
    *⇨ Sales, "Stepped entry" on page D-1022*
9.  For BOM editing after the fact, see the following chapter:
    *⇨ Sales, "Edit BOM" on page D-1010*
10. The **Comm** field is already pre-populated from the master data if you are working with commission calculation within the A+W Enterprise program. In this case, you can change the commission rate with `<F9>`. Otherwise, the field will be skipped.
    *⇨ Master Data, "Commission" on page B-503*
11. The **P.type** field is also pre-populated from the master data. You can change the procurement type depending on the order. To do this, press the `<Spacebar>` until you reach the desired value and confirm your selection with `<Enter>`. However, note that the change of the procurement type can cause various other changes and possibly make other details necessary.
    Then A+W Enterprise calculates the values for the fields **QU/pc** and **kg/pc** and the price details and inserts these into the item.
12. Complete the item in the **Price/pc** field as follows:
    *   Use `<Enter>` or `<F6>` to enter additional items.
    *   Use `<End>` to save the order and go to the order footer.
    *   Define the article as a fixed-size customer product if your customer frequently orders articles of the same size.
        *⇨ Sales, "Article details for dimensioned variants" on page D-1214*
    A+W Enterprise will ask for further input if necessary. This can be processing parameters (drilling diameter, radii for rounded corners, etc.) for processed glass, or the article color.
    Usually, the item list on tab **General** is sufficient as A+W Enterprise loads all other entries from master data.

### Here's how to add additional items

You can add new items to an order after the fact. Generally the items are added after the items already entered. In rare cases, you can also add new items between existing items. In this case, please note that the item number (kpos.posnr) will no longer be assigned in ascending order and the sequential number (kpof.Ifdpos, **General** tab > **Item** field) will be renumbered. The same number assignment process applies as for canceled items.

1.  Position the cursor on the **General** tab on the line above on which you want to insert a new item.
2.  Press `<F6>` to add a new item at the end of the existing items.
3.  Press `<Shift>`+`<F6>` to add an item between existing items.
4.  Enter the new item.
    *⇨ Sales, "Here's how to enter an item with article number" on page D-1001*

### Here's how to edit the properties of individual items

Some details of an item entered can be changed depending on the order. This way, you can edit the **Prod.description** or **Cost center** on the **Properties** tab after the fact.

*⇨ Sales, "Order entry - properties" on page D-1178*

1.  On the item level, press `<F2>` on the **General** tab.
    The **Properties** tab appears. A+W Enterprise pre-populates the fields with data from the article master data or the existing system configuration.
2.  Press `<F5>` to enter the fields on the **Properties** tab.
3.  Make the change. Note the possible consequences of the correction made:
    *   The changed **Description** will be transferred to production and printed on the relevant papers.
    *   The changed **Cost center** affects the cost center statistics.
    *   For articles in stock, the stock removal will be taken from another **Stock** in case of change.
    *   In the **CAD file** field, you can attach a new S/N or DXF file (with `<F9>`). With this change, you can adjust the BOM. For this, you have to answer the question about whether the BOM should be synchronized with **Yes**.
    *   Depending on the system configuration, in the **DP number** field, you can determine a new declaration of performance from the master data (`<Ctrl>`+`<R>`), set according to structure (`<Ctrl>`+`<L>`), generate by inputting technical values (`<Ctrl>`+`<T>`) or select freely (`<F9>`/`<Ctrl>`+`<K>`).
    *   The change by a system configuration default value **Sketch print** value causes changes to the forms.
4.  Use `<End>` to return to the **General** tab.
    Or use `<F 2>` to switch to another tab.
    Or use the `<Page Down>` key to reach the new item on the **Properties** tab.

### Here's how to change supplier-related data

You can change the supplier and the delivery time for an existing item after the fact. If you re-enter a supplier for an item already entered, the Procurement type of this item is automatically set to PO. And vice-versa, the specification of the Supplier is required insofar as the Item procurement type is set to PO.

1.  After specifying the article number, you can press `<Shift>` + `<F12>` from any field on the **General** tab.
    The fields **Supplier** and **Deliv..time** appear temporarily.
2.  Enter the supplier or select it from the list with `<F9>`.
3.  Enter the delivery time in days, in field **Deliv..time**. Via a corresponding system configuration, you determine whether this specification is made in **Days** or in **Hours**.
4.  Answer the following questions with **[Yes]** or **[No]**.
    *   "Recalculate the order?"
        The type of calculation that can be executed. The following selection is possible with the `[Spacebar]`.
        *   No new calculation
        *   Sales and purchase prices
        *   Sales prices
        *   Purchase prices
    *   Use the supplier for the entire order?
        All previously entered items with procurement type PO get this supplier insofar as you answer this question with **[Yes]**. Then the next question is posed.
    *   Use the new supplier for this item only?
        *   If you answer this question with **[Yes]**, the new supplier is only taken over in items whose procurement type=PO.
        *   If you answer this question with **[No]**, the new supplier is taken over in all items and the procurement type of all items is set to PO.
    *   Do you want to use the new supplier for the items below?
        *   The new supplier is also taken over into the newly entered items.
5.  Close item entry.

### Here's how to enter a shape in the item

You can enter a shape in the item. Normally, shapes are entered for a new order. Changes after the fact for an existing item for a shape is only possible until production has begun. Note that shape information also influences rack planning.

1.  Press `<Ctrl>` + `<F12>` on the **General** tab.
    The **Shape** field appears temporarily.
2.  Enter the shape number.
    Or press `<F9>` in the **Shape** field and select a shape number from the list.
    Or press `<F2>` in the **Shape** field and select a shape from the **Shapes** dialog.
    An entry dialog for the selected shape number opens automatically.

> **Shape catalog**
> With a system setting, it is determined which shape catalog is available in the entire program. The default setting is the **A+W Shape Catalog**. To configure another catalog, contact an A+W employee. It is not possible to use several catalogs.

3.  Enter the shape sizes on the **Shape sizes** dialog.
4.  To depict a shape geometrically or be able to produce it, there are various restrictions per shape.
    e.g. W2 + W1 >= W.
    If you have violated the dimensions of the shape restriction, a notice will appear. You must correct the entry in order to exit the dialog.
5.  The shape number is taken over into the item. In the sketches area, a schematic shape depiction appears. The item includes a shape icon.

> **UI Screenshot Descriptions:**
> 1.  The first image shows the "Shape-dimensions" dialog for a trapezoidal shape (shape 5). It has input fields for W (1200), H (1140), W1 (140), and W2 (250). It also lists geometric constraints like W > W1+W2.
> 2.  The second image shows the "Order Entry" screen. The item list now shows an item with "shape 5" entered. A small icon representing the shape is visible in the item line.

6.  Close item entry.

## Entering items (depending on product type)

There are a few particularities with the entry of some product types. The item entry is determined by a series of various criteria, e.g. how many parameters and which parameters are required for entry, or in which quantity units the product is sold or produced, etc. In the following chapter, you will learn about some of the particularities during item entry.

### Here's how to enter stock items with dimensional or color variants

Stockplates are defined as stockplate variants in article master data. All available size variants of a glass type (of the same thickness) are listed under the same article number. The dimensional variants available in the system are described in the following chapter:
*⇨ Master Data, "Dimension variants" on page B-299*

The color variants are also generally kept in stock. E.g. a red color exists in a bucket with 5 liters, 10 liters, and 15 liters. For the dialog description, see:
*⇨ Master Data, "Color variants" on page B-296*

The description of the dimensional variants is also available in the master data:
*⇨ Master Data, "Size variants" on page B-302*

The entry of all stock variant articles differs from glass entry in that here an additional field for the selection of the variant appears.

1.  Start the order entry and enter the order up to the **Article** field (item level).
2.  Enter an article number for the stock sizes of the required glass in field **Article**.
    Or select an article with `<F9>` selection. There is no possibility to search only for variants (dimension, size, color) articles on the Article Search dialog. Filtering by appropriate article types, e.g. stock dimension article types, can also help.
3.  After you have entered the quantity, a selection of available stock size variants appears.

    > **UI Screenshot Description:** The "Variant Selection" dialog is shown. It lists available variants for an article, with columns for "Code", "Type", "Variant", "Stock Desc", "Stock", and "Supply". It shows different dimensional variants (e.g., 200.0 x 321.0) and their current stock levels.

    The stock for all available article variants across all warehouses is displayed totaled up on this dialog. Negative stock means that currently there are more removals than additions booked in the system.
    Choose a stock size variant and confirm with `<Enter>`.
4.  Proceed with the item input as usual.

However, the stock is not updated from item to item. The removals from stock are only done when the stock booker has finished processing.

A+W Enterprise takes over the dimensions for the selected variant in the fields **Width** and **Height**.

### Here's how to enter a float or basic glass

Glass articles with article type 100, 170, and 180 are marked as float or basic glass. Enter the item as described in chapter:
*⇨ Sales, "Here's how to enter an item with article number" on page D-1001*

Please note the following differences.

Basic glass (float) can be entered in different ways:

*   **As stock dimension.**
    *⇨Sales, "Here's how to enter stock items with dimensional or color variants" on page D-1007*
*   **An unprocessed fixed dimension**
    *   Select an article. Alternatively, start the `<F9>` search and filter out all articles with the article type=170.
    *   Enter the quantity.
    *   Enter width and height.
*   **As processed fixed dimension**
    *   Select an article. Alternatively, start the `<F9>` search and filter out all articles with the article type=100.
    *   Add the processings.
    *   Enter the quantity.
    *   Enter the sizes.

### Here's how to enter tempered glass (single-lite safety glass)

Enter the item as described in chapter Tutorial, "Here's how to enter an item with article number" on page D-1001. Please note the following differences.

Tempered glass can be entered in different ways:

*   **As unprocessed tempered glass**
    *   Select an article.
    *   Enter the quantity.
    *   Enter width and height.
*   **As processed tempered glass**
    *   Select an article.
    *   Add the processings.
    *   Enter the quantity.
    *   Enter the sizes.

### Here's how to enter LAMI (laminated glass)

Entering laminated glass items is very similar to entering float glass. A specific feature can be colored film that can be added to the BOM.

> **Pay attention to the assembly position of the lite**
> The lite surfaces of multi-lite safety glass are counted from the outside to the inside (= assembly position). Please note the assembly position when you change the BOM.

Enter laminated glass as described in:
*⇨ Sales, "Here's how to enter an item with article number" on page D-1001*

### Here's how to enter IG (insulated glass)

IG comes in a multitude of variants. The products can consist of different glass types (float, tempered, laminated) and different thicknesses. Basically, IG is entered in just the same way as other product groups.

Enter IG as described in:
*⇨ Sales, "Here's how to enter an item with article number" on page D-1001*

You can also enter muntins for IG units.
*⇨ Sales, "Here's how to operate muntin entry" on page D-1018*

### Here's how to enter units or quantities

Input of units requires no sizes.

Enter units as described in:
*⇨ Sales, "Here's how to enter an item with article number" on page D-1001*

### Here's how to enter hour articles (working time)

When you enter hour articles, you have to define the multiplier in field **Qty**. The unit is entered in hours.

Enter hour articles as described in:
*⇨ Sales, "Here's how to enter an item with article number" on page D-1001*

### Here's how to enter a colored article

Entry of a colored article differs from the entry of variant articles only in the selection of the color instead of dimensional variant.

## Edit BOM

**Objectives**
*   Get to know BOM concept.
*   Possibility to adjust BOM customer-specifically.
*   Learn how to simplify operation.

**Benefits**
*   A customer-specific adjustment of the product structure can be made directly in the order and calculated.

**Note**

*   **Original BOM**: Product structure in which the master data can be specified.
*   **Curr. BOM**: If the BOM consists of several levels, on the first tab of the BOM dialog, you will see the listing of the current level.
    *⇨ Sales, "Processing param. (short) tab" on page D-1261*
*   **Processing parameter (short)**: On the second tab of the BOM dialog, you will see the display of important processing parameters that can generally also be changed. Which parameters are displayed here depends among other things from the processing type. A complete listing of all parameters for the processing in question is on the `[F5]` dialog.
    *⇨ Sales, "All parameters/sketch tab" on page D-1263*

To consider specific customer requests during document entry, the original BOM is taken over into the document automatically and it can then be changed order-specifically without causing changes that will affect the original BOM. You can replace lites with others, add processing steps, choose alternative material, etc. All BOM changes will only refer to this copy. The original BOM will remain unchanged in master data.

Whether or not the BOM tree can be changed during document entry can be defined in the article master data - this also depends on the user rights. If the change is allowed, a component can be replaced by another equivalent component in this BOM or additional components can be added.

The BOM structure of an item is automatically transferred to the following item if you enter the same item number. The BOM number can be changed. You can also display the BOM and edit it.
*⇨ Master Data, "BOM" on page B-478*

All changes to the BOM must be made carefully. Incorrect actions can cause other problems, including a program crash.

The **Edit BOMs** chapter includes the following information:
*⇨ Sales, "General steps in the BOM" on page D-1012*
*⇨ Sales, "Complex steps in the BOM editor" on page D-1014*

### General steps in the BOM

You can view the BOM of an item in nearly any document type. To do this, you need to start the BOM editor for the item in question:
*⇨ Sales, "Here's how to mark the BOM for the processing" on page D-1012*

The extent to which the BOM can be edited and changes saved depends on various criteria, such as user rights, article master data, document type, and document status.

#### Here's how to mark the BOM for the processing

To be able to open the BOM editor, the article entered must be dimensioned completely. During the dimensioning, the program automatically determines relevant parameters and writes them to the order BOM. As long as this dimensioning is not complete, the BOM editor for opening can only be marked. This is the case if the cursor is in the order entry in the **Quantity** field of the item to be changed:

1.  Use `<F3>` to load the BOM.
    A+W Enterprise informs you that the BOM is now marked for the processing and the BOM editor is opened after complete dimensioning. After entry of the necessary parameters, such as Width/Height/AIR, the program opens the BOM view.
    *⇨ Sales, "BOM view" on page D-1249*
2.  Choose the article you want to change. If necessary, use `<F3>` or a mouse-click to open additional BOM levels with the plus node.
3.  Press `<F5>` to open the BOM of the relevant BOM level for processing.
    A+W Enterprise opens the BOM editor.

#### Here's how to open the BOM editor or BOM view directly

You can open the BOM editor directly in the following cases:

*   With `[F5]` from the fields **SN**, **Comm** (Commission), **P.type** (procurement type)
*   With `[F5]` from the fields **Quantity**, **Width**, **Height**, (**AIR**) if the item was already entered completely.

The same applies for the BOM view, which can be reached with `[F3]`.

Use `<F2>` to change to the next tab in the BOM.
*⇨ Master Data, "BOM" on page B-478*

#### Here's how you can change an article in the BOM

You can change items or product structure during order entry, i.e. before the order is saved.
Once an order has been saved, it can only be corrected.
*⇨ Sales, "Change/correct order" on page D-997*

1.  Open the BOM editor.
    *⇨ Sales, "Here's how to mark the BOM for the processing" on page D-1012*
2.  Override the article number in field **Article** with the new article number or select an article number with `<F9>`. The program sets the code **E** (exchange) in the **Print** field automatically. This code can affect the item price.

    > **Only exchange identical article types**
    > You can replace an article only with an article of the same type.
    > Example: Replacing glass with a processing step would be nonsense. You have to define the corresponding technical restrictions in article master data so that A+W Enterprise issues a warning.
    > *⇨ Master Data, "Article" on page B-377*

3.  Confirm the new article number with `<Enter>`.
    A+W Enterprise updates the name and all other fields.
4.  Close the dialog with `<End>` to save the changes you have made. Use `<Home>` to reject the changes.

#### Here's how to add a new article to the BOM

If necessary, you can also add new articles to the BOM.

1.  Open the BOM editor.
    *⇨ Sales, "Here's how to mark the BOM for the processing" on page D-1012*
2.  Navigate to the BOM level on which an additional article should be added.
3.  Use `[F6]` to create a new line in this BOM level.
4.  In the **Article** field, enter the number of the new article if you have it handy. Alternatively, select the number from the `[F9]` selection.
    If several completely entered articles (e.g. processings) should be added, the program offers additional steps to simplify entry, which will be described in the next chapter.
5.  Close the dialog with `<End>` to save the changes you have made. Use `<Home>` to reject the changes.

### Complex steps in the BOM editor

The A+W Enterprise offers a series of possibilities for making complex changes to the BOM quickly. Please note that some steps described here may depend on the configuration. If necessary, contact the responsible A+W employee.

#### Here's how to add more articles at the desired location of the BOM

You can add new data records to the BOM, also to a particular location. The sequence of the articles can be important if, for example, the processings are based on a production machine one after another.

1.  Open the BOM editor.
    *⇨ Sales, "Here's how to mark the BOM for the processing" on page D-1012*
2.  Position the cursor in a BOM record so that a new article can be inserted above this data record:
    Press `<Shift>`+`<F6>`
    The new record is added above the marking.
    You can now enter the new additional article.

    > **Sequence of articles in the BOM**
    > The BOM article sequence does not necessarily match the production sequence. ERP and production systems must be attuned to one another.

3.  Save the BOM with `<End>`. Under some circumstances, a new BOM number may be assigned here.

#### Here's how to copy articles already entered

It frequently happens that in a BOM several nearly identical processings must be entered that differ only in one parameter. In such cases it can make sense to enter the processing in question once completely, then to copy it several times and change the relevant parameter.

1.  Open the BOM editor.
    *⇨ Sales, "Here's how to mark the BOM for the processing" on page D-1012*
2.  Insert a new processing into the BOM.
3.  Keep the cursor on the data record with the processing.
4.  Press the **Copy** button (if the buttons for BOM editing do not appear, they must be configured appropriately).
5.  Create a new data record using the **New** button or `<F6>`.
6.  Press `Ins.` [Insert]. The processing in question is added with all parameters.

> **Applicability of the clipboard**
> Please note that the copied article is only available as long as you are in the BOM editor. If you exit the BOM, the clipboard is emptied. If, however, you would like to insert the copied article into another BOM level, follow the program instructions and other descriptions:
> *⇨ Sales, "Here's how to copy already entered processings to another BOM level" on page D-1016*

7.  Save the BOM with `<End>`. Under some circumstances, a new BOM number may be assigned here.

#### Here's how to have the BOM number changed by the system

You can allocate a new BOM number to an article and keep the BOM structure. This makes sense for example if you want to print article text for this item again, or print changed article text.

1.  To change the BOM number, enter a new BOM number on the **General** tab in the corresponding item, field **BOM**.
    Or on the **General** tab in the corresponding item, field **Article**, **BOM** or **Quantity** `<Shift>` + `<F5>`.
    The BOM number will be changed.

#### Here's how to assign a new item the original BOM

When you enter a further new item, you can allocate the original BOM defined in master data.

1.  To allocate the original BOM, press `<F5>` on the **General** tab in this new item, in the **Article** field.
    The original BOM will be allocated to the new item.

> **Original BOM for already entered items**
> You cannot allocate the original BOM to an already entered item because you will not be able to access the field **Article**.

#### Here's how to copy the completely entered processing to another glass

> **UI Screenshot Description:** The "BOM View" dialog is shown. It displays a hierarchical "Product Structure" on the left and a "Current BOM Level" table on the right. The table lists articles like "A+W Float 5mm", "A+W Float cutting", and "A+W Cut-off corner refined". Checkboxes for "Cop" (Copy) are visible, allowing users to select items for copying.

You can transfer a completely entered processing to another glass in the BOM. This way, you can insert several processings in the BOM from one level to the other in order to enter several processings with many parameters more easily and faster.

Frequently it happens that you must enter several almost identical processings in a BOM, which only differ in one parameter. In such cases it can make sense to enter the processing in question once completely, then to copy it several times and change the relevant parameter.

For both use cases, A+W Enterprise offers entry aids:

#### Here's how to copy already entered processings to another BOM level

1.  Open the BOM editor.
2.  Insert a new processing into the BOM, enter this processing completely.
3.  You can first enter several processings completely in order to transfer them together to another glass.
4.  Use `<F2>` to change to the **Processing param. (short)** tab.
5.  Mark the processings that should be transferred by activating the **Cop** (copy) checkboxes for the relevant processings (this function must first be released).
6.  Copy the processings using the **[Copy]** button or with the key combination `<Ctrl>` + `<B>`. The changes to parameters that are made now are no longer intended for transfer.
    If you only mark the processings and do not copy them, you will be made aware of this when changing the BOM levels.
7.  Change to the BOM level to which the marked processings should be transferred. Here you will be asked whether you actually want to transfer the marked processings to another level. Only if you answer this question with yes will the clipboard at the destination be available.
8.  Create a new data record using the **[New]** button or `<F6>`. Please note that the processings of the BOM to be copied are attached (with `<F6>`) and not inserted (with `<Ctrl>`+`<F6>`).
9.  Press the **[Insert]** (insert) button or use the key combination `<Ctrl>` + `<O>`. The relevant processings will be added with all parameters.
10. Change the necessary parameters if necessary.
11. Save the BOM with `<End>`. Under some circumstances, a new BOM number may be assigned here.
12. Repeat steps 7 and 11 if you want to add the marked processings to additional BOM levels.
13. Leave the BOM editor and save.

## Muntin entry

**Objectives**
*   Get to know muntin entry in orders.
*   Recognize the possibilities and limitations of A+W Enterprise muntin entry.
*   Get to know the possibilities and limitations of the A+W CAD Designer (Bars) muntin entry.

**Benefits**
*   Muntins are fixed components of a window or a lite. Entry of the correct muntin structure is important and indispensable for production.

**Note**

*   **Muntin/muntin bar**: A muntin is a muntin bar in a whole structure.
*   **Muntin pattern**: A muntin pattern is the entire structure of all muntins that are installed in a frame or glued to a glass.
*   **Glass dividing muntin**: This term comes from the window industry.

Generally muntins are installed directly in IGUs. Muntins are thus a component of the IG BOM and only permissible for IG. An exception are glued muntins. However, these are generally included and installed during window manufacturing. In A+W Enterprise you can enter simple muntin patterns directly in the order. More complex structures are so-called Macros, e.g. Sun; these must be entered in other programs, e.g. A+W CAD Designer (Bars) and then transferred to A+W Enterprise and they can no longer be changed there. If you have questions about A+W CAD Designer (Bars), contact the responsible A+W employee.
*⇨ Sales, "Muntin entry" on page D-1281*

### Here's how to open muntin entry

1.  Enter an IG item.
    *⇨ "Here's how to enter IG (insulated glass)" on page D-1009*
2.  After entering the sizes, use `<Shift>` + `<F8>` to load **Muntin entry** or click on the **[Muntins]** button to open **Muntin entry**.

### Here's how to operate muntin entry

1.  Open **Muntin entry**. The fields for the dialog are described in the following section:
    *⇨ Sales, "Muntin entry" on page D-1281*
2.  Enter an article number of article group 57*** in field **Muntin** or select an article number with the search function `<F9>`, `<F8>`.
    Confirm your input with `<Enter>`. A+W Enterprise automatically fills in the field **Name**.
3.  Enter the number of horizontal and vertical muntins and confirm with `<Enter>`.
4.  Use the `<Spacebar>` key to select the symmetry and confirm with `<Enter>`.
5.  If you have chosen a muntin that is available in different colors, select the color in field **Color**.
6.  If muntins have to be ordered, choose a **Supplier** via `<F8>`, `<F9>`.
7.  Select the supply type in field **S** by `<F9>` or click on the arrow.
8.  Field **Spacer** defines the airspace in which the muntins will be fitted.
    This entry is possible only for triple IG.
9.  Field **Glass** defines the lite onto which the muntins shall be glued.
    This input is possible only for glued-on muntins or for triple IG.
    After all entries have been made, A+W Enterprise automatically calculates the total muntin length and displays it in field **Lin.m**.
10. Leave **Muntin entry** with `<End>` or enter more muntins.
    If you have selected **Muntin symmetry** with editor, the **Muntin editor** appears now.

> **Notes on pricing**
> Please note that pricing can handle maximally two muntin articles.

### Here's how to start the muntin editor

1.  If you have selected **muntin symmetry** with editor, the muntin editor automatically appears when you leave **Muntin entry** with `<End>`.
2.  Alternatively, you can press `<F3>` on the **Muntin entry** dialog after you have changed this item in the **Muntin editor**.
    *⇨ Sales, "Muntin editor" on page D-1286*

### Here's how to define auxiliary muntin

You can remove individual muntins.
1.  Open the **Muntin editor**.
    *⇨ Sales, "Here's how to start the muntin editor" on page D-1019*
2.  Click on the muntin you want to remove.
    The muntin will be removed.

> **Restore muntin**
> To restore the muntin, click on its original position. The muntin appears again.

### Here's how to delete muntin sections

You can remove entire muntin sections.
*⇨ Sales, "Muntin sections" on page D-1289*

1.  Open the **Muntin editor**.
    *⇨ Sales, "Here's how to start the muntin editor" on page D-1019*
2.  Press `<F6>`.
    A+W Enterprise marks a muntin in red.
    *   If you want to keep the section like that, press `<1>`.
    *   To delete the section, press `<2>`.
    *   To stop editing muntin sections, press `<3>`.
3.  Treat all other muntins in the same way. A+W Enterprise will check one segment after the other in this way.
4.  Use `<End>` to quit the **Muntin editor**.

### Here's how to move drill points

1.  Open the **Muntin editor**.
    *⇨ Sales, "Here's how to start the muntin editor" on page D-1019*
2.  Click on one of the edge connections to activate **Input of drill points**.
    Or press `<Shift>` + `<F12>`.
3.  Enter the new drill point position on the dialog.
    Reference point is the bottom left corner of the lite.
    Confirm using `<Enter>`.
4.  Use `<End>` to quit **Drill point input** or proceed with the other drill points.

### Here's how to change the size of a clear field

1.  Open the **Muntin editor**.
    *⇨Tutorial, "Here's how to start the muntin editor" on page D-1019*
2.  Click on the field you want to change.
    Or press `<Ctrl>` + `<F8>`.
    The system will want to know if the field height should be changed. If you answer **[no]**, the width can be changed in the following dialog.
3.  Enter the new field size in the dialog.
4.  Use `<End>` to quit the **Muntin editor** or proceed with the other fields.

### Here's how to adjust the muntin sections in the table

*⇨ Sales, "Muntin sections" on page D-1289*

1.  Open the **Muntin editor**.
    *⇨ Sales, "Here's how to start the muntin editor" on page D-1019*
2.  Click on **[Tab]**. Or press `<Shift>` + `<F 11>`.
    Dialog **Muntin sections** appears.
3.  Change the drill points by entering the new value.
4.  Use `<End>` to save and quit the **Muntin sections** dialog.

### Here's how to reject changes in the muntin editor

1.  Open the **Muntin editor**.
    *⇨ Sales, "Here's how to start the muntin editor" on page D-1019*
2.  Click on **[New]** or use `<F3>` to reject the changes and restore the symmetry in the **Muntin editor**.
3.  Use `<End>` to quit the **Muntin editor** or change the pattern once more.

## Stepped entry

**Objectives**
*   Get to know stepped entry.
*   Recognize prerequisites of stepped entry.
*   Note restrictions of the stepped entry.
*   Recognize benefits of the function.

**Benefits**
*   This function is especially important for the manufacturing of glass for the construction sector.
*   A step on a lite affects some subsequent functions, such as shape degrading, sealing depth, production sketch, etc.

**Note**

*   **Step**: Edge deduction on the lite starting from the reference glass.
*   **Reference glass**: Structures entered in advance that are used cheaply.

It happens often that assembled glass units (IG or LAMI) are not flush on the edges. This happens if, for example, for a facade, glass used is fastened to the first lites. This step reduction can be used on only one glass edge or on several or all edges.

For correct entry, you need a dummy article with the article type = **500 Step**. An important prerequisite for this article is that it is not a **meta part**. Another prerequisite includes the calculation of the step reduction dimension. This calculation is done using formulas that are stored in the master data and assigned to the lites in the BOM.
*⇨ Master Data, "BOM" on page B-442*

A reference lite receives a form without the step reduction in the BOM. All other lites in the BOM must be assigned a formula with step reduction. Appropriate formulas are also assigned for IG frames.
*⇨ Master Data, "Compulsory sizes size parameter selection" on page B-427*

**Example**
Formula **100** has the value **N** in the Step field.
Formula **110** has the value **Y** in the Step field.
*⇨ Master Data, "Formula editor" on page B-482*

In the BOM for IG, the first lite is assigned the formula **100**. This defines the first lite as reference glass. All other lites are assigned the formula **110**.

### Here's how to enter stepped IG in an order

1.  Open the **Order Entry** dialog and enter the order header as described in the following chapter:
    *⇨ Sales, "Here's how to enter an order" on page D-986*
2.  After entry of the **Article number** and **Quantity** in the item, you can now start the step entry with `<Shift>` + `<F10>`.

    > **UI Screenshot Description:** The "Stepped Entry (Relevant Parts)" dialog is shown. It lists the components of an IGU, including "A+W Float 4mm (AP: 1)" designated as "REFERENCE GLASS" and "A+W Float 4mm (AP: 3)". A shape sketch is shown on the right.

3.  According to the formulas stored in the article BOM, it is determined which glass serves as "reference glass" and is marked accordingly. Under some circumstances, the reference can be changed with `<Shift>` + `<F5>`. The manufacturability of the glass structure should be checked in this case.
4.  You can adjust the glass structure as you wish with the **[Glass exchange]** button.
5.  You can also assign a shape number for a lite. If you want to have the entire product structure as shape, enter the shape in the item:
    *⇨ Sales, "Here's how to enter a shape in the item" on page D-1005*
6.  Press **[OK]** to continue with the entry if the details on this dialog match the input request.
7.  The **Shape Dimensions** dialog for reference glass shape now opens. On this dialog, enter the dimensions of the reference glass and confirm your input with **[OK]**.
8.  The **Step Reductions** dialog now opens separately for each stepped lite:

> **UI Screenshot Description:** The "Step reductions" dialog is shown. It displays a rectangular shape with input fields on each edge for the reduction dimension. The dimensions are W=1000, H=1450. Reductions of 80.0, 100.0, and 80.0 are entered on the top, bottom, and right edges respectively.

9.  Enter in the fields that are visibly on the edge the reduction dimension per edge. Please note that the deduction is made parallel to the selected edge.

    **Example**
    The reduction 100 mm is deducted parallel to the lower edge.
    The reduction 80 mm is deducted parallel to the upper edge.
    The reduction 80 mm is deducted parallel to the right edge.
    that is, the dimension of the stepped lite is calculated as follows:
    H = 1450-100-80 = 1270 mm
    W = 1000-80 = 920 mm.
10. Confirm the entry with **[OK]**.
    If you want to enter more than one stepped lite, this dialog opens for each lite. The fields for the reduction input are pre-populated with the values already entered. You can then change the reduction dimension or confirm the same value input with **[OK]**.
11. The dialog for step entry closes. You can now enter the rest of the item.
12. You can check the dimensions for the header article as for each lite and each frame/LAMI foil in the price field with `<F3>`.

## iTOE - entry and reworking

**Objectives**
*   Get to know technical order entry.
*   Recognize possibilities of technical order entry.
*   Note restrictions on technical order entry.
*   Recognize benefits of the function.

**Benefits**
*   With iTOE, you can enter a technical drawing simply and precisely. This drawing is then taken over in A+W Enterprise and the BOM synchronized.

**Note**

*   **ITOE**: Integrated CAD-based item entry. Usage assumes the correct system configuration.
*   **Template**: Structures entered in advance that are used cheaply.
*   **SN file**: A+W CAD Designer (Shapes) file.

ITOE offers the opportunity to enter specific form elements and import and export technical drawings. Based on templates, you can perform technical order entry for complex elements, generate the BOM automatically and compare it. In the process, all necessary commercial documents (orders, production papers, delivery notes, etc.) and the machine control are supported.

You can use the following entry variants:

*   **Automatic generation of a SN file**
    *⇨ "Here's how to generate the SN file automatically" on page D-1026*
*   `<Ctrl>` + `<E>` **manually attach a SN file**
    *⇨ "Here's how to attach the SN file to the item" on page D-1026*
*   `<Ctrl>` + `<F>` **start the technical entry (TOE)**
    *⇨ "Here's how to start the technical order entry" on page D-1027*
*   `<Ctrl>` + `<B>` **start the DXF import**

> **iTOE exchange rules**
> To ensure smooth communication between the two programs A+W Enterprise and A+W CAD Designer (Shapes), iTOE exchange rules must be stored carefully in advance:
> *⇨ Master Data, "iTOE exchange rules" on page B-359*

### Here's how to generate the SN file automatically

1.  Start order entry. Enter the order header:
    *⇨ Sales, "Here's how to enter an order" on page D-986*
2.  Enter the desired product number in the item.
3.  To have the program generate an SN file, your system has to be configured appropriately. If this is the case, right after you enter the product number, the question appears whether the SN file should be generated for the item automatically. Confirm this question with **[Yes]**.
4.  The **SN** checkbox is activated and it cannot be changed.
5.  Finish entering the item.
6.  On the **Prop.** tab, in the **CAD file** field, the newly generated SN file is assigned to the item and displayed.
7.  Then you have the following possibility:
    *⇨ Sales, "Here's how to start the technical order entry" on page D-1027*
    or to delete this SN file with `<Ctrl>`+`<F9>`.

### Here's how to attach the SN file to the item

1.  Start order entry. Enter the order header:
    *⇨ Sales, "Here's how to enter an order" on page D-986*
2.  Enter the desired Product number and Quantity.
3.  Press `<Ctrl>` + `<E>`. The program changes to the **Prop.** tab, **CAD file** field, and opens the Windows dialog **Open file**:

    > **UI Screenshot Description:** The image shows the A+W Enterprise order entry screen with the Windows "Open" file dialog overlaid. The "Open" dialog is pointed to a 'cadfiles' folder, showing a list of `.SN` files. The user is about to select a file to attach to the order item.

4.  Choose a required file and confirm with **[OK]**.
5.  The **SN** checkbox is activated and it cannot be changed.
6.  Finish entering the item.
7.  On the **Prop.** tab, in the **CAD file** field, the newly generated SN file is assigned to the item and displayed.
8.  Then you have the following possibility:
    *⇨ Sales, "Here's how to start the technical order entry" on page D-1027*
9.  or to delete this SN file with `<Ctrl>`+`<F9>`.

### Here's how to start the technical order entry

1.  The master data for iTOE exchange/addition are assumed for the technical order entry.
    *⇨ Master Data, "iTOE exchange rules" on page B-359*
2.  Start the **Order Entry** dialog.
3.  Enter the data in the order header and on the item level the fields **Article**, **Quantity**, **Width/Height/AIR** (for IG).
4.  Use `<Ctrl>` + `<F>` to start the technical order entry with A+W CAD Designer (Shapes).
5.  The fields already entered and the product structure are taken over for further entry. With an appropriate configuration, the product names of glass and films (artikel.artbez1) can also be taken over in A+W CAD Designer (Shapes).

    > **Working with A+W CAD Designer (Shapes)**
    > For technical entry in A+W CAD Designer (Shapes), see the manual for A+W CAD Designer (Shapes). If you are interested, please contact an A+W employee.

6.  After completion of the product drawing, you now have the following possibilities:
    *   **Exit TOE (`<F2>`)**: You exit the technical order entry and return to the A+W Enterprise order entry. The possible changes in A+W CAD Designer (Shapes) are taken over automatically, insofar as these are covered with iTOE exchange/addition rules. However, the sn file is not included. Should you want to do further processing or make corrections to the product structure, the technical entry must be done again.
    *   **Cancel TOE (`<F3>`)**: You exit the technical order entry and return to the A+W Enterprise order entry. Possible changes in A+W CAD Designer (Shapes) are discarded.
    *   **Exit TOE and save (`<F4>`)**: You end the technical order entry, the sn file is saved, name of the file is also saved in the item. The BOM is compared based on the pre-defined exchange/addition rules. The sn file can be edited again if necessary.
    *   **Exit TOE without SL comparison (`<F5>`)**: You exit the technical order entry. The sn file is taken over into the item and saved. However, there is no BOM comparison.

### Here's how to compare the BOM manually

If the BOM comparison between A+W CAD Designer (Shapes) and A+W Enterprise could not be executed, you are offered the opportunity to determine the appropriate product assignment yourself.

1.  Start the **Order Entry** dialog.
2.  Perform iTOE item entry.
    *⇨ "Here's how to start the technical order entry" on page D-1027*
3.  If no appropriate assignment is determined for a relevant BOM item from the iTOE exchange rules, a notice appears that no A+W Enterprise article was found for this CAD processing. A value entry dialog now opens automatically.
4.  You can select the desired A+W Enterprise article from the selection and confirm the entry with **[OK]**.
5.  The processing is added to the item BOM.

### Here's how to reset the SN status manually

After the BOM comparison and successful data takeover, it can be necessary to lock the A+W Enterprise BOM for repeated data transfer in the A+W CAD Designer (Shapes). Perform the following steps:

1.  Start the **Order Entry** dialog.
2.  Perform iTOE item entry.
    *⇨ "Here's how to start the technical order entry" on page D-1027*
3.  Position the cursor in the **SN file** on an item whose SN status must now be changed.
4.  Press `<Ctrl>` + `<A>`. The status change is made only after confirmation of a CU message (customizing message). SN-Status=100 is now set for this item.
5.  End the item entry.

## Product replacement

**Objectives**
*   Get to know product replacement in the order entry.
*   Use the possibility for quick product replacement in an existing order.
*   Note restrictions of the function for product replacement.
*   Recognize benefits of the function.

**Benefits**
*   With the product replacement function, you can easily change several BOMs at once in an order already entered. The changed product structures can now apply for this order or optionally be written back to the master data.

**Note**

*   **Product replacement**: A product replacement is an exchange of a complete item article, as well as a change of the product structure in an order already entered.
*   **Original structure**: BOM tree of an item from the master data.
*   **Favor. structure**: New or changed BOM of an item.

On the item level in the order entry, you can make a product replacement. This way, it is possible to make changes quickly and easily for various products or the product structure at the same time for several items. Some user cases are described in this chapter:
*⇨ "Here's how to make a product replacement" on page D-1030*
*⇨ "Here's how to make an exchange from double IG to triple IG" on page D-1031*

### Here's how to make a product replacement

> **UI Screenshot Description:** The "Product Replacement" dialog.
> *   **A - Old BOM/type:** The BOM/customer item type number.
> *   **B - Current product structure:** Shows the current structure in the item (e.g., Cust. Product, 1st lite, Frame/Foil).
> *   **C - Original product structure:** Shows the original structure from master data.
> *   **D - Desired product structure:** Shows the proposed new structure after replacement.

1.  Start the **Order Entry** dialog.
2.  Select or enter the order number on which you want to make the changes.

    > **Order status**
    > Note that changing the BOM is among the production-relevant changes. This way, the changes to the BOM can only be made as long as the order has not been released to the system for processing.

3.  Start the **Product Replacement** dialog from `<F4>` > **Product Details**.
4.  On the **Product Replacement** dialog under (A), **Old BOM/type**, enter the BOM number of the type of customer item.
5.  The current product structure is displayed on the **Product Replacement** dialog under (B).
6.  In the **Exchange Article** field, enter the desired article number or select the number via the article selection with `<F9>`.
    *⇨ Sales, "Find article" on page D-1097*
7.  The original structure is now displayed under (C) and (D) on the dialog.
8.  You can change the fields for the desired structure, e.g.:
    *   For the **1st lite**, select a different glass
    *   For the **2nd lite**, enter another assembly position
    *   In the **Additional article** field, add another processing.
9.  Then you have the following option for selection:
    *   Use `<Original>` to display the desired structure from the master data again.
    *   Use `<F3>` or `<Start>` to execute the action.
    *   Use `<Next>` to enter the product replacement for additional BOMs/type.
    *   Use `<Cancel>` to exit the **Product Replacement** dialog without having made any changes.

### Here's how to make an exchange from double IG to triple IG

> **UI Screenshot Description:** The "Product Replacement for Items" dialog.
> *   **A - Display which articles are replaced:** Shows the old and new article numbers.
> *   **B - AIR fields that can be changed:** A grid lists items with columns for `Article`, `Width`, `Hght`, `AIR`, and a new `AIR2` field, allowing users to define the second airspace for the triple IG unit.

1.  Execute the steps from 1 to 8.
2.  Then execute the replacement from: with `<Start>` or `<F3>`.
3.  The program automatically detects that for the replacement, the entry for **AIR2** is missing and starts the **Product replacement for item** dialog.
4.  On this dialog, area (B), you can assign for each position in which a product replacement is detected, an existing AIR to be changed or assign a new **AIR2**.
5.  Then execute the action with `<Start>`.

> **Note compulsory sizes**
> Whether AIR2 can be entered or changed depends on the compulsory sizes for the selected article or its article type. Only if the entry for the size parameter AIR2 is permitted can you make the change in the order.
> *⇨ Master Data, "Compulsory sizes — size parameter selection" on page B-427*
> *⇨ Master Data, "Compulsory dimensions — view 1" on page B-428*

## Entry without prices

### Price Calculation

> **Image Description:** A schematic diagram shows the structure of a simple IG (Insulated Glass) lite. "IG" is at the top, branching down to "Float", "Spacer", and another "Float". "Float" further breaks down into "Cutting". "Spacer" breaks down into "Profile" and "Drying agents". All components lead to "Assembly", which in turn leads to "IG production".

Price calculation allows the quick calculation of purchase and sales prices without saving the results.
*⇨ Software Reference, "Price calculation" on page D-1378*

### Entry without prices

Customer orders can be entered quickly by means of **Input without prices**. The advantage of this method is that the customer can follow the input of orders but has no access to pricing. Pricing - based on the valid prices and conditions - is done in the background after the actual order entry. Prices can be changed easily if necessary.
*⇨ Software Reference, "Entry w/o prices" on page D-1132*

You can run customized pricing without creating or saving a document (quotation, order).
Fill in all the fields as you do at order entry; price calculation does not require to fill in all the fields in the document header however.

- Operation, quotation and order entry on page D-33
- Software reference, price calculation on page D-68
- Calculate prices

1.  Open menu **Sales > Price calculation**.
    A+W Enterprise shows the selected dialog.
2.  Select a customer:
    Enter the customer number, if known to you.
    Or press `<F9>` to search by customer number, or `<F8>` to search by matchcode.
    The **Search market partner** dialog opens.
3.  Use `<F 2>` to open the extended search.
4.  Fill in the search criteria.
5.  Use `<F3>` to start the search.
    *Software "Execute search" on page A-60*
    *Software "Customer" on page D-73*
6.  Assign the document to a project (optional) to take into account special conditions for this document.
    Press `<F9>` in the **Project** field. Select a project from the list.
    *Software reference "Project" on page C-77*
7.  Enter the items and products.
    *Operation, "Create items and products" on page D-39*
8.  Complete the document.
    *Operation "Complete order entry" on page D-56*

You can enter documents (quotation, order) without the price calculation being visible at the time of entry. The advantage of this method is that the customer can follow the input of orders but has no access to pricing.

After saving, A+W Enterprise will add the prices and show them on the printout.
Input is just like order entry.

See the next chapter to learn how you enter the individual fields:
*⇨ Software Reference, "Entry w/o prices" on page D-1132*

## Delivery Notes

Every shipment of an order is accompanied by a delivery note. On the one hand, it serves as a proof for the customer and on the other hand shows the status of order processing. You can issue complete or partial delivery notes. The latter will be issued if the shipment is not complete, but is made in several partial deliveries. You can define whether delivery notes will be released automatically, or issued manually.
*⇨ Software Reference, "Delivery" on page D-1384*

## Invoices

Invoicing is based on the delivery and payment terms agreed for the order. After delivery, you can issue partial or collective invoices. An invoiced document can no longer be corrected. If price corrections should be made, this is only possible via the issuing of a credit note or an additional charge.

The assignment of invoice numbers is done automatically by the system. For manual invoice entry, first an internal number is assigned and only when the invoice has been entered completely is this invoice saved under its final number. This guarantees a seamless numbering.

In extremely rare cases (program crash directly after the final invoice number has been assigned) it can happen that during the assignment of invoice numbers, there are gaps. Since these gaps can cause problems in controlling, a possibility has been created to re-use these numbers. This logic requires a special system configuration and may only be activated in consultation with A+W. If you are interested, contact an A+W Software GmbH employee.

Apart from that, you can issue deposit or final invoices with a previously created payment plan, and select automatic release or manual invoicing.

## Credit Notes

If an order is cancelled, if the goods are damaged during transport, or in case of complaints, you can issue complete or partial credit notes and book them immediately. You can also issue a credit note for a lump sum when referring to a certain invoice so that the credit note can be handled by accounting.

## Order Release

Orders that have not been released right at order entry can be released later. When an order is released, its data are processed for and transferred to other A+W Enterprise components (production, purchasing, stock, despatch).

The order can be changed until production is started, or until a purchase order or a delivery note has been issued. Changes must be released again for processing.
*⇨ Software Reference, "Release" on page D-1379*

### Release order

1.  Select menu **Sales > Release order > Release**.
2.  Use `<F9>`, `<F8>` to select the department in which the order has been entered.
    Or press `<Enter>` to view all as yet unreleased orders.
    The list **Release order** shows all unreleased orders.
3.  Use the `<arrow keys>` to select the order to be released.
4.  Change the status in column **free**.
5.  Release the order with `<F3>`.
    All sources of supplies (stock, purchasing, production) involved are informed about the order, and will trigger the necessary steps. Moreover, the order is also reported to the dispatch control system to schedule transport capacities.
    *⇨ Software Reference, "Release" on page D-1379*

## Print

**Note**
*   **VODR**: Access to the **Print Form** dialog is controlled by the EDI module abbreviation VOKA.
*   **VOEM**: Access to the **Send E-Mail** dialog is controlled by the EDI module abbreviation VOKA.

The **Forms** menu is used to print or email documents such as quotations, orders, order confirmations, etc. If you still use the fax function, it can also be reached via this menu element.

Since version 2008, A+W Enterprise offers all print functions and the REPGO environment (Unix/Linux) as well as the Crystal Reports connection. Both possibilities must be configured completely.

> **Requirements**
> *   Form types are set up
> *   Printers (also PDF and e-mail printing) are set up.
> *   Customers' e-mail addresses are maintained.
> *   Customers' fax numbers are maintained.

### Here's how to work on the Forms dialog:

> **UI Screenshot Description:** The image shows two dialogs. The background is the "Form printing" dialog, listing invoices with details like document number, partner, and date. The foreground is the "Select printer" dialog, prompting the user to choose a printer.

1.  **Sales > Forms > Print** menu.
    The **Form type** dialog opens.
2.  Select form type and take over with `<End>`, e.g. **Invoice**.
    The **Print form** dialog opens.
3.  Select pre-settings and take over with `<Enter>`, e.g.:
    *   1 additional copy
    *   Specify various numbers.
4.  Select **Document** field with `<F9>` and take over.
5.  Confirm invoice number(s) with **[OK]**.
    The **Print** dialog opens.
6.  Select printer and start printing of the invoice with `<Enter>`.

**Print several invoices:**
7.  Select pre-settings, e.g. **Select numbers** and take over with `<Enter>`.
8.  Add order numbers, e.g. on individual orders from the previous day:
    *   Enter employee number.
    *   Restrict input date.
    *   Select first and last document.
9.  Read in order numbers from the restricting ranges with `<F3>`.
10. Select **Pr** field for print output **Y** or **N**.
11. Trigger printing with `<F3>`.
    The **Print** dialog opens.

Select printer and start printing of the invoices with `<Enter>`.
*⇨ Software Reference, "Form printing" on page D-1419*

## List printing

A list of the individual master and document data is available in the **Printing of lists** menu. This menu offers a number of useful lists such as article or customer base data, orders received or invoices issued, commissions, or muntin types available.

## Overview Functions in Sales

The **Overview** menu offers the following submenus:
*   Overview
*   Order Information

### Overview

The **Overview** menu allows the display of documents by various criteria. You can display as yet uninvoiced orders, orders blocked from invoicing, or invoices that have not been booked yet.
This menu also provides information on the status of orders, incomplete shipments, and information on orders.
*⇨ Software Reference, "Document Research" on page D-1447*

### Order Information

This dialog provides information on the individual order items. When a dialog has been opened, you can use `<F2>` to scroll through the different statuses.

**Show order information**
1.  Load the order information as follows:
    *   On the **Sales > Overview > Order information** menu
        *⇨Sales: Software Reference, "Order information" on page D-1428*
    *   or in the header or order body via `<Shift>` + `<F10>` **Order information**
        *⇨Sales: Software Reference, "Order items – status" on page D-1186*
2.  Select the required submenu (status) from the list.
3.  If you have not loaded the Order information menu from the order, enter the order number on the **Document status** dialog or search for the document.
    *⇨ Tutorial, "Overview" on page D-1042*

### Background checks

The **Checks** menu consists of the **Input** and **Background check** submenus.
The **Input check** basically shows the existing orders in the shape of text. Item data relevant for pricing are shown in detail.
The **Background check** includes an error message system that lists where background processes have caused processing errors. The orders in question can be loaded and edited or corrected as required.
*⇨ Software Reference, "Document Research" on page D-1447*

## Resubmission

**Objectives**
*   Get to know the difference between document-related and free resubmissions.
*   Get to know the possibilities of the resubmission function.
*   Recognize benefits of the function.

**Benefits**
*   The resubmission function handles reminders for the editing of documents that can be defined according to particular criteria.

**Note**
*   **SYWV**: Access to the **Resubmission Mode** dialog is controlled by the EDI module abbreviation SYWV.

Notes and processing instructions referring to a certain time are set on Resubmission. Resubmission allows you to display the text right after starting the system, or show it in the mailbox of the user in charge.
The **Resubmission** dialog is described in detail in the following chapter:
*⇨ Sales, "Resubmission" on page D-1467*

**Free resubmission** is not connected to any document.
For document-related resubmission for quotations, the shipping date entered counts as the presentation date. However, this variant must be configured explicitly.

Notes and processing instructions referring to a certain time are set on Resubmission. We distinguish document-related and free resubmission.

**Document-related resubmission** is defined when a document - e.g. an order or an invoice - is created.

**Free resubmission** reminds you of - freely definable - facts or events that are not related to a commercial document.

For both free and document-related resubmission, you can display the relevant text at the login, or save it in the virtual mailbox of the employee it concerns.
*⇨Sales: Software Reference, "Resubmission" on page D-1467*

### Activation of resubmission

1.  Open the **Resubmission Mode** dialog (System > Document Management > Resubmission Mode).
    A+W Enterprise opens the **Resubmission** dialog.
2.  In the **Document** field, select the document type for which the resubmission mode should be used.
3.  In the **Mode** field, define how the resubmission should be handled. The following options are available:
    *   **no resubmission**: no automatic resubmission is created for the selected document type
    *   **mandatory submission**: when saving the document type selected here, the Resubmission dialog opens automatically. The Resubmission dialog can only be exited and details saved if the details are complete.
        *⇨ "Define order-related resubmission" on page D-1045*
    *   **autom. resubmission after**: with this mode, you enter in the following field (Days) the number of days after which the resubmission is created automatically.
    *   **autom. deletion after**: with this mode, you enter in the following field (Days) the number of days after which the resubmission will be deleted automatically.

### Define order-related resubmission

1.  Open a dialog for document entry, e.g. **Order Entry**.
2.  Use `<F4>` on any document level (header, body, footer) to start the **Resubmission** dialog.
3.  Fill in the fields of the **Resubmission** dialogue.
    *⇨ "Fill in the fields on the Resubmission dialog" on page D-1046*

### Define free resubmission

1.  Open the **Sales > Resubmission** menu.
    A+W Enterprise opens the **Resubmission** dialog.
2.  Fill in the fields of the **Resubmission** dialogue.
    *⇨ "Fill in the fields on the Resubmission dialog" on page D-1046*
3.  Fill in the fields of the **Resubmission** dialogue.

### Fill in the fields on the Resubmission dialog

1.  Select a resubmission date in field **Subm..date**. At the resubmission date, the selected employee receives notification in the form of a text pop-up on the monitor or via e-mail if additional fields are filled out.
2.  Choose the submission type for the resubmission. The following options are available:
    *   **Message in message system**: with this mode, you specify in the following field (Employee) the employee number to which the resubmission e-mail is sent. The message system will inform the user. Use `<Ctrl>` + `<F4>` to retrieve messages in the system menu. If an e-mail address has been entered in the employee master data, the message recipient will be informed by external e-mail.
    *   **active resubmission**: with this mode, you enter in the following field (Employee) the employee number of the person who will receive the resubmission (on the screen at the start of the program).
    *   **direct deletion of the document**: with this mode, you specify in the following field (Note) a note why the document will be deleted. This option is only permitted for customer quotations and supplier inquiries. After the date has elapsed (On the Resub.date) the corresponding document is suspended and the resubmission text entered as cancellation reason.
3.  Enter the employee number who receives the resubmission. By default, the individual entering the document or A+W Enterprise user is preset here.
4.  Enter the resubmission text.
5.  To create additional resubmission dates for this document (document-related dialog filling) or another free resubmission, press the text fields with `<Enter>` or press `<F6>` to create another resubmission immediately.
    New lines will appear.
    This way, you can add as many resubmissions as you wish.
6.  Use `<F7>` to delete resubmissions that are no longer required.
7.  Save the dialog with `<END>`.

## Modification Functions in Sales

The table below provides a brief overview of the other functions in the Sales sector.

| Function | Overview |
| :--- | :--- |
| **Completion report** | Completion reports are used to report the current production status to A+W Enterprise. Completion reports refer to a quantity unit. This way, a completion report can be issued for partly delivered quantities of an item.<br>Manual completion reports differ from the normal procedure and make sense only for small retailers. Completion reports should be made on the shop floor or in the purchasing department.<br>*⇨ Software Reference, "Completion report" on page D-1469.* |
| **Document change** | Function for changing particular order data without going into the document.<br>*⇨ "Document change" on page D-1048* |
| **Sales** | Sales staff can use A+W Enterprise to create, edit, and manage their visiting reports, visiting statistics, and commission. Apart from that, budgets concerning the entire company are available as well as comprehensive project budgets.<br>You can create distribution matrices, distribution vectors, budgets, and comparisons of calculated/actual values.<br>Project budgets are versatile, allowing to manage project accounts and lists, assembly costs, or even payroll accounting.<br>For additional information about this area, contact your A+W Software GmbH contact person. |

## Document change

**Objectives**
*   Get to know dialog operation.
*   Make a route or shipping date change.
*   Get to know prerequisites and restrictions of the function.

**Benefits**
*   Quick and easy change of one or several order(s).
*   Simultaneous change of several quotations, orders or delivery notes.

**Note**
*   **VOKA**: Access to the **Document Change** dialog is controlled by the EDI module abbreviation VOKA.

On the **Document Change** dialog, you can change document data without having to load the appropriate dialog. You can make changes to the following document types this way:
*   Quotation
*   Order
*   Delivery note

Another advantage of this function: you can make changes to several documents at the same time. You can change the scheduled shipping date, the route, the cancellation status, and the client number.

Changes to orders will be transferred to the production scheduling system again and to dispatch control if the order had already been released. If the order has not been transferred to dispatch so far, or if it is still in the release pool, the relevant fields are inaccessible.

Changes to quotations are only transferred to the production system if the system is configured for this.

Changes to delivery notes are only possible as long as the delivery note is still open and does not count as delivered completely.

Changes that are not forwarded to subsequent processes are marked with **Local change**. Orders with this code must, e.g. be transferred manually to dispatch.
*⇨ Software Reference, "Document change" on page D-1471*

The following limitations must be noted:
*   For call center orders that are entered using the multi-client logic in A+W iQuote Enterprise, no company change can be made with this function.
*   ?

### Here's how to make the document change quickly

1.  Select the **Sales > Document Change** menu.
    **Document change** dialog opens.
2.  **Document** field: select document type, e.g. **Order**.
3.  **Number** field: press `<F9>`.
    The **Find Orders** dialog opens.
4.  **Customer** field: enter customer number and start search.
    Hit list is displayed.
5.  Take over order with double-click on the **Document Change** dialog.
6.  Jump to the fields and change setting, e.g.:
    *   **Local correct** field: enter free text.
    *   **Std** field: set cancellation code.
    *   **Route** field: change route.
    *   **Date** field: change delivery date.
    *   **Free** field: release changes.
7.  Make changes with `<F3>`.
    To check, you can use `<Shift>`+`<F5>` to change to the current document:
8.  Open document for processing with a double-click.
9.  Check data and change if necessary.
    Save changes with **[OK]**.
10. You return to the **Document Change** dialog and can make additional change if you wish.

### Here's how to adjust particular costs quickly

Since the surcharges must often be adjusted due to increasing energy costs, it is also possible to update these in the existing documents. You can create an appropriate script yourself or with the help of A+W service employees in order to place these document in the document process `intauf` with `(still=-26)`. This `intaufart` then has updated the methods defined by the environment variable `RABATTMETHODEN_UPDATE` and recalculated the order.

You can also initiate this update on the **Document Change** dialog.

1.  Start the **Document Change** dialog.
2.  Select one or several orders.
3.  Use `<F2>` to change to the 3rd tab **Calculation**.
4.  In the **Discounts** field, select the type of change. Here, the selected orders with an appropriate `inataufart` are presented to the background process again. The following options are available for selection:
    *   Update Discounts (intauf -26)
    *   Insert the new discount methods (intauf -28)
    *   Redraw all discounts and retotal the order.
5.  Use `<F3>` to execute the action
    This functionality is only available for non-invoiced orders, quotations or delivery notes.

### Here's how to recalculate a quotation or an order

1.  Start the **Document Change** dialog.
2.  Select one or several orders.
3.  Use `<F2>` to change to the 3rd tab **Calculation**.
4.  In the **Calculation** field, select the type of change that will be transferred accordingly to the background process. The following options are available for selection:
    *   **SA**- Only recalculate sales prices
    *   **PU**- Only recalculate purchase prices
    *   **SA+PU** - recalculate the entire order
5.  Use `<F3>` to execute the action
    This functionality is also only available for non-invoiced orders, quotations or delivery notes.

# A+W Enterprise Sales - Software Reference

## Table of Contents

*   **Overview** ... D-1057
    *   Sales menu ... D-1058
    *   Invoices submenu ... D-1059
    *   Overview submenu ... D-1060
    *   Supplementary menu ... D-1060
    *   Addresses submenu ... D-1062
    *   Texts submenu ... D-1062
    *   Special texts submenu ... D-1063
    *   Prices submenu ... D-1063
    *   Order prices submenu ... D-1064
    *   Product details submenu ... D-1064
    *   Technical values submenu ... D-1065
    *   Info menu ... D-1066
    *   Notes submenu ... D-1067
*   **Search Functions** ... D-1068
    *   Find orders ... D-1069
        *   Find orders - document key ... D-1069
        *   Find orders - item code ... D-1072
        *   Find Orders - Direct Search ... D-1074
        *   Find Orders - Hit List ... D-1076
        *   Find orders - delivery information ... D-1077
        *   Find orders - miscellaneous ... D-1079
        *   Find orders - quantities ... D-1081
        *   Find orders - properties ... D-1083
        *   Find orders - reference ... D-1085
    *   Find market partner ... D-1087
    *   Employee/authorization groups ... D-1091
    *   Find deference document ... D-1093
    *   Find addresses ... D-1095
    *   Find article ... D-1097
        *   Find article - header, footer areas ... D-1098
        *   Find article names ... D-1101
        *   Find article - article codes ... D-1103
        *   Find article - details ... D-1105
        *   Find article by types ... D-1107
    *   Find product by element ... D-1108
        *   Find product - header, footer area ... D-1109
        *   Find product - customer article ... D-1111
        *   Find product - descriptions ... D-1113
        *   Find product - technical values ... D-1114
    *   Find project ... D-1115
        *   Find Project - header, footer areas ... D-1116
        *   Find project - address ... D-1118
        *   Find project - identification ... D-1120
    *   Enter value - extended search ... D-1122
    *   Enter value - search for reference ... D-1123
    *   Enter value - search for original number ... D-1124
*   **Document Management** ... D-1126
    *   Explanation of symbols ... D-1127
    *   Quick entry ... D-1130
    *   Quotation entry ... D-1131
    *   Entry w/o prices ... D-1132
    *   Order entry ... D-1133
        *   Order entry - header, footer area ... D-1134
        *   Order entry - addresses ... D-1141
        *   Order entry - properties ... D-1144
        *   Order entry - miscellaneous ... D-1150
        *   Order entry - totals ... D-1155
        *   Order entry - detailed view discounts ... D-1160
    *   Order items ... D-1165
        *   Order entry - general ... D-1165
        *   Order entry - properties ... D-1178
        *   Order entry - prices ... D-1183
    *   Order items - status ... D-1186
    *   Order entry - costs ... D-1188
    *   Site change ... D-1190
    *   New delivery address ... D-1191
    *   End customer address ... D-1193
    *   Market partner info ... D-1195
    *   Contacts ... D-1197
    *   Cancel ... D-1198
    *   Staff allocation - special ... D-1199
    *   Configurable fields ... D-1199
    *   Overview ... D-1200
    *   Product sets (Sash Master) ... D-1201
    *   Article dimensions ... D-1203
    *   Stock forecast ... D-1204
    *   Product replacement ... D-1208
        *   Product replacement ... D-1208
        *   Product replacement for items ... D-1210
    *   Complaint ... D-1211
    *   Order types ... D-1212
    *   Article details for dimensioned variants ... D-1214
    *   Variant and color/thickness selection ... D-1217
    *   Private fields ... D-1218
    *   External data - import ... D-1219
    *   Document types ... D-1222
    *   Allocation of document types ... D-1223
    *   File allocation ... D-1226
    *   DXF import ... D-1227
    *   Amendment log ... D-1228
    *   Delivery date change log ... D-1230
    *   Shape catalog ... D-1231
    *   Shape - dimensions ... D-1232
    *   Payment management ... D-1234
    *   Payment plan ... D-1236
    *   Error information system ... D-1238
    *   Production monitor ... D-1240
*   **Technical Details** ... D-1241
    *   Declaration of performance ... D-1241
    *   Order entry - technical values ... D-1242
    *   Calculated technical values ... D-1242
    *   Declared services ... D-1245
*   **Bill of Material (BOM)** ... D-1249
    *   BOM view ... D-1249
        *   BOM structure ... D-1250
        *   Product structure tab ... D-1253
        *   Production sketch tab ... D-1254
        *   Current BOM level ... D-1256
        *   Processing param. (short) tab ... D-1261
        *   Addresses tab ... D-1262
        *   All parameters/sketch tab ... D-1263
    *   Edge allocation ... D-1272
    *   Item processing ... D-1273
    *   Dimensions of individual BOM elements ... D-1274
    *   Spacer offset ... D-1276
    *   Sealing depths ... D-1277
    *   Stepped entry (relevant parts) ... D-1278
    *   Step reductions ... D-1280
    *   Muntin entry ... D-1281
        *   Muntin entry – muntins ... D-1281
        *   Muntin entry – add. info ... D-1284
    *   Muntin product – product number ... D-1285
    *   Muntin editor ... D-1286
    *   Drill point ... D-1287
    *   Clear field ... D-1288
    *   Muntin sections ... D-1289
    *   Muntin pattern ... D-1290
*   **Packaging Planning** ... D-1292
    *   Specs. packaging planning ... D-1292
    *   Packaging planning ... D-1298
*   **Notes** ... D-1300
    *   Document notes ... D-1302
    *   Market partner, project, article notes ... D-1303
    *   Market partner article notes ... D-1305
*   **Texts** ... D-1307
    *   Header and footer texts ... D-1308
    *   Article and item texts ... D-1311
    *   Special texts ... D-1312
    *   Phrases ... D-1314
    *   External information ... D-1316
    *   Box signature ... D-1317
*   **Prices and Conditions** ... D-1319
    *   Order conditions ... D-1320
    *   Order prices ... D-1325
    *   Order muntin prices ... D-1327
    *   Order exchange prices ... D-1330
    *   Order sub-part prices ... D-1332
    *   Post calculation ... D-1334
    *   Step prices ... D-1337
    *   Conditions for PCD processing ... D-1338
    *   Conditions for PCD, PCD BASIC GLASS processing ... D-1339
    *   Conditions for PCD BASIC GLASS ... D-1343
    *   Conditions IG ... D-1345
    *   Conditions IG (SWITZERLAND) ... D-1350
    *   Conditions for PCD COLORED ARTICLE ... D-1354
    *   Conditions for PCD PRICES GENERAL ... D-1356
    *   Conditions for PCD GLASS DOORS ... D-1358
    *   Conditions for manual prices ... D-1361
    *   LAMI exchange/additional prices ... D-1363
    *   Item conditions - processing prices ... D-1365
    *   Item conditions - muntin prices ... D-1368
    *   Production cost calculation ... D-1371
        *   Production cost calculation - overview ... D-1372
        *   Production cost calculation - details ... D-1374
    *   Price calculation ... D-1378
*   **Release** ... D-1379
    *   Order release ... D-1379
    *   Authorization ... D-1382
*   **Delivery** ... D-1384
    *   Delivery plan ... D-1385
    *   Delivery information - delivery details ... D-1387
    *   Delivery notes (automatic) ... D-1391
    *   Delivery notes (manual) ... D-1393
    *   Delivery notes log ... D-1395
*   **Invoices** ... D-1396
    *   Invoices (automatic) ... D-1397
    *   Item info ... D-1400
    *   Invoices (manual) ... D-1402
    *   Cash transaction ... D-1404
    *   Booking of invoices ... D-1405
    *   Partial invoice (automatic) ... D-1407
    *   Partial invoice (manual) ... D-1409
    *   Final invoices (automatic) ... D-1410
    *   Final invoices (manual) ... D-1412
    *   Invoice log ... D-1413
*   **Credit Notes** ... D-1414
    *   Credit notes ... D-1414
    *   Book credit notes ... D-1416
*   **Forms** ... D-1418
    *   Direct printing ... D-1418
    *   Form printing ... D-1419
    *   E-mail ... D-1423
    *   Print on ... D-1426
    *   List printing ... D-1427
*   **Order Status** ... D-1428
    *   Order information ... D-1428
        *   Document info - order ... D-1429
        *   Document info - items ... D-1431
        *   Document info – purchasing ... D-1433
        *   Document info - goods received ... D-1435
        *   Document info – production ... D-1437
        *   Document info – dispatch ... D-1438
        *   Document info - barcoding ... D-1440
        *   Document info - racks ... D-1442
        *   Document info - stock ... D-1444
        *   Document info - linked production ... D-1445
        *   Document info - intermediate disp. ... D-1446
*   **Document Research** ... D-1447
    *   Search document ... D-1447
        *   Search document - search mode ... D-1447
        *   Search document - overview ... D-1451
        *   Search document - employees ... D-1453
        *   Search document - details ... D-1455
    *   Document change log ... D-1458
    *   Items ... D-1460
        *   Items - overview ... D-1460
        *   Items - details ... D-1462
*   **Overviews of Documents** ... D-1464
    *   Order display ... D-1465
    *   Quotation display ... D-1466
*   **Resubmission** ... D-1467
*   **Completion report** ... D-1469
*   **Document change** ... D-1471
*   **Overview of documents** ... D-1476
*   **Sales** ... D-1477

## Overview

In the **Sales** module you manage the documents that are required for the successful processing of the sales business. They include, e.g. quotations, orders, and credits and create invoices.

In the Sales section you will find the following topics:
*   "Search Functions" on page D-1068
*   "Document Management" on page D-1126
*   "Technical Details" on page D-1241
*   "Bill of Material (BOM)" on page D-1249
*   "Packaging Planning" on page D-1292
*   "Notes" on page D-1300
*   "Texts" on page D-1307
*   "Prices and Conditions" on page D-1319
*   "Release" on page D-1379
*   "Delivery" on page D-1384
*   "Invoices" on page D-1396
*   "Credit Notes" on page D-1414
*   "Forms" on page D-1418
*   "Order Status" on page D-1428
*   "Document Research" on page D-1447
*   "Overviews of Documents" on page D-1464
*   "Sales" on page D-1477

## Sales menu

Some of the available menu entries branch out to submenus. If these include more than three entries, they are listed separately according to the following overview.
The displayed entries depend on the respective configuration.
For additional documentation that is not included in this section for the Sales menu or if you have questions, please contact your partner at A+W Software GmbH.

> **Context menus**
> On the context menus (right mouse button), only the menu elements are offered that make sense in the context for the individual fields of the dialogs. You can also call up the functions on the context menus via the menus described. Generally, the menu elements on the context menu correspond to the functions offered on the prompt display.

You can reach all dialogs and functions relating to sales via the **Sales menu**:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Quick entry | *⇨ "Quick entry" on page D-1130* |
| b | Quotation entry | *⇨ "Quotation entry" on page D-1131* |
| c | Order entry | *⇨ "Order entry" on page D-1133* |
| d | Pricing | *⇨ "Price calculation" on page D-1378* |
| e | Entry without prices | *⇨ "Entry w/o prices" on page D-1132* |
| f | Delivery notes | |
| fa | • Automatic release | *⇨ "Delivery notes (automatic)" on page D-1391* |
| fb | • Manual delivery notes | *⇨ "Delivery notes (manual)" on page D-1393* |
| fc | • Log | *⇨ "Delivery notes log" on page D-1395* |
| g | Invoices | *⇨ "Invoices submenu" on page D-1059* |
| h | Credit notes | |
| ha | • Enter credit notes | *⇨ "Credit notes" on page D-1414* |
| hb | • Book credit notes | *⇨ "Book credit notes" on page D-1416* |
| i | Release order | |
| ia | • Release | *⇨ "Order release" on page D-1379* |
| ib | • Authorization | *⇨ "Authorization" on page D-1382* |
| j | Forms | |
| ja | • Print | *⇨ "Form printing" on page D-1419* |
| jb | • E-Mail/Fax | *⇨ "E-mail" on page D-1423* |
| k | Print list | *⇨ "List printing" on page D-1427* |
| l | Overview | *⇨ "Overview submenu" on page D-1060* |
| m | Background check | *⇨ "Error information system" on page D-1238* |
| n | Resubmission | *⇨ "Resubmission" on page D-1467* |
| o | Completion report | *⇨ "Completion report" on page D-1469* |
| p | Document change | *⇨ "Document change" on page D-1471* |
| r | Sales | *⇨ "Sales" on page D-1477* |

### Invoices submenu

**Sales > Invoices**

Use this menu to access all dialogs on which you create and manage invoices.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Automatic release | *⇨ "Invoices (automatic)" on page D-1397* |
| b | Manual invoice | *⇨ "Invoices (manual)" on page D-1402* |
| c | Cash invoice | *⇨ "Cash transaction" on page D-1404* |
| d | Book invoices | *⇨ "Booking of invoices" on page D-1405* |
| e | Partial invoice | |
| ea | • Automatic release | *⇨ "Partial invoice (automatic)" on page D-1407* |
| eb | • Manual invoice | *⇨ "Partial invoice (manual)" on page D-1409* |
| f | Final invoice | |
| fa | • Automatic release | *⇨ "Final invoices (automatic)" on page D-1410* |
| fb | • Manual invoice | *⇨ "Final invoices (manual)" on page D-1412* |
| g | Log | *⇨ "Invoice log" on page D-1413* |

### Overview submenu

**Sales > Overview**

Use this menu to access all dialogs on which you can display an overview of the various documents.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Orders not invoiced | *⇨ "Overview of documents" on page D-1476* |
| b | Invoices not booked | |
| c | Deliveries not complete | |
| d | Orders with invoice block | |
| e | Status of processing | This module is no longer used. |
| f | Number determination | This module is no longer used. |
| g | Order display | *⇨ "Order display" on page D-1465* |
| h | Quotation display | *⇨ "Quotation display" on page D-1466* |
| i | Order information | *⇨ "Order information" on page D-1428* |
| j | Search document | *⇨ "Search document" on page D-1447* |

## Supplementary menu

The supplementary menu can be called up with `<F4>` for entering various documents, e.g. for an order.
Depending on the dialog and area, the entries on the supplementary menu are displayed differently. The example described here is the entries that are displayed when calling up the supplementary menu in the document entry:
*   Supplementary menu for the header and footer area (document entry)
*   Supplementary menu for the item level (document entry)

### Supplementary menu for the header and footer area (document entry)

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Text | |
| aa | • Header Text | *⇨ "Header and footer texts" on page D-1308* |
| ab | • Footer | *⇨ "Header and footer texts" on page D-1308* |
| ac | • External information | *⇨ "External information" on page D-1316* |
| b | Addresses | *⇨ "Addresses submenu" on page D-1062* |
| c | Contact person | *⇨ "Contacts" on page D-1197* |
| d | Cancel | *⇨ "Order items" on page D-1165* |
| e | Prices | *⇨ "Prices submenu" on page D-1063* |
| f | Product details | *⇨ "Product details submenu" on page D-1064* |
| g | Representation | *⇨ "Resubmission" on page D-1467* |
| h | Transfer to production (again) | Transfer the order automatically to production after saving. |
| i | Production monitor | *⇨ "Production monitor" on page D-1240* |
| j | Delivery plan | *⇨ "Delivery plan" on page D-1385* |
| k | Delivery information | *⇨ "Delivery information - delivery details" on page D-1387* |
| l | Payment plan | *⇨ "Payment plan" on page D-1236* |
| m | Payment management | *⇨ "Payment management" on page D-1234* |
| n | Configurable fields | *⇨ "Configurable fields" on page D-1199* |
| o | Site change | *⇨ "Site change" on page D-1190* |
| p | Direct printing | *⇨ "Direct printing" on page D-1418* |

### Supplementary menu for the item level (document entry)

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Text | *⇨ "Texts submenu" on page D-1062* |
| b | Addresses | *⇨ "Addresses submenu" on page D-1062* |
| c | Cancel | *⇨ "Order items" on page D-1165* |
| d | Private fields | *⇨ "Private fields" on page D-1218* |
| e | Prices | *⇨ "Prices submenu" on page D-1063* |
| f | Product details | *⇨ "Product details submenu" on page D-1064* |
| g | Representation | *⇨ "Resubmission" on page D-1467* |
| h | Consignments | |
| ha | • New consignment | Change to the Commis field on the Items tab in order to create or edit a consignment text. |
| hb | • Change consignment | "Order entry - general" on page D-1165 |
| i | Delivery plan | *⇨ "Delivery plan" on page D-1385* |
| j | Stock | |
| ja | • Stack (Ctrl+P) | Display the Stack field on the General tab. The stack display is an optional function and is configured customer-specifically. For customer-specific adjustments, contact your contact person at A+W Software GmbH. |
| jb | • Stock forecast (Ctrl+G) | *⇨ "Stock forecast" on page D-1204* |
| k | Payment plan | *⇨ "Payment plan" on page D-1236* |
| l | Configurable fields | *⇨ "Configurable fields" on page D-1199* |

### Addresses submenu

**<F4> > Addresses**

Use this menu to manage the addresses document-specifically.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Find delivery address(Ctrl+L) | *⇨ "Find addresses" on page D-1095* |
| b | New delivery address (Ctrl+N) | *⇨ "New delivery address" on page D-1191* |
| c | Delete delivery address | Delete the delivery address from the document. |
| d | End customer address | *⇨ "End customer address" on page D-1193* |

### Texts submenu

**<F4> > Texts**

Use this menu to manage the texts. The entries **Article text (F5)**, **Item text (Shift+F5)** and **Special texts** are only displayed on the item level.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | HeaderText | *⇨ "Header and footer texts" on page D-1308* |
| b | Footer | *⇨ "Header and footer texts" on page D-1308* |
| c | External information | *⇨ "External information" on page D-1316* |
| d | Article text (F5) | *⇨ "Article and item texts" on page D-1311* |
| e | Item text (Shift+F5) | *⇨ "Article and item texts" on page D-1311* |
| f | Special texts | *⇨ "Special texts submenu" on page D-1063* |

### Special texts submenu

**<F4> > Texts > Special Texts**

Use this menu to manage all special texts that you can assign to the document or the item.
**Special texts** is an optional function and is configured customer-specifically. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Spacer Text | *⇨ "Special texts" on page D-1312* |
| b | Product code | |
| c | Shape texts | |
| d | Logo texts | |

### Prices submenu

**<F4> > Price info**

Use this menu to manage the prices and conditions for a document or individual items.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Order conditions | *⇨ "Conditions for PCD processing" on page D-1338* |
| b | Order prices | *⇨ "Order prices submenu" on page D-1064* |
| c | Partial calculation | *⇨ "Production cost calculation" on page D-1371* |
| d | New calculation | |
| e | Redetermine discounts | |
| The following entries are only displayed for the document items: |
| d | + | *⇨ "Conditions for PCD processing" on page D-1338* |
| e | Download conditions | Determine the sales price with the item conditions and recalculate the price. |
| f | Price calculation | Recalculate the item price. |
| g | Price control | Display the fields for Price control on the General tab. |

### Order prices submenu

**<F4> > Price Info > Order Prices**

Use this menu to manage the order prices for individual items.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Article prices | *⇨ "Order prices" on page D-1325* |
| b | Muntin prices | *⇨ "Order muntin prices" on page D-1327* |
| c | Exchange prices | *⇨ "Order exchange prices" on page D-1330* |
| d | Sub-element prices | *⇨ "Order sub-part prices" on page D-1332* |

### Product details submenu

**<F4> > Product Details**

Use this menu to manage the details for the products, e.g. exchange and additional rules.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Product replacement | *⇨ "Product replacement" on page D-1208* |
| b | E/A rules | *⇨ Master data* |
| The following entries are only displayed on the item level: |
| c | Prod. group | Edit the product group. The cursor changes to the **Prodgrp.** field. |
| d | Technical values | *⇨ "Technical values submenu" on page D-1065* |

### Technical values submenu

**<F4> > Product Details > Technical Values**

Use this menu to manage the technical values.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Show technical details | Show the technical values.<br>*⇨ "Items tab (left area)" on page D-1166* |
| b | Change technical details | Edit the technical values. The cursor changes to the db value field of the technical values on the Items tab.<br>*⇨ "Items tab (Info area - graphic, technical values)" on page D-1168* |
| c | Declaration of performance | *⇨ "Declaration of performance" on page D-1241* |
| d | Show hidden dimensions | Show the hidden dimensions on the Items tab.<br>*⇨ "Items tab (Info area - graphic, technical values)" on page D-1168* |
| e | Change hidden dimensions | *⇨ "Article dimensions" on page D-1203* |

## Info menu

**<Shift> + <F4>**

Depending on the dialog and area, the entries on the Info menu are displayed differently. The example described here is the entries that are displayed when calling up the Info menu in the document entry:
*   Info menu for the header and footer area (document entry)
*   Info menu for the item level (document entry)

### Info menu for the header and footer area (document entry)

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Document notes | *⇨ "Notes" on page D-1300* |
| b | Market partner notes | |
| c | Project notes | |
| d | Search document | *⇨ "Search document" on page D-1447* |
| e | Document overview | *⇨ "Overview" on page D-1200* |
| f | Market partner information | *⇨ "Market partner info" on page D-1195* |
| g | Change log | *⇨ "Amendment log" on page D-1228* |
| h | Delivery date changes | *⇨ "Delivery date change log" on page D-1230* |
| i | Order information | *⇨ "Order information" on page D-1428* |
| k | Case signature | *⇨ "Box signature" on page D-1317* |
| l | Document types | *⇨ "DXF import" on page D-1227* |
| m | Document overview | *⇨ "Allocation of document types" on page D-1223* |

### Info menu for the item level (document entry)

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Notes | *⇨ "Notes submenu" on page D-1067* |
| b | Search document | *⇨ "Search document" on page D-1447* |
| c | Document overview | *⇨ "Overview" on page D-1200* |
| d | Market partner information | *⇨ "Market partner info" on page D-1195* |
| e | Change log | *⇨ "Amendment log" on page D-1228* |
| f | Delivery date changes | *⇨ "Delivery date change log" on page D-1230* |
| g | Order information | *⇨ "Order information" on page D-1428* |
| h | Case signature | *⇨ "Box signature" on page D-1317* |
| i | Document overview | *⇨ "Allocation of document types" on page D-1223* |

### Notes submenu

**<Shift> + <F4> > Notes**

Use this menu to manage all internal information about documents, market partners, and projects.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Document Notes | *⇨ "Notes" on page D-1300* |
| b | Article notes | |
| c | Customer notes | |
| d | Customer article notes | |
| e | Project notes | |
| f | Project article notes | |
| g | Supplier notes | |
| h | Supplier article notes | |

## Search Functions

In the Sales module, you can search via various categories for documents, market partners, addresses, and articles.
The search dialogs are structured the same way for all document types in Sales. They are described in this chapter using the example Order. Deviations will be described explicitly.
The following dialogs are described in this section:
*   "Find orders" on page D-1069
*   "Find Orders - Hit List" on page D-1076
*   "Find market partner" on page D-1087
*   "Employee/authorization groups" on page D-1091
*   "Find deference document" on page D-1093
*   "Find addresses" on page D-1095
*   "Find article" on page D-1097
*   "Find article by types" on page D-1107
*   "Find product by element" on page D-1108
*   "Find project" on page D-1115
*   "Enter value - extended search" on page D-1122

### Find orders

**Sales >Order Entry > Order field > `<F9>`**

You can search for orders on this dialog.
Specify the search criteria in the header area. With each criterion that you specify, you can reduce the hit quantity.
This dialog contains the following tabs in the header area:
*   "Find orders - document key" on page D-1069
*   "Find orders - item code" on page D-1072
*   "Find Orders – Direct Search" on page D-1074

The search results are shown in the hit list. The hit list is only displayed if you have started the search.
*⇨ "Find Orders - Hit List" on page D-1076*

#### Find orders – document key

**Sales >Order Entry > Order field > `<F9>`**

> **UI Screenshot Description:** Fig. D-6 shows the "Find Orders" dialog with the "Document Key" tab active. Search fields at the top include "Orders from", "Customer", "Deliv. Date", etc. The main area is a list of documents found, with columns like "Site", "Order", "Deliv. Date", and "Cust.".

You can search for orders on this tab using order data.
You can configure in which search criterion field you are first located for input when you open the dialog. Configurable as first input fields on the Document Key tab are the fields **Orders from**, **Customer**, **Proj.**, **InvoiceNo.**, **Deliv. Date**, **P.O.Date**, **VAT ID No.**, **Operator**, **Input Date**, and **Currency**.
You can also specify search criteria on the **Item Code** tab. Configurable as first input fields on the **Item Code** tab are the fields **Article**, **Qty. Unit**, and **Dimension Variant**.

*   Use `<F2>` to change the tab in the header area.
*   Use `<F3>` to start the search.

**Document Key Fields**

*   **Orders from**: Number starting from which orders are searched for. The search is restricted to all orders whose number is equal to or greater than the specified order number. The field name varies depending on the dialog from which you open the search, e.g. Quotations.
    *Technical info: numeric field, DB field: kauf.auftrnr*
*   **Customer**: Customer number. The search is restricted to all orders for this customer. If you specify a number, the customer name is displayed in plain text.
    *Technical info: numeric field, display field, DB field: kauf.kunr, kauf.orgname*
*   **Site No.**: Site number. By default, the number of your own site is filled in. The search is restricted to all orders from this site. The field can only be edited if you are working with internal site separation.
    *Technical info: numeric field, DB field: kauf.hausnr*
*   **Proj.**: Project number for which orders will be searched for. The search is restricted to all orders with this project. The project name is displayed in plain text after input of the number.
    *Technical info: numeric field, display field, DB field: kauf.objnr, kauf.orgname*
*   **External No.**: Order number that is specified by the customer. The search is restricted to all orders with this external number. With a configuration, the search for external numbers in the document search can be set so that it happens without considering upper- and lower-case letters.
    *Technical info: alphanumeric field, DB field: kauf.exaufnr*
*   **Act.Ref.No**: Original document number for transferred documents. The search is restricted to all orders with this reference number.
    *Technical info: numeric field, DB field: kauf._orgauftrnr*
*   **Invoice No.**: The search is restricted to all orders for which this invoice was created.
    *Technical info: numeric field, DB field: kauf.rechnr*
*   **Deliv. Date**: Desired delivery date for the order. The search is restricted to all orders with this delivery date. The delivery date can be specified as date or calendar week. The planned delivery date is displayed in the hit list.
    *Technical info: date field, DB field: kauf.ltplan*
*   **P.O. Date**: PO date of the order. The search is restricted to all orders with this PO date.
    *Technical info: date field, DB field: kauf.bdat*
*   **VAT ID No.**: Customer's VAT ID. The search is restricted to all orders with this identification number.
    *Technical info: alphanumeric field, DB field: kaufp.steuernr*
*   **Operator**: Employee number of the operator who entered the orders. The search is restricted to all orders by this operator.
    *Technical info: numeric field, DB field: kauf.eusr*
*   **Input Date**: Date on which the order was entered. The search is restricted to all orders with this input date.
    *Technical info: date field, DB field: kauf.edat*
*   **Currency**: Currency that is assigned to the order. The search is restricted to all orders with this currency.
    *Technical info: numeric field, DB field: kauf.waehrung*

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
*⇨ "Find Orders - Hit List" on page D-1076*

**Footer**
*   **New Search**: Deletes all search criteria for a new search. Alternatively, you can use `<Ctrl>` + `<F7>` to delete the search criteria.
*   **Search**: Starts the search with the specified criteria. Alternatively, you can start the search with `<F3>`.

#### Find orders – item code

**Sales >Order Entry > Order field > `<F9>` > Item Code tab**

> **UI Screenshot Description:** Fig. D-7 shows the "Find Orders" dialog with the "Item Code" tab active. Search fields include "Article", "Cust. Product", "Width", etc. The result list is an "Item Overview" showing orders that contain the specified item.

You can search for orders on this tab using item codes. You can also specify additional search criteria on the **Document Key** and **Direct Search** tabs.
*   Use `<F2>` to change to the header area of the tab.
*   Use `<F3>` to start the search.

**Item Code Fields**

*   **Article**: Article number. The search is restricted to all orders that contain this article as item article. If you specify a number, the article name is displayed in plain text. The BOMs of the items are not checked.
    *Technical info: numeric field, DB field: kpos.artnr*
*   **Cust. Product**: Reference number for customer-specific products from the master data. The search is restricted to all orders with articles of this customer-specific number.
    *Technical info: alphanumeric field, DB field: kpos.kuposnr*
*   **Width, Height**: Width and height of the item in millimeters. The search is restricted to all orders with articles with these dimensions.
    *Technical info: numeric fields, DB fields: kpos.laenge, kpos.breite*
*   **Reference**: Reference text. The search is restricted to all orders that contain the specified reference text.
    *Technical info: alphanumeric field, DB field: komm.kommtxt*
*   **Quantity Unit**: Quantity unit for the item, e.g. square meter. The search is restricted to all orders with this quantity unit.
    *Technical info: numeric field, DB field: kpos.me*
*   **Dimens. Variant**: Dimensional variant of the article. The search is restricted to all orders with these variant articles.
    *Technical info: numeric field, DB field: kpos.var*

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
*⇨ "Find Orders - Hit List" on page D-1076*

**Footer**
The buttons in the footer are described for the **Item Code** tab:
*⇨ "Find orders - document key" on page D-1069*

#### Find Orders – Direct Search

**Sales >Order Entry > Field Order > `<F9>` > Direct Search tab**

> **UI Screenshot Description:** Fig. D-8 shows the "Find Orders" dialog with the "Direct Search" tab active. The primary search field is "Orders from", allowing for a quick search starting from a specific order number.

You can search for orders on this tab starting with a particular order number. You can also specify additional search criteria on the **Document Key** and **Item Code** tabs.
If the search function should be restricted to the direct search for order numbers, the dialog can be configured so that the **Document Key** and **Item Code** tabs are deactivated. For customer-specific adjustments, contact your contact person at A+W Software GmbH.
*   Use `<F2>` to change to the header area of the tab.
*   Use `<F3>` to start the search.

**Direct Search Fields**

*   **Orders from**: Start number from which orders are searched for in ascending order. The search is restricted to all orders whose number is equal to or greater than the order number specified. The field name varies depending on the dialog from which you open the search, e.g. **Quotations from**.
    *Technical info: numeric field, DB field: kauf.auftrnr*

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
*⇨ "Find Orders - Hit List" on page D-1076*

**Footer**
The buttons in the footer are described for the **Item Code** tab:
*⇨ "Find orders - document key" on page D-1069*

## Find Orders – Hit List

**Sales >Order Entry > Field Order > `<F9>` > Enter search criteria > `<F3>`**

The hit list contains the following tabs:
*   "Find orders - delivery information" on page D-1077
*   "Find orders - miscellaneous" on page D-1079
*   "Find orders - quantities" on page D-1081
*   "Find orders - properties" on page D-1083
*   "Find orders - reference" on page D-1085

### Find orders – delivery information

> **UI Screenshot Description:** Fig. D-9 shows the "Find Orders" hit list with the "Delivery Information" tab active. It lists orders with columns like "Site", "Order", "SubNo", "Deliv. Date", "Cust.", "Proj.", "Invoice", "Act. Ref.No.", and "Cancelled".

This tab displays the delivery information and additional details about the orders that fit the search criteria.
Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Orders** dialog:
*⇨ "Find orders" on page D-1069*

**Record display for the document overview**
The number of hits in the list is indicated on the right, above the tabs, in a frame. The display means *Document overview: No. of the currently marked hits in the list: Total number of hits.*

**Delivery Info tab Columns**
*   **Site**: Site number.
    *Technical info: display field, DB field: kauf.hausnr*
*   **Order**: Order number. The column name and number vary depending on the document from which you open the search, e.g. quotation and quotation number for the quotation search.
    *Technical info: display field, DB field: kauf.auftrnr*
*   **SubNo**: Number of the partial delivery note or partial invoice.
    *Technical info: display field, DB field: kauf.subnr*
*   **Deliv. Date**: Planned delivery date.
    *Technical info: display field, DB field: kauf.ltplan*
*   **Customer**: Customer name.
    *Technical info: display field, DB field: kauf.orgkunr*
*   **Proj.**: Project number for orders to which a project is assigned.
    *Technical info: display field, DB field: kauf.objnr*
*   **Invoice**: Invoice number for invoiced orders.
    *Technical info: display field, DB field: kauf.rechnr*
*   **Act.Ref. No.**: Original reference number for transferred documents.
    *Technical info: display field, DB field: kauf._orgauftrnr*
*   **Cancelled**: Specification of the processing state, e.g. cancellation status.
    *   0: Order not cancelled.
    *   1: Order cancelled by the operator.
    *   2: Order cancelled by the system.
    *   -3, -10, ..., -x: Order in background processing.
    *Technical info: display field, DB field: kauf.still*

**Footer**
The buttons in the footer are described for the **Item Code** tab:
*⇨ "Find orders - document key" on page D-1069*

### Find orders – miscellaneous

> **UI Screenshot Description:** Fig. D-10 shows the "Find Orders" hit list with the "Miscellaneous" tab active. Columns include "Site", "Order", "SubNo", "Entry", "Operator", "Invoice", "VAT ID No.", "Ref.", and "Cancelled".

This tab displays various information about the orders that fits the search criteria.
Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Orders** dialog:
*⇨ "Find orders" on page D-1069*

**Show record**
The number of hits in the list is indicated on the right, above the tabs, in a frame. The display means *Document overview: No. of the currently marked hits in the list: Total number of hits.*

**Miscellaneous tab Columns**
The columns are described for the **Delivery Information** tab.
*⇨ "Find orders - delivery information" on page D-1077*
In addition, the following columns are displayed:
*   **Entry**: Date on which the order was entered.
    *Technical info: display field, DB field: kauf.edat*
*   **Operator**: Name of the operator who entered the orders.
    *Technical info: display field, DB field: kauf.eusr*
*   **VAT ID No.**: Customer's VAT ID.
    *Technical info: display field, DB field: kaufp.steuernr*
*   **Ref.**: Document number that is being referenced in the document entry.
    *Technical info: display field, DB field: kauf.referenz*

**Footer**
The buttons in the footer are described for the **Item Code** tab:
*⇨ "Find orders - document key" on page D-1069*

### Find orders – quantities

> **UI Screenshot Description:** Fig. D-11 shows the "Find Orders" hit list with the "Quantities" tab active. This view is an item overview, listing individual items from orders with columns like "ArtNo", "Article", "Qty", "Shipped", and "Invcd".

This tab displays item information about the orders that fit the search criteria. One line is displayed per order item.
Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Orders** dialog:
*⇨ "Find orders" on page D-1069*

**Show record for the item overview**
The number of hits in the list is indicated on the right, above the tabs, in a frame. The display means *Item overview: No. of the currently marked hits in the list: Total number of hits.*

**Quantities tab Columns**
The columns are described for the **Delivery Information** tab.
*⇨ "Find orders - delivery information" on page D-1077*
In addition, the following columns are displayed:
*   **Itm**: Item number in the order.
    *Technical info: numeric field, DB field: kpos.posnr*
*   **ArtNo, Article**: Article number and article name of the header article.
    *Technical info: numeric field, alphanumeric field, DB fields: kpos.artnr, kpos.artbez1*
*   **Qty**: Item quantity.
    *Technical info: numeric field, DB field: kpos.menge*
*   **Shipped**: Quantity of the item already shipped.
    *Technical info: numeric field, DB field: kpos.gelief*
*   **kmp.**: An asterisk `*` indicates if the item has been delivered completely.
    *Technical info: display field*
*   **Invcd**: Invoiced item quantity.
    *Technical info: display field*
*   **kmp.**: An `F` indicates if the item has been invoiced completely.
    *Technical info: display field*

**Footer**
The buttons in the footer are described for the **Item Code** tab:
*⇨ "Find orders - document key" on page D-1069*

### Find orders – properties

> **UI Screenshot Description:** Fig. D-12 shows the "Find Orders" hit list with the "Properties" tab active. This is an item overview focusing on physical properties, with columns like "QU", "sf", "ft", "Weight", "Width", "Hght", and "Dimens. Variant".

This tab displays additional item information for orders. One line is displayed per order item.
Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Orders** dialog:
*⇨ "Find orders" on page D-1069*

**Show record for the item overview**
The number of hits in the list is indicated on the right, above the tabs, in a frame. The display means *Item overview: No. of the currently marked hits in the list: Total number of hits.*

**Properties tab Columns**
The columns are described for the **Delivery Information** and **Quantities** tab:
*⇨ "Find orders - delivery information" on page D-1077*
*⇨ "Find orders - quantities" on page D-1081*
In addition, the following columns are displayed:
*   **QU**: Quantity unit for the item, e.g. square meter.
    *Technical info: display field, DB field: kpos.me*
*   **sf**: Glass area in square meters.
    *Technical info: display field, DB field: kpos.qm*
*   **ft**: Length specification for the item per piece in linear meters.
    *Technical info: display field, DB field: kpos.umlfdm*
*   **Weight**: Weight of the item in kilograms.
    *Technical info: display field, DB field: kpos.gewicht*
*   **Width, Hght**: Dimensions of the item in millimeters.
    *Technical info: display fields: DB field: kpos.laenge, kpos.breite*
*   **Dimens. Variant**: Dimensional variant of article.
    *Technical info: display field, DB field: kpos.var*

**Footer**
The buttons in the footer are described for the **Item Code** tab:
*⇨ "Find orders - document key" on page D-1069*

### Find orders – reference

> **UI Screenshot Description:** Fig. D-13 shows the "Find Orders" hit list with the "Reference" tab active. This item overview displays the "Article" and "Reference" text for each item.

This tab displays information about the references of the orders that fit the search criteria. One line is displayed per order item.
Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Orders** dialog:
*⇨ "Find orders" on page D-1069*

**Show record for the item overview**
The number of hits in the list is indicated on the right, above the tabs, in a frame. The display means *Item overview: No. of the currently marked hits in the list: Total number of hits.*

**Reference tab Columns**
The columns are described for the **Delivery Information** and **Quantities** tab:
*⇨ "Find orders - delivery information" on page D-1077*
*⇨ "Find orders - quantities" on page D-1081*
In addition, the following columns are displayed:
*   **Reference**: Reference text.
    *Technical info: display field, DB field: komm.kommtxt*

**Footer**
The buttons in the footer are described for the **Item Code** tab:
*⇨ "Find orders - document key" on page D-1069*

## Find market partner

**Sales > Order Entry > Field Customer > `<F9>`**

> **UI Screenshot Description:** Fig. D-14 shows the "Find Market Partner" dialog. It has search fields like "Matchcode", "Name", "Town", etc., and two tabs for the results: "Address" and "Identification". The Address tab is active, showing a list of customers with their addresses.

You can search for market partners on this dialog. You enter the search criteria in the header area. If you open **Find Market Partners**, you will see all market partners in the hit list that are stored in the master data and not yet disabled. With internal site separation, only the market partners are listed that are assigned to the site. Using the filter criteria, you can restrict the hit list.

You can configure in which search criterion field you are first located for input when you open the dialog. Configurable as initial input fields are the fields **From No.**, **Matchcode**, **Name**, **1stName**, **Cntry**, **PCd**, and **Town**.

You can call up the market partner search via various menu paths. The dialog always looks the same.
*   Use `<F3>` to start the search.
*   Use `<F2>` after the search to change tabs on the hit list.
*   Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

The hit list displays the addresses and information for identification of the market partners:
*   "Address tab" on page D-1089
*   "Identification tab" on page D-1090

> **Default setting for the market partner types**
> Depending on which menu path you use to open the dialog, the market partner type you're looking for can be set already, e.g. customer or supplier. The hit list is then filtered accordingly. The selection of the market partner types is only possible when searching in the master data.

### Search fields

*   **From No.**: Start number from which market partners are searched for in ascending order. The market partners whose number is smaller than the number specified are excluded from the hit list.
    *Technical info: numeric field, DB field: mp.mpnr*
*   **Matchcode**: Alphanumeric matchcode of the market partner. The market partners whose match code does not include the data specified are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: mp.mc*
*   **Type**: Display of the market partner type. The type is stored in the market partner master data. The field is automatically pre-populated by the system.
    *Technical info: display field, DB field: mp.kuliflag*
*   **Name, 1stName**: Name and first name of the market partner. The market partners whose names do not include the data specified are excluded from the hit list.
    *Technical info: alphanumeric fields, DB fields: mp.name, mp.vaname*
*   **Street**: Street address of the market partner. The market partners whose street address does not include the data specified are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: mp.strasse*
*   **Site**: Site number with internal site separation. The market partners that are not assigned to the specified site are excluded from the hit list.
    *Technical info: numeric field, DB field: mpmdzu.hnr*
*   **Country**: International country code of the market partner. The market partners whose country codes do not include the specified data are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: mp.land*
*   **PCd, Town**: Postal code and city name for the market partner's address. The market partners whose postal code and city do not include the data specified are excluded from the hit list.
    *Technical info: alphanumeric fields, DB fields: mp.plz, mp.ort*
*   **VAT ID No.**: Market partner's VAT ID number. The market partners whose identification number does not include the specified data are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: mp.steuernr*
*   **Kind**: Market partner status. In the order entry, only active market partners are displayed. This field cannot be edited.
    *Technical info: display field, DB field: mp.still*

### Show record for the market partner overview

The number of hits in the list is indicated on the right, above the tabs, in a frame. The display means *Item overview: No. of the currently marked hits in the list: Total number of hits in the list.*

> **The display of hits is loaded record by record**
> If a large number of hits has to be displayed, under some circumstances, it can take some time for the system to do this. So that the hit list can be displayed quickly, it is loaded record by record. The record size is configured in the system settings. The hits are loaded in numeric sequence, e.g. the first 100 hits numerically. Additional hits can be loaded with the **[More Data]** button.

**Example**
`11:100 (1256)` is displayed in the record display.
*   **11** stands for the number of the marked hit in the hit list.
*   **100** stands for the number of hits that are currently displayed in the hit list.
*   **1256** stands for the number of all hits.

### Address tab

The columns in the hit list correspond to the fields in the header area. In addition, the following columns are displayed:
*   **Number**: Market partner number.
    *Technical info: display field, DB field: mp.mpnr*
*   **Addition**: Additional note, e.g. an address addition.
    *Technical info: display field, DB field: mp.branche*

### Identification tab

The columns in the hit list correspond to the fields in the header area. In addition, the following columns are displayed:
*   **Number**: Market partner number
    *Technical info: display field, DB field: mp.mpnr*
*   **Dis.**: Disabled: Indication of whether the market partner has been disabled.
    *   **Y**: Market partner has been disabled.
    *   **N**: Market partner is active.
    In the order entry, only active market partners are displayed.
    *Technical info: display field, DB field: mp.still*
*   **Type**: Type of the market partner, e.g. customer, supplier.
    *Technical info: display field, DB field: mp.kuliflag*
*   **Company**: Number of the company of the market partner with internal site separation. The company number is drawn from the system master data.
    *Technical info: Anzeigefeld, DB field: xcompany.compid*

### Description of buttons in the footer

Use the buttons in the footer to navigate in the hit list, display additional hits, and update the hit list.

*   **[OK]**: Cancels the current order.
*   **[Cancel]**: Cancels the cancellation.
*   **[<]** and **[>]**: Use these buttons to jump to the first or last entry in the hit list.
*   **[<<]** and **[>>]**: Use these buttons to display the previous or next page of the hit list.
*   **[Refresh]**: Updates the entries in the search fields. Corrected or additional entries in the search fields are taken into account during the search. The button is only enabled in the **Search fields** area.
*   **[Additional data]**: Displays additional entries in the hit list that correspond to the search criteria. If no more hits can be displayed, the button is locked.
*   **[New search]**: Deletes all search criteria for a new search. Alternatively, you can use `<Ctrl>` + `<R>` to delete the search criteria and start a new search.

## Employee/authorization groups

**Sales > Order entry > Properties tab > Operator field > `<F9>`**

> **UI Screenshot Description:** Fig. D-15 shows the "Employee / Authorization Group" dialog. It allows searching for employees with fields like "Name", "Departm.", and "Login". The results are listed with columns for "Number", "Name", "1stName", "Login", "Departm.", and "Type".

Use this dialog to search for employees. Enter the search criteria in the header area. If you open the employee search, all employees are displayed in the hit list. You can use the filter criteria to restrict the hit list.

You can call up the employee search via various menu paths. The dialog always looks the same.
*   Use `<F3>` to start the search.
*   Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

The hit list displays the employees who correspond to the search criteria:
*⇨ "Hit list" on page D-1092*

### Search fields

*   **From No.**: Start number from which employees are searched for in ascending order. The employees whose number is smaller than the number specified are excluded from the hit list.
    *Technical info: numeric field, DB field: mp.manr*
*   **Type**: Display of the employee type. The type is stored in the employee master data. The field is automatically pre-populated by the system.
    *Technical info: display field, DB field: mitarb.matyp*
*   **Name, 1stName**: Employee's last name and first name. The employees whose names do not contain the specified data are excluded from the hit list.
    *Technical info: alphanumeric fields, DB fields: mitarb.maname, mitarb.vname*
*   **Departm.**: Number and name of the department. If you specify a number, the name of the department is displayed in the second field.
    *Technical info: numeric field, display field, DB fields: mitarb.abtnr, abteilung.bez*
*   **Login**: User name of the employee for login to A+W Enterprise.
    *Technical info: alphanumeric field, DB field: mitarb.loginname*

### Show record for the employee overview

The number of hits in the list is indicated on the right, above the tabs, in a frame.
The record display is described for the **Find Market Partner** dialog:
*⇨ "Find market partner" on page D-1087*

### Hit list

The columns in the hit list correspond to the fields in the header area. In addition, the following column is displayed:
*   **Number**: Employee number
    *Technical info: display field, DB field: mitarb.manr*

### Footer

Use the buttons in the footer to navigate in the hit list, display additional hits, and update the hit list.
The fields and buttons in the footer are described in detail in the the **Find Market Partner** section:
*⇨ "Find market partner" on page D-1087*

## Find deference document

**Sales > Order Entry > Reference field > `<F9>`**

> **UI Screenshot Description:** Fig. D-16 shows the "Find Reference Document" dialog. It is structured similarly to the "Find Orders" dialog, with tabs for "Document Key", "Item Code", "Direct Search", and several hit list tabs. It is used to find and link to other documents within the system.

Use this dialog to search for documents to which you can make reference in document entry.
Specify the search criteria in the header area. The search results are shown in the hit list. The hit list is only displayed if you have started the search.
*   Use `<F2>` to change to the header area of the tab.
*   Use `<F3>` to start the search.
*   Use `<F2>` after the search to change tabs on the hit list.

The dialog is structured the same as the **Find Orders** dialog.
*⇨ "Find orders" on page D-1069*

### Item Code tab

Most fields are described for the Item Code tab for finding orders:
*⇨ "Find orders - document key" on page D-1069*
In addition, the following fields are displayed:
*   **Document**: Document type. The search is restricted to all documents of this type.
    *   Quotation
    *   Order
    *   Supplier inquiry
    *   P.O.
    *Technical info: selection field, DB field: kauf.vorgang*

    > **Default setting for the document type**
    > The document type is pre-set user-specifically, e.g. Quotation. You configure the default setting in the system settings.

*   **Document number**: Number and subnumber of the reference document. The search is restricted to all documents with this number and/or subnumber.
    *Technical info: numeric field, display field, DB fields: kauf.auftrnr, kauf.subnr*
*   **Scheduled**: Scheduled delivery date of the reference document in the format DD.MM.YYYY. The search is restricted to all documents with this delivery date.
    *Technical info: date field, DB field: kauf.ltplan*

### Item Code tab

The fields are described for the **Item Code** tab for finding orders:
*⇨ "Find orders – item code" on page D-1072*

### Direct Search tab

*   **Orders from**: Start number from which orders are searched for in ascending order. The search is restricted to all orders whose number is equal to or greater than the order number specified. The field name varies depending on the dialog from which you open the search, e.g. **Quotations from**.
    *Technical info: numeric field, DB field: kauf.auftrnr*

### Hit list

The tabs in the hit list are described in detail for finding orders:
*⇨ "Find Orders - Hit List" on page D-1076*

### Footer

The buttons in the footer are described in finding orders for the **Item Code** tab:
*⇨ "Find orders - document key" on page D-1069*

## Find addresses

**Sales > Order Entry > Header, Footer, Item level > `<F4>` > Addresses > Find Delivery Address**

> **UI Screenshot Description:** Fig. D-17 shows the "Find Addresses" dialog. It is used to search for a market partner's delivery addresses. Search fields include "Name", "Street", "PCd". The results show different addresses for a selected customer.

Use this dialog to search for the market partner's addresses. Enter the search criteria in the header area. When you open the address search, all the market partner's addresses will be displayed in the hit list. You can restrict the hit list with the filter criteria.
*   Use `<F3>` to start the search.
*   Use `<F2>` after the search to change tabs on the hit list.
*   Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

The delivery addresses and additional contact data for the market partners are displayed in the hit list.
*⇨ "Address tab, Contact Data tab" on page D-1096*

### Search fields

*   **Name**: Customer name. The addresses of customers whose name does not contain the specified data are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: adr.adrname*
*   **Street**: Street address of the delivery address. The addresses whose street addresses do not contain the specified data are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: adr.str*
*   **PCd**: Postal code of the delivery address. The addresses whose postal code does not include the specified data are excluded from the hit list.
    *Technical info: alphanumeric fields, DB fields: adr.plz, adr.ort*
*   **Town**: City name of the delivery address. The addresses whose city does not contain the specified data are excluded from the hit list.
    *Technical info: alphanumeric fields, DB fields: adr.plz, adr.ort*
*   **Cntry**: Country name for the delivery destination. The addresses from countries that do not contain the specified data are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: adr.land*
*   **Address code**: Code of the saved address. The addresses whose address code does not include the specified data are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: adr.text1*
*   **Tel**: Customer's telephone number. The addresses whose telephone number does not include the specified data are excluded from the hit list.
    *Technical info: alphanumeric fields, DB fields: adr.telefon, adr.email*
*   **E-mail**: Customer's e-mail address. The addresses whose e-mail address does not include the specified data are excluded from the hit list.
    *Technical info: alphanumeric fields, DB fields: adr.telefon, adr.email*
*   **Incl. quick entry**: Specification of whether addresses are listed that are saved via quick entry.
    *   The addresses from quick entry are displayed in the hit list.
    *   No addresses from quick entry are displayed in the hit list.
    *⇨ "Quick entry" on page D-1130*
    *Technical info: checkbox*

### Main ship. address

The market partner's main delivery address is displayed on the right above the tabs.
If the market partner is not assigned a main delivery address, no main address is displayed.

### Address tab, Contact Data tab

The columns on the item level correspond to the fields in the header area.
*⇨ "Search fields" on page D-1095*
In addition, the following column is displayed:
*   **First name**: Customer's first name.
    *Technical info: display field, DB field: adr.adrvname*

### Description of buttons in footer

*   **[Details]**: Opens a dialog with the details about the marked delivery address. Alternatively, you can open the dialog with `<F5>`. The button is only enabled if an address is marked in the hit list.
*   **[New search]**: Deletes all search criteria for a new search.

## Find article

**Sales > Order entry > Items tab > General tab > Article field > `<F9>`**

Use this dialog to search for articles that you need for the entry of an order. You can call up the article search via various menu paths. The dialog always looks the same.

The hits for the search are displayed on the tabs. If you open the article search, you will see all articles in the hit list. Using the filter criteria, you can restrict the hit list.
*   Use `<F3>` to start the search.
*   Use `<F2>` after the search to change tabs on the hit list.

The search results are shown in the hit list. The hit list is only displayed if you have started the search.
This dialog contains the following tabs:
*   "Find article - header, footer areas" on page D-1098
*   "Find article - names" on page D-1101
*   "Find article - article codes" on page D-1103
*   "Find article - details" on page D-1105

The search results are shown in the hit list. The hit list is only displayed if you have started the search.

### Find article – header, footer areas

**Sales > Order entry > Items tab > General tab > Article field > `<F9>`**

> **UI Screenshot Description:** Fig. D-18 shows the "Find Article" dialog. The header contains numerous search fields like "Article Code", "Main Name", "Art. Type", "Supplier", etc. The results are displayed in a list with tabs for "Names", "Article Codes", and "Details". An "Article Image" pane is also visible.

Use this dialog to search for articles using various search criteria.
If you open the article search, you will see all articles in the hit list. Using the filter criteria, you can restrict the hit list.

#### Header

Specify the search criteria in the header area. The hits for the search are displayed on the tabs.
Use `<F3>` to start the search.

*   **From no.**: Start number from which articles are searched for in ascending order. The articles whose number is smaller than the number specified are excluded from the hit list.
    *Technical info: numerical field, DB field: artikel.artnr*
*   **Matchcode**: Alphanumerical matchcode of the article. The articles whose match code does not include the data specified are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: artikel.artmc*
*   **Article Code**: Article code from master data. The articles whose article code does not include the specified data are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: artikel.artikelcode*
*   **Short Name**: Short name of the article. The articles whose short name does not include the data specified are excluded from the hit list.
    *Technical info: alphanumeric field, DB field: artikel.kurzbez*
*   **Main Name, Intern. Description, Internal2**: Main name and additional descriptions of the article. The articles whose main name or internal name does not include the data specified are excluded from the hit list.
    *Technical info: alphanumeric fields, DB field: artikel.artbez1, artikel.artbez2, artikel.artbez3*
*   **Art. Type, to**: Number and description of the article type. In the **Art. Type** field, enter the number starting from which you will search for articles. In the **to** field, you restrict the search to articles with the appropriate article type. The articles whose article type number is smaller than the number specified in the **Art. Type** field or greater than the number in the **to** field are excluded from the hit list. When you enter a number, the description of the article type is displayed in plain text. Use `<F9>` to search for an article type.
    *Technical info: numeric fields, display fields, DB fields: artikel.atyp*
*   **A+W Proc. Type, to**: Number and description of the A+W-specific processing type. In the **A+W Proc. Type** field, enter the number starting from which you want to search for articles. In the **to** field, you restrict the search to articles with the appropriate processing type. When you enter a number, the description of the processing type is displayed in plain text. With `<F9>` you can search for a processing type.
    *Technical info: numeric fields, display fields, DB field: artikel.awtyp*
*   **Prod. Group**: Code of the product group to which the article is assigned.
    *Technical info: alphanumeric field, DB field: artikel.wagrp*
*   **Material Grp.**: Code of the material group to which the article is assigned.
    *Technical info: alphanumeric field, DB field: artikel.artgrp*
*   **Supplier**: Number of supplier from whom the article is ordered. You can select the supplier from the list of suppliers using `<F9>` > `<F8>`.
    *Technical info: numeric field, DB field: artikel.stdlinr*
*   **Type**: Display of the article status. In the document entry, only active articles are displayed. The field cannot be edited.
    *Technical info: display field, DB field: artikel.still*

#### Article Image

The lite structure of the marked article from the hit list is shown in cross-section here. The sun marks the outside of the lite.

#### Description of buttons in footer

Use the buttons in the footer to navigate in the hit list, display additional hits, and update the hit list.
*   **[OK]**: Cancels the current order.
*   **[Cancel]**: Cancels the cancellation.
*   **[<]** and **[>]**: Use these buttons to jump to the first or last entry in the hit list.
*   **[<<]** and **[>>]**: Use these buttons to display the previous or next page of the hit list.
*   **[Refresh]**: Updates the entries in the search fields. Corrected or additional entries in the search fields are taken into account during the search. The button is only enabled in the **Search fields** area.
*   **[Additional data]**: Displays additional entries in the hit list that correspond to the search criteria. If no more hits can be displayed, the button is locked.
*   **[New search]**: Deletes all search criteria for a new search. Alternatively, you can use `<Ctrl>` + `<R>` to delete the search criteria and start a new search.
