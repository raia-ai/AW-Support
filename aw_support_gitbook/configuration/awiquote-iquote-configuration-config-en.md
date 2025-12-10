---
description: "A+W iQuote v6 Configuration Instructions"
---


# A+W Configuration Instructions: A+W iQuote v6

**-INTERNAL-**

*A+W - Software for Glass*

---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2015-01-14 | D. Langsdorf | Release version | 13.0.0 |
| 2015-09-01 | D. Langsdorf | SN configuration | 13.0.1 |
| 2015-10-05 | D. Langsdorf | Print server configuration | 13.0.2 |
| 2015-12-14 | D. Langwald | Master data consolidation before introduction of iQuote | 13.0.3 |
| 2015-12-14 | D. Langsdorf | Workflow configuration | 13.0.4 |
| 2016-01-14 | D. Langsdorf | Reworking | 13.0.5 |
| 2016-01-18 | D. Langsdorf | Decimals of sizes | 13.0.6 |
| 2016-01-28 | D. Langsdorf | Activities Model Mapping | 13.0.7 |
| 2016-01-29 | D. Langsdorf | Description of article images | 13.0.8 |
| 2016-02-10 | D. Langsdorf | Business Case configuration | 13.0.9 |
| 2016-02-12 | D. Langsdorf | Production area and document numbers | 13.0.10 |
| 2016-02-19 | D. Langsdorf | Print Job documentation adjusted | 13.0.11 |
| 2016-03-04 | D. Langsdorf | Rounded corners parameter values 2.3 | 13.0.12 |
| 2016-04-15 | D. Langsdorf | Correction of business cases | 13.0.13 |
| 2016-06-23 | D. Langsdorf | Macro recording configuration 2.12 | 13.0.15 |
| 2016-09-30 | D. Langsdorf | Workflow Properties built-in | 13.2.1 |
| 2016-10-24 | D. Langsdorf | Variants of implementation | 13.2.2 |
| 2016-11-29 | D. Langsdorf | Exchange groups not for gas 2.4 | 13.2.3 |
| 2017-01-05 | D. Langsdorf | Product release and sorting | 13.3.1 |
| 2017-01-23 | D. Langsdorf | Box sales 4.3 + 2.13 | 13.3.2 |
| 2017-02-02 | D. Langsdorf | Check in workflow 4.4 | 13.3.3 |
| 2017-02-17 | D. Langsdorf | Self pick-up 4.5 + 2.14 | 13.3.4 |
| 2017-02-27 | D. Langsdorf | Commission and customer PO number 2.15 | 13.3.5 |
| 2017-03-22 | D.Langsdorf | Restriction of the processings 2.16 + 4.3 | 13.3.6 |
| 2017-03-30 | D. Langsdorf | History for A+W Business documents 2.17 + 2.18 | 13.3.7 |
| 2017-04-20 | D. Langsdorf | Document attachments in history 2.18 | 13.4.1 |
| 2017-05-02 | D. Langsdorf | Report attachments in history 2.19 | 13.4.2 |
| 2017-07-03 | D. Langsdorf | Save the shopping cart and the configuration 2.20 | 13.4.4 |
| 2017-08-03 | D. Langsdorf | Total thickness for insulated glass 2.21 + Show IG structure 2.22 | 13.4.5 |
| 2017-09-26 | D. Langsdorf | Addition of property total thickness IGU 2.21 + 4.3 | 13.4.7 |
| 2017-10-13 | D. Langsdorf | Color selection for products 2.23 + 4.3 | 13.4.8 |
| 2018-01-10 | D. Langsdorf | Filtering of products and ISO exchange 2.24 + 4.7 | 13.4.1525 |
| 2018-07-20 | D. Langsdorf | IG replacement with spacer colors 2.26 + 4.3 | 13.4.2201 |
| 2018-10-22 | D. Langsdorf | AutoCollapsible property Workflow Activities 4.6 | 13.4.2538 |
| 2018-10-22 | D. Langsdorf | Multilingual Workflow 4.8 | 13.4.2538 |
| 2018-11-21 | D. Langsdorf | Processing parameters min/max values 2.3.2 | 13.4.2538 |
| 2018-11-21 | D. Langsdorf | New workflow definitions 4.2 | 13.4.2538 |
| 2018-12-10 | D. Langsdorf | Dynamic values for workflow 4.9 | 13.4.2538 |
| 2019-02-26 | D. Langsdorf | Color filter and special colors 2.27 + 4.7 | 13.4.2705 |
| 2020-05-04 | D. Langsdorf | Sorting the processing types with filters 2.16 | 13.4.3805 |
| 2019-05-04 | D. Langsdorf | Printout with Crystal Reports 2.9 | 13.4.3805 |
| 2020-06-18 | D. Langsdorf | 2-phase commit with document creation (breaking change) 2.6 + 2.28 | 13.4.3924 |
| 2020-08-10 | D. Langsdorf | File upload and web links 2.29 + 4.3 | 13.4.4104 |
| 2020-08-11 | D. Langsdorf | Access to internal data structures in the workflow 4.10 | |
| 2020-09-23 | D. Langsdorf | Pattern/coating side and side for single glass 2.30 + 4.3 | 13.4.4263 |
| 2020-11-26 | D. Langsdorf | Project selection with products 2.31 + 4.4 + 4.7 | 13.4.4448 |
| 2021-01-05 | D. Langsdorf | Creation of processings from the workflow 2.32 + 4.7.1 | 13.4.4499 |
| 2021-02-01 | S. Weil | Filter by name (single and IG) 2.25 | 13.4.4569 |
| 2021-03-05 | D. Langsdorf | Set Bestelltext2 for the 3 entry paths (evaluate entry quote) 2.33 | 13.4.4569 |
| 2021-03-24 | D. Langsdorf | Extension of mapper workflow added, processing with "ActionMapperAddAction" 4.6 | 13.4.4670 |
| 2021-06-22 | D. Langsdorf | Customer's own icon for the browser 3.3 | |
| 2021-07-06 | D. Langsdorf | Customer's own texts for the user interface 3.4 | 13.4.4899 |
| 2021-11-22 | D. Langsdorf | Product filter for processings 2.34 + 4.7 | 13.4.5228 |
| 2022-01-11 | D. Langsdorf | Suppress credit limit message 2.35 | 13.4.5350 |
| 2022-01-21 | D. Langsdorf | Model filter in the workflow 4.3 + 2.36 | 13.4.5357 |
| 2022-03-11 | D. Langsdorf | Takeover of the CSS customizing possibilities 6 | 13.4.5500 |
| 2022-05-10 | D. Langsdorf | History with exact status release 2.37 | 13.4.5596 |
| 2022-11-28 | D. Langsdorf | Multi-sites and load distribution 2.38 | 13.4.7459 |
| 2023-07-10 | D. Langsdorf | Product widget by product groups and article numbers from-to 4.3 | 13.4.9342 |
| 2023-07-28 | D. Langsdorf | Checkbox widget for GTCs and HTML widget designations 2.39 and 4.5 | 13.4.9433 |
| 2023-10-06 | D. Langsdorf | Login page configuration 7 | 13.4.10144 |
| 2024-01-16 | J. Nießner | Login Page Okta | |
| 2024-01-29 | J. Nießner | Okta login page reworked | |

