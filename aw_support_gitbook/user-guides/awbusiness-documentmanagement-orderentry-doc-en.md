---
title: "EN_AWBusiness_Sales_4_5-2"
source: "EN_AWBusiness_Sales_4_5-2.pdf"
tags: ["A+W Business Sales", "Software Reference", "Document Management", "Order Entry", "Item Data", "Header Data", "Pricing", "BOM", "ERP", "Window Manufacturing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for A+W Business Sales, focusing on document management features. It details the various fields, tabs, and settings within the order entry and item data modules, including header data, technical parameters, attachments, pricing settings, and item-specific configurations."
long_description: "This document serves as a detailed software reference manual for the A+W Business Sales application, specifically covering the \"Document Management\" and \"Item Data\" sections. It provides comprehensive explanations for managing orders and related documents. The first part focuses on \"Header Data,\" which includes defining payment terms, rabbet deductions, sales and purchase price settings, technical parameters for spacers and labels, and managing attachments and customer-specific information. The second part delves into \"Item Data,\" explaining the item entry menus (Start, View, Functions, Options, Structure) and the various tabs for defining individual order items. This includes managing Bill of Materials (BOM), shapes and processing, grills, supplements, and other technical values. The guide is intended for users who need to understand the detailed functionality of creating, editing, and managing sales documents like quotations, orders, and credit notes within the A+W Business Sales system. It includes navigation paths, field definitions, and references to master data settings."
---

# Document Management & Software Reference

Define how the customer will pay this invoice. The selection list shows all methods of payment defined in the master data.
⇨ Master Data, "Payment Mode" on page B-914

---
### Rabbet
Rabbet deduction in mm. Automatically taken into account for the width and height during production. Details on the rabbet dimension are important for glaziers and for window construction.
The rabbet deduction must be specified if the dimensions provided by the customer specify the interior dimensions of the window frame. Since a distance of 4 to 5 mm will be required between glass and frame, the actual glass size is smaller than the rabbet dimensions defined by the customer.

### Doc. reference
In an original document, the value 0 is displayed in this field. In documents created from an original document, the number of the original order is shown, e.g. in partial deliveries, complaints, credit notes.

### Sales price settings, Purchase price settings
Minimum quantities and size rounding can be considered for calculating the order value. These are defined in the product master data. The appropriate surcharges are retrieved from the customer master data.
Minimum quantities and size rounding can be changed for the current order.
⇨ Tutorial, "Calculation settings" on page C-138
⇨ Master Data, "Price Parameters" on page B-602

### Min. quantity
Deviating minimum quantity for this order.

### Size rounding
Deviating measurement rounding for this order, according to which the surface will be calculated.
This value will be considered for calculating the technical totals.
⇨ "Totals (technical parameters)" on page C-513

### Parameters

**Monthly invoice**
Invoices can be printed and sent individually, collectively, or on a monthly basis.
- ☐ The order is invoiced with a separate invoice.
- ☑ The invoice for this order will be included in a monthly invoice.

### Grillpads
Calculation of grill pads is defined in the customer master data. If grill pads are used, these can optionally be invoiced.
- ☐ Grill pads will not be invoiced.
- ☑ Grill pads installed in the IG units will be invoiced.
⇨ "Grill pads" on page C-491

### Weight rounded
The weight can be used to calculate the energy surcharge. Calculation of the energy surcharge is defined in the customer master data. Company master data defines in general whether and how this surcharge will be applied.
- ☐ The energy surcharge is based on the actual weight.
- ☑ The energy surcharge is based on the rounded weight.
⇨ Master Data, "Rounding" on page B-880
⇨ Master Data, "Do not calculate energy surcharge by item weight" on page B-950

### Surcharges/discounts
This field lists the automatic surcharges and special discounts. The surcharges/discounts are defined in the Product surcharge allocation dialog in the master data.
- ☐ The surcharge will not be charged.
- ☑ The surcharge will be charged.
⇨ Master Data, "Defining a Miscellaneous Surcharge" on page B-318
⇨ Master Data, "Calculate surcharges with rounded quantities" on page B-950
⇨ Master Data, "Surcharge Product Assignment" on page B-1024

### Terms / Order volume

**Cust. project**
When you select the customer project, the pricing terms defined for this project will be automatically used for pricing.
All projects defined in the master data for this customer can be allocated to the order.
⇨ Master Data, "Project/Invoice Management" on page B-494
⇨ Master Data, "Projects (Customer, Supplier)" on page B-821

**Supplier**
By default, the purchase orders are transferred to the supplier defined as standard supplier for the concerned products.
⇨ Master Data, "Supplier List" on page B-854
If you enter a supplier, the purchase orders for this order will be transferred to this supplier.
If you save the changes, you can define whether the entire order will be purchased, or just the purchase articles.
If you confirm the question with [Yes], the procurement type of all items will be set to Purchase articles.
⇨ Master Data, "Product Codes" on page B-608

**Name**
Name of the defined supplier.

**Suppl. project**
If you have agreed on special terms for a certain construction project with your supplier, you can select the supplier's project for this order.
⇨ Master Data, "Projects (Customer, Supplier)" on page B-821

**Invoicing**
The invoice date is the basis for calculating the payment term. This value specifies the day as of which the payment term will be calculated, e. g. 5 means that the 5th of each month will be the calculation basis.
⇨ Tutorial, "Due Dates” on page C-205

**Payment. date 1, 2, 3**
Payment date for calculating the payment term.
⇨ Master Data, "Due date calculation" on page B-774

**Currency**
You can define a different currency for this order than the one transferred from the customer data. Prices can be shown in the selected currency.
⇨ Master Data, "Currency settings" on page B-921
⇨ Master Data, "Show currency at order entry" on page B-921

**Exchange rate**
If an exchange rate has been defined in the master data for the selected currency, this will be displayed and can be changed if required.

**Rate fixed for invoicing**
If you have entered an exchange rate, this exchange rate will be used for printing the invoice. If no rate has been entered, the system will use the rate defined in the master data.
If invoices for a customer are included in a collective invoice, the system will come up with a query should you change the setting. You can decide whether the current exchange rate will be omitted from the collective invoice.
- ☐ By default, the current exchange rate from the master data will be used for invoicing.
- ☑ The current exchange rate is fixed and will be used for invoice printing regardless of whether it has been changed in the master data after the order was created.

## Header data - Text
*Documents > Order > Select order > Header Data tab > Text tab*

*Fig. C-241 Header data - Text*

Use this tab to add information about this order that is important to e. g. the customer, Production or Dispatch.
⇨ Tutorial, "Enter text" on page C-52

> **Do not change text numbers by mistake**
> To avoid the inadvertent changing of (standard) text and text numbers, you should enable the option Check when changing the text number.
> ⇨ "Options menu" on page C-410

### Block overview

**Number**
You can choose a standard text module by entering the text number. If you want to enter text for this order manually, keep the 0.

**Buttons**
Use these buttons to add or remove text.
⇨ Tutorial, "Enter text" on page C-52

**Text code**
This text code controls the forms on which the text will be printed. The text code is automatically displayed when you select a text module. If you change the text code, the text corresponding with the new text code will be printed on the forms.
⇨ Master Data, "Text Code" on page B-1039
⇨ Master Data, "Text" on page B-1040

**Manual change**
This checkbox is ticked automatically when you add new text or delete added text.

**Overview (table)**
This table shows all the text you have added to this order.

### Text block

**Buttons**
You can change the font type and size and add hyperlinks, images and tables.
⇨ Tutorial, "Enter text" on page C-52

**Text field**
Click on the 'add text' button to release the text field. You can type directly into the text field to enter or change the text.

## Header data - Attachments
*Documents > Order > Select order > Header Data tab > Attachments tab*

*Fig. C-242 Header data - Attachments*

Use this tab to add files as attachments. All attachments are shown in the list. For each customer, one folder is created in which copies of the documents are saved. Define the path for the storage location in the company data.
⇨ Master Data, "File attachments" on page B-932
⇨ Tutorial, "Attaching documents" on page C-55
You can enter a remark for each file attachment. Frequently-used remarks can be stored in the master data and are available in the combo box.
⇨ Master Data, "File Attachment Remarks" on page B-1044

## Header Data - Technical parameters
*Documents > Order > Select order > Header Data tab > Technical parameters tab*

*Fig. C-243 Header Data - Technical parameters*

Use this tab to define the details on spacers and production labels. Any entry in here overwrites the settings in the master data.
The fields in the Identification and Address sections are described in detail in the chapter on the Documents tab.
⇨ "Header data - Document" on page C-414

### Spacer settings
The settings from the customer master data are used for entering IG products. These settings can be changed for the order.
⇨ Master Data, "Spacer settings" on page B-786

**Type**
Choose the spacer type to be used for IG units in this order.

**Color**
Choose the color to be used for the spacers. This entry will be checked when you enter spacers; a warning will be displayed if this colour is not available.

**Spacer text**
By default, the text to be printed on the spacers is transferred from the master data. It can be changed for this order.
⇨ Master Data, "Spacer Text" on page B-462

### Production labels

**Layout**
Printing of labels is based on the settings in the customer data. The layout number is transferred to the label printer.
⇨ Master Data, "Production labels" on page B-785

### Label parameters
If you want to print labels for an order, you have to define for each order how many labels will be printed for the IG units.
- **None:** No labels will be printed.
- **Per unit:** One label per IG unit will be printed, e. g. four labels for four IG units of the same structure.
- **Per item:** There will be one label per item, irrespective of the quantity.
⇨ Master Data, "Form Management" on page B-1045
⇨ "Form/Label Printing - Labels" on page C-642

### Claims
Blanket orders are settled by means of claims. For each claim (invoice), one production order is created.

**Number**
Number of the claim for which this production order is created.

**Order No.**
Number of the blanket order for which this production order is created.

## Header data - customer info
*Documents > Order > Select order > Header Data tab > Customer Info tab*

*Fig. C-244 Header data - customer info*

This dialog provides general information on the corresponding customer and on the attached documents referring to this customer. Details are adopted from the master data. In addition, you can save notes for the order.
⇨ Master Data, "Specification" on page B-761
The fields in the Identification and Address sections are described in detail in the chapter on the Documents tab.
⇨ "Header data - Document" on page C-414

### Information

**[Customer info]**
In the Information field, the general information is displayed that is taken over from the master data.

**[Note (...)]**
In the Information field, an overview of all notes created for the order is displayed.

**[New note ...]**
With this button you open the Add manual entry dialog on which you can add a note about the order.

## Item Data
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items*

Item entry and the corresponding menus are the same for all document types. We are going to describe it in connection with an Order in this manual.

This chapter provides information on the following subjects:
- "Item Entry Menus" on page C-436
- "Document - Items" on page C-447

### Item Entry Menus
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items*

The item entry menus can be used to define the standard settings for the dialog and to open other dialogs without having to close item entry.

This chapter provides information on the following subjects:
- "Start menu" on page C-437
- "View menu" on page C-437
- "Functions menu" on page C-439
- "Options menu" on page C-441
- "Structure menu" on page C-446

### Start menu
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items > Start Menu*

The default menu entries are explained in the Overview section.
⇨ Overview, "User Interface" on page A-13

**Print group**
*Documents > Order > Select order > Start menu > Print group*
This group is only enabled in the Header data tab.
⇨ "Print group" on page C-405

**ITOE group**
*Documents > Order > Select order > Start menu > iTOE Group*
This group is only enabled in the Item tab.
Opens the Product comparison dialog or the A+W CAD Designer (Shapes) in order to check the imported SN file and/or define rules.
⇨ "Product Comparison" on page C-585

### View menu
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items > View Menu*

**Prices group**
By default, prices in item entry are shown as sales prices. Sales price keys are offered for selection in the Keys column. You can switch the price display by using the View menu:
- **(PU) Purchase prices:** Display of the purchase prices of the individual components. Purchase price keys are offered for selection in the Keys column. The Price/PU field shows the price for auxiliary material. All manual changes refer to the purchase prices.
⇨ Master Data, "Cost Calculation" on page B-645
- **(FC) Prices in foreign currency:** Sales prices are shown in foreign currency. The input fields Keys, Price/PU, Unit, and Discount are locked.
- **Euro (Prices in Euro):** This setting is useful for countries in which the Euro is about to replace the national currency. Prices are shown in Euro if the price lists are kept in foreign currency. The input fields Keys, Price/PU, Unit, and Discount are locked.

> **Prices cannot be converted**
> Prices cannot be converted if the option No currency is active in company data.
> ⇨ Master Data, "Show currency at order entry" on page B-921

**Terms group**
- **Terms:** Opens the Terms/individual price dialog to obtain information on individual prices and discounts.
⇨ "Terms" on page C-592
- **Price/term information:** Opens the dialog for information on prices and discounts on the selected item. This entry is released for individual customers only.

**Documents group**
- **Show document:** Opens the Document view dialog as a preview of the document.
⇨ "Document View" on page C-543
- **Customer information:** Opens a dialog providing brief information about the customer.
⇨ "Customer Info" on page C-544

**Item group**
- **Article info:** Opens a dialog that provides details on the current product.
⇨ "Product Information" on page C-597

**Production group**
- **Product overview:** You can use this option to display a list of production reports.
⇨ "Status Message Overview" on page C-571

**Capacity overview group**
This group is only enabled if you are working with A+W Business Capacity Planner and A+W Capa View.
With this option, you can display an overview of the free and assigned capacities from A+W Business Capacity Planner.
⇨ "Capacity Overview" on page C-545

**Processing/shapes group**
The group is only enabled for the Shapes/processing tab. Use the buttons to select the presentation.
- Default
- Zoom in on sketch
- No BOM
- BOM at bottom right

### Functions menu
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items > Functions menu*

The groups are described in connection with section Document management.
The menu is divided into the following groups:
- "Document overview" on page C-407
- "Document overview group" on page C-408
- "Info group" on page C-408
- "Capacity group" on page C-409
- "Finance group" on page C-409
- "Calculation group" on page C-409
- "Optimization group" on page C-409
- "Item group" on page C-439
- "Purchasing group" on page C-441

**Item group**
- **Quick inquiry:** Opens the Quick inquiry dialog to enter a customer's (phone) inquiry without closing the current order.
⇨ "Quick Inquiry" on page C-582
- **Complaint:** Opens the Complaint dialog to enter a complaint for the selected item.
⇨ "Complaints" on page C-586
- **BOM supplement:** Opens the Supplement dialog to enter a cost center and cost type for a BOM element. This function is only available if a component has been marked in BOM tab.
⇨ "BOM - Supplements" on page C-602
- **Stock search:** Opens the Stock Info dialog to show the current stock on hand for the requested product.
⇨ "Stock Info" on page C-736
- **SNEditor:** This feature is only available if A+W CAD Designer has been installed on your system. It can be used for editing grill patterns and shapes.
- **Insurance prices:** Use this function to enter insurance payments for an item.
⇨ "Insurance Settlements" on page C-609
- **Delete item settings:** All manual price and discount settings for the selected item will be deleted. Prices and discounts will be reloaded from the master data.
- **Delete BOM item settings:** Only the manual price and discount settings for the selected BOM components will be deleted. Prices and discounts will be reloaded from the master data.
- **Delete preset item price:** The manually entered prices for the selected item will be deleted. The price will be reloaded from the master data.
- **Delete document reference settings:** The references are entered for order confirmations, invoices and dispatch notifications. These references are required for the data exchange with openTRANS.
- **Apply price settings to following items:** The prices for the selected item will be applied to all following items.
- **Change locked item:** This function is only available if you want to change an ordered item. The fields Product, Qty., Height and Width are enabled in the input line. The (changed) P.O. is automatically transferred to the order pool when you close item entry.
⇨ "Order Transfer - Order Pool" on page C-654
- **Price recorder:** Opens dialog Price recorder to check the price for the entered product for a certain period.
⇨ "Price Recorder" on page C-603
- **Reason for manual price setting:** You have to enter a reason for a manual change of price. This function is only available if the corresponding checkbox has been ticked in the company data.
⇨ Master Data, "Extended pricing (reference price, manual change)" on page B-952
- **Fix article:** Opens the Fix article dialog where you can e.g save the item as a customized article (product).
⇨ "Fix Product" on page C-605
- **Fix prices/terms:** The prices and discounts for a fixed (customized) product are fixed and cannot be changed.
- **Cost and surcharge calculation:**
    - **Overview:** The Cost and surcharge calculation dialog opens where you can check the calculation.
    ⇨ "Cost and Surcharge Calculation (Item)" on page C-608
    - **Detail - Item:** The Cost and surcharge calculation dialog shows a detailed view of the selected item.
    - **Detail - BOM:** The Cost and surcharge calculation dialog shows a detailed view of the BOM for the selected item.
    - **Delete and recalculate:** The prices for the selected item will be deleted and recalculated.
- **Copy from item...:** Opens the Copy from... dialog to apply the values of another item to the selected item.
⇨ "Copy Item" on page C-606
- **Start price calculation:** This function starts the price calculation for the selected item.
⇨ "Prices and Price Calculation" on page C-137

**Purchasing group**
This group is only enabled in the Item tab.
- **Inquiry for item:** Opens the Price comparison dialog to search for the best price on offer for the selected item.
⇨ "Price Comparison" on page C-659
- **Document enquiry:** Opens dialog Price comparison to search for the best price offered for the entire P.O.
⇨ "Price Comparison" on page C-659

### Options menu
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items > Options menu*

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

> **Activated options after opening the dialog**
> Please note that changed options will only become effective the next time you open the dialog.
> If an activated option has started a check, opening the document can be delayed. The extent of the delay depends on the performance of the computer.
> Activated options are described in the following.

**Documents group**
This group is described in chapter Document management.
⇨ "Documents group" on page C-410

**Items group**
The following entries are displayed:
- **Adopt for new entries:**
    - Adopt grills
    - Adopt shapes
    - Adopt surcharges/processing steps
    - Adopt gas
    The selected BOM components are always adopted for the next item. After that, they can be edited or deleted.
- **Additional product field:** You can display an additional field for the product number. The additional field is displayed next to the data field for the thickness of the glass if you enter or change a product number in the Items area of the order entry. With this option, during the quick entry of orders, you have an overview of the product numbers entered.
- **Keep spacers and gas when entering a new main product:** When the main product is changed, spacers and gas will not be deleted or changed.
- **Show CPIP code on BOM:** The BOM shows the CPIP code. This function is only required in France.
- **Delete glass, gas and airspace surcharges at preset of unit price (also for French pricing):** The corresponding surcharges will be deleted if you replace a lite, gas, or airspace in an IG item and enter a manual price for the item. This option can be enabled across the company data.
⇨ Master Data, "Delete glass, gas, and airspace surcharges if price/unit is defined (not for French pricing)" on page B-951
- **Quantity input for current item:** The quantity (area/weight) can be entered for the current item.
- **Adopt further details:** The entries in the Further details tab will be automatically adopted from the previous item.
- **Automatic tab change to:**
    - BOM
    - Supplement
    - Text
    - Further details
    Use the `<Tab>` key to go from the input line directly to the selected tab.
- **Do not adopt complaint reason and cause:** The reason and cause of a complaint will not be automatically adopted from the previous item.
- **Automatic stock search for stock articles:** After you have entered a stock article, the Stock info dialog opens.
⇨ "Stock Info - Stock Search" on page C-737
- **Start stock search in selection mode:** The Stock search dialog is started in selection mode. You start the search manually after you have entered the search criteria. This reduces the hit quantity and increases the speed of the query.
- **Limit stock search to dimension:** On the Stock search dialog, the dimension is taken over into the query in addition to the item number. This increases the speed of the query.
- **No error reports at pricing:** There will be no report on pricing errors. You should disable this option because otherwise you will not detect errors in prices.
- **Report if there is no PO exchange surcharge:** If you replace lites, missing purchase exchange surcharges will be reported when you close item entry.
- **Report if there is no BOM price:** If you have edited the BOM, missing prices will be reported when you close item entry.
- **Report if minimum stock is not met:** When you close item entry, the system will inform you that the quantity you have entered exceeds the current stock on hand.
- **Do not save in case of restriction errors:** If restrictions were violated at item entry, the system will issue a notification to this effect; the item cannot be saved. You will have to amend your input.
- **Report if glass article has no size:** The system will issue a notification if you have entered glass articles without sizes.
- **Adopt default surface for exchange surcharges:** If lites have been exchanged, the entered surfaces are used for calculating the exchange surcharges. You should use this option if you have enabled the option Enter quantity for the current item.
- **Delete discount if price is entered manually:** Discounts will be set to zero if prices have been changed manually.
- **Calculate prices only when saving:** By default, price calculation is executed immediately when the item is entered. This option defines that the prices of the entered items will only be calculated when the item is saved. This will improve performance for orders with many items.
- **Determine procurement type only when saving:** By default, the procurement type is calculated when the item is entered. With this option, the procurement type for all items entered is only determined when saving the item. This will improve performance for orders with many items.
- **No recalculation of automatic surcharges:** Automatic surcharges will not be recalculated in items.
- **Message in case of missing declaration of performance:** With this option, an error message is output if there is no declaration of performance for a product. This option is only activated for document type Order.
- **Check processing parameters**
    - At least one parameter set
    - Check all
    Parameters are checked at entry based on the selected option. The more parameters you have activated, the longer this data process is going to take.
- **Positioning of text:**
    - Text before item
    - Text after item
    - Product-related text
    This option defines the standard position of inserted text. This setting can be changed in the Text tab for each order item and text.
    ⇨ "Before, After item, Product referenced" on page C-508
- **Retaining texts by default:** The Retain text check box on the Texts tab of item entry is activated by default.
- **Purchasing:**
    - **Report ordered articles:** Automatically reports the ordered articles included in the item.
    - **Report status change at P.O. transfer:** If ordered articles are transferred to purchasing again, a query will appear before the order status is changed.
    - **Product description as per supplier file:** The product name entered in the supplier file will be used for the P.O.
- **Customer-based article search:** If you want to enter products via the search function, the customized products for this customer will also be displayed.
- **BOM image thickness display:** With this option, you can display the thickness of the individual BOM elements of the selected item. The thickness of the BOM elements is displayed in the page view on the Item tab of the item entry.
- **ATP query after item entry:** The ATP queries are only released customer-specifically. The dialog can be called automatically when leaving the item entry if at least one item was changed.
- **Open color search dialog with F4:** With this option, the dialog for searching for product variants (colors) can be opened with `<F4>`.

**Processing/shapes group**
The options are only enabled in the Shapes/processing tab. The following entries are displayed:
- **Select all edges for new entries:** When entering a new shape, all the edges are always selected for processing. This selection can be changed subsequently.
- **Check whether tangential edges should be selected:** If the previous option has been selected, a query concerning automatic selection is shown for round edges.
- **Multiple entry as default for new entry:** In the case of multiple entries, usually only the quantity can be entered for the processing steps. It is not possible to specify dimensions. This setting is particularly useful for quotations for which the exact dimensions of processing steps are not relevant. In standard entry all parameters can be entered. The mode can be changed by using the Multi checkbox when entering the processing step. This setting is saved for each document type and employee.
- **Select shape with double-click:** By default, the shapes can be selected with a simple click. If this option is activated, a shape is selected with a double-click.
- **No automatic recreation:** By default, with a click on a BOM element in the processing entry, a processing is attached automatically. If this option is activated, to attach a processing to a BOM element, you must select the menu option New.
- **Reentry as default:** When entering a processing, you can change automatically to entry mode.
- **1st field is shape number:** The shape number is displayed in the shape entry as the 1st field.
- **1st field is product number:** The product number is displayed in the shape entry as the 1st field.
- **Highlight selected processing:** The selected processing is highlighted in color in the display.

**Grill group**
The options are only enabled in the Grill tab. The following entries are displayed:
- Drill hole symmetrical:
- Field symmetrical:
- Drill hole asymmetrical:
- Field asymmetrical:
Depending on the selected option, the corresponding fields are activated and enabled by default.
- **Apply horizontal grill to vertical:** When entering grills, the article number of the horizontal grills is automatically adopted for the vertical grills.
    - This setting allows you to define that this handling behavior is applied when you change horizontal grills subsequently.
    - If you do not select this option, the vertical grills are not changed when you enter a different article number for the horizontal ones.

### Structure menu
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items > Structure menu*

Use this menu to define the levels of glass and manage processing macros.

**Structure group**
- **Pattern level 1 – 6:** The patterned side of the selected lite is turned to the selected level. You can also turn the levels by using the Item tab in the Prices section.

**Coating group**
- **Coating level 1 – 6:** The coated side of the selected lite is turned to the selected level. You can also turn the levels by using the Item tab in the Prices section.

**Macro group**
- **Save:** Opens the Macro dialog to save the data of the selected item as a macro.
⇨ Tutorial, "Save Macro" on page C-158
⇨ "Save Macro" on page C-618
- **Delete:** Opens the Macro dialog to delete a macro.
- **Change:** Opens the Change macro dialog to edit a macro.
⇨ "Change Macros" on page C-619
- **Search:** Opens the Search macro dialog to select a certain macro.
⇨ "Macro Search" on page C-621
- **Copy:** Opens the Copy macros dialog to copy a macro.
⇨ "Copy Macros" on page C-622
- **Only copy the product structure from macro:** Prices will not be adopted when an item is entered by means of the macro function.

### Customizing menu
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items > Customizing menu*

These functions are used for adjustments in dialogs.
This menu is accessible only if Customizing active is enabled in company data.

## Document - Items
*Documents > Quotation, Order, Credit Note, Inquiry, P.O. > Items, <F9>*

The tabs for item entry are the same for all document types. We are going to describe it in connection with an Order in this manual.
All details on the selected products are transferred from product definition. They can be changed according to the order.
⇨ Tutorial, "Order Items" on page C-57

> **Red letters for manual changes**
> Entries that have been changed manually will be displayed in red. Changes made to the items can be canceled in the menu Functions > Delete item setting.
> ⇨ "Functions menu" on page C-407

> **Additional information**
> ⇨ Tutorial, "Quick entry" on page C-91
> ⇨ "Document - Header Data" on page C-413

This dialog offers the following tabs:
- "Items - Item" on page C-448
- "Items - BOM" on page C-457
- "Items - Shapes/processing tab" on page C-461
- "Items - Grills" on page C-488
- "Items - Service" on page C-497
- "Items - Supplement" on page C-499
- "Items - Further details" on page C-503
- "Items - Text" on page C-507
- "Items - Attachments" on page C-509
- "Items - technical values" on page C-510
- "Items - Classifiers" on page C-512

### Items - Item
*Documents > Order > Select order > Items tab*

*Fig. C-245 Order entry - Items*

Use this tab to enter order items. Products and prices of all BOM elements can be edited in the first tab.
The items are entered in the Items section. The fields show the details of the selected item. Further features can be edited in the BOM tab. All manual changes are shown in red.
⇨ Tutorial, "Order Items" on page C-57

The menus can be used to make various standard settings, e.g. transferring data, update after a change, etc.
⇨ "Item Entry Menus" on page C-436

> **Exceed credit limit**
> If the current order exceeds the credit limit defined for the customer, you may not be able to enter further orders. However, the current order can be entered (in the amount required).
> ⇨ Tutorial, "Credit limit" on page C-45

**Product**
**(Product names)** The product name is transferred from the master data. It can be changed for the respective order item. Names 1 and 2 will be displayed for the main product.
For IG lites, the third line shows the technical parameters. The details from this line can be printed on the form.
⇨ Master Data, "Create product description from BOM" on page B-939
⇨ Master Data, "Form Management - Options 1" on page B-1051

**Product structure**
This section shows the actual BOM structure of the item. Use the context menu to add or remove individual components.
- Attach components, insert (before), insert (after), delete.
- Attach shape/processing.
- Production BOM breakdown.
- Cutback per edge.
BOM components relevant for production are displayed in blue. They show the processed component.

> **Print production BOM**
> Production-relevant bills of material will only be printed if the corresponding option has been selected in management of forms.
> ⇨ Master Data, "Define Production BOM Breakdown" on page B-189
> ⇨ Master Data, "BOM printing" on page B-1053

The symbols represent the product structure schematically. The sun represents the outside of the lite.
⇨ Tutorial, "Icons for item entry" on page C-62
⇨ Tutorial, "Enter Order Item" on page C-93

**Variation**
Shows the variation that has been selected for the main product or a component.

**Thickness**
The total thickness is the sum of the individual lites' thicknesses, including film layers, spacers, etc. If you enter a different total thickness, A+W Business will check if a suitable spacer is available. If no suitable spacer is available, the original value is displayed. The thickness can be used as a calculation basis for the item price.
⇨ Master Data, "Price Management" on page B-710

**Procurement**
The procurement type is adopted from the product definition. You can select a different procurement type if required.
If a main item or a superior BOM component is marked with the procurement type P.O. complete, the corresponding BOM components will not be booked out of stock if their procurement types are set to Stock withdrawal. The procurement type cannot be changed for these components in this case.

### Sales prices
This overview lists all the BOM components for the entered product. The fields are locked if the order has been transferred to production. You can undo the lock by using the function Change locked item.
⇨ "Item group" on page C-439
By default, the prices displayed are sales prices (SP). You can switch the price display using the View menu.
⇨ "Prices group" on page C-437

The following fields can be displayed:
- **Art.no.:** Product number of the BOM component. Enter a new product number in order to change a BOM component. Changing the spacer may result in a change of the value in the Thickness field.
- **Search:** Opens the dialog for the product search.
- **Name:** Name 1 defined in the master data.
- **PU:** Price unit.
- **Price/PU:** Price per price unit.
- **Net:** Price of the BOM component minus discount. This display depends on the price setting (implicit) in the product definition. If individual price calculation for IG and LG has been activated in the company data, then the individual price is displayed. If it has not been activated, then the exchange surcharges are displayed.
⇨ Master Data, "IG + LG single price calculation" on page B-947
- **Net total:** If a different quantity is entered in the BOM tab, then the values in the Net and Net total columns differ. E. g. if three covers that are the same belong to one fitting set, then this component is entered once in the BOM with the quantity 3. The price under Net total is then 3 x net.
- **Sense of pattern, patterned side:** Use these two buttons to define how patterned glass is to be fitted into the IG unit. The patterned side is always viewed from the outside in.
- **Coated side:** Use this button to define how a coated lite is to be fitted into the IG unit. The coated side is always viewed from the outside in.
- **Procurement type:** Procurement type for the selected BOM component.

You can view and edit prices and additional details for each individual BOM component in the BOM tab.
