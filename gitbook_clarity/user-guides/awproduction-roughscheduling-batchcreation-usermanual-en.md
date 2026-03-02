---
description: "EN_UM_AWProduction_2"
---


# A+W Production Rough Scheduling

**A+W Software for Glass, Windows & Doors**

---
## Revision overview of the module

| Date | Change |
| :--- | :--- |
| 01-2023 | Search for document added. |
| 01-2017 | Product and company names adjusted. |
| 07-2014 | New tutorial and software reference. |
| 08-2013 | Complete revision of ALCIM documentation and adjustment to A+W Production |
| 03-2006 | Original version. |

This module provides information on the following subjects:
- Tutorial
- Software Reference

# Tutorial

## A+W Production Rough Scheduling

### This section provides information on the following subjects:
- Overview
- Rough Scheduling

### Table of Contents

*   **Overview**
    *   Tutorial structure
*   **Rough Scheduling**
    *   Production Scheduling Process
*   **Views**
    *   Views in Rough Scheduling
    *   Configure views, work with views
        *   Create and configure tabs
        *   Create and configure columns
        *   Create and configure totals row
        *   Define new column or totals row
        *   Create and configure filters
        *   White screen in a view
        *   Exercises: Configure views, work with views
*   **Orders / Pool**
    *   Orders in Rough Scheduling
*   **Buckets**
    *   Buckets in Rough Scheduling
*   **Batches and Batch Strategies**
    *   Batches in Rough Scheduling
*   **Items**
    *   Items in Rough Scheduling
    *   Search for document

## Overview

The tutorial on the **Rough Scheduling** process addresses the batch creation in A+W Production. With the different views in Rough Scheduling, the individuals responsible for the production scheduling process obtain an overview and create batches with different strategies that allow for an optimal production process.

> **The functions depend on the enabled modules**
> Please note that the individual functions are available only if the corresponding modules and interfaces have been installed and enabled.
> If you detect functions in this description which are not available in your version, please contact A+W Software GmbH.

### Required knowledge

This tutorial is meant for persons in charge of production scheduling in A+W Production who are responsible for organizing the optimum production process. Participants must be familiar with the master data concept in A+W Production.

### Tutorial structure

This tutorial consists of sets of topics with several training modules in each. Each module consists of the following elements:

*   **Overview**: Each training module starts with an overview of the major topics:
    *   Objectives: What shall be conveyed?
    *   Benefit: What can this knowledge be used for?
    *   Maxims: Which correlations are to be remembered?
*   **Concepts**: First, the concepts and terms of the corresponding training module will be explained. This is followed by examples and instructions.
*   **Exercises**: There are exercises featuring special tasks for some of the training sessions.
*   **Cross-references**: At the end of each training module there is a section with cross references pointing to additional information in the software reference and in other sections. This will help you to extend your newly acquired knowledge.

### Reading tip
The content of a training module is based on the knowledge conveyed in the previous module. We therefore recommend you do not skip any modules.
If you are already familiar with a subject, you should at least read the summary at the start of the module in order to bring the main details to mind.

## Rough Scheduling

This tutorial will show you which sections of A+W Production are part of Rough Scheduling and how you execute Rough Scheduling.
Different views (display dialogs) provide you with an overview and apply strategies to create batches.
The following chapters are included in Rough Scheduling:
- "Production Scheduling Process" on page C-108
- "Views" on page C-111
- "Orders / Pool" on page C-129
- "Buckets" on page C-132
- "Batches and Batch Strategies" on page C-138
- "Items" on page C-145

### Production Scheduling Process

[Image: Fig. C-1 Production scheduling process diagram showing flow from ERP System to Orders/Pool, then to Batch/Bucket (Status 100), Detailed Scheduling, Released for Production (Status 200), and finally Production (Status 300), with options to reset or resolve at various stages.]

The diagram above shows the production scheduling process including rough scheduling. After scheduling from the ERP system, the orders and/or items are included in the Pool, i.e. the Orders dialog. You can get an overview by using the overview dialogs and you can apply strategies to create batches. If you have created batches you can carry out Detailed Scheduling (rack allocation and optimization) and subsequently release them for production. The orders are shown in the views of production scheduling during the entire process. You can also track the statuses of individual orders.

If you resolve batches and buckets, they are returned to the pool. You can reset orders from a higher status and carry out new detailed scheduling or create new batches or buckets.

### Rough Scheduling and Capacity Planning

Some functions of Rough Scheduling interact with Capacity Planning. The corresponding points are referred to in this tutorial.

Capacity Planning provides you with a direct access point to Rough Scheduling; from within the Production Monitor you can open the Workplan dialog. Here you can create and manage batches and order items by taking the results of capacity planning into account. With active capacity planning we therefore recommend to start the steps of production scheduling from within the production monitor.

#### Set status
If you are working with capacity planning:
If you set the status or orders to produced, ready for shipment or delivered, capacity planning releases the capacities again. The respective functions are described in the Capacity Planning Manual.

### Terms in Rough Scheduling

The following terms are used in the description of Rough Scheduling.

| Term | Description |
| :--- | :--- |
| **Orders / Pool** | After the order data from the ERP system has been scheduled, the orders are listed in the Orders view which is also called Pool. |
| **Pool_tables** | The database tables Pool_ are filled with data during scheduling of the order data from the ERP system. Pool_tables describe the BOM and order header of a product. |
| **Bill of materials (BOM)** | The BOM shows the elements that are included in an order in a tree structure. The BOM also describes the interdependencies of the items. |
| **Item** | Items are parts of orders. An item includes different parts, e.g. float 4 mm and therm. 4 mm. The parts are subject to different kinds of processing, e.g. cutting or polishing. |
| **Processing** | Processing procedure with which the item is processed, e.g. polishing or grinding. |
| **Work process** | Work processes bring together the properties of processing, e.g. Polishing with the properties of the work piece. An item from the BOM, for example, includes the request to be polished in a certain way. Based on this request, the work process defines the special type of polishing. |
| **Release parts** | Parts that are explicitly to be planned for production. Release parts are shown in the views. Release parts are defined in the master data. |
| **Non-release parts** | Parts that are implicitly to be planned for production. Non-release parts are defined in the master data. |
| **Batch** | Group of orders and/or items that should be produced together. |
| **Bucket** | Repository or buffer in which you manage orders for which the further procedure is yet to be clarified. For example, you can keep orders in a bucket until there are enough items with the same glass type. Subsequently, you create a batch from this bucket or buckets. |
| **Lot** | Part of a batch that runs through the same production processes as a group. A lot can be created simultaneously on the same machine with the same tool. |
| **Start date** | Date when the production of a batch starts. |
| **Production date** | Assembly date of the head piece. |

## Views

**Objectives**
- What are views?
- How are views configured?
- How do you work with views?

**Benefits**
- Views provide you with an overview of orders and/or items.
- Views help you to decide on a batch strategy.
- With views you can see the status of orders or items.
- Edit the orders from within the views, e.g. by creating batches or buckets.

**Please note**
Views: Overview dialogs in which orders and/or items are displayed grouped by topic, e.g. by orders, processing or buckets.

### Views in Rough Scheduling

[Image: Fig. C-2 Screenshot of the Orders view in Rough Scheduling.]

The overview dialogs or views in rough scheduling are predefined so that you can directly work with them. You can create the orders and/or items from within the views, e.g. by creating batches or buckets. You control the dialogs mainly via context menus.

#### Configurable components
Most dialogs can be configured so that you can have exactly the information displayed that you need for your production. In this chapter you will learn how to work with overview dialogs and how to configure them.
The following components of the overview dialogs can be configured:
- Tab
- Columns
- Totals row
- Filter

The following dialogs are overviews and described in detail in the Software Reference:

