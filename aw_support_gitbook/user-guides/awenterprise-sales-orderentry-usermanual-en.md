---
title: "EN-UM-AW_Enterprise-Sales_4_2"
source: "EN-UM-AW_Enterprise-Sales_4_2.pdf"
tags: ["A+W Enterprise", "Sales", "Order Entry", "Software Reference", "Document Management", "Article Search", "Product Search", "Quotation", "User Manual", "Search Functions"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the A+W Enterprise Sales module, focusing on search functions and document management. It details procedures for finding articles, products, and projects, as well as managing sales documents like quotations and orders."
long_description: "This comprehensive software reference manual provides detailed instructions for using the A+W Enterprise Sales application. The guide is divided into two main parts: Search Functions and Document Management. The Search Functions section covers various methods for locating information within the system. It explains how to use the 'Find Article' dialog, including searching by header/footer areas, names, article codes, and details. It also covers 'Find Product by Element' which allows searching for products based on their bill of materials (BOM) structure, and 'Find Project' for locating project-related data. The Document Management section offers a thorough guide to creating, editing, and managing sales documents. It begins with an explanation of symbols used throughout the application to indicate status and mode. Key processes covered include 'Quotation Entry,' 'Entry w/o Prices,' and a detailed breakdown of the 'Order Entry' dialog. The 'Order Entry' section is extensively detailed, covering header/footer areas, address management, properties, and various tabs for general information, pricing, status, and costs. The document provides menu paths, keyboard shortcuts, field descriptions, and technical database information for each function, making it an essential resource for users of A+W Enterprise Sales."
---

---
## Search Functions

### Find Article

**Sales > Order entry > Items tab > General tab > Article field > <F9>**

Use this dialog to search for articles that you need for the entry of an order. You can call up the article search via various menu paths. The dialog always looks the same.

The hits for the search are displayed on the tabs. If you open the article search, you will see all articles in the hit list. Using the filter criteria, you can restrict the hit list.

- Use `<F3>` to start the search.
- Use `<F2>` after the search to change tabs on the hit list.

The search results are shown in the hit list. The hit list is only displayed if you have started the search.

This dialog contains the following tabs:

- "Find Article - header, footer areas" on page D-52
- "Find Article – Names" on page D-55
- "Find Article – Article codes" on page D-57
- "Find Article - Details" on page D-59

The search results are shown in the hit list. The hit list is only displayed if you have started the search.

### Find Article – header, footer areas

**Sales > Order entry > Items tab > General tab > Article field > <F9>**

Use this dialog to search for articles using various search criteria.

If you open the article search, you will see all articles in the hit list. Using the filter criteria, you can restrict the hit list.

#### Header

Specify the search criteria in the header area. The hits for the search are displayed on the tabs.

Use `<F3>` to start the search.

**From no.** Start number from which articles are searched for in ascending order. The articles whose number is smaller than the number specified are excluded from the hit list.
Technical info: numerical field, DB field: artikel.artnrThe employees whose number is smaller than the number specified are excluded from the hit list.

**Matchcode** Alphanumerical matchcode of the article. The articles whose match code does not include the data specified are excluded from the hit list.
Technical info: alphanumeric field, DB field: artikel.artmc

**Article Code** Article code from master data. The articles whose article code does not include the specified data are excluded from the hit list.
Technical info: alphanumeric field, DB field: artikel.artikelcode

**Short Name** Short name of the article. The articles whose short name does not include the data specified are excluded from the hit list.
Technical info: alphanumeric field, DB field: artikel.kurzbez

**Main Name, Intern. Description, Internal2** Main name and additional descriptions of the article. The articles whose main name or internal name does not include the data specified are excluded from the hit list.
Technical info: alphanumeric fields, DB field: artikel.artbez1, artikel.artbez2, artikel.artbez3

**Art. Type, to** Number and description of the article type. In the Art. Type field, enter the number starting from which you will search for articles. In the to field, you restrict the search to articles with the appropriate article type. The articles whose article type number is smaller than the number specified in the Art. Type field or greater than the number in the to field are excluded from the hit list. When you enter a number, the description of the article type is displayed in plain text. Use `<F9>` to search for an article type.
Technical info: numeric fields, display fields, DB fields: artikel.atyp

**A+W Proc. Type, to** Number and description of the A+W-specific processing type. In the A+W Proc. Type field, enter the number starting from which you want to search for articles. In the to field, you restrict the search to articles with the appropriate processing type. When you enter a number, the description of the processing type is displayed in plain text. With `<F9>` you can search for a processing type. Technical info: numeric fields, display fields, DB field: ar-tikel.awtyp

**Prod. Group** Code of the product group to which the article is assigned.
Technical info: alphanumeric field, DB field: artikel.wagrp

**Material Grp.** Code of the material group to which the article is assigned.
Technical info: alphanumeric field, DB field: artikel.artgrp

**Supplier** Number of supplier from whom the article is ordered. You can select the supplier from the list of suppliers using `<F9> > <F8>`.
Technical info: numeric field, DB field: artikel.stdlinr

**Type** Display of the article status. In the document entry, only active articles are displayed. The field cannot be edited.
Technical info: display field, DB field: artikel.still

**Article Image**

The lite structure of the marked article from the hit list is shown in cross-section here. The sun marks the outside of the lite.

#### Footer

Use the buttons in the footer to navigate in the hit list, display additional hits, and update the hit list.

- **[|<] and [>|]**: Use to jump to the first or last entry in the hit list.
- **[<<] and [>>]**: Use to display the previous or next page of the hit list.
- **Refresh**: Updates the entries in the search fields. Corrected or additional entries in the search fields are taken into account during the search. The button is only enabled in the Search fields area.
- **More Data**: Displays additional entries in the hit list that correspond to the search criteria. If no more hits can be displayed, the button is locked.
- **New Search**: Deletes all search criteria for a new search. Alternatively, you can use `<Ctrl> + <R>` to delete the search criteria and start a new search.

### Find Article – Names

**Sales > Order Entry > Items tab >General tab > Article field > <F9> > Enter search criteria > <F3>**

This tab displays the names of the articles that match the search criteria.
Enter the search criteria in the header area.

- Use `<F2>` to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

#### Header

The fields in the header area are described for the Find Article – Header, Footer dialog:
⇨ "Find Article – header, footer areas" on page D-52

#### Show record for the article overview

The number of hits in the list is indicated on the right, above the tabs, in a spacer.
The record display is described for the Find Market Partner dialog:
⇨ "Find Market Partner" on page D-41

#### Names tab

The columns correspond to the fields in the header.
In addition, the following columns are displayed:

- **Number:** Article Code.
  Technical info: display field, DB field: artikel.artnr
- **Aband:** Indication of whether the article has been discontinued.
  - Y: Article is discontinued.
  - N: Article is active.
  In the document entry, only active articles are displayed.
  Technical info: display field, DB field: artikel.still

#### Footer

The fields in the footer area are described for the Find Article – Header, Footer dialog:
⇨ "Find Article - header, footer areas" on page D-52

### Find Article – Article codes

**Sales > Order Entry > Items tab >General tab >Article field > <F9> > Enter search criteria > <F3> > Article Codes tab**

This tab displays additional information about the articles that match the search criteria.
Enter the search criteria in the header area.

- Use `<F2>` to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

#### Header

The fields in the header area are described for the Find Article – Header, Footer dialog:
⇨ "Find Article – header, footer areas" on page D-52

#### Show record for the article overview

The number of hits in the list is indicated on the right, above the tabs, in a spacer.
The record display is described for the Find Market Partner dialog:
⇨ "Find Market Partner" on page D-41

#### Article Codes tab

The columns are described for the Names tab.
⇨ "Find Article - header, footer areas" on page D-52

In addition, the following columns are displayed:

- **Main Name:** Name of the article.
  Technical info: display field, DB field: artikel.artbez1
- **Supplier, Name:** Supplier number and name of the supplier.
  Technical info: display field, DB field: artikel.stdlinr

#### Footer

The fields in the footer area are described for the Find Article – Header, Footer dialog:
⇨ "Find Article – header, footer areas" on page D-52

### Find Article – Details

**Sales > Order Entry > Items tab > General tab >Article field > <F9> > Enter search criteria > <F3> > Details tab**

This tab displays details of the articles that match the search criteria.
Enter the search criteria in the header area.

- Use `<F2>` to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

#### Header

The fields in the header area are described for the Find Article – Header, Footer dialog:
⇨ "Find Article - header, footer areas" on page D-52

#### Show record for the article overview

The number of hits in the list is indicated on the right, above the tabs, in a spacer.
The record display is described for the Find Market Partner dialog:
⇨ "Find Market Partner" on page D-41

#### Details tab

The columns are described for the Names tab.
⇨ "Find Article - header, footer areas" on page D-52

In addition, the following columns are displayed:

- **Description (article number):** Description of the article.
  Technical info: display field, DB field: artikel.artbez1
- **Atyp, Description:** Number and description of the article type. The description is displayed automatically in the selected system language.
  Technical info: display field, DB field: artikel.atyp
- **A+W Type, Description:** Number and description of the A+W processing type. The description is displayed automatically in the selected system language.
  Technical info: display field, DB field: artikel.awtyp

#### Footer

The fields in the footer area are described for the Find Article – Header, Footer dialog:
⇨ "Find Article – header, footer areas" on page D-52

### Find Article by Types

**Sales > Order Entry > Items tab > General tab > PType field > <F5> > <F6> > [Find Article]**

Use this dialog to find articles using the A+W processing types or the article types. All articles of the selected types are displayed on another selection dialog.

#### Processing Steps tab

This tab displays the processing types for selection that are included in the standardized A+W processing catalog and processings included in the article master data. Discontinued processing types are not displayed.

- **Number:** Number of the A+W processing type
- **A+W Processing Type:** Designation of the A+W processing type

#### Article Types tab

This tab displays the article types for selection that include articles in the article master data. Discontinued article types are not displayed.

- **Number:** Number of the article type
- **Article Types:** Name of the article type

#### Selection dialog

- **Article:** Article, processing number
- **Description:** Article, processing description
- **2nd Description:** Additional informational text about the description, e.g. short name of the article or processing type.

### Find Product by Element

**Sales > Order Entry > Items tab > General tab >Article field > <Shift> + <F8>**

Use this dialog to search for products using the components they contain. You can call up the product search using various menu paths. The dialog always looks the same.

The hits for the search are displayed on the tabs. The hit list is only displayed if you have started the search.

- Use `<F3>` to start the search.
- Use `<F2>` after the search to change tabs on the hit list.

This dialog offers the following tabs:

- "Find Product by Element – Header, Footer area" on page D-63
- "Find Product by Element - Cust. Article" on page D-65
- "Find Product by Element – Names" on page D-67
- "Find Product by Element – Tech. Values" on page D-68

### Find Product by Element – Header, Footer area

**Sales > Order Entry > Items tab > General tab > Article field > <Shift> + <F8>**

Use this dialog to search for products using elements from their BOM structure.

#### Header

Specify the search criteria in the header area. The hits for the search are displayed on the tabs.
Use `<F3>` to start the search.

**Product Type** Type of the product:
- IG
- LAMI
- Cast resin
Technical info: toggle field, DB field: artikel.artgrp

**GI 1** Number of the first glass article. This field is a mandatory field. If you leave the field without specifying a number, a list of the glass articles is displayed for selection.
Technical info: mandatory field, numeric field, DB field: artkuzu.kuartnr

**GI 2** Number of the second glass article. This field is optional.
Technical info: numeric field, DB field: artkuzu.kuartnr

> **Position of the glass article in the lite**
> The search criteria Gl1 and Gl2 do not consider the installation position of the glass article in the lite. The search is done for all lites that include the specified glass. In the hit list, the glass is displayed according to its installation position in the lite from outside to inside. Gl1 is the glass on the outside of the lite.

**Foil Type** Number of the foil type. The field is only enabled for the product type LAMI.
Technical info: numeric field, DB fields: artikel.folientyp

**AIR** Size of the spacer in millimeters. This field is only enabled for the product type /G.
Technical info: numeric field, DB field: mussken.gv11

#### Footer

**Selected AcosCode** Currently not used.

**Article descript. 1** Currently not used.

**Tech.Values** Displays the technical values in the volumns Ug value, g value, dB value, and Tv value. The button is only enabled customer-specifically.

**Search** Starts the search. The button is only enabled in the header area.

**Selection** Opens a selection dialog for the current field. The button is only enabled if selection options are stored for the field.

### Find Product by Element – Cust. Article

**Sales > Order Entry > Items tab > General tab > Article field > <Shift> + <F8> > Enter search criteria > <F3>**

This tab displays information about the structure of the articles that match the search criteria.

- Use `<F2>` to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

Specify the search criteria in the header area.

#### Header, footer area

The fields in the header and footer area are described for the Find Product by Elements – Header, Footer dialog:
⇨ "Find Product by Element - Header, Footer area" on page D-63

#### Cust. Article tab

- **Sta:** Displays the status of the item.
  ⇨ "Explanation of Symbols" on page D-79
  Technical info: display field
- **Article:** Article number.
  Technical info: display field, DB field: artikel.artnr
- **Description:** Description of the article.
  Technical info: display field, DB field: artikel.artbez1
- **G11, GI2, G13:** Numbers of the glass articles. The number of glass items depends on the article. For articles with more than three glass items, only the first three glass items for the lite are displayed.
  Technical info: display fields
- **AIR1, AIR2:** Size of the spacer in the first and second lite interlayers in millimeters. The quantity of spacers depends on the number of lites in the IG (insulated glass). For articles with more than two spacers, only the first two spacers are displayed.
  Technical info: display fields
- **Interlayer:** Number and description of the spacer or the foil. For articles with more than one spacer or foil, only the first spacer or the first roil is displayed.
  Technical info: display field
- **Gas:** Number of the gas in the interlayer.
  Technical info: display field

### Find Product by Element – Names

**Sales > Order Entry > Items tab > General tab > Article field > <Shift> + <F8> > Enter search criteria > <F3> > Names tab**

This tab displays information about the descriptions of the articles that match the search criteria.

- Use `<F2>` to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

#### Header, footer area

The fields in the header and footer area are described for the Find Product by Elements – Header, Footer dialog:
⇨ "Find Product by Element – Header, Footer area" on page D-63

#### Names tab

- **ACOS Product:** Article number.
  Technical info: display field, DB field: artikel.artnr
- **Description:** Description of the article.
  Technical info: display field, DB field: artikel.artbez1
- **Main description:** Main description of the article.
  Technical info: display field, DB field: artikel.artbez2
- **Int. Descr.:** Internal article description.
  Technical info: display field, DB field: artikel.artbez3
- **Short Name:** Short name of the article.
  Technical info: display field, DB field: artikel.kurzbez

### Find Product by Element – Tech. Values

**Sales > Order Entry > Items tab > General tab > Article field > <Shift> + <F8> > Enter search criteria > <F3> > Tech. Values tab**

This tab displays information about the technical values of the articles that match the search criteria.

- Use `<F2>` to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

#### Header, footer area

The fields in the header and footer area are described for the Find Product by Elements – Header, Footer dialog:
⇨ "Find Product by Element - Header, Footer area" on page D-63

#### Tech. Values tab

Some of the columns are described for the dialogs Find Product by Elements Cust. Article and Find Product by Elements – Names dialogs:

⇨ "Find Product by Element – Cust. Article" on page D-65
⇨ "Find Product by Element - Names" on page D-67

In addition, the following columns are displayed:

- **Gas1, Gas2:** Numbers of the gases in the interlayers.
  Technical info: display fields
- **UgValue:** Heat absorption coefficient.
  Technical info: display field
- **g Value:** Energy transmission coefficient (total transmittance).
  Technical info: display field
- **DB Value:** Sound damping value of the item in decibels.
  Technical info: display field
- **Tv Value:** Degree of light transmission).
  Technical info: display field

