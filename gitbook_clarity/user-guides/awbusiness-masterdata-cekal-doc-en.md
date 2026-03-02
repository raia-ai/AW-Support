---
description: "EN_AWBusiness_Master_Data_9_11-4"
---


# CEKAL

---
## Restrictions

> **Master Data > CEKAL > Restrictions**

*Fig. B-295 CEKAL restrictions*

This dialog serves to enter the restrictions for the CEKAL check.

These restrictions can be used to check technical values, e.g. the lite size or the grill thickness. There will be no CEKAL classification if these values are not met.

### Restriction values

**Number**
The numbers are defined by the system.

**Parameters 1-4**
Values for the individual restriction parameters. The number of changeable parameters depends on the selected restriction.

**Remark**
Shows the predefined text for the restriction.

### Text

**General**
This text will be printed on the forms and can be up to 80 characters.

**Label**
This text will be printed on the labels and has to be short enough.

**Production**
This text is printed on the production papers (in A+W Business or production software). It serves for internal purposes.

**Bender**
This text can be transferred to the spacer bender provided that the bender can import text. When a number has been entered in the Bender section in field Number, the text entered in field Bender will not be taken into account.

### Bender

**Number**
Text number to be transferred to the bender. The bender text shown above will not be taken into account when you enter a text number.

### Restrictions

This list shows all restrictions that can be used for the check.

## Product Texts

> **Master Data > CEKAL > Product Texts**

*Fig. B-296 CEKAL product text*

This dialog is used for entering CEKAL text for special products that refer to a certain structural level. If such a product is part of an IG unit, this CEKAL text has absolute priority over other CEKAL text.

### Product selection

**Product**
Product that has been allocated a special product text.

**Level**
Structural level to which the text applies.

**Remark**
Brief explanation of the text.

### Text

**General**
This text will be printed on the forms and can be up to 80 characters.

**Label**
This text will be printed on the labels and has to be short enough.

**Production**
This text is printed on the production papers (in A+W Business or production software). Used for internal purposes.

**Bender**
This text can be transferred to the spacer bender provided that the bender can import text. When a number has been entered in the Bender section in field Number, the text entered in field Bender will not be taken into account.

### Bender

**Number**
This text can be transferred to the spacer bender provided that the bender can import text. If you have entered a bender number in section Text, the bender text entered here will be ignored.

### Text allocation

This list shows the structure-related text allocations.

# CE Code

> **Master Data > CE code**

IG units that are marked with this certificate have to meet fixed quality criteria.
The CPIP code (Characteristic Performance Identification Paper) is only required in France. It provides details on the characteristics and the performance.

Menu CE code offers the following entries:
- "CPIP Code” on page B-1079
- "Size Restrictions" on page B-1080
- "IG Search Data" on page B-1081
- "Restrictions" on page B-1076
- "Settings" on page B-1082

## CPIP Code

> **Master Data > CE code > CPIP Code**

*Fig. B-297 CE code - CPIP code*

You can use this dialog for entering details regarding the CPIP code, e.g. its validity, whether it has been certified, and if it matches a CE standard.

The standards and rules for CPIP creation can be imported in dialog Settings.
(See "Settings" on page B-1082)

The CPIP code has to be entered for the corresponding products in product management.

## Size Restrictions

> **Master Data > CE code > Size Restrictions**

*Fig. B-298 CE code - size restrictions*

This dialog allows entering the size restrictions for CPIP codes.
At order entry, the program checks whether the current item exceeds CE-relevant size restrictions. A message will appear should a restriction be violated.

## IG Search Data

> **Master Data > CE code > IG Search Data**

*Fig. B-299 IG Search Data*

This dialog serves for managing the CPIP code data for IG. These data control the behaviour of order entry.

> **Entering a new record**
> When you enter a new record you have to define a default for grills.

Values that are not preset for the IG unit will be preset by default values in order to determine the CPIP code in search data.

### Table

This tab lists all search data defined in the system.

## Settings

> **Master Data > CE Code > Settings**

*Fig. B-300 Master Data > CE Code > Settings*

This dialog serves for importing the files with the necessary CPIP codes and other definitions. The interface files are separated by a ^ sign. The first line must show the column name.

Depending on the size of the file, import may take some time.

### Standard values for the IG search function

This is where the standard values for non-glass elements are kept.