*   **Orders dialog**: The Orders dialog provides you with an overview of all orders that have been scheduled but not yet processed. From this view you can further process the orders in the process of production scheduling, e.g. create batches and buckets. (⇨ "Orders" on page C-154)
*   **Order overview dialog**: The Order Overview dialog provides you with an overview of details in orders. You can sort the order overview by items, parts or processings. In addition, you can hide or show the spacers or foils. From the Order Overview dialog you cannot create batches or buckets. (⇨ "Order Overview" on page C-157)
*   **Filler order dialog**: The Filler Order dialog provides you with an overview of all filler orders. For example, you can use it to display how many items of the filler orders have already been produced and how many still have to be produced. (⇨ "Filler Orders" on page C-160)
*   **Bucket dialog**: The Buckets dialog provides you with an overview of buckets in AWP. You can sort the buckets by different criteria and edit them. (⇨ "Buckets" on page C-168)
*   **Reservation orders dialog**: Use the Reservation Orders dialog to display reservation orders. The dialog serves for overview purposes of scheduled capacities only; you cannot create any batches or buckets from the dialog. (⇨ "Reservation Orders Bucket" on page C-171)
*   **Purchase parts dialog**: The Purchase Parts Bucket dialog provides you with an overview of buckets that have been created with purchase parts. (⇨ "Purchase Parts Bucket" on page C-175)
*   **Batches dialog**: The Batches dialog provides you with an overview of the created batches. (⇨ "Batches" on page C-182)
*   **Items dialog**: The Items dialog provides you with an overview of items in the orders. (⇨ "Items" on page C-193)
*   **Processing dialog**: The Processing dialog provides you with an overview of processings in the orders. (⇨ "Processings" on page C-203)
*   **Glass Types dialog**: Use the Glass Types dialog to display an overview of the included glass types for selected orders or items and to create a batch. (⇨ "Glass Types" on page C-208)
*   **Details dialog**: Use the Details dialog to view details on selected orders, items, parts, batches or buckets. You can open the Details dialog from any view in Rough Scheduling; it is therefore recommended that you configure this view optimally. (⇨ "Details" on page C-211)
*   **Barcoding dialog**: The Barcoding dialog provides you with an overview of information relating to production data collection. (⇨ "Barcoding" on page C-215)
*   **Lots dialog**: The Lots dialog provides you with an overview of the created lots of the selected batches. (⇨ "Lots" on page C-219)
*   **Work Plan dialog**: Use the Work Plan dialog to obtain an overview from within the production monitor view. The work plan shows you all the planned batches on a machine or in a shift. (⇨ "Work Plan" on page C-223)

### Configure views, work with views
You can configure views to meet your demands. Compile the most important information on the first tab of a dialog and let other information follow on other tabs. Use the views to show as much information as required and as little as possible to keep dialogs clearly arranged. Add totals rows in order to obtain a faster overview. Use filters for specific applications.

#### Create and configure tabs
Please see the following instructions concerning inserting and configuring tabs:
- "How to insert a tab" on page C-115
- "Configuring a tab" on page C-116

**How to insert a tab**
1.  Open the view in which you would like to insert a tab, e.g. `Display > Orders`.
2.  Open the context menu of the tab next to which the new tab shall be inserted. Or open the context menu in the head section of the dialog if no tabs exist yet.
    [Image: Fig. C-3 Orders - Tab context menu showing options like Save, Insert, Delete, Properties.]
3.  Click **Insert** in the context menu.
    [Image: Fig. C-4 Screenshot of the 'Properties of (tab)' dialog with fields for Tab Text and Description.]
    The **Properties of (tab)** dialog opens in which you provide the tab with a tab text and description. With the **System-wide Display** checkbox you can define whether the tab is displayed to all users or just to you.
    The new tab is inserted next to the tab, the context menu of which you have opened. You can move a tab by dragging it with the cursor to the required location.

**Configuring a tab**
1.  Open the view which you would like to configure, e.g. `Display > Orders`.
2.  Open the context menu of the tab you would like to edit.
3.  The options are:
    *   Click **Autosave** to automatically save all changes to the respective tab. If you do not select Autosave you must click **Save** after every change to the tab so that all the changes are adopted.
        [Image: Fig. C-5 Orders - Enabled autosave. A pound sign '#' next to the tab name indicates Autosave is on.]
    *   The pound sign next to the name of the tab shows that Autosave has been enabled.
    *   Click **Properties** in the context menu of the tab in order to edit the properties of a tab. The **Properties of (tab)** dialog opens. Here you can edit the tab text and description. With the System-wide Display checkbox you can define whether the tab is displayed to all users or just to you.
    *   You can import or export the configured tab and thus use it as a template for other dialogs or users.

#### Create and configure columns
Please see the following instructions concerning inserting and configuring columns:
- "How to insert a column" on page C-117
- "How to configure a column" on page C-118

**How to insert a column**
1.  Open the view in which you would like to insert a column, e.g. `Display > Orders`.
2.  Open the context menu of the column next to which the new column shall be inserted.
    [Image: Fig. C-6 Orders - Column context menu showing Insert options for different data categories.]
3.  Click **Insert** in the context menu. Different categories are available for selection. The new column is inserted next to the column, the context menu of which you have opened.

**How to configure a column**
1.  Open the view in which you would like to configure a column, e.g. `Display > Orders`.
2.  Open the context menu of the column you would like to edit.
3.  The options are:
    *   Click **Resort** to sort the respective columns in the reverse order, e.g. by ascending or descending date.
    *   Click **Format** in the context menu of a column in order to assign a unit to the column, e.g. information in millimeters. Different categories are available for selection.
    *   Click **Display Definition** in the context menu of a column in order to show details concerning the column.
        [Image: Fig. C-7 Screenshot of the 'Column Definition' dialog showing Title, Format, Info, Menu, and SQL Def fields.]
    *   You can move a column by dragging it to the required location.

> **Colors in columns**
> Please contact the Customer Service of A+W Software GmbH if you want to assign colors to the columns in views.
> An entry in the database is required to show columns in different colors.

**How to use the list**
1.  Open the view with which you would like to work, e.g. `Display > Orders`.
2.  Open the context menu of the list.
    [Image: Fig. C-8 Orders - List context menu showing options like Create Batch, Create Bucket, Order Overview, etc.]
3.  Select an option from the list. The context menus are described in the Software Reference.

#### Create and configure totals row
Please see the following instructions concerning inserting and configuring totals rows:
- "How to insert a totals row" on page C-119
- "How to configure a totals row" on page C-120

**How to insert a totals row**
1.  Open the view in which you would like to insert a totals row, e.g. `Display > Orders`.
2.  Open the context menu of the totals row next to which the new totals row shall be inserted. Or open the context menu in the field of the totals rows if no totals row exists yet.
    [Image: Fig. C-9 Orders - Totals row context menu.]
3.  Select a filter criterion, e.g. **Total sum pieces**.
    The totals row is inserted. Any additional totals row is inserted after the totals row in the context menu which you have opened.

**How to configure a totals row**
1.  Open the view in which you would like to configure a totals row, e.g. `Display > Orders`.
2.  Open the context menu of the totals row you would like to configure.
3.  The options are:
    *   Click **Format** in order to assign a unit to the totals row, e.g. information in millimeters. Different categories are available for selection.
    *   Select **Display Definition** in the context menu in order to show settings for the totals row.

#### Define new column or totals row

**How to define columns or totals rows**
1.  Open the view in which you would like to insert a column or totals row, e.g. `Display > Orders`.
2.  Open the context menu or a column or totals row.
    [Image: Fig. C-10 Orders - Column context menu with Insert > Field Definitions > Edit highlighted.]
3.  Click **Insert > Field Definitions > Edit** in the context menu.
    The **Field Definition** dialog opens.
    [Image: Screenshot of Field Definition dialog.]
4.  Select the group in the context menu to which the column or totals row is assigned to in the **Menu Group** field, e.g. **Accumulated parts**.
5.  Enter a name for the column or totals row in the **Menu Entry** field, e.g. **Finished parts**.
6.  In the field **Column Header**, enter the name for the column or totals row with which it shall be displayed in the dialog, e.g. **Finished parts_all**.
7.  In the **Description** line, enter a description for the column or totals row, e.g. **Shows all finished parts**.
8.  With the button **Format** you select the format for the column or totals row, e.g. **Text**.
9.  With the button **Open Selection** you select an SQL printout that is stored for the column or totals row. Select the entry **SQL printout** to enter an individual SQL printout.
    [Image: Screenshot showing SQL printout selection.]
10. Select the display options for the column or totals row, e.g. whether the sorting of data should be in ascending or descending order.
11. Click on **[Save]** to adopt the changes.
12. Click on **[Close]** to close the dialog.
    The new column or totals row **Finished Parts** is now available in the context menu.
    [Image: Context menu showing the newly added 'Finished Parts' column option.]

#### Create and configure filters
Please see the following instructions concerning selecting, inserting, configuring and defining filters:
- "How to select a filter" on page C-124
- "How to add a filter" on page C-125
- "How to configure filters or define new filters" on page C-125

**How to select a filter**
1.  Open the view in which you would like to select a filter, e.g. `Display > Orders`.
2.  Open the dropdown menu of a filter in order to select a filter.
    [Image: Fig. C-11 Orders - Filter dropdown menu showing a list of available filters.]
3.  Select a filter. Now the view is filtered.

**How to add a filter**
1.  Open the view in which you would like to add a filter, e.g. `Display > Orders`.
2.  Click **[Add filter]** in order to add a filter. A new filter dropdown is added.