### Find Project

**Sales > Order Entry > Project field > <F9>**

Use this dialog to search for projects.

If you open the search in the Project field, all projects of the market partner will be displayed in the hit list. You can restrict the hit list using the filter criteria.

> **Selecting Project before Market Partner**
> You can use `<Ctrl>+<F11>` in the Customer field to search for projects before you select the market partner. All objects are then displayed on the Find Project dialog. If you select a project, only the customers are displayed on an additional dialog to whom the current project is assigned. If the project is only assigned to one market partner, it is selected automatically.

If you select a project, depending on the system configuration, some data for the selected market partner or creditor may be overwritten, e.g. delivery address, cost center, discounts.

The search results are shown in the hit list.

This dialog offers the following tabs:

- "Find Project – header, footer areas" on page D-70
- "Find Project – Address" on page D-72
- "Find Project - Identification" on page D-73

### Find Project – header, footer areas

**Sales > Order Entry > Project field > <F9>**

Use this dialog to search for projects using various search criteria. Only the projects are displayed that are assigned to the market partner that was selected in the Customer field in the order entry. You can restrict the hit list using the filter criteria.

#### Search fields

Specify the search criteria in the header area. The hits for the search are displayed on the tabs. Depending on the system configuration, not all of the following fields are displayed.

**from Project** Start number from which projects are searched for.
Technical info: numeric field, DB field: objekte.objnr

