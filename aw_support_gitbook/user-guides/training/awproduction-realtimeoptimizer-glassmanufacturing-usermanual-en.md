---
title: "A+W Production Packing Optimization - Software Reference"
category: "training"
product: "AWProduction"
doc_type: "User Manual"
language: "EN"
tags: ["AWProduction", "RealtimeOptimizer", "GlassManufacturing", "UserManual"]
version: "1.0"
last_updated: "2025-12-10"
description: "title: "EN_UM_AWProduction_12" source: "EN_UM_AWProduction_12.pdf" tags: ["A+W Production", "Realtime Optimizer", "Software Reference", "Glass Manufacturing", "Windows and Doors", "Cutting Optimization", "Packing Optimization", "Software Tutorial"] version: "1.0" last_updated: "2025-10-03" short_description: "A user manual for the A+W Production Realtime Optimizer and Packing Optimization software. This document serves as a software reference and tutorial, detailing functionalities for optimizin"
source_file: "AWProduction-RealtimeOptimizer-GlassManufacturing-UserManual-EN.md"
---


title: "EN_UM_AWProduction_12"
source: "EN_UM_AWProduction_12.pdf"
tags: ["A+W Production", "Realtime Optimizer", "Software Reference", "Glass Manufacturing", "Windows and Doors", "Cutting Optimization", "Packing Optimization", "Software Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A user manual for the A+W Production Realtime Optimizer and Packing Optimization software. This document serves as a software reference and tutorial, detailing functionalities for optimizing glass cutting and packing processes. It covers weight distribution, load balancing, and integration with various modules."
long_description: "This document is a comprehensive user manual for A+W's software solutions, specifically the 'A+W Production Realtime Optimizer' and 'A+W Production Packing Optimization'. It is structured into two main parts: a tutorial and a software reference. The tutorial section provides step-by-step guidance on using the software, covering basic ideas, data import, optimization techniques, cutting processes, and interplay with other modules like the Residual Stock Manager, Pattern Viewer, and DynOpt Compact. The software reference section offers detailed descriptions of all menus, dialogs, fields, and functions available within the software. Key topics include managing rush orders, creating manual cutting plans, handling rejects, optimizing cutting tables for yield improvement, and controlling the cutting process. The manual is intended for operators and administrators of the A+W software, providing the necessary information to efficiently manage and optimize the production of glass, windows, and doors."
---

# A+W Production Packing Optimization - Software Reference

## Menus

### Section B

Section B shows the weight distribution in kg, per rack and per side.

**Fig. 1-64: Weight in kg**
`383 (183+200) Kg`

For the image above, this means: The total rack weight is 383 kg. The values in brackets show the weight per rack side, i.e. 183 kg for side 1 and 200 kg for side 2.

### Section C

Section C shows the load distribution in % for the right and left side of the rack.

**Fig. 1-65: Weight in %**
`51% 49%`

For the image above, this means: 51 % of the load are on the left and 49 % on the right. The percentage also considers the weight of units on the outside as compared with units on the inside. This may result in distinctive differences in the load distribution (such as 30 % vs. 70 %).

---

# A+W Production Realtime Optimizer

## Revision overview of the module

| Date | Change |
| :--- | :--- |
| **05-2024** | Stack number added |
| **01-2023** | Additions |
| **10-2020** | Dialog Table Optimization added |
| **04-2019** | Dialog DynOpt Settings added |
| **09-2018** | Fields added |
| **01-2017** | Product and company names adjusted. |
| **03-2015** | Complete revision |
| **07-2013** | Complete revision of XOPT-ON documentation and adjustment to A+W Production. |
| **09-2007** | Complete revision |
| **03-2003** | Original version |

**This module provides information on the following subjects:**
- Tutorial
- Software Reference

---

# Tutorial

This section provides information on the following subjects:
- Basic Ideas
- Using A+W Production
- Input
- Optimization
- Cutting
- Interplay with Other Modules

## Table of Contents

*   **Basic Ideas** - J-1108
    *   Features - J-1109
*   **Using A+W Production** - J-1110
    *   Overview - J-1111
    *   Import of data - J-1112
    *   Working with A+W Production - J-1113
    *   Master data - J-1114
    *   Use as a stand-alone system - J-1114
    *   Import optimizations - J-1114
*   **Input** - J-1116
    *   Overview - J-1117
    *   Rejects, rush order lites or filler orders - J-1118
    *   Manual entry of lites - J-1119
    *   Manual creation of plans - J-1122
    *   Charge editor - J-1123
*   **Optimization** - J-1124
    *   Overview - J-1125
    *   Cutting table optimizations - J-1126
    *   Create table optimizations - J-1126
    *   Check and process table optimization result - J-1128
    *   Resolve table optimization - J-1129
    *   Linking of table optimizations - J-1131
    *   Create a quick optimization - J-1132
    *   Linking of batches - J-1133
    *   Cutting table control - J-1134
*   **Cutting** - J-1135
    *   Overview - J-1136
    *   Selecting batches for cutting - J-1137
    *   Check optimization and cut - J-1140
    *   Interrupt and continue work - J-1142
    *   Cutting overview - J-1143
    *   Reset cutting status - J-1145
*   **Interplay with Other Modules** - J-1146
    *   Overview - J-1147
    *   A+W Residual Stock Manager - J-1147
    *   A+W Planning Web - J-1147
    *   Interface - J-1148
    *   Master data - J-1148
    *   A+W Pattern Viewer - J-1156
    *   Settings - J-1156
    *   The interface - J-1157
    *   The menu bar - J-1157
    *   Information about lite and waste - J-1167
    *   Display linked batches - J-1167
    *   Display setting edge - J-1168
    *   Display symbol for processings, stamp, logo or reference mark - J-1168
    *   Color selection for order items - J-1169
    *   Mark the first and last lite - J-1169
    *   Rejects - J-1170
    *   A+W PlanEditor - J-1171
    *   A+W Continuous Cutting - J-1172
    *   Overview of the planned batches - J-1172
    *   Grouping - J-1175
    *   Rush groups - J-1176
    *   Resetting batches - J-1176
    *   Cutting - J-1176
    *   A+W Defect Optimizer - J-1178
    *   A+W DynOpt Compact - J-1179
    *   A+W DynOpt Compact Import - J-1179
    *   A+W DynOpt Compact Optimization - J-1179
    *   Create A+W DynOpt Compact batch - J-1180

## Basic Ideas

A major potential for saving in flat glass processing is the optimal use of the stockplates at cutting. The smaller the waste or the residual plates, the greater is the use of material, and the lower the material cost. Controlling cutting tables with optimized cutting plans directly from the optimization speeds up the work process.

A+W Production is based on two fundamental ideas:
- Cutting optimization for the linked cutting table
- Transfer of cutting codes to the linked cutting table

*Fig. J-1: A screenshot showing the cutting optimization and cutting table control interface.*

### Features

A+W Production supports these fundamental ideas with the following features:
- A+W Production controls cutting by means of optimized detailed scheduling data.
- Rush orders, rejects or filler sizes can be automatically re-optimized in a residual plate.
- Cutting tables are controlled mainly online by means of communication logs supported by the table manufacturers.
- Rush order lites, rejects, and fillers are optimized directly at the cutting table.
- Existing optimizations can be checked with regard to table optimization, to be resolved and reassembled if required. By adding rejects, filler sizes and rush order lites, bigger optimizations can be created. Defined sequences on A racks are maintained.
- Even at the detailed scheduling stage, A+W Production allows optimizing the cutting of every batch on the scheduled cutting table.
- A+W Production is especially configured for a cutting table, and can transfer the scheduled and optimized batches to this cutting table, together with the cutting code.
- Once the appropriate cutting code has been transferred to the cutting table, the breakout pattern can be displayed via XTV.

## Using A+W Production

This subject area introduces the functions of A+W Production.
This subject area includes the following training sessions:
- Import of data
- Working with A+W Production
- Use as a stand-alone system

### Overview

**Objectives**
- Getting to know and understanding import of data
- Getting to know and understanding the connection to A+W Production.
- Getting to know and understanding the operation as stand-alone system

**Benefit**
The data has to be imported correctly before working with A+W Production.

**Definitions**
- **Pre-systems**: These systems supply orders (batches) containing master data and cutting optimizations.
- **Stand-alone variant**: The stand-alone system imports the data by means of save files which must be provided in a special directory.
- **Residual stock**: The residual stock manages residual plates at the cutting table.

**Note**
- **A+W Production**: Can be adapted to all common cutting tables.
- **Stand-alone variant**: The A+W Production can be used stand-alone.
- **Connection**: The staff of A+W configure the import of data.

### Import of data

Depending on the basic system, data is imported fully or semi-automatically. These systems supply A+W Production with orders (batches) containing master data and cutting optimizations.

*Fig. J-2: A diagram showing an overview of the work with A+W Production. Batches are fed into the A+W Realtime Optimizer, which handles optimization and cutting code creation, interacts with a database, and controls the cutting table.*

A multitude of possible configurations open up the following possibilities in connection with A+W Production:
- Integrated into an A+W Production or an A+W Business Pro environment.
- Adapting to all common cutting tables
- Link to a residual stock
- Use as a stand-alone system

The system is configured and installed by A+W staff.

Possible basic systems are:
- A+W Production
- A+W Business Pro

> **Linking to the basic system**
> The staff of A+W configure the basic system and the import of data.

*Fig. J-3: A diagram showing data import in A+W Production. Import files are processed by the A+W Realtime Optimizer, which checks and imports data into the A+W Production database containing batches, master data, articles, glass types, tables, and optimization parameters.*

If A+W Production works with A+W Production, A+W Production uses the A+W Production database as well. If another system is used, A+W Production needs an empty A+W Production database. Master data and optimizations included in the batches of the basic system will be adopted by A+W Production into the empty A+W Production database. Data is checked at the same time.

The system rejects data that causes errors during import. The error log shows why the individual records were rejected. The data can be processed further.

#### Working with A+W Production

When A+W Production is linked to an existing A+W Production system, data is exchanged automatically. Master data, batches, rejects, rush and filler orders are directly loaded from the A+W Production database. Apart from that, status reports for the individual batches are saved in the database.

#### Master data

If the access to master data was released at configuration, these can be viewed and processed.

Master data includes:
- Articles
- Glass Types
- Tables
- Optimization parameters
- Stockplates

Master data and their use are described in the Detailed Scheduling section of the A+W Production user manual.

#### Use as a stand-alone system

A+W Production is installed with an empty A+W Production database. When batches are imported, the database is filled with master data.

The stand-alone system imports the data by means of save files, which must be provided to A+W Production in a special directory. Save files have to stick to a defined structure and are usually available in the working directory `.\Xopton\im-port\work\*save.*`. Imported data is removed from the working directory, and transferred to archives.

#### Import optimizations

The Import optimizations function is only required and valid for A+W Production stand-alone versions.
A+W Production can supply a cutting table with cutting data or create table optimizations if batches are provided by another system. If batches are supplied, A+W Production can import them for further processing.

The following steps can be performed in connection with the import of batches:
- Switch on import.
- Switch off import.
- React to error reports.

**Switch on import**
1.  Open the Import dialog. Select `View > Import`.
2.  Use the [Start] button to start the import.
    A+W Production checks the working directory for import files. If import files are found, the data are imported into the database while the import files are transferred to archives.
    Imported batches are available for further processing on the `Select a batch` and `Select glass for optimization` dialogs.
    Button [Start] becomes [Stop].
3.  Close the dialog. Click the [Close] button.

A+W Production monitors the working directory until the import function is switched off.
Should errors occur during import, these are recorded; and the batches in question will not be imported. Errors can be processed manually.

**Switch off import**
1.  Open the Import dialog. As long as import is switched on, a minimized dialog is shown in the bottom left corner of the A+W Production dialog.
2.  Use the [Stop] button to terminate import.
    Import files just stored in the working directory remain there, unprocessed.
    Button [Stop] changes into [Start].
3.  Close the dialog. Click the [Close] button.

**React to error reports**
Should errors occur during import, these are recorded; and the batches in question will not be imported.
Import is stopped only if there is an imminent loss of data. This may be the case if an existing optimization should be overridden. Depending on the configuration, an error message appears.
1.  Answer the question in the error report dialog xopt-on. Select the appropriate button, [Yes] or [No]. Import of data is resumed.
2.  Open Error messages dialog. Select `View > Error reports` menu.
3.  Check the error messages and respond accordingly.

> **Additional information**
> - "React to error reports" on page J-1115
> - Software Reference, "Error reports" on page J-1254

## Input

This section tells you how to handle the input.
This subject area includes the following training sessions:
- Rejects, rush order lites or filler orders
- Manual creation of plans
- Charge editor

### Overview

**Objectives**
- Getting to know and understanding rejects.
- Getting to know and understanding rush order lites.
- Getting to know and understanding filler orders.

**Benefit**
By using rejects, rush order lites and filler orders you can improve the yield.

**Definitions**
- **Reject**: A lite broken during cutting.
- **Rush order lite**: A lite, that must be cut quickly
- **Filler order**: Serves to use capacities and material efficiently.

**Note**
- **Rejects**: Rejects can be entered manually via A+W Production, or at another place within a networked production.
- **Rush order lites**: Rush order lites are created by A+W Production and are saved in the database.
- **Filler orders**: Filler orders can be used only if A+W Production is used together with AWP.

### Rejects, rush order lites or filler orders

Rejects can be entered manually via A+W Production, or at another place within a networked production. Depending on the configuration, rejects are shown directly in the A+W Production rejects pool. At the next opportunity, the broken lites are optimized automatically with the residual plate, or (depending on the configuration) integrated manually into a table optimization.

Rush order lites are created by A+W Production and are saved in the database. Rush orders can be integrated in the next table optimization with a suitable glass type and thickness.

Filler orders can be used only if A+W Production is used together with A+W Production. In this case, filler orders are directly taken from the A+W Production database.

*Fig. J-4: A diagram showing input and processing of data in A+W Production. Rush order lites, Breakage, and Filler are fed into the Realtime Optimizer to create table optimizations, which interacts with the A+W Production database.*

### Manual entry of lites

In addition to batches from another system, A+W Production allows to enter lites, add them to table optimizations, and transfer them to the cutting table.

Use the following steps to enter or delete lites manually:
- Enter rush order lites.
- Editing rush order lites.
- Delete rush order lites.
- Enter rejects.
- Delete rejects.

#### Enter rush order lites
1.  Open dialog **Rush order lites**. Select menu `Input > Rush order lites`. The Rush orders dialog shows all entered rush order lites that have not been used in an optimization so far.
2.  Open the **Enter rush order lites** dialog. Click the [Add] button.
3.  In the **Glass type** field, select the glass type for these rush order lites. If various thicknesses are available, enter the required thickness in field **Thickness**.
4.  In field **Rack**, enter the rack onto which the rush order lites should be put after cutting. Depending on the organization, this field can also remain empty.
5.  Enter the number of lites in field **Quantity**.
6.  In the **Shape** field, select the shape number if you want to enter a shape. If you want to enter shaped lites, you can also edit the shapes. To do this, use the [^] button. You can also define a free shape for rush order lites. Enter shape number 99. Select the corresponding SN file (entered and exported as Block-Ind file via CAD Designer Shapes from the catalog directory).
7.  Enter the lite dimensions in the fields **Width** and **Height**. When you enter a shape, these fields automatically show the dimensions of the surrounding rectangle.
8.  Save the input of rush order lites. Click the [OK] button. Entered data are saved and shown in the list.
9.  Enter more lites or close the dialog. To enter more lites, repeat the procedure starting from step 2. Use the [End] button to close the dialog.

#### Editing rush order lites
1.  Open the dialog **Enter rush order lites**. Select menu `Input > Rush order lites`. Dialog Rush order lites shows all entered rush order lites that have not been used in an optimization so far.
2.  On the rush order list, tag the line you want to edit.
3.  Click the [Edit] button. This opens the **Rush order lite entry** dialog. The fields show the data of the lite you want to change.
4.  Enter the required changes and quit the dialog using [OK].

#### Delete rush order lites
1.  Open the **Enter rush order lites** dialog. Select the `Input > Rush order lites` menu. The Rush order lites dialog shows all entered rush order lites that have not been used in an optimization so far.
2.  Tag a line in the list of rush orders.
3.  Click the [Delete] button. The tagged rush order lite will be deleted.
4.  Close the dialog. Click the [OK] button.

#### Enter rejects
If you use A+W Production (XTV) at the cutting table, rejects can be entered directly at the table, and is automatically transferred to A+W Production. Rejects can also be entered manually:
1.  Open the dialog **Add Rejects**. Select menu `Cutting > Reject pool > [Add]`.
2.  In the **Product ID** section, enter order number, item number, and sub item number to which the broken lite belongs.
3.  If you are working with barcoding, you can enter the reject reason. Select the appropriate entry from the combo box **Reject reason**.
4.  Save the entries. Click the [Save] button.

#### Delete rejects
1.  Open the dialog **Rejects pool**. Select menu `Cutting > Rejects pool`. The Rejects pool dialog shows all broken lites that have been entered, and have not been used for optimization.
2.  Tag one or more lines on the reject list.
3.  Click the [Delete] button. The tagged reject will be deleted.
4.  Close the dialog. Click the [Close] button.

> **Booking rejects**
> Use the [Booking F5] button to transfer the rejects to production. In case you have reported lites as rejects by mistake, you can also use this button the report the lites as OK.

> **Additional information**
> - Software Reference, "Input of shapes" on page J-1243
> - Software Reference, "Rush order lites" on page J-1189
> - Software Reference, "Rejects pool" on page J-1239
> - Software Reference, "Add rejects" on page J-1241

### Manual creation of plans

This option allows you to create a purely manual plan and save it as table optimization in the database. The manual plan can be edited and changed afterwards. This is done by means of the A+W PlanEdit module. For details on this module, please refer to the corresponding documentation. No barcode information will be available for manual plans.

**How to create a new plan**
1.  Select menu `Input > Manual Plan`. The **Manual Plan Input Cutting Table ...** dialog opens.
2.  In section **Glass Types** select the glass type you want to create the plan for.
3.  On the left select the stock dimension in the **Stockplates** section that should be used for the manual cutting pattern.
4.  In section **Residue Plates** define height and width for the residual plate to be created.
5.  Click the [New] icon. A+W PlanEditor opens.
6.  Enter the requested lites via the context menu. Thus, select the **Insert** option and enter the specific lite data.
7.  Via `File > Save as` it is possible to save the cutting plan as file.
8.  Use `Output > AWC` for transfer to cutting.

**How to edit a manual plan**
1.  To edit a manually entered cutting plan, select `Input > Manual Plan` from the menu. The **Manual Plan Input Cutting Table ...** dialog opens. The lower section **Plan** shows the plan previously entered.
2.  Use the [Edit] button to open the plan, previously entered and make the modifications.
3.  Don't forget to save the modifications or to release the data via `Output > AWC`.

**How to select a plan manually entered for cutting**
1.  A plan entered manually can only be cut directly via **Cutting**.
2.  Use the [Cutting] button to select all batches optimized and prepared for cutting.
3.  The manually created plan appears in the list of available batches with batch number >15000 and has the additional information **PlanEdit**.
4.  Select the batch and prepare it for cutting ([Options] button) or cut it directly ([Cutting] button).

> **Additional information**
> - Software Reference, "Manual creation of plans" on page J-1196

### Charge editor

Via this dialog it is possible to define a charge number. Tag the checkbox and the entered charge number will be inherited to the following stockplates of the same glass type/thickness. The last charge number is saved per glass type/thickness/stockplate. Next time, this editor will be opened the input field will be preset with this value. The allocation always affects the selected stock dimension (and in case of inheritance those below).

A set charge (including inheritance) can also be deleted via this editor.

If the cutting process for a stock dimension has no batch allocation, the user has to enter a charge number first. The Charge Editor dialog appears with a corresponding info in A+W Production Terminal (XTV).

> **Additional information**
> - Software Reference, "Charge editor" on page J-1199

## Optimization

This section shows you how the optimization works.
This subject area includes the following training sessions:
- Cutting table optimizations
- Create a quick optimization
- Linking of batches
- Cutting table control

### Overview

**Objectives**
- Getting to know and understanding table optimizations
- Getting to know and understanding quick optimizations
- Getting to know and understanding linking of residual plates
- Getting to know and understanding cutting table control

**Benefit**
The more efficiently the optimization works, the higher the yield. This saves money.

**Definitions**
- **Cutting table optimizations**: Optimizations, created with A+W Production.
- **Quick optimization**: Plates, not sent yet to the cutting table can be resolved completely and re-optimized.

**Note**
- **Batch**: A batch is a composition of glass from one or more orders, to be considered and produced at once in optimization and production (e.g., same route, same customer, same glass types, same production dates). The optimizations of prior systems exist in the shape of batches.
- **Lot**: A part / a glass type of a batch, that should be processed / cut under identical conditions at the same time (e.g. all Float 4 of a batch).
- **Cutting table control**: The cutting table to be controlled by A+W Production is defined during installation.
- **Rejects**: Can either be cut in the re-optimization at the end of a batch to be cut or transferred to rejects pool and can be cut together with the next batch.

### Cutting table optimizations

Table optimizations are optimizations created by A+W Production. Upstream systems provide complete optimizations that are resolved by A+W Production to be rearranged. You can combine any number of batches, provided there is enough space for the racks at the cutting table.

When you create table optimizations, you can take into account residual plates on the cutting table, use different stockplates, or use a residual stock. Rejects, rush or filler orders can be excluded or integrated as required.

Table optimizations are saved in the database, and are used for cutting if required.

#### Create table optimizations

The following steps are necessary when creating a new table optimization:
- Select glass type and batch for table optimization.
- Create table optimization.

**Select glass type and batch for table optimization**
1.  Open the dialog **Select glass for optimization**. Select `Optimization > Table Optimization`.
2.  From the **Glass type** list, select the glass type to be optimized. The **Glass type** list shows if special orders (reject, rush order lites, etc.) exist in A+W Production for the glass type.
    - If you select a glass type for which there are broken lites or rush order lites, these will be automatically integrated in the new table optimization (if configured).
    - If your system is configured to work with residual plate storage, this list shows whether a residual plate is available for the glass type in question.
    - The **Available optimizations** list shows all batches containing optimizations for the glass type and thickness selected from the **Glass type** list.
3.  Tag the **Permit manual cutting** checkbox to show even glass types that are only meant to be cut manually.
4.  From the list **Available optimizations** select the batches to be arranged in a table optimization.
    > **Select only rejects and rush order lites**
    > If there are broken lites or rush order lites for the selected glass type, these lites can be optimized without another batch. Do not select a batch from the list in this case.
    > If you have tagged a batch but do not want to select it, change the selected glass type. When you select the required glass type again, no batch will be tagged.
5.  Click [Select] to compile the selected batches in a table optimization.
The dialog closes. Dialog **Table optimization** appears in which the tab **Optimize** shows the selected batches.

**Create table optimization**
1.  Please make sure that in the previous step, **Select batches for table optimization**, batches have been actually selected. Dialog **Table optimization** appears with the tab **Optimize**.
2.  Select the necessary optimization parameters.
3.  Select the required parameter from tab **Stockplates**.
4.  Select the required parameters from tab **Filler**.
5.  To create the optimization, return to tab **Optimize** and click the [Optimize] button. The calculation of the optimization starts, the dialog disappears, and the optimization is run in the background. As long as the optimization is running, you can go on working with A+W Production. As soon as the optimization result is available, the dialog reappears automatically. The optimization result is shown on the **Overview** tab.
6.  To save the optimization, click [Save].
The optimization is now shown on the **Select a batch** dialog and can be transferred to the cutting table.

> **Additional Information**
> - Software Reference, "Select glass for optimization" on page J-1202
> - Software Reference, "Optimize" on page J-1210
> - Software Reference, "Residue plates and stockplates" on page J-1212
> - "Selecting batches for cutting" on page J-1137

### Check and process table optimization result

Table optimizations can be checked anytime before they are transferred to the cutting table. To change a table optimization, to add reject, rush order lites, or filler sizes, or to add or delete whole jobs, you need to resolve the entire optimization, and create a new one.

The following steps are possible when creating a table optimization:
- Select other stockplates for optimization.
- Use residual plate from previous optimization.
- Add filler sizes to the optimization.

Changes are impossible once a table optimization was saved.

**Select other stockplates for optimization**
1.  From dialog **Table optimization**, select tab **Stockplates**. The list on the right side shows all stockplates defined in master data for this glass type and thickness, which are available for cutting.
2.  Tag the stockplate(s) A+W Production may use for cutting optimization. During optimization A+W Production checks how many lites of which size are needed to achieve the optimum result.
3.  To create the optimization, switch to the tab **Optimize** and click the [Start] button.
4.  To save the optimization, click [Save].

**Use residual plate from previous optimization**
1.  From dialog **Table optimization**, select tab **Stockplates**. If there is a residual plate of the same glass type and thickness on the cutting table as required in the present optimization, this can be integrated in the table optimization.
2.  Enter the height and width of the residual plate on the cutting table in section **Residual plate**.
3.  To create the optimization, switch to the tab **Optimize** and click the [Start] button.
4.  To save the optimization, click [Save].

**Add filler sizes to the optimization**
1.  From dialog **Table optimization**, select tab **Filler**. The list on the right shows all filler orders defined for the glass type and thickness of this batch.
2.  Tag the filler orders to be integrated into the table optimization. Ideally, filler orders are used to minimize the waste, or the residual plate.
3.  To create the optimization, go to tab **Optimize** and click [Optimize].
4.  Continue to add or delete filler orders until the optimum result is reached.
5.  To save the optimization, click [Save].

> **Additional information**
> - "Resolve table optimization" on page J-1129

### Resolve table optimization

Table optimizations can be resolved only if they were saved after having been created. As long as **Table optimization** dialog is open and the table optimization in question has not been saved, the optimization can be rejected by pressing the Cancel button.

When you resolve a table optimization, the batches included are returned to the batch list. Possibly included breakage, rush order lites, or filler orders are returned to the appropriate pools, and are available again for new optimizations.

Optimizations for which cutting was started and cancelled, can also be resolved. Batches for which lites were cut already are reset and treated as if cutting had not taken place.

**Resolve created and saved table optimizations**
1.  Open the dialog **Reset cutting batch**. This is done in menu `Optimization > Reset`. The **Reset a cutting batch** dialog shows a list of all batches available for status changes. The list is sorted by batch numbers. Table optimizations are shown as batches with numbers starting from 15000 (can be configured).
2.  Tag the table optimization you want to break down. Tag the corresponding batch with a number higher than 15000. You can tag several table optimizations to be resolved at the same time.
3.  To save the optimization, click the [OK] button. A security query appears.
4.  Confirm this query. Select the [Yes] button.
The batches and lites of the selected table optimization are now available for new table optimizations. If the table optimization was using ReMaster lites, these are available again after the optimization was resolved.

> **Additional information**
> - "Create table optimizations" on page J-1126

### Linking of table optimizations

To improve the waste it is possible to link table optimizations. Linking is only possible for table optimizations with the same glass types, which means that the table optimizations must exist.

To link table optimizations the following steps are required:
- Select glass type and batch for table optimization.
- Create table optimization.

**Linking of table optimizations**
1.  Open the dialog **Select glass for optimization**. Select `Optimization > Table optimization`.
2.  From the **Glass type** list, select the glass type to be optimized. The **Glass type** list shows if special orders (rejects, rush order lites, etc.) exist in A+W Production for the glass type. If you select a glass type for which there are broken lites or rush order lites, these will be automatically integrated in the new table optimization (if configured). If your system is configured to work with residual storage, this list shows whether a residual plate is available for the glass type in question. The list **Available optimizations** shows all batches containing optimizations for the glass type and thickness selected from the list **Glass type**.
3.  Tag the checkbox **Permit manual cutting** to show even glass types that are only meant to be cut manually.
4.  From the list **Available optimizations** select the batches to be arranged in a table optimization.

> **Additional information**
> - "Linking of table optimizations" on page J-1131

### Create a quick optimization

Plates / patterns already optimized (via A+W Production or via Table optimization in A+W Realtime Optimizer), but still not sent to the table, can be resolved completely and re-optimized. Thus, rush order lites and rejects will also be optimized and a completely new cutting pattern is the result for the re-optimized plates.

The following steps are necessary when creating a quick optimization:
- Create table optimization.
- Cutting of table optimization has been started

In case of reject during cutting, this can be re-cut in real-time by using the quick optimization.

*Fig. J-5: A screenshot showing the Cutting overview.*

Via the context menu it is possible to resolve the optimization from the next pattern on and to re-optimize.

In example Fig. J-5 (Cutting overview) the patterns / plates 1 and 2 were sent to table and cut. The plates / patterns 3-6 can be resolved and re-optimized (quick optimizations) via right click.

*Fig. J-6: A context menu showing "Resolve and re-optimize optimization 1004 lot 1 from pattern 7 on."*

After confirming the message the plates still to be cut will be removed. Then, the broken lites and the plates still to be cut will be re-optimized.

> **Additional information**
> - "Cutting overview" on page J-1143

### Linking of batches

With the linking of batches, A+W allows you to avoid residual plates. In the past, residual plates had to be assembled manually. This is no longer necessary.

Linking takes place during cutting and is synchronized with it.

**Batch: #** dialog activates the option for linking batches in section **Residual plate management**.

When cutting is started, the system will send the first pattern of a batch then search - starting from the next batch- the database for a suitable batch of this glass type; the corresponding data will be loaded.

The next batch must have the status **Released**. The batch is loaded in the background so as not to interrupt cutting. When the penultimate lite (can be configured) of a glass type has been cut, the user will be informed (optionally!) as to which batch and lot the residual plate will be linked to. The user can abort the linking at this point or choose a corresponding lot.

When the user confirms this link, rush order lites and rejects of this glass type will be loaded, and added to the next optimization with priority 0. The residual plate of the currently cut batch becomes the start plate of the next optimization. Then optimization is started. After the optimization, the next optimization will be linked with the original optimization so that the residual plate of the original optimization will be filled with the lites of the first plate of the next optimization. All other patterns of the next optimization will be resolved in the last cut optimization. The system now creates and transfers a new cutting code.

The first pattern of the next optimization is market **Cut**. Using the mechanism from the table optimization, the next optimization is first saved as a table optimization, after which the batch and batch number of the original, next optimization are added. The status of the next optimization is changed to **Started**.

> **Additional information**
> - Software Reference, "Select the Optimizations to be linked" on page J-1237

### Cutting table control

A+W Production works as a cutting control station.

> **Parameters of the linked table**
> The cutting table to be controlled by A+W Production is defined during installation. The corresponding parameters are defined at installation. Optimizations are created with the parameters set in A+W Production or A+W Production.

A cutting code is created and transferred to the cutting table, or is made available in a defined directory. Depending on the cutting table and the table control, the cutting table is transferred to the table by a special program, or is loaded from the defined directory by the cutting table software.

*Fig. J-7: A diagram showing input and processing of data in A+W Production. The Realtime Optimizer (handling cutting code creation, re-optimization, and status management) interacts with the Production Database and sends data to the Cutting table.*

Once the cutting code for a stockplate was sent to the cutting table, A+W Production considers this stockplate completed. If transfer of the cutting code is interrupted, work can be resumed at this precise spot.

In connection with XTV, breakage at the cutting table is directly reported to A+W Production. As long as the cutting code for the last stockplate of a glass type (a batch) has not been transferred to the cutting table, breakage can be automatically re-optimized, to be cut with the last stockplate of the batch.

## Cutting

This section tells you how to handle the cutting.
This subject area includes the following training sessions:
- Selecting batches for cutting
- Check optimization and cut
- Interrupt and continue work
- Cutting overview

### Overview

**Objectives**
- Getting to know and understanding the cutting process.

**Benefit**
A+W Production can be used to the best effect only if you are capable of the process.

**Definition**
- **Panorama**: Part of the program that can be configured to control complex machines or more machines (cutting lines).

**Note**
- **Batch number 1000-9999**: Come from a prior system.
- **Batch number from 15000**: Batches starting from number 15000 contain table optimizations created by A+W Production. The number range can be configured.
- **Panorama**: Administration of Panorama is password-protected.

### Selecting batches for cutting

Optimizations exist in the form of batches. Select the batches containing the optimizations you want to cut on the cutting table.

**Selecting batches for cutting**
1.  Open dialog **Select a batch**. Select menu `Cutting > Cutting optimization`.
2.  Select a batch. Select an entry in the **Batch** list. The **Optimisation** list shows the optimizations existing for this batch.
    > **Batch numbers**
    > Batches with the numbers 1000-9999 come from an upstream system and contain one or more optimizations. Batches starting from number 15000 contain table optimizations created by A+W Production.
3.  Select one or all optimizations. If no optimization is tagged, the system assumes that all to be selected. You can configure whether individual optimizations can be selected.
    > **Optimization numbers**
    > Optimizations are defined per lot (per glass type), and numbered consecutively for every batch.
4.  Click [OK]. The tagged optimizations are selected for cutting and shown in dialog **Batch [number -] - batch [number]**.
5.  Close the dialog. Click the [OK] button.
6.  Start the cutting process. Click the [START] button.

**Re-cut already cut batches**
When all plates of an optimization have been cut, the entire batch gets the status **Produced**. This status can be reset to status **Released**, and the entire batch can be cut again.
1.  Open the dialog **Reset cutting batch**. This is done in menu `Optimization > Reset`. The **Reset a cutting batch** dialog shows a list of all batches available for status changes. The list is sorted by batch numbers. Completely cut batches are shown with status **Produced**.
2.  Select the batch you want to reset from status **Produced** to status **Released**. You can tag several jobs, and reset them together.
3.  Click the [OK] button to reset the batch. The batch is now available again for cutting as a complete optimization.

**Skip pattern**
If you choose **Skip pattern** for a lite, no cutting code will be created, and no breakout pattern will be shown for this lite.
1.  Open dialog **Residual plate handling**. Click the button [Options] in dialog **Batch: [No.] - Batch: [No.]** for the batch you want to edit.
2.  Tag in the **Optimizations** list the glass type for which individual stockplates should be cut again. The **Lites** list shows all lites for a batch belonging to the selected glass type. The **Status** column shows the status of each stockplate. You can skip only lites with a status other than **Cut**.
3.  Click the right mouse key on the lite to be skipped during cutting. A context menu appears with the entries **Skip pattern**, and **Do not send cutting code**.
4.  Select **Skip pattern** to stop the system from creating a cutting code and a breakout pattern for this lite.
5.  Close the dialog. Click the [OK] button.

**Suppress cutting code creation**
If you select **Do not send cutting code** for a lite, the system will create no cutting code, but the breakout pattern will be shown in A+W Production Terminal (XTV).
1.  Open dialog **Residual plate handling**. Click the button [Options] in dialog **Batch: [No.] - Batch: [No.]** for the batch you want to edit.
2.  Tag in the **Optimizations** list the glass type for which individual stockplates should be cut again. The **Lites** list shows all lites for a batch belonging to the selected glass type. The **Status** column shows the status of each stockplate. You can send no cutting code only for lites with a status other than **Cut**.
3.  Click the right mouse key on the lite to be skipped during cutting. A context menu appears with the entries **Skip pattern**, and **Do not send cutting code**.
4.  Select **Do not send cutting code** to stop the system from creating a cutting code for this lite, but show the breakout pattern in A+W Production Terminal (XTV).
5.  Close the dialog. Click the [OK] button.

> **Additional Information**
> - Software Reference, "Batch: Number" on page J-1233
> - Software Reference, "Select a batch" on page J-1226

### Check optimization and cut

Once you have selected optimizations for cutting, you can run some checks, then transfer the optimizations to the cutting table.

This chapter describes the following steps:
- Show scheduled cutting sequence.
- Check residual plates.
- Define start of cutting and start cutting.

The following descriptions are based on the assumption that you have completed the previous step **Selecting batches for cutting** and that the **Batch [Number] - Batch [Number]** dialog is displayed.

**Show scheduled cutting sequence**
1.  Click the button [Sequence]. Dialog **Cutting sequence** appears.
    > **Sequence in case of several batches**
    > If several batches have been selected for cutting, the stockplates will be sorted acc. to the configuration of A+W Production. All residual plates can be cut at the end of the batch for example, or at the end of a glass type. A+W Production can be configured to cut stockplates alternately (e.g. coated - uncoated).
2.  Click [OK] to close the dialog.

**Check residual plates**
1.  Click the button [Residual plates]. Dialog **Residual plate handling** appears.
2.  Check the displayed values.
3.  Amend the status of individual plates, or the settings for reject handling if necessary.
4.  If the PlanEdit module is installed on your workstation, you can view the cutting pattern for the selected stockplate by using the button **Process pattern**.
5.  Click [OK] to close the dialog.

**Define start of cutting and start cutting**
1.  In the **Optimizations** list, tag the lot from where cutting should start.
2.  From the **Pattern** list, select the stockplate from where cutting should start.
3.  Click the [START] button.
    The system creates the cutting code for the optimizations displayed, and transfers it to the connected cutting table.
    Wording and function of the button changes into [STOP].
    If A+W Production works with A+W Production Terminal (XTV), the A+W Production Terminal (XTV) breakout pattern can be controlled by the keys [Stop] and [<<].

> **Additional Information**
> - Software Reference, "Batch: Number" on page J-1233
> - Software Reference, "Batch [number] - batch [number]" on page J-1230

### Interrupt and continue work

An optimization that cuts the stockplates in succession can be interrupted due to technical interferences or the end of a shift. A+W Production marks the point at which the work was interrupted and allows you to go on from there.

The following steps are described below:
- Interrupt cutting during an optimization.
- Continue cutting after an interruption.

**Interrupt cutting during an optimization**
1.  You are in dialog **Cutting overview**.
2.  Click the [STOP] button.
3.  Close the dialog.

**Continue cutting after an interruption**
A+W Production remembers optimizations that have not been cut completely.
1.  Select menu `Cutting > Cut optimization` to select an optimization for cutting. A security query appears. The system shows the incomplete batch and asks whether this should be completed.
2.  To view the interrupted batch, select [Yes]. A+W Production shows the interrupted batch in dialog **Batch [number] - batch [number]**. If you answer the security query with **No**, the interrupted optimization will be set to **Started**. Already transferred cutting patterns remain on status **Cut**. The **Select a batch** dialog appears.
3.  To continue the interrupted cutting, click [Start]. The cutting code of the already cut lites is not transferred to the cutting table again.

### Cutting overview

The cutting overview shows the glass to be cut next.

*Fig. J-8: Screenshot of the cutting overview dialog, broken down into A (Menu), B (Plate view), and C (Lite view).*

- To show or hide the menu (A) on the left side of the dialog press the respective icon.
- It is also possible to expand and reduce the individual entries (Cutting, Panorama, Administration).
- The view can be configured via the options in entry cutting.

*Fig. J-9: A popup menu showing display options for the Plate view, including No., Batch, Lot, Pattern, Glass, etc.*

- The plate view (B) can be configured per table. The combo box serves to control which fields should be displayed.
- To reflect the plate picture, enable the requested axis in the **Plate picture** section.

*Fig. J-10: A popup menu showing display options for the Lite view, including No., Batch, Rack - Slot, Order No., etc.*

- The same applies to lite picture (C). Here you can also show or hide the requested display options.
- The point **Shape** in entry **Panorama** visualizes the shape saved for machine control in A+W Production.
- The section **Administration** is password-protected. Here you make general settings.
- Click the [Start] icon to start the cutting. Press the [Stop] icon to stop the cutting.
- Via the context menu, you can set stop codes for particular elements and reset them again. Mark the appropriate element and open the context menu. Then select the **Stop** entry.

*Fig. J-11: A context menu with a "Stop" option checked.*

- You can cancel the stop code by deactivating the **Stop** entry again.
> **Stop code**
> Stop codes that are set on the cutting dialog are not saved in the Ope2Out exchange file. This means that they are not saved if the cutting dialog is closed and that they are not visible on the Options before cutting dialog.

### Reset cutting status

If a batch or individual stockplates has already reached the status **Cut** but should be cut again, the production status can be reset, and cutting can be repeated.

The production status can be reset with the following steps:
- Re-cut already cut lites.
- Re-cut already cut batches.

If the whole optimization was reset, but only individual stockplates should be cut again, you can exclude parts of the optimization from being cut again by:
- Skip pattern.
- Suppress cutting code creation.

**Re-cut already cut lites**
Individual lites or whole batches can be cut again as long as A+W Production can still access the batches. Cutting of the corresponding batch has to be selected and displayed in the **Batch: [No.] - Batch: [No.]** dialog.
1.  Open dialog **Residual plate handling**. Click the button [Residual plates] in dialog **Batch: [No.] - Batch: [No.]** for the corresponding batch.
2.  Tag in the **Optimizations** list the glass type for which a stockplate should be cut again. The **Lites** list shows all lites for a batch belonging to the selected glass type. The **Status** column shows the status of each stockplate.
    - Software Reference, "Batch: Number" on page J-1233
3.  Click the right mouse key on the lites you want to reset from status **Cut** to be cut again. A context menu appears showing the entry **Cut**.
4.  Select **Cut** to reset the lite.

> **Additional Information**
> - Software Reference, "Batch: Number" on page J-1233

## Interplay with Other Modules

**Objectives**
- Getting to know and understanding the work with A+W Residual Stock Manager.
- Getting to know and understanding the work with A+W Pattern Viewer.
- Getting to know and understanding the work with A+W PlanEditor.
- Getting to know and understanding the work with A+W Continuous Cutting.
- Getting to know and understanding the work with A+W Defect Optimizer.

**Benefit**
The performance of A+W Production can be increased by adapting other modules.

**Definitions**
- **A+W Residual Stock Manager**: The residual stock storage manages residual plates at the cutting table.
- **A+W Pattern Viewer**: Offers a breakout display at the cutting table.
- **A+W PlanEditor**: Shows the data of patterns to be cut, tabulated and graphically.
- **A+W Continuous Cutting**: Controls from the office what is cut so that the operators know automatically what they have to do.
- **A+W Defect Optimizer**: The intelligent defect optimization
- **A+W DynOpt Compact**: A+W entry level solution for dynamic optimization

**Note**
- **Configuration**: A+W Production can be configured to work with different modules.

### Overview

A+W Production can be configured to work with different modules. For information on linking with different basic systems please refer to the previous chapter.

If A+W Production was configured accordingly, it can work with the following modules:
- A+W Residual Stock Manager
- A+W Pattern Viewer
- A+W PlanEditor
- A+W Continuous Cutting
- A+W Defect Optimizer
- A+W DynOpt Compact

### A+W Residual Stock Manager

This module is a residual stock storage system in which residual plates are managed on the cutting table. If during cutting there is a residual plate, it is not discarded, but saved temporarily in the A+W Residual Stock Manager. Information on glass type, thickness, and dimensions of the residual plates are entered and saved in a management program (A+W Planning Web). A+W Production can work with the A+W Planning Web. Here, data about the residual plates is exchanged. Residual plates can then be integrated by A+W Production into table optimizations. If an optimization is cut, the residual plate can be replaced by a plate from the residual stock (without re-optimization).

As soon as a residual plate is planned into an optimization, A+W Production informs the A+W Planning Web about this status. The residual plate can then no longer be used for other cuts.

If a table is controlled with a cutting code that was optimized for a residual plate, the cutting code controls the residual plate storage, and the required residual plate is put onto the table for cutting.

#### A+W Planning Web

You undertake the configuration for the A+W Residual Stock manual in this module.

> **A+W Planning Web Configuration**
> The default configuration is done by A+W employees during installation. We explain in this documentation how you create Warehouse, Storage locations, and Racks in A+W Planning Web.

#### Interface

If you have started A+W Planning Web, the following view appears:

*Fig. J-12: The A+W Planning Web interface, showing options for "Capacity View" and "Warehouse".*

Then select the **Warehouse** entry. You are in the **Orders** area.

*Fig. J-13: The Orders area in A+W Planning Web.*

#### Master data

This is where the settings for the master data are located. These include:
- Warehouse
- Storage locations
- Racks
- Groups

**Warehouse**
You can display the corresponding content with the Warehouse icons.

*Fig. J-14: The Master Data area for Warehouses, showing a list of existing warehouses.*

All warehouses created for your company are displayed in this area. There are the following options:
- Change the name of an existing stock
- Add a new stock
- Delete an existing stock

**Here's how to change the name of an existing stock**
1.  Click the mouse in the **Description** field. The field opens for editing.
2.  Change the name and exit the field.
3.  The field now has a small red triangle in the top left corner. The triangle indicates that there are changes that were not yet saved. It is displayed until you click the [Save] button.
4.  Click the [Save] button to save the entries.
5.  The small red triangle is no longer there.

**Here's how to add a new stock**
1.  Click the [Add] button. A new line is inserted at the top of the table.
2.  In the **ID** field, the next possible number is suggested automatically. You can overwrite this number.
3.  In the **Description** field, enter the name for the stock and exit the field.
4.  The field now has a small red triangle in the top left corner, indicating unsaved changes.
5.  Click the [Save] button to save the details.
6.  The small red triangle is no longer there.

**Here's how to delete a stock**
1.  Click the line with the stock in question.
2.  Click the [Delete] button.
3.  The stock is deleted. Caution: there is no security query.

> **Additional information**
> - Software Reference, "Stock" on page J-1255

**Storage locations**
Storage locations are spaces or areas where lites can be stored. To add more storage locations to a warehouse, change or delete existing storage locations, click the [Edit] button on the entry for the warehouse in question. Then you will see all storage locations that are created for the warehouse.

*Fig. J-15: The Storage Location information area.*

There are the following options:
- Add a new storage location
- Delete an existing storage location
- Make changes to an existing storage location

**Here's how to add a new storage location**
1.  Click the [Add] button. A new line is inserted at the top of the table.
2.  In the **ID** field, the next possible number is suggested automatically. You can overwrite this number.
3.  In the **Description** field, enter the name for the storage location.
4.  Select the corresponding type from the **Warehouse type** combo box (storage location/stock receipt).
5.  Select the appropriate status from the **Allocation status** combo box.
6.  Click the [Save] button to save the details.

**Here's how to delete a storage location**
1.  Click the line with the storage location in question.
2.  Click the [Delete] button.
3.  The storage location is deleted. Caution: there is no security query.

**Here's how to make changes to a storage location**
1.  Click the field with the entry in question.
2.  Overwrite the entry or select the desired entry from the combo box.
3.  Click the [Save] button to save the details.

> **Additional Information**
> - Software Reference, "Rack information" on page J-1257

**Racks**
The racks created for a storage location are displayed in this area.

*Fig. J-16: The Master data area for Racks.*

There are the following options:
- Add a new rack
- Delete an existing rack
- Make changes to an existing rack

**Here's how to add a new rack**
1.  Click the [Add] button. A new line is inserted at the top of the table.
2.  In the **ID** field, the next possible number is suggested automatically. You can overwrite this number.
3.  In the **Description** field, assign a unique name to identify a rack type.
4.  Select the appropriate status from the **Allocation status** combo box.
    - Realtime Optimizer: Software Reference, "Allocation status" on page J-1259
5.  Select the appropriate type from the **Property** combo box.
6.  Click the [Save] button to save the details.

**Here's how to delete an existing rack**
1.  Click the line with the rack in question.
2.  Click the [Delete] button.
3.  The rack is deleted. Caution: there is no security query.

**Here's how to make changes to a rack**
1.  Click the field with the entry in question.
2.  Overwrite the entry or select the desired entry from the combo box.
3.  Click the [Save] button to save the details.

> **Additional Information**
> - Software Reference, "Racks" on page J-1259

**Rack properties**
In this area, the properties of the various rack types are displayed. The rack type should be understood as the property here (A-rack, L-rack, harp rack, etc.).

*Fig. J-17: The Master data area for Rack properties.*

There are the following options:
- Add a new rack property
- Delete an existing rack property
- Make changes to an existing rack property

**Here's how to add a new rack property**
1.  Click the [Add] button. A new line is inserted at the top of the table.
2.  In the **Description** field, assign a unique name to identify the rack type.
3.  In the **Access Behavior** field, select the appropriate type from the combo box.
    - Realtime Optimizer: Software Reference, "Access type" on page J-1261
4.  Select the corresponding type from the **Warehouse type** combo box (storage location/stock receipt).
5.  Select the appropriate status from the **Allocation status** combo box.
6.  Click the [Save] button to save the details.

**Here's how to delete an existing rack property**
1.  Click the line with the corresponding property.
2.  Click the [Delete] button.
3.  The rack property is deleted. Caution: there is no security query.

**Here's how to make changes to a rack property**
1.  Click the field with the entry in question.
2.  Overwrite the entry or select the desired entry from the combo box.
3.  Click the [Save] button to save the details.

> **Additional Information**
> - Software Reference, "Rack properties" on page J-1261

**Overview of Stored Residual Plates**
All residual plates that were stored are displayed in this area.

*Fig. J-18: An overview screen showing stored residual plates with details like Glass Type, Location, Dimensions, and Status.*

The data can be edited in the view, e.g., the size of the residual plate stored. Using the filter functions that are available to you in the table header of each field, you can restrict the display results.

There are the following options:
- Make changes to a stored residual plate
- Add a new residual plate
- Delete an existing residual plate

**Here's how to make changes to a stored residual plate**
1.  For the entry that you want to change, click the [Edit] button. The **Add/edit** dialog opens.
2.  Make the desired changes.
3.  Click the [Apply] button to save the details.

**Here's how to add a new residual plate**
1.  Click the [Add new data records] button. The **Add/edit** dialog opens.
2.  In the **Warehouse** field, select the appropriate warehouse from the combo box.
3.  In the **Storage location information** field, select the storage location where the residual plate is from the combo box.
4.  In the **Rack** field, select the appropriate rack on which the residual plate is located from the combo box.
5.  In the **Group** field, select the appropriate group from the combo box.
6.  In the **Glass type** field, select the glass type of the residual plate from the combo box.
7.  In the **Width** and **Height** fields, enter the dimensions of the residual plate.
8.  In the **Info** field, you can store additional information about the residual plate.
9.  In the **Allocation status** field, select the appropriate status from the combo box.
    - Software Reference, "Allocation status" on page J-1264
10. In the **Date** field, enter when the residual plate was stored.
11. Click the [Apply] button to save the details.

**Here's how to delete a stored residual plate**
1.  Click the line with the corresponding property.
2.  Click the [Delete] button.
3.  The stored residual plate is deleted. Caution: there is no security query.

> **Plates from the residual plate storage and residual plates cannot be used at the same time!**
> If you want to use plates from the residual plate storage for optimization, a previously entered residual plate will be ignored. A+W Production displays a message to that effect.

**Use residual storage plates for optimization**
1.  Select **Residual storage plates** on the **Table optimization** dialog. The list on the right shows all plates that exist in the A+W Residual Stock Manager for the glass type and thickness that exist and are available to the cutting table.
2.  Tag the residual stockplate A+W Production should use for cutting optimization. Up to ten residual stockplates can be integrated in an optimization.
3.  To create the optimization, go to tab **Optimize** and click [Optimize]. The residual stockplate is now reserved for this batch in the program that manages the residual stockplates; they cannot be used by another batch now.
4.  To save the optimization, click [Save].

> **Additional information**
> - Software Reference, "Residue plates and stockplates" on page J-1212

**Printing labels**
Printing of the appropriate labels is also possible from the overview. To do this, click the [Print] button on the entry.

> **Printing labels**
> To print labels, the appropriate printer must be set up.

### A+W Pattern Viewer

The A+W Pattern Viewer provides a breakout display at the cutting table, which, depending on the configuration, can be used to enter breakage. A+W Production provides the information to the A+W Pattern Viewer, once the cutting code for the connected table has been created. The A+W Pattern Viewer can then show the breakout pattern for this optimization. The display matches the stockplate or residual plate to be cut and provides all essential information on the optimization, the article, and the individual lites. If A+W Pattern Viewer is used to enter breakage, the module provides appropriate information to A+W Production.

#### Settings

You can reach the Settings via the A+W logo:

*Fig. J-19: The Settings Menu showing Language, Register Application, Breakage Reasons, and About.*

- **Language**: This entry includes all languages in which the module is available. The language can be switched at runtime.
- **Register Application** and **Breakage Reasons**: These are required by A+W employees to configure the module at your company according to your requirements.
- **About**: This area displays the version number of the module.
- You can return to the breakout display with the **Back** button.

*Fig. J-20: The back button to return to the breakout display.*

#### The interface

*Fig. J-21: The main breakout display of the A+W Pattern Viewer, showing a cutting pattern with individual lites.*

**The menu bar**
The menu bar in the A+W Pattern Viewer includes the entries: View and Size.

*Fig. J-22: The complete menu bar, with sections for Breakout pattern, Zoom, Input Type, Configure View, Tool Tip, Validation buttons, and Colors.*

The menu bar is divided into individual sections:
- Breakout pattern
- Zoom
- Input type
- Configure view
- Tool tip
- Validation buttons
- Colors

*Fig. J-23: The information area below the menu bar, showing Batch, Lot, Pattern number, Glass Type, Dimensions, and Yield.*

The batch, lot, and pattern number are displayed all the way to the left. In the example above, this means:
- Batch number: 2689
- Lot number: 3
- Pattern number: 3

Next, you see the number of the current pattern and the total number of patterns. In the example above, pattern number 3 of a total of 5. Then the glass type is displayed. In the example above, Star S 4 mm 4.00. Then comes the width x height of the stockplate used. The optimization result for the current pattern is displayed all the way to the right.

**Breakout pattern**
In this area, you can select the type of display by clicking on the appropriate button. There are two possibilities:
- Breakout pattern
- JSON

You will use the **Breakout Pattern** setting for your daily work. If there are problems, you can change to the **JSON** setting, copy the content via the context menu and then make this available to an A+W employee for a detailed analysis.

**Zoom**
This area includes settings for the size of the breakout pattern and the information area directly below the menu bar.

*Fig. J-24: The zoom dropdown for the breakout pattern.*

The combo box includes the values 0 to 4.

*Fig. J-25: A diagram illustrating different cut types (1, 2, 3, 4).*

- **0**: The complete breakout pattern for a lite is displayed.
  *Fig. J-26: Example of a complete breakout pattern.*
- **1**: The individual X-cuts are displayed. An X-cut (normally the cross cut) runs parallel to the left or right edge of the light (cut) or vertically to the lower lite edge. This cut divides the stockplate into parts or subplates. You can use the right and left arrow keys to switch the individual cross cuts back and forth.
  *Fig. J-27: Example of a breakout pattern showing subplates after an X-cut.*
- **2**: The individual Y-cuts are displayed (from bottom to top). A Y-cut runs parallel to the upper or lower edge of the lite (cut). This cut divides a subplate into upper and lower sections. You can use the right and left arrow keys to switch the individual cuts back and forth.
  *Fig. J-28: Example of a breakout pattern showing a Y-cut.*
- **3**: The individual Z-cuts are displayed (from left to right). A Z-cut runs parallel to a left or right lite edge (cut) and/or an X-cut. It divides the sections formed by Y-cuts. You can use the right and left arrow keys to switch the individual cuts back and forth.
  *Fig. J-29: Example of a breakout pattern showing a Z-cut.*
- **4**: The individual W-cuts are displayed (from bottom to top). A W-cut runs parallel to a Y-cut and lies between an X-cut (or the left or right edge of the lite (cut)), and a Z-cut. You can use the right and left arrow keys to switch the individual cuts back and forth.
  *Fig. J-30: Example of a breakout pattern showing a W-cut.*

**Font size**
You can use the combo box to control in which size the information area is displayed directly below the menu bar. The values **small**, **medium**, and **large** are available.

*Fig. J-31, J-32, J-33: Examples of small, medium, and large font sizes for the information bar.*

**Input type**
This area includes the **Individual lite** entry. Automated operations work in this mode. Each lite is specified individually for processing. The corresponding mode is set for set-up of the A+W Pattern Viewer by A+W employees.

**Configure view**
Various properties are in this area, with help of which you can set the breakout display according to your needs.

- **Coordinates**: Use this button to enable or disable the display of the coordinates.
  *Fig. J-34 & images A/B: Showing coordinates disabled and enabled.*
- **Dimensions**: Use this button to enable or disable the display of the dimensions of the lite.
  *Fig. J-35 & images A/B: Showing dimensions disabled and enabled.*
- **Rack number**: Use this button to enable or disable the display of the rack number.
  *Fig. J-36 & images A/B: Showing rack number disabled and enabled.*
- **Breakout sequence**: Use this button to enable or disable the display of the breakout sequence. The lite with the smallest number is broken first.
  *Fig. J-37 & images A/B: Showing breakout sequence disabled and enabled.*
- **Second glass type or batch number**: Use this button to enable or disable the display of the second glass type or batch number.
  *Fig. J-38 & images A/B: Showing batch number disabled and enabled.*
- **Barcode**: Use this button to enable or disable the display of the barcode.
  *Fig. J-39 & images A/B: Showing barcode disabled and enabled.*
- **Additional text**: Use this button to enable or disable the display of additional text in the header and footer area. Background colors change to indicate if text is present.
  *Fig. J-40 & images A/B: Showing header/footer areas with and without additional text.*
- **Rotate subplate**: With this button, it is possible to rotate subplates automatically by 90° if the size ratio of the subplate fits better on the screen in order to create a large display.
  *Fig. J-41 & images A/B: Showing a subplate not rotated and rotated.*
- **Stack number**: The stack number is always displayed if the rack number is also displayed. The display can be varied (e.g., Stack 2, /2).
  *Fig. J-42: Example of a stack number display.*

**Tool tip**
In this area, there is a combo box you can use to set the display duration for a tool tip. You can select from one to eight seconds.
*Fig. J-43: Dropdown for tool tip display duration.*

**Validation buttons**
In this area, there are buttons you can use to change the working direction (Normal/Invert). Normally, you start breaking on the left side and use the right arrow to advance. If the lite is positioned to be broken from the right, activate the [Invert] function to use the right arrow correctly.
*Fig. A/B: Normal and Invert buttons.*

**Colors**
In this area, you will find the colors that you can use for the background. The currently set background color is displayed under the letter A.
*Fig. J-44: Color selection for the background.*

#### Information about lite and waste

If you place the mouse on a lite or on an empty area, you will see the corresponding information.
- *Fig. J-45 A*: Lite information pop-up (Sheet) with details like Rack, Sequence, Width, Height, Order no., Shape, Label, Coating.
- *Fig. J-45 B*: Waste information pop-up (Waste) with Height and Width.

> **Information**
> The information displayed depends on the customer and the configuration. It will be set up accordingly by A+W employees during installation. If you want to make changes to your configuration (e.g., the customer's name should be displayed), please contact an A+W employee.

#### Display linked batches

The blue triangle at the upper edge in the A+W Pattern Viewer indicates where the linked batch begins.
*Fig. J-46: A screenshot showing the beginning of a linked batch, indicated by a blue triangle.*

#### Display setting edge

If for a free shape a marking for the setting edge was stored in the SN file (e.g., in the order entry with iTOE), this edge is indicated in the A+W Pattern Viewer with a yellow arrow.
*Fig. J-47: A screenshot showing the setting edge for free shapes, indicated by a yellow arrow.*

> **Display setting edge**
> By adding the activity `HideStandingEdge`, the display of the setting edge (triangle) is removed for all lites.

#### Display symbol for processings, stamp, logo or reference mark

The A+W Pattern Viewer also provides the ability to display an image instead of a stamp or a logo.
> **Symbols**
> The symbols depend on the customer and configuration. They will be set up accordingly by A+W employees during installation. If you want to make changes to your configuration (e.g., display a logo or stamp), please contact an A+W employee.

#### Color selection for order items

The A+W Pattern Viewer also offers the opportunity to color glass in a user-defined color. There are various colors available for selection.
> **Colors**
> The selection of colors is based on the desires of the individual customer. They will be set up accordingly by A+W employees during installation.

#### Mark the first and last lite

The A+W Pattern Viewer offers the opportunity to mark the first and last lites in a storage location accordingly.
> **Marking the first and last lite**
> Whether the first and last lites in a storage location are marked is based on the desires of the individual customer. This will be set up accordingly by A+W employees during installation.

#### Size

If you click **Measurements**, the **Unit System** area opens:
*Fig. J-48: The Measurements menu with options for Unit System (Metric/Imperial) and Decimal Places/Precision.*

In the **Unit System** entry, you can select between:
- Metric
- Imperial

The combo box below depends on the selection of the unit system. If you have selected **Metric**, you can use the **Decimal Places** combo box to decide how many decimal places (up to three) should be displayed. If you have selected **Imperial**, you can use the **Precision** combo box to select this (1/16, 1/32, 1/64, 1/128, 1/256).

#### Rejects

In the A+W Pattern Viewer you can mark lites as broken by marking the appropriate lite on the breakage display. There is a selection with all breakage reasons created. Select the appropriate breakage reason. The selection is closed and the selected lite marked accordingly.

### A+W PlanEditor

The A+W PlanEditor shows the data of patterns to be cut, as a table and graphically. The results show the statistical evaluation of the existing patterns. You get a quick overview of the lites to be produced, stock dimensions, residual plates, waste, etc.

Depending on the configuration, the graphics editor shows the patterns to be cut, and offers various ways of processing. You can create and change patterns, add lites, save and print the pattern.

If the A+W PlanEditor is installed on your workstation, you can start the A+W PlanEditor by double-clicking on an optimized plate after creating a table optimization. It then shows the cutting pattern for this plate. Changes that you make to such a pattern with the A+W Plan Editor are taken over into A+W Production.

> **Additional Information**
> For more information on A+W PlanEditor please refer to the appropriate documentation.

### A+W Continuous Cutting

If the A+W Production on the cutting table is running in **Continuous Cutting** mode, an overview of the batches planned for this table is displayed before the start of cutting. Here it is possible to reset a batch if necessary. If you continue cutting, the first group in the cutting is loaded and cutting is started. If there is a rush group, it is loaded first and the subsequent group is attached. When the last batch of the current group has almost been cut, the next group is loaded into cutting automatically. This way, all planned batches are gradually processed automatically according to the settings made in planning.

#### Overview of the planned batches

In the planning view in AWP, all batches optimized and released for cutting are displayed with their properties. Here, you can now select which batches should be cut on the cutting table for which they were optimized. Here, the sequence can be specified and various settings made. For batches already planned, it is possible to make changes, assuming that the cutting has not yet begun.

If you click `Cutting > Continuous Cutting ...` in the A+W Production, a list appears with the released batches:

*Fig. J-49: A screenshot of the Released Lots dialog.*

With the **Cutting Tables** combo box, you can restrict the display if necessary. Click the [Planning F5] button at the lower right to open the planning view:

*Fig. J-50: A screenshot of the main Planning view.*

**Description of fields**

**Filters**
For a better overview, filters can be applied in order to filter the batches displayed by glass types, for example. The corresponding settings are in `AWP > Configuration > Parameters > A+W Production > Continuous Cutting > AUW_CONTINUOUS_CUTTING > Filters`.

*Fig. J-51: Parameter Administrator window showing filter settings.*

To create a new filter or make changes to an existing filter, please click the three dots. A dialog opens:

*Fig. J-52: Dialog for creating or changing a filter.*

To make changes to an existing filter, mark the filter in question and click the [Edit] button. To create a new filter, click the [New] button. The **Create/edit Filter** dialog opens.

*Fig. J-53: Dialog for editing an existing filter.*

Give the filter a meaningful name and make sure the syntax of the filter is correct. You can define a permanent filter, e.g. `pool_teile.glasart = 1004` or a filter with one or two placeholders, e.g. `pool_teile.glasart = [TTV1NUM]`. For filters with placeholders, the user enters the desired value himself later on.

**Production date**
If a time span is specified here, only batches are displayed whose production date is in this time span.

**Re-optimization**
Here the mode for the re-optimization and the quantity of broken lites from which this should be triggered is specified.

**Rush optimization**
Here you specify whether a rush optimization should be executed for the batch if a particular quantity of broken lites has been reached.

**Residual plate management**
Here you specify whether in which mode the residual plate should be linked.

**Editing a residual plate**
Here you specify whether the residual plate can be processed and starting at which length.

**Grouping**
Several batches can be combined into a group. Batches of the same group will be sent together to the cutting table in cutting in A+W Production. If cutting has begun for a group in cutting, no batch in this group may be changed. A batch must be assigned to a group in order to be released for cutting.

**Here's how to create a group for a batch**
1.  Select the appropriate table.
2.  Mark the desired batches.
3.  Click the [Group] button.
4.  Click the [Release] button.
5.  The group is created and attached behind the already-released batches.

**Here's how to move a group for a batch**
The sequence of released lots not yet begun can be changed
1.  Select the appropriate group.
2.  Move the selected group to the desired position with the arrow keys.
3.  Click the [Release] button.
4.  The group is moved to the desired location.

**Here's how to resolve a group**
1.  Mark the desired lots in a group.
2.  Click the [Reset] button.
3.  Click the [Release] button.
4.  The group is resolved.

**Rush groups**
Rush groups include batches that are handled with priority.

**Here's how to create a rush group**
1.  Select the desired batches.
2.  Click the [Rush group] button.
3.  Click the [Release] button. If the rush group is not in the desired position, you can use the arrow keys to move it to the desired position (as long as cutting has not yet begun).

**Resetting batches**
Already planned batches and settings can be reset so that they are not cut automatically.

#### Cutting

On the A+W Production menu, click `Settings > Cutting`. This dialog opens:

*Fig. J-54: Automatic Cutting dialog.*

From the combo box, select **Automatic** and click [OK].
Now open the cutting via the icon on the menu bar.

You will see an overview of the planned cutting.

*Fig. J-55: Planned cutting overview.*

With the [Options] button, you can (if necessary) reset the status of the batches.
Click the [Start] button to start the cutting. The optimizations for the first group are transferred to cutting.

*Fig. J-56: Cutting overview in progress.*

If the last pattern of the group has been sent to the cutting table and cut, the next group will be loaded into cutting automatically.

### A+W Defect Optimizer

... the intelligent defect optimization.

The stockplates are scanned in conjunction with a quality scanner, e.g., from Viprotron, and any faults or defects are detected and displayed. The earlier defects are detected during the process, the lower the incurred costs.

Defects are taken into account during optimization for the restructuring of the sectional image. If there are any orders that are to be considered, then those will of course be taken into account.
Defects in residual plates are also stored, and can thus be reused later without additional inspections.

If defects cannot be avoided through the optimization process (e.g. number and size of stock lites on pattern), the optimization process tries to use smaller and thus cheaper glass panes for the defects.
Glass that is positioned on defects is automatically reported as breakage and is recut.

> **Requirements**
> The production system A+W Production as well as the A+W Realtime Optimizer are prerequisites to use the A+W Defect Optimizers.

> **Additional information**
> For more information on A+W Defect Optimizer please refer to the appropriate documentation.

### A+W DynOpt Compact

A+W DynOpt Compact is the entry level solution of A+W for Dynamic Optimizations.

The system is based on the A+W Realtime Optimizer and loads the batches, pre-optimized and sent by the prior production system A+W Production. These batch are resolved completely and re-optimized systematically and dynamically. This method improves the yield and reduces the number of residual plates to be saved.

You can consider A+W DynOpt Compact to be an automatic A+W Real-time Optimizer.

A+W DynOpt Compact works with the following two modules:
- A+W DynOpt Compact Import
- A+W DynOpt Compact Optimization

#### A+W DynOpt Compact Import

During import, the batches released for A+W DynOpt Compact are converted into so-called Cluster. A cluster is a - initially random - production unit, e.g. a rack, a group of racks, or an individual lite.

#### A+W DynOpt Compact Optimization

After the import, the processing sequence for the clusters is defined considering the available space. This more or less matches the production sequence; in special cases, clusters may be moved up in the sequence to improve the yield. You can use harp racks, A racks, or both.

About half of the computed clusters become primary clusters and the rest, secondary clusters. Primary clusters get priority 1 and are completely optimized in the optimization on hand. Secondary clusters are used as fillers; the optimization itself decides whether or not they are required.

**Example:**
Available space: 6. The space for a harp rack is 1, the space for an A rack 0,5 (in terms of harp racks, i.e. 1 harp rack = 2 A racks).
If there are as many harp racks as there are A racks and the splitting is applied to the clusters, this means: 4 harp racks plus 4 x 0.5 A racks = 6. Half of the numbers each means: two primary and two secondary harp racks and A racks.

| | Imported | Used | Primary | Secondary |
| :--- | :--- | :--- | :--- | :--- |
| **Harp rack** | 16 | 4 | 2 | 2 |
| **A Rack** | 17 | 4 | 2 | 2 |

*Tab. J-1: Example*

The following conditions are kept when calculating the time-line:
- The primary sorting of clusters is the production sequence.
- As long as clusters from the current batch can fill the available space, no clusters of the following batch will be used to create the time-line.
- If the secondary clusters include a glass type that does not appear in the primary clusters, there are two options:
    - If the cluster consists of lites of a glass type for which there are primary lites as well, only those will be optimized. The lites of the glass type that does not appear in the primary clusters, will be optimized when the cluster becomes primary.
    - If the cluster consists only of lites of a glass type that does not appear in the primary clusters, the system searches the present batch for an alternative cluster which consists (at least partly) of lites of a primary glass type. If this can be found, the clusters will be exchanged; otherwise, the present cluster will not be included in the optimization.

Every step of A+W DynOpt Compact provides all primary and all secondary clusters for optimization. The primary lites will always be used for optimization and the secondary only if required. After this step, all primary clusters have been filled and can be replaced by secondary clusters or even new ones.

#### Create A+W DynOpt Compact batch

There are two ways of creating A+W DynOpt Compact batches.
- Creating A+W DynOpt Compact batches in the cluster view.
- Creating a A+W DynOpt Compact batch at cutting.

**Creating A+W DynOpt Compact batches in the cluster view**
1.  Open the dialog **Cluster view**. Select `Cutting > A+W DynOpt Compact`.
2.  On the left side, select the batch(es) you want to use to create an A+W DynOpt Compact batch.
3.  Open the context menu and select **Create A+W DynOpt Compact batch**.
4.  After the A+W DynOpt Compact batches have been created, they are displayed in the top left section of the dialog. They are headed by **+**. If you open up the tree, you can view the rack data for the batches.

**Creating a A+W DynOpt Compact batch at cutting**
1.  Open **Select a batch** dialog. Select either `Cutting > Cut optimization` or use the corresponding icon.
2.  From the batch list, select the batch you want to use to create an A+W DynOpt Compact batch.
3.  Open the context menu and select **Create A+W DynOpt Compact for batch XXXX**.
4.  When the A+W DynOpt Compact batch has been created, it appears in the top left section of the dialog, marked by **Cut&Go**. Tag the batch in the left section to display the appropriate information in section **Optimizations**.

> **Requirements**
> The production system A+W Production as well as the A+W Realtime Optimizer are prerequisites to use the A+W DynOpt Compact.

> **Additional Information**
> For more information on A+W DynOpt Compact please refer to the appropriate documentation.

---

# Software Reference

This section provides information on the following subjects:
- Overview
- Entry
- Optimization
- Cutting
- Settings
- View
- A+W Residual Stock Manager

## Table of Contents

*   **Overview** - J-1186
    *   Menus - J-1186
    *   Icons - J-1187
*   **Entry** - J-1188
    *   Rush order lites - J-1189
    *   Enter rush order lites - J-1191
    *   Shape input - J-1193
    *   Shape number - J-1195
    *   Manual creation of plans - J-1196
    *   Charge editor - J-1199
*   **Optimization** - J-1201
    *   Select glass for optimization - J-1202
        *   Table optimization in the Default variant - J-1202
        *   Table optimization in the Production date variant - J-1205
    *   Local optimization job [no] - J-1207
        *   Overview - J-1207
    *   Optimize - J-1210
    *   Residue plates and stockplates - J-1212
    *   Parameter - J-1216
    *   Number of stockplates - J-1219
    *   Resetting a cutting batch - J-1220
    *   Pausing glass types - J-1222
    *   Currently changed settings - J-1224
*   **Cutting** - J-1225
    *   Select a batch - J-1226
    *   Batch [number] - batch [number] - J-1230
    *   Optimization sequence - J-1232
    *   Batch: Number - J-1233
    *   Select the Optimizations to be linked - J-1237
    *   Optimization result - J-1238
    *   Rejects pool - J-1239
    *   Add rejects - J-1241
    *   Input of shapes - J-1243
    *   A+W DynOpt editor - J-1244
*   **Settings** - J-1248
    *   Settings - J-1249
    *   Table optimization - J-1251
*   **View** - J-1252
    *   Import - J-1253
    *   Error reports - J-1254
*   **A+W Residual Stock Manager** - J-1255
    *   A+W Planning Web - J-1255
    *   Stock - J-1255
    *   Rack information - J-1257
    *   Racks - J-1259
    *   Rack properties - J-1261
    *   Glass overview - J-1263
    *   Add/Edit new data record - J-1266

## Overview

The following chapter describes all dialogs available in A+W Production. Depending on the program version, some dialogs or fields in the dialogs are invisible. The following versions are possible:
- A+W Production integrated into the A+W Production environment.
- A+W Production integrated into A+W Production environment together with a ReMaster dispenser.
- A+W Production stand-alone.

The description of the individual dialogs shows if an information applies only to a certain version.

### Menus

The following menus appear after starting Realtime Optimizer:

*Fig. J-57: A screenshot showing the menu bar of A+W Realtime Optimizer with Exit, Input, Optimization, Cut, View, Help.*

The menus contain functions, sub-menus, and dialogs. The following table describes the functions and lists the sub-menus and dialogs. Description of the dialogs in the following chapters is sorted by menu.

### Icons

Some dialogs can be directly loaded via icons:

| Icon | Dialog/Function |
| :--- | :--- |
| `Rush Order Lite` | Opens the dialog "Rush order lites" on page J-1189 |
| `Optimization` | Opens the dialog "Select glass for optimization" on page J-1202 |
| `Cutting` | Opens the dialog "Select a batch" on page J-1226 |
| `Rejects Pool` | Opens the dialog "Rejects pool" on page J-1239 |
| `Error` | Opens the dialog "Error reports" on page J-1254 |
| `Info` | Opens the dialog with information about the A+W Realtime Optimizer. |

*Tab. J-2: Icons and their function*

## Entry

Open **Input** menu.
The Input menu offers the following options:
- **Rush order lites**: This menu allows you to enter rush order lites directly in Realtime Optimizer.
  - Software Reference, "Enter rush order lites" on page J-1191
- **Manual plan**: This menu allows you to create a purely manual plan and save it as a table optimization in the database.
  - Software Reference, "Manual creation of plans" on page J-1196
- **Master data**: This menu gives you access to the master data. These are described in detail in the AWP manual.

### Rush order lites

`Input > Rush order lites`

*Fig. J-58: The "Rush order lites" dialog.*

Rush order lites can be integrated into local optimizations. This dialog shows all the rush order lites entered. The combo box for the **Table** field allows you to view the rush order lites per table, or for all tables. For details on rush order lites, please refer to section Detailed scheduling.

#### Description of fields

- **Glass type**: Shows the product number of the glass type. The value is adopted from field **Glass type** in dialog **Enter rush order lites**.
- **Thickness**: Shows the thickness of the glass type. The value is adopted from field **Thickness** in dialog **Enter rush order lites**.
- **Rack**: This field shows the rack number. The value is adopted from field **Rack** in dialog **Enter rush order lites**.
- **Quantity**: This field shows the number of rush order lites. The value is taken from field **Quantity** in dialog **Enter rush order lites**.
- **Shape**: If the rush order lite is a shape, this field shows the shape number. 0 stands for "no shape". The value is adopted from field **Shape** in dialog **Enter rush order lites**.
- **Width**: This field shows the width of the rush order lite. The value is taken from field **Width** in dialog **Enter rush order lites**.
- **Height**: Shows the height of the rush order lite. The value is adopted from field **Height** in dialog **Enter rush order lites**.
- **Priority**: Shows the priority of the rush order lite. Default priority is 0.
- **All stations**: This checkbox defines the rush order lites to be displayed. Usually, only those rush order lites will be displayed that were entered at this particular terminal. If activated, all rush order lites in the database are shown. (Technical info: Database field: FEIN_TEILE:STATIONID)
- **Table**: The combo box shows all cutting tables defined. This allows you to allocate rush order lites to a certain cutting table. The **All tables** option shows all rush order lites entered.

#### Description of buttons

- **Add**: Use this button to open the dialog **Enter rush order lites**.
- **Process**: Use this button to open the **Enter rush order lites** dialog for the tagged record.
- **Delete**: This button serves to delete the tagged rush order lite. This produces a security check.

> **Additional information**
> - Tutorial, "Rejects, rush order lites or filler orders" on page J-1118
> - Software Reference, "Shape" on page J-1191
> - Software Reference, "Enter rush order lites" on page J-1191

### Enter rush order lites

`Input > Rush order lites > [Add]`

*Fig. J-59: The "Input of Rush Order Lites" dialog.*

This dialog allows you to enter rush order lites. For details on rush order lites, please refer to section Detailed scheduling.
Technical info: Database table: FEIN_TEILE

#### Description of fields

- **Glass type**: The combo box shows all defined glass products. Select the required glass type from the combo box. (Compulsory field, DB field: POOL_TEILE:GLASART)
- **Thickness**: The combo box shows all thicknesses defined for the selected glass type. Select the required thickness. (Compulsory field, DB field: POOL_TEILE:DICKE)
- **Rack**: Enter the number of the rack onto which the rush order lite will be put. Racks are defined in master data. (Compulsory field, 4 digit, DB field: FEIN_TEILE:BOCK)
- **Quantity**: Enter the number of rush order lites. (Compulsory field, DB field: FEIN_TEILE:MENGE)
- **Shape**: If the rush order lite is a shape, enter the appropriate shape number. When you enter the shape number and leave the field, the **Shape input** dialog appears automatically. (Compulsory field, DB field: POOL_MODELL:MODELL_NR)
- **Width**: Enter the width of the rush order lite. If it is a shape, enter the width of the surrounding rectangle. (Compulsory field, DB field: POOL_MODELL:BREITE)
- **Height**: Enter the height of the rush order lite. If it is a shape, enter the height of the surrounding rectangle. (Compulsory field, DB field: POOL_MODELL:HOEHE)

#### Description of buttons

- **Magnifier**: Use this button to open the **Shape input** dialog.

> **Additional information**
> - Software Reference, "Shape input" on page J-1193
> - Detailed Scheduling: Software Reference, "Racks" on page D-394
> - Tutorial, "Rejects, rush order lites or filler orders" on page J-1118

### Shape input

`Input > Rush order lites > [Add] > [Magnifier]`

*Fig. J-60: The "Input of Shapes" dialog with areas for A) Input required per shape, B) Shape numbers, C) Graphic overview of shapes, D) Shape overview, E) Parameter list, F) Input field.*