**How to configure filters or define new filters**
1.  Open the view in which you would like to configure or define filters, e.g. `Display > Orders`.
2.  Open the context menu of the filter you would like to configure or after which you would like to add a new filter. The **(Filter Name)** dialog opens.
3.  Click on **[Manage]**. The **Filter Definition** dialog opens.
    [Image: Screenshot of Filter Definition dialog.]
4.  Select a filter from the list if you want to configure it or select **New Filter** from the list if you want to define a new filter.
5.  Edit the name of the filter in the **Name** field, e.g. **only IG**.
6.  Enter a description for the filter in the **Description** field, e.g. **Shows only IG orders**.
7.  Define a default value in the **Standard Parameters** field, e.g. default date.
8.  In the **Valid for Display** field, select the views in which the filter is shown, e.g. **Pool view**, **Bucket view** and **Batch view**.
9.  Click on **[Save]** to save the changes or the new filter.
    Now you have configured or created the filter and it is available in the respective views. You can export or import the filters with the buttons **[Export]** or **[Import]** and thus use them as templates for other dialogs or users.

### White screen in a view
If a view does not display any orders and/or items, then either there are none available or you have set the criteria of the view in a manner that no orders or items meet the criteria. Examples of possible reasons for blank lists:
-   **There is only one column in the view.** A category has been defined for this column that is not included in the orders. For example, the column shows LAMI, but the orders do not include any LAMI.
    *   **Remedy:** Define a criterion in the column that corresponds to the orders.
-   **There are several columns in the view.** The criteria of the columns restrict the orders so much that none are shown or the criteria are contradictory. For example, you have two columns, one showing LAMI and the other IG. Orders that only include LAMI or IG cannot meet both criteria.
    *   **Remedy:** Define criteria in the columns that correspond to the orders.
-   **You have activated a filter,** the criterion of which does not correspond to any order. For example, the list is blank if the filter **only IG** is activated and no IG is included in the orders.
    *   **Remedy:** Remove the filter or select a different one.
-   **You have added a column that filters for batch-related information.** If you have not yet created a batch for the displayed orders or items, the column filters non-existing data and the result is a white screen.
    *   **Remedy:** Add columns for later work processes in production scheduling only to those views that show later processes, e.g. batch-related data in the batch view.

### Exercises: Configure views, work with views
The following exercises shall help to strengthen your newly acquired knowledge.
- Open a view in Rough Scheduling.
- Enable autosave.
- Review which information is missing in this view.
- Create a corresponding tab.
- Create pertaining columns.
- Insert a totals row.
- Add a filter.
- Define an individual column and/or totals row and insert it into the view.

**Additional information**
⇨ Software Reference, "Rough Scheduling" on page C-152

## Orders / Pool

**Objectives**
- How do you work with the Orders view?

**Benefits**
- The Orders view provides you with an overview of all the orders that have been scheduled from the ERP system.
- In the Orders view you can order other views.

**Please note**

| Term | Description |
| :--- | :--- |
| **Orders** | After import from the ERP system, orders are shown in the Orders dialog. |
| **Pool** | The Orders dialog is also called Pool. |
| **Order overview** | The order overview shows the BOM. |
| **Items** | The Items dialog provides you with all details concerning items in the orders. |
| **Filler orders** | Filler orders are not assigned to any batch and are used by Detailed Scheduling to optimize waste. |
| **Surplus** | Edit business- and production-related surpluses in the Surplus Editor. (⇨ Software Reference, "Surplus Editor" on page C-163) |
| **Change procurement type** | In the Modification of Procurement Type dialog you can change the procurement type from TG to LAMI. (⇨ Software Reference, "Change of Procurement Type" on page C-165) |

### Orders in Rough Scheduling

[Image: Fig. C-12 Screenshot of the Orders dialog.]

The **Orders** dialog provides you with an overview of all orders that have been scheduled but not yet processed. From this view you can further process the orders in the process of production scheduling, e.g. create batches and buckets. The Orders dialog is also called **Pool**.

Resolved batches and buckets are automatically returned to the Pool. The Orders dialog can be configured.

In the Pool you can open the **Order Overview**, in which the BOM is shown. You can open the **Surplus Editor**, in which you can edit production- and business related surpluses.
In addition, you can access Rescheduling to Other Machines and Machine Allocation from the Pool.

The Orders dialog is intended to provide you an overview of the delivery data, products and processings that are included in the orders. Keep the Orders dialog as simple and clearly arranged as possible. If you have scheduled orders, they are no longer shown in the Pool. You will find the scheduled orders in other views, e.g. in the Batches dialog. Create a tab in the Orders dialog in which you will find the customer data, e.g. delivery names, delivery addresses and routes.

> **Rescheduling to other machines, machine allocation and capacity planning**
> If you are working with capacity planning you must take the following into account:
> A new rescheduling to another machine or machine allocation from within Rough Scheduling will affect the planned and calculated capacities.
> The respective functions are described in the Capacity Planning Manual.

#### Orders with faulty information
With respect to orders with missing or faulty information you can either edit the faulty items or the entire order. Either you delete the respective orders or items or you move them back to the pool.
Delete faulty items from batches to ensure that they do not remain in the system.

## Buckets

**Objectives**
- What is a bucket?
- How do you work with the Buckets view?
- How to create a bucket?

**Benefits**
- Buckets help you to keep an overview of orders that are not immediately further processed.
- You can create buffers with buckets, e.g. by collecting orders of the same type.

**Please note**

| Term | Description |
| :--- | :--- |
| **Bucket** | A bucket is a repository in which you manage orders for which the further procedure is yet to be clarified. |
| **Resolve bucket**| Orders from resolved buckets are returned to the pool. |

### Buckets in Rough Scheduling

[Image: Fig. C-13 Screenshot of the Buckets dialog.]

The **Buckets** dialog provides you with an overview of all buckets in Rough Scheduling. A bucket is a repository or buffer in which you manage orders for which the further procedure is yet to be clarified. This could be the case, for example, if you are waiting for order changes or additional panes made of high-cost glass type.

You can create buckets from almost all overviews or assign orders to existing buckets. The created buckets are then moved to the Buckets dialog. From here, you can manage the buckets, e.g. by creating batches or resolving buckets. Orders from resolved buckets are returned to the **Pool**.

For details on how to work with buckets, please see the following instructions:
- "How to create a bucket" on page C-134
- "How to add orders to an existing bucket" on page C-135
- "How to resolve a bucket" on page C-137

#### How to create a bucket
1.  Open the view in which you would like to create a bucket, e.g. `Display > Orders`.
2.  Open the context menu of the orders from which you would like to create a bucket and select **Create bucket**.
    The **Create Bucket** dialog opens.
    [Image: Fig. C-14 Screenshot of the Create Bucket dialog.]
3.  Select the bucket type in the **Bucket Type** dropdown menu.
4.  AWP creates a new bucket in the **Bucket** field. Adopt this name or rename it.
5.  Select the production start in the **Production Date** calendar field. Please note that a modified production date affects capacity planning.
6.  In the **Production Shift** field, enter the shift in which production shall be started. Please note that a modified shift affects capacity planning.
7.  In the **Article Type Filter** field, select whether an article type filter is defined for the bucket.
8.  Select with the **Keep Order Together** checkbox whether the order should be kept together in production.
9.  Click on **[OK]** to save the data.
    The bucket has been created and is listed in the **Buckets** view.

#### How to add orders to an existing bucket
1.  Open the view in which you would like to add orders to a bucket, e.g. `Display > Orders`.
    [Image: Fig. C-15 Screenshot of the Orders list context menu.]
2.  Open the context menu of the orders that you would like to add to a bucket and select **Create Bucket**. The **Create Bucket** dialog opens.
    [Image: Screenshot of the Create Bucket dialog.]
3.  Select the bucket type in the **Bucket Type** dropdown menu.
4.  Select an existing bucket in the **Bucket** field in order to add the orders to a bucket.
5.  Select the production start in the **Production Date** calendar field. Please note that a modified production date affects capacity planning.
6.  In the **Production Shift** field, enter the shift in which production shall be started. Please note that a modified shift affects capacity planning.
7.  In the **Article Type Filter** field, select whether an article type filter is defined for the bucket.
8.  Select with the **Keep Order Together** checkbox whether the order should be kept together in production.
9.  Click on **[OK]** to save the data. The orders have been added to the bucket.

#### How to resolve a bucket
1.  Select `Master Data Display > Buckets`.
2.  Open the context menu of the bucket or buckets you would like to resolve and select **Resolve Bucket**.
    The orders have been returned to the **Pool**.
    [Image: Fig. C-16 Screenshot of the Buckets list context menu with 'Resolve Bucket' selected.]

## Batches and Batch Strategies