**Project Abbr.** Two-letter abbreviation of the project from the master data that can be printed on the lite label.
Technical info: alphanumeric field, DB field: objekte.etitxt2

**Description** Description.
Technical info: alphanumeric field, DB field: objekte.bez

**External number** Project number that is specified by the customer.
Technical info: alphanumeric field, DB field: objekte.exobjnr

**LabelText** Text for the project that is printed on the lite label.
Technical info: alphanumeric field, DB field: objekte.etitxt1

**All** Specification whether glazing work is intended for the project:
- Y: Glazing work is planned for the project.
- N:No glazing work is planned for the project.
Technical info: toggle field, DB field: objekte.vergl

**Sales Repr.** Employee number to which the project is assigned. The representative is incorporated into the commission calculation, for example. If you specify a number, the name of the employee is displayed in plain text.
Technical info: numeric field, DB field: objekte.vertreter

**Route** Route number that is assigned to the project. If you specify a number, the name of the route is displayed in plain text.
Technical info: numeric field, DB field: objekte.routenr

**Glazing Employee** Employee number for the glazing work. If you specify a number, the name of the employee is displayed in plain text.
Technical info: numeric field, DB field: objekte.verglmanr

**Cost Center** Abbreviation of the cost center for the object. If you specify an abbreviation, the name of the cost center is displayed in plain text.
Technical info: alphanumeric field, DB field: objekte.kostenst

#### Footer

**New Search** Deletes all search criteria for a new search.

### Find Project – Address

**Sales > Order Entry > Project field > <F9> > Address tab**

This tab displays the address-related data of projects that match the search criteria.

Enter the search criteria in the header area.

- Use `<Shift>+<F2>` to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.
- Use `<Ctrl>+<R>` to delete the search criteria input.

#### Search fields

The fields in the header area are described for the Find Project – Header, Footer dialog:
⇨ "Find Project - header, footer areas" on page D-70

#### Address tab

The columns in the hit list correspond to the fields in the header area. In addition, the following columns are displayed:

- **Abbrev.** This column corresponds to the Project Abbr. field from the header.
  ⇨ "Project Abbr." on page D-70
  Technical info: display field, DB field: objekte.etitxt2