### File update CPIP code

Some of the database tables in this section can be filled via interface files. Select a file and start the process by pressing the [Upload] button.

# B2B

> **Master Data > B2B**

This is where interface data for data transfer are entered.
Menu B2B offers the following entries:
- "Products (Customer, Supplier)" on page B-1083
- "Copying of External Products" on page B-1090
- "Spacer (Customer, Supplier)" on page B-1091
- "Gas (Customer, Supplier)" on page B-1092
- "Routes (Customer, Supplier)" on page B-1093
- "Customer, Supplier" on page B-1094
- "Document Export" on page B-1100
- "SN File Rules" on page B-1102
- "Product Import" on page B-1103
- "Price Import" on page B-1105

## Products (Customer, Supplier)

> **Master Data > B2B > Customer, Supplier > Product**

Orders can be imported by EDI, and purchase orders exported. The product data for this data transfer are kept separately for customers and suppliers. The dialogs structures are identical. In this document, they are described for customers.

This section provides information on the following subjects:
- "Functions Menu" on page B-1083
- "Products - Bill of Materials" on page B-1084
- "Products - Parameters" on page B-1086
- "Products - Table" on page B-1087
- "Products - Shapes/Processings" on page B-1088
- "Products - Grills" on page B-1089

### Functions Menu

> **Master Data > B2B > Customer, Supplier > Product > Functions menu**

This menu is used for exporting data. The following entries are displayed:

- **Define Dorma reference:**
  Enter references for Dorma products. With this function, the matchcode will always include the product's external Dorma number. This function is available for suppliers only.
- **Copy article:**
  Opens the dialog Copy external articles for copying the current customer's articles.
  (See "Copying of External Products" on page B-1090)

### Products – Bill of Materials

> **Master Data > B2B > Customer, Supplier > Product > Bill of materials tab**

*Fig. B-301 Products - Bill of Materials*

This tab is used for allocating your own glass products to the business partner's products.

#### External product

**Partner**
Business partner for whom the allocation is valid.

**Valid from**
Data from which the allocation is effective.

**Article number**
Alpha-numerical article number used by the business partner.

**Name**
Name used by the business partner.

**Width/Height**
Sizes valid for the business partner.

**Color**
Color variant valid for the business partner.

**Prices / PU**
Price: Price per price unit.

#### Identification

**Article/MCode**
Article (product) number acc. to A+W Business master data.

**Name**
Name as defined in master data.

#### BOM product

The fields in this section are accessible only if a BOM element has been selected.

**Article/MCode**
Article (product) number of the selected BOM element.

**Name**
Name of the selected BOM element.

**Qty. / Width / Height**
Details for boxes.

**Color**
Color variant of the selected BOM element.

**Pattern level**
Pattern level of the selected BOM element.

**Sense of pattern**
Sense of pattern of the selected BOM element.

**Coating side**
Coated side of the selected BOM element.

#### BOM

The list shows the bill of materials for the selected product. Select an element to view its details in section BOM.

### Products – Parameters

> **Master Data > B2B > Customer, Supplier > Product > Parameters tab**

*Fig. B-302 Products - Parameters*

This tab serves to specify whether the corresponding product number should be searched and entered automatically when the invoice is checked.

If you are using the electronic invoice check via openTRANS you can have the references entered automatically.

### Products – Table

> **Master Data > B2B > Customer, Supplier > Product > Table tab**

*Fig. B-303 Products - Table*

This tab lists all allocated products.

### Products – Shapes/Processings

> **Master Data > B2B > Customer, Supplier > Product > Shapes/Processings tab**

*Fig. B-304 Products - Shapes/Processings*

This tab serves to enter the parameters for shapes and processing steps. The fields are described in detail in connection with product master data in section Sales.
(See "Product Management - Shapes/Processing" on page B-611)

### Products – Grills

> **Master Data > B2B > Customer, Supplier > Product > Grill tab**

*Fig. B-305 Products - Grills*

This tab is used for entering the parameters for grills (patterns). The fields are described in detail in connection with product master data in section Sales.
(See "Product Management - Grills" on page B-625)

## Copying of External Products

> **Master Data > B2B > Customer, Supplier > Product > Functions menu > Copy articles**

*Fig. B-306 B2B - Copy external products*

This dialog can be used to copy one business partner's data and transfer them to another partner.