**Objectives**
- What is a batch?
- How do you work with the Batches view?
- How to create a batch?
- Which strategies are available to schedule a batch?

**Benefits**
- The Batches view provides you with an overview of all the created batches.
- The Batches view displays the status of the batches.
- In the Batches view you can manage batches e.g. by setting a status, resetting or resolving batches.
- In the Batches view you can transfer batches to Detailed Scheduling.

**Please note**
**Batches**: Batches are a grouping of orders and/or items that are to be processed together in the process of production preparation and production release. Rough scheduling, detailed scheduling, optimization and batch release are executed on the basis of the batches.

### Batches in Rough Scheduling

[Image: Fig. C-17 Screenshot of the Batches dialog.]

The **Batches** dialog provides you with an overview of all created batches. From this view, you can further process the batches in the process of production scheduling, e.g. by linking or resolving batches or transferring them to Detailed Scheduling.

Batches are a grouping of orders and/or items that are to be processed together in the process of production preparation and production release. Detailed scheduling, optimization and batch release are executed on the basis of the batches.

Resolved batches are automatically returned to the **Pool**. The Batches dialog can be configured. For example, you can access Rescheduling to Other Machines from the Batches dialog.

> **Rescheduling to other machines, machine allocation and capacity planning**
> If you are working with capacity planning you must take the following into account:
> A new rescheduling to another machine or machine allocation from within Rough Scheduling will affect capacity planning.
> The respective functions are described in the Capacity Planning Manual.

#### Useful batches and batch strategies
The following applies in general: A batch strategy is good if it works. If you mix different pane sizes into a batch, the yield is improved. Do not isolate special products, but include special products in the batches.

You can pursue the following batch strategies:
-   **By glass type**: You can create separate batches with thick glass panes. Thick glasses are usually larger in size and thus result in a worse yield; it may therefore be beneficial to create separate batches and produce thick glass when it fits best into production.
-   **By product type**: In the case of more complex productions, e.g. IG, TG or LAMI, it may be beneficial to compile product types in batches. You will get a better overview of production and accept a lower yield.
-   **By processing**: You can compile orders or items to batches on a processing-oriented basis, e.g. to minimize set-up costs and times.
-   **By production date**: Capacity planning assigns production dates to the individual processings. You can use those as a basis and create batches from the respective processings with the same date.
-   **By order and/or item**: You can create batches from items or individual elements of orders. In the case of multi-step productions, this strategy will help you to organize the individual departments. If you need space for changes you can distribute different product types of an order to several batches.
-   **Schedule in several stages**: Here, you separate orders and/or items by your main criteria and check the result. Depending on the yield, quantity, residual plates and number of required racks, you separate parts into individual batches and add parts to the batches.
-   **Empty pool**: With this strategy you pack new orders and/or items into buckets or batches as fast as possible. The advantage of this strategy is that you see new orders and/or items immediately when they are moved to the pool. The disadvantage is that it is more difficult to keep track of existing buckets and batches.
-   **Full pool**: You keep orders and/or items in the pool as long as possible. The advantage of this strategy is that you completely keep track. The disadvantage is that it is more difficult for you to notice new orders and/or items.

> **Careful with batch strategies**
> A+W Production gives you complete freedom in planning your production and consequently full responsibility.
> For example, you can ignore results of capacity planning.

You should not use the following batch strategies:
-   Using today's small sizes to increase today's yield. This strategy results in problems on the following day.
-   Mixing too many products or glass types into the batches without appropriate organization. This strategy results in an unclear production process and jams.
-   Default glass quantity too small.
-   Delete batches to accept order modifications. It is better to move items or batches back to the pool.

For details on how to work with batches, please see the following instructions:
- "How to create a batch" on page C-141
- "How to add orders to an existing batch" on page C-142
- "How to manage batches or resolve batches" on page C-144

#### How to create a batch
1.  Open the view in which you would like to create a batch, e.g. `Display > Orders`.
2.  Open the context menu of the orders from which you would like to create a batch and select **Create batch**.
    The **Create Batch** dialog opens.
    [Image: Fig. C-18 Screenshot of the Create Batch dialog.]
3.  AWP automatically creates a new batch number in the **Batch** field.
4.  Enter the description for the batch in the **Description** field.
5.  Select the production start in the **Production Date** calendar field. Please note that a modified production date affects capacity planning.
6.  In the **Production Shift** field, enter the shift in which production shall be started. Please note that a modified shift affects capacity planning.
7.  In the **Article Type Filter** field, select whether an article type filter is defined for the batch.
8.  Select with the **Keep Order Together** checkbox whether the order should be kept together in production.
9.  Click on **[OK]** to save the data.
    The batch has been created and is listed in the **Batches** view.

#### How to add orders to an existing batch
1.  Open the view in which you would like to add orders to a batch, e.g. `Display > Orders`.
2.  Open the context menu of the orders that you would like to add to a batch and select **Create Batch**.
    The **Create Batch** dialog opens.
    [Image: Fig. C-19 Screenshot of the Create Batch dialog.]
3.  Select an existing batch in the dropdown menu in order to add the orders to a batch.
4.  Enter the description for the batch in the **Description** field.
5.  Select the production start in the **Production Date** calendar field. Please note that a modified production date affects capacity planning.
6.  In the **Production Shift** field, enter the shift in which production shall be started. Please note that a modified shift affects capacity planning.
7.  In the **Article Type Filter** field, select whether an article type filter is defined for the batch.
8.  Select with the **Keep Order Together** checkbox whether the order should be kept together in production.
9.  Click on **[OK]** to save the data.
    The orders have been added to the batch.

#### How to manage batches or resolve batches
1.  Select `Display > Batches`.
2.  Open the context menu of the batch or batches you would like to edit or resolve and select the corresponding option in the context menu.
    The batch or the orders can now be seen in the corresponding views.
    [Image: Fig. C-20 Batches - List context menu with options like Release Batch, Reset Batch, Resolve Batch.]

## Items

**Objectives**
- What are items?
- How do you work with the Items view?

**Benefits**
- The Items view provides you with an overview of all the items in orders.

**Please note**
**Items**: Items are parts of orders.

### Items in Rough Scheduling

[Image: Fig. C-21 Screenshot of the Items dialog showing a tree view of orders and items, and their properties.]

The **Items** dialog provides you with an overview of items of scheduled orders. The Items dialog can be configured. However, you cannot create batches or buckets from within the view.

Items are parts of orders. An item includes different parts, e.g. float 4 mm and therm. 4 mm. The parts are subject to different kinds of processing, e.g. cutting or polishing.

#### Split items
The **Split Items** dialog is used for splitting order items by different criteria. You can divide items into additional items or create items that include a certain number of panes. You can furthermore divide items in accordance with packaging optimization.

**How to split an item**
1.  Select `Display > Orders > Context menu on selected orders> Processings > Context menu > Split items`.
2.  Select the items (A) you want to split in the list **Selected Items**.
    [Image: Screenshot of the Split Items dialog, showing 'Selected Items' and 'New Items' lists, and splitting options.]
3.  Select the option (B) with which you want to execute splitting.
4.  Click on **[Split]**. The items have been split and are listed in the **New Items** field.
5.  Click on button **[End]** to close the dialog.

### Search for document
`Processing > Search for document`

[Image: Fig. C-22 Screenshot of the 'Search for document' dialog.]

Here, you can search the system for orders and/or quotations. When you open the dialog, it is empty. Content is only displayed after you have made the appropriate selections and pressed the **Display** button.

In the first step, in the **Search by document type** area, you specify whether you want to search for an order, a quotation or both when searching.

Then, in the **Search for ...** area, you must enter the appropriate document number (for order or quotation) or the desired customer number.

In the **Display by** area, you can select whether the display should be sorted by document number and item or by batches.

In the **Display from ...** area, you have another opportunity to subdivide the content displayed. For example, you can use the **Parts** radio button to display the appropriate parts numbers. The **Batch** radio button shows you the entire batch.

# Software Reference

## A+W Production Rough Scheduling

### This section provides information on the following subjects:
- Rough Scheduling
- Orders in Rough Scheduling
- Buckets in Rough Scheduling
- Batches in Rough Scheduling
- Items in Rough Scheduling
- Processings in Rough Scheduling
- Glass types, Details, Barcoding and Lots
- Overlapping Dialogs
- Overlapping Context Menus

### Table of Contents

*   **Rough Scheduling**
*   **Orders in Rough Scheduling**
    *   Orders
    *   Order Overview
    *   Filler Orders
    *   Surplus Editor
    *   Change of Procurement Type
*   **Buckets in Rough Scheduling**
    *   Buckets
    *   Reservation Orders Bucket
    *   Purchase Parts Bucket
    *   Bucket Creation
    *   Edit bucket description
