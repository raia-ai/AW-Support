---
description: "EN_AWBusiness_Master_Data_9_9-1"
---


# Partner Management

---
## Terms

**Path:** `Master Data > Partners > Customer, Supplier > Customers, Suppliers > Functions menu > Miscellaneous group > Terms`

*Fig. B-152 Terms*

This dialog shows the discounts and individual prices that apply to this customer or supplier.

Discounts and prices for product groups are shown in blue and discounts for products in red.

> ⇨ Tutorial 1, "Discounts" on page B-341

### Discounts
This dialog shows all discounts valid for this customer. These can refer to the individual customer or to the customer group this customer belongs to.

### Individual prices
The prices in this section have been especially defined for this customer or customer group. This field is blank if no customer-specific prices have been defined.

## Customer

**Path:** `Master Data > Partners > Customer`

This program section serves to enter data that can be allocated to your customers. The actual customer data are entered in dialog Partner management.

> ⇨ "Partner Management" on page B-755

**Dialogs for customer and supplier data**
Some of the dialogs are the same for customers and suppliers. They will therefore be described just once in this document.

In addition to partner management, menu Customer offers the following entries:

*   "Discount Management (Customers, Suppliers)" on page B-803
*   "Change/Copy Discounts" on page B-811
*   "Delete Discounts" on page B-815
*   "Parameters (Customers, Suppliers)" on page B-816
*   "Customer Individual Products" on page B-818
*   "Delivery Time (Customer, Supplier)" on page B-820
*   "Projects (Customer, Supplier)" on page B-821
*   "Projects - Documents" on page B-834
*   "Purchase Hours" on page B-835
*   "Purchase" on page B-836
*   "Claims Calculation" on page B-837
*   "History of Claims" on page B-838
*   "Rounding (Customer, Supplier)" on page B-839
*   "Rounding for Customer/Supplier Groups" on page B-840
*   "Logo Position" on page B-841
*   "Different Customer/Supplier Groups" on page B-843
*   "Credit Limit Analysis" on page B-844
*   "Marginal Income Limits" on page B-846
*   "Exceeds Amount" on page B-847
*   "Calendar (Customer)" on page B-849

## Discount Management (Customers, Suppliers)

**Path:** `Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts`

Discounts can be defined for individual customers, suppliers, or for customer or supplier groups. The discounts are defined for the individual product groups and/or for the actual product.

At order entry, the program checks if a discount has been entered for the product and for the customer. If not, it will check the customer group and product group. The same applies to the input of purchase orders.

> **Dialog for customer and supplier data**
> The Discount management dialog is the same for customers and suppliers. It will therefore be described just once in this document.

Dialog Customer discounts offers the following tabs:

*   Discount Management - Discount List
*   Discount Management - Divergences
*   Discount Management - Graduated Discounts
*   Discount Management - Exchange Discounts
*   Discount Management - Table

The tabs Divergences, Grad. discount, and Exchange discounts are accessible only if you have selected a discount from the list.

**Additional information**
> ⇨ Tutorial 1, "The Function of Discounts" on page B-343
> ⇨ "PGR" on page B-566
> ⇨ "Product Management" on page B-590

### Functions menu

**Path:** `Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu`

This menu allows to copy or delete discounts.

*   **Copy discounts, Change discounts:**
    Opens the dialog Copy discounts where discounts for the selected partner can be copied or changed.
    > ⇨ "Change/Copy Discounts" on page B-811
*   **Delete discounts:**
    Opens dialog Delete discounts where discounts for the selected partner can be deleted.
    > ⇨ "Delete Discounts" on page B-815

## Discount Management - Discount List

**Path:** `Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Discount List tab`

*Fig. B-153 Customer discounts - Discount list*

This tab is used for discount input and management. To edit a discount, select it from the list. The corresponding data will be loaded automatically; the appropriate fields will be released.
Discounts for product groups are shown in blue and discounts for products in red.

