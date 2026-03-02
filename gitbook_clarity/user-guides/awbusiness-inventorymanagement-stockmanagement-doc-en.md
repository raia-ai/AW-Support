---
description: "EN_AWBusiness_Inventory_Management_6_1-1"
---


# A+W Inventory Management: A+W Business

**A+W - Software for Glass, Windows and Doors**

---
## Introduction

This part of the documentation contains editorial notes.

### Revision Overview

| Section Version/Date | Description                                                                                             |
| :------------------- | :------------------------------------------------------------------------------------------------------ |
| 6.1/04-2020          | New: Stock management > Critical stock on hand                                                          |
| 6.0/10-2019          | Box management settings transferred to separate part and deleted from Inventory Management part.        |
| 5.2/08-2019          | New settings for inventory lists and printing of box labels.                                            |
| 5.10/01-2017         | Revision of Inventory, new dialog Stock assessment.                                                     |
| 5.00/08-2013         | Complete revision of ALFAK documentation and adjustment to A+W Business.                                |
| 4.12/01-2013         | Layout adapted to CI 2013.                                                                              |
| 4.11/02-2012         | Corrections                                                                                             |
| 4.10/11-2010         | Update and conversion to documentation concept 2010                                                     |
| 4.00/08-2009         | Complete revision                                                                                       |
| 3.02/09-2008         | Illustrations and section number amended.                                                               |
| 3.01/08-2008         | Correction of spelling errors                                                                           |
| 3.00/12-2003         | Structural conversion to program structure 4.0                                                          |
| 2.00/08-2000         | Revision Stock                                                                                          |
| 1.00/03-1998         | Original version                                                                                        |

### Editorial

The editorial provides information on the following topics:
- Notes on this document
- Copyrights
- Trademarks
- Contact

### Notes on this document

This document is intended for end users of *A+W Business*.

The documentation and software described are licenses that must only be used or copied in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of *A+W Business*.

### Copyrights

© 2020, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation.

The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademarks

All hardware and software names mentioned in this documentation can also be registered trademarks or other property rights of third parties. Third party copyrights must be observed.

### Contact

**A+W Software GmbH**

Am Pfahlgraben 4-10
D-35415 Pohlheim

📞 +49 6404 2051 0
📠 +49 6404 2051 877
📧 aw.zentrale@a-w.com
🌐 http://www.a-w.com

## Contents
*This section provides an overview of the document's structure. The full table of contents is omitted for brevity, but the document follows this outlined structure.*

- **Introduction** (G-3)
- **Tutorial** (G-7)
  - Overview (G-9)
  - Basic Principles of Stock (G-14)
  - Master Data (G-17)
  - Stock control on BOM level (G-58)
  - Stock Management (G-64)
  - Stock Booking (G-75)
  - Queries (G-85)
  - Stock information (G-94)
  - Stock P.O. (automatic) (G-103)
  - Stock Articles in Documents (G-113)
  - Manual Stock P.O. (G-122)
  - Production Orders (G-126)
  - Inventory (G-136)
- **Section Index** (G-159)
- **Index** (G-161)

## Tutorial

### Overview

The tutorial for the *Stock Management* module deals with the stock management basics in *A+W Business*. The tutorial is based on the knowledge of master data, purchasing, and sales.

> **i The functions depend on the enabled modules**
> Please note that the individual functions are only available if the corresponding modules and interfaces have been installed and enabled.
>
> If you detect functions in this description that are not available in your version, please contact A+W Software GmbH.

#### Subjects
This tutorial includes the following subjects:
- Basic Principles of Stock
- Master Data
- Stock Management
- Stock Articles in Documents
- Inventory

#### Required knowledge
This tutorial is meant for those who manage stock in *A+W Business*. Participants must be familiar with the concept of master data, sales, and purchasing in *A+W Business*.

> **i Box management in stock**
> The settings for box management are described in the separate part *Box management*.

### Documentation

The following documents are available for the Stock Management module:

| Format           | Volume                                                                    |
| :--------------- | :------------------------------------------------------------------------ |
| **Handout**      | Printout of tutorial for training session                                 |
| **PDF**          | Complete documentation: Tutorial, Software reference, Index               |
| **Online help <F1>** | Context-sensitive dialog help of *A+W Business* software reference and tutorials. |