*   **Batches in Rough Scheduling**
    *   Batches
    *   Batch creation
    *   Create Special Glass Batch
    *   Edit Batch Description
    *   Release of Batch (Name): AUW – Repetition
*   **Items in Rough Scheduling**
    *   Items
    *   Add Order to Items
    *   Split Items
    *   Field Definition
    *   Export/Import Item View
*   **Processings in Rough Scheduling**
    *   Processings
    *   Change Default Times
*   **Glass types, Details, Barcoding and Lots**
    *   Glass Types
    *   Details
    *   Barcoding
    *   Lots
*   **Overlapping Dialogs**
    *   Work Plan
    *   Properties of (tab)
    *   Column Definition
    *   (Filter Name)
    *   Filter Definition
    *   Links to Documents
    *   Edge Deletion
*   **Overlapping Context Menus**

## Rough Scheduling

In Rough Scheduling you create batches that you subsequently plan in detail and optimize in the process of production preparation. The size and composition of the batch is decisive for the optimization results and production capacity utilization.

After scheduling the orders, you will find them in the Orders dialog, also called Pool. From here you are able to presort the orders into buckets or create batches directly. The different views help you to obtain an overview of the order data and details. From the views you create batches and transfer these to the next process step in production scheduling: detailed scheduling.

You can adjust the views of Rough Scheduling to your demands so that they show exactly the information that you require.

## Orders in Rough Scheduling
This chapter provides you with information on all the dialogs with which you can get an overview of orders or order data. You can manage filler orders and process surplus quantities.

The chapter covers the following topics:
- "Orders" on page C-154
- "Order Overview" on page C-157
- "Filler Orders" on page C-160
- "Surplus Editor" on page C-163

### Orders
**Display > Orders**
⇨ Processings

[Image: Fig. C-23 Orders - Totals (Example) screenshot.]

The **Orders** dialog provides you with an overview of all orders that have been scheduled but not yet processed. From this view you can further process the orders in the process of production scheduling, e.g. create batches and buckets and show order details from different perspectives. The **Orders** dialog is also called **Pool**.

You can configure the following components of the Orders dialog as you like:
- Tab
- Columns
- Totals row
- Filter

You control this dialog mainly via context menus.

The **Totals** tab includes the following columns, for example:
- **Delivery date**: Delivery date for the order.
- **TG pc**: Number of TG included in the order.
- **Shp pc**: Number of shapes included in the order.
- **Muntin pc**: Number of muntins included in the order.
- **Muntins produced**: Number of muntins already produced for the order.
- **Muntins purchased**: Number of muntins already purchased for the order.
- **Qty. triple**: Quantity of triple IG included in the order.
- **Qty. stepped IG**: Quantity of stepped IG included in the order.

> **Database information from columns**
> You can open the **Column definition** dialog by right-clicking on a column and selecting the option **Show definition**. In the Column definition dialog you will find the respective database information of a column.
> ⇨ "Column Definition" on page C-227

#### Totals row
- **Qty final product**: Quantity of selected final products, e.g. IG or LAMI.
- **IG pc**: Quantity of selected IG if multiple selection.
- **only cutting**: Total of all lites that must be cut.

#### Filter
- **[Add filter]**: Adds a filter.
- **Drop-down menu**:
    - Click: Opens the drop-down menu from which you select a filter.
    - Right-click: Opens the dialog (Filter Name). The Manage button opens the Filter Definition dialog in which you edit the respective filter.
    ⇨ "Filter Definition" on page C-229

#### Context menus
Context menus are offered in the following sections of the **Orders** dialog:
- Tab
- Columns
- List
- Totals row
- Filter

Context menus that appear in the entire area of production scheduling are listed in the chapter Overlapping Context Menus. (⇨ "Overlapping Context Menus" on page C-234)

| Group | Path | Remark |
| :--- | :--- | :--- |
| List | Work schedule > Machinery reallocation | Opens the Rescheduling dialog to reschedule to other machines. ⇨Capacity Planning: Software Reference, "Machine Reallocation" on page E-610. The results of the machine allocation within the scope of scheduling are overwritten. |
| | Work schedule > Machinery reallocation | Carries out the machine allocation for selected orders again. The results of the machine allocation within the scope of scheduling are overwritten. |
| | Work plan > Recalculate work plan | Currently not being used. |
| | Change procurement type | Opens the Change procurement type dialog. ⇨ "Change of Procurement Type" on page C-165. The option only works with TG and LAMI. |

#### Buttons
- **[Batch]**: Creates a batch from selected orders, items or parts.
- **[Glass types]**: Shows the glass types for the selected orders.
- **[Details]**: Shows the details for the selected orders.

### Order Overview
*   Display > Orders > Context menu > Processings > Context menu > Order Overview
*   Display > Orders > Context menu > Glass types > Context menu > Order Overview
*   Display > Orders > Context menu > Details > Context menu > Order Overview
*   Display > Buckets > Context menu > Order Overview
*   Display > Batches > Context menu > Order Overview
*   Display > Filler orders > Context menu > Order Overview

[Image: Fig. C-24 Order Overview, sorted by processings (example).]

The **Order Overview** dialog provides you with an overview of details in orders. You can sort the order overview by items, parts or processings. In addition, you can hide or show the spacers or foils.

From the **Order Overview** dialog you cannot create batches or buckets.

In the **Order Overview** dialog you can adapt tabs and columns to fit your needs so that exactly the required information is shown. You control this dialog mainly via context menus.

- **[Autosave]**: Activates automatic saving.
- **[Save]**: Saves the current data.
- **[System-wide display]**: Changes in the Order Overview dialog are saved system-wide.

The Order Overview dialog includes the following information, for example:
- **Order**: Order for which the details are shown.
- **[Items]**: Sorts the view by items.
- **[Parts]**: Sorts the view by parts.
- **[Processings]**: Sorts the view by processings.
- **Show spacers, foils**: Checkbox (If checked, processings that include spacers and foils are shown. If unchecked, they are not shown).
- **Item**: Item number of the order item.
- **Name**: Article or order item.
- **Size**: Size of the lites.
- **Quantity**: Number of articles.
- **Machine**: Machine used for this processing.
- **Prod. Date**: Date when this processing will be executed.
- **Prod. Quantity**: Number of lites already produced.
- **Batch**: Batch allocated to the processing.
- **Procurement type**: Procurement type allocated to the article.
- **Shape number**: Shape number of the lite.
- **Processing text**: Remarks about the processing.

> **Database information from columns**
> You can open the **Column definition** dialog by right-clicking on a column and selecting the option Show definition. In the Column definition dialog you will find the respective database information of a column.
> ⇨ "Column Definition" on page C-227

#### Context menus
Context menus are offered in the following sections of the Order Overview dialog:
- Button bar
- Header
- Columns

| Group | Path | Remark |
| :--- | :--- | :--- |
| Header | Formatting | Select format or unit for the columns in the header, e.g. date format or length unit. |
| | Insert | Inserts a new column in the header. Different categories are available. |
| | Delete | Deletes a selected column. |
| | Display definition | Opens the Column Definition dialog. ⇨ "Column Definition" on page C-227 |
| Columns | Formatting | Select format or unit for the columns in the list, e.g. date format or length unit. |
| | Insert > Processing data | Inserts a new column with processing data. Different categories are available. |
| | Insert > BOM data | Inserts a new column with BOM data. Different categories are available. |
| | Delete | Deletes a selected column. |
| | Display definition | Opens the Column Definition dialog that shows details concerning the respective column. ⇨ "Column Definition" on page C-227 |

### Filler Orders
**Display > Filler orders**

[Image: Fig. C-25 Filler orders (example) screenshot.]

The **Filler Order** dialog provides you with an overview of all filler orders. For example, you can use it to display how many items of the filler orders have already been produced and how many still have to be produced.

You can configure the following components of the Filler Orders dialog as you like:
- Tab
- Columns
- Totals row
- Filter

The Filler Order dialog includes the following columns, for example:
- **Order**: Order number for the corresponding order.
- **Itm (int Itm)**: Internal A+W Production sub-item, assigned, for example, after an item split.
- **Article description**: Name of the article included in the order.
- **Produced quantity**: Number of already produced items in the corresponding order.

> **Database information from columns**
> You can open the Column definition dialog by right-clicking on a column and selecting the option Show definition.
> ⇨ "Column Definition" on page C-227

#### Totals row
- **Qty final product**: Quantity of selected final products, e.g. IG or LAMI.
- **IG pc**: Quantity of selected IG.
- **only cutting**: Number of selected lites that must be cut.

#### Filter
- **[Add filter]**: Adds a filter.
- **Drop-down menu**:
    - Click: Opens the drop-down menu from which you select a filter.
    - Right-click: Opens the dialog (Filter Name). The Manage button opens the Filter Definition dialog.
    ⇨ "Filter Definition" on page C-229