Discounts can be entered for every price list and price key. You can also enter different discounts for the same product group for example by allocating them to different price lists and/or price keys.

> ⇨ Tutorial 1, "Discounts" on page B-341

### Discount for
Choose an option to define for whom the discount should be valid:

*   **Group:**
    Group discounts for customers or suppliers.
*   **Customer or supplier:**
    Discounts for individual customers or suppliers.

### Project
Discounts can be applied to a certain project. You can select only projects that are allocated to the group, the customer, or the supplier.
> ⇨ "Projects" on page B-750
> ⇨ "Projects (Customer, Supplier)" on page B-821

### Price list, Price key
Discounts are always allocated to a price list and a price key (rate).

### Discount information

**Product, Prod. grp.** The discount always refers to a certain product or product group (MPG, PSG, PGR). If you need discounts for a project with different products, you have to enter a discount for the corresponding products or product groups.

**Discount** Discount in percent.

**Default disc.** If several discounts have been entered for a product or product group, one of them must be defined as the standard discount.
- The discount has not been defined as the standard discount.
- This discount is the standard discount and will be shown by default in the corresponding fields at order entry. It can be changed.

**Valid from/to** You can restrict the validity of discounts to a certain period. This is useful if more than one discount has been defined for a customer and a product or product group. After the defined time, the discount will not be used any more for pricing, and will not be offered for selection either.

## Discount Management - Divergences

**Path:** `Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Divergences tab`

*Fig. B-154 Customer discounts - Divergences*

This tab can be used for defining rounding parameters and referring to other surcharges valid for this customer.

The fields in sections Discount for and Discount information are described in connection with the tab Discount list.

> ⇨ “Discount Management - Discount List" on page B-804

### Rounding

**Size rounding width/height** You can enter customised size roundings. At pricing, the size roundings will be taken into account in the following order: Individual prices -> Discounts -> Prices -> Products -> Partners. This means that the individual price is decisive.

**Min. quantity** Different minimum quantities for this product or product group.

### Group-based surcharges
The price list and the key for the main item will be automatically used for surcharge calculation.
You can allocate another price list and/or key for surcharge calculation. The system will check whether the corresponding price groups have been defined for the price list, the price key, and the product. If so, A+W Business will search for the appropriate entries in group surcharges. If there are no entries, a message will be issued at order entry saying that no surcharges were found.
> ⇨ "Price Groups" on page B-684
> ⇨ "Group Surcharges" on page B-687

### Group-independent surcharges
These surcharges are managed in A+W Business as Exchange surcharges. The principle is the same as for group-independent surcharges.
> ⇨ "Exchange Surcharges" on page B-666

### Miscellaneous Surcharges
Different, Miscellaneous surcharge for the customer or customer group.

### PP calculation by supplier
Purchase price calculation is usually based on all suppliers. If no standard supplier has been defined in the order, the purchase prices can be calculated based on the prices defined for the selected supplier.

## Discount Management - Graduated Discounts

**Path:** `Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Grad. discount tab`

*Fig. B-155 Customer discounts - graduated discount*

This tab is used for entering graduated discounts based on quantity limits.
The fields in sections Discount for and Discount information are described in connection with the tab Discount list.
> ⇨ “Discount Management - Discount List" on page B-804

### Scaling

**Quantity limit (unit)** Unit of the quantity limit on which the graduation is based.

**Overview** This list shows all defined grades. To add another grade please double-click on the header of the first line and select the option Add.

## Discount Management - Exchange Discounts

**Path:** `Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Exchange discounts tab`

*Fig. B-156 Customer discounts - replacement discounts*

You can use this tab for defining discounts on exchange surcharges referring to a product or product class.

The fields in sections Discount for and Discount information are described in connection with the tab Discount list.
> ⇨ “Discount Management - Discount List" on page B-804

### Products
This list shows all discounts granted on exchange surcharges for glass. Whether or not these discounts will actually be used for calculation, depends on the setting Adopt from main item in product master data.

