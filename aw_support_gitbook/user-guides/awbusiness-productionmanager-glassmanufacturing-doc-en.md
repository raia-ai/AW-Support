---
title: "EN_AWBusiness_ProductionManager_2.21"
source: "EN_AWBusiness_ProductionManager_2.21.pdf"
tags: ["A+W Business Pro", "Production Manager", "Software Manual", "Glass Manufacturing", "Window Manufacturing", "Door Manufacturing", "ERP", "Production Planning", "Batch Management", "Optimization"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive user manual for the A+W Production Manager, a module within the A+W Business Pro software suite. It provides a tutorial and software reference for production planning and management in the glass, window, and door manufacturing industries."
long_description: "This is the official user guide for the A+W Production Manager module, an integral part of the A+W Business Pro software designed for the glass, window, and door industries. The manual serves as both a training tutorial and a detailed software reference. It is intended for end-users responsible for preparing and managing production orders. The document is structured into several key parts. The 'Introduction' provides version history and legal notices. The 'Tutorial' section offers a hands-on guide to using the Production Manager, split into a simplified 'Standard Mode' for quick, wizard-driven processes and an 'Expert Mode' for detailed, manual control over every step. Topics covered include order selection, batch creation, detailed scheduling, optimization, managing rejects, and generating output like reports and machine codes. The tutorial also explains the setup and use of 'Master Data' such as racks, criteria, and sorting keys, which are fundamental to the system's logic. The 'Software Reference' section acts as a detailed encyclopedia of every dialog, field, and function within the Production Manager, providing explicit descriptions for both Standard and Expert modes. It systematically breaks down UI elements, offering clarity on their purpose and usage. An 'Index' is included for quick look-ups of specific terms and features."
---

# A+W Production Manager

---
## Introduction

This part of the documentation contains editorial notes.

### Revision Overview

| Section Version/Date | Software version | Description |
| :--- | :--- | :--- |
| 1.00/07-2013 | 5.0 | Original version |
| 2.00/04/2014 | 5.4 | Revision. |
| 2.10/02-2015 | 5.5 | Revision. |
| 2.20/04-2016 | v6 | Rejects added. |
| 2.21/01-2017 | | Product and company names adjusted. |

### Editorial

The editorial provides information on the following topics:
*   Notes on this document
*   Copyrights
*   Trademarks
*   Contact

#### Notes on this document

This document is intended for end users of A+W Business Pro.

The documentation and software described are licenses that must only be used or copied in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of the master data.

#### Copyrights

© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, either electronically, mechanically, or by recording or in any other way, without A+W Software GmbH's prior written approval.

#### Trademarks

All hardware and software names mentioned in this documentation can also be registered trademarks or other property rights of third parties. Third party copyrights must be observed.

#### Contact

**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
Tel: +49 6404 2051 0
Fax: +49 6404 2051 877
Email: Zentrale@a-w.com
Website: http://www.a-w.com

## Tutorial

### Overview

The tutorial for the Production Manager module deals with the basics of the production solution in A+W Business Pro. This tutorial is based on the understanding of the master data and the number manager.

> **The functions depend on the released modules**
> Please note that the individual functions are available only if the corresponding modules and interfaces have been installed and released.
>
> If you detect functions in this description which are not available in your version, please contact A+W Software GmbH.

**Sets of Topics**

This tutorial offers the following sets of topics:
*   Key Notes on the Production Manager
*   Standard Mode
*   Expert Mode

**Required knowledge**

This tutorial is meant for those who prepare orders for production in A+W Business Pro. Participants must be familiar with the master data and number manager concept.

#### Documentation

The following documents are available for the Production Manager module:

*   **Hand-out**: Printing the tutorial documents for training
*   **PDF**: Complete documentation
    *   Tutorial
    *   Software Reference
    *   Index
*   **Online help <F1>**: Context-sensitive dialog help for the A+W Business software references and tutorials on the basic version

#### Tutorial Structure

This tutorial consists of sets of topics with several sessions each. Each session consists of the following elements:

*   **Overview**: Each training session starts with an overview of the major topics:
    *   Objectives: What shall be conveyed?
    *   Benefit: What can this knowledge be used for?
    *   Maxims: Which correlations are to be remembered?
*   **Concepts**: First, the concepts and terms of the corresponding training session will be explained. This is followed by examples and operating instructions.
*   **Exercises**: For some of the sessions, exercises with certain tasks and suggested solutions are available.
*   **Cross-references**: At the end of each training session there is a section with cross references pointing out additional information in the software reference and in other sections. This shall help you to extend your new-found knowledge.

**Reading instructions**

The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any learning units. The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any learning units.

If you are already familiar with a subject you should at least read the summary at the beginning of the session in order to bring the main details to mind.

#### Display Conventions

Certain parts of the sentences are specially marked. The meanings are:

*   **Italics**: mark character strings describing the software elements, e.g. the dialog *Number manager*.
*   **Bold**: marks character strings to be entered via keyboard, e.g.: Enter **0**.
*   **>**: The so-called breadcrumb trail marks shows how to open a dialog, e.g. Production > Production > Transfer to production.
*   **[]**: Square brackets mark the buttons in the dialog, e. g. [OK] to save the data.
*   **< >**: Pointed brackets refer to keys or shortcuts on the keyboard, e. g. <F1> is used to open the online help.

### Key Notes on the Production Manager

The task of the production manager is to support your planning and preparation process for production - from batch creation to printing production papers and creating machine codes.

The procedure is as follows:
Order/Element selection > Batch creation > Rack organization > Optimization > Release

This represents the standard process for the production solution.

The orders are released for internal capacity planning automatically by means of a predefined status or manually through the user. In this process, a table is filled with all necessary data. These data are accessed by the Production Manager.

The process is handled by a single dialog so that the user does not have to switch between different dialogs.

The module can be found in section **Production > Production**.

*Figure 1-2 shows the Production Manager in the A+W Business menu.*

### The User Interface

Production Manager can be operated in two different ways:
*   Standard Mode
*   Expert Mode

#### Standard Mode

In this mode, the program can be operated by means of a simplified user prompt, the so-called Wizard.
The Wizard permits to finish the whole process (batch creation, optimizations, etc.) with just a few entries. The optimization results are displayed at the end of this process and you can decide whether you are going to accept the batch and the optimization results.

The standard mode is enabled by pressing the corresponding icon.

#### Expert Mode

In this mode, the user performs the individual steps (job creation, optimizations, etc.) manually. The user can influence the individual batch creation and processing steps in detail and quite specifically.

The expert mode is enabled by pressing the corresponding icon.

### Standard Mode

This subject area shows you how to use Production Manager in standard mode.
This includes the following training sessions:
*   "Starting the Standard Mode"
*   "Batch Creation"
*   "Detailed Scheduling of a Batch"
*   "Output"
*   "Results"
*   "Stockplates and Optimization Parameters"

#### Overview

**Objectives**
*   Becoming acquainted with and understanding the standard mode (Wizard)

**Benefit**
*   Using the Wizard you can complete the whole process with just a few mouse clicks. This saves time and minimises the risk of errors.

**Note**

| Term | Description |
| :--- | :--- |
| **Standard mode** | The production manager always opens in standard mode. |
| **Rack Organization** | Is preset by the standard organization defined in master data. Another organization can be selected if required. |
| **Rack depth** | By changing this entry you can influence the optimization result. |
| **Variant** | The tried variants will be kept. This way you can choose the best variant. |

#### Starting the Standard Mode

When the Production Manager is started, it will open in standard mode. You can switch from expert mode to standard mode by pressing the corresponding icon. In this mode, the program appears as follows:

*Figure 1-3 shows the main dialog in standard mode, which includes sections for Batch Creation, Detailed Scheduling and Optimization, Output, Optimizations, Total Result, and tabs for Stock Plates and Optimization Parameters.*

In standard mode, the program can be operated by means of simplified user prompts (Wizard). The Wizard permits to start the whole process (batch creation, optimization, etc.) with just a few entries. The optimization results are displayed at the end of this process and you can decide whether you are going to accept (save) the batch and the optimization results or repeat the optimization with other settings to achieve a better result.

#### Batch Creation

As a first step, select the number manager (NM). All orders included in this NM will be compiled in a batch. The number manager compiles the orders which are going to be processed by the Production Manager in the same batch.

*Figure 1-4 shows the Batch Creation section with fields for Number Manager, Batch Number, Status, Description, and Batch Content (IG, LAMI, TG, Glass).*

The batch number is automatically assigned by the system and cannot be changed. Field *Status* shows the status of the batch. In the above example, the status is *Scheduled in detail*, i.e. detailed scheduling has been completed for this batch. Field *Description* shows the name of the number manager, the user, and the batch creation date.

Section *Batch content* will be filled in only after the batch has been created. You can see the number of IG units, laminated, toughened, and processed lites included in the batch.

#### Detailed Scheduling of a Batch

In the second step, the settings for detailed scheduling and optimization are made. This is done by selecting a predefined rack organization from a combo box. You can also define the depth of the rack.

Rack organizations and the rack depth are managed in master data (Master data > Production > Rack organisa-tion).

*Figure 1-5 shows the Detailed scheduling and Optimization section with fields for Rack Organization, Rack Depth Factor, Unlimited Rack Depth, and N° of Variants.*

If a *Range* is set for the rack depth (e.g. 80-120%), field *No. of variants* defines the number of variants which are created by clicking on the icon [Start]. Example:
*   Rack depth: 80 - 120 %
*   No. of variants: 5
*   Detailed scheduling with a rack depth of 80, 90, 100, 110, and 120%.

#### Output

This is where all output types are set, no matter if the output is to be on paper or as a file. The combo box offers the following selection:
*   **None**: There will be no output.
*   **All**: The following media will be issued:
    *   Production lists for the batch
    *   Labels for the batch
    *   Machine control for the batch
    *   Standard lists for optimization (spacer bender, IG line)
    *   Cutting plans for optimization
    *   Cutting labels for optimization
    *   Machine control for optimization (cutting table)
*   **Selection**: This is where the media listed under the item *All* can be enabled.

*Figure 1-6 shows the Output selection dropdown and the selectable list of reports and machine controls.*

#### Results

The *Optimizations* section shows the optimization results. The table will provide data only after the batch has been created and detailed scheduling and optimization are completed. You can choose in which sequence the glass types shall be optimized or set individual glass types to manual cutting.

*Figure 1-7 shows the Optimizations section, a table with columns for Glass Type, Cutting Table, Batches, Quantity, Area, and Result.*

When you press the [Start] icon, the suggested batch will be roughly scheduled before being scheduled in detail. After that, the individual lites will be optimized in the sequence displayed.

When all optimizations have been completed you can use the icon [Save] to save them. The created batches and optimizations will be saved in the database.

> **Output is initiated**
> When you press the [Save] icon, all active output will be initiated including the transfer of data to the appropriate machines.

**Description of the fields in section Overall Result**

Section *Overall result* shows the different optimization variants. By modifying the settings (e.g. rack depth or the glass type to be optimized first) you can create different optimization results (different variants). As a next step, you can choose the best of these variants and save it. This way, the output (papers and machinery codes) will only be created for the selected variant. This table will provide data only after the batch has been created and detailed scheduling and optimization are completed.

*Figure 1-8 shows the Overall result table with columns for Variant, Rack Organization, Factor for Rack Depth, etc.*

*   **Field Variant** shows how many detailed scheduling and optimization cycles you have gone through. Every click on the [Start] icon creates another variant which appears in this column. The individual variants will be kept so that you can eventually choose the best variant.
*   **Field Rack organization** shows the rack organization which has been used. This is the rack organization you have selected in section *Detailed scheduling and optimization* (the entry is loaded from master data: Production > Rack organization).
*   **Field Factor** is the factor for the rack depth you have set in section *Detailed scheduling*.
*   If the lites are put onto harp racks, **field Harp racks** shows the number of harp racks which are necessary to put away the lites of the batch. If the lites are loaded onto A racks, **field No. of A racks** shows the number of A racks required.
*   **Field Result** shows the overall result for this variant in % while **field Waste** shows the total waste for this variant in Euros.

*Figure 1-9 shows an example of the Optimization per Variant section.*

*   **Field Optimization** shows the respective optimizations per variant.
*   **Field Glass type** shows the glass types included in the batch. The number in front of that shows the optimization sequence. The next column shows the cutting table on which the glass is cut, followed by the batch number. **Field Quantity** shows the quantity per glass type; the next field shows the surface in square metres.
*   **Field Result** shows the optimization result for the glass type in question. The first figure is the result in %. The following brackets show the number of patterns and the number of stockplates the optimization will need, plus the length of the residue plate. If the Production Manager automatically sets one of the glass types to *Manual cutting*, this is due to the fact that the minimum surface defined for optimization in master data has not been reached.
*   The last column shows the **waste in Euros**.

#### Stockplates and Optimization Parameters

There are two more tabs at the right side of the screen which can be expanded if required:
*   Tab Stockplates
*   Tab Optimization parameters

> **Tab Stockplates and Optimization Parameters**
> When detailed scheduling and optimization of a batch have been completed, the tabs *Stockplates* and *Optimization Parameters* are filled.

You can open the tab **Stockplates** by clicking on it.
*Figure 1-10 shows the Stockplates tab for a specific glass type and cutting table.*
This tab provides all information on the stockplates for the corresponding glass type. The displayed values are managed in the *Stock* module.

You can open the tab **Optimization parameters** by clicking on it.
*Figure 1-11 shows the Optimization parameters tab with sections for Global Settings, Cutting Distances, Trims, etc.*
This tab provides all information on the optimization of the corresponding glass type. The values displayed are loaded from master data (Articles > Articles).

Section **General settings** offers a selection of the following optimization modes:
*   **XOPT**: This optimization variant is random, i.e. the sequence of the lites after optimization does not matter and the lites of an item do not have to be kept together. This will result in quite a good yield but all lites on the racks have to be rearranged prior to IG production.
*   **XOPT-S**: This is the standard mode for IG production. The sequence of lites on the racks defined by the rack organization will be kept. Synchronous optimization of the lites is possible to make sure that lite and counter-pane can be matched on the IG line. The lites of an order item are always loaded together on the same A rack after optimization, i.e. the item will not be split.

#### Information

This section serves to search an order by its number. Thus, open menu *Information* and the entry *Search order*. Enter the order number, the corresponding data are displayed.

**How to find the orders**
1.  Open the entry *Information* in the menu.
2.  Press the [Order] button. *Search order* opens.
3.  Enter the desired number in field *Order number*.
4.  Press the [Filter] button.

### Expert Mode

This subject area will convey the use of the Production Manager in expert mode.
This includes the following training sessions:
*   "Overview"
*   "Order Selection"

#### Overview

**Objectives**
*   Getting to know the view
*   Knowing how data be loaded
*   Editing the contents of the views neatly.

**Benefit**
*   In expert mode you will perform the individual steps like creating batches, optimising them, etc. You can try out different variants to achieve the best possible result.

**Note**
*   **Expert Mode**: You have to switch explicitly to expert mode.

#### Start the Expert Mode

You can start the expert mode by pressing the corresponding icon. Among other things it is meant for multi-stepped glass production. You can perform all the necessary steps like e.g. compiling the individual batches. You can thus compile batches from different orders based on specific processing steps or optimize different batches together. In this mode, the program appears as follows:

*Figure 1-12 shows the main dialog in expert mode, with tabs for 1. Order Selection, 2. Batch Overview, 3. Optimization Manager, 4. Optimization Overview, and 5. Output. It displays sections for Selection Criteria, Orders, and Items.*

Production Manager consists of the main dialog and different tabs. The following main tabs are available:
*   Order selection
*   Batch list
*   Optimization manager
*   Optimization overview
*   Output

Apart from the main tabs there are the tabs which will flash up during the runtime. These include e.g. the *Detailed view* which is accessible from the *Batch view* tab. This view will appear to the right of the tab *Batch view*.

#### Order Selection

The *Order selection* offers various selection criteria for compiling an order item's BOM elements in one batch. It serves to restrict the number of orders/order items/BOM elements to be used for batch creation. If an order is selected, all of its items are selected too. You can select or deselect individual items however. If you select an item in section *Items*, the corresponding order will be selected too in section *Orders*.

The dialog consist of several sections. The top right section shows a list of the lites to be optimized. Here you can see the size of the batch. The bottom section offers order and item data for selection.

*Figure 1-13 shows the Selection criteria section with fields for Number Manager, Work Process, and Date range.*

Orders can be selected from the *Number manager* or from the *Process*. Processes can also be filtered by *Production date*.

##### Select the Orders

This unit teaches you how to select orders for the production manager. This unit includes the following authorizations to act:
*   How to select orders from the number manager
*   How to select orders by means of the process
*   How to find the orders

**How to select orders from the number manager**
1.  Click on the [Filter] icon. The fields for editing can be accessed now.
2.  Tick the radio button *Number manager*.
3.  Open the combo box.
4.  Choose the required NM.
5.  Press the [Search] icon.
6.  The data will be loaded.

**How to select orders by means of the process**
1.  Click on the [Filter] icon. The fields for editing can be accessed now.
2.  Tick the radio button *Process*.
3.  Open the combo box.
4.  Choose the required process.
5.  If required, the date fields *from* and *to* can be used to restrict the selection. These fields refer to the selection you have made in field *Process*. You can restrict the process to a certain date. This date refers to the production date. Example: Process *Drilling*, production date 15/06/2013 to 20/06/2013. If you have selected the process *Dispatch*, the defined date represents the shipping date.
6.  Press the [Search] icon.
7.  The data will be loaded.

##### The Order and Item Sections

The data shown in these areas are based on the settings in section *Selection criteria*. Section *Orders* offers a list of orders including order number, customer number, etc.

The contents of section *Items* depend on the selection criteria. The two examples below shall help to illustrate this. We will be using the same order which will be displayed with regard to different *Processes*.

If we select the entry *IG production*, the following data will be displayed:
*Figure 1-14 shows the order and item sections when the process is set to IG production. The Items section lists IG units.*

The order section shows all orders which include items to be arrissed (or drilled). We select order number 20143. In section *Items*, mark the individual items of the order 20143 that have to be arrissed. Please note that all items of an order will be marked and locked on the selection list when you select and mark an order in section *Order*.

You can now select individual items and include them in a special batch. To do this, first deselect the order in section *Orders* before selecting the relevant order items individually in section *Items*.

Selecting the entry *Cutting* results in the display of the following data:
*Figure 1-15 shows the item section when the process is set to Cutting. It now lists all the individual lites to be cut.*

#### Grouping of Data

Sometimes, a vast bulk of data will be displayed. To be able to keep still track of things, you can group the data then sort them in the group. Grouping of data is identical in the sections *Orders* and *Items*. To avoid redundant explanations we are going to describe this process in connection with the example of *Orders*.

Grouping is made in the table header: "Drag a column header to this point to group by this column".

The [Column selection] icon opens a box containing all the columns that can be used as grouping criteria. The following chart shows a small selection of columns.

*Figure 1-17 shows the Column selection popup with available columns like Order Number, Customer Number, Status, etc.*

##### Sorting of data

You can use the arrows at the end of the column for sorting the data of a group in ascending or descending order:
*   Up arrow: sorts the data in ascending order.
*   Down arrow: sorts the data in descending order.
If there is no arrow at the bottom of the column there will be no sorting.

##### Display the Data Clearly Arranged

This unit teaches you how you can show the displayed data clearly arranged through grouping.
This unit includes the following authorizations to act:
*   How to group the orders
*   Adding further groupings
*   How to save a group
*   How to remove the grouping

**How to group the orders**
1.  Click on the [Column selection] icon.
2.  A selection dialog appears.
3.  Click the left mouse key on the required field (e.g. customer number) and keep pressing the mouse key.
4.  Keep pressing the mouse key and move the field to the required point in the table header.
5.  When you have reached the required point, release the mouse key.

*Figure 1-19 shows data in the Orders section grouped by customer number.*

**Adding further groupings**
1.  Click on the [Column selection] icon.
2.  A selection dialog appears.
3.  Click the left mouse key on the required field (e.g. input date) and keep pressing the mouse key.
4.  Keep pressing the mouse key and move the field to the required point in the table header.
5.  When you have reached the required point, release the mouse key.

*Figure 1-20 shows data grouped by customer number and then by input date.*

**How to save a group**
1.  After you have created the group(s) you can save them.
2.  Press the [Save] icon.
3.  The dialog *Save view* appears.
4.  Enter a descriptive name in field *Name of the view*.
5.  Click on [OK].
6.  The dialog is closed; the name appears on the right side of the table header.

**How to remove the grouping**
1.  Select the group you want to delete.
2.  Click on the [X] icon.
3.  The selected group will be removed.

> **Deletion of groups**
> Groups will be deleted without a security query. The group will be deleted when you press the [X] icon!

#### Product

There is one more tab at the right side of the screen which can be expanded if required: **Tab Product**.

You can open the tab *Product* by clicking on it.
*Figure 1-21 shows the Product tab on the right side of the screen, displaying details like Quantity, Width, Height, Shape Number, and a graphic preview of the shape with dimensioning.*

This tab shows detailed information regarding the selected item including the shape parameter and a graphic preview with dimensioning.

#### Information

The fields in this section are the same as in the identically named sections in Standard mode which is why we are not going to explain them here again.

#### Rejects

If during the production lites with defects occur, these can now be entered for reproduction. Use the mouse to click the [Rejects] button to open tab *Reject Items*.

*Figure 1-22 shows the Reject Items tab, which lists existing rejects.*

This tab provides information on existing rejects and shows detailed information on rejects to be scheduled. To filter the data you can use the grouping types mentioned above.

You have the following options:
*   Enter rejects
*   Delete rejects
*   Create a reject batch

##### Enter rejects

Use this dialog to enter rejects. Open in tab *Reject Items* the context menu and the entry *Enter Rejects*. A dialog with the same name appears.

*Figure 1-23 shows the Enter Rejects dialog with fields for Order, Item, Quantity, Reason, and Location.*

Enter the order and item number and press the [Find] button to display all BOM parts for entered order and item number. Select the BOM parts that shall be entered as rejects and enter the requested quantity in field *Quantity*.

##### Create a reject batch

Use this dialog to create a reject batch. In tab *Reject Items* select the requested order number, open the context menu and the entry *Create New Reject Batch*. The *Create New Batch* dialog opens.

*Figure 1-24 shows the Create New Batch dialog with fields for Batch Number, Description, Rack Organization, and options for Steps after Batch Creation.*

This dialog is described in detail in chapter: Software Reference, "Create New Batch".

#### Working with Rejects

In this module you will learn how to deal with rejects.
This unit includes the following authorizations to act:
*   How to enter rejects
*   How to delete rejects
*   How to create a new reject batch

**How to enter rejects**
1.  Click on the icon button [Rejects].
2.  The *Reject Items* dialog opens.
3.  Go to field *Order* and enter the order number.
4.  Enter the item number in field *Item*.
5.  Click the [Find] icon button. The requested data is displayed in the list.
6.  Use the mouse to select the lite to be reproduced.
7.  In Field *Quantity* enter the number of lites to be reproduced.
8.  Choose the reject reason from the combo box *Reason*.
9.  Choose the reject place from the combo box *Location*.
10. Click on the [Save] button to save the data. The dialog is empty.
11. Click on button [End] to close the dialog. You are now back in tab *Reject Items*.

**How to delete rejects**
1.  Click on the icon button [Rejects].
2.  The *Reject Items* dialog opens.
3.  Select the item that is to be deleted.
4.  Open the context menu.
5.  Select *Delete Rejects*. There will be a security query. The item will be deleted if you confirm this by [Yes].

**How to create a new reject batch**
1.  Click on the icon button [Rejects].
2.  The *Reject Items* dialog opens.
3.  Select the order number the reject batch shall be created with.
4.  Open the context menu.
5.  Choose *Create New Rejects Batch*. The dialog *Create New Batch* opens.
6.  Enter the description for the reject batch in the *Description* field.
7.  Select the required organization from the combo box *Rack Organization*.
8.  Enter the factor in field *Factor for Rack Depth*.
9.  If necessary, enable the checkbox *Unlimited Rack Depth*.
10. Use the checkboxes below to control how to proceed with the batch. Enable the required checkbox(es).
11. Click on [OK].
12. The selected order number vanishes from the tab *Reject Items*.

#### Batch Management

**Objectives**
*   Learning how to create a batch.
*   Knowing how data be loaded
*   Editing the contents of the views neatly.

**Benefit**
*   Compiling batches in the optimal way will reduce the waste.

**Note**
*   **Batch number**: The batch number is assigned by the system.
*   **Rack Organization**: Can be changed after batch creation.
*   **Rack depth**: Changing the rack depth will influence the optimization result.

##### General

When a batch is created, all selected elements which have not been scheduled otherwise will be included.

Batches are either created by means of the number manager or by process using the tab *Order selection* (context menu *Create new batch*). The following dialog appears:

*Figure 1-25 shows the Create new batch dialog.*

**Description of fields**
*   **Description**: Can be used to enter a detailed description of the batch.
*   **Rack organization**: Select the required organization type from the combo box. The combo box lists all rack organizations defined for your site.
*   **Factor for the rack depth**: The factor for the rack depth to be used for this batch, in percent. The value for the rack depth is defined in master data (Production > Logical racks). You can use the factor to temporarily change the entry. 100% means that the entry made in master data will be used. 90% means that only 90% of the depth defined in master data will be used, i.e. less lites will fit onto the rack. An increase of this value will result in an overload.
*   **Unlimited rack depth**: Ticking this checkbox will overrule all the entries in master data.
*   **Steps after Batch Creation**:
    *   **Detailed Scheduling**: Enable this and the detailed scheduling starts automatically after batch formation.
    *   **Optimization Manager**: Can be enabled only if *Detailed Scheduling* is enabled. Then, the tab *Optimization Manager* opens after batch formation and detailed scheduling, but an optimization will not be generated.
    *   **Total Manual Cutting**: Can also be enabled after activating *Detailed Scheduling*. Then, all lites are set to manual cutting after batch formation and detailed scheduling.
    *   **Output**: Can be enabled only if *Detailed Scheduling* and *Total Manual Cutting* are enabled. Then, the tab *Output* opens automatically after batch formation, detailed scheduling, and manual cutting.

##### The batch has been created...

When the batch has been created, its status is *Roughly scheduled*. The created batches can be found on tab *Batch list*.

Roughly scheduled batches can be handled in the following way:
*   You can change the rack organization allocated at batch creation.
*   You can add further elements to the batch.
*   You can remove elements from the batch.
*   You can resolve the batch.
*   You can transfer the batch to detailed scheduling.

*Figure 1-26 shows the main dialog in expert mode on the batch list tab.*

The dialog consist of several sections. The top section shows the selection criteria. The bottom section lists the existing batches.

**Information and filter settings**

*Figure 1-27 shows the selection criteria for batches.*

*   **Batch number**: Can be used to display batches by number.
*   **Input date**: Can be used for displaying the batches by the date on which they were created.
*   **Status**: Combo boxes can be used to display the batches by status. The following statuses are valid:
    *   *Roughly scheduled*: No rack allocation has been made for these batches yet.
    *   *Scheduled in detail*: These batches have been allocated to racks.
    *   *Partly optimized*: Some of the glass types included in these batches have already been optimized.
    *   *Optimized*: All glass types of these batches have been optimized already.
    *   *Partly finished*: This field will not be analysed at present.
    *   *Completed*: All elements belonging to these batches are completed.
*   **Description**: Use this field to display the batches by name.

**Information and filter settings in section Batches**
Entries which appear in light grey in this section have already been transferred to the optimization manager. If you click on such an entry, a message to that effect will pop up. You can display the detailed view and the detailed scheduling results for these entries and start the output (machines, reports, etc.). Grouping and sorting can be used to manage large amounts of data.

##### Select Batches Based on Certain Criteria

This unit teaches you how to select batches for production.

**How to select the batches by means of the batch number**
1.  Click on the [Filter] icon.
2.  Enter the lowest batch number in field *from* and the highest batch number in field *to*.
3.  Click on the [Search] icon.
4.  The data will be loaded.

**How to select the batches by means of the input date**
1.  Click on the [Filter] icon.
2.  Enter the input date in the fields *from* to.
3.  Click on the [Search] icon.
4.  The data will be loaded.

**How to select the batches by status**
1.  Click on the [Filter] icon.
2.  Enter the appropriate criteria in the fields *from* to.
3.  Click on the [Search] icon.
4.  The data will be loaded.

**How to select the batches based on their description**
1.  Click on the [Filter] icon.
2.  Enter the appropriate text in the *Description* fields.
3.  Click on the [Search] icon.
4.  The data will be loaded.

##### Detailed View for Batches

The context menu permits to view the batches in detail. The corresponding batch appears on a separate tab. After selecting a batch, select the entry *Detailed view* from the context menu. The batch and all its elements appear on a separate tab. This dialog is also split into different sections:

*Figure 1-28 shows the detailed view for a batch, including sections for Detailed Scheduling, Optimization Article, Orders, and Items.*

*   **Detailed scheduling**: Shows the data you have selected or entered for creating the batch. You can change the batch description, rack organization, and rack depth factor here.
*   **Optimization articles**: This section shows the glass type, the quantity to be optimized, the square metres of surface per glass type, and the corresponding amount of square metres compared with the total surface of the batch. Example: The batch has a total surface of 67.86 sqm to be optimized. Article 104 A+W Float 4 mm has a surface of 16.35 sqm. These 16.35 sqm represent 24.10 % of the total surface.
*   **Orders and Items**: Show all information relevant for the order and items.

##### Tab Product and Cutting

There are two more tabs at the right side of the screen which can be expanded if required: *Tab Product* and *Tab Cutting*.

**Tab Product**
The tab is the same as the identically named fields on tab *Order selection* which is why they are not described here again.

**Tab Cutting**
You can open the tab *Cutting* by clicking on it.
*Figure 1-31 shows the Cutting tab on the right side of the screen, with shape parameters and a preview.*
It shows detailed information regarding the selected lite including the shape parameter and a graphic preview. The dotted line shows the shape trims. Use the button [Edit] to open dialog *Edit cutting*.

*Figure 1-32 shows the Edit cutting dialog.*
This dialog allows various modifications. You can select e. g. a different shape, the shape parameter as well as the shape trims and change the quantity to be produced. The dotted line shows the shape trims. The modifications will be displayed in section preview.

> **Edit Cutting Data**
> Please consider that any modifications made here, will only affect the cutting. They will not be transferred to the order system.

#### Detailed Scheduling

**Objectives**
*   Getting acquainted with and understanding detailed scheduling
*   Getting acquainted with and understanding optimization modes
*   Circumstances in which the individual modes are used

**Benefit**
*   Only knowing and understanding the different optimization modes will enable you to adapt detailed scheduling to your production so that it will operate effectively and in a time-saving manner.

**Note**
*   **Variant**: The optimization variants you have been trying out will be kept so that you can choose the best ones.
*   **Detailed scheduling**: Distribution of the lites of an order to different glass stacks and racks according to defined criteria for grouping and sorting.

##### The Process of Detailed Scheduling

Roughly scheduled batches can be transferred from tab *Batch list* to detailed scheduling. The task of detailed scheduling is to determine a production sequence for the elements of these jobs/batches.

The production sequence can be determined by criteria like:
*   Customer's requirements
*   Production restrictions

This step also includes the currently assigned rack organization. The batch status changes from *Roughly scheduled* to *Scheduled in detail*.

Batches which have been scheduled in detail can be treated in the following ways:
*   You can repeat detailed scheduling any number of times (e.g. due to changed rack organization master data).
*   The batches can be transferred to the optimization manager.
*   You can resolve the batch.
*   You can view the rack load.

#### Optimization Manager

Batches which have been scheduled in detail can be transferred to the optimization manager. When the first optimization for a batch has been run and confirmed, the status changes to *Partly optimized*.

Partly optimized batches can be handled in the following ways:
*   You can edit individual optimizations of the batch.
*   You can treat these batches in just the same way as batches which have been scheduled in detail (except resolving the batch).

*Figure 1-33 shows the Optimization manager tab, which is split into sections for Batches, Glass Types, Optimizations, and Total Result.*

This tab serves to optimize the individual glass types for the selected batches.

*   **Description of fields in section Batches**: Shows details of the selected batches (number, creation date, status, etc.).
*   **Description of fields in section Glass Type**: Shows the individual glass types included in the batch, with quantity, surface, and batch information.
*   **Sections Optimizations and Total Result**: The fields are the same as in Standard mode.
*   **The tabs Stockplates and Optimization Parameters**: The tabs are the same as in Standard mode.

##### Optimize Batches

This session shows you how to optimize batches.

**How to transfer batches to the optimization manager**
1.  Select the required batch(es) on tab *Batch list*.
2.  Open the context menu.
3.  Click on the menu entry *Optimization manager*.
4.  Tab *Optimization manager* appears and the data are loaded.

> **Batch transfer**
> Only batches with the status *Scheduled in detail* can be transferred to the optimization manager!

**How to set a glass type to manual cutting**
1.  Select the required glass type(s) in section *Optimizations*.
2.  Open the context menu.
3.  Click on the menu entry *Manual cutting*. The tick in front of the glass type vanishes and the *Result* field shows the entry *Manual cutting*.

**How to start the optimization**
1.  Select the required glass type on tab *Optimization manager* in section *Optimizations*.
2.  Open the context menu.
3.  Click on the menu entry *Start optimization*.
4.  After optimization, the section *Total result* is filled with data.
> **Ribbon bar**
> You can also use the ribbon bar (start) to start the optimization. Opening the context menu can be omitted in this case.

**How to save the optimization**
1.  Open the context menu.
2.  Click on the menu entry *Save optimization*.
3.  The optimization will be saved.

##### Temporary Optimization

> **Ribbon bar**
> You can also use the ribbon bar (save) to save the optimization. Opening the context menu can be omitted in this case.

Every click on the [Start] icon starts a new optimization. This process serves to optimize batches with different variations. You can e.g. exchange glass types or change optimization parameters or stockplates. Existing optimizations are shown as variants in section *Total result*.

In section *Optimizations* you can use the context menu to open the detailed view. It appears on a separate tab.

*Figure 1-36 shows the detailed view of an optimization, including sections for Rack, Batches, Stock Sizes, Pattern, and a visual Cutting Plan.*

This dialog is also split into different sections:

*   **Description of the fields in section Rack**: Displays batch number, rack number, rack type, and logical rack.
*   **Description of fields in section Batches**: Displays batch number and creation date.
*   **Description of the fields in section Stocksizes**: Shows quantity, height, width, surface, and priority of stock plates.
*   **Description of the fields in section Pattern**: Lists individual patterns with their optimization group, quantity, height, and width.
*   **Description of the fields in section Cutting Plan**: Shows a sketch of the cutting plan created by the optimization. It represents the stockplate to be cut and provides information on the optimization, the article, and the individual lites (rack number, lite size, order/item number).

##### Abort Optimization

Here it is possible to stop a running optimization by clicking on [Abort].
*Figure 1-42 shows the optimization progress dialog with a [Cancel] button.*

#### Optimization Overview

The optimization overview provides a comprehensive view of the optimizations that have been run.

*Figure 1-43 shows the Optimization overview tab, listing all executed optimizations with their details.*

This tab shows the optimizations which have been run for the individual glass types. Various selection criteria can be used to keep the contents of this list at bay. You can view the details of a selected glass type (detailed view) and start the output (machine output, reports).

**Description of fields in section Selection Criteria**
*   **Optimization**: Use *from* to fields to filter by optimization number.
*   **Input date**: Use to display optimizations run on certain days.
*   **Batch numbers**: Use to filter for specific batch numbers.

**Description of fields in section Optimizations**
*   **Optimization**: The optimization number.
*   **Optimization mode**: Random (XOPT) or standard for IG (XOPT-S).
*   **Glass type**: The glass types included in the optimization.
*   **Cutting table**: The table on which the glass is cut.
*   **Batches**: The batch number.
*   **Status**: *Optimized, Released, Partly completed, Completed, Withdrawn*.
*   **Quantity**: Quantity per glass type.
*   **Surface**: Surface in square metres.
*   **Result**: The optimization result for the corresponding glass type in %.

#### Optimization Detailed View

In section *Optimization overview* you can use the context menu to open the detailed view. It appears on a separate tab.
This dialog is the same as dialog *Temporary optimization*.

*Figure 1-46 shows the detailed view of an optimization, which is identical in layout to the Temporary Optimization view.*

#### Output

**Objectives**
*   Knowing the different views of the tab.
*   Knowing about the output of the different media.

**Benefit**
*   The optimization manager knows which output is required for the individual batches. Nothing will be omitted.

**Note**
*   **Entries shaded in grey**: There will be no output for entries shaded in grey.
*   **Printer**: Printing can be done on the standard printers or on other printers.
*   **Paper and cutting code**: Tab *Output* serves to print all necessary / selected production papers and start the data transfer to the machines.

##### Reports and Cutting Codes

All output, no matter if on paper or in the shape of a file, is started from this tab. The dialog is accessible directly (tab *Output*), from the tab *Batch list*, and from the tab *Optimization overview*.

From the *Batch list* you can access the output only for batches with the status *Scheduled in detail*, *Optimized*, or *Released*. For batches the status of which is roughly scheduled, output cannot be started because detailed scheduling is missing. Output is accessible for all optimizations from the *Optimization overview*.

*Figure 1-47 shows the Output tab, split into sections for Batches/Optimizations, Reports, and Machines.*

**Description of fields in section Batches/Optimizations**
The content of this section depends on whether it was accessed from the *Batch list* or *Optimization overview*. It shows details of the selected batch(es) or optimization(s). A symbol in the *Message* column indicates if the output is correct.

**Description of fields in section Reports**
*   **Name**: Defines the report (e.g., Production lists, Manual cutting lists, Labels).
*   **Printer**: A combo box to select the printer.
*   **Copies**: Field to set the number of copies.
*   **Settings**: Offers context menus depending on the report type. For *Labels*, you can define serial label printing behavior (e.g., series from a certain quantity, one label per item/unit).
*   **Message**: An icon shows the current status. Greyed-out entries will not be printed.

**Description of fields in section Machines**
*   **Machine**: Shows the machine name.
*   **Output**: Defines the directory in which the machine code is saved.

##### Data Issued

This unit teaches how a list is printed and how a cutting code is generated.

**How to print a list**
1.  Select the optimization for which the list must be printed in the *Optimizations* section.
2.  Select the required list in the *Reports* section.
3.  Press the [Start] icon.
4.  The output will be started.

**This is how you generate the cutting code for a machine**
1.  Select the optimization for which the cutting code must be generated in the *Optimizations* section.
2.  Select the machine for which the code must be generated in the *Machine* section.
3.  Press the [Start] icon.
4.  The output of machine control begins.

### Master Data

This subject area introduces the production manager's master data and how to use them.
This includes the following training sessions:
*   "Racks"
*   "Criteria"
*   "Grouping and Sorting"

#### Racks

**Objectives**
*   Knowing and understanding racks
*   Knowing and understanding stacking modes
*   Understanding the effects of the rack modes

**Benefit**
*   Once you have understood the functions of the stacking modes you can organize your production accordingly. A well-organized production will save time, space, and money.

**Definitions**
*   **Physical rack**: Rack (A rack, L rack, fixed rack)
*   **Logical rack**: A logical rack consists of one or more stacks of glass and defines how these stacks belong together (e.g. to turn them into IG or laminated glass units). This depends on the selected stacking mode. A logical rack is just an area on a physical rack with a certain number, onto which glass stacks can be put that belong together.
*   **Rack depth**: The rack depth defines the maximum stack depth (maximum load) of the rack. The bigger the entry here, the more lites can be loaded in front of each other.

**Note**
*   **What can be put on a rack?** Generally, only parts of a batch can be put onto a stack or on a harp rack.
*   **Different glass types on a stack**: The program generally separates different glass types and allocates them to different stacks.
*   **Stacking mode**: Different glass types can be combined on a logical rack.

##### Logical Racks and Rack Depth

A logical rack consists of one or more stacks of glass and defines how these stacks belong together. A logical rack is just a numbered section on a physical rack onto which matching stacks of glass are loaded. Lites are loaded onto the logical racks in the production sequence defined for the individual racks.

Physical racks are created from the logical racks. For A racks and L racks, this is done by taking into account the rack depth plus the number of rack sides (1 or 2 for L or A racks).

*Figure 1-52 illustrates the concept of Logical Racks and Rack Depth.*

The rack depth defines the maximum stack depth (maximum load) of the rack. The bigger the entry here, the more lites can be loaded in front of each other. A new stack will be started when the rack depth and thus the maximum load has been reached.

##### Rack Mode for A Racks

Production Manager uses a rack mode in which different glass types can be combined in several stocks on a logical rack. Different product combinations to be produced can be loaded.

*Figure 1-53 illustrates the rack mode for A racks.*

*   Each glass type is set onto a different stack.
*   Different glass types are put onto a logical (or physical) rack together.
*   When a stack has reached the maximum, the whole rack number is considered to be "full".
*   Groups belonging together must be defined and kept together.
*   You will need less physical racks.
*   You will need additional auxiliary and control mechanisms (e.g. production papers or monitoring systems) to keep track of things.

> **Separation of glass types**
> The program always separates the glass types. This applies to the stacking of glass types and to optimization.

**Stacking of split groups**
When a stack has reached the maximum load, the last group will be split. The lites of this group which exceed the maximum load (rack depth) and the corresponding lites of the appropriate group on the other rack are moved to a new rack together - with a new rack number. (e.g., Group 3 is over the limit, so the last lite of group 3 and the last lite of group 4 will go to a new rack: 1002). New glass types and new groups can be put onto this rack. Rack 1001 is considered to be full while rack 1002 can take more groups until the maximum load is reached.

*Figure 1-54 illustrates the stacking of split groups.*

**Buffer rack**
There is a special rack for each of the three sections IG, laminated glass and glass which collects all those BOM elements which are not put onto a regular rack. These three racks are A racks with an unlimited rack depth and fixed rack numbers: 9991 (glass), 9992 (laminated glass), and 9993 (IG).

> **Clashing numbers**
> When racks are allocated for rack organization, the program checks if the rack numbers used (from-to) clash with other rack numbers or with the fixed rack numbers 9991, 9992, and 9993. Clashing numbers are invalid! If this occurs, the program will inform you accordingly. The conflicts must now be solved.

##### Rack definition and management

The entries are loaded from master data (Production > Rack organization). This is where the rack types can be defined and managed: **Master data > Production > Logical racks**.

*Figure 1-55 shows the Logical Racks management dialog.*

The dialog consists of several sections. The top left section shows the fields rack name and type. The type is the detailed scheduling type. The following types are available:
*   IG
*   LG
*   Glass (individual lites as complete lites to be shipped, or processed lites)

> **Detailed scheduling type and racks**
> This allocation also makes sure that the lites are loaded onto the appropriate racks. This means that if you choose the detailed scheduling type LG for example, the lites will be automatically loaded onto racks meant for laminated glass. No additional filter (criterion) is required. Within the rack organization for LG racks (allocation) you can use criteria to distinguish e.g. shapes and rectangles and distribute them to different rack numbers.

The section below refers to the *Grouping* and *Sorting* of the groups. You can assign existing groupings here and define whether groups shall be sorted.

The data concerning the physical racks are shown below this. The fields *Rack no. from to* define the range of numbers for the corresponding rack.

#### Rack Groups

Rack groups serve for processing racks in front of the IG line or laminating compound by turns. They are essential if a rack-wide production sequence is required. Racks which have not been allocated to any rack group can be used for production at random.

**Example**: lites (from one rack group) smaller than 2500 x 1400 are put onto harp racks. All other lites are loaded onto A racks. The desired production sequence is: by order (order A, order B, order C). Lites from orders A, B, and C are put onto harp racks as well as onto A racks. If this is the case, both racks have to be accessible at the same time for IG production. This method is only possible if a *Rack group* is used for *Rack organization*.

The rack group is assigned a sorting key. This key sorts the lites on the racks that belong to this group. The corresponding settings are made in dialog *Rack groups*: **Master data > Production > Logical rack groups**.

*Figure 1-56 shows the Rack Groups dialog.*

##### Working with Rack Groups

This unit teaches you how to handle rack groups.

**How to define a new rack group**
1.  Click on the icon [New].
2.  Enter the desired name in the *Name* field.
3.  Choose the corresponding sorting from combo box *Sorting key*.
4.  Click on the [Save] icon.

**How to change an existing rack group**
1.  Go to section *Rack groups* and select the group you want to change.
2.  Make the required changes. You can change the name as well as the sorting key.
3.  Click on the [Save] icon.

**How to delete a rack group**
1.  Go to section *Rack groups* and select the group to be deleted.
2.  Click on the [Delete] icon.
3.  There will be a security query. Click on [Yes].
4.  The entry will be deleted.

#### Criteria

Criteria serve for checking whether a certain BOM element can be allocated to a logical rack. Criteria are computing rules using formulas to define whether an element meets the specified conditions of the logical rack. It may be required to allocate lites to a new subsequent rack based on a certain criterion. This is done by means of the checkbox *Change rack at*.

The corresponding dialog is at: **Master data > Production > Criteria**.

*Figure 1-57 shows the Criteria dialog, with a list of criteria on the left and a formula builder with variables on the right.*

The dialog consists of several sections. The top section shows the details of the selected criterion. Field *Name* shows the name of the criterion. Field *Description* contains a more detailed description. Section *Formula* shows the formula of which the criterion consists.

**Formula**
The term *Formula* stands for a (mathematical) function based on the properties of the BOM elements which has a certain value (variable). The variables which can be used in formulas have English names and are shown in the national language, e.g. *Width*.

##### Working with Criteria

This unit teaches you how to handle criteria.

**How to define a new criterion**
1.  Click on the icon [New].
2.  Enter the desired name in field *Name*, e.g. **Series**.
3.  Field *description* can be used to enter an additional description, e.g. **Quantity > 15**.
4.  The *Formula* field is used for assigning the criteria to the formula in the tree structure on the right. Example: If you double-click on the entry *Quantity*, the entry appears in section *Formula*. Now move the cursor right behind the entry and enter **>15**.

**How to change an existing criterion**
1.  Go to section *Selection* and choose the entry you want to change.
2.  Make the required changes in section *Criterion*.
3.  Press the [Save] button.

**How to delete a criterion**
1.  Go to section *Selection* and enter the formula to be deleted.
2.  Click on the [Delete] icon.
3.  There will be a security query. Click on [Yes].
4.  The entry will be deleted.

#### Sorting Key

So-called sorting keys help to sort a large number of elements. A sorting key can be a single field, e.g *Order number* or *Customer number* or can consist of several, linked fields. In the rack organization, a sorting key is allocated to a rack group. This key sorts the elements of a group. The appropriate settings are made in dialog *Sorting key*: **Master data > Production > Sorting key**.

*Figure 1-59 shows the Sorting key dialog.*

The dialog is split into different sections. The top section shows the name of the sorting key. Section *Sorting key* shows the name and a preview. The fields *Formula* and *Sorting* in section *Details* are combo boxes which can be expanded. Combo box *Formula* contains all entries made in dialog *Criterion*. Combo box *Sorting* defines whether the entries are sorted in ascending or descending order. The sorting keys also serve for *Grouping* and *Sorting* within the groups on the logical racks.

##### Working with Sorting Keys

This unit teaches you how to handle sorting keys.

**How to define a new sorting key**
1.  Click on the icon [New].
2.  In field *Name*, enter the name of your choice, e.g. **Order**.
3.  Choose the required entry from the combo box *Formula*.
4.  Choose the required sorting from combo box *Sorting*.
5.  Click on the [Save] icon.

**How to change an existing rack group**
1.  Go to section *Sorting key* and choose the entry to be changed.
2.  Change the fields *Formula* and *Sorting* as required.
3.  Click on the [Save] icon.

**How to delete a sorting key**
1.  Go to section *Sorting key* and choose the entry to be deleted.
2.  Click on the [Delete] icon.
3.  There will be a security query. Click on [Yes].
4.  The entry will be deleted.

#### Rack Organization

Tailored to the individual production, different rack organizations can be defined in the program. One of these rack organizations can be selected as the standard organization. When a batch is created, this rack organization will be assigned to the batch by default. This assignment can be changed prior to detailed scheduling.

The rack organization mainly describes the following aspects of production:

*   **The products to be produced (what):** The rack organization is used to classify the different product types collected in a batch (IG, laminated glass, toughened glass, processed glass) by the following three types: IG, Laminated glass, Glass (including toughened glass). This classification results in lot types.
*   **Racks onto which the lites or intermediate products are to be loaded (where):** The second step defines the logical rack onto which the lites of the (intermediate) product are to be loaded. The criterion of each logical rack will be determined based on the properties of the (intermediate) product to be sorted and if the criterion is relevant for a logical rack, the (intermediate) product will be allocated to this logical rack. If none of the rack organization criteria applies, this product is passed on to the automatically created buffer rack.
*   **Chronological and organizational production process (how):** The sequence of lines from top to bottom represents the chronological sequence in which the logical racks will be processed. Lites allocated to a logical rack are actually loaded onto physical racks (harp racks, A racks, L racks) which have natural restrictions (e.g. number of slots, rack depth).

The corresponding dialog is at: **Master data > Production > Rack organization**.

*Figure 1-60 shows the Rack Organization dialog.*

#### Grouping and Sorting

**Objectives**
*   Knowing and understanding grouping
*   Knowing and understanding sorting
*   Understanding the effects of grouping and sorting.

**Benefit**
*   Grouping and sorting serves to organize the stacking of the individual lites in the required sequence. Without grouping and sorting, the lites would have to be resorted prior to every production step.

**Definitions**
*   **Grouping**: is done by different, unique values for a property, e. g. by customer number, glass thickness.
*   **Sorting**: is based on properties which assume a progressive value within the defined group (e.g. size).

**Note**
*   **Creation**: Grouping or sorting is created by random combinations of properties and formulas.

##### General

The groups and sorting allows allocating the required production sequence to the individual racks. Production Manager allows defining grouping criteria and deciding whether grouping shall be done in a certain sequence (sorted groups) or whether the contents of the groups shall be sorted (sorting within the group). Every logical rack can have its own grouping and sorting.

Optimization calculates the optimum yield taking into account the grouping and sorting. Once it has been set up, the defined sequence can be used for matching lites of an IG and laminated glass unit.

*Figure 1-61 illustrates grouping by glass type and sorting by size within each group.*

The illustration above shows lites grouped by thickness. Within each group (perhaps one rack per thickness), lites are sorted by height. Grouping and sorting depend on how your production is organized and being run. They are defined by a random combination of properties and formulas. The appropriate settings are made in dialog *Sorting key*.

## Software Reference

### Overview

Open the menu **Master data > Production**.

All data required for the correct operation of the production manager are entered and managed in module *Master data* (section *Production*).

Master data are arranged in the following menus:
*   **Rack organization**: This menu item is used to define the rack organization.
*   **Criteria**: This menu item is used to define the criteria.
*   **Logical racks**: This menu item serves to define the logical racks.
*   **Rack groups**: This menu item is used to define the rack groups.
*   **Sorting key**: This menu item serves to define the sorting keys.

> **Dialog buttons**
> The standard buttons and menus are described in detail in section Overview and in the tutorials. We are therefore not going to describe them in connection with the dialogs.

### Rack Organization

**Master Data > Production > Rack Organization**

*Figure 1-62 shows the Rack Organization dialog.*

This dialog is used to define the rack organization or to change existing organizations.

**Description of the fields in section Selection**

*   **Name**: Enter the name of the rack organization or change the name of an existing rack organization.
*   **Standard**: This checkbox defines whether the rack organization shall be used as the standard organization. Only one rack organization can be used as a standard at a time.

**Description of the fields in section Rack Organization**

*   **Name**: This field shows the name of the rack organization.
*   **Standard**: This checkbox defines whether the rack organization shall be used as the standard organization.
    *   Yes: This rack organization is the standard organization.
    *   No: This rack organization is no standard organization.

**Description of the fields in section Details**

*   **Type**: This field shows the detailed scheduling type. Valid options: IG, LG, Glass.
*   **Formula**: This field shows the formula for the rack organization, based on criteria.
*   **Rack (logical)**: This field shows the logical rack.
*   **Rack group**: This field shows the rack group.
*   **Production sequence**: Defines the production sequence if more than one detailed scheduling type is used.
*   **Sequence of checks**: Defines the sequence in which the logical racks are going to be checked.
*   **Rack no. (from)**: This field shows the start of the rack number range for the rack in question.
*   **Rack no. (to)**: This field shows the end of the rack number range for the rack in question.
*   **Rack no. (current)**: This field shows the current rack number.
*   **Rack (physical)**: This field shows the name of the physical rack.
*   **Rack depth**: This field shows the depth of the physical rack if the rack is an A or L rack.
*   **Number of slots**: If the rack is a harp rack, this field shows the number of slots this rack offers.
*   **Number of lites per slot**: If the rack is a harp rack, this field shows how many lites can be put into a slot.

### Criteria

**Master Data > Production > Criteria**

*Figure 1-63 shows the Criteria dialog.*

This dialog is used to define the criteria for the racks to change them.

**Description of the fields in section Selection**

*   **Name**: Enter the name of the criterion or change the name of an existing criterion.
*   **Sorting key**: The combo box lists all sorting keys defined for your company. Expand the box and choose the required sorting key.

**Description of the fields in section Rack Groups**

*   **Name**: This field shows the name of the rack group.
*   **Sorting key**: This field shows the name of the sorting key.
*   **Sorting key preview**: This field shows the formula which defines the sorting key.

### Logical Racks

**Master Data > Production > Logical Racks**

*Figure 1-64 shows the Logical Racks dialog.*

Use this dialog to define the logical racks which exist in your company, or change existing racks.

**Description of the fields in section Logical Racks**

*   **Name**: Enter the name of the logical rack.
*   **Type**: Choose the required type from the combo box. Valid options: IG, LG, Glass.

**Description of the fields in section Grouping/Sorting**

*   **Grouping**: The combo box lists all groups defined for your company. Select the required group.
*   **Sorting within groups**: The combo box lists all sortings defined for your company. Choose the required sorting.
*   **Sort groups**: This checkbox defines whether the groups shall be sorted.

### Rack Groups

**Master Data > Production > Rack Groups**

*Figure 1-65 shows the Rack Groups dialog.*

This dialog can be used to collect certain racks in a rack group. This means that for laminated glass production, racks belonging to the same group will be alternately accessed before proceeding to the next rack.

**Description of fields**

*   **Name**: Enter the name of the rack group.
*   **Sorting key**: The combo box lists all sorting keys defined for your company.
*   **Sorting key preview**: This field shows the formula which defines the sorting key.

### Sorting Key

**Master Data > Production > Sorting Key**

*Figure 1-66 shows the Sorting key dialog.*

This is where you can define a sorting key to sort a number of elements. This key sorts the lites on the racks that belong to this group.

**Description of the fields in section Logical Racks**

*   **Name**: Enter the name of the sorting key.
*   **Formula**: Select the required formula from the combo box.
*   **Sorting**: Select the required sorting from the combo box (Ascending/Descending).

### Standard Mode

This section offers the data you will need to operate the Production Manager in standard mode. You will find the following entries:
*   "Order Selection"

#### Wizard

**Production Manager > Standard Mode**

*Figure 1-67 shows the standard mode dialog.*

In standard mode, the program can be operated by means of simplified user prompts (Wizard). The Wizard permits to start the whole process (batch creation, optimization, etc.) with just a few entries.

**Description of the fields in the section Batch creation**

*   **Number manager**: Use the combo box to access the corresponding data.
*   **Batch**: After you made the selection in the number manager, this field shows the batch number.
*   **Status**: This field shows the batch status.
*   **Name**: This field shows the name of the number manager, the user, and the batch creation date.
*   **Batch content**: This field will be filled after batch creation.

**Description of the fields in section Detailed Scheduling and Optimization**

*   **Rack organization**: The combo box lists all rack organizations defined for your company.
*   **Factor for the rack depth**: The factor for the rack depth (in percent) to be used for this batch.
*   **Unlimited rack depth**: This checkbox defines whether the depth of this rack is unlimited.
*   **No. of variants**: If a Range is set for the rack depth (e.g. 80-120%), this field defines the number of variants created.

**Description of the fields in the section Save**

*   **Output**: This is where all output types are set. Options are *None, All, Selection*.

**Description of fields in section optimizations**

*   **Glass type**: This field shows the glass types included in the batch.
*   **Cutting table**: Here, you see the table on which the glass shall be cut.
*   **Jobs**: This field shows the batch number.
*   **Quantity**: This column shows the number of lites to be optimised.
*   **Size**: This column shows the total surface of the article to be optimised.
*   **Result**: This field shows the optimization result for the glass type in question.
*   **Waste**: This field shows the total waste of the glass type in the currency set for A+W Business Pro.

**Description of the fields in section Overall Result**

*   **Variant**: This field shows the different optimization variants.
*   **Rack organization**: This is where the rack organization that you have chosen at batch creation is shown.
*   **Number of harp racks**: Here you see the number of harp racks which are necessary to put away the lites of the batch.
*   **Number of A racks**: Here you see the number of A racks which are necessary to put away the lites of the batch.
*   **Result**: This field shows the total waste of the glass type in the currency set for.
*   **Waste**: This field shows the total waste of the glass type in the currency set for A+W Business Pro.

### Expert Mode

This section offers the data you will need to operate the Production Manager in expert mode. You will find the following entries:
*   "Order Selection"
*   "Reject Items"
*   "Create New Batch"
*   "Cutting"
*   "Optimization Manager"
*   "Output"

#### Order Selection

**Production Manager > tab Order Selection**

*Figure 1-68 shows the Order selection in expert mode.*

Use this dialog to create production batches and optimizations.

**Description of fields in section Selection Criteria**

*   **Number manager**: After ticking the radio button you can access the corresponding data in the combo box.
*   **Work Process**: After ticking the radio button you can access the corresponding data in the combo box.
*   **Date from - to**: These fields refer to the selection you have made in field *Process*.

**Description of the fields in section optimization Articles**

*   **Product**: The product number.
*   **Product name 1**: The product name.
*   **Quantity**: The number of lites to be optimised.
*   **Size**: The total surface of the article to be optimised.
*   **m²%**: The surface of the article in relation to the total surface of the batch.

**Description of the fields in section Orders**

*   **Order number**, **Customer number**, **Status**, **Input date**, **Order area**, **Consultant**, **Salesman**, **P.O. date**, **Shipping date**, **Requested date**, **Delivery date**, **Route**, **Priority**, **Customer data**.

**Description of the fields in section Items**

*   Includes fields such as **Order number**, **Item number**, **BOM item**, **Product**, **Product name 1+2**, **Quantity**, **Width**, **Height**, **Product type**, **Procurement type**, and many others detailing each line item.

#### Save View

**Production Manager > tab Order Selection > Group Orders > icon [Save]**

*Figure 1-69 shows the Save view dialog.*

This dialog allows saving the grouping, the sequence and the number of fields in the list for the view in question.

*   **Name of view**: Enter the name of the view by which this grouping shall be saved.

#### Product

**Production Manager > tab Order Selection > tab Product**

*Figure 1-70 shows the Product tab.*

This tab shows detailed information regarding the selected lite including the shape parameter and a graphic preview.

**Description of fields**
*   **Quantity**, **Width**, **Height**, **Shape number**, **SN file**, **Shape parameter**.

#### Reject Items

**Production Manager > tab Reject Items**

*Figure 1-71 shows the Reject items tab.*

This tab appears after you press the icon button [Rejects]. You can enter rejects or create reject batches with existing reject lites.

**Description of fields**
*   Includes **Order number**, **Item number**, **Sub-item number**, **BOM item**, **Batch**, **Product**, **Quantity**, **Width**, **Height**, etc.

#### Enter Rejects

**Production Manager > tab Reject Items > Context menu > Enter Rejects**

*Figure 1-72 shows the Enter rejects dialog.*

In this dialog, you have the opportunity to enter rejects manually.

**Description of fields**
*   **Order**, **Item**, **Quantity**, **Reason**, **Location**, **Sub-item number**.

#### Create New Batch

**Production Manager > tab Order Selection > Select order > Open context menu > Create New Batch** or from **Reject Items** context menu.

*Figure 1-73 shows the Create new batch dialog.*

This dialog is used for creating new batches.

**Description of fields**
*   **Batch number**: Assigned by the system.
*   **Name**: Enter the name of the batch.
*   **Rack organization**: Select the organization type.
*   **Factor for the rack depth**: The factor for the rack depth (in percent).
*   **Unlimited rack depth**: Checkbox to define if depth is unlimited.
*   **Description of check boxes**: *Detailed scheduling*, *Optimization manager*, *Total manual cutting*, *Output*.

#### Batch Overview

**Production Manager > tab Batch List**

*Figure 1-74 shows the Batch list.*

This dialog shows you all saved created batches.

**Description of fields in section Selection Criteria**
*   **Batch number**: Fields *from to* can be used to display batches by number.
*   **Creation date**: This field can be used for displaying the batches by date.
*   **Status**: This combo box can be used to display the batches by status.
*   **Name**: You can use this field to display the batches by name.

**Description of fields in section Batches**
*   **Batch number**, **Creation date**, **Status**, **Description**, **Rack organization**, **IG**, **LG**, **Toughened glass**, **Glass (single and processed)**, **Factor for the rack depth**.

#### Detailed View

**Production Manager > tab Batch List > Select batch > Open context menu > Detailed View**

*Figure 1-75 shows the Detailed view for a batch.*

This dialog allows viewing a selected batch in detail.

**Description of the fields in section Detailed Scheduling**
*   **Name**, **Rack organization**, **Creation date**, **Status**, **Factor for the rack depth**, **Unlimited rack depth**.

**Description of the fields in section optimization Articles**
*   **Product**, **Product name 1**, **Quantity**, **Surface**, **Surface %**.

#### Cutting

**Production Manager > tab Details > tab Cutting**

*Figure 1-76 shows the Cutting tab.*

This tab shows detailed information regarding the selected lite including the shape parameter and a graphic preview.

**Description of fields**
*   **Quantity**, **Width**, **Height**, **Shape number**, **SN file**.

#### Edit Cutting

**Production Manager > tab Details > tab Cutting > Button [Edit]**

*Figure 1-77 shows the Edit cutting dialog.*

This dialog shows detailed cutting information regarding the selected lite.

**Description of fields**
*   **Quantity**, **Width**, **Height**, **SN file**, **Shape parameter**, **Shape trims**.

#### Set Batch Status

**Production Manager > tab Batch List > Select order > Open context menu > Set Batch Status**

*Figure 1-78 shows the Set batch status dialog.*

This dialog serves to change the status of a batch.

*   **New batch status**: Use the combo box to set the batch status to *Completed*.

#### Machine Rescheduling

**Production Manager > tab Batch List > Select batch > Open context menu > Machine Rescheduling**

*Figure 1-79 shows the Machine rescheduling dialog.*

Use this dialog to re-schedule products to other machines. It consists of two sections: *Current machine allocation* and *Alternative machines*.

#### Optimization Manager

**Production manager > tab Optimization manager**

*Figure 1-80 shows the Optimization manager.*

This dialog displays the batches that were transferred to the optimization manager. It consists of sections for *Batches*, *Glass type*, *Optimizations*, and *Total result*.

#### Abort Optimization

**Production Manager > tab Optimization Manager > Execute > Optimizations > [Cancel]**

*Figure 1-81 shows the optimization in progress with a Cancel button.*

This dialog shows the optimizations regarding the corresponding batches. To abort the optimization click on button [Cancel].

#### Temporary Optimization

**Production Manager > tab Optimization manager > Details**

*Figure 1-82 shows the Temporary optimization dialog.*

This dialog shows the detailed view for an optimization variant.

**Description of the fields in section Rack**
*   **Batch number**, **Rack**, **Rack type**.

#### Optimization Overview

**Production Manager > tab Optimization Overview**

*Figure 1-83 shows the optimization overview.*

This dialog shows the optimizations which have been run for the individual glass types.

**Description of fields in section Selection Criteria**
*   **Optimization**, **Creation date**, **Batch number**.

**Description of the fields in section optimization**
*   **Optimization**, **Optimization mode**, **Creation date**, **Glass type**, **Cutting table**, **Batches**, **Status**, **Quantity**, **Surface**, **Result**.

#### Optimization Detailed View

**Production Manager > Optimization Overview Tab > Detailed View**

*Figure 1-84 shows the Optimization detailed view.*

This dialog shows the detailed view for an optimization. The content is identical to the *Temporary Optimization* dialog.

#### Output

**Production Manager > tab Output**

*Figure 1-85 shows the Output tab.*

All output is started from this tab. The dialog is accessible from the *Batch list* and *Optimization overview*.

**Description of fields**
*   **Batches section**: Shows details of the selected batch.
*   **Optimization section**: Shows details of the selected optimization.
*   **Reports section**: Lists available reports (**Name**, **Printer**, **Copies**, **Settings**, **Message**).
*   **Machine section**: Lists machines for code output (**Machine**, **Output**).

#### Printer Settings

**Production Manager > tab Output > Print Settings**

*Figure 1-86 shows the Printer settings dialog.*

This dialog is used to establish the settings for Labels, Cutting Plan, and Printer.

#### Search Order

**Information > Order**

*Figure 1-87 shows the Search order dialog.*

This dialog allows to search orders.

**Description of fields in section Selection Criteria**
*   **Order number**, **Number manager**, **Customer**.

## Section Index

### Index

#### A
*   Abort optimization

#### B
*   Batch
*   Batch overview
*   Batch creation
*   Batches

#### C
*   Criteria
*   Criterion
*   Cutting

#### D
*   Detailed view batch
*   Detailed view for batches
*   Display conventions
*   Documentation

#### E
*   Edit cutting
*   Enter rejects
*   Expert mode

#### F
*   Find order

#### G
*   Grouping

#### L
*   Logical rack

#### M
*   Machine load transfer
*   Master data
*   Module

#### N
*   Name of view
*   New batch

#### O
*   Optimization detailed view
*   Optimization manager
*   Optimization overview
*   Order selection
*   Output

#### P
*   Printer settings
*   Product

#### R
*   Rack group
*   Rack Organization
*   Racks
*   Rejects

#### S
*   Save view
*   Set batch status
*   Sorting key
*   Standard mode

#### T
*   Temporary optimization
