---
title: "EN-CONFIG-AW_Business-2"
source: "EN-CONFIG-AW_Business-2.pdf"
tags: ["A+W Business", "Software Configuration", "SQL", "ERP", "BMECat", "Article Import", "Product Classifiers", "Invoice Management", "Delivery Management", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides detailed configuration instructions for the A+W Business software, covering procedures, article imports, product management, and document handling. It includes SQL scripts, UI settings, and process flows for various modules."
long_description: "This technical manual is an internal configuration guide for A+W Business software. It outlines a series of procedures and settings to customize and manage the system's functionality. The document begins with a detailed breakdown of a stored procedure (PROC_TEMP) used for updating product data related to laminated and toughened glass. It then delves into article data management, explaining how to import articles using the BMECat standard from various manufacturers like Dorma, Pauli, and SWS, and how to configure settings for product prefixes, pricing, and master data. A significant portion is dedicated to the implementation and use of freely-definable product classifiers, including how to define them, enter values, and use them for searching and reporting with examples in SQL and Crystal Reports. The guide also covers advanced document management features such as active edgework entry support, assigning fittings to processings for items like studio doors, and checking spacers using the LeCheck system. It further details different modes of invoice and project management, generation of partial deliveries, and methods for calculating delivery dates using A+W Capacity and A+W Business Capacity Planner. Finally, it addresses specific functionalities like TPS/LSG invoicing, user-defined fields in document headers, status management per user group, and the turning of shapes in document entry."
---

---
## STORE PROC_TEMP

Note: e.g. for (laminated glass, product type = 3); for toughened glass, this must be changed to 2. In a second step, the documents will be changed.

### PROCEDURE: PROC_TEMP STATIC

**Local Variables**

- **Sql Handle:** hSqlCur1
- **Sql Handle:** hSqlCur2
- **Sql Handle:** hSqlCur3
- **Sql Handle:** hSqlCur4
- **Number:** nind
- **Number:** nBA_PRODUKT
- **String:** sProdArtVSG

**Actions**

**On Procedure Startup**
```
Call SqlConnect(hSqlCur1)
Call SqlConnect(hSqlCur2)
Call SqlConnect(hSqlCur3)
Call SqlConnect(hSqlCur4)
```

**On Procedure Execute**
```sql
Call SqlPrepareAndExecute ( hSqlCur1, 'SELECT BEZ FROM KA_PRODUKTART WHERE PRD_NR = 3 INTO :sProdArtVSG')

Call SqlFetchNext (hSqlCur1, nInd)

Call SqlPrepareAndExecute( hSqlCur1, 'UPDATE BA_PRODUKTE SET FER_BESCHAFFARTNR = 1 WHERE BA_PRODUKTART = :sProdArtVSG AND FER_BESCHAFFARTNR = 0')

Call SqlPrepare ( hSqlCur3, 'UPDATE BA_STUKL SET FER_BESCHAFFARTNR = 1 WHERE BOM_PRODUKT = :nBA_PRODUKT AND FER_BESCHAFFARTNR = 0')

Call SqlPrepare ( hSqlCur4, 'UPDATE BA_LAGMA SET FER_BESCHAFFARTNR = 1 WHERE BA_PRODUKT = :nBA_PRODUKT AND FER_BESCHAFFARTNR = 0')

Call SqlPrepareAndExecute ( hSqlCur1, 'SELECT BA_PRODUKT FROM BA_PRODUKTE WHERE BA_PRODUKTART = :sProdArtVSG INTO :nBA_PRODUKT')

While SqlFetchNext (hSqlCur1, nInd)
    Call SqlExecute (hSqlCur3)
    Call SqlExecute (hSqlCur4)
```

**On Procedure Close**
```
Call SqlDisconnect(hSqlCur1)
Call SqlDisconnect(hSqlCur2)
Call SqlDisconnect(hSqlCur3)
Call SqlDisconnect(hSqlCur4)
```

```sql
EXECUTE PROC_TEMP;
ERASE PROC_TEMP;

UPDATE BW_AUFTR_POS SET FER_BESCHAFFARTNR = 1 WHERE PROD_PRODART = 3 AND @MOD(POS_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_ANGEB_POS SET FER_BESCHAFFARTNR = 1 WHERE PROD_PRODART = 3 AND @MOD(POS_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_ANFR_POS SET FER_BESCHAFFARTNR = 1 WHERE PROD_PRODART = 3 AND @MOD(POS_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_BEST_POS SET FER_BESCHAFFARTNR = 1 WHERE PROD_PRODART = 3 AND @MOD(POS_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_GUTSCH_POS SET FER_BESCHAFFARTNR = 1 WHERE PROD_PRODART = 3 AND @MOD(POS_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BA_MAKRO_POS SET FER_BESCHAFFARTNR = 1 WHERE PROD_PRODART = 3 AND @MOD(POS_BIT/524288,2)!=1 AND FER_BESCHAFFARTNR = 0;UPDATE BA_MAKRO_POS SET FER_BESCHAFFARTNR = 1 WHERE PROD_PRODART = 3 AND @MOD(POS_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_AUFTR_STKL SET FER_BESCHAFFARTNR = 1 WHERE STL_PRODART = 3 AND @MOD(STL_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_ANGEB_STKL SET FER_BESCHAFFARTNR = 1 WHERE STL_PRODART = 3 AND @MOD(STL_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_ANFR_STKL SET FER_BESCHAFFARTNR = 1 WHERE STL_PRODART = 3 AND @MOD(STL_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_BEST_STKL SET FER_BESCHAFFARTNR = 1 WHERE STL_PRODART = 3 AND @MOD(STL_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BW_GUTSCH_STKL SET FER_BESCHAFFARTNR = 1 WHERE STL_PRODART = 3 AND @MOD(STL_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;

UPDATE BA_MAKRO_STKL SET FER_BESCHAFFARTNR = 1 WHERE STL_PRODART = 3 AND @MOD(STL_BIT/524288, 2)!=1 AND FER_BESCHAFFARTNR = 0;
```

## 1.8. Article Import

### 1.8.1. BMECat
Importing files in the format BMECat (standardized format of the Fraunhofer Institute) is carried out via the external BMECat importer. This is called up from the A + W business MDI functions menu. This program imports articles from manufacturers Dorma, Schlechtendahl, KL_Megla, Provitris, Pauli and SWS.

#### Settings
The settings for importing the articles can be made as follows in the company master data using tab 16: (> Company> Company data master data). Other settings can be set as follows:

*(Fig. 23 Company data shows the settings for BMECat Import, including configurations for various manufacturers like Dorma, Megla, Schlechtendahl, SWS, Provitris, and Pauli. It details settings for Template Product, Match Code Prefix, Price List, Variants, and options for importing Product Info and Pictures.)*

#### Pattern/template item
Since not all the relevant data for an item is going to be available in the import file, a sample item must be created for the product installation. For this item, all values must be entered that do not come with the import file (e.g. procurement type, product group...). This item needs to be selected for import.

#### Product prefix
The product prefix determines the match codes for the imported products. When importing, the external number for that article from the import file is appended to this prefix. Different prefixes should be chosen for each manufacturer. The product prefix also determines which products can no longer be used. Since at the start of the import, all products with this prefix will be decommissioned, and upon importing each product, the article is re-enabled, then all items that are not in the import file remain after import remain deactivated.

#### Pricing List/Code
Entering the pricing list and price key determines which tariff prices will be applied to the imported product.

#### Creating Product Numbers/Variations
This specification determines which number a new item should be inserted at. If an item that was not previously in the database is imported, then the next number available right above the entered number will be used. The same applies to creating prices for variations.

#### Importing abbreviations, product info and images
These options control whether the corresponding values for articles should be filled in:
- **Brief description:** The short name of the article can be filled out with the values from the import file using this option.
- **Product Info:** this option lets you fill in the product info for an article from the import file.
- **Images:** If an archive of product images still exists in addition to the import file, then in the option activated, they are transmitted to the product images folder. The image file name must be entered in the import file and it must exist in the digital photo archive.

#### Import
When importing a new file, the manufacturer's existing products are first blocked. Decommissioning is carried out for all products that begin with the article prefix that has been entered. Thereafter, the import file is read and the products with their variations are determined. Next, the products with variants and prices are imported. The left window shows the import progress. During the import of an item, the message "Item XXX is being processed..." appears. This text changes to "Item XXX imported successfully" if the import of the item was completed without errors.

### 1.8.2. B2B Article Import
Importing items from other formats is done via the master data > B2B > Product Import menu item. An import is possible for the following manufacturers:
- Dorma
- Bohle
- Pauli
- Velux
- Roto
- Roto2004
- Wolff
- SWS
- BET 2000
- Schlechtendahl

This should be the preferred method meanwhile for manufacturers for whom import files exist in the BMECat.

#### Settings
The following settings must be entered before importing:

*(Fig. 24 Article import shows the interface for importing Velux articles, with parameters for Matchcode prefix, Product Type, Product Group, Price List, and others.)*

#### Matchcode prefix
All of a manufacturer's products are created using the match code prefix that has been created here. The manufacturer's product numbers are attached to the prefix.

#### The product type, product group, WGR, WGR statistics, procurement type, type of stock booking
These values are used to create new articles and to update all imported articles.

#### Year, code, first price table for product colors
The tariff rate and the table numbers for newly created prices can be determined using these values.

#### sketches
Drawings can also be imported for articles.

#### Import
When importing a new file, the manufacturer's existing products are first blocked. Decommissioning is carried out for all products that begin with the article prefix that has been entered. Thereafter, the import file is read and the products with their variations are determined. Next, the products with variants and prices are imported. The table on the right tracks import progress.

## 1.9. Product classifiers
Starting with the version 13.03.138, freely-definable product classifiers are available for products. The definition of the usable classifiers can be undertaken in the master data:

*(Fig. in text shows the 'Klassifikatoren' (Classifiers) definition screen where classifiers like 'Certification', 'Color variation', and 'Year' can be defined with their properties.)*

Since the classifiers are saved in an XML column, the classifier name should not contain any special characters. Umlauts are allowed, however. Blank spaces in classifier names are replaced in the database with an underscore. However, this is filtered out in the display.

After the definition, the values for the classifiers for products can be entered.

*(Fig. in text shows the product master data screen where values for the defined classifiers (Year, Certification, Color variation) can be entered for a specific article.)*

If a value in the classifiers appears in red, this means that the classifier is no longer defined in the master data. The classifiers can only be created on the main product level. However, the classifiers are taken over into the BOM during entry. That is, if for the float glass 104 the classifier "Suitable for IG" is entered with the value "Yes," then all products that contain the product 104 in the BOM will take over this classifier if they are selected in the item entry. In the item entry, the values for the classifiers can be overwritten:

*(Fig. in text shows an order entry screen where classifiers for a BOM item are displayed and can be edited.)*

### Search
In the product search and in the order search, it is possible to search for classifiers.
In the product search, a new tab ("by classifiers") appears, on which a search can be performed using up to 5 different classifiers. In addition, in the lower area of the search dialog, there is an option whether the classifier entered must only be present in the main product or also in the BOM.

*(Fig. in text shows the product search dialog with the 'by classifiers' tab, allowing users to search for products based on classifier values.)*

In the order search, on the tabs "Item-related" and "BOM-related" it is possible to search by the classifiers:

*(Fig. in text shows the document search dialog, where users can search for orders based on classifier values in the 'Item-related' or 'BOM-related' tabs.)*

If a classifier is selected, the selection list is filled with the values that are stored in the products. The filling of the values from the documents cannot be executed due to performance reasons.

### Printing
In the form printing and the document view, the classifiers can be transferred to the report (see Chapter 3. Print variables).

For the item, the variables `F_PRCL_XXX` (whereby XXX is the classifier name) and BOM elements the variables `F_STX_PRCL_XXX` (whereby the first X is the number of the BOM element) are used. If the classifier contains a blank space, this must be replaced with an underscore in the variable name.

### Customizing
Should the classifier be used in a customizing, the value of a classifier can be read with the following command (in the example, "Name" and "Age" are the names of the classifiers):

**Insert records to the XML**
```sql
insert into [SYSADM].[XMLTEXT] (CLASSIFIERS) values('<Name>Müller</Name><Age>43</Age>');
insert into [SYSADM].[XMLTEXT] (CLASSIFIERS) values('<Name>Meier</Name><Age>43</Age>');
insert into [SYSADM].[XMLTEXT] (CLASSIFIERS) values('<Name>Fritz</Name><Age>44</Age>');
insert into [SYSADM].[XMLTEXT] (CLASSIFIERS) values('<Name>Max</Name><Age>46</Age>');
```

**Select the XML column**
```sql
SELECT ID, CLASSIFIERS.value('(/Name)[1]','varchar(100)') AS Name,
CLASSIFIERS.value('(/Age)[1]', 'Int') AS Age FROM SYSADM.XMLTEXT;
```

**Select the XML column with condition in where**
```sql
SELECT Id, CLASSIFIERS.value('(/Name)[1]', 'varchar(100)') AS Name,
CLASSIFIERS.value('(/Age)[1]', 'Int') AS Age FROM SYSADM.XMLTEXT
WHERE CLASSIFIERS.value('(/Name)[1]', 'varchar(100)')='Müller';
```

For access to the production classifier in the item or BOM from customizing code, the function `udf_GetClassificator()` is used.
`m_Pos[m_nCurltemIdx].udf_GetClassificator( 'Supplier', m_sUdv[0], g_sqlUdv[0])`

Changing of the product classifiers is currently not implemented.

### Crystal Report
In Crystal Reports, the following notation can be used to print the classifiers:

*(Fig. in text shows the Crystal Reports interface in Visual Studio, demonstrating how to construct an SQL query to extract data from an XML column. The query shown is `SELECT Id, XMLData.value('(/Name)[1]', 'varchar(100)') AS Name, XMLData.value('(/Age)[1]', 'Int') AS Age FROM SYSADM.XMLTEXT`. A second image shows the resulting report with columns for Id, Name, and Age, populated with data extracted from the XML.)*

## 2. Documents

### 2.1. Active entry support of edgework
To simplify and speed up the entry of edgework, a new functionality has been added to processing entry that has to be activated in the company master data.

*(Fig. in text shows the company master data settings for document entry, highlighting the 'Delete inferior edge processing' option.)*

With this option, the presence of more than one edgework on one edge is prevented, e.g. as a result of incorrect entry. Tempered glass manufacturers set up their glass in the master data with one edgework. If you wished to enter a different edgework than the original edgework in the master data, i.e. arrissing, e.g. by replacing it with polishing, you used to have to remove the arrissing manually and then enter polishing.

This is no longer necessary with this option. Edgework entry makes sure that there can only be one edgework per edge. If an edge is marked, edgework entry automatically disables all other edgeworks that apply to the same edge. If no more edges are marked for edgework, edgework entry will remove these excessive edgeworks automatically. This deletion is performed when returning to item entry.

If, for instance, a manually added edgework for TG is removed, and an edgework has already been entered in the master data of the TG, this edgework is transferred fully automatically from the master data into the item. This only happens with TG, since each edge for this type of product must always be processed before tempering.

### 2.2. Assigning fittings to processings
This functionality enables the creation of e.g. studio doors by means of the simply entry of fittings. During assignment, left and right side mounting is always differentiated. This setting can be changed during subsequent entry.

This functionality is currently only practical for shapes with four edges, as the reference point also has to be specified during assignment.

#### 2.2.1. Master Data
Before the new functionality can be put to use, assignments for the fittings have to be created in the master data. For this, use the dialog under Master data > Products > Articles > Fitting allocation:

*(Fig. 25 Fitting processing allocation shows the user interface for assigning processing steps (like drillings) to a selected fitting. It includes parameters for mounting type, priority, hinge side, and specific dimensions for the processing.)*

**UI Field Descriptions:**

1.  **Selected fitting:** The fitting to which processing is being allocated.
2.  Enter a **mounting type** here for the allocation. You can either select an existing one or enter a new one. It must be ensured that, if possible, the same mounting type is used to simplify subsequent exchangeability.
3.  With the **priority**, the sequence in which the allocations are selected is determined. If the fitting is entered in the BOM, the next unused allocation is always entered. **Priorities must start with the number 1 and be consecutive!**
4.  With the **hinge side**, it is determined whether the allocation is to be used for a left-sided or right-sided door. The setting "Both" is only used for searching.
5.  Here it can be stipulated whether the fittings should be **changed** when changing the hinge side. This is e.g. important for locks, as a left lock and a right lock are usually two different articles.
6.  The **list of processings** that are to be added with the fittings into the BOM is shown here. We recommend using macros to keep the number of processings as low as possible. The Insert and Delete functions can be used to add or remove processings. The sequence can be changed with the two center buttons.
7.  Here you can define **parameters** for the fitting currently selected in the processing list. These values overwrite the values from the master data if the processing is to be added to the BOM together with the fitting. The dimension fields support size formulas. We recommend the use of size formulas.

It must be ensured that a left-sided and right-sided definition are always created, as otherwise the exchange of hinge side would not work properly in document entry.

#### 2.2.2. Processing text
The new placeholder `<18>` is available for all processings. This placeholder is replaced with the mounting type when a processing is to be inserted in the BOM with a fitting. If the processing has been inserted without a fitting, the parameter is deleted when replacing. The parameter can therefore be added to all processing without any risk (if desired).

#### 2.2.3. Entry
To enter a fitting, simply enter the product number in the product field in processing entry. The fitting is then entered in the BOM with its processings and the entry mask switches to fitting mode.

*(Fig. 26 Fitting entry shows the fitting entry mode in the order entry screen. It details the current mounting type, version, hinge side, and a list of fittings and their associated processings in the BOM.)*

**UI Field Descriptions:**

1.  **Current mounting type.** The mounting type can be changed by pressing F4. The list only shows the mounting types that do not yet exist in the BOM for this fitting. If a different mounting type is selected, the processings in the BOM are exchanged with the new assignment.
2.  **Current version.** Here you can select the fitting variant by pressing F4. The default variant is always selected during entry.
3.  **Current hinge side.** Here you can define for which direction the fittings are to be mounted. This setting applies for all fittings, and all allocations are exchanged in the event of one change. If exchange articles are defined, they are also exchanged.
4.  With **"share variant"** you can exchange the variants of all fittings. As long as the fittings have the same variant, it is shown here. When opening the list, all variants are visible that apply to all fittings.
5.  The **BOM** shows the fittings and the corresponding processings. The processings are always added below the fitting in order to obtain a better overview.

Now further fittings can be added by pressing the New button. The allocations are entered based on their priority in ascending order. If no further allocations exist, the fitting is inserted in the BOM, but no processings. This can be determined in fitting entry by the fact that there is no area available in the list for a fitting. Existing fittings can also be exchanged with other fittings. To do so, the fitting has to be selected and a new product number has to be entered. If multiple mounting types are set up for a fitting, they can also be changed in fitting entry.

#### 2.2.4. Inserting and exchanging
A fitting can either be exchanged by entering a new article number or via product search. If the product search is opened for an article, the option "Only articles with allocation" can be used to select all fittings that comply with the current hinge side and that have the same mounting type as the current fitting. The mounting type can also be set to "All" if the fitting and the mounting type are to be exchanged all at once.

*(Fig. 27 Product search for fittings shows the product search dialog, filtered by "Only articles with allocation" for a specific mounting type.)*

#### 2.2.5. Finished products
The entry of fittings with the processing can also be used in product management to create respective templates. They can be used in order entry (including exchange). Here it must be observed that the size formulas are calculated in product management. However the calculated values are replaced in document entry by the size formulas from the allocation.

### 2.3. Checking spacers with LeCheck

#### 2.3.1. Preconditions
1.  To enable the spacer check, first enable rule number 5087 in the spacer restrictions dialog.
2.  The rule should only be enabled for product class TPS.
3.  If the item cannot be produced with TPS spacers, the alternative spacer is suggested.

*(Fig. 28: LeCheck - Precondition shows the 'Abstandhalterrestriktionen' (Spacer Restrictions) dialog, highlighting rule 5087 for enabling the LeCheck check for TPS spacers.)*

Since LeCheck also checks the sealing depth, either the item cutback or the cutback per edge must be entered for the order.

*(Fig. 29: LeCheck - Back cut shows the order entry screen where the 'Rückschnitt' (Back cut) value is entered.)*

*(Fig. 30: LeCheck - Sealing depth shows the detailed view for entering the sealing depth per edge.)*

For LeCheck, this value is reduced by the spacer width defined in product management. The resulting sealing depth is transferred to LeCheck.

*(Fig. 31: LeCheck - Product management shows the product management screen for a TPS spacer, where properties like thickness/spacer width are defined.)*

Since even quotations shall be checked, the processing parameters (e.g. radius of rounded corners) must be filled in for the processing steps to be checked (e.g. rounded corners) in the quotation.

LeCheck must be properly installed by a member of the ALCIM team first. The LeCheck.ini to be used must include the details of the TPS line.

#### 2.3.2. Type
If an item with a TPS spacer is entered (quotation, order, complaint), the LeCheck check is made under the following conditions when the item is saved:
1.  The item will be produced.
2.  The item includes a TPS spacer.
3.  One of the following conditions applies:
    a. The item includes a shape that is not 0
    b. The item includes steps
    c. The item includes one of the following processing steps: Cut-out corner, rounded corners, cut-off corner, internal cut-out, ticket window, notch, arch-shaped notch, SN Macro

**Process:**
1.  The check creates a file in the user directory (`%APPDATA%\A+W\Techsoft\ProcessAWISO.dat`). The format is described in document `\\JUPITER\DOKU_DocuWare\XOPT_XOPTS\Tools\AWISO.doc`. If the item includes at least one of the above processing steps, a SN file is created as well.
2.  After that, the program `%ALLUSERSPROFILE%\A+W\Techsoft\ProcessAWISO\ProcessAWISO.bat` is loaded. An error report will be issued if this program does not exist. The path containing the output file (`%APPDATA%\A+W\Techsoft\ProcessAWISO.dat`) is transferred as an argument to the program.
3.  After running the program, the value in fifth position (separated by semicolon) is checked in the LECHECK.OUT report file. If this shows 1, the check was successful. If this digit is 0, the item cannot be produced by the TPS line. Since the program cannot handle multiple users, the call may have to be repeated three times, in intervals of three seconds. If the check is still impossible after three attempts, the user is informed of the error.
4.  If the check is successful, the item can be saved. Otherwise, the program suggests the alternative spacer. If the user rejects this, the item will not be saved. The item must be changed in that case, and the check repeated if required.

**Possible errors:**
1.  Program `%ALLUSERSPROFILE%\A+W\Techsoft\ProcessAWISO\ProcessAWISO.bat` does not exist.
2.  The sealing depth cannot be determined (see requirements).
3.  No output file can be created.
4.  The file containing the LeCheck test result does not exist.
5.  Internal LeCheck error.
6.  The check cannot be made even at the third attempt.

The files used for the check are saved in zipped archives in directory `%ALLUSERSPROFILE%\A+W\Techsoft\ProcessAWISO\SAVE`. Zipped archives will be deleted after sixty days.

### 2.4. Invoice management / Project management

#### 2.4.1. The four different modes
Version 3.3.359 offers four different modes of invoice management. These are activated by the key file in ALFAK2000. Please make sure that only one of the modes is active, or one of the following combinations: 1+2 or 1+3 or 4+2 or 4+3.

Modes 1+4 and 2+3 must not be active simultaneously.
1.  Standard mode (module 122060 item 8)
2.  Invoice management (module 122800 item 80) (only DMS, Australia)
3.  Invoice management with allocated orders (module 122062 item 120) (SGG)
4.  Extended project management (module 122064 Pos 121) (made for the Spanish market)

#### 2.4.2. Standard mode
This is the original project management used by ALFAK2000 so far. We therefore refrain from detailed explanations.

#### 2.4.3. Invoice management
Invoice management is a version that was specially created for DMS; it has been part of ALFAK2000 since version 3.0.

#### 2.4.4. Invoice management with allocated orders
This mode allows to allocate an overall order to a project. In this overall order, only products will be used for the individual items, without detailed information on the product structure. Based on this overall order, claims will be specified, defining the percentage, quantity, or amount presently required. These claims will be transferred to financial accounting by a special mode. No invoices will be created. When the overall order has been completely fulfilled, and the project is finished, the overall order will be invoiced.

The user creates work orders and allocates these to the project. Purchase orders created for these work orders will also be allocated to the project. These purchase orders can be created manually, or via automatic transfer to purchasing. Both types of purchase orders can be listed separately. No invoices will be issued for work orders.

*(Fig. 32: Invoice management with allocated orders shows a flowchart of the process. A master order (Rahmenauftrag) generates claim orders (Forderungs Aufträge), which in turn create production orders and purchase orders. These are managed within a project (Objektverwaltung).)*

First, enter the overall order with the document type „Overall order" at order entry. Now, define the project in invoice management, and allocate the overall order.

*(Fig. 33: Creating a project in invoice management shows the UI for defining a new project and linking it to a master order.)*

The second tab of invoice management shows the items of the overall order. It also shows how many items have been claimed so far. Click the right mouse key on the table to view a history of the claims for this overall order.

To define a claim, select function „Issue request invoice". The dialog shows all items of the overall order, plus the claimed totals. You can enter a claim for a certain percentage of an item, or the claimed quantity. Alternatively, you can enter the amount. Once you have chosen one of the three options, this cannot be changed for the following claims for this item.

Printing of forms now offers some new variables for the document types „Claim“ and „Overall order" which are briefly described below.

- **CONTR_CLAIM_TYPE**: Claim type (percentage, quantity, or amount)
- **CONTR_CLAIMED_ACT**: Quantity for the actual claim
- **CONTR_CLAIMED_PREV**: Quantity of previous claims
- **CONTR_AMNT_ACT**: Amount of the actual claim
- **CONTR_AMNT_PREV**: Amount of previous claims
- **CONTR_PAID_AMNT**: Total claims paid
- **CONTR_CURRENT_AMNT**: Amount to be paid at present
- **CONTR_MWST_AMNT**: VAT for the present claim
- **CONTR_BRUTTO_AMNT**: Gross amount of the present claim
- **CONTR_FI_NETTO_GES**: Net amount of the corresponding overall order
- **CONTRACT_ORDER_ID**: Number of the corresponding overall order

Please make sure to use the product description from the overall order when you print the claim! The forms are based on the reports claim.qrp for claims, and contract.qrp for the overall order.

Tab Allocated orders shows the allocated orders and credit notes and the items involved. Credit notes are shown in red.

Tab Allocated P.O.s shows the purchase orders. Checkbox „Order-related P.O.s" allows to switch between P.O.s automatically created via transfer to purchasing, and manually entered P.O.s.

#### 2.4.5. Extended Project Management
The general conditions for a project are defined per product or product group. First, enter a customer project and define a sales representative and payment terms. At order entry, this information is imported into the order when the project is allocated to the order. Tab Allocated orders shows the orders allocated to the project.

*(Fig. 34: Project totals shows the 'Summen' (Totals) tab in the project management screen, displaying accumulated quantities, area, and revenue for products and product groups against their planned values.)*

Tab Totals shows the accumulated amounts for the project. In connection with the data on tab Scheduled quantities, this list shows how far the limits for every product and product group have been reached. When the limit of a product or product group has been reached or even exceeded, the appropriate entries will appear at the top of the list, in red.

The information shown on these two tabs can be printed. This information is printed for all projects selected in the dialog in QBE mode.

The project totals will be updated automatically during order entry.

Once a project has been tagged as completed, no further orders can be entered.

When you leave item entry, tab Totals in project management gives an overview of the project progress.

### 2.5. Product Exchange Groups

#### 2.5.1. General information
This function can prevent any glass, spacers or film from being installed in insulating glass and laminated glass that are not designed for or are not suitable for these products.

#### 2.5.2. Set-up
To enable the new functionality, the "Apply Product Exchange Rules For BOM Exchange" option must be activated in the company master data on tab 5:

*(Fig. in text shows the company master data settings, highlighting the activation of "Apply Product Exchange Rules For BOM Exchange".)*

Next, exchange groups can be defined:

*(Fig. in text shows the 'Exchange Groups' dialog where groups like 'Heat insulation', 'Sound insulation', 'Safety glass', etc., are defined.)*

Glass, spacers and films will now be added to the exchange groups:

*(Fig. in text shows the 'Exchange Allocation' dialog, where specific products (e.g., '1204 Wärmeschutz 4 mm Gold') are assigned to the previously defined exchange groups (e.g., 'Heat insulation').)*

Now, glass, spacer and film exchange groups can be defined for insulating glass and laminated glass in the product's BOM:

*(Fig. in text shows the product's BOM definition screen, where an exchange group ('Heat insulation') is assigned to a specific BOM item.)*

This definition then stipulates that in item input and in the alternatives the first BOM item can only be replaced by products in the "Heat insulation" exchange group. Consequently, based on the data created above, only 1204, 1205 or 1206 products could replace the first glass in the BOM. Entering a product that is not in the defined group will be rejected with an error message. Furthermore, only products that have the defined exchange group can be searched for in the product.

#### 2.5.3. Application
The exchange group is checked before a replacement is made if that product is detected in the item input and an attempt has then been made to replace an element. If no exchange group was specified for the BOM item or the new BOM element from the matching exchange group is associated with the BOM element, then the element can be replaced. If this is not the case, then the user will receive an error message indicating this and the exchange will not be performed:

> **Error [5618]**
> The product 1005 can't be inserted because its not part of the exchange group Heat insulation.

*(Fig. in text shows the error message appearing in the order entry screen when a user tries to substitute a BOM item with a product not belonging to the assigned exchange group.)*

If the search dialog is opened for an item in the exchange group, then only those products in this exchange group will be indicated. The exchange group can also be used as search criteria for items that are not associated with an exchange group:

*(Fig. 35 Selection shows the product search dialog being filtered by the 'Heat insulation' exchange group.)*

### 2.6. Generation of partial deliveries

#### 2.6.1. Per ready report / goods receipt

**Master Data**

At the beginning, a new status *Ready for delivery note printing* (status should be less than delivery note printing) should be defined in the status management. Then, the new status point *855 – Ready for delivery note printing* (arrived in the database via script) of the newly-created status *Ready for delivery note printing* must be assigned in the status assignment as User status. The status point *102 - Delivery note printing* thus requires the status *Ready for delivery note printing* as Minimum status.

So that the module can determine whether an order is already produced and ready, in the company data management on tab 7.Stock / PCH / EDI, the registration point starting at which an order is ready for dispatch/finished, is allocated. Furthermore, it is possible to define here whether a goods receipt of purchased parts (purchase orders) also travels via a registration point or whether the purchased parts must be checked in purchasing (booking of goods receipt).

*(Fig. 36 Company data - Allocation of the registration points shows the company master data settings for allocating registration points for production and goods receipt.)*

**Documents**

The screen table Documents contains all documents of the current number manager. Orders/purchase orders that have been reported completely ready or whose goods receipt is not complete are depicted in green and the Ready % column contains a value of 100%.

*(Fig. 37 - Document produced shows a list of documents, with a fully produced order highlighted in green.)*

Orders/purchase orders that have not been reported completely ready or whose goods receipt is not complete are depicted in red and the Ready % column contains a value less than 100%.

*(Fig. 38 - Document not produced shows a list of documents, with an incompletely produced order highlighted in red.)*

If a document is selected in the screen table, then all items are displayed in the detail table. In the detail table, the original item quantity, the partially-delivered quantity, the quantity reported produced, and the partial delivery quantity (quantity reported ready - partially-delivered quantity) are displayed.

These can be edited item by item, that is, with this quantity, the user can define how much of the quantity reported ready should be delivered partially.

*(Fig. 39 Document is ready for partial delivery shows the detail view where the user can edit the quantity for partial delivery.)*

The user also sees directly via the table column *Ready for part. del. %* how much of the order/purchase order can be partially delivered.

If, for example, due to technical problems there is no report from production (fileless reporting must be active) and the order must be delivered, in the table the order (< 100%) can be set to delivery (table column *Complete*) to be set and the document status is thus adjusted accordingly.

*(Fig. 40 - Document report complete shows a confirmation dialog asking if the user wants to report the whole order as completed.)*

Before the partial deliveries are created, a target number manager should be defined. If the program creates the partial delivery, it includes all item quantities ready, whereas the uncompleted ones remain in the original order. However this depends on whether or not the option *Do not delete partial delivery item* in the company data is active.

Furthermore, the user can override the AV area from the original order for the partial delivery if desired. The partial delivery gets a new status *Ready for delivery note printing*. The delivery note printing must have the new status as minimum status (see 0).

If the partial delivery has been created, the user is asked whether the delivery note should be printed.

*(Fig. 41 Delivery note printing starts automatically shows a dialog asking the user if they want to print the partial delivery note.)*

However, it is also possible to call up the print program manually.

*(Fig. 42 Start delivery note printing manually shows the general form printing menu where partial delivery printing can be initiated.)*

#### 2.6.2. Per rack
As an additional functionality, the generation of partial deliveries per rack was implemented in the module. On the new tab *Per rack*, the user has the opportunity to display the rack-order assignments by Number manager. In contrast to this, you can also filter your selection by Customer. Additional selection possibilities are a limitation by Deliv. Date and Status.

*(Fig. 43 Rack order assignments shows the UI for viewing orders assigned to specific racks, with details on delivery date, status, and completion percentage.)*

The rack orders are loaded on the upper screen table. Here, the user has information about which orders are on which rack. Both the delivery date and status of the order as well as the percentage values, how much of the rack order is ready and how much of the order was already delivered are displayed in the table.

If you click an assignment, all order items that are stored on the rack are loaded into the lower screen table. In the table, the item status, the product with its dimensions, and the quantities are displayed. The original item quantity (original), the quantity on the rack, and the already partially-delivered quantity are displayed.

In order to generate a partial delivery now, the rack must be marked with a double-click on the row header, that is, the complete rack is always partially delivered. However, not all orders per rack are combined into a partial delivery (one order = one partial delivery).

*(Fig. 44 Marking the rack-order assignments for partial delivery shows a rack being selected (marked with an X) to generate a partial delivery.)*

The user has, before he generates the partial delivery, the opportunity to override the order header fields *Deliv. Date, Route, Truck, and Driver*. For this, you must activate the appropriate option, at which point the data field (the selection box) can be edited. A target number manager should also be selected. At the start of the program, the same number manager is set as in the selection criteria.

*(Fig. 45 Overwriting header fields shows the UI elements for overriding delivery date, lorry, route, and driver for the partial delivery.)*

If the partial delivery has been created, the user is asked whether the delivery note should be printed. If this should happen at a later point in time, you can also call the print program via the menu function.

### 2.7. Delivery date calculation
It is now possible to calculate the earliest possible delivery date for an order or quotation using the capacity planning. Here it must be heeded that the delivery date calculated is only a snapshot since the capacities calculated are not reserved. Therefore, the delivery date can still shift if other orders are then scheduled and thus take up capacities that were necessary for the previous delivery date calculation.

The delivery date calculation can be executed from the order or quotation entry by clicking the button next to Delivery. For this, the document must be saved.

*(Fig. 46 Delivery date calculation shows the order header with a button next to the delivery date field to trigger the calculation.)*

#### 2.7.1. A+W Capacity
The delivery date calculation with A+W Capacity is done asynchronously by the AWSOA Planning Service. This schedules a transferred document in the capacity planning and returns the delivery date calculated.

The connection is made via the AWSOA.Commercial.Export.ComProxy, which awaits the response of the service so that the user can keep working with the program, because delivery date calculation for orders with a lot of items can take quite a while. If you click the button, a dockable window opens, which displays the progress of the ongoing date calculation(s). After one or several calculations have been completed, the user can take over the date calculated into the order. Furthermore, in case of error, the messages from the service are displayed there.

In order to use the functionality, the AWSOA infrastructure services must be installed and configured. Furthermore, the license 149 must be enabled and the OrderXML version must be at least 5.3; otherwise the button is hidden. The OrderXML can be set on a subdialog of the company master data on tab 13.Production.

The import in the planning service uses the settings for the OrderXML import. Therefore, the MZO must be set up in advance in the production system.

*(Fig. 47 OrderXML Version shows the settings dialog for 'Transfer to Production', highlighting the OrderXML version setting, which must be 5.3 or higher.)*

**Participating components:**

*A flowchart shows the data flow: `A+W Business` sends an `OrderXML` via `AWSOA.Commercial.Export.ComProxy.exe` to the `AWSOA.Planning.Import Service`. The service then returns the `Delivery date or error message`.*

The tracing is set up in the A+W Protocolling Config Tool:

*(Fig. in text shows the A+W Protocolling Config tool, where trace levels for various 'Commercial Export COM' components can be set.)*

The Commercial Export COM service is responsible for setting the tracing for all components. The associated file has the name `Commercial.ExportComProxy_<DATE>.awtrc`. The OrderXML generated can also be viewed in the file.

The import in the A+W Planning Import Service can be traced in the following trace settings:

*(Fig. in text shows the A+W Protocolling Config tool, where trace levels for various 'Planning Import Service' components can be set.)*

The tracing for all components for the Planning Import Service can be set here. The associated files have the following name: `Planning.ImportService._<DATE>.awtrc` and `Planning.ImportService.NET_<DATE>.awtrc`. The import messages from the production system can be viewed in the file.

#### 2.7.2. A+W Business Capacity Planner
Delivery date calculation is also possible with A+W Business Capacity Planner. Here a document is scheduled and if the current delivery date cannot be adhered to, there is an attempt to find the next day until a suitable date has been found.

A particularity here is that orders are actually scheduled and thus capacities are assigned; however this does not apply for quotations. The delivery date calculated and the time costs are written back to the document in question.

Prerequisite for this functionality is a set-up A+W Business Capacity Planning.

*(Fig. 48 Delivery date calculation 2 shows a progress dialog 'Scheduling the order' that appears when using the A+W Business Capacity Planner.)*

The scheduling is done in A+W Business. The tracing can be done in the trace file of the running A+W Business.

### 2.8. TPS/LSG invoices
Documents > Order > TPS invoice

*(Fig. in text shows the A+W Business main screen with the 'TPS Faktura' (TPS Invoice) menu item.)*

#### TPS invoice
The TPS/LSG invoice serves the internal charging of services between 2 sites and was implemented exclusively for Fandel.

An order with TPS will be produced by Europane since a TPS line only exists there. For this order, an incoming invoice is generated, which includes the entire item, plus a surcharge for the assembly of the IGU. The price calculation is done using the conditions for the supplier Europane.

At the same time, an outgoing invoice is generated for Europane for the glass and the cutting of the basis glass. Some of the glass is cut by Fandel. Products ordered are always invoiced since the order was placed by Fandel.

If the machine is placed in production areas 8 and 10, this is the criterion that carries out the charging.

#### LSG invoices
Cut glass that is not in a TPS IGU must be invoiced from site 2 to Fandel. For this, as 3rd charging, outgoing invoices for LSG are generated. The price is to be taken for the conditions for Fandel and also its energy surcharges. Processings on simple glass that are made on the Europane units must also be taken over.

The Europane units are:
- 901 - PCH LSG cutting 1
- 902 – PCH LSG cutting 2
- 905 - PCH LSG manual cutting
- 907 - PCH KBF 1

#### Status Points
- **770 - TPS invoice created**: The incoming invoice for the TPS IGU was created.
- **790 - TPS invoices invoice**: The outgoing invoice for the basis glass cutting was created.
- **795 - LSG charging**: The outgoing invoice for LSG was created.
- **796 - LSG invoice checked**: Order does not include any LSG charging.
- **800 - TPS invoice checked**: Order does not include any TPS charging.

### 2.9. User-defined text fields in the document header
In the document header on the 3.Addition tab, there are three user-defined text fields available:

*(Fig. in text shows the 'Addition' tab in the document header, highlighting three user-definable text fields: 'Default-Test', 'New customer', and 'Last Contact'.)*

The leading text of the fields can be defined with the system texts 2000, 2001 and 2002. By default after the database update, the designations are `Textfield 1`, `Textfield 2` and `Textfield 3`.

The new fields can be used on the forms in document printing and document display (USER_FIELD1, USER_FIELD2 and USER_FIELD3).

### 2.10. Status management per user(-group)
Under Master Data > Company a new management dialog *Status management per employee (group)* was implemented.

*(Fig. 49 - Status Administration per employee (group) shows the dialog for managing status access rights, where status areas can be defined and assigned to employee groups and document types.)*

Effective immediately, you can now define four status areas per employee and/or employee group that can be assigned to one of the five document types Quotation, Order, Credit, Inquiry or Purchase order.

In order to select data, the user has the opportunity to filter by employee (group) and/or the document type.

*(Fig. 50 - Defining status areas shows the dialog with specific status ranges defined for an employee (Sebastian Weil) for the 'Order' document type.)*

If you would now like to make a manual status change, e.g. under Documents > Order > NM order > Functions > Status change, these status areas serve to check the current document status. Depending on whether or not the document status is in one of the four areas, a status change is possible or not permitted.

> **Message 5737**
> You don't have the necessary rights to change the status of document 990106. The current document status is not in your accessable status range!

*(Fig. 51 - Manual status change not permitted shows the error message displayed when a user without sufficient rights attempts to change a document's status.)*

### 2.11. Resubmission of orders
The resubmission of documents (e.g. Documents > Order > Resubmission) has been enhanced. Up to now, only quotations could be fixed for resubmission. Effective immediately, in the company master data (Master Data > Company > Company data) on tab 10.System, you can define the lead days for the resubmission of an order.

*(Fig. 52: Company data: lead days for resubmission of orders shows the company master data settings, highlighting the 'Lead days for resubmission' for an 'Order'.)*

Depending on the setting here, the presentation date will be calculated during entry of an order. For this, for orders there is now the new data field *Presentation* in the document entry (Documents > Order > Order).

*(Fig. 53: Order entry presentation date shows the 'Presentation' date field in the order entry screen, which is automatically calculated based on the lead days.)*

The date entered is compared to the current date when A+W Business starts up and there is a check of whether documents for resubmission exist. The user then has the choice whether or not the documents should be displayed. If so, the resubmission dialog opens.

*(Fig. 54: Resubmission of orders shows the resubmission dialog, listing orders that are due for follow-up.)*

The already familiar functionalities are available to the user here, e.g. the assignment of transfer to archive or the authorization to delete. The display of alternative orders under Functions > Alternatives and the printing of the data records present in the screen table has also been adjusted for orders.

*(Fig. 55: Resubmission of alternative orders shows the alternative orders overview for a selected resubmission item.)*

*(Fig. 56: Printing of orders shows a printed report of the orders due for resubmission.)*

### 2.12. Turning of shapes in the document entry
Starting with Version 13.4.80, it is possible to turn shapes in the document entry. So that the new feature is active, the following switch must be activated in the company master data:

*(Fig. in text shows the company master data settings, highlighting the 'Turn Shapes' option.)*

Then in the shape/[processing entry, the angles of rotation 90, 180 and 270 degrees are available. The turning can be applied for the shapes with shape numbers smaller than 137 except for 0, 24, 98, 99, 60, 61, and 81 (these shapes are symmetrical or free shapes):

*(Fig. in text shows the shape processing entry screen with a dropdown menu 'Turn by' allowing the user to rotate the shape by 90, 180, or 270 degrees.)*

**Sense of pattern**
The sense of pattern is not turned. That is, if glass is turned by 90°, the sense of structure does not change. It is assumed that the sense of structure refers to the turned shape.

**Effects**
- The printout is done with the turned form, that is, the customer sees the shape turned.
- For the production transfer, for directional glass and a turning of 90 or 270 degrees, the structure is turned since the turning is not known in the production system.
- The same applies for the export via the EDI interface.
- In the production manager, the turning is considered during optimization.
- The checking of the dimensions is also done with the turned dimensions for 90 or 270 degrees.

> **Caution:** ERP Webservice and production manager must be updated, since otherwise for directional glass the sheet will be cut incorrectly.