## Content

- **1. System Configuration**
    - 1.1. Infrastructure Configuration
    - 1.2. Business Case Configuration
- **2. Configuration**
    - 2.1. Enable customer employees
    - 2.2. Enabling products, shapes, and processings
    - 2.3. Processing parameter values Restrictions
        - 2.3.1. Processing parameter limit values for round corners
        - 2.3.2. Processing parameters min/max values
    - 2.4. Definition of the IGU exchange groups
    - 2.5. PS area assignment for iQuote User
    - 2.6. Status allocation
    - 2.7. Enabling status points
    - 2.8. PS order area assignment and document numbers
    - 2.9. Printout and mail sending with Crystal Reports
    - 2.10. Number of places after the decimal point for dimensions
    - 2.11. Setting up an iQuote user
    - 2.12. Configuration of the Macros
    - 2.13. Setting up stock dimensions and boxes
    - 2.14. Self pick-up
    - 2.15. Commission and customer PO number
    - 2.16. Restriction of the processings in the workflow
    - 2.17. History display of A+W Business documents
    - 2.18. Document attachments in the history display
    - 2.19. Report attachments in the history display
    - 2.20. Save the shopping cart and the current configuration
    - 2.21. Total thickness for insulated glass and product designation
    - 2.22. Insulated glass product designation 2 as structure
    - 2.23. Product colors for items
    - 2.24. Product and ISO exchange filter
    - 2.25. Filter by name
    - 2.26. Spacer colors in IG replacement
    - 2.27. Color filter and special colors
    - 2.28. 2-phase commit with document creation
    - 2.29. File upload and web links
    - 2.30. Pattern/coating side and side for single glass
    - 2.31. Project selection with products
    - 2.32. Creation of processings from the workflow
    - 2.33. Set document flags per entry path
    - 2.34. Product filter for processings
    - 2.35. Suppress credit limit message
    - 2.36. Model filter for geometry entry
    - 2.37. History with exact status release
    - 2.38. Multi-tenancy and load distribution
    - 2.39. Checkbox widget and HTML designation
- **3. System Configuration**
    - 3.1. Integration into a start page
    - 3.2. Setting up the product images
    - 3.3. Customer's own logo for the browser
    - 3.4. Customer's own texts for the user interface