### Tutorial structure

The tutorial consists of subjects with several training modules each. Each training module consists of the following elements:

- **Overview**
  Each training module starts with an overview of the major topics:
  - Objectives: What shall be conveyed?
  - Benefit: What can this knowledge be used for?
  - Maxims: Which correlations are to be remembered?
- **Concepts**
  First, the concepts and terms of the corresponding training module will be explained. This is followed by examples and instructions.
- **Exercises**
  For some of the training modules, exercises with certain tasks and suggested solutions are available.
- **Cross-references**
  At the end of each training module there is a section with cross references pointing out additional information in the software reference and in other sections. This will help you to extend your newly acquired knowledge.

#### Reading instructions
The contents of a training module are based on the knowledge conveyed in the previous module. We therefore recommend not to skip any training modules.
If you are already familiar with a subject you should at least read the summary at the start of a training module in order to bring the main details to mind.

### Display conventions

Certain parts of sentences are specially marked. The meanings are:

| Convention | Description                                                                                                        |
| :--------- | :----------------------------------------------------------------------------------------------------------------- |
| *Italic*   | marks character strings describing the software elements, e. g. the *Stock info* dialog.                           |
| **Bold**   | marks character strings to be entered via the keyboard, e.g.: Enter the value **0**.                               |
| >          | The so-called breadcrumb trail marks shows how to open a dialog, e. g. *Stock management > Inventory > Final inventory* |
| []         | Square brackets mark buttons in a dialog, e. g. [OK] to save the data.                                            |
| < >        | Angle brackets refer to keys or shortcuts on the keyboard, e. g. <F1> is used to open the online help.             |

### Menu Overview

This chapter provides a brief overview of the program sections that will be addressed in the subjects of this training.

*Fig. G-1 Stock Management menu*
*(Image shows the main Stock Management interface in A+W Business, with sections for articles, prices, supplements, stock levels, storage places, and inventory details.)*