> **Example**
> A 5% discount is granted on the surcharge of the exchanged glass.
> A 10% discount is applied for IG.
> *   Adopt from main item: 10% discount for IG will be applied.
> *   No adoption: 5% discount of the exchange discount will be granted.

> ⇨ "Price Parameters" on page B-602

**Product** Exchange product for which the discount is defined.
**Discount** Discount (in per cent) granted for the exchange product.

### Product Classes
This list shows all product types and classes including the discounts currently defined.

**Product type/ Product class** Product type and class for which the discounts should be granted.

**Discount** Discount (in per cent) to be granted for this product type and class.

## Discount Management - Table

**Path:** `Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Table tab`

*Fig. B-157 Customer discounts - table*

You can use this tab to view all customers or suppliers for whom discounts have been entered.

The fields in sections Discount for and Discount information are described in connection with the tab Discount list.
> ⇨ "Discount Management - Discount List" on page B-804

## Change/Copy Discounts

**Path:** `Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu > Copy/change discounts`

This dialog is used for changing or copying discounts of the selected partners. This dialog offers the following tabs:
*   Copying Discounts
*   Change Discounts

### Copying Discounts

**Path:** `Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu > Copy discounts`

*Fig. B-158 Copying discounts*

This tab is use for copying the discounts of the selected partner in order to transfer them to another partner or group of partners.

> **General change**
> To change existing discounts in general you can leave these fields blank, only entering the new values.

#### Source:
The fields in this section are the same on both tabs.

**Customer/supplier, from/to** You can select a single partner or several partners in a row. The names of the first and last partner will be displayed automatically. To select just one partner, enter the same number in both fields.

**Group from/to** You can select a single partner group or several partner groups in a row. The names of the first and last group will be displayed automatically. To select just one group, enter the same number in both fields.

**All** This checkbox is accessible only if you have selected a price list or a price key. In this case you can decide whether the discounts for all customers, suppliers, or groups should be edited or copied.
- Only the discounts of the selected price list and/or key defined for certain partners or groups will be edited.
- All discounts of the selected price list and/or key will be edited or copied.

**Price list, key** You can restrict the selection to the discounts allocated to a certain price list and/or key. In this case you can use the checkbox all to define whether all the appropriate discounts should be edited or just those for certain partners or groups.
Please note that the `<n.e.>` entries refer to a price list or a price key.
If no price list and/or key is selected, the changes will be valid for all discounts.

**Product grp./Product - from** You can restrict the selection to discounts allocated to a certain product group (PGR, SPG, MPG) and/or a certain product. A sequence of product groups or products can be selected in both cases. The names will be shown automatically.

#### Target

**Customer, supplier** Partner for whom the discounts should be defined.

**Group** Group for which the discounts should be defined.

**Price list, key** Price list and/or key to which the discounts should be allocated. These fields will be released only if a price list and/or key has been selected in section Source.
Please note that the `<n.e.>` entries refer to a price list or a price key.

**Overwrite existing records** You have to decide whether existing discounts should be changed.
- Existing discounts will be ignored.
- The existing discounts should be changed as defined. Checkbox Delete all discounts for the target is locked.

**Delete all discounts for the target** You can decide whether the existing discounts should be deleted before new discounts are entered.
- Existing discounts will not be deleted.
- Existing discounts will be deleted first. The new discounts (from the source) will be created afterwards as defined. Checkbox Overwrite existing discounts is locked.

**Target discounts get default code** If discounts have been entered for several rates you can define whether the new discounts should be marked as the standard discounts.
- The new discounts should not be marked as default discounts.
- The new discounts should be marked as default discounts.

### Change Discounts

**Path:** `Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu > Change discounts`

*Fig. B-159 Change discounts*

This tab is used to change the discounts for the selected partner.
If no restriction has been made in section Source, all discounts will be changed as defined.

> **General change**
> To change existing discounts in general you can leave these fields blank, only entering the new values.