- **4. Workflow**
    - 4.1. Workflow Studio
    - 4.2. Workflow Management
        - 4.2.1. Configurator Extension Point (0000)
        - 4.2.2. Mapper Extension Point (0001)
        - 4.2.3. Check In Extension Point (0002)
        - 4.2.4. Check Out Extension Point (0003)
        - 4.2.5. Document Validation Extension Point (0004)
        - 4.2.6. Add To Cart Extension Point (0005)
        - 4.2.7. Backend Update Extension Point (0006)
    - 4.3. Activities Configurator
    - 4.4. Activities Checkin
    - 4.5. Activities Checkout
    - 4.6. Activities Model Mapping
    - 4.7. Activities Methods
        - 4.7.1. Modify Processings
    - 4.8. Multilingual Workflow
    - 4.9. Dynamic values for the workflow
    - 4.10. Access to iQuote data structures
- **5. Master data Consolidation**
    - 5.1. Exact product designations
    - 5.2. Drillings for different diameters
    - 5.3. Recording the correct edge processings
    - 5.4. Use of color variants
    - 5.5. Tempered glass always with a complete bill of materials
- **6. CSS Customizing**
    - 6.1. General and basic principles
    - 6.2. How Custom Theme works
    - 6.3. Overriding rules and own CSS rules
    - 6.4. Background color in the main menu
    - 6.5. iQuote navigation bar colors
    - 6.6. Configurator navigation bar colors
    - 6.7. Change loading icon
- **7. Login Page Configuration**
    - 7.1. First login as administrator
    - 7.2. Pages
    - 7.3. Users
    - 7.4. Links
    - 7.5. Settings
    - 7.6. User self-registration and password reset
    - 7.7. Customizing the Login Page
        - 7.7.1. View Layout for Customizing
        - 7.7.2. Custom Header and Footer
        - 7.7.3. Adding a View in the Menu
        - 7.7.4. Access to customer texts
        - 7.7.5. Adapting customer emails
- **8. Login Page Okta Configuration**
    - 8.1. Okta Platform Configuration
        - 8.1.1. Creating a group and assigning a tenant
        - 8.1.2. Creating a user and linking to an ERP customer
        - 8.1.3. The standard customer
    - 8.2. Configuration of “A+W iQuote Login Page Okta"
    - 8.3. Preparing iQuote for the Okta Login
    - 8.4. Customization

---

# 1. System configuration

## 1.1. Infrastructure Configuration
Please start the Web interface of the Infrastructure Services.

*(Image showing the Windows Start Menu path: Local Disk (C:) > ProgramData > Microsoft > Windows > Start Menu > Programs > A+W. The "A+W Infrastructure 6 Web" shortcut is highlighted.)*

Now select the Configuration dialog.

*(Image showing the A+W Infrastructure Services web interface. The main menu on the right has "Configuration" highlighted.)*

On the Configuration dialog, the database connection of the A+W Business COM is entered first.

*(Image showing the System Switch Management screen within the Infrastructure Services. The "A+W Business" section is shown with fields for Database Connection: Host Name, Instance, Database, Windows Authentication, User, and Password.)*

In the A+W Business User area, the logical Business User must be entered.

*(Image showing the "A+W Business User" subsection with a "User" and "Password" field. The "User" field is highlighted.)*

In its number manager, the purchase orders are collected by iQuote.

Under Company logo file name, a deviating company logo can be entered. This file must be in the Context directory. It is suggested that this is organized in a subdirectory. It should contain all content for the customer.

*(Image showing the "Company Logo File Name" field with an example path `awsoa/images/logo.png`.)*

It must be specified which back end is operated under iQuote: A+W Business or Cantor.

*(Image showing the "Back End" dropdown menu with "A+W BUSINESS" selected.)*

In the Web settings, it is possible to change the appearance of the Website; for iQuote, please select the "Web" tab.

- **Advertising file name:** The advertising on the left side of iQuote can be filled with several image files, they are displayed in alternation, the files must be separated with a semicolon (e.g. "ads1.jpg;ads2.jpg").
- **Background file name:** The background image can be entered here.
- **Schema:** Under schema, you can search for one of the existing ones or select custom if you have selected an individual one.
- **Specify schema:** If the schema is not specified, then under "Schema" you set the default. This can be overwritten by the cookie (by other A+W Websites) or via URL (Web.Web/?theme=black). If you would like to force Website users to use the pre-set theme, you can specify the schema.

*(Image showing the "Website Settings" for the iQuote web tab, with fields for "Advertise file name", "Background file name", "Theme", and "Theme is Mandatory".)*

The workflow must be determined; to do this, please select the workflow management.

