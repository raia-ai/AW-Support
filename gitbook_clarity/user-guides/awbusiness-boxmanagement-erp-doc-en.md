---
description: "EN_AWBusiness_Box_Management_1_1-2"
---


---
## Master Data for Boxes

5. Check the checkbox **Search stock PP (C)** if the stock size is to be included in pricing.
6. In addition, you can enter name and short name (matchcode), e.g. for better identification of stock articles.
7. Enter the procurement type (D), e.g. **Stock withdrawal** for stock articles.
8. Go to the menu **Start > Save** to save the data.
   The data is saved. Next, the system will want to know whether you want to define this stock size as a stock article as well.
9. Choose [Yes] if the stock size is also to be managed as a stock article.
   The **Stock management** dialog opens.

### Creating stock articles for box

For a stock article Box you have to define at least the following settings in order to manage the stock:
- Article number and name
- Sizes for stock sizes, sizes and contents for boxes
- Storage location and standard storage location (default storage location)
- Stock on hand

> **Stock start-up**
> If no stock articles have been entered at all, you can facilitate this task by running the so-called initial inventory. This function is described in the **Stock management** section.

**How to create a stock article**

1. Go to menu **Stock management > Stock management**.
   The **Stock management** dialog opens.
2. Go to the menu **Start > New** to switch to the input mode.
   If you open the **Stock management** dialog from the master data, this step can be omitted. The fields for articles and sizes are filled in already.

*Fig. K-11: Fields for new stock articles are enabled. (A) Stock article number, (B) Size and content of the box, (C) Storage location, (D) Main product, (E) Stock on hand, (F) Inventory audit.*

3. Enter the number (A) the size and the content of the box (B).
4. Choose a storage location (C).
   If no storage location is selected, the storage location `<n.e.>` will be entered. In stock management, this will be treated like the defined storage locations, e. g. for stocktaking purposes and queries.
   If a stock article is kept in different storage locations, you have to define one of them as the standard storage location.
5. Check the **Default storage location** checkbox.
6. Go to the **Main product** field (D) and select the article for which you want to enter the minimum stock for the inventory audit.
   For boxes, this is the stock plate from which the sheets are cut.
7. Check the checkbox **Inventory audit per stock location (F)** if all storage locations shall be evaluated separately when checking the inventory for this stock article.
8. Change to the **Prices** tab and enter the quantity unit with which the average price is calculated.

*Fig. K-12: Average price for stock articles. (A) Average price, (B) Quantity unit.*

9. Change to the **Supplement** tab and check whether the supplier 0 is entered for the boxes from production.
   With this setting, you specify that you yourself are the supplier. This setting has no effect on the boxes that you can alternatively order from a supplier, for such boxes are not kept in stock.
10. Go to the menu **Start > Save** to save the data.
    The data is saved.
11. Repeat steps for all fixed dimensions that can be entered as boxes.
    For boxes, you specify a stock article per glass, dimension, content, and price key.
    Thus all necessary information A+W Business needs for reservations and booking have been defined.

## Box with BOM

**Objectives**
- Getting familiar with the product structure of boxes with BOMs (pallets).

**Benefits**
- Boxes with a deeply graduated BOM can be defined and entered as products.

**Please note**
- **Product structure**: The article structure of boxes with a BOM is more complex than that of simple glass boxes.
- **Default settings**:
    - **Stock management**
    - **Master data**:
        - Product management
        - Supplier list
    - **Company data**:
        - Parameters tab
        - Stock / PP / EDI tab

### Master data for boxes with BOMs

Boxes with BOM are articles the structure of which is more complex than the glass boxes known so far. Picture frame glass can be wrapped in paper for example, and can then be put onto a pallet.

The pallet is defined as the main product and the paper box with the sheets, as its BOM. Both the pallet and the paper box belong to the product type Box.

> **Previous knowledge required for this unit**
> This session is not about working on new dialogs or functions. Boxes with BOMs have a special product structure that is defined by means of the already known tools. For information regarding the production BOMs, please see the **Master Data** section.

### BOM structure

*Fig. K-13: Product management – BOM with complex box. (A) Main product: pallet, (B) BOM: box with glass sheets.*

The illustration shows the BOM structure of such a pallet. You will thus require a product for the pallet, a product for the box and the glass itself.

### Product type

To make sure that A+W Business interprets the pallet and the box as boxes, product type **200 - Box** must be set for both.

*Fig. K-14: Product management – Product tab.*

### Procurement type and stock booking type

To maintain both products on stock, the procurement type must be set to **Stock withdrawal**, and the stock booking type to **size-dependent**.