- **Sales Repr., Name:** The columns correspond to the Sales Repr. field in the header. The name of the representative is drawn from the employee master data.
  ⇨ "Sales Repr." on page D-71
  Technical info: display fields, DB field: objekte.vertreter
- **Rte. No., Route** The columns correspond to the Route field in the header. The route name is drawn from the route master data.
  ⇨ "Route" on page D-71
  Technical info: display fields, DB field: objekte.routenr

#### Footer

**New Search** Deletes all search criteria for a new search.

### Find Project – Identification

**Sales > Order Entry > Project field > <F9> > Identification tab**

This tab displays the identification characteristics of projects that match the search criteria.

Enter the search criteria in the header area.

- Use `<Shift>+<F2>` to change tabs on the hit list.
- Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.
- Use `<Ctrl>+<R>` to delete the search criteria input.

#### Search fields

The fields in the header area are described for the Find Project – Header, Footer dialog:
⇨ "Find Project - header, footer areas" on page D-70

#### Identification

The columns in the hit list correspond to the fields in the header area. In addition, the following columns are displayed:

- **Cost Center, Description:** Abbreviation and description of the cost center that is assigned to the project. The name of the cost center is drawn from the master data.
  Technical info: display fields, DB field: objekte.kostenst
- **Glaz.:** Specification whether glazing work is intended for the project:
  - Y: Glazing work is planned for the project.
  - N: No glazing work is planned for the project.
  Technical info: display field, DB field: objekte.vergl
- **GlazEmp, Name:** Employee number and name of the employee for the glazing work. The name of the employee is drawn from the master data. Technical info: display fields, DB field: objekte.verglmanr

### Enter Value – Extended Search

**Sales > Order Entry > Order field > <Shift> + <F5> or <Ctrl> + <E>**

On these dialogs, you can search for orders using a particular criterion. The dialog is called up for each criterion using a different key combination. The Enter Value search dialog looks the same for all criteria, but it differs depending on the criterion in the description of the search field.

The following dialogs are described in this section:

- "Enter Value – search for reference" on page D-75
- "Enter Value - search for original number” on page D-76

### Enter Value – search for reference

**Sales > Order Entry > Order field > <Shift> + <F5>**

Use this dialog to search for orders using the reference text.

#### Enter value

**Reference** Reference text or part of the reference text. With an asterisk * in front of the search term, you extend the search to all orders that contain the reference text.

#### Selection dialog

This dialog displays all orders with the specified reference text.
Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the selection dialog.

- **Reference:** Reference text for the item.
- **Cust.:** Customer name.
- **Order:** Order number.

Use `<Enter>` to apply the order number of the marked entry in the order entry.

### Enter Value – search for original number

**Sales > Order Entry > Order field > <Ctrl> + <E>**

Use this dialog to search for orders that were entered with reference to an original order. You can search for orders using the original order number to which they refer.

#### Enter value

**Original number** Original number of the order that was specified as reference during document entry. You can use `<F9>` to search for a number.

#### Search dialog

In the Original Order Number field on the Enter Value dialog, you can use `<F9>` to open the selo search for original orders.

**Search** Original order number starting with which documents are searched for. If you do not enter a number, all available original orders will be displayed in the hit list.

Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the hit list.

- **Original Order Number:** Order number of the original order.
- **Site:** Site number.
- **Number:** Order number of the new order.
- **Subnr:** Subnumber of the new order.
- **Customer:** Customer name of the new order.

If you select an original number with `<Enter>`, a selection dialog opens on which all orders are displayed that refer to this original order number.

#### Selection dialog

This dialog displays all orders with reference to the order with the specified original order number.
Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate the selection dialog.

- **Order:** Order number.
- **Original Order Number:** Order number of the original order.
- **Customer:** Customer name.

Use `<Enter>` to open the marked order in the order entry.

## Document Management

In the document management, all dialogs and functions are described with which you can edit documents. In this section, you enter and edit the documents for sales, e.g. quotations and orders.

The following dialogs are described in this section:

- "Explanation of Symbols" on page D-79
- "Quotation Entry" on page D-82
- "Entry w/o Prices" on page D-83
- "Order Entry" on page D-84
- "Order Items" on page D-116
- "Site Change" on page D-140
- "New Delivery Address" on page D-141
- "End customer address" on page D-143
- "Market Partner Info" on page D-145
- "Contacts" on page D-147
- "Cancel" on page D-148
- "Staff Allocation – Special" on page D-149
- "Configurable Fields" on page D-149
- "Overview" on page D-150
- "Product Sets (Sash Master)" on page D-151
- "Article Dimensions" on page D-153
- "Stock Forecast" on page D-154
- "Product Replacement" on page D-157
- "Complaint" on page D-161
- "Order Types" on page D-162
- "Article Details for Dimensioned Variants" on page D-164
- "Variant and Color/Thickness Selection" on page D-167
- "Private Fields" on page D-168
- "External Data - Import" on page D-169
- "Document Types" on page D-171
- "Allocation of Document Types" on page D-172
- "File Allocation" on page D-174
- "DXF Import” on page D-175
- "Amendment Log" on page D-176
- "Delivery Date Change Log" on page D-178
- "Shape Catalog" on page D-179
- "Shape - Dimensions" on page D-180
- "Payment Management" on page D-182
- "Payment Plan" on page D-184
- "Error Information System" on page D-186
- "Production Monitor" on page D-188

### Explanation of Symbols

This section describes the identifiers for the dialog mode, the item status, and the item identifier.

#### Dialog mode

The dialog mode is shown in the title line of the dialog.

| Symbol | Symbol description | Meaning |
| :--- | :--- | :--- |
| Dialog with cross | In this mode you can create new records. |
| Dialog with pen | In this mode, you can edit a data record. |
| Yellow triangle with exclamation point | In this mode, you cannot edit a data record, e.g. because it has already been transmitted to production. |
| Search | In this mode, you can search for data records. |

#### Item status and item identifier

The item status is displayed on the Items tab next to the Item field.

| Symbol | Symbol description | Meaning |
| :--- | :--- | :--- |
| (green) | green | The item can be edited at will since production has not begun yet. |
| (yellow) | yellow | The item or sub-parts of the item have been ordered or the purchase order has been printed. |
| (red) | red | Item has been planned in production. It can no longer be edited. |
| (three quarters red, one quarter blue) | three quarters red, one quarter blue | Item has been partially delivered. |
| (half red, half blue) | half red, half blue | Item has been fully delivered. |
| (two quarters red, two quarters blue) | two quarters red, two quarters blue | Item has been partially invoiced. |
| (blue) | blue | Item has been invoiced completely. |
| (Red cross) | Red cross | The item will be deleted. |

The item identifier is displayed in front of the Item field.

