---
title: "EN_UM_AWProduction_13"
source: "EN_UM_AWProduction_13.pdf"
tags: ["A+W Production", "Realtime Optimizer", "glass manufacturing", "software reference", "cutting optimization", "table optimization", "batch processing", "residual stock", "DynOpt", "Production Terminals"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive software reference manual for the A+W Production Realtime Optimizer and A+W Production Terminals. It details functionalities for optimizing glass cutting processes, including table optimization, batch management, reject handling, and settings configuration. The manual also covers the A+W Residual Stock Manager and provides step-by-step 'Help Cards' for common operational workflows."
long_description: "This document serves as a detailed technical guide and user manual for the A+W Production software suite, primarily focusing on the Realtime Optimizer and Production Terminals. The first part of the manual is dedicated to the 'Realtime Optimizer,' covering the entire workflow from input to cutting. The 'Optimization' section explains how to create and manage table optimizations, select glass types, handle batches, and reset cutting jobs. It describes two main variants for table optimization: a default mode and a production date-driven mode. The 'Cutting' section outlines the process of selecting and cutting batches, managing rejects through a rejects pool, linking optimizations, and using the DynOpt editor for dynamic optimization. It also details how to handle residual plates and stock. The 'Settings' section provides instructions on configuring system parameters for tables and optimizations at runtime. A significant portion is also dedicated to the 'A+W Residual Stock Manager,' a web-based interface for managing residual plates, including the setup of warehouses, storage locations, and racks. The second half of the document consists of 'Help Cards,' which are concise, task-oriented tutorials for key operations like entering rush orders, creating optimizations, and managing the cutting process. Finally, the manual introduces the 'A+W Production Terminals,' explaining their role in the production workflow, their various types (e.g., Manual Cutting, IG-In, TG-Out), and their operational goals, such as providing graphical information to workers and enabling real-time process tracking."
---

# Software Reference

---
## Optimization

Open Optimization menu.

The Input menu offers the following options:

- **Table optimization:**
  Use this menu to create a table optimization.
  ⇨ Software Reference, "Select glass for optimization" on page J-1202
- **Reset:**
  Use this menu to reset batches.
  ⇨ Software Reference, "Resetting a cutting batch" on page J-1220

---
A+W Production Realtime Optimizer

## Select glass for optimization

**Optimization > Table optimization**

There are two different variants of this dialog. Which variant is displayed depends on which settings you have made for the table optimization:

- Standard
- Production date

⇨ Chapter "Table optimization" on page J-1251

### Table optimization in the Default variant

*Fig. J-64: Select glass for optimization - default*

In this dialog, A+W Production lists all glass types for which there are batches and rush order lites to be optimized. The available jobs for the selected glass type will be displayed.

#### Description of fields in section Available glass types

**Glass type** Shows the article number of the glass type for which jobs are available. The value is loaded from master data.

**Thickness** Shows the thickness of the glass type. The value is loaded from master data.

**Residual stock** This column only appears if A+W Production has been configured to operate with a residual plate dispenser. This column shows an entry if the residual plate dispenser contains a lite of the required glass type and thickness. The number displayed is the length of the residual plate in mm found in the residual plate dispenser. If the dispenser contains several residual plates of this glass type and thickness, the longest residual plate will be displayed.

**Breakage** If breakage has been entered for this glass type, this field shows the number of broken lites.

**Broken surface** If breakage has been entered for this glass type, this field shows the total surface of the breakage.

**Rush order quantity** If rush orders have been entered for this glass type, this field shows the number of lites.

**Rush order surface** If rush order lites have been entered for this glass type, this field shows the total surface.

**Glass name** This field shows a description of the glass type. The value is loaded from master data.

#### Description of fields in section Optimizations available

**Batch** This column shows the number of the job containing optimizations for the selected glass type.

**Lot** This column contains the batch number of the job that includes optimizations for the selected glass type.

**Locked** This column defines if and from which the terminal the job has been locked for processing or optimization.

**Parameter** This column shows the table for which the displayed batch has been optimized.

**Stockplates** This column defines the number of stockplates required for optimizing the batch.

**Number of lites** This column shows the number of lites included in the lot optimization.

**Lite surface** This column shows the square metres of glass included in the lot optimization.

**Waste** This column shows the waste in % resulting from the present batch optimization.

**Residual (mm)** Shows the length of the residual plate resulting from batch optimization on the cutting table.

**Information** This column displays the batch name.

**Date** In this column, you see the production date that was calculated during batch creation by capacity planning.

**Shift** This column displays the production shift that was determined during batch creation by capacity planning.

### Description of checkbox

**Permit manual cutting** If this checkbox is tagged, the list **Glass types** also shows the glass types for optimization that were defined in master data only for manual cutting.

- [ ] show only glass types for automatic cutting
- [x] show glass types for manual cutting as well

### Table optimization in the Production date variant

*Fig. J-65: Select glass for optimization - Production date*

This dialog displays the production dates and allows you to filter the optimizations by production date. This makes it easier to meet deadlines and plan the production process.

First, select a production date from the **Production Date** list.

The **Available Glass Types** area shows all glass types that are included in optimizations with the selected production date. Select the glass type you want to cut.

The **Available Optimizations** area shows all optimizations that should be produced by the selected production date. For a better overview, the optimizations are marked in color:

- **Green:** The production date is in the future.
- **Yellow:** The production date is today.
- **Red:** The production date is in the past.

The fields in the **Available Glass Types** and **Available Optimizations** areas are identical to the fields on the **Table optimization in the default variant** dialog and will be explained there.
⇨ Chapter "Table optimization in the Default variant" on page J-1202

> **Additional information**
> ⇨Tutorial, "Selecting batches for cutting" on page J-1137

## Local optimization job [no]

This dialog serves to set various optimization parameters. The dialog is split into the following tabs:

- Overview
- Optimize
- Residue plates and stockplates
- Parameter

### Overview

**Optimization > Table optimization > Select glass - [Select] > Overview**

*Fig. J-66: Table optimization - Overview*

This dialog presents the batches selected in dialog **Select glass for optimization**. If an optimization has been run, its results appears here. If no optimization has been run so far, the fields **Plates, Waste** and **Residual (mm)** are empty.

After an optimization has been run, you can double-click on the glass type to start **PlanEdit** if this is installed at your workstation. **PlanEdit** shows the breakout pattern for the stockplate in graphic form.

#### Description of the list at the top

**Glass type** Shows the article numbers of the glass types included in the selected local optimization. The value is loaded from master data.

**Thickness** This field shows the thickness of the glass type. The value is loaded from master data in mm or inch (configurable).

**Parameter** When an optimization has been run, the system shows the optimization parameters applied.

**Quantity** This field shows the number of lites.

**Surface** This field shows the total surface for the optimized glass type in square metres.

**Stockplates** Shows the number of stockplates required for optimization (only after optimization).

**Waste** Shows the waste in % (only after optimization).

**Residual (mm)** Shows the width of the residual plate (in mm) remaining on the table for further use (only after optimization).

#### Description of the list at the bottom

**Batch** This field shows the numbers of the batches batches of which are included in the table optimization displayed.

**Lot** Shows the number of the lots that are included in the table optimization displayed.

**Cutting racks** Shows the number of cutting racks scheduled for the lites of this lot.

**Special glass batch** Defines whether this is a special glass batch. Special glass batches contain glass types that were defined in master data as special glass types. Valid options:
- Yes
- No

**Stockplates** Shows the number of stockplates scheduled for cutting this lot. This is the result of Detailed scheduling, not table optimization.

**Waste** Shows the waste in % for this lot. This is the result of Detailed scheduling, not table optimization.

**Residual (mm)** This field shows the width of the residual plate (in mm) remaining on the table after cutting this lot that can be used further. This is the result of Detailed scheduling, not table optimization.

> **Additional information**
> ⇨ Tutorial, "Create table optimizations" on page J-1126
> ⇨ Tutorial, "Cutting table optimizations" on page J-1126

### Optimize

**Optimization > Table optimization > Select glass - [Select] > Optimize**

*Fig. J-67: Optimize*

This dialog serves to enter the settings for optimization. The list provides information on the selected glass type.

#### Description of fields in section Optimization Sequence

**Batch** This field shows the batch(es) to be optimized.

**Lot** Shows the batch numbers of the individual batches.

**Rank** Shows the optimization rank. Click the ? or ? buttons to change the rank. Identical ranks can be mixed, different separated.

**Items** Shows the number of items included in this batch.

**A Racks** This field shows the number of A racks required for this batch.

**Harp rack** Shows the number of harp racks required for this batch.

**Number of lites** Number of lites included in this batch.

**Lite Sqft.** This field shows the lite surface (in sqm) included in this batch.

**Stockplates** Shows the number of stockplates needed to cut this batch.

#### Description of buttons in section Sequence

**^** This button is used to change the sequence. If you choose a batch with rank 1 for example and click ^, the rank will change from 2 to 1. The sorting of the table may change as well.

**v** This button is used to change the sequence. If you choose a batch with rank 1 for example and click v, the rank will change from 2 to 1. The sorting of the table may change as well.

**Select** This combo box controls the rank. The combo box consists of as many ranks as there are batches on the table. You can select a batch from the table, open the combo box and assign the selected batch the required rank. The ranks have to be assigned consecutively, i.e. you cannot skip a rank. Rank 1 is followed by rank 2, then rank 3. Rank 2 cannot be skipped. If you assign a lower tank to a batch, sorting of the table will change.

#### Description of fields in Automatic compilation section

**Split lots** This checkbox defines whether lots will be split.
- [ ] Lots will not be split.
- [x] Lots will be split. Activating this checkbox may affect the field Rank.

**Divide lots by maximum number of cutting racks** This checkbox defines whether lots will be split and if so, when this is done. If you want to split up lots after a certain number of cutting racks, enable the checkbox and enter in the following field the quantity after which the lot will be split.

**Use minimum lite surface for splitting lots** This checkbox defines whether lots will be split and if so, when this is done. If you want to split up lots after a certain number of cutting racks, enable the checkbox and enter in the following field the quantity after which the lot will be split.

> **Splitting of lots**
> Lots can be split either by the maximum number of cutting racks, or by minimum lite surface. These two checkboxes cannot be active at the same time.

#### Description of fields in section Batch parameters

**XOPT-S** This parameter needs to be set if you are working with A racks. The optimization then takes into account that the lites need to be set on A racks, maintaining a certain sequence for the following processings.

**Rejects** This parameter defines that whenever there are rejects for the selected glass type, it will be automatically included in the imminent optimization.

> **Consider settings in xopton.cfg**
> The behavior of this field depends on the settings you have made in the xopton.cfg file. In the [TOptimization] area: OptimizeBrokenSheets, you can make the following settings:
>
> - **0:** You can choose whether rejects should be optimized or not. (default)
> - **1:** Checkbox is deactivated and deselected. No rejects are allowed in the table optimization.
> - **2:** Checkbox is deactivated and selected. Rejects should always be optimized.

**Rush order lites** Selecting this parameter means that you permit than whenever there are rush order lites for the selected glass type, these are automatically integrated in the upcoming optimization.

**Filler only for gaps** This parameter defines that should there be filler orders for the same glass type, gaps in the optimization will be filled with filler orders. The residual plate will not be filled up with filler orders. Existing filler orders for a glass type are displayed on tab **Filler**.

**Residual stock** This checkbox only appears if you have a residual plate stock.
- [ ] The residual plate stock will not be used
- [x] The residual plate stock will be used

#### Description of fields in section Table

**Table** The combo box shows all tables configured for your production. Select the required table from the combo box.

#### Description of fields in section Optimization parameters

**Optimization parameters** The combo box lists the optimization parameters for creating the optimization. The system presents only parameters that can be used by the selected table. Select the required table from the combo box. The section below shows the parameter name.

#### Description of buttons

**Optimize** Use this button to start the optimization. The optimization will be run in the background. The optimization is run in the background. The results can be viewed in tab Overview as soon as they are available. The optimization result will be saved in the database only if the button [Save] or [Cut] is clicked.

> **Additional information**
> ⇨Tutorial, "Cutting table optimizations" on page J-1126

### Residue plates and stockplates

**Optimization > Table optimization > Residue plates and stockplates**

*Fig. J-68: Residue plates and stockplates*

This dialog serves to select for the previously selected glass type the residue plates and stockplates to be used for optimization. The selected glass type is shown on the left. The right side shows the suitable stockplate or, if available, the suitable residue plates. These are sorted according to availability and grouped in terms of the unloading order of the rack.

#### Description of fields in section List of stockplates (right)

**Width** Shows the width of the stockplate in mm.

**Height** Shows the height of the stockplate in mm.

**XY?** This column defines the direction of the subplate. Possible values:
- **X:** The subplate must be vertical to the bottom edge of the plate.
- **Y:** The subplate runs parallel with the bottom edge of the lite.
- **?:** The optimization can choose one of the two directions for the subplate.

**Residual plate slot** This field shows where the stockplate can be found. If it says stock, the plate is a stockplate. If it shows a number, e.g. 2, the plate is a residue plate which can be found in slot number 2. If the field shows WH (warehouse), the plate is in a vertical Remaster. If the field shows RM, the plate is in a horizontal Remaster.

If you only want to use residue lites from the residue storage for the optimization, in the [Cutting] section of the Xopton.cfg file, you must set the OptimizeResidualsOnly switch to Y (standard is N). Then only residue lites will be available for selection in the table optimization and the stock sizes from the master data will be ignored. If the selected batches do not fit the available stock sizes, an appropriate message will be output. As with normal table optimization, here the maximum possible number of different stock sizes is limited to 10.

During the reoptimization, if this is active, only existing lites from the residue storage will be used. So that the reoptimization is possible, at least one residue lite must be present in the residue storage. If this is not the case or if there are not enough residue lites available, the reoptimization is canceled and the original pattern is cut.

**Storing time / quantity** If the plate is a residual plate, this field shows the date and time at which the plate was added to the residual plate stock. If it shows a number, e.g. 7670, this is a stockplate of which there are still 7670 pieces on stock.

#### Description of fields in section Residual plate

**Height/width** If there is still a residual plate of the same glass type and thickness from the last cutting, this can be used. Enter height and width of the residual plate. The optimization will use this residual plate first, before using a new stockplate.

> **Residual plate and lite from residual stock cannot be used at the same time!**
> If you are already using a residual stock plate, you cannot use a residual plate in addition. If A+W Production has been configured to work with a residual plate dispenser, use of residual stock plates can be switched on or off on tab Optimize via checkbox Use.

> **Additional information**
> ⇨ Tutorial, “A+W Residual Stock Manager" on page J-1147

### Parameter

**Optimization > Table optimization > Parameters > [Quantity]**

*Fig. J-69: Parameter*

This dialog serves to enter the parameter settings for table optimization. The list shows the available stockplates.

#### Description of fields in section Coating

**None/top/bottom** If the stockplate is coated, use the radio buttons to define if the coating is on top or at the bottom. If the stockplate is not coated, enable radio button **None**.

#### Description of the button

**Quantity** Use this button to open dialog **Number of stockplates**.

#### Description of fields in section Optimization parameters

**Trim** The fields **left trim, right trim, top trim** and **bottom trim** show the trim entered for this glass product. The gray fields refer to the values taken from the glass product base data. The values in the white fields can be overridden. This is just a temporary change of trim for the batch on hand.

**Auto-subplate** This checkbox defines whether the defined, maximum subplate width can be extended.
- [x] Maximum subplate width may be enlarged
- [ ] Maximum subplate width may not be enlarged.

**Max. subplate** Field Max. subplate refers to the maximum subplate width for the selected glass product. The gray field refers to the values taken from the glass product master data. This entry can be changed in the white field. This means a temporary change of the maximum subplate width for the corresponding batch.

**Cutting mode** This field defines the cutting mode for the XOPT(S) optimizations. The radio button shows the cutting mode used for detailed scheduling. Selection of the appropriate cutting mode depends on the cutting table and the company's requirements. Generally, cutting mode 1 will produce the best yield while cutting mode 4 shows the worst results. Higher waste might be compensated by quicker breakout and stacking (due to the simpler cutting mode). The cutting mode determines the position of the lites on the subplate between two adjacent Y cuts. Possible values:
- **1:** Between two Y cuts, lites of different width and height can lie next to another. Hence, W cuts may be made.
- **2:** Between two Y cuts, only lites of different width and the same height can lie next to another.
- **3:** Between two Y cuts, only lites of the same item can lie next to another.
- **4:** Between two Y cuts, only up to two lites of the same item can lie next to another.
- **5-7:** Special mode for Coopmes tables. This mode is identical with modes 2-4.

#### Description of buttons

**PlanEdit** This button will be active after an optimization has been run. Use this button to open the program PlanEdit.

**Cutting** This button will be active after an optimization has been run. Use this button to start cutting.

> **Additional information**
> ⇨ Software Reference, “Number of stockplates" on page J-1219

### Number of stockplates

**Optimization > Table optimization > Parameters > [Quantity]**

*Fig. J-70: Number of stockplates*

This dialog shows the number of stockplates available for the selected glass type.

## Resetting a cutting batch

**Optimization > Reset**

*Fig. J-71: Resetting a cutting batch*

This dialog allows to reset batches already started or produced, to be processed again. Saved table optimizations can be resolved. Produced batches that have not been booked yet, can be booked as produced. Delete routines for old (produced) batches are taken over by the ALCIMServer. Please refer to the documentation for information on the deletion of batches.

### Description of the batch list

**Batch** Shows the numbers of the batches the status of which can be changed. Numbers 1000 - 9999 represent completely optimized batches (e.g. from A+W Production) ready for cutting. Numbers 15000 - 15999 (number range can be configured) are reserved for self-created table optimizations.

**Locked** There is an entry in this column if another A+W Production or another process is currently handling this batch.

**Status** Shows the processing status of the individual batches. The following display options are available:

| Status | Meaning |
| :--- | :--- |
| **Released** | An optimization has been released for cutting. These batches can be processed by a table optimization prior to cutting. |
| **Started** | Processing of the batch has been started. Lots of this batch are already being cut, or optimized locally. This status appears even if a table optimization was not cut but was resolved. |
| **Produced** | Batch has been produced. |

*Tab. J-4: Status of batches*

### Description of buttons

**Produced** If a released batch is tagged and this button is selected, the batch is marked as produced, and is no longer available for optimization.

**OK** If a released table optimization (batch from no. 15000) (configurable) is tagged, and this button is selected, the table optimization will be resolved. The included batches, rejects, rush or filler orders are available for new optimizations. Execution of this function is preceded by a security check.
If a produced batch is tagged, and this button is selected, the batch is reset and can be produced again.

> **Additional information**
> ⇨Tutorial, "Reset cutting status" on page J-1145

## Pausing glass types

**Optimization > DynOpt settings**

*Fig. J-72: Pausing glass types*

If a batch is imported into DynOpt, it has to be ensured that there are enough plates of this glass type in stock. You may never import a batch that includes the missing glass types.
Sometimes, however, it happens that you only determine during production that some glass types are not available. With this dialog, you now have the opportunity to lock individual glass types or remove them from production. The dialog shows you all glass types that are in production.

### Explanation of the individual fields

**Filter** With this combo box, you can restrict the list of glass types. The following values are available:
- **All:** all glass types are displayed that are in production.
- **Locked** - only locked glass types are displayed.
- **Urgent:** only urgent glass types are listed. Urgent refers to such lites of this glass type that are waiting by the DynOpt exit lines.

**Exit** This combo box is only active if you have selected the **Urgent** setting on the combo box. Here you have the possibility to display the urgent glass types per exit. To do this, the exits have to be configured appropriately.

**Reason for pausing** To lock a glass type, mark it and select the reason from the combo box.

**Stop optimization** Use this button to stop the optimization. This is necessary if you would like to remove a glass type completely from production. To do this, you first have to stop the optimization and then remove the glass type.

**Remove** This button is only active if you have stopped the optimization for a glass type. Then you can remove the glass type.

**Lock** Use this button to lock a glass type for the next optimization process. First select the glass type, then the reason, then click [Lock].

**Release** Use this button to release a locked glass type. First select the glass type and then click [Release].

**Overview** Use this button to open the **Current changed settings** dialog with an overview of the current settings.

**Resolve** This button is only active if the production is active. Then you can use this button to force a new DynOpt optimization.

**Apply** Use this button to confirm the actions. Ex: You have locked a glass type, then click [Apply] to complete the action.

## Currently changed settings

**Optimization > DynOpt settings > [Overview]**

*Fig. J-73: Currently changed settings - overview*

This dialog provides a summary view of the settings for the tab
- General
- Entries
- Exits
- Buffer

## Cutting

Open **Cutting** menu.

The **Cutting** menu offers the following options:
- **Cut optimization:**
  Use this menu to cut a batch.
  ⇨ Software Reference, "Select a batch" on page J-1226
- **Reject pool:**
  Use this menu to access the reject pool.
  ⇨ Software Reference, "Rejects pool" on page J-1239
- **Panorama:**
  Use this menu to get access to Panorama (optional)

### Select a batch

**Cutting > Cut optimization**

*Fig. J-74: Select a batch*

This dialog is used to select one of the batches available. Select one or all optimizations from the selected batch.

#### Description of the batch list

**Batch** Shows the numbers of the batches the status of which can be changed. Numbers 1000 - 9999 represent completely optimized batches (e.g. from A+W Production) ready for cutting. Numbers 15000 - 15999 (number range can be configured) are reserved for self-created table optimizations. If the term **DynOpt Compact** appears at this point, this is an DynOpt Compact batch.

**Status** Shows the processing status of the individual batches. The options are:

| Status | Meaning |
| :--- | :--- |
| **Released** | An optimization has been released for cutting. These batches can be processed by a table optimization prior to cutting, or can be cut directly. |
| **Started** | Processing of the batch has been started. Lots of this batch are already being cut, or optimized locally. This status appears even if a table optimization was not cut but was resolved. |
| **Produced** | Batch has been produced. |

*Tab. J-5: Status of batches*

**Information** This column displays the batch name.

**Date** In this column, you see the production date that was calculated during batch creation by capacity planning.

**Shift** This column displays the production shift that was determined during batch creation by capacity planning.

> **Change sorting**
> With a click on the column headers, you can sort the list content in ascending or descending order.

#### Description of list Optimization

**No.** Batch number of the optimizations included in this batch.

**Status** Shows the processing status of the individual batches.

**Glass type** Article number of the glass type included in this optimization. The value is loaded from master data.

**Thickness** Thickness of the glass type included in this optimization. The value is loaded from master data.

**Glass name** Shows the name of the glass type. The value is loaded from master data.

**Parameter** Name of the table for which the optimization has been created. The value is loaded from master data.

**Stockplates** Number of stockplates needed for this optimization.

**Waste** Percentage of waste for this optimization.

**Residual (mm)** Length of the residual plate remaining after optimization.

#### Description of fields

**Old batches** Check this box to display even the batches that have already been produced, and still have got the status **Produced**.
- [ ] do not show batches of status **Produced**.
- [x] show only batches of status **Produced**.

**Hide optimizations already cut** When you tag this checkbox, the system hides the optimizations that were already cut.
- [ ] Show optimizations already cut.
- [x] Hide optimizations already cut.

**Reoptimization** Use this combo box to control re-optimizations. Possible values are:
- **No:** there is no reoptimization.
- **Yes:** there is a reoptimization without user intervention. If an optimization that was not optimized for the configured table is transferred to cutting, then a table optimization is created automatically without dialog display and inserted into the cutting process instead of the original optimization.
- **Expanded:** Reoptimization with display of the existing optimization of the glass type to be cut. Here, you can add additional optimizations for table optimization to the optimization to be reoptimized. The table optimization can then be created as usual. After the optimization has been done, the optimization can be discarded or transferred to the cutting process with the [Cutting] button. If the optimization is discarded, you have the opportunity to cut the original optimization or to skip the optimization.
- **Table optimization:** Reoptimization with display of the **Table optimization** dialog. If an optimization that was not optimized for the configured table is transferred to cutting, then the **Table optimization** dialog is started. Here, the optimization parameters such as edge cuts and cutting mode can be changed. After the optimization has been done, the optimization can be discarded or transferred to the cutting process with the [Cutting] button. If the optimization is discarded, you have the opportunity to cut the original optimization or to skip the optimization.

If the optimization was transferred to cutting accidentally, the cutting can be ended and the table optimization dissolved. After that, the original optimization is again available for the cutting.

**Combo boxes** The upper combo box marks the machine status. Possible values are:
- **Ready:** Cutting table is ready for work.
- **Off:** Cutting table is not ready for work (e.g. break).

Use the lower combo box to decide which batches will be displayed. Possible values are:
- **Batches for the own table:** Displays cutting batches for the own table only.
- **Batches for alternative tables:** Displays cutting batches also for alternative tables.
- **Batches for all tables:** Displays batches for all cutting tables.

**Select table** The combo box can be used to restrict the display. The combo box shows all cutting tables defined. You can define whether optimization jobs of all tables will be shown, or only those optimized for the table configured in your A+W Production installation. If A+W Production has been configured for "Table 9 logic", you can also choose **Alternative tables**.

#### Description of buttons

**Options** Use this button to create cutting data out of the optimization data, and transfer these to the cutting table. Cutting is started at the connected cutting table. The button changes to **STOP**.

**Sort** This button will be active for a batch with more than one optimization only. If you click this icon, the **Optimization sequence** dialog opens.

**Cutting** Use this button to open the **Cutting overview** dialog.

> **Additional information**
> ⇨Tutorial, "Selecting batches for cutting" on page J-1137
> ⇨Tutorial, "Cutting table control" on page J-1134

### Batch [number] - batch [number]

**Cutting > Cutting optimization > [OK]**

*Fig. J-75: Batch nnn - Batch mmm*

This dialog shows batches and lots selected in dialog **Select a batch for cutting**.

#### Description of the List of Optimizations

⇨ Software Reference, "Description of list Optimization" on page J-1227

#### Description of the Pattern List

**No.** Consecutive numbering of stockplates used in this optimization. Numbers correspond to the cutting sequence.

**Width** This field shows the stockplate width in mm. The input in this field is loaded from master data.

**Height** This field shows the stockplate height in mm. The input in this field is loaded from master data.

**Opt Gr.** Shows which optimization groups fill the stockplate with lites. Only two groups per stockplate are valid.

**Status** Shows the status of the individual stockplates of the optimization. The following statuses are valid:

| Status | Meaning |
| :--- | :--- |
| **Sent** | Cutting code was created. |
| **Skip** | No cutting code will be created for this stockplate, and no breakout pattern will be supplied. |
| **Do not send cutting code** | No cutting code will be created for this stockplate, but a breakout pattern will be supplied. |
| **Cut** | This status is set when the cutting table has received or picked up the cutting code (serial link or via network). The system does not check whether the lite was actually cut. |

*Tab. J-6: Status of batches*

#### Description of buttons

**Table - START** Use this button to create cutting data out of the optimization data, and transfer these to the cutting table. Cutting is started at the connected cutting table. The button changes to **STOP**.

**Table - STOP** Click this button to stop the transfer of cutting data to the cutting table. The cutting table finishes cutting the started stockplate. The button changes to **START**.

**Pattern - sequence** Use this button to open the dialog **Optimization sequence**.

**Pattern - options** Use this button to open the dialog **Batch: Number**.

**XTV - stop** This button serves to stop the communication. The previous cutting pattern remains.

**XTV - <<** This button scrolls back the breakout display in the connected XTV.

**Close** This button closes the dialog. This is possible only if the system currently creates no cutting code. If cutting code creation is under way, use [STOP] first to stop it.

> **Additional information**
> ⇨ Software Reference, "Optimization sequence" on page J-1232
> ⇨ Software Reference, "Batch: Number" on page J-1233
> ⇨ Tutorial, "Check and process table optimization result" on page J-1128
> ⇨ Tutorial, "Cutting table optimizations" on page J-1126

### Optimization sequence

**Cutting > Cut optimization > Select optimization > [Sorting]**

*Fig. J-76: Optimization sequence*

If the selected batch contains several glass types to be optimized, this dialog shows the scheduled cutting sequence for these glass types. To change the sequence use the arrow keys.

#### Fields

**Status** Shows the status of the optimization.

**Glass type** Shows the product number for the glass type. The value is loaded from master data.

**Thickness** This field shows the thickness of this glass type in mm. The input in this field is loaded from master data.

**Glass name** This field shows the name of the glass type. The value is loaded from master data.

**Parameter** Shows the cutting table on which the optimization will be cut.

**Stockplates** Shows the number of stockplates used for optimization.

**Waste** Shows the waste of the optimization.

**Rest** Shows the residual plate.

### Batch: Number

**Cutting > Cut optimization> Select optimization > [Options]**

*Fig. J-77: Residual handling*

This dialog defines what may or will happen to the rejects and residual plates of each glass type of the selected optimization.

#### Description of the optimization list

**Lot** Lot number of the displayed glass type within the optimization.

**Glass type** Shows the product number for the glass type. The value is loaded from master data.

**Thickness** This field shows the thickness of this glass type in mm. The input in this field is loaded from master data.

**Glass description** This field shows the name of the glass type. The value is loaded from master data.

**Parameter** Shows the cutting table the optimization is meant for.

**Stockplates** Number of stockplates required to cut this batch.

**Waste** Percentage of waste for this optimization.

**Residual (mm)** Length of the residual plate remaining after optimization.

#### Description of the Plate list

**No.** Number of the stockplate which is needed for the optimization tagged on the **Optimizations** list.

**Width** This field shows the stockplate width in mm. The input in this field is loaded from master data.

**Height** This field shows the stockplate height in mm. The input in this field is loaded from master data.

**Opt Gr.** Shows which optimization groups fill the stockplate with lites. Only two groups per stockplate are valid. An optimization group may be a job or a re-optimization.

**Cutting status** Shows the cutting status of the individual stockplates of the optimization. The following statuses are valid:

| Status | Meaning |
| :--- | :--- |
| Sent | Cutting code was created. |
| Skip | No cutting code will be created for this stockplate, and no breakout pattern will be supplied. |
| Do not send cutting code | No cutting code will be created for this stockplate, but a breakout pattern will be supplied. |
| Cut | This status is set when the cutting table has received or picked up the cutting code (serial link or via network). The system does not check whether the lite was actually cut. |

*Tab. J-7: Cutting status of batches*

#### Description of the fields in the Reject optimization section

**Optimize rejects** Here you specify the way A+W Production will handle rejects transferred to cutting. The following settings are possible:
- **No:** no re-optimization,
- **Separate:** The new re-optimization was added at the end of the existing optimization. This results in a subplate between the existing optimization and the new part.
- **Mix:** The previous stock plate will be re-optimized completely. This often results in a better yield.

**Cut rejects by residual plate length** This checkbox defines whether the rejects will be optimized with a new residual plate if the existing residual plate does not suffice. If this checkbox is tagged, the entry in the following field is important.
- [ ] Do not start new stockplate to cut rejects.
- [x] Start new stockplate if the new residual plate is smaller than the new residual plate length defined in the following field, **Length**.

**Cut residual plate below a length of** This field is active only if the previous checkbox was tagged. Enter the maximum size for the new residual plate. No new residual plate will be started if reoptimization results in a bigger residual plate. Rejects are collected in the breakage pool.

#### Description of the fields in the Residual plate management section

**Link** Here you specify the way A+W Production will handle residual plates. The following settings are possible:
- **No:** no linking,
- **Separate:** The new re-optimization was added at the end of the existing optimization. This results in a subplate between the existing optimization and the new part.
- **Mix:** The lites will be resolved on the residual plate and re-optimized together with the quantity to be optimized.

**Edit residual plate before cutting** If this box is checked, the system will ask whether PlanEdit will be started.

#### Description of the fields in the Quick optimization section

**Quick optimization**
- **Standard:** In this mode, you can dissolve and re-optimize the pattern of a glass type for which no cutting code was transmitted during the cutting process. The idea is that for optimizations with many patterns, the broken lites are not only optimized on the last lite. The broken lites are placed in the new optimization at the start (without further user intervention).
- **Expanded:** In this mode, additional user inputs are required. The glass selection menu for the table optimization is called up automatically. There, however, only the glass type of the dissolved optimization is visible. Here you can add additional optimizations. Then the **Table optimization** dialog opens. There, you can change edges, etc. When the optimization is finished, the optimization can be transferred directly to the cutting process using the [Cut] button.

**Reloading** Use this setting to load a further batch. The following settings are possible:
- **Manual:** Reloading is done manually.
- **Requirement:** The user gets a message as soon as the number of uncut patterns in A+W Production falls below a defined threshold. The user can reject reloading, or select a new batch to be loaded from the selection.
- **Automatic:** Reloading is done automatically.

#### Description of the fields in Label printing section

**Active** Use this checkbox to activate or deactivate the label printing.
- [ ] Label printing is deactivated.
- [x] Label printing is activated. You can print labels directly.

#### Description of buttons

**PlanEdit** If you select this button, and module **PlanEdit** is installed on your system, **PlanEdit** is started and gives a graphic display of the optimization.

**Cutting** Use this button to start the **Cutting overview**.

#### Description of the context menu

Click the right mouse key on a lite with status **Cut** to delete the status **Cut** and allow to cut the lite again.

Click the right mouse key on a lite without a status to set the status **Do not send cutting code** or **Skip** can be set for the selected lite.

> **Additional Information**
> ⇨ Tutorial, “A+W Pattern Viewer" on page J-1156
> ⇨ Tutorial, “A+W Residual Stock Manager" on page J-1147

### Select the Optimizations to be linked

**Cutting > Cut optimization > Select batch > [OK] > Dialog Active batch: xxx opens > Select optimization > [Start]**

*Fig. J-78: Select the optimizations to be linked*

The list **Available optimizations** shows all batches containing optimizations for the glass type and thickness selected from the Glass type list. The dialog header contains the selected batch, the lot, and the glass type.

#### Description of fields in section Selection parameters and residual plate

**All tables** This checkbox defines the optimizations to be displayed. If this box is checked, optimizations for other tables will be displayed too.

**Permit manual cutting** If this box is checked, the list **Available optimizations** shows even the glass types designed only for manual cutting in master data.

**Residual plate** Shows the length of the residual plate resulting from the selected optimization (dialog Active job: xxx).

### Optimization result

**Cutting > Cut optimization > Select batch > [OK] > Dialog Active batch: xxx being opened > Select optimization > [Start] > Select batch > [Link]**

*Fig. J-79: Optimization result*

This dialog shows the optimization result after linking. It consists of two sections. Section **New optimization after linking** shows the result after linking. Section **Original optimization** shows the result prior to/without linking.

The gray area above the buttons tells you what and which quantity has been additionally optimized.

#### Description of buttons

**Repeat** Click this button to return to the selection for link optimization where batches can be selected.
⇨ Software Reference, "Select the Optimizations to be linked" on page J-1237

**Linking** This button is used to confirm the result and start cutting of the optimization.

### Rejects pool

**Cutting > Rejects pool**

*Fig. J-80: Rejects pool*

This dialog shows all lites entered as or reported broken. If glass type and thickness fit, lites from the breakage pool can be optimized once more in local optimizations or reoptimization.

#### Description of the Rejects list

**Glass type** Shows the product number for the glass type. The value is loaded from master data.

**Description** This field shows the name of the glass type. The value is loaded from master data.

**Thickness** This field shows the thickness of this glass type in mm. The input in this field is loaded from master data.

**Width** This field shows the stockplate width in mm. The input in this field is loaded from master data.

**Height** This field shows the stockplate height in mm. The input in this field is loaded from master data.

**Batch** Shows the batch number the lite originally belonged to.

**DynOpt** With this field, you can set a DynOpt flag for individual broken lites, so that they can be re-optimized by DynOpt. To do this, select the lite in question and then click the **DynOpt** button. Only lites can be selected for which no lock station is entered.

**Customer** Shows the name of the customer the broken lite belongs to.

**Order** Shows the number of the order the broken lite belongs to.

**Itm** Shows the item number of the order the broken lite belongs to.

**Quantity** Shows the number of lites.

**ShapeNo** If the broken lite is a shape, the shape number appears in this field.

**Rack** Number of the storage location (rack or harp rack) that would have held the lite were it not broken.

**Label no.** Label number of the broken lite.

**Lot** This field is used only for program-internal purposes and has no meaning.

#### Description of buttons

**Update** If more broken lites are reported (e.g. A+W Production Terminal XTV) while you are using this dialog, these will be shown only after the dialog display was updated by means of this button.

**Delete** Use this button to delete the tagged broken lite from the rejects pool. You can tag and delete several lites at the same time. If you work with barcoding, you can also book the lites.

**Shape info ...** This button starts the shape display of A+W Production.

**Printing** This button starts a printout listing the contents of the rejects pool. This button is available only if the system was configured accordingly.

**Add** This button opens the **Reject input** dialog.

#### Explanation of the combo box

With the combo box, you can select to which table the break that you want to add should be booked.

If you open the rejects pool for the first time, by default the table is selected on which the A+W Production is attached.

> **Additional information**
> ⇨Tutorial, "Rejects, rush order lites or filler orders" on page J-1118
> ⇨ Software Reference, "Shape input" on page J-1193
> ⇨ Software Reference, "Add rejects" on page J-1241

### Add rejects

**Cutting > Rejects pool > [Add]**

*Fig. J-81: Add rejects*

This dialog can be used to enter broken lites that will be included in an optimization once more.

#### Description of fields

**Order** Enter the order number the broken lite belongs to.

**Item** Enter the item number of the order the broken lite belongs to.

**Reject reason** Select the reject reason from this combo box. You can select only reject reasons defined in master data.

#### Description of the Part list

**Ordno** Order number the broken lite belongs to.

**PartNo** Part number of the lite.

**Description** This field shows the name of the glass type. The value is loaded from master data.

**Width** Shows the width of the glass type in mm or inch (configurable).

**Height** Shows the height of the glass type in mm or inch (configurable).

### Search fields

**Cutting > Rejects pool > [Add] > <Ctrl> + <F12>**

*Fig. J-82: Search fields*

On the **Add Rejects** dialog, up to three freely configurable search fields can be added. These are the fields **Searchfield1, Searchfield2,** and **Searchfield3**. The fields are added with the form administration:

- **Control with action:** Entry can freely be defined
- **Selected part:** Searchfield1, ...).
- **Action:** Combo box Searchfield1, ...