*(Image showing the A+W Infrastructure Services web interface. The main menu on the right has "Workflow" highlighted.)*

The appropriate workflow must be set.

*(Image showing the Workflow Management screen. A table lists Extension Points and their corresponding Workflows. The row for "0000 - iQuote Configurator" is highlighted.)*

- The expansion point **000-iQuote Configurator** is the workflow for the display of the widgets and controls which queries are displayed.
- The expansion point **001-iQuote Assignment** handles the assignment/mapping of the data structures of the front end into the back end. Normally nothing must be done here.
- The expansion point **002-iQuote Check In** handles the display of the widgets before the configuration process.
- The expansion point **003-iQuote Check Out** handles the display of the widgets after the configuration process.

## 1.2. Business case configuration
The possible functions in iQuote are controlled via business cases. This can be managed in the infrastructure configuration. The functions can be switched on or off per business case.

Please start the Web interface for the infrastructure via Configuration > Business case functions. You can manage the functions there.

*(Image showing the "Business case functions" screen. A table shows various functions (e.g., Show overviews, Print reports, Quotation to order) as rows, and business cases (e.g., Dealer, Trading company, Customer order) as columns, with checkboxes to enable/disable each function for each case.)*

The business cases are listed horizontally; this must be entered in the A+W Business customer employee management. The business cases are fixed and the default for an employee is "Access declined". It must be heeded that after a change, the IIS must be started anew, as these settings are cached.

| Function | Description |
| :--- | :--- |
| **Display overviews** | Display quotation and order overviews |
| **Form printing** | Allow printout of an entry confirmation |
| **Order export** | Only Cantor (disable A+W Business) |
| **Request order export** | Only Cantor (disable A+W Business) |
| **Quotation to order** | Copy quotation to order |
| **Quotation to quotation** | Copy quotation to quotation |
| **Order to order** | Copy order to order |
| **Order to quotation** | Copy order to quotation |
| **Back up shopping cart** | Allows the saving/caching of the shopping cart and the last configuration |
| **Direct check-out** | Allows the transfer of the shopping cart to ERP (order) |
| **Enter quotations** | Allow entry of quotations |
| **Enter orders** | Allow entry of orders |
| **Display prices** | Display prices; otherwise the user does not have any prices |
| **Price Change** | Only Cantor (disable A+W Business) |
| **All documents in history**| Determines to display documents in history that are not entered in iQuote. |

# 2. Configuration

## 2.1. Enable customer employees
The customer's employee must be enabled for iQuote and the mail address and password/PIN must be assigned.

*(Image of the A+W Business customer employee screen. Highlighted fields are "E-Mail/Login", "Password", "Unlock" button, and "Business case" dropdown.)*

The business case must be assigned; through this it is possible to determine which functions are available in iQuote.

## 2.2. Enabling products, shapes, and processings
**Release**
Items, shapes, and processings must be enabled in product management. This also affects the insulated glass; the exchangeable components are defined by the IGU exchange groups. These products do not have to be released explicitly. However, then no determination of the sequence is possible. The customer determines what should be activated here and the workflow created.

*(Image of the A+W Business product screen. The "iQuote" section is highlighted, showing a "Release" checkbox and a "Sort" field.)*

**Sorting**
In addition to the release of the products for iQuote, the sequence of the products in iQuote can be determined; for this the entry of the sorting key is necessary. If this is on 1 (default), then the sorting is always done by product number. However, the sorting key takes precedence and thus it is possible to get a sensible sorting of the products (e.g. by thickness) even if the product numbers are not ascending by thickness.

## 2.3. Processing parameter values Restrictions

### 2.3.1. Processing parameter limit values for round corners
The iQuote user should only be able to enter defined values for round corners; intermediate dimensions should be avoided for production-technical reasons. For this, a round corner must be selected in the product master data and the value with text entered on the Radius field of the Processing parameters dialog. For the entry of the processing, only a rounding of 5,10,15 is possible. You must pay attention that the default value matches an entry. Otherwise, there will be inconsistent display behavior.

*(Image of the processing parameters dialog for a round corner, showing a dropdown for the "Radius" parameter with options like "5 mm", "10 mm", "15 mm".)*

### 2.3.2. Processing parameters min/max values
In the production master data of A+W Business, it is possible to define the minimum dimension and the maximum dimension for edge cutouts, area cutouts, notched corners, and corner cut-offs. For round corners and holds, this is according to the diameter.

*(Image of the product master data screen showing P.O. parameters "Max. width P.O." and "Max. height P.O.", and Stock control parameters "Max. width stock" and "Max. height stock".)*

From the values for warehouse and purchase order, the maximum values will be used in iQuote. The input of a larger or smaller value is not possible and iQuote will jump back to the maximum or minimum value.

