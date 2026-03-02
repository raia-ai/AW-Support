---
description: "EN_AWBusiness_Sales_4_6-4"
---


---
## Overviews and References concerning Header Data

**Software Reference**

**Employee**
Name of the employee logged in to A+W Business.

**Comment**
You can enter comments about the down payment here, e.g. agreements in connection with this down payment or partial payment.

**Payment direction**
Select one of the defined payment directions.

**Payment procedure**
Enter the payment procedure.

**Payment reference**
Enter the payment reference.

**Overview**
This list shows all payments made for the current order that have been entered in this dialog. Down payments entered by means of a down payment invoice will not be taken into account.

### Totals

**Gross amount**
Gross amount of the order.

**- Down payment**
Total of down payments entered in this dialog.

**= Remainder**
Difference between the order total and the total down payments entered in this dialog.

### Backup

**Import file, Export file**
The data can be imported and exported.

### Miscellaneous

**Down payment via EDI**
You can specify whether down payments can be imported via EDI.
- [ ] Down payments are not imported via EDI.
- [ ] Down payments can also be imported via EDI. This setting is set automatically if orders are imported via EDI that contain down payments.

## Overviews and References concerning Items

The item entry menus can be used to display different types of information without closing the dialog itself. The dialogs are the same for all document types. We are going to describe them in connection with an Order in this manual.

This chapter provides information on the following subjects:

- "Product Search" on page C-577
- "Quick Inquiry" on page C-582
- "Parameter Replacement" on page C-584
- "Product Comparison" on page C-585
- "Complaints" on page C-586
- "Cutback" on page C-587
- "Variant Selection (Color Search)" on page C-588
- "Fixed Price Setting" on page C-589
- "Global Changes" on page C-590
- "Production BOM Breakdown" on page C-591
- "Terms" on page C-592
- "Prices/Term Information" on page C-593
- "Product Information" on page C-597
- "BOM - Supplements" on page C-602
- "Price Recorder" on page C-603
- "Fix Product" on page C-605
- "Copy Item" on page C-606
- "Cost and Surcharge Calculation (Item)" on page C-608
- "Insurance Settlements” on page C-609
- "Partial Deliveries" on page C-611

## Product Search

> Documents > Quotation, Order, Credit, Inquiry, Purchase Order > Quotation, Order, Credit, Inquiry, Purchase Order > Items > Shapes/processings > [magnifying glass]

This dialog offers the following tabs:
- "Selection - By Product" on page C-578
- "Selection - By Technical Parameters" on page C-580
- "Selection - by Classifiers" on page C-581

### Selection - By Product

> Documents > Order > Select order > Items > Shapes/processings > [magnifying glass] > by Product tab

*Fig. C-302 Selection - By Product*

Use this tab to select the search criteria. The system will display all products matching the selected criteria. If no criteria are selected, all products will be listed.

**Product type**
Restrict the search to the product type this searched for product has been assigned to.
⇨ Master Data, "Product Types and Product Groups" on page B-140

**Product group**
Restrict the search to the product group this searched for product has been assigned to. The product group depends on the product type.

**Matchcode**
Matchcode of the product you are looking for.

**Show locked products**
Products can be locked if they should not be entered in an order.
- [ ] Search only for products that can currently be offered for sale.
- [ ] Search for all products matching the selected criteria. This includes products that can no longer be offered for sale.
⇨ Master Data, "Product Definition" on page B-182

**Product no. from, to**
Restrict the search to a sequence of product numbers.

**Product group**
Restrict the search to the product group this searched for product has been assigned to.

**Description 1, Description 2**
Restrict the search to the restrictions that are defined in the master data. For float glass, usually only Description 1 is defined.

**Article info includes**
Restrict the search to a word in the article information. Entries are case-sensitive.

#### Overview

The list shows all products matching the selected search criteria.

**Automatic search**
The search can be started manually or automatically.
- [ ] The search is started by using the [Search] button when all criteria have been entered.
- [x] The search starts once you have entered the first search criterion.

**Searching with classifiers in BOM**
The search using classifiers can refer to the main product and the BOM.
- [ ] The search using classifiers only searches in the main products. For products with BOM, the levels are not searched.
- [ ] The search includes the BOM.

### Selection – By Technical Parameters

> Documents > Order > Select order > Items > Shapes/processings > [magnifying glass] > by technical parameters tab

*Fig. C-303 Selection - by technical parameters*

Use this tab to restrict the search by using technical parameters.