If you are not familiar with this technology, please contact an A+W employee.

> **Additional information**
> ⇨Tutorial, "Rejects, rush order lites or filler orders" on page J-1118

### Input of shapes

**Cutting > Rejects pool > [Shape Info]**

*Fig. J-83: Shape input*

| | |
| :--- | :--- |
| **A** | Input required per shape |
| **B** | Shape numbers |
| **C** | Graphic overview of shapes |
| **D** | Shape overview |
| **E** | Parameter list |
| **F** | Input field |

The fields and buttons in this dialog are the same as in dialog **Shape input** in the rush order lite section. The dialog is described there.

> **Additional Information**
> ⇨ Software Reference, "Shape input" on page J-1193

### A+W DynOpt editor

**Cutting > DynOpt Compact ...**

*Fig. J-84: Editor*

On the left, the editor shows in section **Released batches** all batches from detailed planning that can be processed by **DynOpt Compact**.

#### Description of fields in section Released batches

**Batch** Shows the batch number from detailed scheduling.

**Text** This field shows the name of the batch number.

Section **Imported batches** contains already optimized or imported batches. Open the tree structure to view more information on the batch in question. The first level of the tree shows the batch number, the second contains the rack number while the third tells you the status, the number of lites, and the rack type. If you click on the second level (rack number) of the tree, the list **Imported lites** provides detailed information on the individual lites.