#### Source:
The fields in this section are the same on both tabs.

**Customer/supplier, from/to** You can select a single partner or several partners in a row. The names of the first and last partner will be displayed automatically. To select just one partner, enter the same number in both fields.

**Group from/to** You can select a single partner group or several partner groups in a row. The names of the first and last group will be displayed automatically. To select just one group, enter the same number in both fields.

**All** This checkbox is accessible only if you have selected a price list or a price key. In this case you can decide whether the discounts for all customers, suppliers, or groups should be edited or copied.
- Only the discounts of the selected price list and/or key defined for certain partners or groups will be edited.
- All discounts of the selected price list and/or key will be edited or copied.

**Price list, key** You can restrict the selection to the discounts allocated to a certain price list and/or key. In this case you can use the checkbox all to define whether all the appropriate discounts should be edited or just those for certain partners or groups.
Please note that the `<n.e.>` entries refer to a price list or a price key.
If no price list and/or key is selected, the changes will be valid for all discounts.

**Product grp./Product - from** You can restrict the selection to discounts allocated to a certain product group (PGR, SPG, MPG) and/or a certain product. A sequence of product groups or products can be selected in both cases. The names will be shown automatically.

#### Discount change
Choose an option to define how the discounts should be changed:
*   **Absolute** and a number, e.g. 5 or -5 to reduce or increase the discounts by 5 Euros.
*   **Proportional** plus a number, e.g. 2 or -2 to increase or reduce the prices by 2 per cent.
*   **Fixed** if a fixed value should be applied to the discounts, e.g. 5 to set all selected discounts to 5%.

**Rounding** Rounding to be used for the calculated discounts.
Roundings are defined in `Master Data > Order > Rounding`.
> ⇨ "Rounding" on page B-880

**Price list, key** Price list and key to which the amended discounts should be allocated. These fields will be released only if a price list and/or key has been selected in section Source. Please note that the `<n.e.>` entries refer to a price list or a price key.

**Main discounts, Graduated discounts, Exchange discounts** You can choose the discounts to be edited. All checkboxes are checked by default.
- These discounts should not be changed.
- These discounts are going to be changed as defined.

**Discounts get default code** If discounts have been defined for several rates you can specify which of them is going to be marked as the standard discount.
- The selected discounts will not be marked as default discounts.
- The selected discounts should be marked as default discounts.

## Delete Discounts

**Path:** `Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu > Delete discounts`

*Fig. B-160 Delete discounts*

You can use this dialog for deleting the selected discounts.

### Selection
Choose an option to define the discounts to be deleted:

*   **Customer:**
    The fields for selecting a certain customer are accessible.
*   **Group:**
    The field for selecting the group can be accessed.
*   **Rate:**
    The fields for selecting the price list and the corresponding key are released.

## Parameters (Customers, Suppliers)

**Path:** `Master Data > Partners > Customer, Supplier > Parameters`

*Fig. B-161 Customer - order parameters*

This dialog is used to define settings that override the settings from product master data or item entry. The settings only apply to the selected combination of partner and product group or product.

> **Dialog for customer and supplier data**
> The Parameters dialog is the same for customers and suppliers. It will therefore be described just once in this document.

### Identification
Choose an option to define the partners and products to which the settings in section Parameters should apply:

*   **Customer group, Supplier group:**
    The settings apply to the selected group.
*   **Customer number, Supplier number:**
    The settings apply to the selected partner.
*   **Product group:**
    The settings apply to the selected product group. Any of the three product group levels can be selected.
*   **Article number:**
    The settings apply to the selected product.

### Parameters

**Enter customer item/supplier item** You can define that the option Input control > Enter customer item is overwritten at item entry.
- The settings in dialog Document Management for the partner or group of partners will not be changed.
- The cursor automatically moves to the Consignment field when item entry is opened.