## 2.4. Definition of the IGU exchange groups
Definition of the IGU exchange groups serves to guide the user precisely. Thus, for example, it is no longer possible to exchange a TG for an ornamental glass in the IGU.

*(Image showing the "Exchange groups" definition screen in A+W Business Master Data.)*

**Assignment of the products to the exchange groups**

*(Image showing the "Product allocation" screen, where individual products are assigned to the previously defined exchange groups.)*

Assignment of the exchange groups to each BOM element spacer and glass. Only then is an exchange possible in iQuote.

*(Image showing the Bill of Materials (BOM) setup for an IGU, with the "Group for BOM exchange" field highlighted and set to "Spacer Alu".)*

> **Warning:** Gases cannot be exchanged in iQuote.

## 2.5. PS area assignment for iQuote user
Assign production area for the user who was determined as Business User in the configuration management. It is recommended that you create an individual iQuote user here.

*(Image of the A+W Business employee settings screen. Under "Input parameters", the "Order area" for "Quotations" is highlighted.)*

The quotations and orders for iQuote are created in this production area.

## 2.6. Status allocation
Via the Change 24-iQuote status point, it is controlled up to which order status the user can change a procedure in iQuote. The lock status must be set to this document status. The user status is assigned in case of change, may not be over the lock status. Otherwise only one change is possible.

*(Image of the "Status allocation" screen in A+W Business Master Data. The configuration for status point "024-Web-Konfigurator ändern" is shown, with "User status", "Min. status", and "Lock status" defined.)*

**Expansion: 2-phase commit**
The order in A+W Business is first created with the status of the status point 502 – deletion release. Only in the release phase is the status of the status point 1 entry assigned to the document and the further processing started (commit, ...) An assignment of the status point 502 is thus always required.

## 2.7. Enabling status points
The user can only see the history points that are enabled in the status points for iQuote. Here at least the points 1, 2, 4, and 8 should be enabled.

*(Image of the "Status Points" management screen. The "Release for web-configurator" column with checkboxes is shown.)*

## 2.8. PS order area assignment and document numbers
Documents that are entered with iQuote receive their document numbers from the number range of the default production area of the employee who is entered as A+W Business User. The default assignment can be found on the A+W Business employee dialog.

*(Image of the Infrastructure Services configuration, highlighting the "A+W Business Login" section where the default Business User is defined.)*

However, this is only the case if in the assignment workflow, a mapping to the default production area of the customer consultant of the entering customer was not undertaken.

*(Image of the iQuote Mapper workflow in Workflow Studio. An activity named "Get Consultant Department" is highlighted, which maps the WebDocument.Department.)*

## 2.9. Printout and mail sending with Crystal Reports
For the set-up of automatic confirmation mail or any other form printout with Crystal Reports, the workflow "...Formula\ExchangeService\workflow_print_documents.txt" has to be used. See also A+W Business Configuration Chapter 10.26.

## 2.10. Number of places after the decimal point for dimensions
In the glass area, a dimension in the millimeter range is always entered; only in the area of furniture glass is there work with 1/10 millimeter precision. In order to satisfy this, iQuote can be set flexibly.

In the company parameters, on the System tab, the number of places after the decimal point can be set.

*(Image of the A+W Business company parameters screen, on the "System" tab. The "Metric digits after colon" field is highlighted and set to 0.)*

If you enter a 0 here, then no more decimal places can be entered in iQuote. The step change is displayed to 1, 5, 10, 100 instead of 0.1, 1, 10, 100.

## 2.11. Setting up an iQuote user
The iQuote user is entered in A+W Business under Master Data -> Partner -> Customers. Please select a customer and use the functions to reach the employees.

On the employee dialog, it is possible to configure access under the iQuote group. Activate the [active] check box and enter the e-mail address as login. Now assign a password and define the business case under the employee who should work with iQuote. Use the [Unlock] button to enable a locked login. The locking happens after an incorrect password has been entered three times.

*(Image of the customer employee dialog, highlighting the "iQuote" section with the "Active" checkbox, "E-Mail/Login", "Password", and "Business case" fields.)*

## 2.12. Configuration of Macros
iQuote can record all familiar macro types (corner, edge, area macros and their parameterizable types). The macros are released in A+W Business for iQuote like any other processing.
Important is that the SN macro files are reachable via the UNC path for the Commercial Document Service.

*(Image of A+W Business company parameters, "System" tab, showing the "Path to product images" field, which is used for SN macro files.)*

In iQuote, a new macro icon appears. The positioning is done as in the corresponding processings (corner, edge, interior cut-out). In addition, the parameters of the parameterizable macros are queried. The defaults for the parameters are taken from the CAD file and overwritten by the stored defaults from A+W Business.

*(Image of the iQuote processing selection screen, showing the "Macro" icon and a parameter entry dialog for a selected macro.)*