#### Description of buttons

**>** Use this button to move a tagged batch from section **Released batches** to section **Imported batches**.

**<** Use this button to move a tagged batch from section **Imported batches** back to section **Released batches**.

**^** This button is used to change the sequence. Select a batch in section **Released batches** and click ? to move it one slot upwards on the list.

**v** This button is used to change the sequence. Select a batch in section **Released batches** and click ? to move the batch one position down on the list.

#### Description of fields in section Imported lites

**Batch** Shows the batch number from detailed scheduling.

**Batch sequence** Shows the sequence of the rack. This is a serial number for imported racks within a batch.

**Serial no.** This field lists, in ascending sequence, the serial number within the batch.

**Slot no.** If the rack is a harp rack, this field shows the slot number. For A racks, it shows 0.

**Glass type** Shows the product number of the glass type.

**Thickness** Shows the lite thickness in mm or inch (configurable).

**Width** Shows the lite width in mm or inch (configurable).

**Height** Shows the lite height in mm or inch (configurable).

**Order** This field shows the order number.

**Itm** Shows the item number of this order.

**Status** This field shows the status. For details, please see below.

**DynOpt Compact batch** Shows the batch number of DynOpt Compact optimization.

**DynOpt Compact lot** Shows the lot number of the DynOpt Compact optimization.