| Symbol | Symbol description | Meaning |
| :--- | :--- | :--- |
| Yellow star | Yellow star | The product dimension and additional processing of the article are stored for the selected customer. After saving the customer-specific article, a green star is displayed. ⇨ "Article Details for Dimensioned Variants" on page D-164 ⇨ Help Cards, "Fix item" on page D-29 |
| Green star | Green star | The article has been defined customer-specifically and can only be entered for this specific customer. When you create a customer-specific article, you can create the BOM structure with additional processings, articles, dimension changes and additional customer-specific requests. ⇨ "Article Details for Dimensioned Variants" on page D-164 |
| Shape | Shape | Item is entered with shape. ⇨ "Shape - Dimensions" on page D-180 |
| Window with muntins | Window with muntins | Item has been entered with muntins. ⇨ "Muntin Entry" on page D-229 |
| Shape with muntins | Shape with muntins | Item is entered with shape and muntins. ⇨ "Shape - Dimensions" on page D-180 ⇨ "Muntin Entry" on page D-229 |

### Item status and document status in text form

The status of the document and the items entered can also be displayed in text form.

- **A Document status**: If the document status changes, the current status will be displayed in the title line of the dialog (e.g. (partially) produced, GLOBAL CORRECTION, SHIPPING, PLANNING IN PROGRESS).
- **B Item status**: If the item status changes, the status of the appropriate item is displayed on the right of the dialog on the item level, e.g. packed, FIXED, local correction. Each item can have a different status. The item status displayed applies for the marked item.

For additional information about the various status indicators, contact your A+W Software GmbH contact person.

### Quotation Entry

**Sales > Quotation Entry**

Use this dialog to enter and edit quotations. Use `<Enter>` to assign the quotation number assigned by the system. To open a quotation that has been entered, enter the quotation number in the Quotation field or use `<F9>` to change to the search dialog.

If for quotations you enter a delivery date, depending on your system configuration, you can create a resubmission date to follow up on the quotation. When the resubmission date has arrived, a message will be displayed at the program start or a reminder e-mail sent.
⇨ "Resubmission" on page D-402

You can create an order from any quotation by creating a reference to the quotation in the order entry. If you enter the quotation number in the Reference field in the order entry, the data from the quotation will be taken over into the order.

The Quotation Entry dialog is structured in the same way as the Order Entry dialog. Differences from the Order Entry dialog will be described:
⇨ "Order Entry" on page D-84

### Entry w/o Prices

**Sales > Entry w/o Prices**

Use this dialog to enter customer orders without prices. In the case of orders in the store, this will prevent customers from viewing the purchase prices. In addition, employees who cannot see the operational prices can enter orders. These orders are then checked by a technician after the fact.

The price calculation for the order is executed hidden when you save the order. The document is saved under the order number assigned by the system.

The Entry w/o Prices dialog is structured in the same way as the Order Entry dialog.
⇨ "Order Entry" on page D-84

### Order Entry

**Sales > Order Entry**

On this dialog, you enter and/or edit orders. The Order Entry dialog is divided into three parts:

- **Header:** The customer data and delivery conditions are displayed in this area.
- **Items:** Information about the order items is displayed in this area.
- **Footer:** Information about the order totals, the discounts, and surcharges is displayed in this area.

This dialog offers the following tabs:

- "Order Entry – header, footer area" on page D-85
- "Order entry - Addresses" on page D-92
- "Order Entry – Properties" on page D-95
- "Order Entry - Miscellaneous" on page D-101
- "Order Entry - Totals" on page D-106
- "Order Entry – Detailed View Discounts" on page D-111

The Items area offers the following tabs:

- "Order Entry - General" on page D-116
- "Order Entry – Properties" on page D-129
- "Order Entry - Prices" on page D-134
- "Order Items – Status" on page D-137
- "Order Entry - Costs" on page D-139

### Order Entry – header, footer area

**Sales > Order Entry**

On this dialog, you enter the header data for the order, e.g. the customer data and delivery conditions. The footer displays information about the order totals.

- Use `<Enter>` to change to the next field in the header area. In the last field of the header area, the Project field, use `<Enter>` to change to the Items tab.
- From the Receipt, Invoice Type or Project fields, use `<F2>` to change to the item level to the Addresses, Properties, and Miscellaneous tabs.
  - ⇨ "Order entry - Addresses" on page D-92
  - ⇨ "Order Entry - Properties" on page D-95
  - ⇨ "Order Entry - Miscellaneous" on page D-101
- Use `<End>` to change from the item level to the General tab in the footer area and to exit the order entry.

#### Header

**Order** Order number. The number is assigned by the system from the assigned number range. If you enter a number that has already been assigned, the corresponding order is opened. Depending on the status, you can edit the order. The field name varies depending on the dialog on which you enter the document, e.g. Quotation in the quotation entry. If you enter the document number, for some document types another field is displayed, e.g. for Invoice or Delivery Note. The subnumber for the document is displayed in this field. You can select a subnumber already assigned or let the system assign the next free number.
Technical info: mandatory field, numeric field, DB field: kauf.auftrnr

> **Automatic assignment of document numbers**
> If you enter a new document, the document number is assigned automatically by the system. For invoices, first an internal, temporary number is assigned. This way, the system ensures that invoices are numbered sequentially.

**Customer** Customer number. If you specify a number, the customer's name and location are displayed in plain text. Only orders for active customers can be entered.
Technical info: mandatory field, numeric field, display fields, DB field: kauf.kunr, kauf.orgname

**Reason** Reason for a date change. The Reason field is only displayed if you change the delivery date in an order previously entered.
Technical info: alphanumeric field, DB field: kaufltedit.text

**Ref.** Document number that is being referenced. You can select a quotation, an order, a supplier inquiry or a PO as reference. You can take over all data from the reference document or only the header data from the reference document.
Use `<F9>` to open the Find Reference dialog:
⇨ "Find Reference Document" on page D-47
Technical info: numeric field, DB field: kauf.referenz

**Pre-selecting document type for the reference**
Depending on the system configuration, it is possible to specify one of the document types as pre-selection for the reference entry:

- Use `<F8>` display the document type configured as default in the Reference field.
- Use `<F9>` to open a selection dialog with all document types that can be referred to. use the arrow keys to select a document type.
- Confirm your entry using `<Enter>`.
- The Reference field displays the number of the current market partner.
- If you would like to specify the current market partner as pre-selection, then confirm with `<Enter>`.
- If you would like to specify another market partner as pre-selection, use `<F9>` to open the Find Market Partner dialog in order to select a market partner. Alternatively, you can enter the market partner number directly in the field. Use `<Enter>` to confirm the selection.
- The Reference field is empty. If you open the Find Reference dialog now, the document type and market partner that you have specified are pre-selected as search criteria.