#### Context menus
Context menus are offered in the Filler Orders dialog, including Tab, Columns, List, Totals row, and Filter. Context menus that appear in the entire area of production scheduling are listed in the chapter Overlapping Context Menus.
⇨ "Overlapping Context Menus" on page C-234

| Group | Path | Remark |
| :--- | :--- | :--- |
| List | Work schedule > Machinery reallocation | Opens the Rescheduling dialog to reschedule to other machines. ⇨Capacity Planning: Software Reference, "Machine Reallocation" on page E-610 |
| | Work schedule > Machinery reallocation | Carries out the machine allocation for selected orders or items again. |
| | Work plan > Recalculate work plan | Currently not being used. |
| | Change procurement type | Opens the Change procurement type dialog. ⇨ "Change of Procurement Type" on page C-165. The option only works with TG and LAMI. |

#### Buttons
- **[Batch]**: Creates a batch from selected orders, items or parts.
- **[Glass types]**: Shows the glass types for the selected orders.
- **[Details]**: Shows the details for the selected orders.

### Surplus Editor
**Display > Orders > Context menu > Reentry > Surplus**

[Image: Fig. C-26 Surplus Editor screenshot.]

Use the Surplus Editor to edit business- and production-related surpluses in orders.

#### Order items
- **Order**: Number of order.
- **Itm**: Number of items included in the order.
- **Product**: Product name from the product master data.
- **Quantity according to order**: Quantity specified in the purchase order.
- **Surplus**: Business-related surplus that can be changed if required.
- **Excess Quantity**: Production-related excess quantity that can be changed if required.
- **Total quantity**: Total quantity of the items after you changed the surpluses and excess quantities.

#### Overview
Display of the lite structure.

#### Shape
Display of the selected product's shape.

#### Buttons
- **[Save]**: Saves the data.
- **[Close]**: Closes the dialog without saving the data.

### Change of Procurement Type
*   Display > Orders > Context menu > Change procurement type
*   Display > Filler order > Context menu > Change procurement type

[Image: Fig. C-27 Modification of procurement type screenshot.]

In the **Modification of Procurement Type** dialog you can change the procurement type from TG to LAMI.

#### Modifiable parts
List of parts for which you can change the procurement type.

#### Details
- **Order number**: Order number of the selected part.
- **Item number**: Item number of the selected part.
- **Article description**: Description of the selected part.
- **Pcs**: Number of parts included.
- **Production date**: Start of production of parts.
- **Current procurement type**: Currently defined procurement type.
- **Structure**: Lites included for which you can change the procurement type.

- **[Arrow down]**: Moves selected parts to the **Selected Parts** field.
- **[Arrow up]**: Moves selected parts back to the **Modifiable Parts** field.

#### Selected parts
List of selected parts.

#### Selection of new procurement type
Selection of new procurement type. Select from **Cutting, Production, P.O.** or **Stock Withdrawal**.

- **[Execute]**: Executes the change of the procurement type.
- **[Close]**: Closes the dialog without saving the data.

## Buckets in Rough Scheduling
This chapter provides you with information on all the dialogs with which you can get an overview of buckets. You can create and edit buckets and manage reserved orders.

The chapter covers the following topics:
- "Buckets" on page C-168
- "Reservation Orders Bucket" on page C-171
- "Bucket Creation" on page C-178
- "Edit bucket description" on page C-180

### Buckets
**Display > Buckets**

**To the dialog description:**
⇨ Reservation Orders Bucket

[Image: Fig. C-28 Buckets - Buckets (example) screenshot.]

The **Bucket** dialog provides you with an overview of buckets in A+W Production. You can sort the buckets by different criteria and edit them.

You can configure the following components of the Buckets dialog as you like:
- Tab
- Columns
- Totals row
- Filter

The **Buckets** tab includes the following columns, for example:
- **Bucket**: Name of bucket.
- **Description**: Description of the bucket.
- **Orders**: Number of orders included in the respective bucket.
- **Items**: Number of items included in the respective bucket.
- **IG**: Number of IG included in the respective bucket.
- **LAMI**: Number of LAMI included in the respective bucket.
- **TG**: Number of TG included in the respective bucket.
- **Shapes**: Number of shapes included in the respective bucket.

> **Database information from columns**
> You can open the Column definition dialog by right-clicking on a column and selecting the option Show definition.

#### Totals row
- **Total area**: Total area of all items.
- **IG total**: Number of IG included.
- **TG pcs**: Number of TG included.

#### Filter
- **[Add filter]**: Adds a filter.
- **Drop-down menu**:
    - Click: Opens the drop-down menu from which you select a filter.
    - Right-click: Opens the dialog (Filter Name). The Manage button opens the Filter Definition dialog.
    ⇨ "Filter Definition" on page C-229

#### Context menus
Context menus are offered in the Buckets dialog for Tab, Columns, List, Totals row, Filter. Context menus that appear in the entire area of production scheduling are listed in the chapter Overlapping Context Menus.
⇨ "Overlapping Context Menus" on page C-234

| Group | Path | Remark |
| :--- | :--- | :--- |
| List | Resolve bucket | Resolves the selected buckets and moves the included orders back to the Orders dialog. |

#### Buttons
- **[Batch]**: Creates a batch from selected orders, items or parts.
- **[Glass types]**: Shows the glass types for the selected buckets.
- **[Details]**: Shows the details for the selected buckets.

> **Late transfer of production-irrelevant data**
> Parts that are already scheduled in buckets are left in the buckets when data that is not relevant to production is transferred late. Use the switch `Remove changed items from buckets` in the parameter administrator to control how the parts of a changed item should be handled. Possible values are:
> 0: Parts remain in the buckets (default)
> 1: If changes are applied at order level, the parts are removed from the buckets.

### Reservation Orders Bucket
**Display > Reservation orders bucket**

[Image: Fig. C-29 Reservation Orders Bucket (example) screenshot.]

Use the **Reservation Orders Bucket** to display reservation orders. The dialog serves for overview purposes of scheduled capacities only; you cannot create any batches or buckets from the dialog.

The Reservation Orders Bucket dialog is not activated by default in AWP. You must activate the dialog view before you can use it.

In the Reservation Orders Bucket dialog you can adapt tabs and columns to fit your needs. The dialog includes the following columns, for example:
- **Order number**: Specifies the order number.
- **Batch number**: Specifies the batch number.
- **Delivery date**: Specifies the delivery date.

> **Database information from columns**
> You can open the Column definition dialog by right-clicking on a column and selecting the option Show definition.
> ⇨ "Column Definition" on page C-227

#### Totals row
- **Pcs**: Number of items of the orders shown in the dialog.

#### Filter
- **[Add filter]**: Adds a filter.
- **Drop-down menu**:
    - Click: Opens the drop-down menu from which you select a filter.
    - Right-click: Opens the dialog (Filter Name). The Manage button opens the Filter Definition dialog.
    ⇨ "Filter Definition" on page C-229

#### Context menus
Context menus are offered in the Glass Types dialog.

| Group | Path | Remark |
| :--- | :--- | :--- |
| Columns | Re-sorting | Sort column in ascending or descending order. Affects the first three columns. |
| | Formatting | Select format or unit for the columns. |
| | Insert | Inserts a new column. |
| | Insert > Field definition > Edit | Opens the dialog to formulate queries for database tables/fields to insert as a column. ⇨ "Field Definition" on page C-199 |
| | Insert > Field definition > Import | Opens the Import Field Definitions dialog. |
| | Insert > Field definitions > Export | Opens the Export Field Definitions dialog. |
| | Delete | Deletes the selected column. |
| | Change | Currently not being used. |
| | Display definition | Opens the Column Definition dialog. ⇨ "Column Definition" on page C-227 |
| List | Order overview | Opens the Order Overview dialog. ⇨ "Order Overview" on page C-157 |
| | Items | Opens the Items dialog. ⇨ "Items" on page C-193 |
| Totals row| Re-sorting | Currently not being used. |
| | Formatting | Select format or unit for the columns. |
| | Insert | Inserts a new field in the totals row. |
| | Insert > Field definitions > Edit | Opens the Field Definition dialog to formulate queries. ⇨ "Field Definition" on page C-199 |
| | Insert > Field definitions > Import | Opens the Import Field Definitions dialog. |
| | Insert > Field definitions > Export | Opens the Export Field Definitions dialog. |
| Filter | (click/right-click) | Opens the dialog (Filter Name). The [Manage] button opens the Filter Definition dialog. ⇨ "Filter Definition" on page C-229 |