**DynOpt Compact pattern** Number of the pattern the corresponding lite belongs to.

Tag a batch in the bottom left section to view detailed information on the individual lites in the window on the left.

A time bar appears at the bottom of the dialog. Every colored rectangle marks the status of a rack.

The following colors may be used:

| Color | Explanation |
| :--- | :--- |
| Blue | All lites of the rack have been cut. |
| Cyan | All lites of the rack have been optimized. |
| Yellow | All lites of the rack have been optimized. |
| Green | Rack has not been optimized yet. |

*Tab. J-8: Explanation of symbols*

The numbers below the colored rectangle indicate the batch and rack number. Example: 1187/9951 means: batch number 1187 and rack number 9951.

#### Description of fields

**Status** The combo box lists the statuses relevant for **DynOpt Compact**. Valid options:
- **0:** unprocessed
- **100:** entire racks which have been only partly optimized.
- **200:** optimized.
- **300:** Cut.
- **500:** If errors have occurred during optimization, the corresponding lites will get status 500. Apart from that, they appear in the right section of the editor in a red bar.

**Time bar view** The time bar view defines the type of view. The editor is available for **Cutting** and for **Optimization**.

#### Description of buttons

**Update** This button serves to update the editor.

> **Create DynOpt Compact batches**
> DynOpt Compact batches can be created in the editor or at cutting. In the cluster view, you can tag one or more batches then create in the context menu the function **Create DynOpt Compact batches**. At cutting, this is possible only for one batch at a time.