## 2.13. Setting up stock dimensions and boxes
With the new widget Stock Dimensions, iQuote now supports the sale of boxes and stock dimensions.
In the stock dimension management `Master Data > Products > Product > Stock Dimensions`, it is possible to release the stock dimension/box and assign a screen to the stock dimension. This screen will be displayed in iQuote, but must be present on the IIS. The content path of the widget in the workflow determines where it appears.

*(Image of the iQuote workflow properties for the Stock Dimensions validator, showing the "ContentPath" property.)*

The box is taken over in the order as if it had been recorded in the order entry, including stock reservation and later removal from stock. The stock on hand is displayed in iQuote with a traffic light.

*(Image of the iQuote screen showing a list of "Stock Sizes + Boxes" with an "Availability" column that uses a traffic light system (green for "On stock", yellow for "Only 9 on stock").)*

With a Stock > minimum stock the stock availability is green, with >0 and < minimum stock it is yellow and with stock 0 it is red. The stock is only displayed if the box/stock dimension is created in the stock.

If no image file is stored in the stock dimension, the display is handled with the CAD sketch; otherwise, the stored image is displayed.

If the box was released incl. the boxes with Ident. no, then these also appear.

*(Image showing the stock sizes list, now including individual boxes with unique "Identification #"s.)*

The price calculation is done as box price or stock dimension price.

## 2.14. Self pick-up
Self-collection can be defined in the check in/out workflow. Here, a collection is filled in the workflow, which includes the self-collection dates available for selection. For example, these can be distinguished according to morning and afternoon collection.

*(Image of the iQuote checkout screen showing a "Delivery" section with a dropdown for "Self collect" options, e.g., "Morning until 12.00".)*

This data is entered as "KeyValue" object in the workflow, whereby the key with the alphanumeric key must match the route in A+W Business.

*(Image of the iQuote workflow in Workflow Studio. The properties for a "SelfCollects" collection are shown, highlighting how KeyValue pairs like "800: Morning" are added.)*

Depending on the self pick-up, the route is then implemented in the order and the order can be provided at the desired time and date. If the collection is not filled with values, then the selection of self pick-up is not displayed.

*(Image of the A+W Business routes table, showing different routes for pickup and delivery.)*

## 2.15. Commission and customer PO number
The commission and customer PO number that are entered during the iQuote configuration are now also visible in the history overview. The user can use these to limit and filter the documents.

*(Image of the iQuote "My Orders" screen, showing columns for "Purchase order no" and "Reference". Filter options for these columns are also visible.)*

All commissions of a document are displayed separately with "-".
The columns can be moved and hidden.

## 2.16. Restriction of the processings in the workflow
The iQuote workflow can now restrict the processings available; this can make sense if for particular products such as kitchen backsplashes, only particular macro processings may be applied. Similarly for particular shapes such as the circle, for example, the application of corner cut-outs is not possible.

Initially, 2 variables must be created and initialized.

| Variable Name | Type | Scope | Default Value |
| :--- | :--- | :--- | :--- |
| ProcessingTypeFilter | CartItemActionFilter | Workflow Core | New CartItemActionFilter() |
| SelectedGeometry | GlassShape | Workflow Core | New GlassShape() |

These serve to accommodate the selected geometry and the filtering of the processings.
The filters are defined in a sequence activity by deleting and adding the filter collection.

**Deleting the filters:**
*(Image showing a `ClearCollection` activity in the workflow to clear the `ProcessingTypeFilter.SelectedFilters`.)*

**Inserting the filters:**
*(Image showing an `AddToCollection` activity in the workflow. The expression editor shows adding a new `FilterDescription` with a "Member" (product group) and "Value" (comma-separated list of processing product numbers).)*

The "FilterDescription" must be filled with the A+W Business product group in "Member" and with a list of processing product numbers separated with commas. If the "Value" is empty, then all products of this product group are permitted.

The filter object must be assigned the property `ProcessingFilter` of the `ActionValidatorProcessing`.

*(Image showing the properties of the `ActionValidatorProcessing` activity, with the `ProcessingFilters` property set to the `ProcessingTypeFilter` variable.)*

Here in the example, there is a different processing filtering according to selected model. The property for this in the `ValidatorGeometry` is `SelectedGeometry`.

*(Image showing the properties of the `ValidatorGeometry` activity, with the `SelectedGeometry` property highlighted.)*

And attach a switch activity to the `SelectedGeometry` object, now it is possible to define a different filter by shape number.

*(Image showing a `Switch` activity in the workflow, with its `Expression` property set to `SelectedGeometry.ShapeNo`.)*

**Sorting the processing types**
The sequence of the filters defines the sequence of the processing types in the processing entry of A+W iQuote. Simply shift the filters in the workflow sequence and the sequence is changed.