## Spacer (Customer, Supplier)

> **Master Data > B2B > Customer, Supplier > Spacer**

*Fig. B-307 B2B - Spacer*

This dialog is used for allocating your own spacer products to the business partner's products.
The spacer data of customers and suppliers are kept separately for data transfer purposes. The dialogs structures are identical.
The fields are described in detail in connection with dialog Products.
(See "Products – Bill of Materials" on page B-1084)

## Gas (Customer, Supplier)

> **Master Data > B2B > Customer, Supplier > Gas**

*Fig. B-308 B2B - Gas*

This dialog is used for allocating your own gas products to the business partner's products.
The gas data of customers and suppliers are kept separately for data transfer purposes. The dialogs structures are identical.
The fields are described in detail in connection with dialog Products.
(See "Products – Bill of Materials" on page B-1084)

## Routes (Customer, Supplier)

> **Master Data > B2B > Customer, Supplier > Routes**

*Fig. B-309 B2B - Routes*

This dialog serves to allocate your own routes to the business partner's routes.
The route data of customers and suppliers are kept separately for data transfer purposes. The dialogs structures are identical.
The fields are described in detail in connection with dialog Products.
(See "Products – Bill of Materials" on page B-1084)

## Customer, Supplier

> **Master Data > B2B > Customer, Supplier > Customer, Supplier**

The settings for customers and suppliers are maintained separately for EDI data transfer. The dialogs structures are identical. In this document, they are described for customers.

This section provides information on the following subjects:
- "Functions Menu" on page B-1083
- "Customer, Supplier - Selection" on page B-1094
- "Customer, Supplier - Parameters" on page B-1096
- "Customer, Supplier - Table" on page B-1099

### Functions Menu

> **Master Data > B2B > Customer, Supplier > Customer, Supplier > Functions menu**

This menu can be used for importing or exporting command scripts.

### Customer, Supplier - Selection

> **Master Data > B2B > Customer, Supplier > Customer, Supplier > Selection tab**

*Fig. B-310 B2B - Partner selection*

This tab serves to enter the settings for the EDI interface for every business partner.

#### Partners

**Number**
Number of the business partner with whom you want to exchange data by EDI.

**Subsidiary number**
Number of the market partner's subsidiary.

#### Different partner for article reference

**Number**
Number of the business partner to whose articles should be used as references if no special references have been defined for the current business partner.

#### Interface

**Type**
Interface version. If you also want to transfer order confirmations and invoices electronically (openTRANS-Format) you have to choose the version you have been using so far for transferring the data. The version is defined when A+W Business is installed.

#### Batch number of target file

**From, Current, To**
First and last number of the number range to be allocated for the batch numbers for transfer.

#### Path name

**Source path, Source file**
Directory and file name for the import/export file.

**One File per document**
This checkbox only appears for suppliers.
- All of a supplier's POs are written to one file.
- During export, one file per PO is generated.

**Protocol path, Log file, Backup path**
Directories and file names for the log and backup file.

#### Command script

This is where you can enter a script that can be used for modifying and copying EDI files.

### Customer, Supplier - Parameters

> **Master Data > B2B > Customer, Supplier > Customer, Supplier > Parameters tab**

*Fig. B-311 B2B - Interface parameters*

This tab serves to enter the parameters for the data transfer by EDI.
The fields in sections Partner to Batch number are described in connection with the Selection tab.
(See "Customer, Supplier - Selection" on page B-1094)

#### Parameters

**Compulsory referencing**
Usually, references for customer or supplier products are defined in full. You have to decide however what is going to happen should references be missing.
- [ ] The product number defined in master data is saved in the interface file. This is e.g. useful if the sending and the receiving system use the same product master data. You do not have to enter data in reference tables if this is the case.
- [ ] If an item without a reference is transferred to an (external) product, this item can be ignored. An error report will be made in the logbook in this case.

**Locking active and maximum lock time**
It may put quite some stress on your system if several users are using the transferred data.
- [ ] The interface file will not be locked. This setting is useful if just one program accesses the file.
- [ ] Just one program can access an interface file at a time for the defined period. The field for entering the time is released.

**Definition of document number permitted**
The document number can be imported or assigned by A+W Business.
- [ ] The document number can be imported or assigned by A+W Business.
- [ ] The document number can be imported from the EDI file if no number has been assigned yet. An error message appears if a number has been assigned already.