> **Additional information**
> ⇨ Tutorial, “A+W DynOpt Compact" on page J-1179

## Settings

Opening the **Settings** menu.

The **Settings** menu includes the following program point:

- **Tables**
  With this menu element, you access the configured tables.
  ⇨ Software Reference, "Settings" on page J-1249
- **Table optimization**
  Use this menu to access the table optimization.
  ⇨ Software Reference, "Table optimization" on page J-1251

### Settings

**Settings > Tables**

*Fig. J-85: Tables*

This dialog is available for all configured tables.
It offers the opportunity to change settings at runtime, which can otherwise only be adjusted with the configuration file (xopton.cfg). Thus, the A+W Production does not have to be exited and re-started.

#### Explanation of the fields in the residual plate stock

**Active** The checkbox controls whether or not the residual plate stock is used.
- [x] The residual plate stock is used.
- [ ] The residual plate stock is not used.

**Store plates** The checkbox controls whether or not residual plates are stored in the residual plate stock.
- [x] Residual plates are stored in the residual plate stock.
- [ ] Residual plates are not stored in the residual plate stock.

**Using plates** The checkbox controls whether or not the optimization uses the residual plates from the residual plate stock.
- [x] Residual plates from the residual plate stock are used.
- [ ] Residual plates from the residual plate stock are not used.

**Minimum storage length** In this field, you enter the minimum length in mm starting with which a residual plate is stored.

#### Description of fields in Cutting area

**Active** The checkbox controls the label printing during cutting.
- [x] Labels are printed during cutting.
- [ ] Labels are not printed.

**Edit residual plate** In this field, you enter the minimum length of a residual plate in mm, so that editing can be done with PlanEdit during cutting.

#### Description of buttons

**Accept** If you click this button, the changes are applied.

**Reject** If you click this button, the changes are discarded.

### Table optimization

**Settings > Table optimization**

*Fig. J-86: Table optimization*

With this dialog, you control whether with the selection of the table optimization the production date is displayed or not.

The combo box has the following modes:
- Standard
- Production date

If you select the **Default** mode, you will see the table optimization *without* production date.
⇨ Chapter "Table optimization in the Default variant" on page J-1202

If you select the **Production date** mode, you will see the table optimization *with* production date.
⇨ Chapter "Table optimization in the Production date variant" on page J-1205

## View

Open menu **View**.

The **View** menu offers the following items:
- **Start and stop import** (only for A+W Production stand alone)
  Use this menu to start and to exit the import.
  ⇨ Software Reference, "Import" on page J-1253
- **Error messages:**
  Use this menu to access the error messages.
  ⇨ Software Reference, "Error reports" on page J-1254
- **Status bar:**
  Use this menu to show or hide the status bar.

### Import

**View > Import**

*Fig. J-87: Import*

This dialog monitors the working directory for import files and shows the import status.

Batches that have been imported without an error message, appear in dialog **Select a batch** for further processing. Imported data are saved in the database while the imported files are moved to archives.

#### Description of buttons

**Start** When you use this button, the import function will monitor the working directory. When new import files are transferred to the working directory, these are automatically checked and imported into the database. The button now reads **Stop**.

**Stop** Using this button terminates the import. When new import files are transferred to the working directory, these remain unprocessed until the import function is restarted. The button now reads **Start**.

> **Additional information**
> Tutorial, "Import optimizations" on page J-1114

### Error reports

**View > Error reports**

*Fig. J-88: Error reports*

This dialog shows a new error as well as all errors occurred since the program was last started.

**The following error occurred** A new error is shown in this area.

**Previous errors** This section shows all previously occurred errors.

**Error file** Use this button to save the contents of this dialog in an error file.

## A+W Residual Stock Manager

With the **A+W Residual Stock Manager**, you can save and process residual plates without machine assistance. For this purpose there is a web interface (**A+W Planning Web**) that can be opened from anywhere via a browser. The stored residual plates are then automatically available in the **A+W Production** for further processing.

### A+W Planning Web

You handle the configuration for the A+W Residual Stock Manager in this module.

> **A+W Planning Web configuration**
> The default configuration is done by A+W employees during installation. We explain in this documentation how you create **Warehouse, Storage locations,** and **Racks** in **A+W Planning Web**.

### Stock

**A+W Planning Web > Stock > Master data**

*Fig. J-89: Master data: Stock*

This area displays all stocks created at your company. You can change existing stocks, add new stocks, or delete existing stocks.

#### Description of fields

**ID** Unique numeric key. This key must be unique across all stocks. If a new stock is created, the next ID not yet assigned will be suggested. Any previous IDs that have been freed up due to the deletion of a stock are not taken into account and therefore not suggested. It is possible to select the ID manually. If the ID already exists, you will be informed of this with an appropriate message and you will not be able to save it.

**Description** Here you assign your stock a unique name.

#### Description of buttons

**Edit** If you click this button, the **Storage location** tab opens. Here, you can see all storage locations that are created for the corresponding stock.

**Save** If you click this button, all changes made will be saved.

**Add** With this button, you add another stock. If you click this button, a row will be added at the beginning of the table in which you can make the appropriate entries.

**Delete** If you click this button, the selected stock will be deleted. Caution: there is no security query.

**Update** If you click this button, the display will be updated.

If you click the **[< Stock]** button, you return to the overview of the individual stocks.

> **Additional information**
> ⇨Tutorial, "Warehouse" on page J-1149

### Rack information

**A+W Planning Web > Stock > Master data > [Edit] Button**

*Fig. J-90: Editing existing storage location*

On this dialog, you can see all storage locations that are created for the corresponding stock.

#### Description of fields

**Top left** Here you can see where you are at the moment. In the example above, this means that you are in the **Master data** and there in the **Overview of the Individual storage locations** for the **Residual plates** storage stock.

**ID** This field shows the unique numeric key. This key must be unique across all stocks. If a new stock is created, the next ID not yet assigned will be suggested. Any previous IDs that have been freed up are not taken into account and therefore not suggested. It is possible to select the ID manually. If the ID already exists, you will be informed of this with an appropriate message and you will not be able to save it.

**Name** This field shows the unique name for identification of the storage location. You can change the name by clicking in the field and overwriting the existing name.

**Stock type** This field shows you which stock type is associated with the corresponding storage location. For each table with the appropriate table ID, a **Stock** and a **Storage location** with the type **Stock receipt** should be created so that new residual plates can be created manually and saved in other storage locations.
The other stock types (Load, Buffer, Loading station, and Loader) are intended for a Sortjet and are not used in the A+W Residual Stock Manager.

**Allocation status** In this field, you can set whether the storage location can be used for racks or it is locked. A manual lock makes sense, for example, if the area is blocked due to goods delivery. Here, storage locations that were locked by the system can be released again.

#### Description of the button

**Stock** If you click the this button, you return to the overview of the individual stocks.

**Save** If you click this button, all changes made will be saved.

**Add** With this button, you add another storage location. If you click this button, a row will be added at the beginning of the table in which you can make the appropriate entries.

**Delete** If you click this button, the selected storage location will be deleted. Caution: there is no security query.

**Update** If you click this button, the display will be updated.

> **Additional information**
> ⇨ Tutorial, "Storage locations" on page J-1150

### Racks

**A+W Planning Web > Stock > Master data > Storage location > [Edit] Button**

*Fig. J-91: Existing racks*

On this dialog, you can see all racks that are created for the storage location in question. Lites can only be booked to racks; therefore, it is recommended that you configure at least one rack for each storage location.

#### Description of fields

**Top left** Here you can see where you are at the moment. In the example above, this means that you are in the **Master data** and there in the **Overview of the Individual racks** for the storage location 101.

**ID** This field shows you the unique numeric key. This key must be unique across all storage locations. If a new rack is created, the next ID not yet assigned will be suggested. Any previous IDs that have been freed up due to the deletion of a rack are not taken into account and therefore not suggested. It is possible to select the ID manually. If the ID already exists, you will be informed of this with an appropriate message and you will not be able to save it.

**Name** This field shows you the unique name for identification of the rack. You can change the name by clicking in the field and overwriting the existing name.

**Allocation status** In this field, you can set whether the rack can be used for lites or it is locked. A manual lock makes sense, for example, if the area is blocked due to goods delivery. Here, racks that were locked by the system can be released again.

**Properties** In this field, you can see which is the rack type in question, e.g., harp rack, A-rack, etc.

#### Description of the button

**Storage location** If you click the this button, you return to the overview of the individual storage locations.

**Save** If you click this button, all changes made will be saved.

**Add** With this button, you add another rack. If you click this button, a row will be added at the beginning of the table in which you can make the appropriate entries.

**Delete** If you click this button, the selected rack will be deleted. Caution: there is no security query.

**Update** If you click this button, the display will be updated.

> **Additional information**
> ⇨ Software Reference, "Racks" on page J-1259

### Rack properties

**A+W Planning Web > Stock > Master data > [Rack Properties] Button**

*Fig. J-92: Rack properties*

In this area, the properties of the various rack types are displayed. You can make changes or create new racks. To make changes to existing racks, just click in the corresponding field.

#### Description of fields

**Name** Unique name for identification of a rack type.

**Access type** The Access type describes how glass can be stacked up or down. The following options are available:
- **Free:** random access to the glass (e.g. harp racks)
- **First in, First out (FiFo):** only the first glass stored can be removed (e.g. through passage)
- **Last in, First out (LiFo):** only the last glass stored can be removed (e.g. A-rack)

**Maximum weight** This field shows the maximum weight in kg.

**Maximum height** This field shows the maximum height of the glass that may be placed on this rack type.