#### Buttons
- **[Batch creation]**: Currently not active.
- **[Glass types]**: Currently not active.
- **[Details]**: Currently not active.

### Purchase Parts Bucket
**Display > Purchase parts bucket**

[Image: Fig. C-30 Purchase Parts Bucket (example) screenshot.]

The **Purchase Parts Bucket** dialog provides you with an overview of buckets that have been created with purchase parts. You can adapt tabs and columns to fit your needs.

The dialog includes the following columns, for example:
- **Order**: Number of order.
- **Article**: Article number.
- **Delivery date**: Date of the delivery.
- **Article description**: Article name.
- **Delivery name**: Name of the customer.

> **Database information from columns**
> You can open the Column definition dialog by right-clicking on a column and selecting the option Show definition.
> ⇨ "Column Definition" on page C-227

#### Totals row
- **Total pcs**: Total of all parts in the selected orders or items.
- **Total duration**: Total processing duration of the selected orders or items. Unit: hours.

#### Filter
- **[Add filter]**: Adds a filter.
- **Drop-down menu**:
    - Click: Opens the drop-down menu to select a filter.
    - Right-click: Opens the (Filter Name) dialog. The Manage button opens the Filter Definition dialog.
    ⇨ "Filter Definition" on page C-229

#### Context menus

| Group | Path | Remark |
| :--- | :--- | :--- |
| List | Move to pool | Moves the selected orders back to the Orders dialog. ⇨ "Orders" on page C-154 |
| | Work schedule > Machinery reallocation | Carries out the machine allocation for selected orders again. The results of the machine allocation within the scope of scheduling are overwritten. |
| | Work plan > Recalculate work plan | Currently not active. |
| | Purchase orders for subsequent parts > Trigger | Currently not active. |
| | Purchase orders for subsequent parts > Do not trigger | Currently not active. |

#### Buttons
- **[Batch]**: Creates a batch from selected purchase parts.
- **[Glass types]**: Currently not active.
- **[Details]**: Currently not active.

### Bucket Creation
*   Display > Orders > Context menu > Create bucket
*   Display > Buckets > Context menu > Create bucket
*   Display > Batches > Context menu > Create bucket
*   Display > Filler orders > Context menu > Create bucket
*   Glass types > Context menu > Create bucket
*   Processing > Context menu > Create bucket
*   Details > Context menu > Create bucket

[Image: Fig. C-31 Bucket creation screenshot.]

Use the **Create Bucket** dialog to create a bucket. It is shown in the Buckets dialog. You can use buckets as intermediate storage.

- **Bucket type**: Selection of the bucket type:
    - Normal
    - Purchase part bucket
- **Bucket**: You can create a new bucket or add the order to an existing bucket.
    - If you do not change anything, a new bucket is created.
    - If you select a bucket from the selection list, the order is added to an existing bucket.
- **Description**: Name of bucket.
- **Production date**: Selection of production date for the batch.
- **Production shift**: Specifies the shift in which the batch should be started.
- **Article type filter**: Selection of the parts for which you are creating a bucket. The following are available: Muntins, Foil, Spacers or Other Non-Glass Articles. For further processing, the parts must have been created in the article master data as released parts.
- **Keep order together**: You can keep the order items together.
    - Unchecked: The order items are not kept together.
    - Checked: The order items are kept together.
- **[OK]**: Saves the data.
- **[Cancel]**: Closes the dialog without saving the data.

### Edit bucket description
**Display > Buckets > Context menu > Change text**

[Image: Fig. C-32 Edit bucket description screenshot.]

Use the **Edit Bucket Description** dialog to change the description, production date and production shift of a bucket.
- **Bucket**: Name of bucket.
- **Description**: Name of bucket.
- **Production date**: Selection of the production start for the bucket.
- **Production shift**: Specifies the shift in which the bucket should be started.
- **[OK]**: Saves the data.
- **[Cancel]**: Closes the dialog without saving the data.

## Batches in Rough Scheduling
This chapter provides you with information on all the dialogs with which you can get an overview of batches. You can create and edit batches, create special glass batches and release batches that are thus released for production.

The chapter covers the following topics:
- "Batches" on page C-182
- "Batch creation" on page C-185
- "Create Special Glass Batch" on page C-187
- "Edit Batch Description" on page C-188

### Batches
**Display > Batches**
**To the dialog description:** ⇨ Release of Batch (Name): AUW – Repetition

[Image: Fig. C-33 Batches (example) screenshot.]

The **Batches** dialog provides you with an overview of the created batches. Batches are a grouping of orders or items that are to be processed together in the process of production preparation and production release. Rough scheduling, detailed scheduling, optimization and batch release are executed on the basis of the batches.

You can sort the batches by different criteria and edit them. You control this dialog mainly via context menus.

The **Batches** tab includes the following columns, for example:
- **Batch**: Name of batch.
- **Status**: Batch status.
- **Number**: Number of orders included in the respective batch.
- **Shapes**: Number of shapes included in the respective batch.
- **Description**: Description of the batch.

> **Database information from columns**
> You can open the Column definition dialog by right-clicking on a column and selecting the option Show definition.

#### Totals row
- **Shapes**: Total of all shapes in the orders or items.
- **Total duration**: Total processing duration of the selected orders or items. Unit: hours.
- **Total pcs**: Total of all parts in the selected orders or items.

#### Filter
- **[Add filter]**: Adds a filter.
- **Drop-down menu**:
    - Click: Opens the drop-down menu to select a filter.
    - Right-click: Opens the (Filter Name) dialog. The Manage button opens the Filter Definition dialog.
    ⇨ "Filter Definition" on page C-229

#### Context menus

| Group | Path | Remark |
| :--- | :--- | :--- |
| List | Release batch | Release selected batches for production. |
| | Manage batch > Reset batch | Batch status is reset. |
| | Manage batch > Resolve batch | The batch is resolved. The order data is returned to the pool. |
| | Manage batch > Archive batch | The batch is archived. The archive view is created by a service from A+W Software GmbH. |
| | Manage batch > Set status | Opens the Set status dialog where you can select the status of the batch: being produced, produced, ready for shipment, delivered. |
| | Detailed scheduling | Transfers the batch to Detailed Scheduling and opens the Detailed Scheduling for Batch (name) dialog. |
| | Print muntins | Starts printing of production papers for muntins. |
| | Muntins machine control | Transfers production data for muntins to the respective machines. |
| | Rescheduling to other machines | Opens the Rescheduling dialog to reschedule to other machines. ⇨Capacity Planning: Software Reference, "Machine Reallocation" on page E-610. The results of the machine allocation within the scope of scheduling are overwritten. |

#### Buttons
- **[Release]**: Releases the selected batches for production.
- **[Detailed sched.]**: Transfers the selected batch to Detailed Scheduling and opens the Detailed Scheduling for Batch (name) dialog.
- **[Glass types]**: Shows the glass types for the selected batches.
- **[Details]**: Shows the details for the selected batches.

### Batch creation
*   Display > Orders > [Batch]
*   Display > Buckets > [Batch]
*   Display > Batches > Context menu > Create bucket
*   Display > Filler orders > [Batch]
*   Glass types > [Batch]
*   Processings > [Batch]
*   Details > [Batch]
*   Lots > [Batch]
*   Barcoding > [Batch]

You can also open the Batch Creation dialog by using the context menu.

[Image: Fig. C-34 Batch creation screenshot.]

Use the **Batch Creation** dialog to create a batch or add orders to an existing batch. The batch is then shown in the Batches dialog.
⇨ "Batches" on page C-182

- **Batch**: You can create a new batch or add the order to an existing batch.
- **Description**: Name of batch.
- **Detailed scheduling organization**: Defines which rack organization shall be used for optimizing the batch. You can change this default setting during the work step Detailed Scheduling.
- **Use selected organization as default**: Use rack organization selected in the Detailed Scheduling Organization field as the default.
- **Production date**: Here, you select a production start date for the batch. If you work with A+W Capacity Planner, you can confirm the calculated start date or specifically change it.
- **Production shift**: Specifies in which shift the production of the batch is started.
- **Article type filter**: You can create special batches for muntins, IG spacers, LAMI foil and other non-glass articles. The batches are only created from the selected article types.
- **Keep order together**: You can keep the order items together.
- **[OK]**: Saves the data.
- **[Cancel]**: Closes the dialog without saving the data.

### Create Special Glass Batch
**Glass types > Context menu – List > Special glass > Add**

[Image: Fig. C-35 Create special glass batch screenshot.]

Use the **Create Special Glass Batch** to specifically create batches for special glass.
- **Special glass batch**: You can either create a new special glass batch or add the order to an existing special glass batch.
- **Description**: Name of the new special glass batch.
- **Detailed scheduling organization**: Selection of racks for the special glass batch.
- **Production date**: Selection of production date for the batch.
- **Production shift**: Specifies the shift in which the batch should be started.
- **[OK]**: Saves the data.
- **[Cancel]**: Closes the dialog without saving the data.

