---
description: "US_AWEnterprise_Sales_HelpCards"
---


# A+W Enterprise Sales: Help Cards

This guide provides instructions for using the A+W Enterprise software, specifically focusing on the Sales module. It is intended for users familiar with the basic operation of the program.

---
## Introduction

The depictions in these Help Cards are based on delivery version **A+W Enterprise V 6**. Individual steps in the workflows can differ depending on the system configuration.

**Orders as Example**
Various functionalities can be started in several transaction types. In these Help Cards, they will always be shown using the example of an order.

**Key and Key Combinations**
Knowledge of program operation is assumed. In the steps, only the possible keys and key combinations are named with which a function or menu can be called up. The functions and keys possible on the open dialog can be displayed on the prompt line at the lower edge of the dialog.

## Table of Contents

### Quotation
| Help Card | Subjects |
| :--- | :--- |
| **Quick entry** | - Create quotation quickly.<br>- Create order quickly. |
| **Enter quotation** | - Enter quotation.<br>- Edit resubmission.<br>- Create manual resubmission. |

### Order
| Help Card | Subjects |
| :--- | :--- |
| **Enter header data** | - Create order. |
| **Enter order with reference** | - Enter order with reference to quotation.<br>- Enter quotation with reference to earlier order. |
| **Specify order type** | - Enter stock order.<br>- Enter parent order.<br>- Enter subsequent delivery as goodwill order. |
| **Edit properties** | - Edit shipping information.<br>- Edit invoice and print options for commercial papers.<br>- Edit field staff employee. |
| **Edit delivery address** | - Enter delivery address for order.<br>- Take over new delivery address in master data. |
| **Edit delivery plan** | - Specify delivery date for item and total quantity.<br>- Create delivery plan for partial deliveries of an item. |
| **Edit payment options** | - Edit payment options. |
| **Release order** | - Release orders of a department and/or a user.<br>- Release all orders.<br>- Check reasons for lock. |
| **Display order information** | - Check production status of the order.<br>- Check delivery date changes. |
| **Edit text in the order** | - Enter header or footer text for the order.<br>- Edit article and item text.<br>- Check article text in customer language. |
| **Edit remarks** | - Enter internal remark about order header or footer.<br>- Enter internal remark about the item or article. |
| **Attach file** | - Attach document for the customer.<br>- Attach document for the item. |

### Order item
| Help Card | Subjects |
| :--- | :--- |
| **Enter item** | - Enter order item.<br>- Add items. |
| **Edit supplier** | - Edit supplier.<br>- Edit procurement type. |
| **Replace glass** | - Edit glass in product structure.<br>- Edit installation position of glass. |
| **Enter shape** | - Enter order item with shape. |
| **Enter processing** | - Enter processing manually. |
| **Take over processings from SN file** | - Take over processings from SN file into BOM. |
| **Attach SN file** | - Take over processings from SN file into BOM.<br>- Attach copy of SN file. |
| **Compare changes to SN file** | - Edit or add processings in attached SN file.<br>- Edit or add processings in BOM. |
| **Enter item in CAD** | - Enter geometry and processings in A+W CAD Designer (Shapes), take over in item and save as SN file.<br>- Interactive entry in A+W CAD Designer (Shapes). |
| **Enter stepped glass** | - Enter stepping on multiple-layer sheet. |
| **G. bars input** | - Enter Georgian bars pattern. |
| **Edit Georgian bar grid** | - Edit Georgian bars pattern with the Georgian bar editor.<br>- Enter non-symmetrical Georgian bar structure. |
| **Spac. Offset and sealing depths** | - Enter edge deletion on IGU. |
| **Replace product** | - Replace article in several order items.<br>- Edit sheet structure in several order items. |
| **Fix item** | - Fix articles of an order item.<br>- Include fixed article in the master data. |
| **Assign declaration of performance** | - Check and/or assign declaration of performance. |
| **Enter technical values** | - Enter technical values.<br>- Generate new declaration of performance. |

### Price calculation
| Help Card | Subjects |
| :--- | :--- |
| **Edit item conditions** | - Check and edit item price. |
| **Edit item prices** | - Edit item prices. |
| **Footer discount, edit surcharge** | - Check and/or edit discounts and surcharges.<br>- Enter order specific discount. |
| **Check production costs** | - Check production costs in the order.<br>- Check production costs in the quotation. |
| **Price report for LSG** | - Check price calculation for LSG item. |

### Invoice
| Help Card | Subjects |
| :--- | :--- |
| **Create invoice manually** | - Create and book invoice.<br>- Create partial invoice. |
| **Generate invoices automatically** | - Generate and book several invoices.<br>- Generate collective invoice. |
| **Book invoice** | - Book invoice. |
| **Print invoice** | - Print single document.<br>- Print several documents. |
| **Enter credit note** | - Enter credit note.<br>- Enter complaint details. |

### Additional topics
| Help Card | Subjects |
| :--- | :--- |
| **Search for transaction** | - Search for orders for the current day.<br>- Search for orders for a customer.<br>- Search for orders for a date and/or user. |
| **Transaction change** | - Edit route.<br>- Edit delivery date.<br>- Set or delete cancellation status. |

---

## Quotation: Quick entry (VK 01-001)

### Objective of this activity
- Enter order quickly.
- Enter quotation quickly.

### Prerequisites
- Quick entry must be configured.
- Master data must be adapted.

[Image: Screenshot of the Quick Entry dialog in A+W Enterprise, showing fields for customer information, shipping information, and address details.]

### Workflow
1.  Select the **Sales > Quick entry** menu. The Order entry dialog opens with **Search market partner**.
2.  Select and take over customer.
3.  Check and fill mandatory fields `*`.
4.  In the Shipping address area, select a delivery address with [Search address]. If necessary, create a new address with [New address].
5.  Change to the **Items** tab.
6.  In the **ProductCode** field, select or enter the item number.
7.  Add item data.
8.  Repeat steps 6 and 7 for additional items if necessary.
9.  Change to the **Overview** tab.
10. Create the order with [Save].

### Enter quotation quickly
11. Perform steps 1 to 9.
12. Create a quotation with [Save as quotation]. A dialog for the quotation reason opens.
13. Enter a reason and take over with [OK].
14. Confirm the reference to the new quotation number.

### Next step
- Create another order using the quick entry.
- Close the dialog with `<Esc>`.

---

## Quotation: Enter quotation (VK 01-002)

### Objective of this activity
- Enter quotation.
- Edit resubmission.
- Create manual resubmission.

### Prerequisites
- Automatic resubmission is set up: **System > Document Management > Resubmission mode**.

### Additional information
- Delete resubmission: Press `<F7>`.
- Automatic resubmissions are set up per activity type.
- Enter manual resubmission for order: **Date > `<Shift>+<F4>` > Resubmission** field.
- See also:
    - Enter item
    - Search for transaction

[Image: Screenshot of the Quotation entry dialog, with an overlay of the Resubmission dialog showing presentation dates and remarks.]

### Workflow

**Enter and Save Quotation**
1.  Select the **Sales > Quotation entry** menu. The **Quotation entry** dialog opens.
2.  Select customer.
3.  In the **Date** field, if necessary, enter a possible delivery date. (Alternative: The delivery date is determined by A+W Production and written back.)
4.  Enter items and save the quotation.

**Edit resubmission**
5.  Select the **Sales > Resubmission** menu. The **Resubmission** dialog opens.
6.  Select the current quotation and:
    - Edit the date for resubmission.
    - Enter a remark.

