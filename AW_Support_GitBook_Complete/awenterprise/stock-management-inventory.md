---
title: "US_AWEnterprise_StockManagement_HelpCards"
source: "US_AWEnterprise_StockManagement_HelpCards.pdf"
tags: ["A+W Enterprise", "Stock Management", "Inventory", "Help Cards", "ERP", "Software Documentation", "Glass Manufacturing", "Window Manufacturing", "Master Data", "Warehouse Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a set of 'Help Cards' for the A+W Enterprise Stock module. It serves as a quick-reference guide for performing various stock management tasks, including master data management, stock movements (booking in/out), inventory counts, and system information retrieval."
long_description: "This document is a comprehensive collection of 'Help Cards' for the A+W Enterprise Stock module, based on the 2015 version of the software. It is designed to guide users through standard procedures related to stock and inventory management within the A+W Enterprise system, which is specialized software for the glass, windows, and doors industry. The guide is broken down into key functional areas: Master Data Management (creating storerooms and stock articles), Stock Management (booking items in and out of various warehouse types like standard, slot, box, and rack warehouses), Inventory Management (performing stock takes), Valuation (evaluating article prices), and using the Info System to view data like stock history, order status, and forecasts. Each help card details the objective of a specific task, lists any prerequisites, provides additional information, outlines a step-by-step workflow, and includes a corresponding screenshot of the user interface. These cards are essential for training and daily operations, ensuring users can efficiently manage stock levels and movements."
---

# A+W Enterprise: Stock Help Cards

> The depictions in the Help Cards are based on delivery version A+W Enterprise 2015. Individual steps in the workflows can differ depending on the configuration.

## Table of Contents

### Master data management

| Help Card | Subjects |
| --- | --- |
| Create a storeroom | Define a stock and all associated master data. |
| Define a stock article | Manage stock articles per stock. |

### Stock management

| Help Card | Subjects |
| --- | --- |
| Book warehouse in | Book warehouse in articles. |
| Book warehouse out | Book warehouse out articles. |
| Book warehouse in in slot warehouse | Book warehouse in articles in slot warehouse. |
| Book warehouse out in slot warehouse | Book warehouse out articles in slot warehouse. |
| Book box warehouse in | Book a complete box in box warehouse in. |
| Book box warehouse out | Book a complete box in box warehouse out. |
| Single sheet box warehouse in | Book single sheets in the single sheet box warehouse. |
| Single sheet box warehouse out | Break up single sheet box and book glass sheets from the single sheet box to another stock. |
| Book rack storage receipt | Book articles on racks in a rack warehouse. |
| Rack storage exit | Book order-related stock removals in the rack warehouse. |
| Transfer rack stock articles | Transfer article variants to a new rack or slot. |
| Book order-related outgoing stocks | Book order-related stock removals. |
| Stack warehouse in | Book a new stack in the warehouse in stack. |
| Modify stack warehouse | Book articles to existing stacks. Break up a stack and book articles from the stack warehouse. |
| Make a booking correction | Correct bookings in the stock. |

### Inventory management

| Help Card | Subjects |
| --- | --- |
| Take inventory of a stock | Take inventory of a stock. |

### Valuation

| Help Card | Subjects |
| --- | --- |
| Evaluation of stock | Undertake a valuation of article prices. |

### Info system

| Help Card | Subjects |
| --- | --- |
| View info about articles | View information about articles of the stock. |
| View stock history | View information about bookings in the stock history. |
| View orders/purchase orders | View information about job and order-related bookings. |
| View booking status | View and correct non-booked or incorrect bookings. Call up overview for all stocks in the inventory. |
| View available stock | View ordered, planned, and available stock. |
| View stock forecast | View stock forecast for planned stocks of a time period. |

### Print

| Help Card | Subjects |
| --- | --- |
| Print box labels | Print box labels for open print orders. |

### System

| Help Card | Subjects |
| --- | --- |
| Delete stock log | Delete stock log on the system. |
| Stock price correction | Correct average price for purchased stock articles. |

---

## Master data management

### Create a storeroom (SD 01-001)

**Objective of this activity**
Define a stock and all associated master data.

**Prerequisites**
None.

**Additional information**
The structuring of the stock master data using the stock must be defined carefully, since subsequent changes can only be made with great effort. If something is not clear, please be sure to contact A+W Software GmbH.

**Workflow**
1. Select menu `Master data > Location`. The `Storeroom administration` dialog opens.
2. Enter at least the following master data for the new stock:
    - Enter stock number.
    - Enter name and short designation for the stock.
    - Select site (at the company).
    - Select the inventory type.
    - Select the stock type.
3. Confirm definition with `[OK]`.

**Next step:** Define stock article.

### Define a stock article (SD 01-002)

**Objective of this activity**
Manage stock articles per stock.

**Prerequisites**
- Stock has been created in the master data.
- Article with variants is created with the procurement type Stock in the master data.

**Additional information**
- Create stock: `A+W Enterprise > STOCK > Master data > Room`.
- Create article: `A+W Enterprise > ALCIB > Master data > Article`.

**Workflow**
1. Select menu `Master data > Article`. The `Article master data stock` dialog appears.
2. Select the article and stock.
3. Select the article variant.
4. Enter the inventory limit for the order variant in the `Minimum`, `Alarm`, and `Maximum` columns.
5. Enter the inventory limits per article variant.
6. If necessary, make a remark per variant with `<F5>`.
7. Save definitions of the inventory limits with `<End>`.

---

## Stock management

### Book warehouse in (LA 01-001)

**Objective of this activity**
Book warehouse in articles.

**Prerequisites**
- Standard stock has been created in the master data.
- Article master data has been entered completely.
- Depending on the system configuration, the articles must be assigned to the selected company.

**Additional information**
- Use `<F5>` to change from a column to the variant-related details in the footer area.
- Use `<End>` to save the entries in the footer area and change to the rump area.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Warehouse in`. The `Warehouse in` dialog opens.
2. Select the article and stock.
3. Enter article variant, article quantity, and purchase price per piece or quantity unit. Total price of the article is displayed. Details about the article are displayed in the footer area.
4. Check the detail information in the footer area.
5. Repeat steps 3 and 4 for the next article variant.
6. Confirm the booking. Articles are booked into stock.

**Check booking:**
7. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
8. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
9. Menu `Infosystem > History > Enter filter criterion > <F3>`.
10. Display additional information with `<F2>` if necessary.
11. Open the detail view of the selected data record of the hit list with `<F5>`.
12. Check booking data.

### Book warehouse out (LA 01-002)

**Objective of this activity**
Book warehouse out articles.

**Prerequisites**
- Standard stock has been created in the master data.
- Article master data has been entered completely.
- Required quantity of articles is in stock.

**Additional information**
- Use `<F5>` to change from a column to the variant-related details in the footer area.
- Use `<End>` to save the entries in the footer area and change to the rump area.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Warehouse out`. The `Warehouse out` dialog opens.
2. Select the article and stock.
3. Enter the article variant and article quantity in pieces or quantity unit. Total price of the article is displayed. Details about the article are displayed in the footer area.
4. Check the detail information in the footer area.
5. Repeat steps 3 and 4 for the next article variant.
6. Confirm the booking. Articles are removed from the stock.

**Check booking:**
7. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
8. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
9. Menu `Infosystem > History > Enter filter criterion > <F3>`.
10. Display additional information with `<F2>` if necessary.
11. Open the detail view of the selected data record of the hit list with `<F5>`.
12. Check booking data.

### Book warehouse in in slot warehouse (LA 01-003)

**Objective of this activity**
Book warehouse in articles in slot warehouse.

**Prerequisites**
- Slot warehouse has been created in the master data.
- Article master data has been entered completely.
- Depending on the system configuration, the articles must be assigned to the selected company.

**Additional information**
- Use `<F5>` to change from a column to the variant-related details in the footer area.
- Use `<End>` to save the entries in the footer area and change to the rump area.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Slots in`. The `Warehouse in` dialog opens.
2. Select the article and stock.
3. Enter article variant, article quantity, and purchase price per piece or quantity unit. Total price of the article is displayed. Details about the article are displayed in the footer area.
4. Check the detail information in the footer area.
5. Repeat steps 3 and 4 for the next article variant.
6. Confirm the booking. Articles are booked into stock.

**Check booking:**
7. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
8. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
9. Menu `Infosystem > History > Enter filter criterion > <F3>`.
10. Display additional information with `<F2>` if necessary.
11. Open the detail view of the selected data record of the hit list with `<F5>`.
12. Check booking data.

### Book warehouse out in slot warehouse (LA 01-004)

**Objective of this activity**
Book warehouse out articles in slot warehouse.

**Prerequisites**
- Slot warehouse has been created in the master data.
- Article master data has been entered completely.
- Required quantity of articles is in stock.

**Additional information**
- Use `<F5>` to change from a column to the variant-related details in the footer area.
- Use `<End>` to save the entries in the footer area and change to the rump area.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Slots out`. The `Warehouse out` dialog opens.
2. Select the article and stock.
3. Enter the article variant and article quantity in pieces or quantity unit. Total price of the article is displayed. Details about the article are displayed in the footer area.
4. Check the detail information in the footer area.
5. Repeat steps 3 and 4 for the next article variant.
6. Confirm the booking. Articles are removed from the stock.

**Check booking:**
7. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
8. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
9. Menu `Infosystem > History > Enter filter criterion > <F3>`.
10. Display additional information with `<F2>` if necessary.
11. Open the detail view of the selected data record of the hit list with `<F5>`.
12. Check booking data.

### Book box warehouse in (LA 01-005)

**Objective of this activity**
Book a complete box in box warehouse in.

**Prerequisites**
- Box warehouse has been created in the master data.
- Article master data has been entered completely.
- Depending on the system configuration, the articles must be assigned to the selected company.

**Additional information**
- Use `<F5>` to change from a column to the box-related details in the footer area.
- Use `<Shift> + <F8>` to change from a column to the variant-related details in the footer area.
- Use `<End>` to save the entries in the footer area and change to the rump area.

**Workflow**
1. Select `Booking > Boxes in`. The `Box warehouse in` dialog opens.
2. Select the article and box warehouse.
3. Select the article variant.
4. Enter the box designation and packaging type.
5. Enter the article quantity and supplier's article price.
6. Repeat steps 3 and 5 for the next box.
7. Confirm booking with `[OK]`. Boxes are removed from the warehouse.

**Check booking:**
8. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
9. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
10. Menu `Infosystem > History > Enter filter criterion > <F3>`.
11. Display additional information with `<F2>` if necessary.
12. Open the detail view of the selected data record of the hit list with `<F5>`.
13. Check booking data.

### Book box warehouse out (LA 01-006)

**Objective of this activity**
Book a complete box in box warehouse out.

**Prerequisites**
- Box warehouse has been created in the master data.
- Article master data has been entered completely.
- Required quantity of articles is in stock.

**Additional information**
- Use `<F5>` to change from a column to the variant-related details in the footer area.
- Use `<End>` to save the entries in the footer area and change to the rump area.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Boxes out`. The `Box warehouse out` dialog opens.
2. Select the article and box warehouse.
3. Select box with appropriate article variant and press `<F4>`. Additional menu appears.
4. Select menu `Boxes > Box warehouse out`. The `Caution` dialog opens.
5. Confirm query whether the box should be removed from the stock with `[Yes]`.
6. Repeat steps 3 and 5 for the next box.
7. Confirm booking with `[OK]`. Boxes are removed from the warehouse.

**Check booking:**
8. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
9. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
10. Menu `Infosystem > History > Enter filter criterion > <F3>`.
11. Display additional information with `<F2>` if necessary.
12. Open the detail view of the selected data record of the hit list with `<F5>`.
13. Check booking data.

### Single sheet box warehouse in (LA 01-007)

**Objective of this activity**
Book single sheets in the single sheet box warehouse.

**Prerequisites**
- Single sheet box warehouse has been created in the master data.
- Article master data has been entered completely.
- Depending on the system configuration, the articles must be assigned to the selected company.

**Additional information**
- Use `<F5>` to change from a column to the variant-related details in the footer area.
- Use `<Ctrl> + <E>` to edit the single sheet information.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Boxes in`. The `Box warehouse in` dialog opens.
2. Select the article and single sheet box warehouse.
3. Select the article variant.
4. Enter the box designation. Cursor changes in the table for the entry of the single sheets to the `Sheet` column.
5. Enter data for single glass sheet.
6. Repeat step 5 until all glass sheets in the box are entered.
7. Enter variant completely.
8. Confirm booking with `[OK]`. Single sheets are booked into single sheet box warehouse.

**Check booking:**
9. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
10. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
11. Menu `Infosystem > History > Enter filter criterion > <F3>`.
12. Open the detail view of the selected data record of the hit list with `<F5>`.
13. Check booking data.

**Book additional glass sheets into existing single sheet box:**
14. Repeat 1 to 3.
15. Select box.
16. Use `<Ctrl> + <E>` to change to the table to enter the single sheets.
17. Use `<F6>` to create a new sheet number.
18. Repeat 5 to 13.

### Single sheet box warehouse out (LA 01-008)

**Objective of this activity**
Break up single sheet box and book glass sheets from the single sheet box to another stock.

**Prerequisites**
- Single sheet box warehouse has been created in the master data.
- Article master data has been entered completely.
- Required quantity of glass sheets is in stock.

**Additional information**
- Use `<F5>` to change from a column to the variant-related details in the footer area.
- Use `<Ctrl> + <E>` to edit the single sheet information.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Boxes out`. The `Box warehouse out` dialog opens.
2. Select the article and single sheet box warehouse.
3. Select variant.
4. Use `<Ctrl> + <E>` to edit the single sheet information.
5. Use `<F7>` to delete single articles. The selected sheet is deleted from the single sheet box. If the last remaining sheet of the single sheet box is deleted, the single sheet box is deleted automatically.
6. Make the booking with `[OK]`.

**Check booking:**
7. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
8. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
9. Menu `Infosystem > History > Enter filter criterion > <F3>`.
10. Display additional information with `<F2>` if necessary.
11. Open the detail view of the selected data record of the hit list with `<F5>`.
12. Check booking data.

### Book rack storage receipt (LA 01-009)

**Objective of this activity**
Book articles on racks in a rack warehouse.

**Prerequisites**
- Rack warehouse has been created in the master data.
- Article master data has been entered completely.
- Depending on the system configuration, the articles must be assigned to the selected company.
- Slots must be transferred as registration points from the production system to A+W Enterprise.

**Additional information**
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Rack receipt`. The `Rack storage receipt` dialog opens.
2. Select either the article and rack warehouse or the rack.
3. Select the article variant.
4. Select rack or create new rack.
5. Select slot for the rack.
6. Enter booking quantity of the variant in quantity unit.
7. Repeat steps 3 and 4 for additional article variants.
8. Confirm booking with `[OK]`. Articles are booked into the rack warehouse.

**Check booking:**
9. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
10. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
11. Menu `Infosystem > History > Enter filter criterion > <F3>`.
12. Display additional information with `<F2>` if necessary.
13. Open the detail view of the selected data record of the hit list with `<F5>`.
14. Check booking data.

### Rack storage exit (LA 01-010)

**Objective of this activity**
Book order-related stock removals in the rack warehouse.

**Prerequisites**
- Rack warehouse has been created in the master data.
- Article master data has been entered completely.
- Rack with the appropriate article variants is in stock.

**Additional information**
- Use `<F2>` to change between the `Order related` and `Transfer` tabs.
- Use `<Shift> + <F8>` to break up an article and book it to another stock.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Rack shipment`. The `Rack storage exit` dialog opens.
2. Select either article and rack warehouse or the rack.
3. Select the `Order related` tab.
4. Select variant on the rack.
5. Enter booking quantity of the variant in quantity unit.
6. Enter order number.
7. Enter item number in the order.
8. Repeat steps 4 to 7 for additional order-related bookings.
9. Confirm booking with `[OK]`. Articles are removed from the rack warehouse.

**Check booking:**
10. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
11. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
12. Menu `Infosystem > History > Enter filter criterion > <F3>`.
13. Display additional information with `<F2>` if necessary.
14. Open the detail view of the selected data record of the hit list with `<F5>`.
15. Check booking data.

### Transfer rack stock articles (LA 01-011)

**Objective of this activity**
Transfer article variants to a new rack or slot.

**Prerequisites**
- Rack stock has been created in the master data.
- Article master data has been entered completely.
- Rack with the appropriate article variants is in stock.

**Additional information**
- Use `<F2>` to change between the `Order related` and `Transfer` tabs.
- Use `<Shift> + <F8>` to break up an article and book it to another stock.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Rack shipment`. The `Rack storage exit` dialog opens.
2. Select either article and rack warehouse or the rack.
3. Select the `Transfer` tab.
4. Select variant on the rack.
5. Enter booking quantity of the variant in quantity unit.
6. Enter new rack.
7. Enter new slot.
8. Repeat steps 4 to 7 for additional transfers.
9. Confirm booking with `[OK]`. Articles are removed from the rack warehouse.

**Check booking:**
10. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
11. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
12. Menu `Infosystem > History > Enter filter criterion > <F3>`.
13. Display additional information with `<F2>` if necessary.
14. Open the detail view of the selected data record of the hit list with `<F5>`.
15. Check booking data.

### Book order-related outgoing stocks (LA 01-012)

**Objective of this activity**
Booking order-related stock removals manually.

**Prerequisites**
- Inventory change of the article in the article master data must be defined as manual booking.
- Stock has been created in the master data.
- Article master data has been entered completely.
- Required quantity of articles is in stock.

**Additional information**
- Use `<F2>` to display the column date for the delivery date of the article.
- Trigger the booking with `<F3>`.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Outgoing stocks (order-related)`. The `Outgoing stocks (order-related)` dialog opens.
2. Select order. Articles of the order are displayed.
3. Select article of the order to remove.
4. Enter quantity of the article.
5. Repeat steps 3 and 4 for additional order-related bookings.
6. Trigger booking with `<F3>`. Order-related articles are removed from the stock.

**Check booking:**
7. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
8. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
9. Menu `Infosystem > History > Enter filter criterion > <F3>`.
10. Display additional information with `<F2>` if necessary.
11. Open the detail view of the selected data record of the hit list with `<F5>`.
12. Check booking data.

### Stack warehouse in (LA 01-013)

**Objective of this activity**
Book a new stack in the warehouse in stack.

**Prerequisites**
- Stack warehouse has been created in the master data.
- Article master data has been entered completely.
- Depending on the system configuration, the articles must be assigned to the selected company.

**Additional information**
- Use `<Shift> + <F8>` to have the system assign a new stack number.
- Use `<Ctrl> + <F12>` to book in the selected stack.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**
1. Select `Booking > Stack in`. The `Stack warehouse in` dialog opens.
2. Select stack warehouse and supplier.
3. Create a new stack number with `<Shift> + <F8>`.
4. Enter article variant, article quantity, and purchase price per piece or quantity unit. Total price of the article is displayed. Details about the article are displayed in the footer area.
5. Repeat steps 3 and 4 for the next stack.
6. Confirm booking with `<End>`. Stacks are booked into the stack warehouse.

**Check booking:**
7. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
8. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
9. Menu `Infosystem > History > Enter filter criterion > <F3>`.
10. Display additional information with `<F2>` if necessary.
11. Open the detail view of the selected data record of the hit list with `<F5>`.
12. Check booking data.

### Modify stack warehouse (LA 01-014)

**Objective of this activity**
- Book articles to existing stacks.
- Break up a stack and book articles from the stack warehouse.

**Prerequisites**
- Stack warehouse has been created in the master data.
- Article master data has been entered completely.
- Warehouse in booking for selected article in stacks has already been made.

**Additional information**
- Use `<Ctrl> + <F8>` to break up the selected stack and book the article of the stack to another stock.
- Use `<Ctrl> + <F12>` to remove the selected stack.
- Bookings can be corrected on the `Booking correction` dialog. ⇨ `Make a booking correction`

**Workflow**

**Book articles to existing stacks.**
1. Select `Booking > Stack modification`. The `Modify stack warehouse` dialog opens.
2. Enter filter criteria. Existing stacks are displayed.
3. Select stack and enter new total quantity in the `Number` field.
4. Confirm booking with `<End>`. Stack is set to the quantity entered.

**Book articles from the stack stock:**
5. Repeat steps 1 to 2.
6. Select stack and enter quantity for the booking.
7. Use `<Ctrl> + <F8>` to show `Target stock` column.
8. Enter new stock for the stack.
9. Use `<Ctrl> + <F12>` to break up the stack.
10. Confirm query for stack removal with `[Yes]`. Articles from the stack will be booked into the target stock.

**Check booking:**
11. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
12. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
13. Menu `Infosystem > History > Enter filter criterion > <F3>`.
14. Display additional information with `<F2>` if necessary.
15. Open the detail view of the selected data record of the hit list with `<F5>`.
16. Check booking data.

### Make a booking correction (LA 01-015)

**Objective of this activity**
Correct bookings in the stock.

**Prerequisites**
- Stock data has been created by the stock booking system.

**Additional information**
- Use `<F5>` to change between the `Overview` and `Detail` view dialogs for the selected article.
- Enter a new date for the current booking record with `<Shift> + <F12>`.

**Workflow**
1. Select `Booking > Correction`. The `Correction` dialog opens.
2. Enter filter criteria. Hit list for the search is displayed.
3. Correct quantity/number and/or price in the columns.
4. Open the detail view of the selected data record with `<F5>`.
5. Confirm booking correction with `<End>`. Quantity/number and/or the price are corrected and booked.

**Check bookings:**
6. Menu `Infosystem > Booking status > Not booked`: Bookings not booked.
7. Menu `Infosystem > Booking status > Error`: Incorrect bookings.
8. Menu `Infosystem > History > Enter filter criterion > <F3>`.
9. Display additional information with `<F2>` if necessary.
10. Open the detail view of the selected data record of the hit list with `<F5>`.
11. Check booking data.

---

## Inventory management

### Take inventory of a stock (IV 01-001)

**Objective of this activity**
Take inventory of a stock.

**Prerequisites**
- The inventory of a stock can only be taken if since the last inventory there has been at least one outgoing booking or one incoming booking.

**Additional information**
- Inventories for the other stock types are taken in the same way on the following dialogs: `Inventory > Crate stock`, `Slot stock`, `Batch stock`, `Rack stock`.
- Stock numbers released for the inventory are marked by the system with a negative leading sign.
- An inventory is only possible for a stock (frm stock = to stock). If a value range is entered, the program branches into evaluation mode.

**Workflow**
1. Select `Inventory > Stock`. The `Inventory` dialog opens.
2. Select area limits for articles in: `frm Article`, `to Article`.
3. Select the same stock number of a stock for the stock number in both fields.
4. Confirm query for releasing of the inventory with `[Yes]`. Default stock is released for inventory.
5. Correct actual stock per article and article variant if necessary.
6. Complete inventory with `<Shift> + <F8>`. Inventory is completed.

**Check inventory for completion:**
7. Menu `Infosystem > Booking status > Inventory`. The `Booking status` dialog opens.
8. Stock numbers for open inventories are listed.

---

## Valuation

### Evaluation of stock (BW 01-001)

**Objective of this activity**
Undertake a valuation of article prices.

**Prerequisites**
- Selected stock may not be released for inventory.
- The evaluation of a stock can only be done if since the last evaluation there has been at least one outgoing booking or one incoming booking.

**Additional information**
- Evaluation for the other stock types is done in the same way on the following dialogs: `Evaluation > Crate stock`, `Slot stock`, `Batch stock`, `Rack stock`.
- An evaluation can only be made if the stock in question is released for inventory/evaluation. Stock numbers released for evaluation are marked by the system with a negative leading sign.

**Workflow**
1. Select `Evaluation > Stock`. The `Evaluation` dialog opens.
2. Select area limits for articles in: `frm Article`, `to Article`.
3. Select the same stock number of a stock for the stock number in both fields.
4. Confirm query for the evaluation with `[Yes]`. Article variants of the default stock are listed.
5. Correct the total price in the `Price` field if needed.
6. Complete evaluation with `<Shift> + <F8>`. Evaluation is completed.

---

## Info system

### View info about articles (IS 01-001)

**Objective of this activity**
View information about articles of the stock.

**Prerequisites**
- Stock data for the selected search criteria must be present in the system.

**Additional information**
Information about article variants, slots, racks, stacks, and single sheets are listed in the same way on the following dialogs: `Info system > Variant`, `Slot`, `Rack`, `Batch`, `Sheet`.

**Workflow**
1. Select menu `Info system > Article`. The `Info: stock products` dialog opens.
2. Enter one or several filter criteria and start the search with `<F3>`. Hit list is displayed.
3. Display additional information with `<F2>` if necessary.
4. Open the detail view of the selected data record of the hit list with `<F5>`. Detail view opens.

### View stock history (IS 01-002)

**Objective of this activity**
View information about bookings in the stock history.

**Prerequisites**
None.

**Additional information**
None.

**Workflow**
1. Select menu `Info system > History`. The `Info-stock-history` dialog opens.
2. Enter one or several filter criteria and start the search with `<F3>`. Hit list is displayed.
3. Open the detail view of the selected data record with `<F5>`. Detail view opens.

### View orders/purchase orders (IS 01-003)

**Objective of this activity**
View information about job and order-related bookings.

**Prerequisites**
- Orders/purchase orders contain stock articles.

**Additional information**
None.

**Workflow**
1. Select menu `Info system > Orders/Purchase orders`. The `Orders/Purch. orders` dialog opens.
2. Enter one or several filter criteria and start the search with `<F3>`. Hit list is displayed.
3. Open the detail view of the selected data record of the hit list with `<F5>`. Detail view opens.

### View booking status (IS 01-004)

**Objective of this activity**
- View and correct non-booked or incorrect bookings.
- Call up overview for all stocks in the inventory.

**Prerequisites**
None.

**Additional information**
Information about the booking status for incorrect data records and is listed in the same way on the following dialogs: `Info system > Booking status > Error`, `Inventory`.

**Workflow**
1. Menu `Info system > Booking status > Not booked`. `Booking status` dialog for unbooked data records opens.
2. Open the detail view of the selected data record with `<F5>`. Detail view is displayed.
3. Correct data.
4. Use `<Ctrl> + <F8>` after correcting the error cause to reset the error status.
5. Activate the stock booker with `<Shift> + <F8>`.
6. Save correction with `<End>`. Correction is saved and the dialog closed.

### View available stock (IS 01-005)

**Objective of this activity**
View ordered, planned, and available stock.

**Prerequisites**
None.

**Additional information**
None.

**Workflow**
1. Select `Info system > Available stock` menu. `Available stock` dialog opens.
2. Enter and confirm filter criteria in the header area. Overview of the stock is displayed.

### View stock forecast (IS 01-006)

**Objective of this activity**
View stock forecast for planned stocks of a time period.

**Prerequisites**
None.

**Additional information**
None.

**Workflow**
1. Select menu `Info system > Forecast`. The `Stock forecast` dialog opens.
2. Enter and confirm filter criteria in the header area. Overview of the stock forecast is displayed.
3. Use `<F5>` to display the order number or purchase order number of the selected data record.
4. Use `<Shift> + <F5>` to display the graphic of the course of inventory.

---

## Print

### Print box labels (DR 01-001)

**Objective of this activity**
Print box labels for open print orders.

**Prerequisites**
None.

**Additional information**
- A print order for label printing is created on the warehouse in automatically for each warehouse in.
- On the `Print labels for crates` dialog, in the column without a name, it is displayed whether or not the print order is released for label printing.

**Workflow**
1. Select `Print > Labels`. The `Print labels for crates` dialog opens.
2. If a box label should not be printed, you must use the `<Spacebar>` to switch the identifier in the `Column without a name` from Y to N.
3. Confirm label printing with `<Shift> + <F3>`. The labels are printed.

---

## System

### Delete stock log (SY 01-001)

**Objective of this activity**
Delete stock log on the system.

**Prerequisites**
None.

**Additional information**
After deleting the stock log, the appropriate records are no longer displayed under `Infosystem > History`.

**Workflow**
1. Select `System > Delete stock transcript`. The `Delete stock log` dialog opens.
2. Enter data for which the stock log should be deleted.
3. Delete stock lock with `<F3>`. Stock log is deleted.