**Explicit display of price/surcharge** You can change the price display settings defined in product master data.
- The settings from product master data will not be changed.
- The price is displayed explicitly. This means that all elements of the price are shown separately if the selected combination consists of partner and product group or product.
> ⇨ Tutorial 1, "Price view Implicit in price per QU" on page B-219

### Table
The column headers in this table are based on the settings in section Identification.
The checkboxes are checked according to the settings in section Parameters.

## Customer Individual Products

**Path:** `Master Data > Partners > Customer > Customer Individual Products`

*Fig. B-162 Customized products*

This dialog is used to enter products that should only be available for a certain customer. This can also be e.g. glass provided by a customer for producing his orders.

> **Customized products at item entry**
> To be able to enter customized product numbers at item entry you have to choose the option Customized article search.
>
> As an alternative for customized products, an item can be saved as a macro. Apart from the sizes, the price and discount will be saved also. The macro can be defined for a single customer or in general.

Whether or not the customised product name should be printed, can be set in management of forms.
> ⇨ "Form Management" on page B-1045

### External product
**Customer** Number of the customer to whom this product belongs.

**Article** Alpha-numerical article number (product number) used for this product by the customer. This number can be used for this product at order entry.

> **Example**
> A customer regularly orders coated toughened glass of a size of x 1800 mm. Enter this product in master data and allocate it to the customer as a customized product. Use bronze as the article number.
>
> At item entry, enter bronze as the product number. The product is displayed together with the sizes entered in product management.

**Name (1-3)** Name and a short description of the product. The name appears at item entry and is analyzed for the printing of forms.
For single lites that are to be assembled in an IG unit, only the first name appears.

**EAN** EAN code (European Article Number) or GTIN code (Global Trade Item Number). In the US, this field can be used for the UPC code (Universal Product Code).

**Additional text** You can allocate text to the product to which the system refers at item entry.

### Own product
**Article** Article number by which the product is listed in A+W Business.

### Overview
The list shows all customers for which customized products have been entered.

## Delivery Time (Customer, Supplier)

**Path:** `Master Data > Partners > Customer, Supplier > Delivery time`

*Fig. B-163 Delivery time for customers or suppliers*

Use this dialog to define the delivery sequence per route and the time required for delivery.

> **Dialog for customer and supplier data**
> Dialog Delivery time is the same for customers and suppliers. It will therefore be described just once in this document.

The delivery time for customers only refers to the actual delivery. Delivery date calculation is based on the delivery time and the lead time used for producing an order. The lead time is set in company data.
> ⇨ "Company Data > System" on page B-970

### Selection

**Customer, supplier** Customer or supplier for whom the delivery time is defined.

**Route** Route allocated in the customer's master data. You can change this setting if required.

**Priority** Sequence number allocated to the partner in master data. You can change this number if required.

> **Details on the route priority in two dialogs**
> Please note that the route and the route priority can be entered in this dialog and in dialog Partner management > Order tab. You can open the Route priority overview in both dialogs to make sure that the entries are identical.

**Delivery time (days)** The delivery date is automatically calculated at order entry. The delivery time per customer will be taken into account.
If a route can be handled in one day, enter 0 in field Delivery time.
For customers who are farther away, enter the actual number of days required, e.g. including the time for customs clearance and sea crossings for cross-border routes.

**[Route list]** Opens the dialog Route list, listing all partners whose goods are delivered on the same route.

## Projects (Customer, Supplier)

**Path:** `Master Data > Partners > Customer, Supplier > Projects`

Projects are available only if project management is active in company data, and if projects have been defined.
> ⇨ "Projects" on page B-750

The tabs in the Invoicing dialog depend on the type of project management enabled in the company data. The following descriptions point out the project management types in which the tabs and fields are available.
> ⇨ Tutorial 2, "Project/Invoice Management" on page B-494

Dialog Invoicing also appears in module Documents. This is where projects are invoiced.
> ⇨ Sales, "Invoicing" on page C-688