**Ug value in W/sqm**
Heat transmission coefficient. The Ug value defines the heat loss of a component in W/sqm. The smaller the Ug value, the higher the thermal insulation.

**Ug value according to DIN 4108-4**
Heat transmission coefficient of the glazing.

**Light transm. in %**
The light transmission expresses the directly transmitted, visible percentage of rays. The reference value of 100% applies to an unglazed hole in the wall.

**g value in %**
The value is composed of the direct transmission of solar energy and of the secondary heat emission to the inside due to long wave radiation and convection.

**Shading coefficient**
This value is the average transmission factor for solar energy, referring to the total degree of energy transmission of a 4 mm lite. This is necessary for calculating the cooling load of a building.

**Sound insulation factor in dB**
The sound insulation factor is the main effect of sound insulation. The lower the dB value, the higher the noise level from outside.

**Thickness tolerance in mm**
The thickness of insulated glass can vary by a few mm. This field is necessary if the thickness of the product is important.

**Size tolerance mm (<200 cm), (>=200 cm)**
Specifies by how many millimeters the IG pane may differ from the specified size.

**Show technical parameters**
By default, apart from the product number, matchcode, and descriptions 1 and 2, the product list only shows the standard height and width.
- [ ] Technical parameters are not shown on the product list.
- [ ] In addition to the standard information, the product list also shows the technical parameters.

### Selection – by Classifiers

> Documents > Order > Select order > Items > [...] > Tab by classifiers

*Fig. C-304 Selection - by classifiers*

On this tab, you restrict the search via the classifiers that are stored for a main product.
⇨ Master Data, "Product Management - Attachments / Classifiers" on page B-623

## Quick Inquiry

> Documents > Order > Quick inquiry
> Documents > Order > Select order > Item tab > Functions menu > Item group > Quick inquiry

*Fig. C-305 Start quick inquiry for the customer*

Select a customer in this dialog to answer an inquiry (via phone) quickly. The selected customer will be displayed together with the current credit limit status.

If you have entered an order including items during this inquiry, you can save or cancel it.
⇨ Tutorial, "Answering Quick Inquiries" on page C-99

Starting a quick inquiry opens a dialog for selecting the customer. Selecting the customer will produce the latest data on his credit limit and receivables.

Item entry opens next, with blank fields. The corresponding document header is already filled with the corresponding customer data.
⇨ "Document - Items" on page C-447

When you have entered the corresponding items, you can close or save the inquiry. You can define whether the inquiry will be saved as a quotation or as an order.

*Fig. C-306 Save quick inquiry*

### Storage location

- **Quotation:** Saves the quick inquiry as a quotation.
- **Order:** Saves the quick inquiry as an order.

**Client**
Selection of the client controls the view in the Area field.

**Area**
Select the corresponding OM area.

**Number manager**
The document is saved in the corresponding number manager. If you save the inquiry as an order, the system will automatically show the number manager belonging to the last edited order.

After exiting quick inquiry (End or [OK] (save)), the document you have been working on last will be displayed.

## Parameter Replacement

> Documents > Order > Select order > Items > Shapes/processings tab > [Formula]

*Fig. C-307 Parameter replacement*

This dialog shows the variables that can be used to amend the description.

**Text replacement**
You can edit the descriptive text. It is displayed in the Processing dialog in the Description field.

**Parameters with identical meaning**
Shows the parameters that can be used as synonyms.

## Product Comparison

> Documents > Order > Select order > Items > Shapes/processing tab > Start menu > ITOE

*Fig. C-308 Product comparison*

On this dialog, you check the rules for an imported DXF or SN file for processings. Changes to the processing in the order item are checked against the stored rules.
⇨ Master Data, "ITOE Rules" on page B-657

If you have entered a shape and processed in A+W CAD Designer, you can save the changes as SN file (TOE file). This way, an SN file is created in the BOM, a shape record inserted and linked to the TOE file.

The TOE files are saved in the form XXXX_TOE.SN, whereby the number at the front is determined by the number ranges of the SN files.

> **Property of CAD processing**
> Changes to properties that are not a component of the A+W processing type catalog are lost during comparison; that is, a drilling hole sequence with series dimensioning: The series dimensioning is deleted as soon as one of the participating drillings is changed in the processing entry. Such changes have to be made in A+W CAD Designer.

### Overview

The stored rules are displayed in the overview. Processing without rule are highlighted in color.

After confirming the product comparison, the BOM on the Shapes/Processings tab is rebuilt and the prices recalculated. Any additional change will be compared to the linked TOE file.