This dialog is used to enter standard shapes. The selection is determined by the shape catalog you are using. The required entries for the selected shapes are shown in the top left window (A). Your entries immediately appear in the right window (D); the shape being shown proportionally. The bottom window (E) shows the input parameters.

The values in front of the required input for the selected shape have the following meanings:

| Value | Explanation |
| :--- | :--- |
| **W** | Width of the shape. In case of several widths = W, W1, W2, etc. |
| **H** | Height of the shape. In case of several heights = H, H1, H2, etc. |
| **T** | Trim. In case of several trims = T, T1, T2, etc. |
| **<-->** | Reflection flag. Valid input: 0: Normal 1: Vertically reflected. |
| **@** | Rotation flag. Valid input: 90: rotate by 90°, 180: rotate by 180°, 270: rotate by 270°. |

*Tab. J-3: Description of input values for the selected shape*

### Shape number

`Input > Rush order lites > [Add] > [Magnifier] > [Magnifier]`

*Fig. J-61: The "Shape Number" selection dialog showing a gallery of shapes.*

If you do not know the exact shape number and do not have a printout of the shape catalog at hand, this dialog will give you an overview of the existing shapes. The shape number highlighted with dots. When you have found the shape you are looking for, double-click on it; it will automatically appear as the Field no. on the **Shape input** dialog.