*Fig. K-15: Product management - tab Stock/Purchasing.*

> **Define pallet with BOM**
> When you define the pallet and the BOM please make sure that the correct procurement type is adopted.

### Standard sizes

Product input at item entry becomes a bit easier if a standard width and a standard height are entered for the product. After entering the article number, the matching box article will be automatically selected at item entry in this case.

*Fig. K-16: Product management – Product tab (optional).*

### Price code

Unlike for the boxes known already, the codes for Price-relevant SP/PP are analyzed for pricing on main product and BOM level.

Previously, the box price used to be calculated and shown only in the box BOM. For boxes with BOMs, this can be configured by means of the Price-relevant codes. Depending on these codes, the sales price is thus determined by the price of the BOM element, the price of the main item, or both.

If in our example, the price of the pallet shall consist only of the total prices of the boxes, i.e. the BOM, the main article's code must be disabled and that of the first BOM component, i.e. of the box, must be enabled.

*Tab. K-1: Pricing in connection with the setting of the 'price-relevant' code*

| Product | Price-relevant | Price calculation |
|---|---|---|
| Pallet | Yes | Price per pallet and number of boxes |
| Box | Yes | |
| Pallet | Yes | Price per pallet |
| Box | No | |
| Pallet | No | Price based on the number of boxes |
| Box | Yes | |

### Price management

Price management allows you to enter the box prices as usual.

*Fig. K-17: Price management – Matrix tab.*

A matrix with the two limit types **Exact width** and **Exact height** can be useful for example. This allows you to define unit prices for the different sizes.

### Stock sizes (product management)

A stock size must be defined for every pallet and box variant in dialog **Stock sizes**. The variants are the glass sizes. The procurement type must be set to **Stock withdrawal** so that the stock size can be kept on stock.

**Example**

The stock size Pallet with boxes shall consist of 80 boxes each, each of which again includes 25 sheets.

It is essential that for every size, just one stock size is defined with unique contents. This means that you must not enter pallets of 50 and pallets with 80 boxes for the size 600 x 700.

*Fig. K-18: Product management stock sizes – Pallet of 80 boxes and box of 25 sheets.*

You can define a diversion to other price keys for the stock sizes (as usual).

When the new stock size is saved, you can directly switch from the query to stock management to define the related stock articles.

### BOM box in stock management

Stock articles are defined in the same way as product stock sizes. The article is entered with the same sizes and contents. Additionally, the current stock on hand and the storage location are defined.

For the automatic creation of stock P.O.s, you also have to fill in the fields **Minimum stock** and **P.O. quantity**.

*Fig. K-19: Stock management – Pallets of 80 boxes, box of 25 sheets.*

### BOM box at item entry

If you enter the pallet in an item, first enter the article number as usual:
- If the standard width and height have been defined in product master data, the box will be automatically created from the product stock sizes.
- To enter the product with other sizes or if no standard size has been defined, use stock search to select the required pallet.

On the **BOM** tab, the components are preset with the corresponding contents.

*Fig. K-20: Document management - tab BOM: Pallet. (A) Number of boxes on the pallet, (B) Number of sheets per box.*

The box and its BOM can be entered like any other product. If kept as a stock article, it can also be used to replenish the stock on hand by means of production orders.

**Additional information**
- Sales, "Order Header" on page C-38
- Sales, "Change P.O. Code" on page C-306

## Orders

Orders for boxes come in two forms:
- **Sales order for a customer.**
- If in addition to the boxes produced, you also sell boxes ordered, the settings for the suppliers must also be specified on the **Supplier** tab.
- **Production order to fill up stock.**

This section provides information on the following subjects:
- "Sales Order with Box" on page K-37
- "Production Orders" on page K-41

### Sales Order with Box

In a sales order, you enter a box for a customer. This box can be removed from your stock on hand or ordered from a supplier.

**How to enter a box as an order item**

1. Go to menu **Documents > Order > Order** and enter the order header.

*Fig. K-21: Order header for sales order. (A) Order area, (B) Order type.*

   Pay attention to the settings for the order area and the order type.
2. Save the data and change to the **Items** tab.
   Item entry opens.
3. Go to the menu **Start > New** to enter a new item.

*Fig. K-22: Enter product number of the glass in the box.*

4. Enter the product number of the glass for which you want to enter an entire box.
5. Go to the menu **Start > Stock search** to open the **Stock info** dialog.

*Fig. K-23: Stock information on boxes. (A) Product number of the glass, (B) Box (without inventory).*

   The **Stock info** dialog shows a list of all boxes and stock sizes available for this product number. Boxes with the storage location `<n.e.>-<n.e.>-<n.e.>` are boxes that are created as stock articles. Boxes with inventory generally have an ID.