**Create manual resubmission**
7.  Select the **Sales > Resubmission > `<F6>`** menu. A new row is added at the end of the list.
8.  Fill out the fields in the new row:
    - Enter date.
    - Select resubmission type and enter text.
    - Select employee.
9.  Close the dialog with `<End>`.

---

## Order: Enter header data (VK 02-001)

### Objective of this activity
- Create order.

### Prerequisites
- Master data has been entered completely.

### Additional information
- Quotations are entered in the same way as orders: **Sales > Quotation entry** menu.
- See also:
    - Enter quotation
    - Enter order with reference
    - Enter item

[Image: Screenshot of the Order entry dialog in A+W Enterprise, focused on the header data fields like Order number, Customer, Date, and Route.]

### Workflow
1.  Select the **Sales > Order entry** menu. The **Order entry** dialog opens.
2.  **Order** field: Jump to the **Customer** field with `<Enter>`. The next free transaction number is added to the **Order** field.
3.  Enter or select customer number.
4.  Go through the following fields with `<Enter>` and check them.
5.  **Ref.** field: If necessary, select a quotation with `<F9>` or enter the number.
6.  **Date** field: If necessary, enter a possible delivery date. (Alternative: The delivery date is determined by A+W Production and written back.)
7.  **Route** field: Check and change the default route from the customer master data if necessary.
8.  Check and add data in the other fields.
9.  Select or enter an object number in the **Contract** field.
10. Save header data with `<Enter>`.

---

## Order: Enter order with reference (VK 02-002)

### Objective of this activity
- Enter order with reference to a quotation.
- Enter quotation with reference to an earlier order.

### Prerequisites
- Master data has been entered completely.

### Additional information
- A quotation with reference to an order is entered in the same way.
- See also:
    - Search for transaction
    - Enter item

[Image: Screenshot showing the 'Search reference document' dialog to find a quote, with a confirmation pop-up asking whether to import the complete document or only header data.]

### Workflow
1.  Select the **Sales > Order entry** menu. The **Order entry** dialog opens.
2.  **Order** field: Jump to the **Customer** field with `<Enter>`. The next free transaction number is added to the **Docum.** field.
3.  Enter or select customer number.
4.  Go through the following fields with `<Enter>` and check them.
5.  **Ref.** field: Press `<F9>`. The **Search reference document** dialog opens.
6.  **Docum.** field: Select the entry **Quote** with `<F9>` and start the search.
7.  Mark and take over the quotation.
8.  Confirm the query for the takeover of the data:
    - **[Yes]**: Take over header and item data.
    - **[No]**: Only take over the header data.
9.  If necessary, confirm the query about discounts.
10. Check and add remaining header data if necessary.
11. Check and add items if necessary.
12. Save the order and exit.

---

## Order: Specify order type (VK 02-003)

### Objective of this activity
- Enter a stock order.
- Enter a parent order.
- Enter a subsequent delivery as a goodwill order.

### Prerequisites
- Order entry is open.

### Additional information
- All order types are entered the same way.
- To enter an order without a price display: **Sales > Order entry (no prices)**. The sales prices will be calculated when the order is printed.
- See also: Enter credit note

[Image: Screenshot of the 'Order entry' screen with the 'Order types' dialog open, showing options like 'Regular order', 'Free-of-charge order', etc.]

### Workflow
1.  Enter order header data up to the **Ref.** field.
2.  Select the order to which the subsequent delivery refers.
3.  Fill in fields up to the **Receipt** field.
4.  **Receipt** field: Press `<Ctrl>+<F12>`. The **Order types** dialog opens.
5.  Select an order type, e.g., **Free-of-charge order**. The **Free-of-charge order** dialog opens.
6.  Enter the item and exit the entry.
7.  Confirm the reference to a zero amount with [No].
8.  If necessary, select reasons for the complaint.
9.  Confirm details with `<Enter>` and take over.
10. Confirm queries.
11. Confirm the query about the completeness of the order with [Yes].
12. Confirm the query about release with [Yes].

---

## Order: Edit properties (VK 02-004)

### Objective of this activity
- Edit shipping information.
- Edit invoice and print options for commercial papers.
- Edit field staff employee.

### Prerequisites
- Order entry is open.
- Order is entered.

### Additional information
- Changes to the fields **Delivery** and **Direct desp.** influence the entire order and purchase order flow.
- Changes to the invoice options can activate surcharges, e.g., a rush order.
- See also: Edit payment options

[Image: Screenshot of the 'Properties' tab in the Order entry dialog, displaying sections for Staff allocation, Shipping information, and Invoice and print options.]

### Workflow
1.  Change to the **Properties** tab.
2.  Edit data in the **Staff allocation** area, e.g.:
    - **Ordered by** field: Change customer contact.
    - **PO date** field: Check and change the date if necessary.
3.  Edit data in the **Shipping information** area, e.g.:
    - **Packing type** field: Select a packing type, e.g., Box.
    - **Rack load** field: Select a sorting sequence for packing, e.g., Reference.
4.  Edit print options for commercial papers, e.g.:
    - **Glazing** field: Indicate the price of the glazing, e.g., *Calculate in item*.
    - **Print product text** field: Y = print texts.
    - **Print shapes** field: Y = print shape sketch.
    - **Suppress item prices** field: Y = do not print item prices.
5.  Change to the order header with `<End>`.
6.  Continue entry or save the order and exit.

---

## Order: Edit delivery address (VK 02-005)

### Objective of this activity
- Enter a delivery address for the order.
- Take over a new delivery address into master data.

### Prerequisites
- Order entry is open.
- Order header has been entered.

### Additional information
- Changes only affect the current order.