**Adopt whole BOM from interface file**
The BOM can be created from the interface file or from product master data.
- [ ] The BOM is adopted from product master data.
- [X] The interface is selected from the structure shown in the EDI reference.

**Unit of measurement**
Choose an option to specify how sizes should be interpreted in the interface file. The settings for the measurements are generally made in company data. This default setting can be changed per customer in master data and in the documents. You have to define which unit of measurement should be used for the import.

**Size precision = 1/**
If imperial measurements are enabled for the interface file, enter 32, 64 or 128, depending on the factor to be used for calculation. If you are using metric sizes, enter 1 in field Size accuracy.

**Do not create order in case of an error**
The interface file may contain errors to which the system must react.
- [ ] The data from the interface file will always be turned into an order.
- [ ] No order will be created if there are errors in the interface file. An appropriate message will be displayed at the import. You can use the log to search for the error and correct it. After that, the data can be imported again.

**Restriction exceeded - item rejected**
The interface file may include items violating the restrictions in A+W Business.
- [ ] Items violating the restrictions will be adopted as they are. The orders have to be edited by hand afterwards.
- [ ] Items violating the restrictions will not be imported. You can use the log to search for the error and correct it.

**Exchange if restriction is not met**
If the interface file contains items violating the restrictions in A+W Business, alternative products can be used automatically.
- [ ] Items violating the restrictions will be adopted as they are. The orders have to be edited by hand afterwards.
- [X] If there are items violating the restrictions, the alternative products defined in A+W Business will be used automatically.

**Permit complaints**
Complaints can be imported through the interface. Complaints are usually not permitted but imported as "common" orders. After that, the system checks if the order is a complaint.
- [ ] Complaints are not permitted.
- [ ] Complaints are permitted.

**Change basic product if 2 elements are exchanged**
If more than two elements of an item are exchanged, another A+W Business product can be used automatically.
- [ ] The items are adopted as they are.
- [ ] If two elements of an item are exchanged, the system will automatically use the basic product specified in product management.
  (See "Basic product" on page B-603)

**Delete inferior edge processing**
Specification of whether for edge processings all processings should be executed if they differ only in the quality, e.g. seaming and polishing on the TG.
- [ ] All edge processings are executed as they are entered.
- [X] Only the superior edge processing is executed. The inferior edge processing is ignored.
If an edge processing should therefore affect no edge, then the whole processing is deleted from the BOM.
See also the setting in the company data.
(See "Company Data - Parameters" on page B-934)

**Check processing parameters**
During EDI import, the processing parameters in the processing record can be checked.
- [ ] Processing parameters are not checked.
- [ ] Processing parameters are not checked. If parameters are not set or values are not permitted, they are corrected automatically.
For edge processings, for example, the number of marked edges are checked; that is, if there is no shape, logically a maximum of 4 edges can be processed.

**Import of market partner-specific texts**
Specification whether individual texts of the market partner should be imported.
- [ ] These texts are not imported.
- [ ] These texts are imported.

#### Prices

**Permit price import**
Defines whether or not prices should be imported or exported.

**Deactivate calculation of surcharges/discounts**
Specification whether surcharges and discounts should be calculated.
- [ ] Surcharges and discounts are calculated. Thus, the price defined in the EDI file is taken over unchanged into the document.
- [X] Surcharges and discounts are not calculated.

### Customer, Supplier - Table

> **Master Data > B2B > Customer, Supplier > Customer, Supplier > Table tab**

*Fig. B-312 B2B - table for customers, suppliers*

This tab lists all defined customers or suppliers. The interface file path is shown for those business partners for whom data transfer for EDI has been set up.

## Document Export

> **Master Data > B2B > Customer > Document export**

*Fig. B-313 Settings for openTrans export*

This dialog serves to make the settings for export in openTrans format per customer. This format can be used for transferring order confirmations, delivery notifications, and invoices.
The openTRANS files have the suffix `*.awotdis`, `*.awotres` oder `*.awotinv`.

### Customer

**Number**
Number of the business partner who should get the documents in openTrans format.

### Interface

**Type**
Interface version. If you also want to transfer order confirmations and invoices electronically (openTRANS-Format) you have to choose the version you have been using so far for transferring the data. The version is defined when A+W Business is installed.