### Edit Batch Description
**Display > Batches > Context menu – List > Change text**

[Image: Fig. C-36 Change batch description screenshot.]

Use the **Change Batch Description** dialog to change the description, production date and production shift of a batch.
- **Batch**: Selected batch.
- **Name**: Name of batch.
- **Production date**: Selection of production date for the batch.
- **Production shift**: Selection of the shift in which the batch should be started.
- **[OK]**: Saves the data.
- **[Cancel]**: Closes the dialog without saving the data.

### Release of Batch (Name): AUW – Repetition
**Display > Context menu – List > Release batch.**

In the **Release of Batch (name): AUW – Repetition** dialog you can release batches for Detailed Scheduling.

#### Menu file
- **Update**: Updates the data in the dialog.
- **All reports on the screen**: Sets all settings in the Lists field to screen.
- **All off**: Sets all setting in the Lists field to Off.
- **Start**: Releases the batch for production; starts the printing process for the selected documents and sends the data to the selected machines.
- **Cancel**: Closes the dialog without transferring the data.

#### Cutting table
- **Cutting table 1, cutting table 2, LAMI cutting table 1**: The following options are available in the drop-down menu: Off, Active, Cutting plan, Cutting code.
- **Cutting plan**: The following options are available in the drop-down menu: Printer, Screen preview.

#### IG
- **Bender 1, bender 2, muntin control, IG line 1, IG line 2, line server**: Checkbox (checked: data is transferred, unchecked: data is not transferred).

#### Initialization
- **Bender texts INIT, sketches INIT, spacer sketches INIT, PMO sketches INIT**: Checkbox (checked: data is transferred, unchecked: data is not transferred).

#### Printer
- **Printer lists**: e.g., Windows default printer, Microsoft XPS Document Writer.
- **Label printer**: e.g., TEC, Microsoft XPS Document Writer.

#### Lists
- **Provision list, rack list, etc.**: The following options are available in the drop-down menu: Off, Screen, Microsoft XPS Document Writer. Specify the number of printouts in the field behind.
- **Production label, shipping label**: The following options are available in the drop-down menu: Off, Screen, TEC B-SX5.

#### Executing processes
The list displays all the processes that are started with this batch.
- ID: ID of the process.
- Station: Station where the process is executed.
- Batch: Batch where the process is executed.
- Computer: Name of the computer on which the process is executed.
- Description: Description of the process.
- Status: Status of the process.
- Error: Specifies whether there is an error in the process execution.

#### Buttons
- **[All reports on the screen]**: Sets all settings in the dialog onto Screen.
- **[All off]**: Sets all setting in Lists field to Off.
- **[Start]**: Releases the batch for production and starts the print operation for the selected documents.
- **[Cancel]**: Closes the dialog without transferring the data.

## Items in Rough Scheduling
This chapter provides you with information on all the dialogs with which you can get an overview of items or can further process these. You can monitor items, split items and import or export items views.

The chapter covers the following topics:
- "Items" on page C-193
- "Add Order to Items" on page C-196
- "Split Items" on page C-197
- "Field Definition" on page C-199
- "Export/Import Item View" on page C-201

### Items
*   Display > Orders > Context menu – List > Items
*   Display > Buckets > Context menu List > Items
*   Display > Batches > Context menu – List > Items
*   Display > Filler orders > Context menu List > Items
*   Glass types > Context menu > Items
*   Processings > Context menu > Items
*   Details > Context menu > Items
*   Lots > Context menu > Items
*   Barcoding > Context menu > Items

[Image: Fig. C-37 Items (example) screenshot with areas for Navigation, Database columns, and List.]

The **Items** dialog provides you with an overview of items in the orders. In the Items dialog you can adapt tabs and columns to fit your needs. You control this dialog mainly via context menus.

#### Navigation
Select in the navigation area which details shall be shown.
- **Order (order number)**: Order number of the selected order:
    - **Item (item number)**: The individual items are listed.
    - **Part (part number)**: The individual part numbers are listed.
    - **Geometry**: Shows details concerning the geometry of the lite.
    - **Text**: Shows texts stored for the order.
    - **Processings**: Shows included processings.

#### Database columns
- **Database column**: List of the database columns pertaining to the element you marked in the navigation.
- **Value**: Value of the respective database column.

#### List
The list shows details pertaining to the element you marked in the navigation.
- **Release part**: Specifies whether this is a release part.
- **Part no.**: Specifies the part number.
- **Type**: Specifies the article or part type.
- **Procurement type**: Procurement type of article or part, e.g. additional purchase.
- **Article no.**: Article number of article.
- **Article description**: Article name.
- **ProdDate**: Production date of the head section.
- **CoatPos**: Specifies whether the coat points to the outside or inside. (0: No coating, 1: Outside, 2: Inside)
- **PatternPos**: Specifies whether the pattern points to the outside or inside. (0: No coating, 1: Outside, 2: Inside)
- **Step**: Specifies whether it is a stepped IG or LAMI.
- **ShpNo.**: Number of the shape that is being used.

> **Database information from columns**
> You can open the Column definition dialog by right-clicking on a column and selecting the option Show definition.
> ⇨ "Column Definition" on page C-227

#### Context menus

| Group | Path | Remark |
| :--- | :--- | :--- |
| Navigation | Add order | Opens the Add Order to Items dialog. |
| | Export view | Opens the Export/Import Item View dialog. |
| | Import view | Opens the Export/Import Item View dialog. |
| Split database | Insert > Order | Inserts a new field in the list. |
| List | Insert > Item | Inserts a new column. |
| | Insert > Parts | Inserts a new column. |
| | Insert > Parts cumulated | Inserts a new column. The cumulative view is the simultaneous retrieval of several database tables and fields, e.g. totals. |

### Add Order to Items
**Items > Navigation > Context menu > Add order**

[Image: Fig. C-38 Add order to items dialog.]

In the **Add Order to Items** dialog you can load additional orders into the Items view.
- **Order number**: Specifies the number of the order to be added.
- **Delete selection first**:
    - Unchecked: Previously displayed orders are not deleted prior to adding.
    - Checked: Previously displayed orders are deleted prior to adding.
- **[OK]**: Saves the data.
- **[Cancel]**: Closes the dialog without saving the data.

### Split Items
*   Display > Orders > Context menu > Split Items
*   Processings > Context menu List > Split items
*   Details > Context menu – List > Split items

[Image: Fig. C-39 Split items dialog.]

The **Split Items** dialog is used for splitting order items.

#### Selected items
The list shows the processings you have selected in the Processings dialog.
⇨ "Processings" on page C-203
- **Order**: Orders which have been selected for splitting.
- **Item**: Number of items in the orders.
- **Sitem**: Currently not being used.
- **Quantity**: Number of parts in the orders.

#### New Items
The list shows the split items.
- **Order**: Split orders.
- **Item**: Number of items in the orders.
- **Subitem**: Currently not being used.
- **New item**: New item resulting from the splitting.
- **Quantity**: Number of lites in the orders.

- **[Remove]**: Deletes a selected item.
- **Split per item in ... items**: Specifies into how many new items the splitting shall be executed.
- **Create items with maximum ... lites**: Specifies how many lites a new item may include at the most.
- **Create per item an item with... lites**: Specifies that for every item, a new item with a certain number of lites shall be created.
- **Split according to PMO result**: This option button defines that the items are going to be split according to the results of packing optimization.
- **[Split]**: Splits the items.
- **[Close]**: Closes the dialog.

### Field Definition
**Items > Context menu Database columns > Insert > Field definitions > Edit**

[Image: Fig. C-40 Field definition dialog.]

Use the **Field Definition** dialog to edit the definitions of the respective fields.
- **Menu group**: Selection of the menu group to which the field is allocated.
- **Menu entry**: Selection of a description for the selected menu group.
- **Column header**: Name of the column.
- **Description**: Field description.
- **Format**: Specifies the format of the field.
- **Database field**: Specifies the database table and corresponding field which is accessed by the new query or column.
- **Options**:
    - Sorting sequence ascending
    - Sorting sequence descending
    - Cumulate
- **Display options**:
    - **Hide identical content in following lines**: If successive fields have the same content, you can hide them.
    - **Value changeable (item view only)**: Specifies whether the values can be changed.
    - **Pull-down criterion (component display only)**: Selection whether there is a pull-down criterion.
- **[Save]**: Saves the menu entry.
- **[Delete]**: Deletes the entire menu entry.
- **[Close]**: Closes the dialog.