*(Image showing a sequence of filter activities in the workflow: Internal Cuts, Edge Cuts, Rounded Corners, etc.)*

## 2.17. History display of A+W Business documents
Via the business cases, it is possible to set the history (overview) using the "All documents in history" entry so that all of the customer's documents are displayed. That is, documents that were not entered in iQuote can thus be displayed and their status history called up.

These documents cannot be edited in iQuote. For each glass item, the SN sketch is created and displayed in the item view.

*(Image of the iQuote item overview for a document not created in iQuote, showing a CAD sketch of the glass item.)*

This function represents the first step toward the expansion of iQuote into a customer information system.

## 2.18. Document attachments in the history display
Document header attachments can now be displayed in the history for iQuote. This applies for quotations and orders. The documents can be downloaded or viewed using the link or the button in the browser. For display, the appropriate client software is required (PDF viewer, Office, etc.).

*(Image of the iQuote history screen showing an "Attachments" tab with links to download attached files.)*

In the browser, it is now possible to select whether the file is saved or displayed.

Which attachments are visible for the iQuote user is controlled by the file attachment types (`Master Data > Texts > File attachment types`).

*(Image of the A+W Business "File attachment types" screen, showing a "Release iQuote" checkbox for each type.)*

## 2.19. Report attachments in the history display
In addition to the document header attachments, form printing generated in A+W Business (quotation, order confirmation, delivery note, and invoice) can also be enabled for iQuote. The condition for this is that the form printing was generated with the new Crystal Report Print Service. Only in this case is forwarding to iQuote possible.

To activate the forwarding, the `Handover to iQuote` option must be activated per form in the form management (`Master Data > Forms > Form Management`). This is only available if the option `Form printing with Crystal Report` is activated in the system parameters.

*(Image of the A+W Business form management screen, with the "Transfer an iQuote" checkbox highlighted.)*

With this option, each printout is saved in the reporting service as a PDF. iQuote then displays these documents in the history.

*(Image of the iQuote history screen showing a "Reports" tab with a link to download a generated PDF report.)*

These can then be downloaded and displayed with the PDF viewer.

## 2.20. Save the shopping cart and the current configuration
iQuote is a Web application with which the browser can be closed at any time. Since the complete configuration is present in the browser and no document has yet been generated in A+W Business, everything is gone after closing. In order to prevent this, the configurator service now saves all data in a storage cache and persists this data in the database every 10 seconds. If the service is stopped, then the saving is done before the stopping, so that in case of a crash of the service, there is a maximum data loss of 10 seconds.

The storage of the configuration is activated with the business case option **Save Shopping Cart**.

*(Image of the Infrastructure Services Business Case Functions screen, with the "Save cart" option highlighted.)*

If now the user makes another product configuration, stores products in the shopping cart and does not end this configuration with an order, then this configuration is saved in iQuote and offered to him for the next configuration. This also works on another device. The user can thus cancel a session in the middle and continue it later on any end user device.

*(Image showing a notification in iQuote: "The following configurations were not completed", with options to Recover, Delete, or Display the saved configuration.)*

The user can load the canceled configuration, delete this configuration or display the contents of the shopping cart. If he does not want to continue the canceled configuration, he can begin a new configuration. The saved configurations are also retained for him.

## 2.21. Total thickness for insulated glass and product designation
iQuote now allows the entry of insulated glass with specification of the total thickness. The total thickness of the insulated glass unit is also displayed.

*(Image of the iQuote configurator for an insulated glass unit. A "Total Thickness" dropdown is shown with preset values like "28 mm [8-8]", "30 mm [8-10]", etc.)*

The thickness specification is retained if a glass is exchanged and the thickness specification can be achieved by changing the spacer. If not, then the thickness specification is deleted.

Starting with 3-layer insulated glass, the thickness specification is always deleted in case of exchange of the exchange glass and its thickness since there are various combination possibilities for the spacers here. The system cannot make an automatic specification here.

The various spacer combinations that belong to a total thickness are displayed in brackets.

Here, iQuote makes the user's life easier since it is also possible to select the spacer combinations purposefully; this is not possible in the A+W Business order entry.

Inch values are supported, however there is no metric thickness in an imperial database.

> **Note:** This function is not activated by default and must be activated in the validator exchange activity workflow with the property "ThicknessPresetHide".

> **Restriction:** The function conditions that in A+W Business the spacers are assigned per spacer type in a separate product group. Only this way is it possible to find the correct spacer. Colors are not currently supported, if these are just in the spacer text, then one product group must be created per color.