**Enter document with reference**
- Use `<F9>` to open the Find Reference dialog in order to select a reference document for the specified criteria. Alternatively, you can enter the document number directly in the field.
- Use `<Enter>` to confirm the selection. You can take over all data from the reference document or only the header data from the reference document.

**Site** Company number and site number in which the order is created. The Site field is only enabled if you are working with internal site separation. The company number is drawn from the system master data automatically and displayed in a display field.
Technical info: numeric fields, DB fields: kauf.company, kauf.hausnr

**Entry Date** Entry date. By default, the field is pre-populated with the current date. If you want to change the entry, you have to enter the new date twice.
Technical info: mandatory field, date field, DB field: kauf.edat

**Cust. PO No.** External customer PO number. For orders from one site, the order number of the sending site is in this field.
Technical info: alphanumeric field, DB field: kauf.exaufnr

**Date** Date of delivery requested by the customer. In the first field you can enter the calendar week. In the second field you can enter the date in the format DD.MM.YYYY. If you have specified the calendar week and route, you can display the possible dates in a second field on a selection dialog with `<F9>`. Only the dates are displayed that are created for route planning in the master data. The system checks whether all order items can be provided in their entirety on the requested delivery date after order scheduling in the production system. If it is not possible to deliver by the desired date, the system reports this circumstance to the person entering the order via e-mail and shifts the date to the next possible date of delivery.
Technical info: mandatory field, numeric field, date field, DB fields: kauf.kwideal, kauf.ltideal

> **Quotation with date**
> The system can be configured so that a quotation with a date causes re-submission. The person entering the order receives a message at program start on the appropriate date so that quotations can be followed up upon.

**Route** Route number. Route selection shows the routes and corresponding route dates. You can store one main route and three alternative routes for a customer in the master data. The route is determined using the customer and address data and system configuration from the master data. If the via-plant function is configured, use `<F5>` to select the site via which the delivery should be organized. For information about the via-plan function, contact your A+W Software GmbH contact person.
Technical info: mandatory field, numeric field, DB field: kauf.routenr

**Scheduled** Display of the planned delivery date. The planned delivery date is calculated using various data, e.g. handling time, travel time, and capacity planning and entered in the Planned field as planned delivery date.
Technical info: display field, DB field: kauf.ltplan

**Cust. Item** Details about the item from the customer's item list. The customer items are displayed on the General tab in the Cu.Itm field:
- **Itm:** The field Cu.Itm is enabled on the item level. The order items can be entered according to customer-specific item designations, e.g. 1.1, 4.2, A_1, G_4.
- **Type:** The items are entered by glass types.
- **none:** The Cu.Itm field is locked on the item level. The customer-specific item descriptions cannot be used.
Technical info: toggle field, DB field: kauf.kndposkz

**DateType** Information about the date type that will be printed on the order. If Call or rush is selected, then the date will be forwarded to A+W Production. For rush, the production of the goods is preferred for scheduling. For Call, the production is planned so that the goods can be delivered on-call.
- **(no selection):** Date type is not specified.
- **Call:** date on call.
- **rush:** order is transferred to production as a rush order.
- **poss. = if possible, by the date.**
- **bind.:** date is binding. The system cannot change the requested delivery date.
- **without:** without binding date.
- **Auto:** date is assigned automatically.
- **follows:** Date to follow. The date agreement has not yet been reached.
Technical info: toggle field, DB field: kauf.abrufkz

**Receipt** Type of the communication channel via which the order was received. This information is used for statistical evaluations, tests, and for research purposes.
- **Representative:** Order was received by a sales representative.
- **Letter:** Order was received by regular mail.
- **Fax:** Order received by fax.
- **Phone:** Order received by phone.
- **EDI:** Order was transferred electronically.
- **Shop:** The order was entered in the shop.
- **Test:** Order was entered for test purposes only and will not be produced.
- **Cash sale:** Order was placed and paid in cash in the shop.
- **C.service:** Order was received by the customer service.
- **Replacement:** A replacement order can be issued if the original order was lost.
- **Euro conv:** Function to convert into euro (cannot be selected).
- **Partial payment:** As soon as a partial invoice is issued, the system enters Partial payment in this field. The value Partial payment cannot be selected manually.
- **Final:** As soon as the final invoice is issued, the system enters Final in this field. The value Final cannot be selected manually.
- **Online:** The order was received online, e.g. via the Web application or iQuote.
- **E-Mail:** The order was received via e-mail.
Technical info: toggle field, Database field: kauf.eingang

**Invoice type** Specification of the services for which the invoice is issued. Usually, the glass and the installation work are invoiced together. Upon request, you can create individual invoices.
- **Total:** The invoice is created for the total order, that is, for material and installation services.
- **Glass:** The invoice is only created for the material of the order.
- **Service** The invoice is only created for the installation services of the order.
Technical info: T=toggle field, DB field: kauf.rechart

**Project** Project. A project is assigned to the market partner and can be, for example, a construction site of the customer or a different delivery address. You can link special conditions to the project, which only apply for this project, e.g. discounts or payment options. You are able to bill project-related.
Use `<F9>` to open the project search.
⇨ "Find Project" on page D-69
Technical info: numerical field, DB field: kauf.objnr

#### Items

In this area, you enter and edit the items of an order. The tabs for the order items are described separately:
⇨ "Order Items" on page D-116

#### Footer

The footer area displays the total order values of the items. You can grant a general discount and manually edit the amount in the Net total field. You can only enter the fields if you have completed the order entry.

- Use `<End>` to change from the item level to the footer area.
- Use `<F2>` to open the Order Entry dialog for calculating discounts and the net amount.
  ⇨ "Order Entry - Totals" on page D-106

**Sender** Display of the site number and the reference number. The reference number can be the document number that was specified as reference in the document entry for the document or for EDI orders the order or PO number.
Technical info: display fields, DB fields: kauf.hausnr

**Qt, kg, m2** Display of the total order value for the quantity in pieces, weight in kilograms, and area in square meters.
Technical info: display fields, DB fields: kauf.gesst, kauf.gesm2, kauf.gesgewicht

**Total** Display of the total price of all items less the item discount from the field Minus on the Prices tab. The total price is calculated differently depending on the price type.
⇨ "Order Entry – Prices" on page D-134
⇨ Preise und Konditionen, "Preisarten" on page K-49
Technical info: display field, DB field: kauf.gesnetto