**Maximum width** This field shows the maximum width of the glass that can be placed on this rack type. In the case of several stacks, this value describes the maximum width of all stacks together.

**Maximum depth** This field shows the maximum depth of the rack. With a glass stack, all thicknesses of the glass in a stack are added together. For harp racks, the maximum depth is set equal to the width of a single slot.

**Minimum height** This field shows the minimum height of the glass that may be placed on this rack type.

**Minimum width** This field shows the minimum width of the glass that may be placed on this rack type.

**Maximum number of stacks/slots** This field shows you the maximum permitted number of stacks on this rack type. With some harp racks, this is the number of slots. If the value -1 is set, the number is unlimited; only the other values such as **Maximum height, Width,** or **Depth** are used for restriction.

**Segment type** This field shows the type of this rack type. Possible values are:
- HarpRack
- L Rack

> **A Rack**
> For configuration of an A-rack, two L-racks must be created.

#### Description of the button

**Save** If you click this button, all changes made will be saved.

**Add** With this button, you add another rack property. If you click this button, a row is added at the beginning of the table in which you can make the corresponding entries.

**Delete** If you click this button, the selected rack property will be deleted. Caution: there is no security query.

**Update** If you click this button, the display will be updated.

> **Additional information**
> ⇨ Software Reference, "Rack properties" on page J-1261

### Glass overview

**A+W Planning Web > Stock > Overview**

*Fig. J-93: Glass overview*

All residual plates that were stored are displayed in this area. The data can be edited in the view, e.g., the size of the residual plate stored. Using the filter functions that are available to you in the table header of each field, you can restrict the display results.

#### Description of fields

**Type** This field shows you which is the glass type in question (residual plate, stockplate, lite). On the right outside, the table header has a filter function. If you click the Filter icon, an area opens in which you can select the desired value from the combo box. If you click [Filter], the display is adjusted based on your selection.

**Storage location information** This field shows you the storage location information for the lite stored. On the right outside, the table header has a filter function. If you click on the Filter icon, all storage locations created will be displayed. You can then click the appropriate checkbox(es). If you click [Filter], the display is adjusted based on your selection.

**Glass type** This field shows you the glass type of the lite stored. On the right outside, the table header has a filter function. If you click the Filter icon, an area opens in which you can enter the name or ID of the glass type. If you click [Filter], the display is adjusted based on your entry.

**Label number** For stored lites, this field shows the label number. On the right outside, the table header has a filter function. If you click the Filter icon, an area opens in which you can enter the name or ID of the glass type. If you click [Filter], the display is adjusted based on your entry.

**Width** This field shows you the width of the stored lite. On the right outside, the table header has a filter function. If you click the Filter icon, an area opens in which you can enter the name or ID of the glass type. If you click [Filter], the display is adjusted based on your entry. If you click the Filter icon, an area opens in which you can enter the value and property (larger than, smaller than, equal to). If you click [Filter], the display is adjusted based on your entry.

**Height** This field shows you the height of the stored lite. On the right outside, the table header has a filter function. If you click the Filter icon, an area opens in which you can enter the name or ID of the glass type. If you click [Filter], the display is adjusted based on your entry. If you click the Filter icon, an area opens in which you can enter the value and property (larger than, smaller than, equal to). If you click [Filter], the display is adjusted based on your entry.

**Info** You can store additional information in this field. On the right outside, the table header has a filter function. If you click the Filter icon, an area opens in which you can enter the name or ID of the glass type. If you click [Filter], the display is adjusted based on your entry. If you click the Filter icon, an area opens in which you can enter the value and property (equal to, contains, start value). If you click [Filter], the display is adjusted based on your entry.

**Allocation status** In this field, you can set whether the storage location can be used for racks or it is locked. A manual lock makes sense, for example, if the area is blocked due to goods delivery. Here, storage locations that were locked by the system can be released again. On the right outside, the table header has a filter function. If you click the Filter icon, an area opens in which you can enter the name or ID of the glass type. If you click [Filter], the display is adjusted based on your entry. If you click the Filter icon, an area opens in which you can select the desired value from the combo box. If you click [Filter], the display is adjusted based on your selection.

**Date** This field shows you when the lite was stored. On the right outside, the table header has a filter function. If you click the Filter icon, an area opens in which you can enter the name or ID of the glass type. If you click [Filter], the display is adjusted based on your entry. If you click the Filter icon, an area opens in which you can enter the value and property (larger than, smaller than, equal to). If you click [Filter], the display is adjusted based on your entry.

#### Description of buttons

**Add new data record** If you click this button, a dialog opens on which you can enter the appropriate data for the data record.

**Highlight usable residuals** If you click this button, all usable residuals in the table are highlighted. The Access type is also considered for the use of the residuals on racks.
- If LiFo is selected, the last residual plate stored is used and highlighted on the display.
- If FiFo is selected, the first residual plate stored on a rack is used and highlighted on the display.
- If Free is selected, there is random access and all residual plates are highlighted on the display.

**Edit** If you click this button, the data record is released for editing and you can make changes.

**Delete** If you click this button, the data record is deleted. Caution: there is no security query.

**Print** If you click this button, the label printing is triggered. Please note that the selected printer is set up accordingly.

> **Additional information**
> ⇨ Software Reference, "Glass overview" on page J-1263

### Add/Edit new data record

- **A+W Planning Web > Stock > Overview > [Add new data record]**
- **A+W Planning Web > Stock > Overview > [Edit]**

*Fig. J-94: Add/edit data record*

This dialog can be used to edit existing data records or create new data records.

#### Description of fields

**Stock** Select the appropriate stock from the combo box.

**Storage location information** Select the required storage location from the combo box.

**Rack** Select the required rack from the combo box.

**Group** Select the required group from the combo box.

**Glass type** Select the required glass type from the combo box.

**Width/Height** Enter the appropriate dimensions in these fields.

**Info** Enter an additional text in this field that serves as information.

**Allocation status** Select the appropriate allocation status from the combo box.

**Date** Select the date from the calendar on which the residual plate was stored.

> **Additional information**
> ⇨ Tutorial, "Overview" on page J-1153

---

# A+W Production Realtime Optimizer Help Cards

This section provides information on the following subjects:
- ⇨ Information about the help cards
- ⇨ Input
- ⇨ Optimization
- ⇨ Cutting

| | |
| :--- | :--- |
| **Information about the help cards** | **J-1271** |
| **Input** | **J-1272** |
| Enter rush order lites | J-1273 |
| Enter rejects | J-1274 |
| Input of charges | J-1275 |
| **Optimization** | **J-1276** |
| Selecting batches and glass types | J-1277 |
| Create table optimization | J-1278 |
| Selecting stockplates | J-1279 |
| Using residual lites | J-1279 |
| Adding filler orders | J-1280 |
| Resolve table optimization | J-1281 |
| Create a quick optimization | J-1282 |
| Linking an optimization | J-1283 |
| **Cutting** | **J-1284** |
| Select batches | J-1285 |
| Cutting batches again | J-1287 |
| Skip pattern | J-1288 |
| Do not generate a cutting code | J-1289 |
| Interrupt cutting | J-1290 |

## Information about the help cards

The depictions in the Help Cards are based on the delivery version A+W Production. Individual steps in the workflows may deviate depending on the configuration.

## Input

| Help Card | Topics |
| :--- | :--- |
| - Enter rush order lites | - You enter rush order lites. |
| - Enter rejects | - You enter rejects manually. |
| - Input of charges | - You enter charges. |

### Enter rush order lites (RTO 01-001)

#### Objective of this activity
You enter rush order lites.

#### Requirements
(None specified)

#### Additional info
- It is also essentially possible to enter rush lites in A+W Production. This procedure serves to enter rush customer orders and to cut these without first having to go through the more time-consuming process of entering the order in the ERP system and then transferring it to the production system.

#### Workflow
1.  Select the **Input > Rush order lites** menu.
    *Dialog Rush order lites opens.*
2.  Click **[Add]**.
    *Dialog Input of rush order lites opens.*
3.  Select the glass type.
4.  Enter the thickness.
5.  In field **Rack**, enter the rack onto which the rush order lites should be put after cutting (optional).
6.  Enter the number of lites in field **Quantity**.
7.  In the **Shape** field, select the shape number if you want to enter a shape.
    Or click the magnifying glass in order to open the **Shape entry** dialog.
8.  Enter the fields **Width** and **Height**.

### Enter rejects (RTO 01-002)

#### Objective of this activity
You enter rejects manually.

#### Requirements
(None specified)

#### Additional info
(None specified)

#### Workflow
1.  Select menu **Cutting > Rejects pool**.
    *Dialog Rejects pool opens.*
2.  Click **[Add]**.
    *Dialog Enter rejects opens.*
3.  Go to field **Order** and enter the order number.
4.  In the **Ppos** field, enter the production item.
5.  Select the required reason for the reject from the combo box **Reject reason**.
6.  Save the entries with **[Save]**.

### Input of charges (RTO 01-003)

#### Objective of this activity
You enter charges.

#### Requirements
(None specified)

#### Additional info
- Via this dialog it is possible to define a charge number. With the activated checkbox, you can specify that the charge number will be inherited by following stockplates of the same glass type/thickness.

#### Workflow
1.  Select the **Input > Charges** menu.
    *The Charges - Editor dialog opens.*
2.  Mark the stockplates.
3.  Enter the charge in the field at the lower right.
4.  Activate the checkbox on the left side if the charge should apply for all stockplates of the glass item.
5.  Save the entries with **[Exit]**.

## Optimization

| Help Card | Topics |
| :--- | :--- |
| - Selecting batches and glass types | - You select glass type and batch for table optimization. |
| - Create table optimization | - You create a table optimization. |
| - Selecting stockplates | - You select other stockplates for the optimization. |
| - Using residual lites | - You use residual plate from the previous optimization. |
| - Adding filler orders | - You add filler orders to the optimization. |
| - Resolve table optimization | - You resolve a table optimization. |
| - Create a quick optimization | - You create a quick optimization. |
| - Linking an optimization | - You are linking two table optimizations. |

### Selecting batches and glass types (RTO 02-001)

#### Objective of this activity
You select glass type and batch for table optimization.

#### Requirements
(None specified)

#### Additional info
(None specified)

#### Workflow
1.  Select **Optimization > Table optimization**.
    *The Select glass for optimization dialog opens.*