### Manual creation of plans

`Input > Manual plan`

*Fig. J-62: The "Manual Plan Input" dialog.*

This dialog allows you to create a purely manual plan and save it as local optimization in the database. The manual plan can be edited and changed afterwards. This is done with the **PlanEdit** module. For details on this module, please refer to the corresponding documentation. No barcode information will be available for manual plans.

#### Description of fields in section Glass Type

- **Glass type**: This field shows the glass type. The value is loaded from master data.
- **Thickness**: This field shows the thickness of the glass type. The value in this field is adopted from master data.
- **Glass name**: This field shows a description of the glass type. The value is loaded from master data.
- **Left trim**: Left edge of the stockplate (in mm) that cannot be optimized. The input in this field is adopted from the master data.
- **Right trim**: Right edge of the stockplate (in mm) that cannot be optimized. The input in this field is adopted from the master data.
- **Top trim**: Top edge of the stockplate (in mm) that cannot be optimized. The input in this field is adopted from the master data.
- **Bottom trim**: Bottom edge of the stockplate (in mm) that cannot be optimized. The input in this field is adopted from the master data.

#### Description of fields in Plan section

- **Batch**: This field shows the number of the job in which the manual plan will be cut.
- **Locked**: This column defines whether and by which terminal the job has been locked for processing or optimization.
- **Glass type**: Shows the glass type for which the manual plan has been created.
- **Thickness**: Shows the thickness of the glass type on the manual plan.
- **Glass name**: Shows the name of the glass that has been added to the manual plan.
- **Table**: Shows the table on which the manual plan will be cut.
- **Number of lites**: Shows the number of lites contained in the manual plan.
- **Lite surface**: Shows the surface of the lites (in sqm) contained in the manual plan.
- **Stockplates**: Shows the number of stockplates required for the manual plan.
- **Waste**: Shows the waste (in %) this manual plan will produce.
- **Residual plate**: Shows the length of the residual plate that results from the manual plan.