> **Dialog for customer and supplier data**
> Dialog Invoicing is the same for customers and suppliers. It will therefore be described just once in this document.

This section provides information on the following subjects:

*   "Project Management / Invoicing Menus" on page B-822
*   "Projects - Invoices" on page B-823
*   "Invoices - Blanket Order" on page B-828
*   "Invoices - Allocated Orders" on page B-829
*   "Invoices - Allocated Purchase Orders" on page B-830
*   "Invoices - Totals" on page B-831
*   "Invoices - Estimated Quantities" on page B-832
*   "Invoices - Table" on page B-833

### Project Management / Invoicing Menus

**Path:** `Master Data > Partners > Customer, Supplier > Projects`

You can use the invoicing menus to make the standard settings for the dialog and open other dialogs without closing the invoicing dialog.
The entries in the menus depend on the active project management mode.

#### Functions Menu
**Path:** `Master Data > Partners > Customer, Supplier > Projects > Functions menu` or `Documents > Order > Project invoicing > Invoicing > Functions menu`

Use this menu to open other dialogs without closing the current one. The available functions depend on the selected project management mode.
The following entries are displayed:

*   **Add hours required:**
    Opens the dialog Hours required in which you can enter e.g. the fees for assembly work (only Invoicing).
    > ⇨ "Purchase Hours" on page B-835
*   **Add purchases required:**
    Opens the Purchasing dialog in which you can e. g. enter the cost of fitting material (only Invoicing management).
    > ⇨ "Purchase" on page B-836
*   **Claims calculation:**
    Opens the Claims calculation dialog in which you can issue and check invoices.
    > ⇨ "Claims Calculation" on page B-837

#### Print Menu
**Path:** `Documents > Order > Project invoicing > Invoicing > Print menu`

Use this menu for drawing up lists of invoices. The entries are only available if the Invoicing mode is active.
The following entries are displayed:

*   **Status report:**
    Produces a list of all projects to be invoiced, including the current claims and current balance.
*   **List:**
    Lists the estimated sums and the accumulated costs for the selected project to be invoiced.

### Projects – Invoices

**Path:** `Master Data > Partner > Customer, Supplier > Projects > Invoices tab`

The fields available on this tab depend on the project management mode enabled:

*   "Standard Project Management" on page B-824
*   "Extended Project Management" on page B-825
*   "Invoice management with allocated orders" on page B-827

### Standard Project Management

*Fig. B-164 Invoices - Invoices (standard project management)*

This dialog can be used to restrict the project to a certain period and define maximum values for this project.

#### Selection
The fields Project and Customer, Supplier are the same for all types of project management and invoicing.

**Project** Project defined in `Partners > General > Projects`.
Standard project management also allows entering a new name and thus create a new project.
> ⇨ "Projects" on page B-750

**Customer, supplier** Partner involved in this project. At document entry, only projects will be shown to which the partner stated in this document has been assigned.

**[Documents/Info]** Pressing this button will open a dialog that shows the number of orders entered for the selected project.
> ⇨ "Projects - Documents" on page B-834

#### Validity
**From, to** Start and end date of the period during which documents can be entered for this project. When the end date has been reached, the project can no longer be selected for document management.

#### Maximum values
You can enter maximum values for every customer project. When you close the order entry, a list of the orders entered plus the accumulated totals will be displayed.

**Net turnover** Maximum amount for this project.
This entry only serves for information in standard project management. The button [Documents/Info] can be used to display the orders actually entered for this project.

**Sqm.** Maximum amount of glass to be used.

**Qty.** Maximum number of lites or products to be used.

**Info** Additional information.

### Extended Project Management

*Fig. B-165 Invoices - Invoices (extended project management)*

You can use this dialog to add details for a project, e. g. an alternative shipping address and alternative payment terms.

**Quotation, No. customer order** Here you can enter the numbers of the quotation and of the order sent by the customer.
These fields are identical for all invoicing versions.

**Insert date** Date on which the number has been entered.