6. Adopt the marked box with a double-click.
   Pay attention to the specified dimensions if you are working with different boxes for a product.

The dialog is closed and you will find yourself back at item entry.

*Fig. K-24: Item with box entered. (A) Procurement type.*

7. Select the procurement type (A).
   - **Stock withdrawal:** The box will be withdrawn from stock.
   - **Order (complete):** The box will be ordered from the supplier who is entered on the **Supplier** tab. For this setting, the order must then be transferred to purchasing.
8. If necessary, correct the quantity if you want to enter more than one box.
9. Go to the menu **Start > Save** to save the data.
   The data is saved. You can now enter additional items and complete the order as usual.
   If you book the goods receipt of the box delivery by a supplier, the boxes delivered will be assigned to the order. There is a detailed description in the **Purchasing** section.

### Production Orders

Production orders are used to replenish the stock on hand. All articles entered in such an order are automatically changed to procurement type **Production**. Unlike customer orders, the items are not reserved on stock but are marked as ordered.

**Manual and automatic stock P.O.**

*Fig. K-25: Stock P.O. vs. production order.*
*This flow chart shows a process: It starts with a `Storage location`. It checks if the stock is `Below minimum stock?`. If yes, it checks for `Standard P.O. quantity?`. If yes, it proceeds to `Search in supplier file`. Then it checks for `Standard supplier?` or `Internal customer`. If `Standard supplier?` is yes, it leads to a `P.O. proposal Stock P.O.`. If `Internal customer` is yes, it leads to a `Production order Document management`.*

This flow chart shows A+W Business's reactions to different presettings in the supplier file.
The program checks whether the current stock on hand plus the already ordered quantities and minus the reserved quantities will fall below the minimum stock on hand. If this is the case, the P.O. proposal shows the multiple of the (standard) P.O. quantity.

**Settings in Supplier File**

If a minimum stock and a (standard) order quantity have been defined for the stock article in dialog **Stock management**, the system can create automatic P.O. proposals. These are listed in dialog **Stock P.O.**

This is how purchase orders of the type **Stock P.O.** are usually created. However, if an internal customer is entered in the supplier file instead of a standard supplier, production orders can be created automatically.

*Fig. K-26: Internal customer for production orders.*

In the supplier file, an internal customer is defined for which the production order is entered automatically. The option **Internal customer** can be enabled on product group or product level. The product settings have priority over the product group settings.

**Purchase order quantity**

The multiplier will be calculated so that as a result of the P.O. proposal the minimum stock is exceeded.

*Fig. K-27: Quantities for stock articles (dialog Stock management).*

**Example**

Laminated glass with article number 107 is kept as a stock article.
- Current stock on hand: 10 pcs.
- Minimum stock: 30 pcs.
- P.O. quantity: 5 pcs.

The P.O. quantity for laminated glass 107 is calculated as follows:
Difference between current stock on hand and minimum stock on hand: 20 pcs. This difference includes the P.O. quantity of 5 pcs. four times.

P.O. quantity: 4 x 5 = 20 pcs.
Current stock on hand plus ordered quantity: 10 + 20 = 30 pcs.

The calculated quantity is adopted for the P.O. proposal. It can be amended in the **Stock P.O.** dialog. How you edit and transfer is described in the **Purchasing** section.

The production order is created by the transfer, in the last active order Number Manager. The production order can be edited and transferred to production.

### Enter production order

If you enter production orders manually, you can enter a previously entered order by copying it and transferring it to production.

> **Labels for receipt of goods**
> In order to enter a self-produced box in receipt of goods via PDC, a label/barcode is required. For this, the print item 973 must be assigned.

This section provides information on the following action sequences:
- "Entering header data for a production order" on page K-44
- "How to enter the glass for the box" on page K-46
- "How to enter a production order by copying" on page K-47

**Entering header data for a production order**

1. Go to **Documents > Order > Order**.
   The dialog **Document management** opens. In this description it is the **Edit** mode.
2. Go to the menu **Functions > Document > Select NM** and check if the correct number manager has been set, and correct the setting if necessary.
   The allocation of the order to a number manager is also shown in the order header.
3. Go to the menu **Start > New** to switch to the input mode.
4. Enter the required header data.

*Fig. K-28: Header data for production order. (A) Order area, (B) Production order.*