2.  In the **Available glass types** area, select the desired glass type.
3.  Enable the **Permit manual cutting** checkbox to show even glass types that are only meant to be cut manually.
4.  In the **Available optimizations** area, select the optimizations to be arranged in a table optimization.
5.  Click **[Select]** to compile the selected batches in a table optimization.
6.  Dialog **Table optimization** appears in which the tab **Optimize** shows the selected batches.

### Create table optimization (RTO 02-002)

#### Objective of this activity
You create a table optimization.

#### Requirements
- Batches are selected for a table optimization.

#### Additional info
(None specified)

#### Workflow
1.  From the **Table optimization** dialog, select the **Optimize** tab.
2.  Select the necessary optimization parameters.
3.  Select the required parameter from tab **Stockplates**.
4.  Select the required parameters from the **Filler** tab.
5.  Return to the **Optimize** tab and click the **[Optimize]** button.
    *The calculation of the optimization starts, the dialog disappears, and the optimization is run in the background. As soon as the optimization result is available, the dialog reappears automatically.*
6.  Click **[Save]** to save the optimization.

### Selecting stockplates (RTO 02-003)

#### Objective of this activity
You select other stockplates for the optimization.

#### Requirements
(None specified)

#### Additional info
(None specified)

#### Workflow
1.  From the **Table optimization** dialog, select the **Stockplates** tab.
2.  Mark the stockplate or stockplates in the right area that can be used for cutting optimization.
3.  Return to the **Optimize** tab and click the **[Start]** button.
4.  Click **[Save]** to save the optimization.

### Using residual lites (RTO 02-004)

#### Objective of this activity
You use residual plate from the previous optimization.

#### Requirements
(None specified)

#### Additional info
(None specified)

#### Workflow
1.  From the **Table optimization** dialog, select the **Stockplates** tab.
    *If there is a residual plate of the same glass type and thickness on the cutting table as required in the present optimization, this can be integrated in the table optimization.*
2.  Enter the height and width of the residual plate on the cutting table in section **Residual plate**.
3.  Return to the **Optimize** tab and click the **[Start]** button.
4.  Click **[Save]** to save the optimization.

### Adding filler orders (RTO 02-005)

#### Objective of this activity
You add filler orders to the optimization.

#### Requirements
(None specified)

#### Additional info
- Filler orders can be used only if A+W Production is used together with A+W Production. In this case, filler orders are directly taken from the A+W Production database.

#### Workflow
1.  From the Table optimization dialog, select the **Filler** tab.
    *The list on the right shows all filler orders defined for the glass type and thickness of this batch.*
2.  Mark the filler orders to be integrated into the table optimization.
3.  Return to the **Optimize** tab and click the **[Optimize]** button.
4.  Continue to add or delete filler orders until the optimal result is reached.
5.  Click **[Save]** to save the optimization.

### Resolve table optimization (RTO 02-006)

#### Objective of this activity
You resolve a table optimization.

#### Requirements
- Table optimizations can be resolved only if they were saved after having been created.

#### Additional info
- You can recognize (table)optimizations created by A+W Production by the batch number >15000. Batches generated and released by A+W Production or A+W Business Pro have batch numbers 1000 - 9999.

#### Workflow
1.  This is done on the **Optimization > Reset** menu.
    *The Resetting a cutting batch dialog opens.*
2.  Mark the table optimization you want to resolve. Mark the corresponding batch with a number higher than 15000.
    *You can mark several table optimizations to be resolved at the same time.*
3.  To resolve the table optimization, click the **[OK]** button.
    *A security query appears.*
4.  Confirm the security query with **[Yes]**.
5.  The batches and lites of the selected table optimization are now available for new table optimizations.

### Create a quick optimization (RTO 02-007)

#### Objective of this activity
You create a quick optimization.

#### Requirements
- Table optimization must be cut.

#### Additional info
- The broken lites can be optimized again before the next, free pattern (quick optimization). In the figure to the right, this means patterns 1 and 2 must already be cut before pattern 3.

#### Workflow
1.  Select the **Cutting overview** dialog.
    *The cutting is started.*
2.  On the **Production Terminal (XTV)**, mark the lites that have broken.
3.  Change back to the **Cutting overview**.
4.  Open the context menu in the overview.
    *The message `Resolve optimization XX Batch X starting with Pattern XY and reoptimize` appears.*
5.  Confirm the message.
    *The lites still to be cut will be removed first.*
6.  Then, the broken lites and the plates still to be cut will be re-optimized.

### Linking an optimization (RTO 02-008)

#### Objective of this activity
You are linking two table optimizations.

#### Requirements
- Table optimizations must exist.

#### Additional info
- The batch numbers for table optimization are from 15000 - 15999.

#### Workflow
1.  Select the **Cutting > Cut optimization** menu.
    *The Select a batch dialog opens.*
2.  In the **Batches** area, mark the first batch and then click **[Options]**. The dialog **Batch: XX** opens.
3.  In the **Reject optimization** area, select the entry **Mix**.
    *In case of rejects, these are then also optimized automatically.*
4.  In the **Residual lite management** area, select the entry **Mix**.
5.  Click **[Cut]**.
    *The cutting overview opens.*
6.  Click **[Start]** to start the cutting.
    *If rejects occur, you can mark them accordingly directly on the A+W Production Terminal XTV.*
    *If A+W Production Terminal XTV has arrived at the last pattern (residual sheet), the Select rejects dialog appears automatically.*
7.  Click **[OK]**.
    *The dialog for linking the batches appears automatically. The optimizations with which the residual lite can be filled up are always available for selection.*
8.  Select the second table optimization and click **[Use]**.
    *The optimization result is displayed.*
    *Click **[Link]** to confirm.*

## Cutting

| Help Card | Topics |
| :--- | :--- |
| - Select batches | - You select batches for cutting. |
| - Cutting batches again | - You can cut batches again. |
| - Skip pattern | - You skip a pattern. |
| - Do not generate a cutting code | - You suppress cutting code creation. |
| - Interrupt cutting | - You interrupt the cutting within an optimization. |

### Select batches (RTO 03-001)

#### Objective of this activity
You select batches for cutting.

#### Requirements
(None specified)

#### Additional info
Batches with the numbers 1000-9999 come from an upstream system and contain one or more optimizations. Batches starting from number 15000 contain table optimizations created by Realtime Optimizer.

#### Workflow
1.  Select the **Cutting > Cut optimization** menu.
    *Dialog Select a batch opens.*
2.  Select the desired batch from the **Batches** list.
    *The Optimization list shows the optimizations existing for this batch.*
3.  Select one or all optimizations.
4.  Click **[OK]**.
    *The tagged optimizations are selected for cutting and shown in dialog Batch [number -] - batch [number].*
5.  Click on **[OK]** to close the dialog.
6.  Click the **[Start]** icon to start the cutting.

### Cutting batches again (RTO 03-002)

#### Objective of this activity
You can cut batches again.

#### Requirements
(None specified)

#### Additional info
- When all stockplates of an optimization have been cut, the entire batch gets the status **Produced**. This status can be reset to status **Released**, and the entire batch can be cut again.

#### Workflow
1.  This is done in the **Optimization > Reset** menu.
    *The Resetting a cutting batch dialog opens.*
2.  Select the batch you want to reset from status **Produced** to status **Released**.
    *You can mark several batches, and reset them together.*
3.  Click **[OK]** to reset the batch.
4.  The batch is now available again for cutting as a complete optimization.

### Skip pattern (RTO 03-003)

#### Objective of this activity
You skip a pattern.

#### Requirements
(None specified)

#### Additional info
- If you choose **Skip pattern** for a lite, no cutting code will be created, and no breakout pattern will be shown for this lite.
- Only lites can be skipped that are not already in the status **Cut**.

#### Workflow
1.  Select the **Cutting > Cut optimization** menu.
    *The Select a batch dialog opens.*
2.  Select the corresponding batch.
3.  Click **[Options]** to open the **Batch> Number** dialog.
4.  Mark in the **Optimizations** list the glass type for which individual stockplates should be cut again.
5.  In the **Lites** section, click the lite to be skipped during cutting.
6.  Open the context menu and select the **Skip pattern** entry.
    *Click [OK] to close the dialog.*

### Do not generate a cutting code (RTO 03-004)

#### Objective of this activity
You suppress cutting code creation.

#### Requirements
(None specified)

#### Additional info
- If you select **Do not send cutting code** for a lite, the system will create no cutting code, but the breakout pattern will be shown in A+W Production Terminal (XTV).
- You can send no cutting code only for lites with a status other than **Cut**.

#### Workflow
1.  Select the **Cutting > Cut optimization** menu.
    *The Select a batch dialog opens.*
2.  Select the corresponding batch.
3.  Click **[Options]** to open the **Batch: Number** dialog.
4.  Tag in the **Optimizations** list the glass type for which individual stockplates should be cut again.
5.  In the **Lites** area, click the lite for which no cutting code should be sent.
6.  Open the context menu and select the **Do not send cutting code** entry. The reject display appears on the Production Terminal (XTV).
7.  Click **[OK]** to close the dialog.

### Interrupt cutting (RTO 03-005)

#### Objective of this activity
You interrupt the cutting within an optimization.

#### Requirements
- Cutting must be started.

#### Additional info
(None specified)

#### Workflow
1.  The **Cutting overview** dialog is open.
2.  Click **[Stop]** to stop cutting.

---
# A+W Production Terminals

### Revision overview of the module

| Date | Additions |
| :--- | :--- |
| 01-2023 | Additions |
| 01-2016 | Remake management added |
| 09-2014 | Terminal Georgian Bars added |
| 04-2013 | Terminal LG and Edit added |
| 01-2012 | Original version |

This module provides information on the following subjects:
- ⇨ Tutorial
- ⇨ Software Reference

## Tutorial

This section provides information on the following subjects:
- ⇨ Overview
- ⇨ Production Terminal Systems
- ⇨ Overview Production Terminal: IG
- ⇨ Overview Production Terminal Manual Cutting
- ⇨ Overview Production Terminal Georgian Bars
- ⇨ Overview Production Terminal: Order
- ⇨ Overview Production Terminal: Processing
- ⇨ Overview Production Terminal: TG
- ⇨ Overview: Production Terminal TG-Out
- ⇨ Overview Production Terminal LG
- ⇨ Overview Production Terminal Edit

### Table of Contents

