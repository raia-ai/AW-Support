---
title: "A+W Enterprise Sales and Purchasing User Manual"
source: "EN-UM-AWEnterprise_16.pdf"
tags: ["A+W Enterprise", "ERP", "Sales", "Purchasing", "Order Management", "Invoice", "Price Calculation", "Glass Manufacturing", "Windows and Doors", "User Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This user manual provides detailed instructions for using the A+W Enterprise Sales and Purchasing modules. It is structured as a series of 'Help Cards' that guide users through specific tasks, including order item management, price calculations, invoicing, and procurement processes. It covers functionalities from editing suppliers and handling complex product configurations like shaped or stepped glass, to managing financial documents and integrating with CAD systems."
long_description: "This comprehensive document serves as a user guide for the A+W Enterprise software, focusing on the Sales and Purchasing modules. It is designed to assist users in navigating and utilizing the system's extensive features for the glass, windows, and doors industry. The manual is organized into distinct sections, each addressing a core area of the software. The 'Order Item' section details procedures for creating and modifying order items, such as editing suppliers, exchanging glass types, inputting custom shapes, adding processing steps, and integrating with CAD (SN) files. It also covers specialized items like stepped glass and muntin structures. The 'Price Calculation' section explains how to manage and adjust pricing, including item conditions, article prices, discounts, and surcharges, as well as how to check production costs. The 'Invoice' section provides step-by-step workflows for creating, booking, printing, and sending invoices, both manually and automatically, including handling credit notes and configuring electronic invoicing. The 'A+W Enterprise Purchasing' module is covered in-depth, with its own detailed table of contents. It explains the entire procurement lifecycle, from creating purchase order proposals in the PO Pool, managing supplier inquiries, and entering purchase orders, to handling goods receipts, and processing supplier invoices. The manual's 'Help Card' format, complete with goals, requirements, and step-by-step workflow instructions, makes it a practical, task-oriented resource for both new and experienced users of the A+W Enterprise system."
---

## Order item

### Edit supplier (SA 03-002)

#### Goal of the action
- Change supplier.
- Change supply type.

#### Requirements
- Suppliers are created.
- Order entry is open.
- Item has been entered.

#### Additional Info
- With the specification of a supplier, the supply type is always changed to PO.
- With the change of the supply type to PO, a supplier must always be specified.

#### Workflow
1. Change to the **Items > General** tab.
2. **Quantity** field: press `<Shift>+<F12>`. The fields **Supplier** and **Deliv.time** are displayed next to the graphic.
3. **Supplier** field: enter supplier number or select with `<F9>`.
4. **Deliv.time** field: enter delivery time in days.
5. Continue with `<Enter>` and confirm the queries. The supplier can be taken over for the entire order, the following items or just for the current item.
6. Continue entry or save and close order.

**Change supply type:**
7. Enter item and enter suppliers.
8. **S.type** field: use the `<Spacebar>` to page to the supply type, e.g. PO.
9. Save item and continue entry.

### Exchange glass (SA 03-003)

#### Goal of the action
- Change glass in product structure.
- Change assembly position of glass.

#### Requirements
- Order entry is open.
- Item is entered with quantity and dimensions.

#### Additional Info
- Exchange glass can be entered in IG and LAMI lites.
- Assembly positions are counted from outside to inside.

#### Workflow
1. **Items > General > Enter IG item** tab, e.g. IG article.
2. Open BOM view dialog: **[BOM]**
3. **Curr. BOM level** tab: mark subelement > **[BOM]**. The current BOM level is marked in the BOM tree.
4. **Curr. BOM level** tab: change article number of the exchange glass.
5. Depending on the glass specify the following details:
   - **Strct** field: select direction of pattern.
   - **Supplier** field: select supplier.
   - **Print** field: select print option for production or sales papers.
6. Take over change with **[OK]**. The **Curr. BOM level** tab displays all subelements.

**Change assembly position:**
7. **AP** field: enter number of the assembly position of the exchange glass. The number of the second glass is changed automatically.

**Exchange pattern position:**
8. Open BOM for exchange glass
9. **AP** field: enter number of the assembly position of the glass.
10. Close **BOM view** dialogs with **[OK]**. The order entry dialog opens again.
11. Confirm query about price calculation.
12. Save changes.
13. Continue or save and close order.

### Shape input (SA 03-004)

#### Goal of the action
- Enter order item with shape.

#### Requirements
- Shape catalog is installed, e.g. the A+W shape catalog.
- Order entry is open.

#### Additional Info
- The dimensions of the circumscribing rectangle from the item entry are used for the price calculation.

#### Workflow
1. Change to the **Items > General** tab.
2. Enter article.
3. **Width** field: press `<Ctrl>+<F12>`. The **Shape** field is displayed next to the graphic.
4. Enter shape number or select with `<F2>`. The **Shape Dimensions** dialog opens.
5. Enter dimensions for all indicated lengths. Heed restriction, e.g. for W (width) and H (height).
6. Take over details with **[OK]**. The item is marked with the shape icon. The shape will be displayed to scale in the graphics area.
7. Save item.
8. Continue entry or save and close order.

### Enter processing step (SA 03-005)

#### Goal of the action
- Enter processing manually.

#### Requirements
- Order entry is open.
- Processing articles are created.

#### Additional info
- All processings are added in the same way.
- For asymmetrical cut-outs, enter each cut-out as a separate processing.
- For IG lite processing, e.g. screen printing, enter separately for each lite.
- Open BOM: in **Article** field, with `<Shift>+<F5>`; in **Quantity** field with `<F5>`.
- Adopt processing from SN file.

#### Workflow
1. **Items > General > Enter item** tab.
2. Open **BOM view** dialog: in **Quantity** field, press `<F5>`.
3. **BOM tree**: select level.
4. Insert new line: press `<F6>`.
5. Search for processing: **[A search]**.
6. Select processing, e.g. *Corner cut-out* and take over.
7. Enter dimension: **[Parameter]**.
8. Mark checkboxes for the corners, which should receive the same cut-out.
9. Specify values for corner cut-outs:
   - Distances A and B.
   - Reference edge, e.g. vertical.
   - Round-off for the cut-outs *Inner radius* and *Outer radius*.
10. Check details, correct if necessary, open product sketch with **[Sketch]**.
11. Take over values with **[OK]**. Product sketch closes.
12. If necessary, repeat the steps 3 to 11 for further processings.
13. Close processing with **[OK]**. The **Order entry** dialog opens.
14. Save item.
15. Continue entry or save and close order.

### Adopt processing from SN file (SA 03-006)

#### Goal of the action
- Take over processings from SN file in BOM.

#### Requirements
- A+W CAD Designer (Shapes) is installed.
- SN exchange rules are defined: **Master Data > Keys > Products > SN exchange rules**.
- SN files are available.
- Path is set up.

#### Additional info
- If no file is attached and saved, the BOM structure can only be changed if the entire action sequence is repeated.
- Add SN file.
- Synchronizing changes with SN file.

#### Workflow
1. **Sales > Order entry** menu > enter item.
2. Enter quantity, width, and height.
3. Press **Height** field: `<Ctrl>+<E>`. Windows Explorer opens in the predefined path.
4. Mark SN file in Windows Explorer and confirm with **[Open]**.
5. Confirm query for synchronization of the BOM with **[Yes]**. Program A+W CAD Designer (Shapes) opens.
6. In CAD Designer: check processings and change if necessary.
7. **File** menu: select **Close TOE**. Program A+W CAD Designer (Shapes) closes. The AWE BOM is compared to the CAD file. The processings are taken over. The SN file will not be attached.
8. Jump to the next field with `<Tab>`. The **Processings for item** dialog opens.
9. Check processings and close dialog with **[OK]**.
10. Save item.
11. Continue entry or save and close order.

### Add SN file (SA 03-007)

#### Goal of the action
- Take over processings from SN file in BOM.
- Attach copy of SN file.

#### Requirements
- A+W CAD Designer (Shapes) is installed.
- SN exchange rules are defined: **Master Data > Keys > Products > SN exchange rules**.
- SN files are available.
- Path is set up.

#### Additional info
- If no SN exchange rule for the processing included in the SN file is stored in A+W Enterprise, a selection dialog for the assignment opens. This assignment applies only to the current item.
- Synchronizing changes with SN file.

#### Workflow
1. **Sales > Order entry** menu > enter item.
2. Enter quantity, width, and height.
3. **Height** field: press `<Ctrl>+<E>`. Windows Explorer opens in the predefined path.
4. Mark SN file in Windows Explorer and confirm with **[Open]**.
5. Confirm query for synchronization of the BOM with **[Yes]**. Program A+W CAD Designer (Shapes) opens.
6. In CAD Designer: check processings and change if necessary.
7. Select **File** menu: **Exit TOE and save file**. Program A+W CAD Designer (Shapes) closes. The processings are taken over into the item's BOM. The SN file is updated.
8. Confirm queries and check notes.
9. Jump to the next field with `<Tab>`. The **Processings for item** dialog opens.
10. Check processings and close dialog with **[OK]**.
11. **Properties** tab: check path and name of the attached SN file. SN file is saved as copy in the TOE directory.
12. Save item.
13. Continue entry or save and close order.

### Synchronizing changes with SN file (SA 03-008)

#### Goal of the action
- Change or add processings in attached SN file.
- Change or add processings in BOM.

#### Requirements
- A+W CAD Designer (Shapes) is installed.
- SN exchange rules are defined: **Master Data > Keys > Products > SN exchange rules**.
- SN files are available.
- Path is set up.
- You know how to work with A+W CAD Designer (Shapes).

#### Additional info
- Complete description in the A+W CAD Designer (Shapes) manual.

#### Workflow
1. Select **Sales > Order entry > Item with SN file** menu.
2. **Width** field: press `<Ctrl>+<E>`.

**Changing processings in A+W CAD Designer (Shapes):**
Program A+W CAD Designer (Shapes) opens.
3. In CAD Designer: change processings, e.g. edgework.
4. Select **File** menu: **Exit TOE and save file**. Program A+W CAD Designer (Shapes) closes. The processings are taken over into the item's BOM. The SN file will be attached.

**Changing processings in the BOM:**
5. Mark item: select **[BOM]**. The **BOM view** dialog opens. A+W CAD Designer (Shapes) opens.
6. Change or add processings, e.g. speech hole.
   - See Help Card: Enter processing step.
7. Save change and close dialog. The processings are taken over into the item's BOM. The SN file is updated.
8. Save item.
9. Continue entry or save and close order.

### Enter item in CAD (SA 03-009)

#### Goal of the action
- Enter geometry and processings in A+W CAD Designer (Shapes), take over into item, and save as SN file.
- Interactive entry in A+W CAD Designer (Shapes).

#### Requirements
- A+W CAD Designer (Shapes) is installed.
- SN exchange rules are defined: **Master Data > Keys > Products > SN exchange rules**.
- Path is set up.
- You know how to work with A+W CAD Designer (Shapes).

#### Additional info
- Complete description in the A+W CAD Designer (Shapes) manual.

#### Workflow
1. **Sales > Order entry** menu > enter item with article number and quantity.
2. **Width** field: press `<Ctrl>+<F>`. A+W CAD Designer (Shapes) opens.
3. Draw CAD structure of the lite with dimensions and necessary processings.
4. Select **File** menu: **Exit TOE and save file**. Program A+W CAD Designer (Shapes) closes. The BOM is displayed in the item. SN file is saved in the TOE directory and attached. Changes are possible: see SA 03-008.
5. Save item.
6. Continue entry or save and close order.

### Enter stepped glass (SA 03-010)

#### Goal of the action
- Enter stepping on multiple lite.

#### Requirements
- Order entry is open.
- Item with type Step is created in the master data.
- For step on shape: shape is entered.

#### Additional Info
- Positive values for the steps are deducted from the edge length, negative values added.
- For steps on LAMI, there is a side view available in the product sketch.

#### Workflow
1. **Items > General > Enter item** tab. Example: specify step on IG lite.
2. Enter IG article.
3. **Width** field: press `<Ctrl>+<F10>`. **Stepped entry (relevant parts)** dialog opens.
4. Select glass for step: in the **S** field, assign stepping with Y and press `<F3>` and **[OK]**. The **Shape Dimensions** dialog opens.
5. Enter dimensions for height and width.
6. Enter dimensions for the steps per edge.
7. Take over dimensions with `<Enter>`.
8. For multiple IG: repeat steps 4 and 7 for the next glass.
9. Take over values from **Stepped entry (relevant parts)** dialog.
10. **PO** field: open BOM view with **[BOM]**. The **BOM view** dialog opens.
11. Change to the **Production sketch** tab and check entries.
12. If necessary, enter spacer and other details and save.
13. Continue entry or save and close order.

### Enter muntins (SA 03-011)

#### Goal of the action
- Enter muntin structure.

#### Requirements
- Muntin articles are created.
- Order entry is open.

#### Additional Info
- For complex muntin structure, attach sketch from A+W Design (Bars).
- Invoice
- Edit muntin structure

#### Workflow
1. Change to the **Items > General** tab.
2. Enter item completely with IG lite.
3. **AIR** field: check AIR and change if necessary.
4. **AIR** field: press `<Shift>+<F8>`. The **Muntin entry** dialog opens.
5. **Muntins** tab:
   - **Muntin** field: enter or select article number for muntin.
   - Fields **hz** and **ve**: enter number of horizontal and vertical muntins.
   - **Symmetry** field: select **F-sym** or **B-sym**.
   - **Color** field: select color variation if necessary.
   - **Supplier** field: select supplier if necessary.
6. **Additional Info** tab: change supply type if necessary.
7. For multiple IG:
   - **IR** field: select spacer for installation.
   - Repeat details for the next AIR (spacer).
8. Take over data with **[OK]**. The item is marked with the muntin icon. The muntin grid will be displayed to scale in the graphics area.
9. Continue entry or save and close order.

### Edit muntin structure (SA 03-012)

#### Goal of the action
- Edit muntin pattern with the muntin editor.
- Enter asymmetrical muntin structure.

#### Requirements
- Order entry is open.
- You are familiar with Help Card "Enter muntins."

#### Additional info
- Max. 11 muntins will be transferred to production.
- The prices are calculated for max. 2 different muntin articles.
- Attach complex muntin patterns, e.g. suns, as sketch from A+W Design (Bars).
- Invoice
- Enter muntins

#### Workflow
1. Change to the **Items > General** tab.
2. Enter item completely with IG lite.
3. **AIR** field: press `<Shift>+<F8>`. The **Muntin entry** dialog opens.
4. Enter the number of vertical and horizontal muntins.
5. **Symmetry** field: select **F-sym+E** or **B-sym+E**.
6. Open muntin editor: **[Editor]**.
7. Remove auxiliary muntin: click on the muntin pattern on the muntin.
8. Discard changes: restore original muntin pattern with **[Update]**.
9. Take over change with **[OK]**.

**Change muntin position:**
10. Edit light fields: press `<Shift>+<F8>` and enter value.
11. Edit drilling points:
    - Press `<Shift>+<F12>` and enter value.
    - Open table: press `<Shift>+<F11>` and edit values.
    - Take over changes with `<Enter>`.
12. Import muntin pattern with **[OK]**. Muntin editor closes. The item is marked with the muntin icon. The muntin pattern will be displayed in the graphics area.

### Edge clearance and sealing depth (SA 03-013)

#### Goal of the action
- Enter edge clearance and sealing depth on IG lites.

#### Requirements
- The module is configured in the system.

#### Additional info
- Dimensions for edge clearance and for sealing depth generally only deviate 1-2 mm from one another.

#### Workflow
1. **Items > General > Enter item** tab.
2. **Price** field: press `<F3>`. The **Dimensions of individual BOM elements** dialog opens.
3. BOM: mark **Inner frame** level and select **[Edge clearance]**. The **Edge clearance (frame thickness)** dialog opens.
4. Enter dimensions on all edges.
5. BOM: mark **Thiokol** level and select **[Sealing depth]**. The **Sealing depth** dialog opens.
6. Enter dimensions on all edges.
7. Take over details with `<Enter>`.
8. Confirm query for price calculation.
9. Save change with `<End>`. The **Dimensions of individual BOM elements** dialog opens. The item is displayed with the updated price.
10. Continue entry or save and close order.

### Replace product (SA 03-014)

#### Goal of the action
- Replace article in several order items.
- Edit lite structure in several order items.

#### Requirements
- Order entry is open.
- Several items with identical BOMs are entered.

#### Additional info
- For a product replacement, the processings for the lite must be re-entered.
- Product replacement for several items affects only items with the same BOM number.

#### Workflow
1. **Items > General** tab: select **<F4> > Product details > Product replacement**. The **Product replacement** dialog opens.
2. **Type** field: specify BOM number from the **SLNo** item column.
3. Specify replacement product.
4. Confirm replacement with **[Start]**.
5. Confirm queries. The items are displayed with the new article numbers and with a new BOM number.

**Editing lite structure:**
6. Step 2: **Replacement article** field: specify old article number.
7. **Desired construction** field: change one or several articles.
8. Confirm replacement with **[Start]**.
9. Confirm queries until query whether replacement should apply for all items.
10. Confirm **Does product replacement apply for all items...** query with **[No]**. The **Product replacement for items** opens.
11. **New** field: deselect all items with **N** in which the product should not be replaced.
12. Confirm replacement with **[Start]**. The dialog closes. The items are displayed with the old article numbers and with a new BOM number.

### Fix product (SA 03-015)

#### Goal of the action
- Fix article of order item.
- Take over fixed article into the master data.

#### Requirements
- Order entry is open.
- Order and item is entered.

#### Additional info
- The user right to write back a fixed item to the article master data must be granted.
- Fixed articles written back to the master data can be entered generally or customer-specifically as item according to the details.

#### Workflow
1. Change to the **Items > General** tab.
2. Enter item completely.
3. **Price** field: press `<Shift>+<F8>`.
4. Confirm the query with **[Yes]**. The item is marked with a yellow asterisk.
5. Enter additional items as necessary or mark for fixing.

**Take over fixed article into the master data:**
6. Save article with `<End>` and confirm query. The **Article details for dimensions variants** dialog is displayed for the first fixed item.
7. **Article (new)** field: enter new article number.
8. Check pre-populated fields and enter different information if necessary, e.g.:
   - Specify customer if the new article is a customer-specific product.
   - Specify customer-specific article number and name.
   - Specify prices.
9. Save details with `<End>`. The item is marked with a green asterisk.
10. If necessary, repeat steps 7 through 8 for each fixed item.
11. Save changes. The article is saved under the number entered in the article master data.

### Allocate declaration of performance (SA 03-016)

#### Goal of the action
- Check or allocate declaration of performance.

#### Requirements
- IG item is entered completely.

#### Additional Info
- All header data of the declaration of performance (DP) will be printed on the document.
- Create declaration of performance according to product structure:
- Enter technical values

#### Workflow
1. **Sales > Open document > Item** menu.

**Take over declaration of performance (DP) from master data:**
2. **Properties** tab > **DP number** field: press `<Ctrl>+<R>`. Code of the DP will be displayed in the **DP number** field.

**Change allocated DP:**
3. **Properties** tab > **DP number** field: press `<Ctrl>+<K>`. The **Declaration of performance** dialog opens.
4. Search for and select document.
5. Confirm allocation with **[OK]**.
6. Take over data with `<End>`. Code of the new DP will be displayed in the **DP number** field.
7. Auftrag speichern (Save order).

### Enter technical values (SA 03-017)

#### Goal of the action
- Enter technical values.
- Generate new declaration of performance.

#### Requirements
- IG item is entered completely.

#### Additional info
- All header data of the declaration of performance (DP) will be printed on the document.
- At least one checkbox of the services must be marked for output in order to generate a declaration of performance.
- A+W SLT interface for external calculation must be configured.

#### Workflow
1. **Sales > Open document > Item** menu.
2. **Properties** tab > **DP number** field: press `<Ctrl>+<T>`. The **Calculation of technical values** tab opens.
3. **Header data of the declaration of performance** area: enter header data of the declaration of performance.
4. **Declared services** tab: fill fields for the confirmed services. Fields with * can be filled via the A+W SLT interface.
5. Mark checkboxes for data that should be output.
6. If necessary, start determination of the technical services: press **[Ext.Calculation]** or `<F3>`.
7. Take over data with **[OK]**.

### Enter edge stripping (SA 03-018)

#### Goal of the action
- Enter edge stripping.

#### Requirements
- The module is configured in the system.
- Entry of edge stripping assumes that meta articles are maintained in the master data, that is, a processing with the BOM. These meta articles must be entered in the order.

#### Additional info
- The edge stripping cannot be entered via the A+W processing types.
- The same also applies for the processings Masking, Enamel strips, UV protection, etc.

#### Workflow
1. **Items > General > Enter item** tab.
2. **Height** field: press `<F5>`. The **BOM view** dialog opens.
3. BOM: press `<F6>` and select meta article for edge stripping. Article is added to the tab **Curr. BOM level**.
4. Mark article: press `<F5>`. The **Depth of the edge stripping** dialog opens.
5. Enter dimensions for the depth of the edge deletion and save with **[OK]**.
6. Save article and dimensions with **[OK]**. The **Processings for item x** dialog opens. The BOM is completed according to the master data.
7. Check details and enter comments if necessary.
8. Save details with **[OK]**. The **Processings for item x** dialog closes. The processings are displayed on the **Items** tab.
9. Confirm query for price calculation if necessary.
10. Save change with `<End>`. The item is displayed with the updated price.
11. Continue entry or save and close order.

## Price Calculation

This section covers topics related to price calculation.

| Help Card                      | Topics                                                                |
| ------------------------------ | --------------------------------------------------------------------- |
| Change item conditions         | Check and change item price.                                          |
| Change article prices          | Change article prices.                                                |
| Edit footer discount, surcharge | Check and/or change discounts and surcharges. Enter order-specific discount. |
| Check production costs         | Check production costs in the order. Check production costs in the quotation. |
| Price report for LAMI          | Check price calculation for LAMI item.                                |

### Change item conditions (SA 04-001)

#### Goal of the action
- Check and change item price.

#### Requirements
- Prices and conditions are created in the master data.

#### Additional info
- Changed conditions are not written back to the master data of the conditions.

#### Workflow
1. Change to the **Items > General** tab, e.g. in IG item.
2. Place the cursor in the **Price** field.
3. Click on the icon bar on icon **[%]**. The **Conditions** dialog (glass type) opens.
4. Change matrix allocation or base price.
5. Enter surcharges and discounts.
6. Take over with **[OK]**.
7. Confirm the query with **[Yes]**: Prices will be recalculated with manual changes.
8. Continue entry or save and close order.

### Change article prices (SA 04-002)

#### Goal of the action
- Change article prices.

#### Requirements
- N/A

#### Additional info
- All prices are changed the same way, e.g. replacement prices, muntin prices, subelement prices.

#### Workflow
1. Change to the **Items > General** tab.
2. Enter item(s).
3. `<F4> > Price information > Order prices > article prices` menu.
4. The **Order prices** dialog opens.
5. Select condition and article, e.g. **Customer** and a float glass.
6. Specify price and price type.
7. Take over change with `<End>`.
8. Confirm the query with **[Yes]**: Prices will be recalculated in all items in which the selected article is included.
9. Save order and close.

### Edit footer discount, surcharge (SA 04-003)

#### Goal of the action
- Check and/or change discounts and surcharges.
- Enter order-specific discount.

#### Requirements
- Discounts are created in the master data.

#### Additional info
- Discount types with negative leading signs are added as surcharges.
- The sequence number defines the sequence in which the surcharges and discounts are calculated.

#### Workflow
1. Change to the **Items > General** tab.
2. Enter items and save.
3. Change to the footer: press `<End>`.
4. **Discount** field: press `<F2>`. Dialog for discounts and surcharges opens.
5. **Discount** field, **Surcharge** field: enter values for surcharges and discounts.

**Enter order-specific discount:**
6. Insert new line: press `<F6>` and specify details:
   - **Name**.
   - **Sequence number**.
   - **Value** and **discount type**: plus (+) = surcharge, minus (-) = discount.
   - **Calculation type**, e.g. %.
   - **Calculation base**, e.g. product group = discount for all items in this product group.
7. Mark checkboxes:
   - Beginning of the line: calculate **yes/no**.
   - **Pos** field: redistribute **yes/no**.
8. Open detail view: press `<F5>` and add or correct data if necessary.
9. Take over change with **[OK]**.
10. Save discounts and take over into the order with `<End>`.
11. Save order and close.
12. Confirm the query about recalculation of the prices with **[Yes]**.

### Check production costs (SA 04-004)

#### Goal of the action
- Check production costs in the order.
- Check production costs in the quotation.

#### Requirements
- Material costs are created in the master data.
- Order must already be transmitted to production.
- Production transfer must be configured for quotations.

#### Additional info
- The personnel and machine costs are determined and reported back if the order was scheduled successfully in production.
- Quotations are only scheduled in A+W Production in preliminary fashion and deleted from the production batch after reporting of the costs.

#### Workflow
1. Enter and save order completely.
2. Confirm release for production with **[Yes]**. The order is placed in the A+W Production order pool.

**After scheduling in A+W Production:**
3. Open order.
4. Select item: press `<Shift>+<F10>` in **Price** field. The **Production cost calculation** dialog opens.
5. **Overview** tab: check calculated quantity and/or price.

**Check individual costs:**
6. Mark line in the overview and change to **Details** tab.
7. If necessary, repeat steps 4 to 6 for all items.

### Price report for LAMI (SA 04-005)

#### Goal of the action
- Check price calculation for LAMI item.

#### Requirements
- The report is not yet available for all price and condition calculations.

#### Additional info
- The price report can be saved in various formats.

#### Workflow
1. Change to the **Items > General** tab.
2. **Price** field: press `<Shift>+<F9>`. The **Conditions for PCd-LAMI** dialog opens.
3. Press `<Ctrl>+<L>`. The report opens in a text editor.
4. If necessary, save report and close text editor.
5. Close the **Conditions for PCd-LAMI** dialog.
6. Continue entry or close order.

## Invoice

This section covers topics related to invoices.

| Help Card                                   | Topics                                                                |
| ------------------------------------------- | --------------------------------------------------------------------- |
| Create invoice manually                     | Create and book invoice. Create partial invoice.                      |
| Create invoices automatically               | Create and book several invoices. Create collective invoice.          |
| Book invoice                                | Book invoice.                                                         |
| Print invoice                               | Print single document. Print several documents.                       |
| Send electronic invoice (e-invoicing)       | Send single invoices. Send several invoices.                          |
| Configure customers for electronic invoices | Configure customers for electronic invoices.                          |
| Enter a credit note                         | Enter a credit note. Enter complaint details.                         |

### Create invoice manually (SA 05-001)

#### Goal of the action
- Create and book invoice manually.
- Create partial invoice.

#### Requirements
- Orders must be released.

#### Additional info
- The system can be configured so that the invoice is created automatically together with the delivery note.
- Collective invoice:Create invoices automatically
- Print invoice

#### Workflow
1. Select **Sales > Invoices > Manual Invoice** menu.
2. Specify customer.
3. **Reference** field:
   - `<F9>`: search for and select order.
   - `<F8> > <F9> > Take over delivery note entry > <F9>`: search for and take over delivery note search.
4. Take over data from document search.
5. **Date** field: specify payment term.
6. Jump further and if necessary, fill out additional fields. Recalculation of the document dialog opens.
7. Select calculation if order should be recalculated.
8. Confirm using `<Enter>`. Order will be recalculated if necessary.
9. Take over change with **[OK]**.

**Create partial invoice:**
10. **Range** field: specify partial quantities.
11. Save changes with **[OK]**.
12. Check fields in footer, e.g. Discount.
13. Confirm query about booking with **[Yes]**.
    - **[Yes]**: The invoice is booked and transferred to the FinAc.
    - **[No]**: invoice is saved and must be booked manually later on.
    The final invoice number is set.
14. Confirm notice about the invoice number and additional queries as necessary.

### Create invoices automatically (SA 05-002)

#### Goal of the action
- Create and book several invoices.
- Create collective invoice.

#### Requirements
- Customer allows collective invoices.
- Orders must be released.

#### Additional info
- The system can be configured so that the invoice is created automatically together with the delivery note.
- Print invoice

#### Workflow
1. Select the **Sales > Invoices -> Automatic Release** menu. The **Invoices** dialog opens.
2. **Release** field: press `<Ctrl>+<F8>`. Dialog for import of the values opens.
3. Enter beginning and ending date for the document search.
4. Start import with **[OK]**. Orders are imported.
5. Repeat steps 2 and 4 as necessary.
6. Jump on and change document date if necessary.
7. Trigger invoice generation with `<F3>`.
8. Confirm queries as necessary.

**Create collective invoice:**
9. **Release** field: press `<Ctrl>+<F8>`. Dialog for specification of the customer number opens.
10. Enter customer number and take over. Orders are imported.
11. Trigger invoice generation with `<F3>`.

### Book invoice (SA 05-003)

#### Goal of the action
- Book invoice

#### Requirements
- Invoices must be created.

#### Additional info
- The system can be configured so that the invoice is printed and booked automatically together with the delivery note.

#### Workflow
1. Select **Sales > Invoices > Book Invoice** menu.
2. **Invoice** field: press `<Ctrl>+<F8>`. Dialog for import of the values opens.
3. Enter beginning and ending date for the document search.
4. Start import with **[OK]**.
5. Repeat steps 3 and 4 as necessary.
6. Mark **Bu** field.
7. Trigger booking with `<F3>`.
8. Confirm query about booking with **[Yes]**. The invoices are booked and transferred to the FinAc.

### Print invoice (SA 05-004)

#### Goal of the action
- Print single document.
- Print several documents.

#### Requirements
- Print management is set up.
- Customers' e-mail addresses are maintained.
- Customers' fax numbers are maintained.

#### Additional info
- Automatic dispatch: **Sales > Forms > E-Mail/Fax** menu
- All documents are printed the same way, e.g. order confirmations, delivery notes, collective invoices.

#### Workflow
1. **Sales > Forms > Print** menu. The **Form type** dialog opens.
2. Select form type and take over with `<End>`, e.g. Invoice. The **Print form** dialog opens.
3. Select pre-settings and take over with `<Enter>`, e.g.:
   - 1 additional copy
   - Specify various numbers.
4. Select document field with `<F9>` and take over.
5. Confirm invoice number(s) with **[OK]**. The **Print** dialog opens.
6. Select printer and start printing of the invoice with `<Enter>`.

**Print several invoices:**
7. Select pre-settings, e.g. Select numbers and take over with `<Enter>`.
8. Add order numbers, e.g. on individual orders from the previous day:
   - Enter employee number.
   - Restrict input date.
   - Select first and last document.
9. Read in order numbers from the restricting ranges with `<F3>`.
10. Select **Pr** field for print output Y or N.
11. Trigger printing with `<F3>`. The **Print** dialog opens.
12. Select printer and start printing of the invoices with `<Enter>`.

### Send electronic invoice (e-invoicing) (SA 05-004)

#### Goal of the action
- Send electronic invoice

#### Requirements
- Print management is set up.
- Customers' e-mail addresses are maintained.
- Electronic invoice creation is activated for the market partner.
- Electronic invoice was created during booking of the invoice.

#### Additional info
- Automatic dispatch: **Sales > Forms > E-Mail/Fax** menu
- All documents are printed the same way, e.g. order confirmations, delivery notes, collective invoices.

#### Workflow
1. Select the **Sales > Forms > Print** menu. The E-mail dialog opens.
2. Select form type **Invoice** and take over with `<End>`.
3. Select pre-settings and take over with `<Enter>`.
4. Select document field with `<F9>` and take over.
5. Confirm invoice number(s) with **Send**.

**Send several invoices:**
6. Select pre-settings and take over with `<Enter>`.

**Select numbers:**
7. Restrict invoice number:
   - Enter employee number.
   - Restrict input date.
   - Select first and last document.
8. Read in order numbers from the restricting ranges with `<F3>`.
9. Select **Pr** field for print output Y or N.
10. Select **RV** field for dispatch of the e-invoice Y or N.
11. Trigger sending with `<F3>`.

### Configure customers for electronic invoices (SA 05-005)

#### Goal of the action
- A customer should receive electronic invoices.

#### Requirements
- The customer exists in the system.
- The form type was allocated a recipient e-mail address.

#### Additional info
- If for order customers a FinAc debtor with deviating market partner number is stored, the entire master data configuration described for the FinAc debtor must be made.

#### Workflow
1. Select **Master Data > Market Partner** menu. The market partner dialog opens.
2. Select partner type **Customer** and take over with `<Enter>`.
3. Enter customer number and take over with `<Enter>`. The customer data is loaded.
4. The following master data must be maintained for the customer:
   - **Address** dialog of the e-mail address
   - **Identification** dialog the VAT ident no.
   - **Invoice** dialog
     - Select **E-invoice** field for creation of XRechnung
     - **Route ID** field: store route ID of the customer.
     - Select **Send type** field for dispatch type **E-invoice+PDF** or **E-invoice**.
5. Confirm definition with **[OK]**.

### Enter a credit note (SA 05-006)

#### Goal of the action
- Enter a credit note.
- Enter complaint details.

#### Requirements
- N/A

#### Additional info
- Credit note can be entered with reference to order, invoice, delivery note or credit note.
- Credit note can be entered without reference, e.g. from goodwill due to poor quality.
- Book credit note: **Sales > Credit notes > Book credit note** menu.

#### Workflow
1. Select **Sales > Credit Notes > Enter Credit Notes** menu. Credit notes dialog opens.
2. Select customer.
3. **Reference** field: press `<F9>`. The **Find Reference Document** dialog opens.
4. Select **Document** field with `<F9>` document type, e.g. Sales invoice.
5. Search for and take over document.
6. Check header data of the credit note.
7. **Items** tab:
   - Specify **Credit**: items quantities for credit.
   - or
   - **Price** field: specify prices for credit.
8. Confirm changes with **[OK]**. Dialogs for selection of Complaint type, Complaint location, etc. open.
9. If necessary, select details for the complaint.
10. Enter complaint data.
11. Confirm and take over details with `<Enter>`.
12. Confirm queries.
13. Save credit note.
14. Confirm query about booking with **[Yes]**.
    - **[Yes]**: The credit note is booked and transferred to the FinAc. The final credit note number is set.
    - **[No]**: credit note is saved and must be booked manually later on.

## Other topics

| Help Card        | Topics                                                                                                 |
| ---------------- | ------------------------------------------------------------------------------------------------------ |
| Search for document | Searching for orders from the current day. Searching for orders for a customer. Searching for date and/or user. |
| Document change  | Change route. Change delivery date. Set or delete cancellation status.                                   |

### Search for document (SA 06-001)

#### Goal of the action
- Searching for orders from the current day.
- Searching for orders for a customer.
- Searching for date and/or user.

#### Requirements
- N/A

#### Additional info
- All documents are searched for in the same way.

#### Workflow
1. Select **Sales > Order entry** menu.
2. Search for orders from the current day: press `<F8>`.
3. Mark and take over order.

**Search for orders starting with a particular order number:**
4. **Order** field: press `<F9>`. The **Find Orders** dialog opens.
5. **Orders starting with** field: enter start number.
6. Trigger search with `<F3>`.

**Searching for orders for a customer:**
7. **Order** field: press `<F9>`. The **Find Orders** dialog opens.
8. **Customer** field: enter customer number.
9. Trigger search with `<F3>`.

**Searching for date and/or user:**
10. **Order** field: press `<F9>`. The **Find Orders** dialog opens.
11. **Document Code** tab:
    - **User** field: enter user number.
    - **Entry date** field: enter date.
12. Trigger search with `<F3>`.
13. Take order over into hit list with double-click in the order entry.

### Document change (SA 06-002)

#### Goal of the action
- Change route.
- Change delivery date.
- Set or delete cancellation status.

#### Requirements
- Document is not locked.

#### Additional info
- Changes that are not forwarded to subsequent processes are marked with **Local change**. Orders with this code must, e.g. be transferred manually to dispatch.

#### Workflow
1. Select **Sales > Document Change** menu. Document change dialog opens.
2. **Document** field: select document type, e.g. Order.
3. **Number** field: press `<F9>`. The **Find Orders** dialog opens.
4. **Customer** field: enter customer number and start search. Hit list is displayed.
5. Take over order with double-click on the **Document Change** dialog.
6. Jump to the fields and change setting, e.g.:
   - **Local correct** field: enter free text.
   - **Std** field: set cancellation code.
   - **Route** field: change route.
   - **Date** field: change delivery date.
   - **Free** field: release changes.
7. Save changes with `<F3>`.

**Change to the document:**
8. Open document for processing with a double-click.
9. Check data and change if necessary.
10. Save changes with **[OK]**.

## A+W Enterprise Purchasing

### Revision overview of the module
- **02-2022**: Additions in software reference
- **08-2020**: Complete revision
- **06-2019**: Complete revision
- **01-2017**: Product and company names adjusted.
- **03-2014**: Complete revision
- **02-2007**: Original version

This module provides information on the following subjects:
- Software Reference

### Overview

In the Purchasing module, you manage the documents that are required for the successful processing of the purchasing business, such as purchase orders, inquiries, receipt of goods, and invoices.

In the Purchasing part, you will find the following topics:
- "Search Functions" on page E-1552
- "Document Management" on page E-1580
- "Purchase Order Pool" on page E-1566
- "Texts" on page E-1629
- "Receipt of Goods" on page E-1637
- "Invoices and Credit Notes" on page E-1664
- "Overviews" on page E-1680

#### The purchasing menu
Some of the available menu entries branch out to submenus. If these include more than three entries, they are listed separately according to the following overview. The displayed entries depend on the respective configuration.

- **PO pool configuration**
- **Configuration Order-Oriented PO Printing** - this configuration is not used. That's why it will not be described here.
- **Individual purchasing documents configuration**

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

> **Context menus**
> On the context menus (right mouse button), only the menu elements are offered that make sense in the context for the individual fields of the dialogs. You can also call up the functions on the context menus via the menus described. Generally, the menu elements on the context menu correspond to the functions offered on the prompt display.

You can reach all dialogs and functions relating to sales via the **Purchasing** menu.

#### PO pool configuration
The purchasing configuration PO pool includes the most-used settings. The explanations, examples, and other notes in this document are based, insofar as nothing else explicit is mentioned, on this configuration.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Create P.O.s | "Creating purchase orders" on page E-1569 |
| b | Inquiries | "Supplier inquiries" on page E-1583 |
| c | PO management | "Purchase order entry" on page E-1584 |
| d | Form | |
| d a | - Print | Sales, "Form printing" on page D-1419 |
| d b | - E-Mail/Fax | Sales, "E-mail" on page D-1423 |
| e | List printing | Sales, "List printing" on page D-1427 |
| f | P.O. release | "Purchase Order Release" on page E-1631 |
| g | Dispatch notifications | "Dispatch notifications" on page E-1637 |
| h | Receipt of goods | "Receipt of goods submenu" on page E-1543 |
| i | Invoices | "Invoices submenu" on page E-1543 |
| j | Credit notes | |
| j a | - Enter credit notes | "Supplier's credit note" on page E-1678 |
| j b | - Book credit notes | Sales, "Book credit notes" on page D-1416 |
| k | Overview | "Overview submenu" on page E-1544 |
| l | Search | "Purchase search" on page E-1682 |

#### Individual purchasing documents configuration

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Generate stock order | "Creating purchase orders" on page E-1569 |
| b | Enter and edit inquiries | "Supplier inquiries" on page E-1583 |
| c | Enter and edit purchase orders | "Purchase order entry" on page E-1584 |
| e | Manage form printing | Sales, "Form printing" on page D-1419 |
| e | Manage list printing | Sales, "List printing" on page D-1427 |
| f | Release and manage several POs | "Purchase Order Release" on page E-1631 |
| g | Release and manage individual POs | "Purchase Order Release" on page E-1631 |
| h | Enter and manage delivery confirmations | "Dispatch notifications" on page E-1637 |
| i | Manage receipt of goods | "Receipt of goods submenu" on page E-1543 |
| j | Enter and edit invoices | "Invoices submenu" on page E-1543 |
| k a | - Enter supplier credit notes | "Supplier's credit note" on page E-1678 |
| k b | - Book credit notes | Sales, "Book credit notes" on page D-1416 |
| l | Display document overviews | "Overview submenu" on page E-1544 |
| m | Search documents in purchasing | "Purchase search" on page E-1682 |

#### Receipt of goods submenu
**Purchase > Goods Receipt**
Use this menu to access the dialogs on which you manage the receipt of goods.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| h a | Delivery plan | "Delivery plan" on page E-1646 |
| h b | Automatic receipt of goods | "Receipt of goods (automatic)" on page E-1649 |
| h c | Manual receipt of goods | "Receipt of goods (manual)" on page E-1654 |
| h d | Rack-related receipt of goods | "Rack-related receipt of goods" on page E-1656 |
| h e | Close purchase orders | "Receipt of Goods" on page E-1637 |
| h f | Check receipt of goods | "Check receipt of goods" on page E-1660 |
| h g | Missing quantities check pool | "Missing quantities check pool" on page E-1661 |
| h h | Log | "Invoice log" on page E-1678 |

#### Invoices submenu
**Purchase > Invoices**
Use this menu to access the dialogs on which you manage purchase invoices.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| i a | Invoice check | "Invoice check" on page E-1664 |
| i b | Automatic invoices | "Supplier's invoice (automatic)" on page E-1671 |
| i c | Invoices transferred | "Transferred invoices" on page E-1673 |
| i d | Manual invoices | "Supplier's invoice (manual)" on page E-1674 |
| i e | Collective invoices | "Supplier's invoice (collective invoice)" on page E-1675 |
| i f | Booking of invoices | "Booking of invoices" on page E-1676 |
| i g | Close purchase orders | "Receipt of Goods" on page E-1637 |
| i h | Log | "Invoice log" on page E-1678 |

#### Overview submenu
**Purchase > Overview**
Use this menu to access the dialogs on which you can display overviews of the various documents.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| k a | Receipt of goods today | "These overviews depend on the configuration and must be released separately. These dialogs can be designed customer-specifically if necessary. Please contact a service employee of A+W Software GmbH." on page E-1681 |
| k b | Delayed receipt of goods | "Overview of documents" on page E-1681 |
| k c | Scheduled receipt of goods from - to | "Overview of documents" on page E-1681 |
| k d | Delivered - but not invoiced | "Overview of documents" on page E-1681 |
| k e | Invoiced - but not booked | "Overview of documents" on page E-1681 |
| k f | Purchase orders not transferred yet: | "Overview of documents" on page E-1681 |
| k g | Search document | Sales, "Search document" on page D-1447 |
| k h | Purchase information | "Document information" on page E-1680 |

#### Supplementary menu
The supplementary menu can be called up with `<F4>` for entering various documents, e.g. for a purchase order. The entries on the supplementary menu are displayed in context-dependent versions.
- Supplementary menu for the header and footer area
- Supplementary menu for the item area

##### Supplementary menu for the header and footer area

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Text | |
| a a | - Header text | Sales, "Header and footer texts" on page D-1308 |
| a b | - Footer text | Sales, "Header and footer texts" on page D-1308 |
| a c | - External information | Sales, "External information" on page D-1316 |
| b | Addresses | |
| b a | - Find delivery addresses | Sales, "Find addresses" on page D-1095 |
| b b | - New shipping address | Sales, "New delivery address" on page D-1191 |
| b c | - Delete delivery address | Deletes the delivery address from the document. |
| b d | - Pick-up address | "Pick-up address" on page E-1625 |
| c | Cancel | "P.O. type" on page E-1627 |
| d | Prices | "Prices submenu" on page E-1546 |
| e | Product details | |
| e a | - Product exchange | "P.O. type" on page E-1627 |
| e b | - E/A rules | "Exchange/additional rules" on page B-151 |
| f | Resubmission | Sales, "Resubmission" on page D-1467 |
| g | Configurable fields | Sales, "Configurable fields" on page D-1199 |

##### Supplementary menu for the item area

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Texts | |
| a a | - Header text | Sales, "Header and footer texts" on page D-1308 |
| a b | - Footer text | Sales, "Header and footer texts" on page D-1308 |
| a c | - External information | Sales, "External information" on page D-1316 |
| a d | - Article text | Sales, "Article and item texts" on page D-1311 |
| a e | - Item text | Sales, "Article and item texts" on page D-1311 |
| a f | - Special texts | "Prices submenu" on page E-1546 |
| b | Addresses | |
| b a | - Find delivery addresses | Sales, "Find addresses" on page D-1095 |
| b b | - New shipping address | Sales, "New delivery address" on page D-1191 |
| b c | - Delete delivery address | Deletes the delivery address from the document. |
| b d | - End customer address | Sales, "End customer address" on page D-1193 |
| c | Cancel | "P.O. type" on page E-1627 |
| d | Private fields | Sales, "Private fields" on page D-1218 |
| e | Prices | "Prices submenu" on page E-1546 |
| f | Product details | "Product details submenu" on page E-1547 |
| g | Resubmission | Sales, "Resubmission" on page D-1467 |
| h | Reference | |
| h a | - New reference | "Purchase order items - general" on page E-1604 |
| h b | - Change reference | "Purchase order items - general" on page E-1604 |
| i | Delivery Plan | Sales, "Delivery plan" on page D-1385 |
| j | Warehouse | |
| j a | - Stack | "Purchase order items - general" on page E-1604 |
| j b | - Stock forecast | Sales, "Stock forecast" on page D-1204 |
| h | Configurable fields | Sales, "Configurable fields" on page D-1199 |

#### Prices submenu
**<F4> > Price info**
Use this menu to manage the prices and conditions for the article of the marked item.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Order conditions | Sales, "Conditions for PCD processing" on page D-1338 |
| b | Order prices | "Order prices submenu" on page E-1547 |
| c | Partial calculation | Sales, "Production cost calculation" on page D-1371 |
| d | Item conditions | Sales, "Conditions for PCD processing" on page D-1338 |
| e | Load conditions | Determine the sales price with the item conditions and recalculate the price. |
| f | Price calculation | Recalculate the item price. |
| g | Price check | "Purchase order items - general" on page E-1604 |

*The entries `d`, `e`, `f`, and `g` are only displayed in the item area.*

#### Order prices submenu
**<F4> > Price Info> Order Prices**
Use this menu to manage the order prices.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Article prices | Sales, "Order prices" on page D-1325 |
| b | Muntin prices | Sales, "Order muntin prices" on page D-1327 |
| c | Exchange prices | Sales, "Order exchange prices" on page D-1330 |
| d | Sub-element prices | Sales, "Order sub-part prices" on page D-1332 |

#### Special texts submenu
**<F4> > Texts > Special Texts**
Use this menu to manage all special texts that you can assign to the document. These texts can generally be configured customer-specifically and are therefore not part of this documentation. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

#### Product details submenu
**<F4> > Product Details**
Use this menu to manage the details for the products, e.g. exchange and additional rules.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Product exchange | "P.O. type" on page E-1627 |
| b | E/A rules | Master Data, "Exchange/additional rules" on page B-304 |
| c | Product group | "Purchase order items - general" on page E-1604 |
| d | Technical values | "Technical values submenu" on page E-1548 |

*The entries `c` and `d` are only displayed in the item area.*

#### Technical values submenu
**<F4> > Product Details > Technical Values**
Use this menu to manage the technical values.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Show technical details | Show the technical values. |
| b | Change technical values | Switches to the technical values so that they can be edited. The cursor changes to the db value field of the technical values on the Items tab. |
| c | Declaration of performance | Sales, "Texts" on page E-1629 |
| d | Show hidden dimensions | Shows the hidden dimensions on the Items tab. |
| e | Change hidden dimensions | Sales, "Article dimensions" on page D-1203 |

#### Info menu
**<Shift> + <F4>**
The info menu is displayed in context-dependent forms:
- Info menu for the header and footer area
- Info menu for the item area

##### Info menu for the header and footer area

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Document notes | Sales, "Notes" on page D-1300 |
| b | Market partner notes | |
| c | Project notes | |
| d | Search document | Sales, "Search document" on page D-1447 |
| e | Document overview | Sales, "Overview" on page D-1200 |
| f | Market partner information | Sales, "Market partner info" on page D-1195 |
| g | Change log | Sales, "Amendment log" on page D-1228 |
| h | Delivery plan | "Delivery plan" on page E-1646 |
| i | Delivery date changes | Sales, "Delivery date change log" on page D-1230 |
| j | Receipt of goods today | "These overviews depend on the configuration and must be released separately. These dialogs can be designed customer-specifically if necessary. Please contact a service employee of A+W Software GmbH." on page E-1681 |
| k | Delayed receipt of goods | "Overview of documents" on page E-1681 |
| l | Scheduled receipt of goods from – to | "Overview of documents" on page E-1681 |
| m | Delivered - but not invoiced | "Overview of documents" on page E-1681 |
| n | Invoiced - but not booked | "Overview of documents" on page E-1681 |
| o | Rack management | "Booking racks" on page E-1652 |
| p | Delivery date | Displays the following information from the customer order for order-related POs: Order number, Delivery date, Route |
| r | Purchase information | "Document information" on page E-1680 |

##### Info menu for the item area

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Notes | Notes submenu |
| b | Search document | Sales, "Search document" on page D-1447 |
| c | Document overview | Sales, "Overview" on page D-1200 |
| d | Market partner information | Sales, "Market partner info" on page D-1195 |
| e | Change log | Sales, "Amendment log" on page D-1228 |
| f | Delivery plan | "Delivery plan" on page E-1646 |
| g | Rack management | "Booking racks" on page E-1652 |
| h | Note | "Purchase order items - general" on page E-1604 |
| i | Delivery date | Displays the following information from the customer order for order-related POs: Order number, Delivery date, Route |
| j | Purchase information | "Document information" on page E-1680 |

##### Notes submenu
**<Shift> + <F4> > Notes**
The Notes info menu is only displayed on the PO Management – Items tab. In the PO header, you open the existing Notes directly via the info menu `<Shift> + <F4>`.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Document notes | Sales, "Notes" on page D-1300 |
| b | Supplier notes | |
| c | Supplier article notes | |
| d | Project notes | |
| e | Project article notes | |
| f | Customer notes | |
| g | Customer article notes | |

#### Goods receipt supplementary menu
On the dialogs with automatic data processing, such as Receipt of goods, Supplier invoice, Close POs, you can use `<F4>` to call up the dialog-specific additional menu. The entries displayed are optional depending on the dialog from which the menu was called. The following overview of the menus always lists all entries.

> **Context menus**
> On the context menus for the individual fields of the dialog, only the menu elements are offered that make sense in the context. The functions correspond to the functions that you call up via the menus described below.

##### Receipt of goods supplementary menu
**Purchase > Receipt of Good > Automatic Receipt of Goods> <F4>**

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Tag (downwards) (Shift+F9) | Enables the Cr. (Create) checkboxes for the selected and all following POs. |
| b | Tag (all) (Ctrl+F9) | Enables the Cr. (Create) checkbox for all POS. |
| c | Import values (Ctrl+F8) | Opens a dialog for specifying a time period and imports all non-booked POs with a delivery date within the specified time period. The hit list also displays future deliveries. |
| d | Supplier evaluation (Ctrl+N) | At present, this menu entry is not supported. |
| e | Check receipt of goods (Shift+F10) | After the successful check of the receipt of goods, it is possible to enable the Chk. checkbox by calling this menu element or using the key combination. |
| f | Status check from current record (Shift+F11) | Enables the Chk. (Check) checkboxes for the selected and all subsequent POs. |
| g | Status check all records (Ctrl+F11) | Enables the Chk. (Check) checkbox for all POs. |
| h | Rack management (Ctrl+G) | Opens the dialog Book racks. "Rack-related receipt of goods" on page E-1656 |
| i | Note (Ctrl+B) | Displays the Note column in which you can specify additional information about the PO. |

### Search Functions
In the Purchase module, you can search via various categories for documents, market partners, addresses, articles, and projects.
The search dialogs are structured the same way for all document types in Purchasing. Operation of the search dialogs has been developed analog to purchasing. In these instructions, the search functions are described using the example of POs. Deviations from other dialogs and from Sales are mentioned explicitly.

The following dialogs are described in this section:
- "Find purchase orders" on page E-1552
- "Find purchase orders - hit list" on page E-1558

Additional search dialogs are the same in Purchasing and Sales. They are described in detail in the Sales section:
- Sales, "Find deference document" on page D-1093
- Sales, "Find market partner" on page D-1087
- Sales, "Find addresses" on page D-1095
- Sales, "Find article" on page D-1097
- Sales, "Find article by types" on page D-1107
- Sales, "Find product by element" on page D-1108
- Sales, "Find project" on page D-1115

#### Find purchase orders
**Purchase > Inquiries > <F9> > Enter Search Criteria > <F3>**
Use this dialog to find purchase orders. Specify the search criteria in the header area. The hits for the search are displayed on the tabs.
- Use `<F2>` to change to the header area of the tab.
- Use `<F3>` to start the search.
- Use `<F2>` to change tabs on the hit list.

This dialog contains the following tabs in the header area:
- "Find purchase orders - document key" on page E-1553
- "Find purchase orders – item code" on page E-1555
- "Find purchase orders - direct search" on page E-1557

The search results are shown in the hit list:
- "Find purchase orders – hit list" on page E-1558

##### Find purchase orders – document key
**Purchase > Inquiries, P.O. Management> <F9>**
You can search for purchase orders on this tab using delivery data.
- Use `<F2>` to change to the header area of the tab.
- Use `<F3>` to start the search.

**Document key**
- **P.O. From**: Number starting from which purchase orders are searched for. The field name varies depending on the dialog from which you open the search, e.g. Inquiries from. Technical info: numeric field, DB field: kauf.auftrnr
- **Supplier**: Supplier number. If you specify a number, the supplier name is displayed in plain text. Technical info: numeric field, display field, DB fields: kauf.kunr
- **Ext. No.**: External number of the document. A number or a free text can be an external number. Depending on the configuration, the field Ext.No. may be pre-populated by the system. This data is described for the PO entry dialog: "Cust. order" on page E-1587. If the field includes alphanumeric characters, then capitalization must be heeded for the search. However, using an environment variable, you can enable the search for alphanumeric characters regardless of capitalization. Technical info: alphanumeric field, DB field: kauf.exaufnr
- **Input date**: Date when the purchase order was released. Technical info: date field, DB field: kauf.bdat
- **Site number**: Number of site. By default, the own site number is selected. The field can only be edited if you ware working with internal site separation. Technical info: numeric field, DB field: xhaus.haus
- **Customer**: Customer number. If you specify a number, the customer name is displayed in plain text. Technical info: numeric field, display field, DB field: kauf.orgkunr, kauf.orgname
- **Input date**: Date of document entry. Technical info: date field, DB field: kauf.edat
- **Entered by**: Employee number of the person who entered the document. If you specify a number, the name of the employee is displayed in plain text. Technical info: numeric field, DB field: kauf.eusr
- **Invoice no.**: Number of the supplier invoice. Technical info: numeric field, DB field: kauf.rechnr
- **VAT ID no.**: Supplier's VAT ID number. Technical info: alphanumeric field, DB field: kaufp.steuernr

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
- "Find purchase orders - hit list" on page E-1558

##### Find purchase orders – item code
**Purchase > P.O. Management> <F9> > Tab Item Code**
You can search for purchase orders on this tab using item codes.
- Use `<F2>` to change to the header area of the tab.
- Use `<F3>` to start the search.

**Item key**
You can search for the POs using the data from the items. For this search, enter the values you know. The following fields are available for entry:
- **Suppl. OC**: Number of order confirmation from supplier. Technical info: numerical field, DB field: bpos.abnr
- **DN No.**: Delivery note number of supplier. Technical info: numerical field, DB field: bpos.lieferschein
- **Remark**: Text field for an item-related remark that you can enter in the dialog **Supplier inquiries > P.O. info tab > Remark** field related to the item. Technical info: alpha-numerical field, DB field: bpos.bemerkung
- **Order no.**: Order number for order-related purchase orders. Technical info: numerical field, DB field: bpos.vksuftrnr
- **Delivery date**: Planned delivery date starting on which POs will be searched for. Technical info: Date field, DB field: bpos.ltplan
- **Project**: Project number. If you specify a number, the project name is displayed in plain text. Technical info: numeric field, display field, DB field: bpos.vkobjnr
- **Article**: Article number. If you specify a number, the article name is displayed in plain text. Technical info: numeric field, DB field: kpos.artnr
- **QU**: Quantity unit for the item, e.g. square meter. Technical info: numeric field, DB field: kpos.me
- **Stock**: Stock number for the purchase order. If you specify a number, the warehouse name is displayed in plain text. Technical info: numeric field, DB field: bpos.Inr
- **Dim. variant**: Dimensional variant of the article. Technical info: numeric field, DB field: kpos.var

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
- "Find purchase orders - hit list" on page E-1558

##### Find purchase orders – direct search
**Purchase > P.O. Management> <F9> > Tab Direct Search**
On this tab, you search for POs starting from a particular PO number. Thanks to a system configuration, it is possible to configure this tab as start dialog to use a simple search.
- Use `<F2>` to change to the header area of the tab.
- Use `<F3>` to start the search.

- **P.O. From**: Number starting from which purchase orders are searched for. The field description varies depending on the dialog from which you open the search, e.g. Inquiries from. Technical info: numeric field, DB field: kauf.auftrnr

**Hit list**
The hit list displays the result of the search. It is structured the same way for all tabs in the header area:
- "Find purchase orders - hit list" on page E-1558

#### Find purchase orders – hit list
**Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3>**
The hit list contains the following tabs:
- "Hit list - general" on page E-1559
- "Hit list - quantities" on page E-1561
- "Hit list - GR info" on page E-1562
- "Hit list - article" on page E-1563
- "Hit list - miscellaneous tab" on page E-1564

##### Hit list – general
**Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3> > General Tab**
This tab displays general information about the purchase orders that fits the search criteria. Use `<F2>` to change tabs on the hit list.

> **Show record**
> At the right top of the dialog frame, the record display is offered: e. g.: Document overview: 137:227.
> 137 = the record number of the selected line in the hit list
> 227 = the number of records in the hit list.

**Header**
The fields in the header area are described for the **Find Purchase Orders** dialog:
- "Find purchase orders" on page E-1552

**General tab**
- **Site:** Site number of the respective purchase order. Technical info: display field, DB field: kauf.hausnr
- **P-Order No.:** Purchase order number. The column name varies depending on the dialog from which you open the search. Technical info: display field, DB field: kauf.auftrnr
- **SubNo:** Number of the partial delivery note or partial invoice. Technical info: display field, DB field: kauf.subnr
- **Supplier:** Name of the supplier. Technical info: display field, DB field: mp.name
- **VAT ID No..:** Supplier's VAT ID number. Technical info: display field, DB field: kaufp.steuernr
- **Invoice:** Number of the supplier invoice. Technical info: display field, DB field: kauf.rechnr
- **Ordered:** Date when the purchase order was released. Technical info: display field, DB field: kauf.bdat
- **Entered:** Date of the purchase order entry. Technical info: display field, DB field: kauf.edat
- **Operator:** Name of the person who entered this order. Technical info: display field, DB field: kauf.eusr
- **Cancelled:** Specification of the processing state, e.g. cancellation status.
  - 0: Order not cancelled.
  - 1: Order cancelled by the operator.
  - 2: Order cancelled by the system.
  - -3, -10, ..., -x: Order in background processing.
  Technical info: display field, DB field: kauf.still

##### Hit list - quantities
**Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3> > Quantities Tab**
This tab displays item information about the ordered articles and the quantities that fit the search criteria. One line is displayed per article order item. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Purchase Orders** dialog:
- "Find purchase orders" on page E-1552

**Quantities tab**
The columns are described for the General tab:
- "General tab" on page E-1559
In addition, the following columns are displayed:
- **Itm:** Item number in the purchase order. Technical info: display field, DB field: kpos.posnr
- **ArtNo, Article:** Article number and article name. Technical info: display fields, DB fields: kpos.artnr, kpos.artbez1
- **Qty:** Ordered quantity of the item. Technical info: display field, DB field: kpos.menge
- **Receipt:** Quantity received in receipt of goods. Technical info: display field, DB field: kpos.geslief
- **Compl.:** An asterisk * indicates if the item has been delivered completely. Technical info: display field
- **Invcd:** Invoiced quantity of the item. Technical info: display field, DB field: kpos.gesberech
- **C:** An C indicates if the item has been invoiced completely. Technical info: display field
- **Width, Height:** Sizes of the item in millimeters. Technical info: display fields: DB fields: kpos.laenge, kpos.breite

##### Hit list - GR info
**Purchase > P.O. Management> <F9> > Enter Search Criteria > <F3> > Tab GR Info**
This tab displays receipt of goods information about the purchase orders. One line is displayed per purchase order item. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Purchase Orders** dialog:
- "Find purchase orders" on page E-1552

**GR info tab**
The columns are described for the General and Quantities tab:
- "Hit list - general" on page E-1559
- "Hit list - quantities" on page E-1561
In addition, the following columns are displayed:
- **Deliv.date:** Planned date of delivery starting on which POs will be searched for. Technical info: display field, DB field: bpos.ltplan
- **OC no.suppl.:** Number of order confirmation from supplier. Technical info: display field, DB field: bpos.abnr
- **Deliv.note:** Delivery note number of supplier. Technical info: display field, DB field: bpos.lieferschein
- **Order:** Order number for order-related purchase orders. Technical info: display field, DB field: bpos.vksuftrnr
- **Delivery:** Planned delivery date of the customer order. Technical info: display field, DB field: bpos.ltplan

##### Hit list – article
**Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3> > Article Tab**
This tab displays information about the article properties of the PO items. One line per PO item is displayed. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Purchase Orders** dialog:
- "Find purchase orders" on page E-1552

**Article tab**
The columns are described for the **General** and **Quantities** tab:
- "Hit list - general" on page E-1559
- "Hit list - quantities" on page E-1561
In addition, the following columns are displayed:
- **QU:** Quantity unit for the item, e.g. square meter. Technical info: display field, DB field: kpos.me
- **Dimens. variant** Dimensional variant of article. Technical info: display field, DB field: kpos.var

##### Hit list - miscellaneous tab
**Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3> > Miscellaneous Tab**
This tab displays various information about the purchase orders that fits the search criteria. One line is displayed per purchase order item. Use `<F2>` to change tabs on the hit list.

**Header**
The fields in the header area are described for the **Find Purchase Orders** dialog:
- "Find purchase orders" on page E-1552

**Miscellaneous tab**
The columns are described for the **Quantities** and **Articles** tab:
- "Hit list - quantities" on page E-1561
- "Hit list - article" on page E-1563
In addition, the following columns are displayed:
- **Stock:** Stock number for the purchase order. Technical info: display field, DB field: bpos.Inr
- **Customer:** Customer name for order-related P.O.s. Technical info: display field, DB field: mp.name

### Purchase Order Pool
In the PO pool, the following PO proposals are collected, which are combined into one or several POs:
- Order-related PO proposals from Sales.
- PO proposals from stock, e.g. before stock inventory runs too low. This function must be configured.

If no automatic PO proposals can be generated by the stock, you can create the stock POs via the **Purchase Order Entry** dialog.

Depending on system configuration and specified supplier master data, POs can be grouped 1:1 from the order data by the background process or first grouped manually in the PO pool, then generated.

The PO release is done either automatically or when the PO is printed. The following are the possibilities:
- The purchase order is created and automatically released.
- The purchase order is printed and automatically released.
- The purchase order is manually released using the **Purchase order release** dialog.

Depending on the system configuration, the PO release is possible via the **Purchase Order Release** menu element:
- "Purchase Order Release" on page E-1631

Another possibility exists if the system is configured accordingly when storing a payment advice note. Insofar as the PO advice note is saved, the order is set to the status **Ordered**.
- "Dispatch notifications" on page E-1637

Use the **Printing of forms** or **Email** dialog to print purchase orders and send them to the supplier. The dialogs are described in detail in the Sales section:
- Sales, "Form printing" on page D-1419
- Sales, "E-mail" on page D-1423

In the change log, you can check the status of a PO. The dialog is described in detail for the Sales section:
- Sales, "Amendment log" on page D-1228

The following information is available on this chapter:
- "Special menus for the PO pool" on page E-1567
- "Purchase Order Release" on page E-1631
- "Creating purchase orders" on page E-1569

#### Special menus for the PO pool
In the PO pool, dialog-specific menus can be called up.
- Use `<F4>` to open the supplementary menu for the PO pool.
- Use `<Shift>` + `<F4>` to open the info menu for the PO pool.

The displayed entries depend on the respective configuration. The following overviews of the menus always list all entries.
The following supplementary menus are available:
- "Purchase order pool – additional menu" on page E-1567
- "Purchase order pool – menu info" on page E-1568

> **Context menus**
> On the context menus, only the menu elements are offered that make sense in the context for the individual fields of the dialogs. The functions are described in the following chapters:

##### Purchase order pool – additional menu
**Purchase > Create Purchase Orders > Enter Department > <F3> > <F4>**
Most-used configuration

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Reset tagged items (Shift+F12) | Disables the Cr. (Create PO) checkbox for the marked items. The items can be edited once again. |
| b | Group by tag (Ctrl+F8) | Groups the items under one PO number. The Cr. (Create PO) checkbox must be enabled. |
| c | Group by order (Ctrl+O) | The Cr. (Create PO) checkbox must be enabled. Items with the same order number and the same supplier are grouped under a common PO. For items with the same order number but different suppliers, individual POs are created for the items per supplier. Grouping by orders depends, among other things, on configuration. Please contact an A+W Software GmbH service employee. |
| d | Sort by purchase order (Ctrl+F12) | Sorts the purchase order numbers in descending order. |
| e | Purchase order header (Ctrl+K) | Sales, "Header and footer texts" on page D-1308 |
| f | Purchase order footer (Ctrl+F) | Sales, "Header and footer texts" on page D-1308 |
| g | Tag (downwards) (Shift+F11) | Enables the Cr. (Create PO) checkboxes for the selected and all subsequent items. |
| h | Tag (all) (Ctrl+F11) | Enables the Cr. (Create PO) checkbox for all items. |
| i | Cancel | No action at this point |
| j | Inquiry (Ctrl+E) | Selects the In (Inquiry) column of the selected item with an E. If the Cr. (Create PO) checkbox of the item is enabled, you can create an inquiry for the supplier with `<Ctrl>+<F8>`. |
| k | All inquiries (Ctrl+L) | Selects the In (Inquiry) column of all items with an E. If the Cr. (Create PO) checkbox of the item is enabled, you can create an inquiry for the supplier with `<Ctrl>+<F8>`. |
| l | Enquiries starting from cursor position (Ctrl+G) | Selects the In (inquiry) column with an E for the selected and all subsequent items. If the Cr. (Create PO) checkbox for the item is enabled, you can create an inquiry for the supplier with `<Ctrl>+<F8>`. |
| m | Tag inquiries (Ctrl+N) | Enables the Cr. (Create PO) checkbox for all items with an E in the In (inquiry) column. |
| n | Purchase orders not transferred yet | "Overview of documents" on page E-1681 |

##### Purchase order pool – menu info
**Purchase > Create Purchase Orders > Enter Department > <F3> > <Shift> + <F4>**

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Show order texts (Ctrl+F10) | "Order texts" on page E-1629 |
| b | Purchase info | In the selected order item to be ordered, an extra field Purchase info is displayed. Insofar as such information was entered in the associated order, this text is displayed in the field. New entry of the purchasing information in the PO pool is not possible. |
| c | Suppliers notes | Sales, "Market partner, project, article notes" on page D-1303 |
| d | Supplier article notes | Sales, "Market partner article notes" on page D-1305 |
| e | Article notes | Sales, "Market partner, project, article notes" on page D-1303 |
| f | Information on complaints | Displays the complaint information for the selected item from the order. "Creating purchase orders" on page E-1569 |

#### Creating purchase orders
**Purchase > Create Purchase Orders > Enter Department > <F3>**
**Purchase > Create Stock Orders**
Use this dialog to convert PO proposals into POs. Depending on the configuration of the program and the desired result, you can also create the PO from a PO proposal or group several POs under one PO number.

PO proposals can also be created automatically if:
- the supplier for the goods ordered from the order is selected in the master data as direct supplier.
- if there is insufficient stock. The function for automatic POs from the stock must be configured. If PO proposals cannot be created automatically by the stock, you must create the stock POs via the **Purchase Order Entry** dialog. "Purchase order entry" on page E-1584

This dialog offers the following tabs:
- "Creating purchase orders - supplier" on page E-1570
- "Creating purchase orders – item" on page E-1574
- "Creating purchase orders - details" on page E-1575

##### Creating purchase orders – supplier
**Purchase > Create Purchase Orders > Enter Department > <F3> > Supplier Tab**
All PO proposals are collected in the PO pool. When working with several purchasing departments and/or companies, you can configure the selection dialog to minimize the data and distribute it appropriately. After selection of the company and/or department, the PO proposals are listed on the **Create PO** dialog. On this tab, the supplier information for the PO proposals is displayed. You can release the purchase orders in the **Purchase Order Release** dialog. "Purchase Order Release" on page E-1631

**Selection dialog**
- **Site**: Selection of the number of the client. This field is only available with internal client separation. Technical info: display field, DB field: kauf.hausnr
- **Department**: Number of department. You can use `<F9>` to search for a number. Technical info: mandatory field, numeric field, DB field: kauf.abtnr
- **Additional purchase orders**: Purchase order number. You can use `<F9>` to search for a number. Use `<Enter>` to specify another PO number that is added in a new cell. You can sort the PO numbers in ascending or descending order with the **Additional POs** button. Technical info: numeric field, DB field: kauf.auftrnr (kauf.vorgang=2)

Use `<F3>` to confirm the selection.

**Create purchase order**
To create the POs, the following steps must be taken:
- In the **Cr.** field, select the PO proposals for which you want to create a PO. Depending on the system configuration, with selection of a PO item from the order, all other PO items from the same order are marked. The **Keep order items together** option can also be used for selection deletion. If an extended workbench PO is to be created from the PO pool, all related components for an order item and the date are marked on the block and thus kept together.
- With `<Ctrl>+<F8>` you group the PO proposals and create POs. If you select several items, one or several POs can be created for the items. The grouping is done either according to selection, supplier change or orders. The type of grouping can be specified via the system configuration.
- Use `<End>` to trigger the PO creation and save the settings made. The POs can be corrected on the PO Management dialog and released on the PO Release dialog.

**Delete grouping**
You can reset the grouped item with already-assigned PO numbers in order to leave the item in the PO pool. For this, select the item in question and remove it from an order-related PO proposal by selecting the order item and deleting the PO number for this PO item via `<F4> > Reset selected items`.

**Supplier tag**
- **Site**: Number of site. Technical info: display field, DB field: kauf.hausnr
- **PO No.**: Purchase order number under which the purchase orders can be grouped. Purchase order numbers are preliminarily created using the selection in the **Cr.** column or canceled using the selection of column **C**. You can confirm your selection using `<End>` or **[OK]**. Technical info: numeric field, DB field: bestpool.baufnr
- **Cr.**: Specification of whether a PO should be created for the item. You can select several entries and group them in a PO.
  - The item in the PO pool is selected for PO creation.
  - There will be no PO creation for this item.
  Use `<Ctrl>+<F8>` to group the selected item for the PO creation. If you select several items at the same time, one or several POs will be created depending on the system configuration. Technical info: checkbox
- **Order**: Order number for PO proposals that are determined with reference to an order. Technical info: numeric field, DB field: bestpool.orgauftrnr
- **Article**: Article number to be ordered. Technical info: mandatory field, numeric field, DB field: bestpool.artnr
- **Description**: Article description of the purchase item. Technical info: alphanumeric field, DB field: bestpool.artbez1
- **C**: Indication whether the article to be ordered was already canceled, e.g. because an order correction has been made in the meantime. The flag is set by the system and cannot be changed here.
  - The PO item was canceled and can no longer be created.
  - The PO item is not canceled and can still be edited.
  Technical info: checkbox, DB field: bestpool.still
- **Supplier**: Supplier number for the article. By default, the number of the default supplier for the article from the master data is displayed. If another supplier was assigned to the article in the customer order, the number of this supplier is displayed.
  - Use `<F10>` to open the market partner search for selection of another supplier.
  - Sales, "Find market partner" on page D-1087
  - Use `<F5>` to open the dialog Addresses for selecting a different address.
  - Use `<Ctrl>` + `<O>` to store the new supplier as default supplier for the selected article in the master data.
  Technical info: mandatory field, numeric field, DB field: bestpool.linr
- **Quantity**: Article quantity of the ordered item. Depending on the assigned quantity unit of the article, the quantity is displayed in this quantity unit. For stock POs, the PO quantity from the stock master data is used. You can change the PO quantity. Technical info: numerical field, DB field: bestpool.menge
- **Ordered for**: Probable delivery date of the PO. The delivery date is calculated from the master data. You can change the date. Technical info: date field, DB field: bestpool.solldat
- **Txt.**: Texts. Specification whether texts are entered for the PO item.
  - A: Article texts are stored for the item.
  - B: Article and item texts are stored for the item.
  - P: Item texts are stored for the item.
  Use `<Shift> + <F4> > Show order texts` to view the stored information. "Order texts" on page E-1629. Technical info: numeric field, DB field: bestpool.arttxtnr and bestpool.poskotxtnr
- **PI**: Purchase information. Indication whether third-party information in the customer order is stored for the PO item. If purchase information is stored, an `/` is displayed in the field. Use `<Shift> + <F4> > Purchase info` to view the stored information. Technical info: display field
- **Cm**: Complaint. Indication whether the PO was created due to a customer complaint.
  - The item is being re-ordered due to a customer complaint.
  - The item is not part of a complaint order.
  Technical info: checkbox
- **In**: Inquiry. Indication whether an inquiry to the supplier is created. If a supplier inquiry is created, an `/` is displayed in the field. Via the supplementary menu, you can specify for which PO items a supplier inquiry should be created. Technical info: display field
- **In**: Info indication. The field is not currently used. Technical info: display field
- **SB**: Substitute order. Indication whether a broken item must be reordered. Technical info: display field

**Footer**
- **Supplier**: Supplier name of the selected item. Technical info: display field
- **[Grouping]**: This button groups one or several POs from the selected PO proposals.
- **[Trigger]**: Triggers the function in question, that is, the grouped PO proposals are transformed into POs and saved in the system under the specified number. The button is only displayed if the grouping has already been made.

##### Creating purchase orders – item
**Purchase > Create Purchase Order > Enter Department > <F3> > Item Tab**
This tab displays item information for ordered articles.

**Item tab**
The fields are described in connection with the **Create Purchase Order** dialog:
- "Creating purchase orders - supplier" on page E-1570
In addition, the following fields are displayed:
- **Itm**: Item number for PO items from customer orders. Technical info: numeric field, DB field: bestpool.orglfdpos
- **Stock**: Stock number for the PO for stock articles. You can change the stock number. Technical info: numeric field, DB field: bestpool.lnr
- **Width, Height**: Dimensions of the item in millimeters. You can change the dimensions if required. If a variant item is entered in the PO item, you can use `<F9>` to select another dimensional variant or remove the variant reference and specify freely selected dimensions. Technical info: numeric fields, DB fields: bestpool.laenge, bestpool.breite
- **Qt**: Indication whether article in the PO item is not an item article, but a subpart from a BOM. If the article is a BOM subpart, an asterisk `*` is displayed in the field. Technical info: numeric field, DB field: bestpool.orglfdpos

**Footer**
The fields and buttons in the footer area are described for the **Create Purchase Order - Supplier** tab:
- "Creating purchase orders - supplier" on page E-1570

##### Creating purchase orders – details
**Purchase > Create Purchase Orders > Enter Department > <F3> > Details Tab**
The detailed information about the articles to be ordered is displayed on this tab. You can add item data if necessary.

**Details tab**
- **Site**: Site number for which the POs are triggered. Technical info: display field, DB field: bestpool.hausnr
- **P.O.**: PO number and item number in the PO. Technical info: display fields, DB fields: bestpool.baufnr, bestpool.orglfdpos
- **Order**: Order number, item number and tuple number for the ordered order subparts for which the PO proposal is made. Technical info: display fields, DB fields: bestpool.orgauftrnr, bestpool.orglfdpos, bestpool.orgtnr
- **Customer**: Number and name of the customer for PO items from customer orders. Technical info: display fields, DB fields: bestpool.kunr, mp.name
- **Operator**: Name of the person entering the order for PO items from customer orders. Technical info: display field, DB field: kauf.eusr
- **Proj.**: Number and description of the project. Technical info: display fields, DB fields: bestpool.objnr, mp.name
- **Purch. info**: Third-party information for purchasing for PO items from customer orders. The field is only shown if purchase info was stored in the order. Technical info: display fields, DB fields: kauf.exbez1
- **(without name)**: Number for different address if it was entered as delivery address. Technical info: numeric field, display field, DB fields: bestpool.divadrnr
- **Stock**: Number and designation of the stock for stock articles. You can change the stock. Technical info: numeric field, display field, DB field: bestpool.Inr
- **Article**: Number and description of the article. Technical info: mandatory field, numeric field, display field, DB fields: bestpool.artnr, bestpool.artbez1
- **Shape**: Shape number for PO items with lite shape. Technical info: display field, DB field: bestpool.modnr
- **Supplier**: Number and name of the supplier. You can change the supplier.
  - With `<F9>` you can select the supplier from the suppliers that are stored for the article in the master data.
  - Use `<F10>` to open the market partner search dialog for selection of another supplier.
  - Use `<Ctrl> + <O>` to store the selected market partner as default supplier for the current article in the master data.
  - Use `<F5>` to change the delivery address. By default, the supplier's main delivery address is selected.
  Technical info: numeric field, display field, DB fields: bestpool.linr, mp.name
- **Fax**: Fax number of the supplier from the master data. Technical info: display field, DB field: bestpool.faxnr
- **P.O. no.**: Supplier-side number and designation of the article if a supplier-specific article number is stored for the article in the master data. Technical info: alphanumeric field, DB fields: bestpool.exartnr, bestpool.exartbez
- **Quantity**: PO quantity of the ordered item in the quantity unit of the article stored in the master data. You can change the PO quantity. Technical info: mandatory field, numeric field, DB field: bestpool.menge
- **QU**: Quantity unit. For length, time, and piece articles, the respective quantity unit is displayed in this field, e.g. meter, liter. Technical info: display field, DB field: bestpool.me
- **Width, Height**: Dimension of the item in the quantity unit of the article stored in the master data. You can change the dimensions. If a variant article is entered in the PO item, you can use `<F9>` to select a different dimension variant or remove the variant reference and specify freely selectable dimensions. For PO proposals from the stock, the dimensions of the PO variant are used. For missing entries, this information is urgently needed when opening the item in question. Technical info: numeric fields, DB fields: bestpool.laenge, bestpool.breite
- **AIR**: Width of the airspace in the appropriate dimensional units. You can change the airspace. The airspace is only displayed if an IG article is entered in the PO item. Technical info: numeric field, DB field: bestpool.szr
- **Variant**: Variant number and variant designation of the article. You can change the variant. If you select another dimensional variant, the **Width** and **Height** fields are adjusted automatically. Technical info: alphanumeric field, DB fields: bestpool.bitnr, bestpool.varart
- **Cust. route**: Delivery date to the customer. Technical info: display field, DB field: bestpool.liefdat
- **Ordered for**: Probable delivery date of the PO. The delivery date is calculated from the master data. You can change the date. Technical info: mandatory field, date field, DB field: bestpool.solldat
- **Ordered on**: Date of the purchase order entry. Technical info: mandatory field, date field, DB field: bestpool.bestdat
- **Own curr.**: Unit price and item price in the national currency, e.g. euros. Technical info: display field, DB fields: bestpool.nstpreis, bestpool.npospreis
- **For. curr.**: Unit price and item price in a foreign currency, e.g. dollars. Technical info: display fields, DB fields: bestpool.fnstpreis, bestpool.fnstpreis
- **Currency, Rate**: Number and name of the currency and currency rate, e.g. rate for conversion of Euros to dollars. Technical info: display fields, DB fields: bestpool.waehrung, waehrung.kurzbez, bestpool.kurs
- **Cost center**: Cost center name for statistical evaluations for PO items from customer orders. Technical info: display field, DB field: bestpool.kostenst
- **Incoterms**: Requested type of delivery:
  - **Pickup**: Customer collects the goods.
  - **Third-party business transaction**: The producing plant will ship the goods directly to the customer.
  - **No selection**: Goods will be delivered via the route that has been entered in the customer order.
  Technical info: toggle field, DB field: bestpool.geschart
- **Reject place**: Number and name of the reject place where the glass break happened. The number only needs to be specified if an item needs to be reordered due to glass breakage. Generally the reject place is transferred from production and taken over in this field. If needed, you can change the reject place in A+W Enterprise. The reject place name is displayed in plain text in the next field. The reject places are stored in the database table xbruchort. The values from production are taken over automatically. There is no maintenance dialog for this table in A+W Enterprise. Technical info: numeric field, display field, DB field: bestpool.bruchort
- **Reject reas.**: Number and designation of the reject reason. The number must only be specified if an item has to be reordered due to a glass break. You can change the reject reason. If you specify a number, the reject reason is displayed in plain text. Technical info: numeric field, display field, DB field: bestpool.bruch

**Footer**
- **Totals**: Total of the item for weight in kilograms, area in square meters, and length in linear meters. Technical info: display fields
- **Item**: The **Item** indication specifies that displayed totals per item apply. Technical info: display field
The buttons in the footer are described for the **Create Purchase Order - Supplier** tab:
- "Creating purchase orders – supplier" on page E-1570

### Document Management

The documents that you edit in the **Purchasing** area include supplier inquiries, POs, receipts of goods, supplier invoices, and credit notes. The dialogs look and work largely the same way as those for the **Sales** area.

The following sections are part of the document management:
- "Explanation of symbols" on page E-1580
- "Supplier inquiries" on page E-1583
- "Purchase order entry" on page E-1584
- "Purchase order items" on page E-1603
- "Pick-up address" on page E-1625
- "P.O. type" on page E-1627
- "Allocation of document types" on page E-1628

#### Explanation of symbols
This section describes the identifiers for the dialog mode, the item status, and the item identifier.

##### Dialog mode
The dialog mode is shown in the title line of the dialog.

| Symbol | Symbol description | Meaning |
| :--- | :--- | :--- |
| Dialog with cross | In this mode, you can create new records. |
| Dialog with pen | In this mode, you can edit a document. |
| Yellow triangle with exclamation point | In this mode, you can not edit the document. |
| Find | In this mode, you can search for documents. |

##### Item status and symbols
The item status is displayed on the **Items** tab next to the **Item** column.

| Symbol | Symbol description | Meaning |
| :--- | :--- | :--- |
| green | The item can be changed as desired since the purchase order has not yet been released. |
| yellow | The item or sub-parts of the item have been ordered or the purchase order has been printed. |
| red | The item is released in the PO. It can no longer be changed. |
| red/red-blue | Item has been partially delivered. |
| red/blue | Item has been fully delivered. |
| red-blue/blue | Item has been partially invoiced. |
| blue | Item has been invoiced completely. |

The item identifier is displayed in front of the **Item** column.

| Symbol | Symbol description | Meaning |
| :--- | :--- | :--- |
| Yellow star | The product dimension and additional processing of the article are stored for the selected supplier. After saving the supplier-specific article, a green star is displayed. Sales, "Fix product" on page D-1515 |
| Green star | The article has been defined supplier-specifically and can only be entered for this specific supplier. When you create a supplier-specific article, you can create the BOM structure with additional processings, articles, dimension changes and additional supplier-specific requests. Sales, "Article details for dimensioned variants" on page D-1214 |
| Lite shape | Item is entered with shape. Sales, "Shape - dimensions" on page D-1232 |
| Window with Georgian bars | Item has been entered with muntins. Sales, "Muntin entry" on page D-1281 |

The status in text format is shown in the dialog line or in the **General** tab above the **Proc.type** column when the item status changes. The following status displays are possible:

| Status in text format | Meaning |
| :--- | :--- |
| Stock withdrawal | A stock withdrawal has been booked for this item. |
| Partially ordered | A partial order exists for the item, e.g. for an article from the bill of material. |
| Cancel | The purchase order has been canceled. |
| Invoiced | The purchase order has been invoiced and can no longer be changed. On the right hand side next to Invoiced, the number of the supplier invoice is displayed. |
| Dispatch planning available | The PO is planned in dispatch. Commercial changes, such as price changes, are still possible under some circumstances. |
| Global correction | Changes in the PO are no longer transferred to the database. Commercial changes such as price changes, are still possible under some circumstances. |
| Local correction | Changes in the item are no longer transferred to the system during PO entry if they affect the PO, e.g. dimension changes. Commercial changes, such as price changes, are still possible under some circumstances. |

#### Supplier inquiries
**Purchase > Inquiries**
Use this dialog to create and edit inquiries to suppliers.
If you enter a delivery date in the inquiry, you can create a resubmission date to ensure the post-processing of an inquiry. When the resubmission date has arrived, a message will be displayed at the program start or a reminder e-mail sent.
The resubmission is described in detail in the Sales section:
- Sales, "Resubmission" on page D-1467
Each inquiry can be converted into a purchase order.
The dialog is structured the same as the **Purchase Order Entry** dialog. Deviations will be described explicitly for the **Purchase Entry** dialog.
- "Purchase order entry" on page E-1584

#### Purchase order entry
**Purchase > P.O. Management**
On this dialog, you enter and/or edit purchase orders.
For regular creation of POs, you usually use the **Create Purchase Order** dialog. Then you can view or edit the POs created on the **Order Management** dialog.
- "Creating purchase orders" on page E-1569
This dialog contains the following tabs in the header area:
- "Purchase order entry - header, footer" on page E-1585
- "Purchase order entry - addresses" on page E-1590
- "Purchase order entry – properties" on page E-1592
- "Purchase order entry – miscellaneous" on page E-1597

The **Items** tab offers the following tabs:
- "Purchase order items - general" on page E-1604
- "Purchase order items - properties" on page E-1613
- "Purchase order items - prices" on page E-1617
- "Purchase order items - order info" on page E-1620
- "Purchase order items - status" on page E-1622
- "Purchase order items - evaluation" on page E-1624

##### Purchase order entry – header, footer
**Purchase > P.O. Management > Open Purchase Order > Items Tab**
On this dialog, you specify the supplier data and enter the PO items. If you enter items, it is generally sufficient to enter the data in the **General** tab.
- Use `<Enter>` to change to the next field, `<Page Up>` to jump to the first item, `<Page Down>` to jump to the last item.
- Use `<End>` to switch to the footer and conclude the purchase order management.
- Use `<F2>` to switch from the **Contract** field to the **Addresses, Properties** or **Miscellaneous** tabs.

**Header**
- Use `<Ctrl>+<F12>` to change from the **Receipt, Invoice Type** or **Project** fields to the **PO Type** dialog.
  - "P.O. type" on page E-1627
- Use `<F2>` to change from the **Receipt, Invoice Type** or **Project** fields to the Item area.

> **List purchase orders**
> If you open the Purchase Order Entry dialog, you can use `<F5>` to change to the S-order field and search for the associated POs by entering the order number. Alternatively, you can list and then select all existing POs with `<F9>`.

- **Purchase**: Purchase order number. Technical info: mandatory field, numeric field, DB field: kauf.auftrnr (kauf.vorgang=2)
- **Supplier**: Supplier number. If you specify a number, the supplier's name and location are displayed in plain text. Technical info: mandatory field, numeric field, display fields, DB field: kauf.kunr, kauf.orgname
- **Reason**: Reason for a date change. The Reason field is only displayed if you change the delivery date in a purchase order previously entered. Technical info: alphanumeric field, DB field: kaufltedit.text
- **Ref.**: Document number that is being referenced.

**Pre-selecting document type for the reference**
Depending on the system configuration, it is possible to specify one of the document types as pre-selection for the reference entry:
- Use `<F8>` to display the document type configured as default in the **Reference** field.
- Use `<F9>` to open a selection dialog with all document types that can be referred to. use the arrow keys to select a document type.
- Use `<Enter>` to confirm the selection.
- The **Reference** field displays the number of the current market partner.
- If you would like to specify the current market partner as pre-selection, then confirm with `<Enter>`.
- If you would like to specify another market partner as pre-selection, use `<F9>` to open the **Find Market Partner** dialog in order to select a market partner. Alternatively, you can enter the market partner number directly in the field. Use `<Enter>` to confirm the selection.
- The **Reference** field is empty. If you open the **Find Reference** dialog now, the document type and market partner that you have specified are pre-selected as search criteria.

**Enter document with reference**
- Use `<F9>` to open the **Find Reference** dialog in order to select a reference document for the specified criteria. Alternatively, you can enter the document number directly in the field.
- Use `<Enter>` to confirm the selection. You can take over all data from the reference document or only the header data from the reference document.
You can take over all data from the reference document or only the header data from the reference document. This decision is made via confirmation of the corresponding Yes/no message.
- Use `<F9>` to open the **Find Reference** dialog. The dialog is described in detail in the Sales section.
  - Sales, "Find deference document" on page D-1093
Technical info: numeric field, DB field: kauf.referenz

> **Reference to order**
> If you reference an order in the PO, then all order items will be loaded into the PO entry. If necessary, items on the General tab must be deleted or adjusted.

- **Site**: Site number at which the PO is entered. If you are working with internal client separation, the **Client** field is released. If you are also working with site-company assignment, the first field displays the company number to which the site is assigned from the system master data. Technical info: numeric fields, DB fields: kauf.company, kauf.hausnr
- **Entry date**: Entry date. By default, the field is pre-populated with the current date. This entry can be changed. Technical info: mandatory field, date field, DB field: kauf.edat
- **Cust. order**: Customer order number from sales for order-related purchase orders. Depending on the configuration, alternative data can be shown:
  - **Cus.ord.-no.**: External customer purchase order number. For orders from another site, the order number of the sending site is in this field.
  - In the event of internal remote data transmissions between two plants, the following data can also be shown in combination: Purchase order number from the sending site, Order number, Customer purchase order number.
  - **Stock P.O.**: Display that a stock purchase order is being executed.
  - **Collective purchase order**: Display that order-related order items have been combined into a collective purchase order. Collective purchase orders can be executed by the supplier in the form of partial deliveries.
  - External number system, e.g. quotation number from the supplier.
  Technical info: alphanumeric field, DB field: kauf.exaufnr
- **Date**: Requested delivery data of purchase order. In the first field you can enter the calendar week. In the second field you can enter the date in the format DD.MM.YYYY. Technical info: mandatory field, numeric field, date field, DB fields: kauf.kwideal, kauf.ltideal
- **Route**: Route number. Route selection shows the routes and corresponding route dates. You can store one main route and three alternative routes for a customer in the master data. If the via-plant function is configured, use `<F5>` to select the site via which the delivery should be organized. Technical info: mandatory field, numeric field, DB field: kauf.routenr
- **Deliv. date**: Display of the planned delivery date. Technical info: display field, DB field: kauf.ltplan
- **Suppl. item**: Specification of supplier items in the PO.
  - **yes**: The items can be entered with the supplier's article numbers. If you have assigned the supplier's article numbers to the articles in your master data, you can select articles via your master data. In the PO, the supplier's article numbers are transferred to the suppliers. For the item entry via supplier-related article data, the field **S.Item** is enabled on the **General** tab.
  - **no**: The individual article numbers are entered.
  Technical info: toggle field, DB field: kauf.kndposkz
- **Date type**: Information about the date type that will be printed on the order.
  - **Call**: date on call.
  - **urgent**: as soon as possible.
  - **poss.**: if possible, by the date.
  - **bind.**: date is binding.
  - **without**: without date type.
  - **Auto**: currently not used.
  - **follows**: date to follow.
  Technical info: toggle field, DB field: kauf.abrufkz
- **Receipt**: Will not be used. Technical info: toggle field, Database field: kauf.eingang
- **Invoice type**: Specification of the services for which the invoice is issued. Usually, the glass and the installation work are invoiced together. Upon request, you can create individual invoices.
  - **Total**: The invoice is created for the total purchase order, that is, for material and installation services.
  - **Glass**: The invoice is only created for the material of the purchase order.
  - **Service**: The invoice is only created for the installation services of the purchase order.
  Technical info: toggle field, DB field: kauf.rechart
- **Project**: Project number. A project is assigned to the market partner and can, e.g. be a construction site that is supplied directly by the supplier and have a different delivery address. You can link particular conditions with the project that only apply to this project, e.g. discounts or payment options. You have the opportunity to bill project-related. Use `<F9>` to open the project search. The project search is described in detail in the Sales section.
  - Sales, "Find project" on page D-1115
  Technical info: numerical field, DB field: kauf.objnr

**Footer**
In the footer area, the total order values for the individual dimensional units and the total amounts of the items are displayed. You can grant a general discount and overwrite the amount in the **Net Total** field, e.g. if you have made a special agreement with the supplier.
Use `<F2>` to open the **Purchase Order Entry** dialog for calculating discounts and the net amount.
- "Purchase order entry - totals" on page E-1601
- **Sender**: Display of the site number and the reference number. The reference number can be the quotation number or for EDI orders the order or purchase order number. Technical info: display fields, DB fields: kauf.hausnr
- **Qt, lb, sf**: Display of the total purchase order value for the quantity in pieces, weight in kilograms, and area in square meters. Technical info: display fields, DB fields: kauf.gesst, kauf.gesm2, kauf.gesgewicht
- **Total**: Display of the total price of all items less the item discount from the field **Minus** on the **Prices** tab. The total price of an item is calculated as item price x item quantity. "Purchase order items - prices" on page E-1617. Technical info: display field, DB field: kauf.gesnetto
- **Discount**: Discount granted for the total amount in percent. With discount granted, the amount in the **NetTotal** field is adjusted. Technical info: numeric field, DB field: kauf.gesfaktor
- **Net total**: Total of all item prices, incl. the discounts and plus the surcharges. It is not possible to edit the amount. The system calculates the difference and displays it in the **Gen. discount** or **Gen. surcharge** field on the calculation dialog. "Purchase order entry - totals" on page E-1601. Technical info: numerical field, DB field: kauf.nettototal
- **+VAT ()**: Display of the VAT. The VAT amount is in the field that is assessed on the net amount. In the brackets, the applicable VAT is displayed in percentage. Technical info: display field, DB field: kauf.mwstbetrag
- **Gross**: Display of the gross total amount. The amount is calculated from the net amount plus the VAT. Technical info: display field, DB field: kauf.gesbrutto
- **C. margin**: Display of the contribution margin (gross margin) that a product contributes to covering the fixed costs and to achieving the net profit. All discounts and surcharges are taken into account. Technical info: display field, DB field: kauf.dbdm

##### Purchase order entry – addresses
**Purchase > P.O. Management > Open Purchase Order > Field Entry Date, Invoice Type > <F2> > Addresses Tab**
On this tab, you can edit the supplier and delivery address. By default, the delivery address from the supplier master data is used in the delivery address area. You can configure the determination of the delivery address customer-specifically. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

**Header**
The fields in the header area are described for the **Purchase Order Entry – Header, Footer** tab:
- "Purchase order entry - header, footer" on page E-1585

**Supplier's address**
- **Name, 1stName**: Supplier's first and last names. Technical info: alphanumeric fields, DB fields: kauf.orgname, kauf.orgvorname
- **Title**: Number of the title. If you select a number, the title is displayed in plain text. Technical info: numeric field, DB field: kauf.organrede
- **Attn.**: For the attention of. Name of the person who should receive the purchase order. Technical info: alphanumeric field, DB field: kauf.orgzhd
- **Addition**: Additional text for address. Technical info: alphanumeric field, DB field: kauf.orgbranche
- **Street**: Street address of the supplier. Technical info: alphanumeric field, DB field: kauf.orgstr
- **PCd. POB**: Postal code and P.O. box number. Technical info: alphanumeric fields, DB fields: kauf.orgpfplz, kauf.orgpostfach
- **PBoxCity**: City name for the PO box of the supplier outside Europe. Technical info: alphanumeric field, DB field: kauf.vertr
- **PCd.City**: Postal code and city of the supplier's address. Technical info: alphanumeric field, DB fields: kauf.orgplz, kauf.orgort
- **Country**: License plate ID for the target country. If you select a code, the country name is displayed in plain text. Technical info: alphanumeric fields, DB fields: kauf.orgkfzcode, kauf.orgland
- **Pho**: Supplier's phone number. Technical info: alphanumeric field, DB field: kauf.orgtel
- **Fax**: Supplier's fax number. Technical info: alphanumeric field, DB field: kauf.faxnr
- **Language**: Number of the national language of the supplier in which the documents will be printed. If you select a number, the language is displayed in plain text. Technical info: numeric field, DB field: kauf.sprkz
- **Code**: Number of tax code. The tax code is the tax key that is used to calculate the VAT. If you select a number, the description of the tax code is displayed in plain text. Technical info: numeric field, DB field: kauf.kukz

**Delivery address**
You can enter a different shipping address, e.g. for direct delivery the address of a construction site.
- Use `<Ctrl>+<N>` to create a new delivery address for the supplier.
- Use `<Ctrl>` + `<L>` to select the stored delivery address of a supplier.
The fields are described for the **Supplier Address** area:
- "Supplier's address" on page E-1590
In addition, the following field is described:
- **Reg. no**: Dispatch region. The dispatch region is stored in the master data and is determined via the postal code. It is relevant only for orders. Technical info: display field

**Footer**
The fields in the footer area can only be entered on the **Items** tab. They are described for the **Purchase Order Entry - Header, Footer** tab:
- "Purchase order entry - header, footer" on page E-1585

##### Purchase order entry – properties
**Purchase > P.O. Management > Open Purchase Order > from Field Entry Date on <F2> > Properties Tab**
On this tab you can edit information relating to staff allocation, shipping information, and invoice and printing options.

**Header**
The fields in the header area are described for the **Purchase Order Entry – Header, Footer** tab:
- "Purchase order entry - header, footer" on page E-1585

**Staff allocation**
- **Ordered by**: Employee number of the supplier. If you select a number, the employee's name is displayed in plain text. Use `<F5>` to open the **Contact Person** dialog where you can select or create a new contact person. The **Contact Person** dialog is described in detail in the Sales section. Sales, "Contacts" on page D-1197. Technical info: numeric field, DB field: kauf.busnr
- **PO date**: Date of the purchase order entry. Technical info: date field, DB field: kauf.bdat
- **Operator**: Displays the number and name of the operator. Technical info: display fields, DB field: kauf.esuer
- **Handled by**: Name of the administrator. If you select a number, the administrator's name is displayed in plain text. Technical info: numeric field, DB field: kauf.abvertr
- **Field staff**: Name of the field employee. Technical info: alphanumeric field, DB field: kauf.vertr
- **Sales repres.**: Sales representative. Number of the representative to whom the commission will be paid. If you select a number, the representative's name is displayed in plain text. Technical info: numeric field, DB field: kauf.vertrerloe

**Shipment information**
- **Maximum load**: Maximum weight that the supplier can unload with its technical equipment. Technical info: numerical field, DB field: kauf.gmaxgew
- **Delivery**: Comment about the requested delivery method. Usually, the type of delivery is not used in the Purchase area.
  - **Pick-up**: Goods will be picked up with PO.
  - **Third-party business transaction**: The producing plant will ship the goods directly to the supplier.
  - **No selection**: Goods will be delivered via the route that has been entered in the header.
  Technical info: toggle field, DB field: kauf.geschart
- **Dir. dispatch**: Indicator as to whether the supplier will receive the delivery directly from the production facilities or whether the goods will be delivered to the dealer. The code is not used in the Purchase area. Technical info: toggle field, DB field: kauf.drkliefkz
- **Incoterm**: Number of the method of delivery, e.g. carriage paid. If you select a number, the name of the delivery type is displayed in plain text. Technical info: numeric field, DB field: kauf.lieferart
- **Disp. type**: Number of the dispatch type, e.g. truck. If you select a number, the description of the dispatch type is displayed in plain text. Technical info: numeric field, DB field: kauf.versandart
- **Packing type**: Number of the packing type, e.g. box. If you select a number, the name of the packing type is displayed in plain text. Technical info: numeric field, DB field: kauf.verpackart
- **Rack load**: Rack load. Select by which criteria the goods shall be sorted on the racks:
  - **Item**: by item.
  - **Size**: by size.
  - **Air+size**: by airspace and size.
  - **Item (free)**: items kept together, but freely organized.
  - **HD glass col thick**: by hard dimension, glass dimension, and color.
  - **HD gl.dim color -** : by hard dimension, glass dimension, and color.
  - **HD gl.dim - thick**: by hard dimension, glass dimension, and thickness.
  - **HD - color thick**: by hard dimension, color, and thickness.
  - **HD glass dim - -** : by hard dimension and glass dimension.
  - **HD - color -** : by hard dimension and color.
  - **HD - - thick**: by hard dimension and thickness.
  - **HD - - -**: by hard dimension.
  - **Reference**: by reference text.
  Technical info: toggle field, DB field: kauf.gbelad
- **Customs exit**: Number of the customs exit office for the delivery papers. If you select a number, the name of the customs office is displayed in plain text. Technical info: numeric field, DB field: kauf.azsnr
- **Destin. customs**: Number of the customs office in the country of destination. If you select a number, the name of the customs office is displayed in plain text. Technical info: numeric field, DB field: kauf.bzsnr
- **Travel time, Distance**: Estimated travel time and display of the route. Depending on the configuration, the travel time is given in hours or days. It can affect the delivery date. The route is drawn from the **Distance** field of the delivery address. Technical info: numeric fields, DB fields: kauf.anfahrt

**Invoice and print options**
- **VAT ID no.**: Supplier's VAT ID no. Technical info: alphanumeric field, DB field: kauf.steuernr
- **Taxpayer's no.**: Supplier's registered tax number at tax office. Technical info: alphanumeric field, DB field: kauf.finstnr
- **Cost center**: Cost center name for statistical evaluations. Technical info: alphanumeric field, DB field: kauf.kostenst
> **Defining the cost center for the entire purchase order**
> If you enter a cost center, the item-exact cost centers from the master data are overwritten related to the purchase order.

- **Invoice type**: Type of invoice.
  - **Separate invoice**: The addressee will receive a separate invoice for every purchase order.
  - **Collective invoice**: The addressee will receive one invoice that combines several purchase orders. You can select at what intervals a collective invoice will be issued: weekly, every 14 days, monthly.
  Technical info: toggle field, DB field: kauf.rechnungsart

> **Note regarding the creation of collective invoices**
> Both the limit for collective invoices and the invoice recipient's consent to collective invoicing must be saved in the market partner master data.

- **Partial inv.**: Specification whether partial invoices are created after a partial delivery:
  - **Y**: permit partial invoices.
  - **N**: do not permit partial invoices.
  If you select **Collective invoice** in the **Invoice Type** field, and you permit partial invoices, goods shipped by partial shipment will be included in the next collective invoice.
  Technical info: toggle field, DB field: kauf. teilfakkz
- **Emergen.purch**: Current purchase order receives preferential treatment and is dispatched to production with higher priority.
  - **Y**: define as high-priority purchase order.
  - **N**: do not assign higher priority for the purchase order.
  Technical info: toggle field, DB field: kauf.gbelad
- **Print gross prices**: Gross prices are printed on market partner documents.
  - **Y**: print gross prices.
  - **N**: do not print gross prices.
  Technical info: toggle field, DB field: kauf.preisdrkz
- **Print customer factor**: The customer-specific factor can be printed on market partner documents.
  - **Y**: print customer factor.
  - **N**: do not print customer factor.
  Technical info: toggle field, DB field: kauf.rabdrkz
- **Print article text**: The article texts can be printed on the market partner documents.
  - **Y**: print product text.
  - **N**: do not print product text.
  Technical info: toggle field, DB field: kauf.atxtdrukz
- **Print shapes**: Print shape sketches for items in the attachment of the market partner documents.
  - **Y**: print shape sketch.
  - **N**: do not print shape sketch.
  Technical info: toggle field, DB field: kauf.moddrkz
- **Suppress item prices**: By default, the item prices are printed on the market partner documents. You can suppress the listing of the item prices, e.g. if you have agreed on a fixed price with the supplier for the whole purchase order.
  - **Y**: do not print item prices.
  - **N**: print item prices.
  Technical info: toggle field, DB field: kauf.posdrkz

**Footer**
The fields in the footer area can only be entered on the **Items** tab. They are described for the **Purchase Order Entry - Header, Footer** tab:
- "Purchase order entry - header, footer" on page E-1585

##### Purchase order entry – miscellaneous
**Purchase > P.O. Management > Open Purchase Order > from Field Entry Data on > <F2> > Miscellaneous Tab**
Use this tab to view complaint information, private fields, additional options, and payment options.

**Header**
The fields in the header area are described for the **Purchase Order Entry – Header, Footer** tab:
- "Purchase order entry - header, footer" on page E-1585

**Complaint information**
You can maintain complaint statistics with the data. The **Reason, Place,** and **Type** of complaint must be created in the master data.
- **Cause**: Number of the complaint type. If you select a number, the description of the complaint type is displayed in plain text, e.g. glass breakage. Technical info: numeric field, DB field: kauf.reklamart
- **Place**: Number of the complaint place. If you select a number, the name of the complaint place is displayed in plain text, e.g. unloading. Technical info: numeric field, DB field: kauf.reklamort
- **Type**: Number of the complaint type. If you select a number, the name of the complaint type is displayed in plain text, e.g. incorrect color. Technical info: numeric field, DB field: kauf.reklamspec
- **Date**: Complaint date in the format DD.MM.YYYY. Technical info: date field, DB field: kauf.reklamdat

**Payment options**
You can view the payment options that are transmitted by the supplier for the purchase order and edit them, if necessary. The payment options are determined from the master data.
- **Curr. rate**: Number and name of the currency and currency rate. The price is calculated customer-specifically in the currency specified. If you select a number, the currency name and currency rate are displayed in plain text. The **Rate** field is locked if **Own Currency** is selected. Technical info: mandatory field, numeric fields, DB fields: kauf.waehrung, kauf.kurs
- **Calculate in**: This field is only enabled if **Own Currency** is not selected in the **Currency** field. You can specify whether the prices are calculated in own currency or in the market partner's foreign currency:
  - **Own currency**: The prices are calculated by A+W Enterprise in own currency.
  - **Foreign currency**: The prices are calculated in the currency that is assigned to the market partner in the Currency field.
  Technical info: toggle field, DB field: kauf.waerprs
- **Print in**: Number for printing the market partner-specific documents in the calculated currency or foreign currency. If you select a number, the name of the print option is displayed in plain text. If you select a number, the name of the print option is displayed in plain text. Technical info: numeric field, DB field: kauf.waehrdru

> **The fields Calculate in and Print in**
> The fields **Calculate in** and **Print in** are only accessible if the currency module is licensed.

- **Pay. term**: Payment term in days, which has been agreed upon with the market partner. Technical info: numeric field, DB field: kauf.zahlziel
- **Val.date**: Period until the value date in days. Technical info: numeric field, DB field: kauf.valuta
- **Cash D.1, 2, 3**: Keys for the cash discount rates for the payment term. You can specify up to 3 different keys. This way, you can define scaled payment terms. Technical info: numeric fields, DB fields: kauf._skonto1, kauf._skonto2, kauf._skonto3
- **Charact.**: Number of the form of payment, e.g. bank debit, bank booking. You store characteristics in the system master data as payment methods. If you specify a number, the name of the characteristic is displayed in plain text. Technical info: numeric field, DB field: kauf.zahlngmerk
- **Payments**: Type and method of payment, e.g. upon delivery or by direct debit. The specifications for payment method are specified by the system. Technical info: toggle field, DB field: kauf.skontoart
- **FIN. key**: Key for transfer to financial accounting. The keys for financial accounting are entered by the system and sent to financial accounting. Technical info: alphanumeric field, DB field: kauf.fibukey
- **FinAc debtor**: Market partner's supplier number, which is intended as invoice recipient. The field is pre-populated by default. Technical info: numeric field, DB field: kauf.stddebnr

**Private fields**
The private fields are used customer-specifically for additional information. They can be configured at will. The field names are set via the environment variables. The two upper lines are numeric field; the two lower lines are free text fields.
Technical info: numeric fields, alphanumeric fields, DB fields: kauf.private_long1, kauf.private_long2, kauf.private_char1, kauf.private_char2

**Further options**
- **Check**: Number of the employee who checks the document. If the field is filled, the documents will only be released after checking by the appropriate employee. Technical info: numeric field: DB field: kauf.kontrollmanr
- **Wind load**: Wind load in the installation location. Wind load (N/m²) is the pressure applied by direct winds onto the external surface of a building. The system uses this value to perform a plausibility check to determine whether the thickness group of the selected glass types suffice for the wind load defined. The wind load can only be specified for glass with multiple lites. Technical info: numeric field, DB field: kauf.wlast

> **Restriction check after input of wind load**
> If an appropriate entry is created for the wind load in the master data, the specified wind load is subjected to a restriction check. A note will be displayed should the restriction check reveal problems.

- **Facade zone**: Specification of the facade zone in which the lites will be installed. E.g. tall buildings or buildings on the outskirts are loaded with increased wind load.
  - **1 Edge**: For buildings with increased wind load.
  - **2 Central**: For buildings without increased wind load.
  Technical info: numerical field, DB field: kauf.bereich
- **Min IG tot.thickn., Max. IG tot.thickn.**: Minimum and maximum glass thickness for the entire IG article in millimeters. The glass thickness depends on the selected facade zone and the wind load. Technical info: numeric fields, DB fields: kauf.minszr, kauf.maxszr
- **Tight size**: Correction size in millimeters. The tight size added to the width and height of the items. For example, for a glass with the dimensions 1050 mm x 1250 mm and a tight size of 2 mm, the dimensions 1052 mm x 1252 mm are stored in the database. The value is transferred to production. If you are working with A+W Production, this value is generally ignored and the tight size is drawn from A+W Production. Technical info: numeric field, DB field: kauf.falzmass
- **Quot. status**: Status of the quotation. This field is only shown for quotations. If referenced, this field content is transferred.
  - **open**: quotation has not yet been confirmed.
  - **won**: quotation has been confirmed.
  - **lost**: inquiry has been rejected.
  - **expired**: quotation is no longer valid.
  Technical info: toggle field, DB field: kauf.angbstatus
- **Text formulas**: Number and description of the product labeling, e.g. spacer text. The text formulas must be created in the master data. Technical info: numeric field, DB field: kauf.artikennfrm

**Footer**
The fields in the footer area can only be entered on the **Items** tab. They are described for the **Purchase Order Entry - Header, Footer** tab:
- "Purchase order entry - header, footer" on page E-1585