5. If necessary, enter an explanation for the order in the fields under the name; for example, that the sheets should be packed in boxes.
6. Choose the order type (B) **Production order**.
7. Check the other details.
8. Go to the menu **Start > Save** to save the data.
   The header data will be saved. Now you can go to the **Items** tab and enter the order items.
   The **Items** tab will be locked again if you change data in the order header. You have to save the changes to enable the **Items** tab again.

**How to enter the glass for the box**

1. Select **Documents > Order > Select order > Items tab** or `<F9>`.
   Item entry opens.
2. Go to the menu **Start > New** to enter a new item.
3. Enter the product number of the glass that should be produced as box.

*Fig. K-29: Enter product number of the glass in the box.*

4. Set the quantity to the content of the box or a multiple of the content.
5. Select in the menu **Start > Save** to save the data.
   The data is saved. It is transferred to production.
   If you enter production orders on a regular basis, you can copy the previously entered order to make this task easier. For a detailed description, please see the **Sales** chapter.
   - Before copying, you have to set the document type of the target document to **Production Order**.
   - If only certain items shall be adopted from the order, you can select them.
   - You can amend the data in the new document.

**How to enter a production order by copying**

1. Select **Documents > Order > Select Order**.
   The order entry opens.
2. Select menu **Functions > Copy documents**.

*Fig. K-30: Create production order by copying. (A) Copy from order to order, (B) Document type of the target order.*

3. Change to the **Copy by item** tab and mark the item(s) that should be copied.
4. Correct the target quantity if necessary.
5. To generate the copy, go to the menu **Start > Execute**.

## Stock Management for Boxes

For stock articles, both the goods receipt as well as the goods removal are entered so that you can manage inventories.

The receipt and withdrawal of boxes can be entered using barcodes (PDC) or manually.

This section provides information on the following subjects:
- "Stock Management of Boxes" on page K-48
- "Stock P.O. of boxes" on page K-49
- "Receipt of Goods via Barcode" on page K-54
- "Manual Stock Bookings" on page K-60
- "Shipping of Boxes" on page K-55

### Scanning

In connection with **AWPort**, stock bookings can also be entered via barcode. This does not only include receipt and withdrawal of goods but also opening of boxes and other reallocation actions.

By scanning, entire boxes can be allocated to a certain order or order item, or can be registered for the inventory including the sheets it contains.

- "Receipt of Goods via Barcode" on page K-54

For more information on barcodes and barcode formats, please refer to the documentation on **AWPort**.

### Stock Management of Boxes

Delivered boxes generally have an ID from the supplier with which they are entered when received.

Every box is booked with its own box ID by which it is kept on stock. The checkbox for assigning virtual item numbers must be checked in the company data.

- "Company Data" on page K-18
- "Receipt of Goods via Barcode" on page K-54

### Open boxes

To register individual sheets of a box you have to open the box. First, a box (with ID) is removed from the stock on hand. The number of sheets is then added to the stock on hand for the corresponding stock article (stock size).

### Stock P.O. of boxes

The inventory of boxes can either be filled up with an automatically or manually generated production order.

Stock P.O.s can also be created manually, via document management.

- "How to enter a stock P.O. with boxes" on page K-51

**P.O. proposals**

Purchase orders are usually created through stock management in order to keep the stock on hand on the required level.

*Fig. K-31: Stock management - Stock on hand figures. (A) Minimum stock, (B) Quantity for P.O. proposal.*

If you have defined minimum quantities (A) for a stock article in dialog **Stock management**, P.O. proposals are created automatically with the stored P.O. quantity (B). You can check these before they are transferred to Purchasing, and change the supplier and date if necessary. Transfer to Purchasing turns the proposal into a stock P.O.

### Stock Addition based on Production Order

On tab **Stock / PP / EDI** in company data, set the limit status for registration points to define from which point on an order counts as produced. The limit status is the status defined for the selected registration point.

*Fig. K-32: Company data – Stock / PP / EDI: Registration point for status change.*

There are two ways of entering additions to stock based on production orders:
- If the status of the production order exceeds the defined status due to a report from production, the addition to stock is booked automatically.
- If you do not use production reports, you can enter the addition to stock by means of the manual status report in the **Production** module. If you set the production order there to a status above the aforementioned limit, the stock withdrawal of the material consumed and the addition of produced stock articles to stock are booked automatically.

If no other storage location has been defined, the order quantity is allocated to the standard storage location.

The booking of production orders is described in detail in section **Production**.

**Additional information**
- Master Data, "Company Data – Stock/Purchasing/EDI" on page B-955
- Sales, "Order Header" on page C-38
- Sales, "Change P.O. Code" on page C-306
- Production, “Production Orders" on page E-128