- **Overview** (L-1297)
- **Tutorial Structure** (L-1297)
- **Production Terminal Systems** (L-1298)
- **Goals of the Production Terminal Technique** (L-1300)
- **Operation of the Production Terminals** (L-1300)
- **Overview Production Terminal: IG** (L-1301)
  - Using Production Terminal IG-In (L-1302)
    - Module Presentation: Production Terminal IG-In (L-1303)
    - Detailed annotations on the individual sections (L-1304)
    - Operating Sequence (L-1307)
      - Loading a lot (L-1309)
      - Changing the machine status (L-1310)
      - Handling of defective lites (L-1311)
      - Loading another item number (L-1312)
      - Loading a remake (L-1313)
    - Additional functions (L-1314)
      - Creation of lists (reports) (L-1314)
      - Export of log entries (L-1314)
      - Choose program language (L-1315)
  - Using Production Terminal IG-Assembly (L-1316)
    - Module Presentation: Production Terminal IG-Assembly (L-1317)
    - Detailed annotations on the individual sections (L-1318)
    - Operating sequence (L-1320)
      - Register at the workstation (L-1320)
      - Changing the machine status (L-1321)
      - Handling of defective lites (L-1321)
      - Skipping a unit (L-1321)
    - Additional functions (L-1321)
  - Using Production Terminal IG-Out (L-1323)
    - Module presentation: Production Terminal IG-Out (L-1324)
    - Detailed annotations on the individual sections (L-1325)
    - Operating sequence (L-1326)
      - Register at the workstation (L-1326)
      - Input of batches (L-1326)
      - Changing the machine status (L-1327)
      - Handling of defective lites (L-1327)
    - Remake management (L-1327)
      - Procedure (L-1328)
- **Overview Production Terminal Manual Cutting** (L-1331)
  - The use of Production Terminal Manual Cutting (L-1332)
    - Module presentation: Production Terminal Manual Cutting (L-1333)
    - Detailed annotations on the individual sections (L-1334)
    - Release a batch (L-1335)
    - Using the rejects pool (L-1337)
    - Adding a lite to the rejects pool by hand (L-1339)
  - Operating sequence (L-1340)
    - Register at the workstation (L-1340)
    - Input of charges (L-1341)
    - Changing the machine status (L-1342)
    - Handling of defective lites (L-1342)
    - Additional functions (L-1342)
- **Overview Production Terminal Georgian Bars** (L-1343)
  - Using Production Terminal Georgian Bars (L-1344)
    - Module presentation Production Terminal Georgian Bars (L-1345)
    - Detailed annotations on the individual sections (L-1346)
    - Release a batch (L-1347)
  - Operating sequence (L-1349)
    - Register at the workstation (L-1349)
    - Input of charges (L-1350)
    - Changing the machine status (L-1350)
    - Additional functions (L-1350)
- **Overview Production Terminal: Order** (L-1351)
  - Using Production Terminal Order (L-1352)
    - Module presentation: Production Terminal Order (L-1353)
    - Detailed annotations on the individual sections (L-1354)
  - Operating sequence (L-1357)
    - Register at the workstation (L-1357)
    - Input of charges (L-1358)
    - Changing the machine status (L-1358)
    - Handling of defective lites (L-1359)
    - Additional functions (L-1359)
- **Overview Production Terminal: Processing** (L-1360)
  - Using Production Terminal Processing (L-1361)
    - Module Presentation: Production Terminal Processing (L-1362)
    - Detailed annotations on the individual sections (L-1363)
  - Operating sequence (L-1366)
    - Register at the workstation (L-1366)
    - Input of charges (L-1368)
    - Changing the machine status (L-1368)
    - Handling of defective lites (L-1368)
    - Additional Functions (L-1369)
- **Overview Production Terminal: TG** (L-1370)
  - Using Production Terminal TG-In (L-1371)
    - Module Presentation: Production Terminal TG-In (L-1372)
    - Detailed annotations on the individual sections (L-1373)
    - Moving or turning lites on the furnace bed (L-1374)
  - Operating sequence (L-1375)
    - Register at the workstation (L-1375)
    - Input of batches (L-1377)
    - Changing the machine status (L-1377)
    - Handling of defective lites (L-1377)
    - Additional functions (L-1377)
- **Overview: Production Terminal TG-Out** (L-1378)
  - Using Production Terminal TG-Out (L-1379)
    - Module presentation: Production Terminal TG-Out (L-1380)
    - Detailed annotations on the individual sections (L-1381)
  - Operating sequence (L-1383)
    - Register at the workstation (L-1383)
    - Input of batches (L-1384)
    - Changing the machine status (L-1384)
    - Handling of defective lites (L-1384)
    - Additional functions (L-1384)
- **Overview Production Terminal LG** (L-1385)
  - Using Production Terminal LG-In (L-1386)
    - Module presentation Production Terminal LG-In (L-1387)
    - Detailed annotations on the individual sections (L-1388)
  - Operating Sequence (L-1389)
    - Register at the workstation (L-1389)
    - Loading a lot (L-1390)
    - Input of batches (L-1390)
    - Changing the machine status (L-1391)
    - Replacing damaged lites (L-1391)
    - Additional Functions (L-1391)
- **Using Production Terminal IG-Assembly** (L-1392)
  - Module Presentation: Production Terminal IG-Assembly (L-1393)
  - Detailed annotations on the individual sections (L-1394)
  - Operating sequence (L-1395)
    - Register at the workstation (L-1395)
    - Input of batches (L-1395)
    - Changing the machine status (L-1395)
    - Handling of defective lites (L-1395)
    - Additional functions (L-1396)
- **Overview Production Terminal Edit** (L-1397)
  - Using Production Terminal Edit (L-1398)
    - Module presentation: Production Terminal Edit (L-1399)
    - Detailed annotations on the individual sections (L-1400)
  - Operating sequence (L-1403)
    - Register at the workstation (L-1403)
    - Additional functions (L-1405)

### Overview

The training on the **Production Terminal** modules is designed for employees working at the corresponding registration points on the shop floor.

We are going to convey to the users how our software shall help him perform his work more efficiently and more easily, and what to do in case of defects etc.

> **Required knowledge**
> Basic IT knowledge and/or Windows knowledge are prerequisite for using the corresponding modules. The user has to know what the physical work processes and process steps at the terminal in question look like, and how to execute them. Basic IT knowledge and/or Windows knowledge are prerequisite for using the corresponding modules. The user has to know what the physical work processes and process steps at the terminal in question look like, and how to execute them.

### Tutorial Structure

This tutorial consists of sets of topics with several sessions each. Each session consists of the following parts:

- **Overview:** Each training session starts with an overview of the major topics:
  - **Objectives:** What shall be conveyed?
  - **Benefit:** What can this knowledge be used for?
  - **Maxims:** Which correlations are to be remembered?
- **Concepts:** Concepts and terms of the corresponding training session will be explained first. This is followed by examples and operating instructions.

#### Reading instructions

The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend that you do not skip any learning units.

If you are already familiar with a subject you should at least read the summary at the start of the session in order to bring the main details to mind.

The practical part of each training unit automatically includes the software reference and the exercises on the cross references. This will provide a central thread through the entire documentation.

### Production Terminal Systems

The **Production Terminals** are software modules of the production control system **A+W Production** that serve to check, enter, modify, control, and divert process steps in the work flow.

The Production Terminals visualize and control individual processing steps and can be configured individually. Labels and reports can be printed online at all Production Terminals; rejects can be entered with all the necessary information. Handling the Production Terminals is easy and uniform. These intelligent systems enable you to inform your customers of the current state of his products at any time.

Below please find a schematic diagram of a possible Production Terminal landscape:

*Fig. L-1: Overview: Production Terminals*

As every workstation on the shop floor requires different information, there are standard terminals configured for the various processes and work flows.

#### A brief explanation of the individual Terminals:

- **Terminal Manual Cutting:** Visualizes the work schedule for the lites to be cut at the manual cutting table.
- **Terminal Order:** Is used wherever large quantities are to be booked.
- **Terminal Processing:** Is the production terminal version used with the processing machinery, automatically controlling the machines. This module provides detailed information on the processing steps to be performed including true-to-scale production drawings.
- **Terminal IG-In:** Is installed at the IG line entrance and visualizes the work schedule for the lites of a batch or of a logical production rack/harp rack, in production sequence.
- **Terminal IG-Assembly:** Is installed between the visual check of lites after the washer, and in front of the spacer applicator, visualising the technical data including the spacer data for each unit to be produced.
- **Terminal IG-Out:** Installed at the IG line exit and shows the technical and shipping-related data for each unit produced.
- **Terminal TG-In:** Is the display system at the furnace entry. It shows the furnace bed load and is controlled by the operator. All lites are scanned; their geometry is checked for completeness of processing.
- **Terminal TG-Out:** This is the display system at the furnace exit. All lites registered at the furnace entry are displayed based on the clock rate. If defined, the user will get information as to the further use or on stacking in the shipping area.
- **Terminal Edit:** Is the control station version that is normally used in the shipping office for rebooking units, lites, or groups and for managing off-site racks.
- **Terminal LG-In:** Installed at the laminating line entrance, it visualizes the work schedule for the lites of a batch or a logical production rack/harp rack to be produced, in production sequence.
- **Terminal LG-Assembly:** Installed in the cleanroom, it shows the work schedule after a lite or unit has been booked at Terminal LG-In. This leaves ample time for cutting the necessary film layers.

### Goals of the Production Terminal Technique

The following goals shall be achieved by means of the production terminal technique:
- Scheduled and optimized jobs or batches are distributed to the appropriate workstations.
- The workers at the machines are provided with graphical information on all relevant details of the lites (shape, alignment, sizes, processing).
- The work performed is booked.
- Deviations from detailed scheduling are registered.
- Scheduled and actual production processes are compared during production.
- The production process is visualized.
- Remakes (due to rejects) are created automatically.
- The workers at the machines are provided with all relevant information on the lites (shape, alignment, sizes, processing).
- The production process can be re-optimized manually.
- The collected data are used for analyses.

Each of the production terminal modules provides special support for one of these goals.

> **Performance counter**
> In the Production Terminals, additional fields can now be displayed that show the produced quantity, area and linear meters for a certain time at a recording point (e.g. a shift). Please contact an A+W employee.

### Operation of the Production Terminals

To use the production terminal technology to the best effect, barcodes are registered in all relevant places. The appropriate workstations or machines are equipped with barcode scanners. A barcode scanner is firmly allocated to a workstation (registration point). Barcodes serve to identify production factors, processes, or states such as:
- Lites (individual or groups)
- Racks
- Employee
- Processing
- Rejects

If a rack barcode is scanned for example, the software will book the corresponding rack automatically to a defined processing station.

If the same scanner is used to scan a lite barcode, the software books the lite e.g. to the currently registered rack.

System configuration defines the actions to be performed automatically upon scanning the barcodes.