## 2.22. Insulated glass product designation 2 as structure
Via workflow, it is possible to configure the back end so that the insulated glass description 2 always consists of the structure (glass and spacers). Up to now, this was only the case if there was an exchange in the BOM. This is useful for customers who do not use the insulated glass description 2 and always specify the structure of the glass in the formula printing. Until now, this could not be displayed this way in iQuote.

*(Image showing the iQuote product details, where the product name is displayed as a full structure: "Insulated Glass Unit Float clear 4mm/12mm Spacer/Float clear 4mm".)*

For set-up, the iQuote workflow for the expansion point 1 must be added. In the `BackendPriceCalculation` activity, the `BackEndUpdateAction` property must be assigned a new object. In it, the property "ProductDescriptionMode" must be set to `ProductDescriptionModes.IsolatedGlassDescription2IsBom`.

```vb
New BackEndUpdateAction() With {.Image = true, .Price = true, .Restriction = true, .ProductDescriptionMode = ProductDescriptionModes.IsolatedGlassDescription2IsBom }
```

Examples with image, price, and restriction must always be set to "true." Otherwise, these actions will not be executed!

## 2.23. Product colors for items
For the selection of product colors in iQuote, the available colors must be assigned to the product.

The RGB color codes must be entered in the colors so that the tiles are displayed in the appropriate color. If the RGB value can not display the color attractively, you can also assign a PNG file. It must be stored in the ContentPath of the widget (e.g. `content\auw\colors`) and the file name must include the variant number with the suffix .png (e.g. `8001.png`). This file is mainly displayed; the image size should not exceed 80x80 pixels.

*(Image of the A+W Business variants screen, showing a list of colors with their preview, RGB code, and other properties.)*

Presently, special colors are not displayed.

In the workflow, the "ProductColor" validator can be inserted into the branch. The product selected in the product validator must go into the color selection as input parameter.

*(Image of the iQuote workflow showing a `ValidatorColors` activity being used, which takes a `productid` as input.)*

For example, this can be done conditionally for some product codes.

## 2.24. Product and ISO exchange filter
In iQuote, it is now possible to use the product filter added in the workflow to filter the available products. This way, the total number of products can be reduced to a few. This applies both for the product selection (single glass, items) as well as for the ISO exchange products (glass and spacers). Therefore it is possible to select the spacers by spacer types or thicknesses, for example.

*(Image of the iQuote IG exchange screen showing filters "by Thickness" and "by Product Group" being applied to the list of available spacers.)*

For setup, there must be an assignment of the filters according to the product validators in the configuration workflow. For parameterization, the functions are described in Chapter 4.7.

Important is that the first filter always gets the option `ClearFilter = True` so that the filter collection can be deleted.

The values of the filters display only the values that actually occur in the complete selected hit quantity. The filters always represent an AND link; only the values within a filter are OR linked. Thus, for example, the selection of the thicknesses 5, 6, 8 mm.

Currently, there are filters available for the following functions:
- Thickn.
- Product type
- Product class

For setup examples, see the standard workflow. The sequences can simply be copied from there and attached to your own workflow.

The filter methods for exchange glass can be attached by product type, that is, for float, TG, LSG, and spacers. For exchange filters, the filters can differ per BOM element. This is achieved since the filters are inserted per product type. See filter definition in the example. With the filter methods `...ByTuple`, however, it is also possible to attach a filter purposefully to the 2nd spacer.

The filters with `...Collection...` allow a free definition of the values to be filtered.

## 2.25. Filter by name
In iQuote, it is now possible to use an added filter in the workflow, which filters the available products by their names. This way, the total number of products can be reduced further with the other filters. The filter can be defined both for the product selection (single glass, articles) as well as for IG exchange products (glass and spacers).

*(Image of the iQuote IG exchange screen, showing an "Exchange by Description" filter, where typing "Float clear" filters the list of available glass.)*

For setup, there must be an assignment of the filters according to the product validators in the configuration workflow.

*(Image of the iQuote workflow, showing various "AddFilters" activities being used for thickness, product type, and description for both single glass and IG exchange.)*

## 2.26. Spacer colors in IG replacement
Defined spacer colors can now be displayed in iQuote during IG replacement. This option `ColorHide` of the ValidatorExchange must be deactivated in the workflow; it is activated by default.

*(Image of the iQuote workflow properties for the `ValidatorExchange` activity, showing the `ColorHide` property set to `False`.)*

The assignment of the spacer variants must have been made in A+W Business.

*(Image of the A+W Business product variants screen, showing different colors (Blue, Brown, Bronze) assigned as variants to a "12 mm ALU" spacer.)*

The IG product structure is also displayed with the color in iQuote. If the glazing thickness is specified or the spacer changed, then the default color of the spacer is always selected again. This behavior is also implemented in A+W Business.

*(Image of the iQuote IG exchange screen showing colored swatches (White, Brown, Red, etc.) for selecting the spacer color.)*