- **CAD processing:** Designation of the processing in A+W CAD Designer.
- **Product, Name:** Number and name of the rule in A+W Business.
- **Edit/insert rule:** Change to the iTOE rules dialog in order to create or edit a rule. ⇨ Master Data, "ITOE Rules" on page B-657
- **Rule found:** Designation of the stored rule for processing.
- **Property:** Content of the stored rule.

## Complaints

> Documents > Orders > Select order > Items > Add-on tab > [folder] next to the Base field

*Fig. C-309 Complaint*

Use this dialog to select a reason and cause of complaint for every item when you are entering a document of the type Complaint.
⇨ Tutorial, "Complaints" on page C-278

> **Complaints in other document types**
> If you do not use the dialog in document type Complaint, the data will not be transferred to complaint statistics.

**Cause**
The cause can be used for the statistical analysis of complaints. Input is optional.

**Reason**
The reason can be used for the statistical analysis of complaints. Input is optional.

**SP**
Shows the sales price of the returned item. This constitutes the lost sales.

**Free**
Complaint items and orders can be used for statistical analysis, e.g. analysis of the sales value.
- [ ] The complaint will be charged.
- [x] The complaint is free of charge, e.g. in cases of goodwill or in the event of an actual fault. The sales price value shows the lost sales.

## Cutback

> Documents > Orders > Select order > Grills tab > [cutback]

*Fig. C-310 Cutback*

Use this dialog to define the dimensions for the cutback per edge. The cutback describes the single distance between the outer edge of the window and the inner edge of the frame.

## Variant Selection (Color Search)

> Documents > Order > Select order > Grills tab > Search for variants [magnifying glass]

*Fig. C-311 Variant selection*

On this dialog, you select the color variants for an entered product.

### Search criteria

**Name**
Designation of the color that should be searched for.

**Foreign key**
Foreign key of the color that should be searched for.

### Overview

- **Variant, Name:** Internal number and name of the color.
- **Foreign key:** For Dorma articles, the Dorma color code. The foreign code can be used for communication with other programs, e.g. for the transfer to production.
- **Preview:** Display of the color variant.
- **Special color:** Special color, e.g. for screen printing.

## Fixed Price Setting

> Documents > Orders > Select order > Items > Items overview > Context menu > Enter fixed price

*Fig. C-312 Fixed price setting*

Use this dialog to enter a fixed price for selected item(s).

**Selected items**
Lists all selected items. The fixed price applies to these items as a whole.

**Default**
**Fixed price**
If you have entered a fixed price for the selected items, the total price of the individual items will be updated in section Selected items.

These entries will be adopted for item entry.

## Global Changes

> Documents > Orders > Select order > Items > Items overview > Context menu > Global changes

*Fig. C-313 Global changes*

Use this dialog to change the overall consignment setting for the selected items.

**Selected items**
Lists all selected items for which the consignment will be changed.

**Changed**
**Consignment**
This change applies to all of the listed items.
- [ ] The customer consignment will not be changed. The input field is locked.
- [x] You can change the customer consignment. The input field is enabled.

## Production BOM Breakdown

> Documents > Order > Select order > Items > BOM tab > BOM structure > Context menu (glass) > Production BOM breakdown

*Fig. C-314 Production BOM breakdown*

Use this dialog to change the production BOM breakdown. Processing steps are always defined for glass.

Production BOM breakdown can be disabled for processing. This means that for the current order, you can define a processing step for individual lites or for the entire unit.
⇨ Master Data, "Define Production BOM Breakdown" on page B-189

## Terms

> Documents > Orders > Select order > Items > View menu > Terms group > Terms

*Fig. C-315 Terms*

This dialog shows the discounts and individual prices that apply to this customer.
⇨ Master Data, "Defining a discount" on page B-353

**Discounts**
Shows the discounts that apply to this customer. These can refer to the individual customer or to the customer group this customer belongs to.

**Individual prices**
Displays the prices that have been specifically defined for this customer or its customer groups. This field is blank if no customer-specific prices have been defined.

## Prices/Term Information

> Documents > Orders > Select order > Items > View menu > Terms group > Price/term information

Use this dialog to obtain information about the prices and terms that apply to this customer.

> **Prerequisite**
> The dialog is only available if you have activated price calculation by macro prices in the company data.

This dialog offers the following tabs:
- "Prices/Term Information - Price Check" on page C-593
- "Prices/Term Information - Macro Prices" on page C-594
- "Prices/Term Information - Discounts" on page C-595
- "Prices/Term Information - Autom. Surcharges" on page C-596
- "Prices/Term Information - Customer" on page C-597