#### Inventory
In this section, prepare the inventory, enter counted values and finalize the inventory.
(See "Stock Management menu" on page G-12, "Inventory” on page G-136)

#### Stock management
Use this dialog to enter and maintain data for stock articles.
(See "Stock Management" on page G-65)

#### Stock movement
Use this dialog to book goods received and issued, changes of stock locations and opening of boxes.
(See "Stock Booking" on page G-75)

#### Queries
In this section, view the stock history, analyses and reservations.
(See "Queries" on page G-85)

#### Search
Use this dialog to check the product availability during a certain time period.
(See "Stock information" on page G-94)

#### Stock P.O.
Use this dialog to transfer purchase orders for stock articles to purchasing.
(See "Transfer Stock P.O. to Purchasing" on page G-105)

#### Additional information
- Overview, "Elements of the Program Window" on page A-51
- Sales, "Document management dialog" on page C-39

## Basic Principles of Stock

*A+W Business's Stock Management* module allows you to manage jumbo sizes, stock sizes, residual plates, boxes, all-glass doors, fittings, frame parts and accessories, such as mirror mountings, sealing tape, etc.

It is possible to map your company's stock organization in the program. You define the locations, corridors, shelves, up to the individual trays and specify which single articles, sqm articles and linm articles are located at which storage location.

*Fig. G-2 Overview of stock management*
*(Image shows a flowchart illustrating the stock management process. An "Order" can lead to a "Stock article" reservation from "Stock on hand". If there's a "Stock shortage", it triggers a "P.O. item" in "Purchasing". The "Supplier" provides goods, which are processed through "Receipt of goods", leading to a "Booking addition to stock". When materials are used, "Booking out of stock" occurs, linked to "Delivery note" and "Invoices". All processes feed into "Analyses".)*

All commercial transactions in *A+W Business* are based on the master data. Only if the master data is properly maintained, stock can be managed without problems. In conjunction with Sales and Purchasing, the following processes are created:

- **Order:**
  An order defines the customer's purchase order. You enter all the items that must be produced in accordance with the customer's specifications.
- **Transfer to production:**
  Order items to be produced are transferred to production. The required materials are reserved and are booked out of stock when the delivery note or invoice is printed. At the same time, the available stock on hand is updated.
- **Stock P.O.**
  If stock articles fall short of the minimum stock, these stock articles must be entered in the form of a stock P.O.
- **Stock addition:**
  The stock on hand of the stock articles is updated by entering the goods receipt. Articles that are not kept as stock articles cannot be kept as stock on hand.
- **Inventory:**
  With the inventory you correct the stock on hand figures in *A+W Business*.

### Stock management processes
You usually maintain the stock on hand by carrying out the following activities:
- Set up master data
- Enter stock articles (initial inventory)
- Book receipt and issue of goods (automatically, manually)
- Queries concerning stock turnover, prices, stocks on hand, etc.
- Enter, check and send stock P.O.
- Carry out inventory:
  - Create inventory list, add supplementary inventory
  - Determine target inventory
  - Print count lists
  - Enter counted values
  - Finalize inventory

### How should stock be managed
All products that are entered in Sales are assigned with a code that defines the type of purchase. In addition to the code (procurement type) *Stock Withdrawal*, glass pieces that are kept on stock have a code (stock booking type) to indicate how its stock on hand is calculated. These two codes are described in the thematic block Master Data.

Before you set up your stock in *A+W Business*, you have to decide on the basis of how your stocks should be managed: as an area (sqm) or in numbers of pieces. A third possibility is the combined stockkeeping, whereby the size-dependent stock mode is combined with the reports from the optimization so that in addition to the stock dimensions, the stock sizes cut can be booked out automatically.

These different options have different effects:

| Mode (Stock code)             | Meaning, example                                                                                                                                                             | Disadvantage                                                                      |
| :---------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------- |
| **sqm = area: (not size-related)** | the area is determined per glass piece:<br>- Float 4 => 10,500 sqm<br>- Float 5 => 11,070 sqm<br>- Float 6 => x sqm                                                        | - no information about the number of stock sizes<br>- no information about how many stock sizes were cut |
| **Piece: (size-related)**     | the quantity is determined per jumbo size and per stock size:<br>- Float 4: 3 pieces of 3210/6000, 3 pieces of 900/1200, n pieces of x/x<br>- Float 5: 3 pieces of 3210/6000, 3 pieces of 800/1200, n pieces of x/x | - no information on the cut jumbo and stock sizes<br>- Stock sizes must be booked out manually |
| **Piece incl. reports: (combined)** | Combination of size-related stock and reports. The cut stock sizes and stock dimensions are automatically booked out. The stock quantity of the quantities are updated. | (For this mode, A+W Optimizer reports must be permitted.)                         |

After deciding about the mode, allocate the corresponding stock code per glass product and define the stockkeeping mode in the company data. These settings are described in the thematic block *Master Data*.

## Master Data

In this thematic block, we will show you how you maintain the master data for managing your stock.

This includes the following training modules:
- "Stock" on page G-18
- "Company Data" on page G-27
- "Status" on page G-32
- "Product Definition" on page G-35
- "Prices" on page G-48

### Stock

#### Objectives
- Name stock levels.
- Define storage location.
- Define stock categories.

#### Benefits
- With storage places you can manage (the same) materials at different locations.
- Analyses can refer to certain storage locations or stock articles that are stored at different locations.

#### Please note:
- **Levels**: Four different levels define e.g. various warehouses, corridors, shelves, and trays.
- **Storage locations**: The combination of the different differentiation levels form the storage locations.
- **Stock categories**: By using stock categories you can restrict the search and analysis to certain products that are stored at different locations.
- **Default settings**: None

### Stock Definition
Set the following settings to display your stock:
- Names of stock levels
- Stock levels
- Storage locations

You can adjust the names of the different levels to the requirements in your company. You should also use this option if you only work with one level.

#### Storage location
You can specify up to four differentiation level to define storage places to differentiate for example between warehouses, aisles, shelves and trays. The storage locations are used for stock management and for the inventory.

*Fig. G-3 Example: Storage location = Warehouse 1*
*(Diagram shows a hierarchical storage structure: Warehouse 1 contains Corridor A and Corridor B. Corridor A has Shelf 1 and Shelf 2, which in turn contain Trays 1-6. Corridor B has Shelf m and Shelf n.)*

#### Stock level
For each level you can define different names, e. g. on level 1 the warehouses at different storage places, on level 2 corridors A through F, etc.

> **i Define at least one storage location**
> You must define a storage location even if you did not divide your stock. In this case, just define level 1 and then define all other levels in the storage location as `<n.e.>`.

### Stock Categories
Stock categories provide you with another search criterion for stock management. For example, if you manage the same material at different storage locations, you can use the stock category to analyze the materials together. For this purpose you must have defined all storage locations where the materials are actually kept.

Assign the defined stock categories to the products in the *Stock Management* dialog.

### Define Stock Levels
This module shows you how to adjust the stock levels to the requirements in your company.
The following instructions exist for this training module:
- "How you define your different stock levels" on page G-20
- "How to name stock levels" on page G-22

#### How you define your different stock levels
The following steps are the same for all stock levels. In this example, we will create a stock level 1 for finished products.

1.  Select menu *Master data > Stock > Level 1*. Dialog *Level 1* opens.
2.  Go to the menu *Start > New* to switch to the input mode.
    *Fig. G-4 Line for new stock level*
    *(Image shows a dialog for Level 1, with existing entries for "Zentrallager/Central stock" and "Außenlager/External storage area" and a new blank line for input.)*
3.  Enter a name for the stock level, e. g. name of the place, cutting, etc.
4.  Go to the menu *Start > Save* to save the data. The data is saved.
5.  Repeat steps 1 through 4 for all levels that you would like to differentiate between in your stock. For this purpose, also open the dialogs to stock levels 2 through 4 and proceed in the same way.

#### How to name stock levels
1.  Select menu *Master data > Stock > Stock definition*. Dialog *Stock definition* opens.
2.  Go to menu *Definition > Levels*.
    *Fig. G-5 Name stock levels*
    *(Image shows the "Stock levels" dialog where names for Level 1 to 4 can be defined, e.g., Level 1: Warehouse, Level 2: Corridor, etc.)*
3.  Define the names of the stock levels, e. g. **Warehouse** for level 1.
4.  Click on [OK] to save the names. The dialog closes. The changes are adopted in the *Stock definition* dialog.
5.  Close the *Stock definition* dialog or define the storage locations now.

### Define Storage Location
This training module shows you how to set up storage locations in *A+W Business*.

You must define a storage location even if you did not divide your stock. In this case, just define level 1 and then define all other levels for the storage location as `<n.e.>`. Please note that a storage location with the definition `<n.e.>` can also be used for booking purposes as the storage location for all levels.

> **i Tip**
> You can move certain materials from a warehouse to the production area. For this purpose, the storage location is changed. In this case, it is helpful if you define the storage location as precisely (detailed) as possible, e. g. concerning the trays.

#### How to define a storage location
1.  Select menu *Master data > Stock > Stock definition*.
    *Fig. G-6 Define storage locations*
    *(Image shows the "Stock definition" dialog. Area A shows dropdowns for each level (Warehouse, Corridor, Shelf, Tray). Area B shows a list of already defined storage locations.)*
    **A** Your selected name of the levels
    **B** List of defined storage locations

    Use this mode to change the defined storage location (A), by changing the names of the levels. The fields of the table are locked if you have chosen the input mode.
2.  Go to the menu *Start > New* to switch to the input mode.
    *Fig. G-7 Fields in the table locked*
    *(Image shows the same dialog in input mode. Area A allows selection from defined stock levels. Area B shows parameters like "Locked" and "Warehouse type".)*
    **A** Selection of defined stock levels
    **B** Parameters
3.  Select an entry on each level (A).
4.  Define one of the parameters (B), if applicable, if the storage location shall be specifically marked, e. g. as default stock.
    If you have selected the entry *Hegla* as stock type, you can specify the storage location for the goods receipt from the Hegla deliveries.
5.  Go to *Menu Start > Save* to save the storage location. The data is saved.
6.  Repeat steps 2 through 5 for all storage location that you require for managing your stock.

### Define Stock Categories
This module shows you how you define the stock categories that you want to allocate to the stock articles.

#### How to define a stock category
1.  Select menu *Master data > Stock > Category*.
    *Fig. G-8 Stock categories*
    *(Image shows the "Stock Category" dialog with columns for ID and Comment, listing entries like "Floatglas" and "Ornament".)*
2.  Go to the menu *Start > New* to switch to the input mode.
3.  Enter an ID for the stock category, e. g. figures or names, such as **raw material**, **production**.
4.  Go to the menu *Start > Save* to save the data. The data is saved.