**Disc.** Discount granted for the total amount in percent. With discount granted, the amount in the NetTotal field is adjusted.
Technical info: numeric field, DB field: kauf.gesfaktor

**Net total** Total of all item prices, incl. the discounts and plus the surcharges. If you edit the amount, the system calculates the difference and displays it in the Gen. discount or Gen. surcharge field on the calculation dialog.
⇨ "Order Entry - Totals" on page D-106
If the Net Total field is empty or if the value is 0, a query will be displayed whether you want to rework the document. With [Yes] you go back to order entry. With [No] the Complaint Statistics dialog opens.
⇨ "Complaint" on page D-161
Technical info: numerical field, DB field: kauf.nettototal

**+VAT ()** Display of the VAT. The VAT amount is in the field that is assessed on the net amount. In the brackets, the applicable VAT is displayed in percentage.
Technical info: display field, DB field: kauf.mwstbetrag

**Gross** Display of the gross total amount. The amount is calculated from the net amount plus the VAT.
Technical info: display field, DB field: kauf.gesbrutto

**C. margin** Display of the contribution margin (gross gain) that the total quantity of items contributes to covering fixed costs. The contribution margin is the difference between the revenue and the variable costs of the items. All discounts and surcharges are taken into account.
Technical info: display field, DB field: kauf.dbdm

**%** Display of the contribution margin in percent.
Technical info: display field, DB field: kauf.dbvh

**Save** Backs up the data already entered in the document entry. In case of a system crash, the document entry can be continued with the data backed up. If the document entry is interrupted, a notice appears that the data backed up will be lost in case of an interruption. If you confirm, the document entry will be interrupted and the data backed up deleted.

### Order entry – Addresses

**Sales > Order Entry > Addresses tab**

On this tab, you can edit the customer and delivery address. The customer address is drawn from the customer's master data or the project.

You can configure the determination of the delivery address customer-specifically. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

#### Header

The fields in the header area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

#### Customer Address

**Name, 1stName** Customer's first and last names.
Technical info: alphanumeric fields, DB fields: kauf.orgname, kauf.orgvorname

**Title** Number of the title. If you select a number, the title is displayed in plain text.
Technical info: numeric field, DB field: kauf.organrede

**Attn.** For the attention of. Name of the person who should receive the delivery.
Technical info: alphanumeric field, DB field: kauf.orgzhd

**Addition** Additional text for address.
Technical info: alphanumeric field, DB field: kauf.orgbranche

**Street** Street address of the delivery address.
Technical info: alphanumeric field, DB field: kauf.orgstr

**PCd. POB** Postal code and P.O. box number.
Technical info: alphanumeric fields, DB fields: kauf.orgpfplz, kauf.orgpostfach

**PBoxCity** City name of the post box. Technical info: alphanumeric field, DB field: kauf.orgpfort

**PCd.City** Postal code and city of the delivery address.
Technical info: alphanumeric field, DB fields: kauf.orgplz, kauf.orgort

**Country** International country code for vehicles in the destination country. If you specify a code, the country name is displayed in plain text.
Technical info: alphanumeric fields, DB fields: kauf.orgkfzcode, kauf.orgland

**Tel** Customer's phone number.
Technical info: alphanumeric field, DB field: kauf.orgtel

**Fax** Customer's fax number. Technical info: alphanumeric field, DB field: kauf.faxnr

**E-mail** Customer's e-mail address.
Technical info: alphanumeric field, DB field: kauf.orgemail

**Language** Number of the national language of the customer in which the documents will be printed. If you select a number, the language is displayed in plain text.
Technical info: numeric field, DB field: kauf.sprkz

**Reg. No** Key number for the tax type. The tax type is stored in the system data. If you select a number, the name of the tax type is displayed in plain text.
Technical info: numeric field, DB field: kauf.kukz

#### Delivery Address

You can enter a different delivery address, e.g. the address of a construction site.

- Use `<Ctrl>+<N>` to create a new delivery address for the customer.
  ⇨ "New Delivery Address" on page D-141
- Use `<Ctrl> + <L>` to select the stored delivery address of a customer.
  ⇨ "Find Addresses" on page D-49

The fields are described for the Customer Address area:
⇨ "Customer Address" on page D-92

In addition, the following field is described:

**Reg. No** Dispatch region. The dispatch region is stored in the system master data and is determined via the postal code.
Technical info: display field

#### Footer

The fields and buttons in the footer area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

You can only edit the fields in the footer if you have completed the item entry. Use `<End>` to change from the item level to the footer area.

### Order Entry – Properties

**Sales > Order Entry > Properties tab**

On this tab you can edit information relating to staff allocation, shipping information, and invoice and printing options.

#### Header

The fields in the header area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

#### Staff Allocation

**Ordered by** Employee number. If you select a number, the employee's name is displayed in plain text. Use `<F5>` to open the Contact Person dialog where you can select or create a new contact person.
⇨ "Contacts" on page D-147
Technical info: numeric field, DB field: kauf.busnr

**PO date** Date the order was received.
Technical info: date field, DB field: kauf.bdat

**Operator** Employee number and name of the operator who entered the document. The fields are pre-populated by the system. They cannot be edited.
Technical info: display fields, DB field: kauf.esuer

**Departm.** Number of the department to which the operator is assigned. The fields are pre-populated by the system. They cannot be edited.
Technical info: display fields, DB field: mitarb.abtnr

**Handled by** Employee number and name of the operator who edited the document but did not enter it. If you select a number, the operator's name is displayed in plain text.
Technical info: numeric field, DB field: kauf.abvertr

**Field Staff** Name of the field employee.
Technical info: alphanumeric field, DB field: kauf.vertr

**Sales Repres.** Sales representative. Employee number of the representative to whom the commission will be paid. If you select a number, the representative's name is displayed in plain text.
Technical info: numeric field, DB field: kauf.vertrerloe

#### Shipment Information

**Maximum Load** Maximum weight that the customer can unload with its technical equipment.
Technical info: numerical field, DB field: kauf.gmaxgew

**Delivery** Comment about the requested delivery method:
- **Pickup:** Customer collects the goods.
- **Third-party business transaction:** The producing plant will ship the goods directly to the customer.
- **No selection:** Goods will be delivered via the route that has been entered in the header.
Technical info: toggle field, DB field: kauf.geschart

**Dir. Dispatch** Indicator as to whether the customer will receive the delivery directly from the production facilities or whether the goods will be delivered to the dealer. The field is pre-populated by the system.
- Y:Goods will be directly shipped to the customer.
- N: Goods will be shipped to the ordering dealer.
Technical info: toggle field, DB field: kauf.drkliefkz