#### Description of fields in section Stockplates

- **Width**: Shows the width of the stockplate in mm or inch (configurable).
- **Height**: Height of the stockplate in mm or inch (configurable).
- **XY?**: This column defines the direction of the cross cut. Valid options:
  - **X**: The cross cut must be vertical to the bottom edge of the plate.
  - **Y**: The cross cut runs parallel with the bottom edge of the lite.
  - **?**: The optimization can choose one of the two directions for the cross cut.
- **Quantity**: Shows the number of stockplates available.

#### Description of fields in section Residual plate

- **Width**: If there is a residual plate with the appropriate combination of glass type/thickness, it can be used. Enter the width of the residual plate in mm.
- **Height**: If there is a residual plate with the appropriate combination of glass type/thickness, it can be used. Enter the height of the residual plate in mm.

#### Description of fields and buttons in the bottom section

- **Unnamed field**: This field shows the number of the job in which the manual plan will be cut.
- **Table**: Shows the table on which the manual plan will be cut.
- **New**: Use this button to start the **PlanEdit** module.
- **Edit**: This button is active when you have added a manual plan. You can use this button to edit the plan.
- **Cutting**: Use this button to start the cutting process.

> **Additional information**
> - Software Reference, "Parameter" on page J-1216

### Charge editor

`Input > Input [F3]`

*Fig. J-63: The "Charge Editor" dialog.*

This dialog allows you to enter a charge number.

#### Description of fields in section Stockplates

- **Glass type**: This field shows the glass type. The value is loaded from master data.
- **Thickness**: This field shows the thickness of this glass type in mm or inch (configurable). The input is loaded from master data.
- **Width**: Shows the width of the stockplate in mm or inch (configurable).
- **Height**: Height of the stockplate in mm or inch (configurable).
- **Charge description**: This field shows the entered charge description.
- **Glass name**: This field shows a description of the glass type.

#### Description of fields in section charge description

- **Checkbox**: Tag the checkbox and the entered charge number will be inherited to the following stockplates of the identical glass type/thickness.
- **Field**: Enter the charge description in this field.

> **Additional information**
> - Software Reference, "Charge editor" on page J-1199