### Prices/Term Information - Price Check

> Documents > Orders > Select order > Items > View menu > Terms group > Price/term information > Price check

*Fig. C-316 Prices/term information - Price check*

This tab provides you with details on the prices. The display can be filtered by different criteria.

#### Selection

By selecting an option you define whether prices for a product, product type or product group should be displayed.

**Price list, key**
You can filter the prices by rates.

#### Print options

You can print the data. Define for this purpose whether the information should be printed from all or just from certain tabs.
- [ ] The data from the corresponding tabs is not printed, e.g. Discounts tab.
- [x] The data from the corresponding tabs is also printed.

### Prices/Term Information - Macro Prices

> Documents > Orders > Select order > Items > View menu > Terms group > Price/term information > Macro prices tab

*Fig. C-317 Prices/term information - macro prices*

This tab lists the macro prices and pertaining product structure.
The fields pertaining to the print options are explained in the section concerning the Price check tab.
⇨ "Prices/Term Information - Price Check" on page C-593

### Prices/Term Information - Discounts

> Documents > Orders > Select order > Items > View menu > Terms group > Price/term information > Discounts tab

*Fig. C-318 Prices/term information - discounts*

This tab shows the discounts that apply to this customer.
The fields pertaining to the print options are explained in the section concerning the Price check tab.
⇨ "Prices/Term Information - Price Check" on page C-593

### Prices/Term Information - Autom. Surcharges

> Documents > Orders > Select order > Items > View menu > Terms group > Price/term information > Autom. surcharges tab

*Fig. C-319 Prices/term information - automatic surcharges*

This tab lists the automatic surcharges that are charged to this customer.
The fields pertaining to the print options are explained in the section concerning the Price check tab.
⇨ "Prices/Term Information - Price Check" on page C-593

### Prices/Term Information - Customer

> Documents > Orders > Select order > Items > View menu > Terms group > Price/term information > Customer tab

*Fig. C-320 Prices/term information - customer*

This tab displays the current credit limit and the customer address from the customer master data.
The fields pertaining to the print options are explained in the section concerning the Price check tab.
⇨ "Prices/Term Information - Price Check" on page C-593

## Product Information

> Documents > Product info
> Documents > Quotation, order, credit note > Quotation, order, credit note > Items > View menu > Item group > Article info

This dialog provides details on a product without you having to switch to the master data.

This dialog offers the following tabs:
- "Product Info – Info" on page C-598
- "Product Info – Prices" on page C-599
- "Product Info – Attachments" on page C-601

### Product Info - Info

> Documents > Product info > Info tab

*Fig. C-321 Product info – info*

This tab shows the data from product definition.

#### Selection

The data in this section is adopted from product definition.
⇨ Master Data, "Product Management - Product" on page B-591

**Article/color**
The article number is automatically shown when you open the dialog through item entry. The defined variations are offered for selection in the Color field.

**Description 1, 2, 3**
Product descriptions from the master data.

**Product type**
The product type is automatically displayed when the dialog is opened through item entry. If it is used for a search, the data display will start from the first product of the selected type.

**Product group**
The product group is automatically shown when the dialog is opened from item entry.

**Reference number**
Reference number for customer products.

#### BOM

The entire BOM is adopted from the master data.

#### Article info

Article information is adopted from the master data.

#### View

If a view (bitmap) of the product has been linked in the product master data, the product image will be shown here.

### Product Info – Prices

> Documents > Product info > Prices tab

*Fig. C-322 Product info - prices*

This tab allows you to view the prices of a product.

#### Selection

These fields are explained in connection with the Info tab.
⇨ "Product Info - Info" on page C-598

**Only default rate**
You can restrict the price view to the standard rates.
- [ ] Shows all prices defined for the product.
- [x] Shows only the standard rates.

**Sort key by description**
The price display can be sorted by price keys.
- [ ] Prices are displayed in the sequence in which they have been entered in the system.
- [x] Prices will be sorted by price key description.

**Sort price list in descending order**
The price display can be sorted by year.
- [ ] Prices are displayed in the sequence in which they have been entered in the system.
- [x] The display will be sorted by price year description.

#### Standard sizes and stock

**Width, height**
Standard width and height from the master data. If no standard sizes have been defined, the display shows 0.

**[F3]**
With the button, you can open the Stock info dialog without closing the product info.
⇨ "Stock Info" on page C-736

#### View

Lists all prices defined for the product. Individual prices are directly shown in this table. Buttons are displayed for all other price types, e.g. [Vector]. These can be used to display the corresponding prices.