[Image: Screenshot of the 'Addresses' tab in the Order entry dialog, showing the customer's main address and the shipping address for the current order.]

### Workflow
1.  Change to the **Addresses** tab.

**Select Existing Address**
2.  Select an address from master data: press `<Shift>+<F8>`. The addresses from the customer master data are displayed.
3.  Select and take over the address.

**Search for an Address**
4.  Start address search: Press `<Ctrl>+<L>`. The **Search address** dialog opens.
5.  Search for and take over the address.

**Enter Alternative Delivery Address for the Order**
6.  Select **`<F4>` > Addresses > New shipping address**. The dialog for entering the address data is displayed.
7.  Enter all required data.
8.  Take over the new address into the order with [OK] and save.

**Take Over New Address into Customer Master Data**
9.  Enter the new delivery address.
10. Start the takeover with `<F3>` and confirm the query.
11. Take over the new address into the order with [OK] and save. The delivery address is saved for the order.
12. Continue entry or save the order and exit.

---

## Order: Edit payment options (VK 02-006)

### Objective of this activity
- Edit payment options.

### Prerequisites
- Order entry is open.
- Order header has been entered.

### Additional information
- The payment options are pre-populated with data from the customer master data.
- Changes only affect the current order.
- **Next step**: Enter item.

[Image: Screenshot of the 'Miscellaneous' tab in the Order entry dialog, focusing on Complaint information, Payment options, and Private fields sections.]

### Workflow
1.  Change to the **Miscellaneous** tab.
2.  Enter data for a complaint in the **Complaint information** area, e.g.:
    - **Type** field: Select a complaint type, e.g., *Packing*.
    - **Place** field: Select a complaint location, e.g., *Shipping*.
3.  Enter data for payment terms in the **Payment options** area, e.g.:
    - **Pay.term** field: Enter the number of days until the due date, e.g., 30 days.
    - **Cash d. 1, 2, 3**: Select cash discount records for graduated payment dates.
    - **Charact., Payments** fields: Select the type of payment, e.g., *Bank transfer*.
4.  **Private fields** area: If necessary, specify the date of the goods receipt from purchasing.
5.  Change to the order header with `<End>`.
6.  Continue entry or save the order and exit.

---

## Order item: Enter item (VK 03-001)

### Objective of this activity
- Enter an order item.
- Add items subsequently.

### Prerequisites
- Item master data is available.
- Order entry is open.
- Order header has been entered.

### Additional information
- See also:
    - Edit supplier
    - Enter stepped glass
    - Enter shape
    - G. bars input
    - Enter processing

[Image: Screenshot of the 'Items' tab in the Order entry dialog, showing a list of entered items with details like quantity, width, height, and price.]

### Workflow
1.  Use `<Enter>` to change from the order header to the **Items > General** tab.
2.  **Article** field: Select an item by:
    - Entering the article number.
    - Starting an article search with `<F9>`.
    - Depending on the item data, various input fields are displayed.
3.  Enter the quantity and jump to the next field with `<Enter>`.
4.  Enter dimensions or select a variant if necessary. For IGU glass, also specify the dimension for the spacer (CAV).
5.  **Comm** field: If necessary, change the commission key with `<F9>`.
6.  **Stype** field: Check the procurement type and change if necessary. The values for the fields **MU/pc**, **kg/pc** and the prices are calculated and filled.

### Add additional item
7.  - **Insert at the end**: Press `<F6>`.
    - **Insert over marked items**: Press `<Shift>+<F6>`.
    - **Copy item**: Mark the item and press `<Alt>+<C>` or [Copy item].
    - When entering an item with the same article number, the BOM structure is taken over.
8.  Complete the entry in the **Price** field:
    - `<End>`: Save the order and check footer data.
    - Use `<F2>` to change to the order header.
9.  Continue entry or save the order and exit.

---

## Order item: Edit supplier (VK 03-002)

### Objective of this activity
- Edit supplier.
- Edit procurement type.

### Prerequisites
- Suppliers are created.
- Order entry is open.
- Item is entered.

### Additional information
- With the specification of a supplier, the procurement type is always changed to **purchase order**.
- With the change of the procurement type to **Purchase order**, a supplier must always be specified.

[Image: Screenshot of the 'Items' tab in the Order entry dialog. The fields for 'Supplier' and 'Del. time' are visible next to the item graphic, indicating a purchase order item.]

### Workflow
1.  Change to the **Items > General** tab.
2.  **Qty.** field: Press `<Shift>+<F12>`. Next to the graphic, the fields **Supplier** and **Del. time** are displayed.
3.  **Supplier** field: Enter a supplier number or select with `<F9>`.
4.  **Del. time** field: Enter the delivery time in days.
5.  Move on with `<Enter>` and confirm the queries. The supplier can be taken over for the whole order, for the following items, or only for the current item.
6.  Continue entry or save the order and exit.

### Edit procurement type
7.  Enter the item and enter the supplier.
8.  **Stype** field: Page to the procurement type with the `<Spacebar>`, e.g., P.O.
9.  Save the item and continue entry.

---

## Order item: Replace glass (VK 03-003)

### Objective of this activity
- Edit glass in a product structure.
- Edit the assembly position of glass.

### Prerequisites
- Order entry is open.
- An item is entered with quantity and dimensions.

### Additional information
- Replacement glass can be entered in IGU and LSG sheets.
- Installation items are counted from outside to inside.

[Image: Two side-by-side screenshots of the 'BOM view'. The left shows the original product structure of an IGU, and the right shows the structure after one of the glass panes has been replaced with a different type.]

### Workflow

**Replace Glass**
1.  Navigate to **Items > General** tab and enter an IGU article.
2.  Open the BOM view dialog: [BOM].
3.  **Current BOM level** tab: Mark a subpart and click [BOM]. In the BOM tree, the current BOM level is marked.
4.  **Current BOM level** tab: Change the article number of the replacement glass.
5.  Depending on the glass, supply the following details:
    - **Strct** field: Select structure.
    - **Supplier** field: Select supplier.
    - **Print** field: Select print option for production or commercial papers.
6.  Take over changes with [OK]. On the **Current BOM level** tab, all subparts are displayed.

**Change Assembly Position**
7.  **AP** field: Enter the number of the assembly position for the replacement glass. The number of the second glass is assigned automatically.

**Replace Structure Position**
8.  Open the BOM for the replacement glass.
9.  **AP** field: Enter the number of the assembly position of the glass.
10. Close the BOM display dialogs with [OK]. The order entry dialog is displayed again.
11. Confirm the query about price calculation.
12. Save changes.
13. Continue entry or save the order and exit.

---

## Order item: Enter shape (VK 03-004)

### Objective of this activity
- Enter an order item with a shape.

### Prerequisites
- A shape catalog is installed, e.g., The A+W shape catalog.
- Order entry is open.

### Additional information
- For the price calculation, the dimensions of the circumscribed rectangle from the item entry are used.

[Image: Screenshot of the Order entry screen with the 'Shapes-dimensions' dialog open, allowing the user to input dimensions for a custom glass shape.]

### Workflow
1.  Change to the **Items > General** tab.
2.  Enter the item.
3.  **Width** field: Press `<Ctrl>+<F12>`. The **Shape** field is displayed next to the graphic.
4.  Enter a shape number or select one with `<F2>`. The **Shapes-dimensions** dialog opens.
5.  Enter dimensions for all lengths displayed. Heed restrictions, e.g., for W (width) and H (height).
6.  Take over details with [OK]. The item is marked with the shape icon. The shape is displayed to scale in the graphic area.
7.  Save the item.
8.  Continue entry or save the order and exit.

---

## Order item: Enter processing (VK 03-005)

### Objective of this activity
- Enter processing manually.

### Prerequisites
- Order entry is open.
- Processing items are created.

### Additional information
- All processings are entered in the same way.
- In the case of asymmetrical cutouts, enter each cutout as a separate processing.
- For IGU sheet processing (e.g., screen printing), enter separately for each sheet.
- To open the BOM: in the **Item** field, press `<Shift>+<F5>`; in the **Quantity** field, press `<F5>`.
- See also: Take over processings from SN file

[Image: Screenshot of the 'BOM view' dialog, showing parameters for a corner cutout processing, including distances, radii, and a visual sketch.]

### Workflow
1.  Navigate to **Items > General > Enter item** tab.
2.  Open the BOM view dialog: In the **Qty.** field, press `<F5>`.
3.  **BOM tree**: Select the desired level.
4.  Insert a new row: Press `<F6>`.
5.  Search for processing: [A srch].
6.  Select processing, e.g., *Proc. corners*, and take over.
7.  Enter dimensions: [Params].
8.  Mark the check boxes for the corners that should receive the same cutout.
9.  Specify values for corner cutouts:
    - Distances A and B.
    - Reference edge, e.g., *On. 1.edge*.
    - Rounding off for the cutouts *Radius int.* and *Radius ext.*
10. Check details and correct if necessary: Open the product sketch with [Sketch].
11. Take over details with [OK]. The product sketch closes.
12. If necessary, repeat steps 3 to 11 for additional processings.
13. Complete processing with [OK]. The **Order entry** dialog opens.
14. Save the item.
15. Continue entry or save the order and exit.

---

## Order item: Take over processings from SN file (VK 03-006)

### Objective of this activity
- Take over processings from an SN file into the BOM.

### Prerequisites
- A+W CAD Designer (Shapes) is installed.
- SN exchange rules are defined: **Master data > Keys > Products > SN exchange rules**.
- SN files are available.
- Path is set up.

### Additional information
- If no file is attached and saved, the BOM structure can only be changed if the entire action sequence is repeated.
- See also:
    - Attach SN file
    - Compare changes to SN file

[Image: Screenshot of the Order entry screen and the 'Item processings' dialog, which shows a list of processings (e.g., polished edges, drill holes) imported from a file.]

### Workflow
1.  Go to **Sales > Order entry > Enter item**.
2.  Enter quantity, width, and height.
3.  **Height** field: Press `<Ctrl>+<E>`. Windows Explorer opens with the pre-defined path.
4.  Mark the SN file in Windows Explorer and confirm with [Open].
5.  Confirm the query for the synchronization of the BOM with [Yes]. The A+W CAD Designer (Shapes) program opens.
6.  In CAD Designer: Check processings and change if necessary.
7.  **File** menu: Select **Exit TOE**. The A+W CAD Designer (Shapes) program is closed. The AWE BOM is compared to the CAD file. The processings are taken over. The SN file is not attached.
8.  Use `<Tab>` to jump to the next field. The **Item processings** dialog opens.
9.  Check the processings and close the dialog with [OK].
10. Save the item.
11. Continue entry or save the order and exit.

---

## Order item: Attach SN file (VK 03-007)

### Objective of this activity
- Take over processings from an SN file into the BOM.
- Attach a copy of the SN file.

### Prerequisites
- A+W CAD Designer (Shapes) is installed.
- SN exchange rules are defined: **Master data > Keys > Products > SN exchange rules**.
- SN files are available.
- Path is set up.

### Additional information
- If in A+W Enterprise no SN exchange rule is stored for the processing entered in the SN file, a selection dialog for the assignment opens. This assignment is only valid for the current item.
- See also: Compare changes to SN file

[Image: Screenshot of the 'Properties' tab for an order item, where the 'CAD file' field shows the path to the attached SN file.]

### Workflow
1.  Go to **Sales > Order entry > Enter item**.
2.  Enter quantity, width, and height.
3.  **Height** field: Press `<Ctrl>+<E>`. Windows Explorer opens with the pre-defined path.
4.  Mark the SN file in Windows Explorer and confirm with [Open].
5.  Confirm the query for the synchronization of the BOM with [Yes]. The A+W CAD Designer (Shapes) program opens.
6.  In CAD Designer: Check processings and change if necessary.
7.  **File** menu: Select **Exit TOE and save file**. The A+W CAD Designer (Shapes) program is closed. The processings are taken over into the BOM of the item. The SN file is updated.
8.  Confirm queries and check notes.
9.  Use `<Tab>` to jump to the next field. The **Item processings** dialog opens.
10. Check processings and close the dialog with [OK].
11. **Properties** tab: Check the path and name of the attached SN File. The SN file is saved as a copy in the TOE directory.
12. Save the item.
13. Continue entry or save the order and exit.

---

## Order item: Compare changes to SN file (VK 03-008)

### Objective of this activity
- Edit or add processings in an attached SN file.
- Edit or add processings in the BOM.

### Prerequisites
- A+W CAD Designer (Shapes) is installed.
- SN exchange rules are defined: **Master data > Keys > Products > SN exchange rules**.
- SN files are available.
- Path is set up.
- Work with A+W CAD Designer (Shapes) is familiar.

### Additional information
- A complete description is in the A+W CAD Designer (Shapes) manual.

[Image: A composite screenshot showing the A+W CAD Designer interface with a technical drawing, alongside the BOM display dialog in A+W Enterprise, illustrating the comparison and editing of processings.]

### Workflow
1.  Go to **Sales > Order entry** and select the item with the SN file to select.
2.  **Width** field: Press `<Ctrl>+<E>`.

**Edit processings in A+W CAD Designer (Shapes)**
3.  The A+W CAD Designer (Shapes) program opens. In CAD Designer, edit processings, e.g., edge processing.
4.  **File** menu: Select **Exit TOE and save file**. The A+W CAD Designer (Shapes) program is closed. The processings are taken over into the BOM of the item. The SN file is attached.

**Edit processings in the BOM**
5.  Mark the item and select [BOM]. The BOM display dialog opens, which in turn opens A+W CAD Designer (Shapes).
6.  Edit or add processings, e.g., a speaker's hole.
    - See Help Card: **Enter processing**
7.  Save changes and close the dialog. The processings are taken over into the BOM of the item. The SN file is updated.
8.  Save the item.
9.  Continue entry or save the order and exit.

---

## Order item: Enter item in CAD (VK 03-009)

### Objective of this activity
- Enter geometry and processings in A+W CAD Designer (Shapes), take over in the item, and save as an SN file.
- Interactive entry in A+W CAD Designer (Shapes).

### Prerequisites
- A+W CAD Designer (Shapes) is installed.
- SN exchange rules are defined: **Master data > Keys > Products > SN exchange rules**.
- Path is set up.
- Work with A+W CAD Designer (Shapes) is familiar.

### Additional information
- A complete description is in the A+W CAD Designer (Shapes) manual.

[Image: Screenshot of the A+W CAD Designer interface, showing a technical drawing being created, which is linked to an order item in A+W Enterprise.]

### Workflow
1.  Go to **Sales > Order entry** and enter an item with the item number and quantity.
2.  **Width** field: Press `<Ctrl>+<E>`. A+W CAD Designer (Shapes) opens.
3.  Draw the CAD construction of the sheet with dimensions and necessary processings.
4.  **File** menu: Select **Exit TOE and save file**. The A+W CAD Designer (Shapes) program is closed. The BOM is generated in the item. The SN file is saved in the TOE directory and attached. Changes are possible (see VK 03-008).
5.  Save the item.
6.  Continue entry or save the order and exit.

---

## Order item: Enter stepped glass (VK 03-010)

### Objective of this activity
- Enter stepping on a multiple-layer sheet.

### Prerequisites
- Order entry is open.
- An item of type *Stepped* is created in the master data.
- For steps on a shape: Shape is entered.

### Additional information
- Positive values for the steps are deducted from the edge length; negative values are added.
- For steps on LSG, there is a side view available in the product sketch.

[Image: Screenshot of the 'Stepped entry (relevant elements)' dialog, used to define step reductions on the edges of an IGU, with a corresponding product sketch.]

### Workflow
1.  Navigate to the **Items > General > Enter item** tab. Example: Enter stepping on an IGU sheet.
2.  Enter the IGU article.
3.  **Width** field: Press `<Ctrl>+<F10>`. The **Stepped entry (relevant parts)** dialog opens.
4.  Select glass for steps: In field **C**, assign stepping with `Y` and press `<F3>` and [OK]. The **Shapes-dimensions** dialog opens.
5.  Enter dimensions for height and width.
6.  Enter dimensions for the steps per edge.
7.  Take over dimension specifications with `<Enter>`.
8.  With multiple IGU: Repeat steps 4 to 7 for the next glass.
9.  Take over values from the **Stepped entry (relevant parts)** dialog.
10. **Stype** field: Open the BOM display with [BOM]. The BOM display dialog opens.
11. Change to the **Production sketch** tab and check entries.
12. If necessary, enter and save spacer and other details.
13. Continue entry or save the order and exit.

---

## Order item: G. bars input (VK 03-011)

### Objective of this activity
- Enter a Georgian bars pattern.

### Prerequisites
- Georgian bars items are created.
- Order entry is open.

### Additional information
- For a complex Georgian bar pattern, attach a sketch from A+W CAD Designer (Bars).
- See also:
    - Attach file
    - Edit Georgian bar grid

[Image: Screenshot of the 'G. bars input' dialog, where users can define the number of horizontal and vertical Georgian bars to create a grid pattern within an IGU.]

### Workflow
1.  Change to the **Items > General** tab.
2.  Enter the item completely with the IGU sheet.
3.  **CAV** field: Check the spacer and change if necessary.
4.  **CAV** field: Press `<Shift>+<F8>`. The **G. bar input** dialog opens.
5.  **G. bars** tab:
    - **GeorgBr** field: Enter or select the item number for the Georgian bar.
    - Fields **ho** and **ve**: Enter the number of horizontal and vertical Georgian bars.
    - **Symmetry** field: Select `F-Sym` or `D-Sym`.
    - If necessary, select color variants with the **Color** field.
    - If necessary, select a supplier with the **Supplier** field.
6.  **Add. info** tab: If necessary, change the procurement type.
7.  With multiple IGU:
    - **IF** field: Select the frame for assembly.
    - Repeat details for the next CAV (frame).
8.  Take over data with [OK]. The item is marked with the Georgian bar icon. The Georgian bar grid is displayed to scale in the graphic area.
9.  Continue entry or save the order and exit.

---

## Order item: Edit Georgian bar grid (VK 03-012)

### Objective of this activity
- Edit a Georgian bars pattern with the Georgian bar editor.
- Enter a non-symmetrical Georgian bar structure.

### Prerequisites
- Order entry is open.
- You are familiar with the Help Card "G. bars input".

### Additional information
- Max. 11 Georgian bars are transferred to production.
- The prices are calculated for max. 2 different Georgian bar items.
- For complex Georgian bar patterns (e.g., Suns), attach a sketch from A+W CAD Designer (Bars).
- See also:
    - Attach file
    - G. bars input

[Image: Screenshot of the Georgian bar editor, allowing for precise adjustment of the grid by editing drill points and clearing fields.]

### Workflow
1.  Change to the **Items > General** tab.
2.  Enter the item completely with the IGU sheet.
3.  **CAV** field: Press `<Shift>+<F8>`. The **G. bar input** dialog opens.
4.  Enter the number of horizontal and vertical Georgian bars.
5.  **Symmetry** field: Select `F-Sym+E` or `D-Sym+E`.
6.  Open the Georgian bar editor: [Editor].
7.  Remove an omitted Georgian bar: Click on the Georgian bar in the diagram.
8.  Discard changes: Restore the original Georgian bar pattern with [New pattern].
9.  Take over changes with [OK].

### Edit Georgian bar item
10. Edit clear fields: Press `<Shift>+<F8>` and enter a value.
11. Edit drill points:
    - Press `<Shift>+<F12>` and enter a value.
    - Open table: Press `<Shift>+<F11>` and edit values.
    - Take over changes with `<Enter>`.
12. Take over the Georgian bar pattern with [OK]. The Georgian bar editor closes. The item is marked with the Georgian bar icon and the pattern is displayed in the graphic area.
13. Continue entry or save the order and exit.

---

## Order item: Spac. Offset and sealing depths (VK 03-013)

### Objective of this activity
- Enter edge deletion on an IGU.

### Prerequisites
- The module is configured in the system.

### Additional information
- Dimensions for spacer offset and sealing depths deviate only 1-2 mm from one another.

[Image: Screenshot showing the 'Dimensions of individual BOM elements' dialog and the 'Sealing depths' dialog, used for defining spacer offsets and sealing on an IGU.]

### Workflow
1.  Navigate to the **Items > General > Enter item** tab.
2.  **Price** field: Press `<F3>`. The **Dimensions of individual BOM elements** dialog opens.
3.  **BOM**: Mark the **Inner frame** level and select [Spac. offset]. The **Spac. offset(frame thickness)** dialog opens.
4.  Enter dimensions on all edges.
5.  **BOM**: Mark the **Thiokol** level and select [Sealing]. The **Sealing depth** dialog opens.
6.  Enter dimensions on all edges.
7.  Take over details with `<Enter>`.
8.  Confirm queries about price calculation.
9.  Save changes with `<End>`. The **Dimensions of individual BOM elements** dialog closes. The item is displayed with the updated price.
10. Continue entry or save the order and exit.

---

## Order item: Replace product (VK 03-014)

### Objective of this activity
- Replace an article in several order items.
- Edit the sheet structure in several order items.

### Prerequisites
- Order entry is open.
- Several items with identical BOM are entered.

### Additional information
- Product replacement for several items affects only items with the same BOM number.

[Image: Screenshot of the 'Product replacement for items' dialog, which allows replacing a product (e.g., one type of IGU with another) across multiple selected items.]

### Workflow

**Replace Product**
1.  **Items > General** tab: Select **`<F4>` > Product details > Product replacement**. The **Product replacement for items** dialog opens.
2.  **Type** field: Specify the BOM number from the **BMno** item column.
3.  Specify the replacement product.
4.  Confirm replacement with [Start].
5.  Confirm queries. The items are displayed with the new item number and a new BOM number.

**Edit Sheet Structure**
6.  Step 2: **Specify Replacement product**: specify the old article number.
7.  **Favor.structure** field: Change one or several items.
8.  Confirm replacement with [Start].
9.  Confirm queries up to the query whether the replacement should apply for all items.
10. Confirm the query "Does the product replacement apply to all items..." with [No]. The **Product replacement for items** dialog opens.
11. **New** field: Deselect all items with `N` in which the product should not be replaced.
12. Confirm replacement with [Start]. The dialog closes. The items are displayed with the old item number and a new BOM number.

---

## Order item: Fix item (VK 03-015)

### Objective of this activity
- Fix articles of an order item.
- Include a fixed article in the master data.

### Prerequisites
- Order entry is open.
- Order and item are entered.

### Additional information
- The employee right to write a fixed item back to the item master data must be granted.
- Fixed items written back to the master data can be recorded generally according to the details or customer-specifically as an item.

[Image: Screenshot showing the 'Article details for dimensioned variants' dialog, which appears when fixing an item to save it as a new article in the master data.]

### Workflow

**Fix an Item in an Order**
1.  Change to the **Items > General** tab.
2.  Enter the item completely.
3.  **Price** field: Press `<Shift>+<F8>`.
4.  Confirm the query with [Yes]. The item is marked with a yellow asterisk.
5.  If needed, enter additional items or mark them for fixing.

**Take over fixed article into the master data**
6.  Save the order with `<End>` and confirm the query. The **Article details for dimensioned variants** is displayed for the first fixed item.
7.  **Article (new)** field: Enter a new item number.
8.  Check pre-populated fields and enter deviating information if necessary, e.g.:
    - Specify customers if the new item is a customer-specific product.
    - Specify a customer-specific item number and designation.
    - Specify prices.
9.  Save details with `<End>`. The item is marked with a green asterisk.
10. If necessary, repeat steps 7 to 8 for each fixed item.
11. Save changes. The item is saved under the number entered in the master data.

---

## Order item: Assign declaration of performance (VK 03-016)

### Objective of this activity
- Check and/or assign a declaration of performance.

### Prerequisites
- An IGU item is entered completely.

### Additional information
- All header data for the declaration of performance is printed on the document.
- To create a declaration of performance according to product structure, see: Enter technical values.

[Image: Screenshot of the Order entry screen with the 'Perform. descrip.' (Performance description) dialog open, allowing a user to assign a Declaration of Performance (DOP) document to an item.]

### Workflow
1.  Go to **Sales > Open transaction** and mark the item.

**Take over declaration of performance from master data**
2.  **Properties** tab > **DOP Number** field: Press `<Ctrl>+<R>`. The identifier of the DOP is displayed in the **DOP number** field.

**Edit assigned DOP**
3.  **Properties** tab > **DOP number** field: Press `<Ctrl>+<K>`. The **Perform description** dialog opens.
4.  Search for and select the document.
5.  Confirm assignment with [OK].
6.  Take over data with `<End>`. The identifier of the new DOP is displayed in the **DOP number** field.
7.  Save the order.

---

## Order item: Enter technical values (VK 03-017)

### Objective of this activity
- Enter technical values.
- Generate a new declaration of performance.

### Prerequisites
- An IGU item is entered completely.

### Additional information
- All header data for the declaration of performance is printed on the document.
- At least one check box for the services must be marked for output in order to generate a declaration of performance.
- The A+W SLT interface for external calculation must be configured.

[Image: Screenshot of the 'Calc. technical values' dialog, which has tabs for 'Main data for decl. of performance' and 'Declared Services', used to input and calculate technical properties like U-value and light transmission.]

### Workflow
1.  Go to **Sales > Open transaction** and mark the item.
2.  **Properties** tab > **DOP number** field: Press `<Ctrl>+<T>`. The **Calc. technical values** tab opens.
3.  **Main data for decl. of performance** area: Enter header data for the declaration of performance.
4.  **Declared Services** tab: Fill in the fields for the confirmed services. Fields with `*` can be filled via the A+W SLT interface.
5.  Mark the check boxes for data that should be output.
6.  If necessary, start the determination of the technical services: Press [Ext.Calc.] or `<F3>`.
7.  Take over data with [OK].

---

## Order: Edit delivery plan (VK 02-007)

### Objective of this activity
- Specify a delivery date for an item and total quantity.
- Create a delivery plan for partial deliveries of an item.

### Prerequisites
- Order entry is open.
- The customer allows partial delivery.

### Additional information
- Delivery notes are created depending on the configuration in the shipping planning.
- **Next step**: Create delivery note and plan shipping.

[Image: Screenshot of the 'Deliv.plan' dialog, which shows how a single order item's quantity can be split into multiple partial deliveries with different dates and quantities.]

### Workflow
1.  In the Order, select **`<F4>` > Delivery schedule**. The **Deliv. plan** dialog opens.
2.  **Deliv. date** field: Specify the delivery date.
3.  **Route** field: If necessary, enter an alternative route.
4.  Repeat steps for all items.
5.  Save changes with [OK].

### Partial delivery of an item
6.  **Scheduled** field: Specify the partial quantity. A new row with the remaining quantity is inserted.
7.  **Deliv. date** field: Specify the delivery date for the remaining quantity.
8.  **Route** field: If necessary, select a route for the remaining quantity.
9.  Save changes with [OK].

---

## Price calculation: Edit item conditions (VK 04-001)

### Objective of this activity
- Check and edit item price.

### Prerequisites
- Prices and conditions are created in the master data.

### Additional information
- Changed conditions will not be written back to the master data of the conditions.

[Image: Screenshot of the 'Conditions for PCD-BASIC GLASS' dialog, where users can manually adjust prices, surcharges, and discounts for a specific item.]

### Workflow
1.  Change to the **Items > General** tab, e.g., in an IGU item.
2.  Place the cursor in the **Price** field.
3.  Click the **[%]** icon on the toolbar. The **Conditions (glass type)** dialog opens.
4.  Edit the matrix assignment or basic price.
5.  Enter surcharges and discounts.
6.  Take over with [OK].
7.  Confirm the query with [Yes]: Prices are recalculated with manual changes.
8.  Continue entry or save the order and exit.

---

## Price calculation: Edit item prices (VK 04-002)

### Objective of this activity
- Edit item prices.

### Prerequisites
- (None specified)

### Additional information
- All prices are changed in the same manner, e.g., exchange prices, Georgian bar prices, subpart prices.

[Image: Screenshot showing the 'Order prices' dialog, accessed through the context menu, which allows editing the price for a specific article type within the context of the customer.]

### Workflow
1.  Change to the **Items > General** tab.
2.  Enter the item.
3.  Select **`<F4>` > Price info > Order prices > Article prices**.
4.  The **Order prices** dialog opens.
5.  Select the condition and item, e.g., *Customer* and a *float glass*.
6.  Specify the price and price type.
7.  Take over changes with `<End>`.
8.  Confirm the query with [Yes]. Prices are recalculated in all items that contain the selected item.
9.  Save the order and exit.

---

## Price calculation: Footer discount, edit surcharge (VK 04-003)

### Objective of this activity
- Check and/or edit discounts and surcharges.
- Enter an order-specific discount.

### Prerequisites
- Discounts have been created in the master data.

### Additional information
- Discounts with negative signs are added as a surcharge.
- The sequence number specifies the sequence in which the surcharges and discounts are calculated.

[Image: Screenshot of the 'Gener. discount' dialog with the 'Detailed view discounts' pop-up, used for applying and configuring order-level discounts and surcharges.]

### Workflow

**Edit Existing Discounts**
1.  Change to the **Items > General** tab.
2.  Enter items and save.
3.  Change to the footer part: Press `<End>`.
4.  **Discount** field: Press `<F2>`. The dialog for discounts and surcharges opens.
5.  Fields **Discountable, Surcharge**: Enter values for surcharges and discounts.

**Enter order-specific discount**
6.  Insert a new row: Press `<F6>` and specify details:
    - Name.
    - Sequence number.
    - Value and discount type: Plus (+) = surcharge, minus (-) = discount.
    - Calculation type, e.g., %.
    - Calculation basis, e.g., *Prod. group* = discount for all items of this goods group.
7.  Mark check boxes:
    - **Beginning of the row**: Calculate yes/no.
    - **Field Itm**: Redistribute yes/no.
8.  Open the detail view: Press `<F5>` and add or correct data if necessary.
9.  Take over changes with [OK].
10. Save discounts and take over into the order with `<End>`.
11. Save the order and exit.
12. Confirm the query for the recalculation of the prices with [Yes].

---

## Price calculation: Check production costs (VK 04-004)

### Objective of this activity
- Check production costs in the order.
- Check production costs in the quotation.

### Prerequisites
- Material costs have been created in the master data.
- The order must have been transferred to production.
- Production transfer must be configured for quotations.

### Additional information
- The personnel and machine costs are determined and reported back if the order has been scheduled successfully in production.
- Quotations are only scheduled temporarily in A+W Production and are deleted from the batch after the costs are reported.

[Image: Screenshot of the 'Production cost calculation' dialog, showing a detailed breakdown of costs, including machinery and labor, for an order item.]

### Workflow
1.  Enter the order completely and save.
2.  Answer the query for release for production with [Yes]. The order is placed in the A+W Production order pool.
3.  After scheduling in A+W Production, open the order.
4.  Select an item: In the **Price** field, press `<Ctrl>+<F10>`. The **Production cost calculation** dialog opens.
5.  **Overview** tab: Check the calculated quantity and/or price.

### Check individual costs
6.  Mark a row in the overview and change to the **Details** tab.
7.  If necessary, repeat steps 4 to 6 for all items.

---

## Price calculation: Price report for LSG (VK 04-005)

### Objective of this activity
- Check the price calculation for an LSG item.

### Prerequisites
- The report function is configured.

### Additional information
- The price report can be saved in various formats.

[Image: Screenshot of a text-based price report displayed within the A+W Enterprise interface, detailing the conditions and calculation for an LSG item.]

### Workflow
1.  Change to the **Items > General** tab.
2.  **Price** field: Press `<Shift>+<F9>`. The **Product prices** dialog opens.
3.  Press `<Ctrl>+<L>`. The report is opened in a text editor.
4.  If necessary, save the report and exit the text editor.
5.  Close the **Product prices** dialog.
6.  Continue entry or exit the order.

---

## Order: Release order (VK 02-008)

### Objective of this activity
- Release orders of a department and/or a user.
- Release all orders.
- Check reasons for lock.

### Prerequisites
- Employee rights are granted.
- The order is in the release pool.

[Image: Screenshot showing the 'Release order' list and the 'Locking reasons for the failed release' dialog, which explains why certain orders could not be released.]

### Workflow
1.  Select the **Sales > Order release > Release** menu. The **Order release** dialog opens.
2.  Select selection criteria, e.g., department or user.
3.  Start the search with [Start]. A list of the orders is displayed.
4.  **Free** field: Select **YES**.
5.  **LL** field: Select **Y**.
6.  Trigger the change with `<F3>`.

### Release series of orders
7.  Select the first order with which all following orders should be released: Press `<Shift>+<F9>`.

### Release all orders
8.  Press `<Ctrl>+<F9>`.
9.  Confirm the queries with [Yes].

### Check reasons for lock
10. Mark an order that was not released.
11. Click [Locked list]. The **Locking reasons for the failed release** dialog opens.
12. Mark check boxes and take over with [OK].
13. Trigger the change with `<F3>`.

---

## Order: Display order information (VK 02-009)

### Objective of this activity
- Check the production status of the order.
- Check delivery date changes.

### Prerequisites
- (None specified)

### Additional information
- See also: Search for transaction

[Image: Screenshot of the 'Document info' dialog, which provides a log of activities and status changes for an order, such as 'Scheduling successful' and 'Item released'.]

### Workflow
1.  Select the **Sales > Order entry** menu. The **Order entry** dialog opens.
2.  **Order** field: Press `<F9>`. The **Find orders** dialog opens.
3.  Search for the order:
    - **Orders from** field: Specify the start number.
    - **Customer** field: Specify the customer number.
4.  Start the search with `<F3>` and take over the order from the hit list.
5.  **Quantity** field: Press `<Shift>+<F10>`. The **Order info** dialog opens.

---

## Order: Edit text in the order (VK 02-010)

### Objective of this activity
- Enter internal header or footer text for the order.
- Edit article and item text.

### Prerequisites
- Order entry is open.
- The item is entered completely.

### Additional information
- Texts can be saved as text modules.
- Texts are displayed in the customer's language.
- To enter article or item text, press `<F5>` in the price field.
- To enter texts for spacer, shape, product code: **`<F4>` > Texts > Special texts**.

[Image: Screenshot of the 'Text' dialog, allowing entry of header and footer text, as well as production and customer-facing text for BOM items.]

### Workflow
1.  Place the cursor in the order header or order footer.
2.  Call up text entry: **`<F4>` > Texts > Header** or **Footer text**. The **Texts** dialog opens.
3.  Select a tab.
4.  Enter free text and take over with [OK].

### Use text modules
5.  Insert a text module: [Phrases] > enter identifier > [OK].
6.  Select a text module: [Phrases] > start search > mark text module > [OK].
7.  **Forms** area: Mark the check boxes of the forms on which the text should be printed.
8.  Confirm the text with [OK].

### Check article text
9.  Press `<F5>` in the price field. The **Texts** dialog opens.
10. Check entries.

---

## Order: Edit remarks (VK 02-011)

### Objective of this activity
- Enter an internal remark about the order header or footer.
- Enter an internal remark about the item or article.

### Prerequisites
- Transaction is open.
- Remarks are stored in the master data if necessary.

### Additional information
- Notes are only displayed automatically if at least one line with priority **high** is contained.
- Remarks from the master data are also displayed in the order with `<Shift>+<F4>`.

[Image: Screenshot of the 'Remarks' dialog, used for adding internal notes to a transaction, with an option to set the priority to low or high.]

### Workflow

**Enter Remark on Order Header/Footer**
1.  In the order header or footer, press **`<Shift>+<F4>` > Remarks > Select Transaction remarks**. The **Remarks** dialog opens.
2.  Enter the remark.
3.  [Priority]: Select priority **high**.
4.  Save and apply the remark with [OK].
5.  Save the order.

**Enter internal remark about the item or article**
6.  **Items** tab: Select **General > `<Shift>+<F4>` > Remarks > Item remarks**.
7.  Repeat steps 2 to 4.
8.  Save changes.

---

## Order: Attach file (VK 01-012)

### Objective of this activity
- Attach a document for the customer.
- Attach a document for the item.

### Prerequisites
- The document path must be set up.
- The file must be available.

[Image: Screenshot showing the 'File allocation for case' and 'Document type allocation' dialogs, used to attach an external file to a transaction in A+W Enterprise.]

### Workflow

**Attach Document to Transaction**
1.  Go to **Sales > open transaction**.
2.  In the **Receipt**, **Invoice type**, or **Contract** field, press `<Ctrl>+<K>`. The **Document type allocation** dialog opens.
3.  Assign the document:
    - **DocType** field: Select the document type.
    - **File** field: [New]. The **File assignment for the transaction** dialog opens.
4.  Search for the file in Windows Explorer.
5.  Drag the file to the folder symbol on the **File assignment for the transaction** dialog and apply with [OK]. The **Document type allocation** dialog opens.
6.  Confirm the assignment with [OK].

**Attach document for the item**
7.  **General** tab: Mark the item.
8.  Press `<Ctrl>+<K>`.
9.  Repeat steps 3 to 6.
10. Save.

---

## Invoice: Create invoice manually (VK 05-001)

### Objective of this activity
- Create and book an invoice manually.
- Create a partial invoice.

### Prerequisites
- Orders must be released.

### Additional information
- The system can be configured so that the invoice is generated automatically together with the delivery note.
- See also:
    - Collective invoice: Generate invoices automatically
    - Print invoice

[Image: Screenshot of the manual 'Invoices' creation screen, showing order items being pulled into a new invoice, with a pop-up asking which prices to recalculate.]

### Workflow
1.  Select the menu **Sales > Invoices > Manual invoice**.
2.  Specify the customer.
3.  **Ref.** field:
    - `<F9>`: Search for and select the order.
    - `<F8>` > `<F9>` > **Apply delivery note entry** > `<F9>`: Search for and take over a delivery note.
4.  Take over data from the transaction search.
5.  **Date** field: Specify payment terms.
6.  Jump on and fill out other fields if necessary. The **New calculation of the order** dialog opens.
7.  Select the calculation if the order should be overridden.
8.  Confirm with `<Enter>`. The order is recalculated if necessary.
9.  Take over changes with [OK].

### Create partial invoice
10. **Calc** field: Specify partial quantities.
11. Save changes with [OK].
12. Check fields in the footer, e.g., discount.
13. Confirm the query for booking with [Yes].
    - **[Yes]**: The invoice is booked and transferred to FinAc.
    - **[No]**: The invoice is saved and must be booked manually later on.
    The final invoice number is set.
14. Confirm the note about the invoice number and additional queries if necessary.

---

## Invoice: Generate invoices automatically (VK 05-002)

### Objective of this activity
- Generate and book several invoices.
- Generate a collective invoice.

### Prerequisites
- The customer allows collective invoices.
- Orders must be released.

### Additional information
- The system can be configured so that the invoice is generated automatically together with the delivery note.
- See also: Print invoice

[Image: Screenshot of the 'Invoices' batch generation screen, showing a list of orders ready to be invoiced.]

### Workflow

**Generate Several Invoices**
1.  Select the menu **Sales > Invoices > Automatic release**. The **Invoices** dialog opens.
2.  **Release** field: Press `<Ctrl>+<F8>`. The dialog for importing values is displayed.
3.  Enter a start and end date for the document search.
4.  Start the import with [OK]. Orders are imported.
5.  Repeat steps 2 and 4 as needed.
6.  Jump on and change the document date if necessary.
7.  Trigger invoice generation with `<F3>`.
8.  Confirm queries as necessary.

**Generate collective invoice**
9.  **Release** field: Press `<Shift>+<F8>`. The dialog for entering the customer number is displayed.
10. Enter the customer number and apply. Orders are imported.
11. Trigger invoice generation with `<F3>`.
12. Confirm queries as necessary.

---

## Invoice: Book invoice (VK 05-003)

### Objective of this activity
- Book an invoice.

### Prerequisites
- Invoices must be generated.

### Additional information
- The system can be configured so that the invoice is printed and booked automatically together with the delivery note.

[Image: Screenshot of the 'Booking invoices' screen, where generated invoices are listed and can be selected for final booking.]

### Workflow
1.  Select the menu **Sales > Invoices > Book invoice**.
2.  **Invoice** field: Press `<Ctrl>+<F8>`. The dialog for importing values is displayed.
3.  Enter a start and end date for the document search.
4.  Start the import with [OK].
5.  Repeat steps 3 and 4 as needed.
6.  Mark the **Bk.** field.
7.  Trigger booking with `<F3>`.
8.  Confirm the query for booking with [Yes]. The invoices are booked and transferred to FinAc.

---

## Invoice: Print invoice (VK 05-004)

### Objective of this activity
- Print a single document.
- Print several documents.

### Prerequisites
- Print management is set up.
- The customers' e-mail addresses are maintained.
- The customers' fax numbers are maintained.

### Additional information
- Automatic sending: **Sales > Forms > E-Mail/Fax**.
- All documents are printed the same way, e.g., order confirmations, delivery notes, collective invoices.

[Image: Screenshot of the 'Form printing' dialog, showing options to select a form type (e.g., Invoice), filter by numbers or date, and choose a printer.]

### Workflow

**Print Single Invoice**
1.  Select the **Sales > Forms > Print** menu. The **Form type** dialog opens.
2.  Select a form type and apply with `<End>`, e.g., **Invoice**. The **Form printing** dialog opens.
3.  Select defaults and apply with `<End>`, e.g.:
    - 1 additional copy.
    - Select numbers.
4.  **Document** field: With `<F9>` select an invoice number and apply.
5.  Confirm the invoice number(s) with [OK]. The **Print on** dialog opens.
6.  Select a printer and start printing the invoice with `<Enter>`.

**Print several invoices**
7.  Select defaults, e.g., **Select numbers**, and take over with `<Enter>`.
8.  Limit order numbers, e.g., to your own orders from the previous day:
    - Enter employee number.
    - Limit entry date.
    - Select the first and last transaction.
9.  Import the order numbers from the delimited area with `<F3>`.
10. **Pri** field: Select **Y** or **N** for print output.
11. Trigger printing with `<F3>`. The **Print on** dialog opens.
12. Select a printer and start printing the invoices with `<Enter>`.

---

## Invoice: Enter credit note (VK 05-005)

### Objective of this activity
- Enter a credit note.
- Enter complaint details.

### Prerequisites
- (None specified)

### Additional information
- A credit note can be entered with reference to an order, invoice, delivery note, or another credit note.
- A credit note can be entered without a reference, e.g., for goodwill due to poor quality.
- To book a credit note: **Sales > Credit notes > Booking of credit notes**.

[Image: Screenshot of the 'Credit notes' entry screen, with dialogs for selecting 'Complaint type' and 'Complaint place' open.]

### Workflow
1.  Select **Sales > Credit notes > Entry of credit notes**. The **Credit notes** dialog opens.
2.  Select the customer.
3.  **Ref.** field: Press `<F9>`. The search reference document dialog opens.
4.  **Docum.** field: With `<F9>` select a transaction type, e.g., **Sales invoice**.
5.  Search for and take over the transaction.
6.  Check the header data of the credit note.
7.  **Items** tab:
    - **Credit note** field: Specify item quantities for the credit note.
    - **OR**
    - **Price** field: Specify prices for the credit note.
8.  Confirm changes with [OK]. A dialog for selecting **Complaint type**, **Complaint place**, etc. opens.
9.  If necessary, select reasons for the complaint.
10. Enter the complaint date.
11. Confirm details and take over with `<Enter>`.
12. Confirm queries.
13. Save the credit note.
14. Confirm the query for booking with [Yes].
    - **[Yes]**: The credit note is booked and transferred to FinAc. The final credit note number is set.
    - **[No]**: The credit note is saved and must be booked manually later on.

---

## Additional topics: Search for transaction (VK 06-001)

### Objective of this activity
- Search for orders for the current day.
- Search for orders for a customer.
- Search for orders for a date and/or user.

### Prerequisites
- (None specified)

### Additional information
- All transactions are searched for in the same way.

[Image: Screenshot of the 'Find orders' dialog, showing various search tabs and criteria like 'Orders from', 'Customer', 'User', and 'Entry date'.]

### Workflow
1.  Select the **Sales > Order entry** menu.

**Search for orders for the current day**
2.  Press `<F8>`.
3.  Mark and take over the order.

**Search for orders starting with a particular order number**
4.  **Order** field: Press `<F9>`. The **Find orders** dialog opens.
5.  **Orders from** field: Enter the start number.
6.  Start the search with `<F3>`.

**Search for orders for a customer**
7.  **Order** field: Press `<F9>`. The **Find orders** dialog opens.
8.  **Customer** field: Enter the customer number.
9.  Start the search with `<F3>`.

**Search for orders for a date and/or user**
10. **Order** field: Press `<F9>`. The **Find orders** dialog opens.
11. **Document key** tab:
    - **User** field: Enter employee number.
    - **Entry date** field: Enter date.
12. Start the search with `<F3>`.
13. Take over the order in the hit list with a double-click on the order entry.

---

## Additional topics: Transaction change (VK 06-002)

### Objective of this activity
- Edit route.
- Edit delivery date.
- Set or delete cancellation status.

### Prerequisites
- The transaction is not locked.

### Additional information
- Changes that are not forwarded to the downstream processes are marked with **Local change**. Orders with this identifier must be transferred to shipping manually, for example.

[Image: Screenshot of the 'Document alteration' dialog, which allows for bulk changes to transactions, such as editing the route, date, or cancellation status.]

### Workflow
1.  Select the **Sales > Document alteration** menu. The **Document alteration** dialog opens.
2.  **Docum.** field: Select a transaction type, e.g., **Order**.
3.  **Number** field: Press `<F9>`. The **Find orders** dialog opens.
4.  **Customer** field: Enter a customer number and start the search. The hit list is displayed.
5.  Take over the order with a double-click on the **Document alteration** dialog.
6.  Jump to the fields and change the setting, e.g.:
    - **Local correct.** field: Enter free text.
    - **Ccl** field: Set cancellation identifier.
    - **Route** field: Edit route.
    - **Date** field: Edit delivery date.
    - **Free** field: Release changes.
7.  Save changes with `<F3>`.

### Change to the transaction
8.  Open the transaction for editing with a double-click.
9.  Check data and change if necessary.
10. Save changes with [OK].