**Delivery type** Number of the method of delivery, e.g. carriage paid. If you select a number, the name of the delivery type is displayed in plain text.
Technical info: numeric field, DB field: kauf.lieferart

**Disp. type** Number of the dispatch type, e.g. truck. If you select a number, the name of the dispatch type is displayed in plain text.
Technical info: numeric field, DB field: kauf.versandart

**Packing type** Number of the packing type, e.g. box. If you select a number, the name of the packing type is displayed in plain text.
Technical info: numeric field, DB field: kauf.verpackart

**Rack load** Rack load. Select by which criteria the goods shall be sorted on the racks:
- **Item** = by item.
- **Size** = by size.
- **Air+Size** = by airspace and size.
- **Item (free)** = items kept together, but freely organized.
- **HM Glas Farb Dick:** by hard dimension, glass dimension, and color.
- **HM GI.maß Farbe - :** by hard dimension, glass dimension, and color.
- **HM Gl.maß - Dicke:** by hard dimension, glass dimension, and thickness.
- **HM - Farbe Dicke:** by hard dimension, color, and thickness.
- **HM Glasmaß - - :** by hard dimension and glass dimension.
- **HM - Farbe - :** by hard dimension and color.
- **HM - - Dicke:** by hard dimension and thickness.
- **HM - - - :** by hard dimension.
- **Reference:** by reference text.
The evaluation of the selected criteria depends on the system configuration.
Technical info: toggle field, DB field: kauf.gbelad

**Customs Exit** Number of the customs exit office for the delivery papers. If you select a number, the name of the customs office is displayed in plain text.
Technical info: numeric field, DB field: kauf.azsnr

**Destin. Customs** Number of the customs office in the country of destination. If you select a number, the name of the customs office is displayed in plain text.
Technical info: numeric field, DB field: kauf.bzsnr

**Travel Time/Mls** Estimated travel time and display of the route. The travel time affects the delivery date. The route is drawn from the Distance field of the delivery address.
Technical info: numeric fields, DB fields: kauf.anfahrt

**Shipping Route** Delivery route for delivery or shipping via a second site. The field is only enabled if the internal site separation is active. Technical info: numeric fields, DB fields: kauf.endroutenr

**Via Site** Display of the site number of the site via which the goods are sent for delivery or shipping via a second site. The site is displayed automatically if you specify a delivery route.
Technical info: display field, DB field: kauf._vsvia

#### Invoice and print options

**VAT ID No.** Customer's VAT ID.
Technical info: alphanumeric field, DB field: kauf.steuernr

**Taxpayer's No.** Customer's registered tax number at tax office.
Technical info: alphanumeric field, DB field: kauf.finstnr

**Cost Center** Cost center name for statistical evaluations.
Technical info: alphanumeric field, DB field: kauf.kostenst

**Invoice Type** Type of invoice.
- **Separate invoice:** The addressee will receive a separate invoice for every order.
- **Cover sheet invoice:** The addressee receives a separate cover sheet invoice for each order.
- **Collective invoice:** The addressee will receive one invoice that combines several orders. You can select at what intervals a collective invoice will be issued.
  - weekly
  - every 14 days
  - monthly
Technical info: toggle field, DB field: kauf.rechnungsart

**Coll. Invoice Limit** Maximum invoice amount up to which you can create a collective invoice. If the credit limit is exceeded, the invoices will be created as separate invoices.
Technical info: numerical field, database field: kauf.srechlimit

> **Note regarding the creation of collective invoices**
> Both the limit for collective invoices and the invoice recipient's consent to collective invoicing must be saved in the market partner master data.

**Partial Inv.** Specification whether partial invoices are created after a partial delivery:
- Y = permit partial invoices.
- N = do not permit partial invoices.
If you select Collective invoice in the Invoice Type field, and you permit partial invoices, goods shipped by partial shipment will be included in the next collective invoice.
Technical info: toggle field, DB field: kauf.teilfakkz

**Invoice Block** Invoicing can be blocked for this document. With active block, the invoice recipient is not issued an invoice for this order for the time being.
- Y = lock for invoicing.
- N = permit invoicing.
Technical info: toggle field, DB field: kauf.fakturastop

**Partial Del.** Specification whether the customer accepts partial deliveries or does not want to receive these. The specification is only for informational purposes. Even if N is selected, it is possible to create partial delivery notes for the order.
- Y = permit partial deliveries.
- N = do not permit partial deliveries.
Technical info: toggle field, DB field: kauf.teilfakkz

**Rush Order** Current order receives preferential treatment and is dispatched to production with higher priority.
- Y = define as high-priority order.
- N = do not assign higher priority for the order.
Technical info: toggle field, Database field: kauf.schnell

**Print Gross Prices** Gross prices are printed on market partner documents.
- Y = print gross prices.
- N = do not print gross prices.
Technical info: toggle field, DB field: kauf.preisdrkz

**Print Customer Factor** The customer-specific factor can be printed on market partner documents.
- Y = print customer factor.
- N = do not print customer factor.
Technical info: toggle field, DB field: kauf.rabdrkz

> **Example:**
> If a customer receives a discount of 10%, the value for the customer factor is 0.9.

**Print Processing Prices** Show processing prices for processing activities separately and print.
- Y = show prices for processing activities separately.
- N = do not show separate prices for processing activities.
Technical info: toggle field, DB field: kauf.explbearbkz

**Glazing** Costs for glazing on the invoice can be shown in different ways.
- **Calculate in item:** costs for glazing are included in the item calculation.
- **Only show in footer:** costs for glazing are shown in the footer of the invoice.
- **In item and footer:** costs for glazing are included in the item calculation and shown in the footer of the invoice.
Technical info: toggle field, DB field: kauf.verglaskz

**Print Article Text** The article texts can be printed on the market partner documents.
- Y = print product text.
- N = do not print product text.
Technical info: toggle field, DB field: kauf.atxtdrukz

**Print Shapes** Print shape sketches for items in the attachment of the market partner documents.
- Y = print shape sketch.
- N = do not print shape sketch.
The setting of Y or N in this field is evaluated depending on the configured report variant, either repgo or Crystal Report.
Technical info: toggle field, DB field: kauf.moddrkz

**Suppress Item Prices** By default, the item prices are printed on the market partner documents. You can suppress the listing of the item prices, e.g. if you have agreed on a fixed price with the customer for the whole order.
- Y = do not print item prices.
- N = print item prices.
Technical info: toggle field, DB field: kauf.posdrkz

#### Footer

The fields and buttons in the footer area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

The fields can only be entered if at least one item is entered. Use `<End>` to change from the item level to the footer area.
