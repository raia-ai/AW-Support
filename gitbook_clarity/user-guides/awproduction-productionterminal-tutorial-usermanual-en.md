---
description: "EN_UM_AWProduction_15"
---


# A+W Production Production Terminals

---
## Tutorial

### Overview Production Terminal Edit

> **Image:** A screenshot of the Production Terminal Edit interface with several sections labeled A, B, C, D, E, and F. The table shows production data grouped by glass type.

-   **A Grouping area**
-   **B Grouping and sorting**
-   **C Table header**
-   **D Table header**
-   **E Fields for the table header**
-   **F Button for showing/hiding the group contents**

In section (A), the loaded data can be grouped and sorted within the groups. To define a group, click on the required field in the table header (e. g. glass type) and keep pressing the mouse key. Still pressing the mouse key, move the field to the grouping area and release the mouse key. Your table header will look like this now:

> **Image:** A simplified table header showing fields like 'Reg. Point', 'Order', 'Item', etc., with 'Glass Type' moved to the grouping area.

Adding a sorting to the group is done in just the same way. Click on the required field in the table header (e.g. old rack) and, keeping the mouse key pressed, drag the field upwards to the grouping area. Your table header will look like this now:

> **Image:** A simplified table header showing 'Glass Type' and 'Old Rack' in the grouping area, indicating sorting.

Use the icon Columns to open the following selection dialog:

> **Image:** The 'Column Chooser' dialog, which allows users to drag and drop columns onto the header or group box. Available columns include 'Rack', 'Order', 'Itm', 'Label', 'Reg. Point', 'Part', 'Prev. Booking', and 'Stacking Time'.

You can click on the individual fields and, keeping the mouse key pressed, drag the field to the required point of the table header. When you have reached the required point, release the mouse key.

The icons Plus and Minus can be used to show or hide the groups' contents.

(A+W Production Production Terminal L-1401)

### Example of a hidden sorting:

> **Image:** A screenshot showing a table where groups are collapsed (hidden sorting). The group headers are visible (e.g., "A+W Float 4 mm (2 Pieces)"), but the individual items within them are not.

### Example of a displayed sorting:

> **Image:** A screenshot showing a table where a group ("A+W Float 4 mm (2 Pieces)") is expanded, displaying the individual items within it.

### Sections H and K - target data and buttons

There are various ways of loading the target data. Target data can be loaded for the following areas:

-   Registration point types, registration types and racks are identical with the fields in section Target.
-   Status type (group of statuses, e. g. start, defect, machine status, etc.).
-   Status (possible states, e. g. scratch, ready).

Choose the requires entries from the combo boxes in the appropriate areas, e. g. the entry Off site in section Registration point. To load the data, press the button [Add].

### Section I - display of target data

When you have made your selection in section Target, press the button [Add]. The data will appear in this section.

The table header in this section matches the table header in section Source data, which is why it will not be described again at this point.

### Section J - buttons for moving the data

These buttons serve to move data from the source area to the target area and vice versa.

> `>`
>
> `<`

(A+W Production Production Terminal L-1402)

### Section L - buttons

The Refresh button [F2] serves for updating the view.

Button [Reset] is used to clear the view.

> **Image:** Icon for the Reset [F9] button.

Press the Adopt button [F5] to book the data from source to target.

> **Image:** Icon for the Accept [F5] button.

### Operating sequence

The operating sequence in Production Terminal Edit is:

-   Start module Production Terminal Edit.
-   Log in (<Name>).
-   Load the source data.
-   Select the rack for the registration point.
-   Choose the target area.
-   Book the data from source area to target area

### Register at the workstation

The registration process is the same for all workstations. It is described in detail in section Production Terminal IG-In.

⇨ Tutorial, "How to register" on page L-1308

**■ How to load a registration point**
1.  Go to field Reg.point, open the combo box and select the appropriate registration point. Alternatively, you can enter the first number of the registration point. This will produce a list of all registration points starting with this number.
2.  Choose the required registration point.
3.  Press the [Add] button.
4.  The data will be loaded.

**■ How to load a rack**
1.  Go to field Rack, open the combo box and select the required rack. Alternatively, you can enter the first number of the rack. This will produce a list of all racks starting with this number.
2.  Choose the appropriate rack.
3.  Press the [Add] button.
4.  The data will be loaded.

(A+W Production Production Terminal L-1403)

**■ How to load an order, a batch, or a label**
1.  Decide whether you want to load an order number, a batch number, or a label number, then choose the corresponding entry from the combo box, Order, batch, or Label.
2.  Enter the number in the field below.
3.  Press the [Add] button.
4.  The data will be loaded.

**■ How to book a lorry off-site**
1.  Go to section Source and open the combo box Reg. point or RP type. Select the entry Lorry.
2.  Press the [Add] button. The data will be loaded.
3.  In section Target, open the combo box Status. Choose the entry Shipped.
4.  Press the [Add] button. The data will be loaded.
5.  Go to section Source and from the list select the lorry you want to rebook. You can also select all lorries and rebook them by one click.
6.  Press the Transfer button.
7.  The data will be moved from source to target area.
8.  Press the [Adopt] button. The data will be booked.

> **i Data booked by mistake or incorrectly**
> Should you have booked data by mistake you can move them back from the target area to the source area as described above.

(A+W Production Production Terminal L-1404)

**■ How to adjust the table header in the source data area**

The layout of Production Terminal Edit is configured during installation. Should you wish to view additional fields later on or remove redundant fields, please proceed as follows.
1.  Select the registration point or the rack.
2.  Press the [Add] button. The data will be loaded.
3.  Dialog Load order appears.
4.  Choose the required order.
5.  Press the button [Load].
6.  The dialog closes and the system loads the selected order. You are back in the main window.

### Additional functions

Additional functions are for instance:

-   Lists (reports)
-   Log entries
-   Different program languages

As the fields of Production Terminal IG-Out are the same as the fields of Production Terminal IG-In in this section, we are not going to expound on them at this point.

**Additional information**
⇨ Tutorial, "Creation of lists (reports)" on page L-1314
⇨ Tutorial, "Export of log entries" on page L-1314
⇨ Tutorial, "Choose program language" on page L-1315
⇨ Software Reference, "Log entries for this session" on page L-1457

(A+W Production Production Terminal L-1405)

## Software Reference

This section provides information on the following subjects:
⇨ Module Operation
⇨ General Overview
⇨ Overview: Production Terminal IG
⇨ Overview: Production Terminal Manual Cutting
⇨ Overview: Production Terminal Georgian Bars
⇨ Overview: Production Terminal Order
⇨ Overview: Production Terminal Proces-sing
⇨ Overview: Production Terminal TG
⇨ OverviewProduction Terminal LG
⇨ Overview Production Terminal Edit
⇨ Reports
⇨ How to Use the Help Function

### Module Operation
-   Software terms
    -   Buttons L-1410
    -   Radio button L-1410
    -   Combo box L-1410
    -   Menu bar/Menu item L-1411
    -   Key combinations L-1411
-   Closing the program L-1412

### General Overview L-1413

### Overview: Production Terminal IG L-1414
-   Registration L-1415
-   Go to production number L-1416
-   Preview L-1417
-   Batch L-1418
-   Load lot L-1419
-   Booking of rejects L-1421
-   Load remakes L-1423
-   Status L-1425
-   Remake management L-1426
-   Remake management - Edit L-1429

### Overview: Production Terminal Manual Cutting L-1432
-   Release L-1433
-   Rejects pool L-1435
-   Breakage entry L-1437

### Overview: Production Terminal Georgian Bars L-1439
-   Release L-1440

### Overview: Production Terminal Order L-1442
### Overview: Production Terminal Proces-sing L-1443
-   Manual entry L-1444

### Overview: Production Terminal TG L-1445
-   Manual entry L-1446
-   Open processing steps L-1447

### Overview Production Terminal LG L-1449
-   Load order L-1450
-   Go to production number L-1452

### Overview Production Terminal Edit L-1453

### Reports L-1454
-   Parameter input for report L-1455

### How to Use the Help Function L-1456
-   Log entries for this session L-1457
-   Language selection L-1458
-   About Production Terminal L-1459

(A+W Production Production Terminal L-1408, L-1409)

### Module Operation

The modules are either started by a desktop shortcut or by means of the corresponding entry in menu Start > Programs (in Windows).

We are now going to explain the terms used in the manuals, and how to terminate the program.
-   Software terms
-   Closing the program

#### Software terms

This section deals with the general operation of menus and dialogs.
Below you will find information on:
-   Buttons
-   Radio button
-   Combo box
-   Menu bar/Menu item
-   Key combinations

**Buttons**

> **Image:** A 'Reject [F7]' button.

**Radio button**

> **Image:** A set of radio buttons for 'Muntins' with options 'No Muntins', 'Horizontal', and 'Vertical'. 'Vertical' is selected.

From a window with radio buttons you can always select one radio button at a time! In the example above, the radio button Vertical has been selected. Clicking e.g. on the radio button Horizontal will automatically deselect the radio button Vertical.

**Combo box**

> **Image:** A 'Language' combo box showing options 'English (United States)', 'French (France)', and 'German (Germany)'. 'German (Germany)' is selected.

Clicking on the arrow on the right in a combo box will open a selection. Click on an entry to select it. The selected item will be displayed.

(A+W Production Production Terminal L-1410)

#### Menu bar/Menu item

> **Image:** A dropdown menu from the 'File' menu bar item, showing options like 'Re-login [F4]', 'Go to ProdNo [F11]', 'Preview Dialog [F12]', 'Charge [F1]', and 'Exit'.

Also called pull-down menu. To create e.g. a house front, click on the menu item Macros to open the appropriate pull-down menu (see picture above) then on the item House front.

#### Key combinations

Hotkeys are keys or key combinations that are used to call a command or execute a function. Hotkeys will help the skilled user to achieve the required result quickly. A list of the major hotkeys and function keys is shown below:

| Hotkey | Explanation |
| :--- | :--- |
| **[F1]** | Use this function key to enter a batch. Dialog Manual input appears. |
| **[F2]** | Press this function key to load a new lot. Dialog Load lot opens. |
| **[F3]** | This function key serves to change the machine status. Dialog Status appears. |
| **[F4]** | This function key is used to register a person at a machine. Dialog ToolTV registration opens. You can also use this key to switch between different screens. |
| **[F5]** | Press this function key to book the status produced for the current unit. |
| **[F6]** | Press this function key to skip the current unit and display the next unit to be produced. No booking will be made. |
| **[F7]** | Pressing this function key books the current lite as Reject. Dialog Status appears. |
| **[F8]** | Press this function key to load a remake. Dialog Load remakes appears. |
| **[F11]** | This function key serves to load another production number. Dialog Go to production number opens. |
| **[F12]** | This function key starts the preview. Dialog Preview appears. |

**Active and inactive buttons**
You will find that there are the active and inactive buttons in the individual menus. These buttons are enabled or disabled depending on your entries!

(A+W Production Production Terminal L-1411)

#### Closing the program

There are various ways of closing the program.
-   Click on the button [Close] in the top right corner of the program to end the program.
-   Use menu File > End.

> **i Notes on ending the program**
> If data has been changed or if new data has been entered and not saved yet, the program will issue a notice to that effect. Select [Yes] to activate the dialog Save file as .... You can save the file and your changes. The program closes after that. Select [No] to quit the program without saving the file or your changes. Choose [Abort] to stop the End process and go on working with the program.

(A+W Production Production Terminal L-1412)

### General Overview

The software reference provides information on the following subjects:
-   Overview: Production Terminal IG
-   Overview: Production Terminal Manual Cutting
-   Overview: Production Terminal Order
-   Overview: Production Terminal Proces-sing
-   Overview: Production Terminal TG
-   Reports
-   How to Use the Help Function

> **i Dialogs are accessible from different points**
> Please note that there are various ways of opening functions and dialogs. The corresponding dialogs will be described just once in this document.

(A+W Production Production Terminal L-1413)

### Overview: Production Terminal IG

Production Terminal IG is used at the IG line and shows all available lots as well as information that supports production.

The modules Production Terminal IG-In, Production Terminal IG-Assembly, and Production Terminal IG-Out have the same menus:

The software reference provides information on the following subjects:
-   **Menu File, menu entry Reregister:**
    This menu item serves to log into Production Terminal.
    ⇨ Software Reference, “Registration" on page L-1415
-   **Menu File, menu entry Go to ProdNo. [F11]:**
    You can use this menu item to go directly to another production number.
    ⇨ Software Reference, "Go to production number" on page L-1416
-   **Menu File, menu entry Preview dialog [F12]:**
    This menu item opens the Preview dialog.
    ⇨ Software Reference, "Preview" on page L-1417
-   **Menu File, menu entry Batch [F1]:**
    Choose this menu item to allocate batches.
    ⇨ Software Reference, "Batch" on page L-1418
-   **Menu Lists, menu entry Order overview:**
    Use this menu item to print the Order overview report.
    ⇨ Software Reference, "Parameter input for report" on page L-1455
-   **Menu Machine, menu entry Machine status dialog [F3]:**
    Choose this menu item to book interruptions in your work.
    ⇨ Software Reference, "Status" on page L-1425
-   **User help:**
    This menu item starts the short descriptions.
-   **Current log entries:**
    This menu item is used to start the log file. This file includes the log entries for the corresponding session.
    ⇨ Software Reference, "Log entries for this session" on page L-1457
-   **Change language:**
    This menu item serves to change the menu language. Dialog Change language appears.
    ⇨ Software Reference, "Language selection" on page L-1458
-   **Information:**
    This menu item can be used to display more information on the modules. Dialog Version Info opens.
    ⇨ Software Reference, "About Production Terminal" on page L-1459

(A+W Production Production Terminal L-1414)

#### Registration

**File > Reregister** or use the function key **F4**

> **Image:** Fig. L-24 Register. The 'Change Person' dialog with fields for 'User' and 'Station', and buttons 'OK [F5]' and 'Cancel [F6]'.

This dialog has two functions. It appears automatically whenever you start the program. Enter your name in field User. The corresponding Production Terminal module starts. Should a Production Terminal module be running already you can use this dialog to register another user (e.g. change of user).

> **i Scan your name**
> When working with a scanner you can scan your name right in the main window - Person - without the need to open the dialog ToolTV Registration.

**Description of fields**
-   **User:** Select the required user from the combo box.
    Technical info: Mandatory field, selection
-   **ToolTV:** Select the production terminal you want to register at from the combo box.
    Technical info: Mandatory field, selection

**Description of buttons**
-   **OK:** When you have made the required selections in the fields User and ToolTV, press [OK] to open the corresponding production terminal. In this case, Production Terminal IG-In opens.
-   **Cancel:** Press this button to close the dialog.

**Additional information**
⇨ Tutorial, "How to register" on page L-1308

(A+W Production Production Terminal L-1415)

#### Go to production number

**File > Go to ProdNo.** or use the function key **F11**

> **Image:** Fig. L-25 Go to production number. The 'Go to Production Number' dialog with an input field 'New Production Number' and buttons 'OK [F5]' and 'Cancel [F6]'.

This dialog can be used to load another production number. The production number determines the sequence of the units to be produced. You can e.g., go directly from production number 3 to production number 15 without having to press the [Skip] button several times. This may be the case if remakes are underway.

**Description of fields**
-   **Production number:** Use the cursor keys to select the production number to be produced next.

**Description of buttons**
-   **OK:** Press this button to adopt the selected production number.
-   **Cancel:** Press this button to close the dialog. The selected production number will not be adopted.

**Additional information**
⇨ Tutorial, "Loading another item number" on page L-1312

(A+W Production Production Terminal L-1416)

#### Preview

**File > Preview dialog** or use the function key **F12**

> **Image:** Fig. L-26 Preview. The 'Preview' dialog showing a workload for a registration point. It has two tables: one for batches/lots and another for the items within the selected batch. Radio buttons for filtering (All, Available, Scheduled, Possible) are present.

This dialog shows the workload for the corresponding registration point and the present day. You can use the radio buttons to restrict the view.

**Description of fields**
-   **Registration point:** This field shows the registration point the preview refers to.
-   **All:** Activate this radio button to view all lites at once.
-   **Available:** Activating this radio button displays only the currently available lites.
-   **Scheduled:** Activate this radio button to view all scheduled lites.
-   **Possible:** Activate this radio button to display only lites that can be processed.

**Description of buttons**
-   **Close:** Press this button or use the function key [F5] to close the dialog.

(A+W Production Production Terminal L-1417)

#### Batch

**File > Batch** or use the function key **F1**

> **Image:** Fig. L-27 Batch. The 'Manual Entry' dialog with a 'Charge' input field for the batch name.

You can use this dialog to allocate batches. Batches are used for quality assurance and quality monitoring. For Production Terminal IG-Assembly for example, a barrel of butyl would be a possible batch at the visual check.

**Description of fields**
-   **Batch:** Enter the batch name in this field. Alpha-numerical entries are valid.

**Description of buttons**
-   **OK:** Press this button to adopt the defined batch.
-   **Cancel:** Press this button to close the dialog. The defined batch will not be adopted.

**Additional information**
⇨ Tutorial, "How to define batches" on page L-1320

(A+W Production Production Terminal L-1418)

#### Load lot

**ToolTV IG-In > [Load lot]** or use the function key **F2**

> **Image:** Fig. L-28 Load lot. The 'Load Lot' dialog showing a list of batches on the left and the parts for the selected batch on the right. Buttons include 'Remove Lot', 'Update [F2]', 'Load [F5]', and 'Show All'.

This dialog shows the batches to be processed including all the included lots. The dialog consists of two sections.

The left section shows a list of all batches to be processed. When you select a batch, the right section shows the units belonging to the batch, and the number of the rack they can be found on. If you do not have access to all the rack numbers listed for the job you can load only the available rack numbers.

> **i Delete the filter**
> Production Terminal IG-In remembers the last processed batch. This is why you have to delete the filter to see all batches. To delete the filter, press [Show all]. You will see the complete list of batches.

(A+W Production Production Terminal L-1419)

**Description of fields**
-   **Batch:** This columns shows all batches to be produced by the registered machine.
-   **Lot:** This column shows the numbers of the lots included in the batch.
-   **Pcs:** This column tells you how many units have to be produced. A unit consists of at least two lites.
-   **Text:** This column shows the glass name. The glass name is defined in and loaded from master data.
-   **Lock:** If lites of a batch are already being processed by another machine, this column shows the name of this machine. These lites will be locked for processing on your machine.
-   **Rack:** This column shows the logical rack (rack number) that holds the lites.
-   **Glass type:** This column shows the glass name.
-   **Parts:** This column shows the number of lites.

**Description of buttons**
-   **Show all:** Press this button to delete the filter for displaying the batches. All batches to be produced will be shown.
-   **Remove lot:** This button will remove old, redundant batches that do not have to be produced.
-   **Update:** Press this button to update the dialog.
-   **Load:** Press this button to load the selected batch.
-   **Cancel:** Press this button to close the dialog. No batch will be loaded.

**Additional information**
⇨ Tutorial, "Loading a lot" on page L-1309

(A+W Production Production Terminal L-1420)

#### Booking of rejects

**ToolTV IG-In > Select unit > [Reject]** or use the function key **F7**

> **Image:** Fig. L-29 Booking of rejects. The 'Status' dialog showing a list of reasons for rejection, such as 'Rejects', 'Damage', 'Scratch(es)', etc.

This dialog is used to book the selected lite as Reject. If you are working with automatic remakes, remakes will be initiated for all parts of the unit.

**Description of fields**
-   **Unit:** Barcode number of the unit to be reported broken.
-   **Breakage reasons:** List of selectable reasons for rejects. Reasons for reject are defined at system configuration. Possible reasons are:
    -   Breakage
    -   Defect
    -   Scratches
    -   Wrong size
    -   Wrong glass type
    -   Scratch (user)
    -   Partial reject

> **i Automatic remakes**
> For some reject types, remakes are created automatically. This can be configured as required. The machine operator has to know these appropriate rules.

(A+W Production Production Terminal L-1421)

**Description of buttons**
-   **OK:** Press this button to adopt the selected reason of reject.
-   **Cancel:** Press this button to close the dialog. The selected reason of reject will not be adopted.

**Additional information**
⇨ Tutorial, "Handling of defective lites" on page L-1311
⇨ Tutorial, "Handling of defective lites" on page L-1311

(A+W Production Production Terminal L-1422)

#### Load remakes

**ToolTV IG-In > [Remakes]** or use the function key **F8**

> **Image:** Fig. L-30 Load remakes. The dialog for loading remakes with a field to enter a barcode ('001042408') and a list below showing the corresponding order, item, and label number.

This dialog serves to load remakes. First, enter the label number by hand or scanner. You can even enter several label numbers in a row.

**Description of fields**
-   **Barcode:** Enter the label number of the remake or scan a label.
-   **Accept [F2]:** After entering or scanning the label number, press this button. The corresponding data appears in the field below.
-   **Order:** Shows the order number for the remake.
-   **Itm:** Shows the item number of the remake.
-   **Label:** This field shows the label number.

(A+W Production Production Terminal L-1423)

**Description of buttons**
-   **Load:** Press this button to close the dialog and load the selected remake.
-   **Cancel:** Press this button to close the dialog. The remake will not be loaded.

**Additional information**
⇨ Tutorial, "How to load remakes" on page L-1313
⇨ Tutorial, "Loading a remake" on page L-1313

(A+W Production Production Terminal L-1424)

#### Status

**Machine > Machine status**

> **Image:** Fig. L-31 Status. The 'Status' dialog showing a list of machine statuses, such as 'Ready', 'Logged off', 'Break', 'Maintenance', etc.

The basis for an expressive analysis of machine data is the correct registration of the machine status.

If the machine is defective, staff is missing, the machine needs servicing, or if production can be resumed, this needs to be registered.

**Description of fields**
-   **No.:** This field shows the status number. The valid statuses have to be configured.
-   **Name:** This field shows the status names. The valid statuses have to be configured.

**Additional information**
⇨ Tutorial, "How to change the machine status" on page L-1310

(A+W Production Production Terminal L-1425)

#### Remake management

**Extras > Remake management**

> **Image:** Fig. L-32 Remake management. A complex dialog showing an 'Overview' of remake items at the top and 'Details' of a selected item's Bill of Materials (BOM) at the bottom.

This dialog displays the remake items for which you must still decide how they should be added to the production and which parts are to be reused if necessary. For such a remake item, a status booking of the type Partial reject is generated.

**Description of the fields in section Overview**
-   **PP:** This field displays whether the part in question is an ordered part. In this case, a blue dot appears in the field.
-   **Label:** This field shows the label number.
-   **Order:** This field shows the order number.
-   **Itm.:** The order item number is displayed in this field.
-   **Pltm.:** This field displays the production item number.
-   **Part:** This field shows the part number.
-   **Description:** This field displays the part description.
-   **Name:** This field displays the reject reason.

(A+W Production Production Terminal L-1426)

-   **Booking time:** This field displays when the booking was made.
-   **Registration Point:** This field displays the registration point at which the reject arose.
-   **Info:** This field displays the info text that was entered.
-   **Employee:** This field displays the employee who booked the reject.

**Description of buttons**
-   **Reallocation:** If you press this button, you can assign the lite another reject reason and enter additional information.
-   **Reuse:** If you press this button, the whole part can be reused. That is, the part receives the procurement type Reuse and disappears from the display.
-   **PS remake:** If you press this button, a completely new production item will be generated in the order pool with the original procurement types. The quantity of the old production item will be reduced so that the total quantity of the order item matches again.
-   **Direct remake:** If you press this button, a direct remark will be triggered for the part. That is, an entry for the part will be generated in the reject pool (global reject management) so that the lite can be recut automatically.

**Explanation of the combo box**
-   **Filter:** With this combo box, you have the opportunity to filter the data displayed according to individual statuses in the remake management.

**Description of the fields in the Details section**
If in the Overview section you select a lite, the entire BOM below the item will be displayed here. This way, you can also make a decision for the associated parts about how they should be treated.
-   **Processed:** This field displays whether the part in question is an ordered part. In this case, a blue dot appears in the field.
-   **PP:** This field displays whether the part in question is an ordered part. In this case, a blue dot appears in the field.
-   **Procurement type:** This field displays the procurement type.
-   **PS remake:** If this checkbox is activated, a new production item is generated in the order pool.
-   **RP:** This field displays the registration point to which the lite should be booked.
-   **Rack:** This field displays the name of the rack to which the lite should be booked.

(A+W Production Production Terminal L-1427)

-   **Name:** This field shows the reject reason.
-   **Defect location:** This field displays the defect location if this was selected.
-   **Label:** This field shows the label number.
-   **Part:** This field shows the part number.
-   **Description:** This field displays the part description.
-   **Batch:** This field shows the batch number.
-   **Prod. Date:** This field shows the production date.

**Description of buttons**
-   **Update:** If you press this button, the screen will be refreshed. It is also possible to set a time after which the screen will be refreshed automatically.
-   **Process:** If you press this button, the Processing dialog opens for the BOM element that you have selected in the Details section.
-   **Undo:** If you press this button, the last action performed will be undone.
-   **Undo all:** If you press this button, all actions that you have performed on the part will be undone.
-   **Save:** If you press this button, the actual booking will be made according to the settings made. That is, as long as you have not yet pressed this button, nothing was written to the database and you can still undo actions.
-   **Close:** Press this button to close the dialog.

**Additional information**
⇨ Software Reference, “Remake management - Edit" on page L-1429
⇨ Tutorial, "Remake management" on page L-1327

(A+W Production Production Terminal L-1428)

#### Remake management - Edit

**Extras > Remake management > [Edit]**

> **Image:** Fig. L-33 Remake management - edit. The 'Edit' dialog allows for detailed settings for an individual part of a remake, including procurement type, registration point, and processing steps.

On this dialog, you can make the precise settings for each individual part.

**Description of fields**
-   **Procurement type:** In this field, you can use the combo box to change the procurement type of the selected part. You can choose either the original procurement type or the Reuse procurement type. If you select Reuse, then the Registration Point and Rack fields below are released for processing.
-   **Registration Point:** If the part can be reused, you select the place here where you store the part until reuse. This information can be displayed in the Production Terminals.
-   **Rack:** If the part can be reused, in addition to the registration point, you can also specify the rack on which the part to be reused is located. This information is displayed during reproduction of the entire IGU on the Production Terminal IG-in instead of the logical rack number.

(A+W Production Production Terminal L-1429)

-   **Defect reason:** If the part cannot be reused and the procurement type Production was selected, then you can select the real reason for the reject here. This can be used later on for statistical evaluations.
-   **Defect location:** In addition to the reject reason, you can specify a defect location here. This can be selected regardless of the registration point at which the defect happened.
-   **PS remake:** If this checkbox is activated, a new production item is generated in the order pool.

**Description of the fields in section Processings**
This section contains all processings that were already booked on the lite in question.
-   **Repeat:** By placing the checkmark in this column, the processings are reset so that you can book them again.
-   **Articles:** This field shows the article number.
-   **ProcNo:** This field shows the processing number.
-   **Processing:** This field shows the processing name.

**Description of the fields in section Possible parts**
In this area, you can see all parts that enter into question for the selected part. That is, you must select a label number from this list that should run together as counterlite with the remake. Ideally here you should use a label number that is not yet in production. If this is not possible, the selected label number must be removed from production so that an unintentional use of this label number is avoided. The assignment of a label number is only required if the parts were not already assembled before this. In this case, unique label number have already been assigned.
-   **Select:** By placing a checkmark in this column, precisely these processings are reset in the PDC table so that you can rebook them.
-   **Label:** This field shows the label number.
-   **Registration point:** This field shows the registration point.
-   **Rack:** This field shows the rack name.
-   **Batch:** This field shows the batch number.
-   **Last Booking:** This field displays when the last booking was made.
-   **Status:** This field shows the status.
-   **Description:** This field shows the article description.

(A+W Production Production Terminal L-1430)

**Additional information**
⇨ Software Reference, "Remake management" on page L-1426
⇨ Tutorial, "Remake management" on page L-1327

(A+W Production Production Terminal L-1431)

### Overview: Production Terminal Manual Cutting

Production Terminal Manual Cutting shows all released batches or lots for a certain cutting table. The cutting table is usually a manual cutting table. If you do not have to create machinery code at the table, Production Terminal Manual Cutting can also be installed at another table.

The menus in Production Terminal Manual Cutting are identical with the menus in Production Terminal IG-In which is why they are not described in detail here again.
⇨ "Overview: Production Terminal IG" on page L-1414

(A+W Production Production Terminal L-1432)

#### Release

**JobTV Manual cutting > Select batch > Button [Release]**

> **Image:** Fig. L-34 Release. The 'Release' dialog shows a list of lites (Section A), a shape view (B), a shape sketch with dimensions (C), a selection counter (D), and rack information (E).

**Description of the fields in section A**
-   **Batch:** This field shows the batch number.
-   **Lot:** This field shows the lot number.
-   **Glass type:** This field shows the glass type.
-   **Barcode:** This field shows the label number.
-   **Rack:** This field shows the rack number.
-   **Slot:** This field contains the slot number.
-   **Pr.No.:** This field shows the production number.
-   **Shape:** The shape number is shown in this field.
-   **CU width:** This field shows the width of the lite.

(A+W Production Production Terminal L-1433)

-   **CU Height:** This field shows the lite height.
-   **Order:** This field shows the order number.
-   **Itm.:** The order item number is displayed in this field.

**Description of the fields in section B**
This section shows the shape.

**Description of the fields in section C**
This section shows the shape sketch.
The table next to it lists the corresponding values. Valid entries are:
-   W = width
-   H = height
-   T1, T2, ... = trim
-   <-> = reflection code
-   @ = rotation code

**Description of the fields in section D**
This section shows how many lites have been selected from the table, and the total number. Example: 1/64 means that 64 lites are listed in the table and that 1 of them has been selected.

**Description of the fields in section E**
This section contains the rack data. You can enter the rack number, or scan it. If the rack is empty, check the checkbox Start.

**Description of buttons**
-   **Production:** Press this button to book the selected lite.
-   **Print label:** Press this button to print a label for the selected lite.
-   **Breakage:** Press this button to book the selected lite 'broken'.

**Additional information**
⇨ Tutorial, "The use of Production Terminal Manual Cutting" on page L-1332
⇨ Tutorial, "How to book the selected lite(s)" on page L-1341

(A+W Production Production Terminal L-1434)

#### Rejects pool

**JobTV Manual cutting > Button [Rejects pool]**

> **Image:** Fig. L-35 Rejects pool. The 'Rejects Pool' dialog, similar to the Release dialog, but for handling broken lites. It allows for quick re-cutting of broken items.

This instrument permits quick reactions when there are broken lites. If a lite is scanned as breakage somewhere on the shop floor, dialog Rejects pool opens automatically. The broken lite appears in the rejects pool and can be cut without delay (without a detour via the main cutting tables).

**Description of the fields in section A**
-   **Articles:** This field shows the article number.
-   **Name:** This field shows the glass type.
-   **Glass type:** This field shows the glass type.
-   **Thickness:** This field shows the lite thickness.
-   **Width:** This field shows the width of the lite.
-   **Height:** This field shows the lite height.

(A+W Production Production Terminal L-1435)

-   **Batch:** This field shows the batch number.
-   **Customer:** The customer name is displayed in this field.
-   **Order:** This field shows the order number.
-   **Itm:** The order item number is displayed in this field.
-   **Label:** This field shows the label number.
-   **Shape:** The shape number is shown in this field.
-   **Rack:** This field shows the rack number.
-   **Delivery date:** The delivery date is shown in this field.

**Description of buttons**
-   **Update:** Press this button to update the display.
-   **Add:** Pressing this button will open the dialog Breakage Entry.
-   **Delete:** Press this button to delete the selected lite.
-   **Print/Print2:** These buttons will be configured on site and serve to print labels or reports.
-   **Book PDC:** Press this button to book the selected lite.
-   **Cancel:** Press this button to close the dialog.

> **i Automatic update**
> The rejects pool is automatically updated every x seconds. This setting can be changed.

**Additional information**
⇨ Tutorial, "The use of Production Terminal Manual Cutting" on page L-1332
⇨ Tutorial, "How to book the selected lite(s)" on page L-1341

(A+W Production Production Terminal L-1436)

#### Breakage entry

**JobTV Manual cutting > button [Rejects pool] > button [Add]**

> **Image:** Fig. L-36 Breakage entry. The 'Entry of Rejects' dialog, used to manually add a broken item to the rejects pool. It shows customer order information and a list of parts associated with that order.

Dialog Breakage Entry allows to add breakage manually to the rejects pool.

**Description of the fields in section Customer**
-   **Order:** This field shows the order number.
-   **Item:** The order item number is displayed in this field.

**Description of the fields in section Parts**
-   **Order:** This field shows the order number.
-   **Itm:** The order item number is displayed in this field.
-   **PartNo:** This field shows the part number.
-   **Glass type:** This field shows the glass type.
-   **Width:** This field shows the width of the lite.
-   **Hght:** This field shows the lite height.

(A+W Production Production Terminal L-1437)

**Description of the fields in section Reject reason**
Select the required reason for the reject from the combo box.

**Description of the fields in section Barcodes**
-   **Label:** This field shows the label number.
-   **RP:** This field shows the registration point.
-   **Rack:** This field shows the rack number.

**Additional information**
⇨ Tutorial, "The use of Production Terminal Manual Cutting" on page L-1332
⇨ Tutorial, "How to add rejects by hand" on page L-1341

(A+W Production Production Terminal L-1438)

### Overview: Production Terminal Georgian Bars

Production Terminal Georgian Bars shows all released batches or lots for muntin construction.

The menus in Production Terminal Georgian Bars are identical with the menus in Production Terminal IG-In which is why they are not described in detail here again.
⇨ "Overview: Production Terminal IG" on page L-1414

(A+W Production Production Terminal L-1439)

#### Release

**Terminal Georgian Bars > Select batch > Button [Release]**

> **Image:** Fig. L-37 Release. The 'Release' dialog for Georgian Bars, showing a list of muntins (Section A), rack info (B), selection counter (C), a visual representation of the muntin construction (D), and action buttons (E).

This dialog shows the muntins you have previously selected in Production Terminal Georgian Bars. You can book all muntins at once, or just individual muntins. When you open the dialog, all muntins are selected by default. To book a single muntin, select it from the table.

**Description of the fields in section A**
-   **Batch:** This field shows the batch number.
-   **Label:** This field shows the label number.
-   **Description:** This field shows the muntin name.
-   **Order:** This field shows the order number.
-   **Itm:** The order item number is displayed in this field.
-   **PPos.:** This field shows the production item number.
-   **Date:** This field shows the production date.

(A+W Production Production Terminal L-1440)

-   **Shape:** The shape number is shown in this field.
-   **Width:** This field shows the width of the shape (circumscribing rectangle).
-   **Height:** This field shows the height of the shape (circumscribing rectangle).

**Description of the fields in section B**
This section contains the rack data. You can enter the rack number, or scan it. If the rack is empty, check the checkbox Start.

**Description of the fields in section C**
This section shows how many muntins have been selected from the table, and the total number. Example: 1/64 means that 64 muntins are listed in the table and that 1 of them has been selected.

**Description of the fields in section D**
This section shows the construction.

**Description of buttons**
-   **Produce:** Press this button to book the selected lite.
-   **Printing:** Press this button to print the construction.
-   **Rejects:** Press this button to book the selected muntin 'broken'.

**Additional information**
⇨ Tutorial, "Using Production Terminal Georgian Bars" on page L-1344
⇨ Tutorial, "How to book the selected muntin(s)" on page L-1349

(A+W Production Production Terminal L-1441)

### Overview: Production Terminal Order

Production Terminal Order permits to book large quantities. Processing steps linked with the registration point will be registered automatically.

The menus in Production Terminal Order are identical with the menus in Production Terminal IG which is why they are not described here again in detail.
⇨ "Overview: Production Terminal IG" on page L-1414

**Menu entry Notes**
The entry Notes is on the Extras menu. With this entry, you can enter a note for a booking. If you click the entry, a dialog opens on which you can enter the text. If in Production Terminal Order you then click [Produce], the text is written to the table awbar_historie. With such note texts, you can save special production circumstances or quality features for later evaluation. For all other bookings, a new text must or can be entered.

(A+W Production Production Terminal L-1442)

### Overview: Production Terminal Proces-sing

Production Terminal Processing is a control station used in connection with processing machinery. Production Terminal Processing provides detailed information on the processing steps to be executed including true-to-scale production drawings.

The menus in Production Terminal Processing are identical with the menus in Production Terminal IG which is why they are not described here again in detail.
⇨ "Overview: Production Terminal IG" on page L-1414

**Menu entry Notes**
The entry Notes is on the Extras menu. With this entry, you can enter a note for a booking. If you click the entry, a dialog opens on which you can enter the text. If in Production Terminal Order you then click [Produce], the text is written to the table awbar_historie. With such note texts, you can save special production circumstances or quality features for later evaluation. For all other bookings, a new text must or can be entered.

(A+W Production Production Terminal L-1443)

#### Manual entry

**Extras > Barcode**

> **Image:** Fig. L-38 Manual entry. The 'Manual Entry' dialog with a 'Barcode' input field.

This dialog can be used to load another lite. Enter the label number in field Barcode or scan the barcode. Now press [OK].
The dialog closes. You will find yourself back in the main window. The loaded lite appears at the end of the list.

**Additional information**
⇨ Tutorial, "Using Production Terminal Processing" on page L-1361
⇨ Tutorial, "How to scan a label" on page L-1366

(A+W Production Production Terminal L-1444)

### Overview: Production Terminal TG

Production Terminal TG is installed at the tempering furnaces where it supports the loading and unloading of the furnace beds.

The modules Production Terminal TG-In and Production Terminal TG-Out have the same menus as Production Terminal IG and are therefore not described again at this point.
⇨ "Overview: Production Terminal IG" on page L-1414

(A+W Production Production Terminal L-1445)

#### Manual entry

**ToolTV TG-In > Extras > Barcode**

> **Image:** Fig. L-39 Manual entry. The 'Manual Entry' dialog with a 'Barcode' input field.

This dialog can be used to load another lite. Enter the required label number in the Barcode field and press [OK]. The dialog closes, and the label number is loaded.

**Additional information**
⇨ Tutorial, "Using Production Terminal TG-In" on page L-1371
⇨ Tutorial, "How to scan a label" on page L-1375

(A+W Production Production Terminal L-1446)

#### Open processing steps

**ToolTV TG-In > Load label number**

> **Image:** Fig. L-40 Breakage Entry. The 'Open Processings' dialog shows a list of processing steps for a given label/order. It indicates whether each step is completed (green checkmark) or still open (red X).

This dialog appears automatically if there are open processing steps before the tempering process. The open processing steps are displayed and you can decide how the lite shall be treated.

**Description of fields**
-   **Label:** This field shows the label number.
-   **Order/item:** This field shows the order and item number.

**Table explanation**
-   **Completed:** This field shows the open processing steps. Valid options:
    -   Red X: The processing step is still open
    -   Green checkmark: The processing step has been executed.
-   **Date:** This field shows when the processing step was/will be executed.
-   **Processing:** This field shows the processing step.

**Description of buttons**
-   **Load anyway:** You have to use this button if the processing was executed but has not been booked. The dialog closes. You are back in the main window. The loaded lite appears on the list.

(A+W Production Production Terminal L-1447)

-   **Close:** You have to use this button if the processing step is really missing. The dialog closes, and the lite has to be processed first.

**Additional information**
⇨ Tutorial, "Using Production Terminal TG-In" on page L-1371
⇨ Tutorial, "Using Production Terminal TG-Out" on page L-1379
⇨ Tutorial, "How to treat open processing steps" on page L-1375

(A+W Production Production Terminal L-1448)

### Overview Production Terminal LG

Production Terminal LG is used at the laminating line and shows all available lots as well as information supporting production.

The modules Production Terminal LG-In and Production Terminal LG-Assembly offer the same menus as Production Terminal IG and will therefore not be described at this point.
⇨ “Overview: Production Terminal IG" on page L-1414

The software reference provides information on the following subjects:
-   **Menu File, menu entry Load order:**
    This menu item is used to load a certain order.
    ⇨ Software Reference, "Registration" on page L-1415

(A+W Production Production Terminal L-1449)

#### Load order

**Terminal LG-In > File > Load order**

> **Image:** Fig. L-41 Load Order. The 'Load Order' dialog shows a list of orders in the top pane and the parts for the selected order in the bottom pane. Radio buttons allow filtering by 'All', 'Available', 'Scheduled', and 'Possible'.

This dialog allows loading a certain order. The radio buttons can be used for restricting the view.

**Description of fields**
-   **all:** Select this radio button to view all lites at once.
-   **Available:** Selecting this radio button displays only the currently available lites.
-   **Scheduled:** Select this radio button to view all scheduled lites.
-   **Possible:** Select this radio button to display only lites that can be processed.
-   **Order:** This field shows the order number.
-   **Itm:** This field shows the item number.
-   **Part:** This field shows the part number.
-   **Name:** This field shows the part name.
-   **Batch:** This field shows the batch number.
-   **Qty.:** This field shows the quantity to be produced.

(A+W Production Production Terminal L-1450)

The table below offers detailed information on the order selected above.

**Description of buttons**
-   **Load:** Press this button or function key [F5] of adopt the selection.
-   **Cancel:** Press this button or use the function key [F6] to close the dialog.

**Additional information**
⇨ Tutorial, "Using Production Terminal LG-In" on page L-1386
⇨ Tutorial, "Using Production Terminal LG-Assembly" on page L-1392

(A+W Production Production Terminal L-1451)

#### Go to production number

**File > Go to ProdNo.** or use the function key **F11**

> **Image:** Fig. L-42 Go to production number. The 'Go to Production Number' dialog.

This dialog can be used to load another production number. The production number determines the sequence of the units to be produced. You can e.g. go directly from production number 3 to production number 15 without having to press the [Skip] button several times.

**Description of fields**
-   **Production number:** Use the cursor keys to select the production number to be produced next.

**Description of buttons**
-   **OK:** Press this button to adopt the selected production number.
-   **Cancel:** Press this button to close the dialog. The selected production number will not be adopted.

**Additional information**
⇨ Tutorial, "Loading another item number" on page L-1312

(A+W Production Production Terminal L-1452)

### Overview Production Terminal Edit

Production Terminal Edit allows correcting missing or incorrect bookings and booking large quantities at one go.

This module offers the same menus as Production Terminal IG which is why these menus are not going to be described again at this point.
⇨ "Overview: Production Terminal IG" on page L-1414

(A+W Production Production Terminal L-1453)

### Reports

Open the Lists menu

Menu Lists contains the customized reports. In our example it shows the menu item:
-   **Order list:**
    You can use this menu item to start the report for the order list.
    ⇨ Software Reference, "Parameter input for report" on page L-1455

(A+W Production Production Terminal L-1454)

#### Parameter input for report

**Lists > Order list**

> **Image:** Fig. L-43 Parameter input for report. A dialog prompts the user to 'Please Enter the Order Number'.

The top of the dialog shows the parameter input for an order list. Production Terminal offers many different lists (reports). A+W creates them for each customer, adapting them to the individual requirements.

> **Image:** Fig. L-44 Example report: Order overview. A sample 'Order Overview' report showing item details like barcode, glass type, dimensions, and booking time.

**Additional information**
⇨ Tutorial, "Creation of lists (reports)" on page L-1314
⇨ Tutorial, "How to print an order overview" on page L-1314

(A+W Production Production Terminal L-1455)

### How to Use the Help Function

Go to menu ?

Menu ? offers the following menu items:
-   **User help:**
    Use this menu item to start the short descriptions.
-   **Current log entries:**
    This menu item is used to start the log file. This file includes the log entries for the corresponding session.
    ⇨ Software Reference, "Log entries for this session" on page L-1457
-   **Change language:**
    This menu item serves to change the menu language. Dialog Change language appears.
    ⇨ Software Reference, "Language selection" on page L-1458
-   **Information:**
    This menu item provides more information on the corresponding module.
    ⇨ Software Reference, "About Production Terminal" on page L-1459

(A+W Production Production Terminal L-1456)

#### Log entries for this session

**? > Current log entries**

> **Image:** Fig. L-45 Log entries. The 'Log Entries for this Session' dialog, which displays a detailed, timestamped log of system events and debug information.

This dialog provides details on the actual session. You can export the log entries in the shape of a text file. In case of an error it can be beneficial to send this text file to A+W for analysis.

**Description of buttons**
-   **Update:** Press this button to update the display.
-   **Export:** Pressing this button will open the dialog Save as ... You can save the log entries as a text file.
-   **Close:** Press this button to close the dialog.

**Additional information**
⇨ Tutorial, "How to export log entries" on page L-1314

(A+W Production Production Terminal L-1457)

#### Language selection

**? > Change language**

> **Image:** Fig. L-46 Change language. The 'Change Language' dialog with combo boxes to select the 'Language' and 'Alternative Language'.

Use this dialog to select the language for the corresponding Production Terminal. When you leave the dialog by [OK], Production Terminal will change the language.

**Description of fields**
-   **Language:** Choose the language from the combo box and press [OK]. The language changes automatically. Rebooting is not required.
-   **Alternative language:** Select the alternative language from the combo box. The alternative language will be used if e.g. the translation of an entry is missing.

**Additional information**
⇨ Tutorial, "Select another language" on page L-1315

(A+W Production Production Terminal L-1458)

#### About Production Terminal

**? > Information**

> **Image:** Fig. L-47 About ToolTV. The 'ToolTV Version Infos' dialog showing details about the application version, file version, PPS-Webservice, and database connection.

This dialog offers further information on the individual modules, e. g. version and release.

(A+W Production Production Terminal L-1459)

## Help Cards

This section provides information on the following subjects:
⇨ Information about the help cards
⇨ Terminal IG-IN

-   **Information about the help cards** L-1463
-   **Terminal IG-IN** L-1464
    -   Procedure L-1465
    -   Produce a lite L-1466
    -   Change the machine status L-1467
    -   Book damaged lites L-1468
    -   Load production number L-1469
    -   Book damaged lites L-1470
    -   Load production number L-1471
    -   Load remakes L-1472

(A+W Production Production Terminal L-1462)

### Information about the help cards

The depictions in the Help Cards are based on the delivery version A+W Production. Individual steps in the workflows may deviate depending on the configuration.

(A+W Production Production Terminal L-1463)

### Terminal IG-IN

| Help Card | Topics |
| :--- | :--- |
| • Procedure | • Operation of Production Terminal IG-In. |
| • Change the machine status | • You change the state of the machine. |
| • Book damaged lites | • How you proceed with damaged lites. |
| • Load production number | • You change the state of the machine. |
| • Book damaged lites | • How you proceed with damaged lites. |
| • Load production number | • You load another production number. |
| • Load remakes | • You load a remake. |

(A+W Production Production Terminal L-1464)

### Terminal IG-IN: Procedure (PT 01-001)

> **Image:** A screenshot of the Production Terminal IG-In interface, showing the main screen with lite information for production.

**Goal of the action**
Operation of Production Terminal IG-In.

**Requirements**
(None listed)

**Additional info**
(None listed)

**Workflow**
1.  Log into the Terminal IG-In.
2.  Press the [Load lot] button or the function key `<F2>`.
3.  Select the lot that you would like to produce.
4.  Press the [Load] button or the function key `<F5>`.
5.  Terminal IG-In displays the exact sequence of the lites.
6.  Place the lites for the unit on the line. Heed the coating and structure.
7.  Press the foot pedal to produce or the function key `<F5>`.
8.  If the lite is not available, click Skip or `<F6>`.
9.  If the lite cannot be used, scan the barcode or click Reject/<F7>.
10. If you need to interrupt work on the machine, select Machine > Machine status from the menu and specify the corresponding reason.

(Help Cards L-1465)

### Terminal IG-IN: Produce a lite (PT 01-002)

> **Image:** A screenshot of the Production Terminal IG-In interface.

**Goal of the action**
You produce a lite.

**Requirements**
(None listed)

**Additional info**
(None listed)

**Workflow**
1.  Move the lite from the rack to the line and press the button [Produce].
2.  The lite is moved to the next station.

(Help Cards L-1466)

### Terminal IG-IN: Change the machine status (PT 01-003)

> **Image:** The 'Status' dialog for changing the machine status.

**Goal of the action**
You change the state of the machine.

**Requirements**
(None listed)

**Additional info**
-   It may be necessary to interrupt an ongoing production process. These interruptions must always be logged. Possible reasons for an interruption:
    -   Machine maintenance
    -   Machine failure
    -   Breaks
    -   Set-up times

**Workflow**
1.  Go to the Machine > Machine status menu. Or press [F3].
2.  The Status dialog appears.
3.  Select the reason from the list.
4.  Press [OK].
5.  The dialog closes and you will find yourself back in the main window. Section Status shows the selected status.

(Help Cards L-1467)

### Terminal IG-IN: Book damaged lites (PT 01-004)

> **Image:** The 'Status' dialog for booking rejects.

**Goal of the action**
How you proceed with damaged lites.

**Requirements**
-   The machine operator must know the rules for automatic remakes.

**Additional info**
-   It may happen that you cannot produce the lite suggested by the module because the lite is defective. You will have to mark the lite accordingly in this case. Causes of defects can be:
    -   Rejects, scratches
    -   Defect (quality assurance reason)
    -   Wrong size, wrong glass type
    -   Cracks

**Workflow**
1.  Select the lite in question.
2.  Press the [Rejects] button.
3.  The Status dialog opens.
4.  Choose the appropriate reason from the list.
5.  Press [OK]. You can open the report for the optimization at any time via the Attachments tab to view the result.
6.  The dialog closes and you will find yourself back in the main window.

(Help Cards L-1468)

### Terminal IG-IN: Load production number (PT 01-005)

> **Image:** The 'Status' dialog (incorrectly shown, should be 'Go to Production Number' dialog).

**Goal of the action**
You change the state of the machine.

**Requirements**
-   The machine operator must know the rules for automatic remakes.

**Additional info**
-   It may be necessary to interrupt an ongoing production process. These interruptions must always be logged. Possible reasons for an interruption:
    -   Machine maintenance
    -   Machine failure
    -   Breaks
    -   Set-up times

**Workflow**
1.  Go to the Machine > Machine status menu. Or press [F3].
2.  The Status dialog appears.
3.  Select the reason from the list.
4.  Press [OK].
5.  The dialog closes and you will find yourself back in the main window. Section Status shows the selected status.

(Help Cards L-1469)

### Terminal IG-IN: Book damaged lites (PT 01-006)

> **Image:** The 'Status' dialog for booking rejects.

**Goal of the action**
How you proceed with damaged lites.

**Requirements**
-   The machine operator must know the rules for automatic remakes.

**Additional info**
-   It may happen that you cannot produce the lite suggested by the module because the lite is defective. You will have to mark the lite accordingly in this case. Causes of defects can be:
    -   Rejects, scratches
    -   Defect (quality assurance reason)
    -   Wrong size, wrong glass type
    -   Cracks

**Workflow**
1.  Select the lite in question.
2.  Press the [Rejects] button.
3.  The Status dialog opens.
4.  Choose the appropriate reason from the list.
5.  Press [OK]. You can open the report for the optimization at any time via the Attachments tab to view the result.
6.  The dialog closes and you will find yourself back in the main window.

(Help Cards L-1470)

### Terminal IG-IN: Load production number (PT 01-007)

> **Image:** The 'Go to Production Number' dialog.

**Goal of the action**
You load another production number.

**Requirements**
(None listed)

**Additional info**
-   It may be impossible to produce the production number suggested by Terminal IG-In or you may have to produce another production number first.

**Workflow**
1.  Go to the File > Go to ProdNo menu.
2.  The Go to production number dialog opens.
3.  Go to the New production number field and use the cursor keys to select the required production number.
4.  Press [OK].
5.  The dialog closes and the selected production number is loaded. You are back in the main window.

(Help Cards L-1471)

### Terminal IG-IN: Load remakes (PT 01-008)

> **Image:** The 'Insert' dialog for loading remakes.

**Goal of the action**
You load a remake.

**Requirements**
(None listed)

**Additional info**
-   It may be impossible to produce the production number suggested by Terminal IG-In or you may have to produce another production number first.

**Workflow**
1.  Press the [Remakes] button.
2.  The Insert dialog opens.
3.  In the Barcode field, enter the label number of the IG unit by hand, or scan it.
4.  Press the [Adopt] button.
5.  The corresponding data appear in the field below.
6.  Press the [Adopt] button.
7.  The dialog closes; the remake is loaded. You are back in the main window.

(Help Cards L-1472)

## Index

### A
-   A racks
    -   Grouping and sorting: D-343
    -   Number ranges: D-344
    -   Optimization: D-344
    -   Production sequence: D-342
    -   Standard production organization: D-342
-   A racks AIR
    -   Number ranges: D-336
    -   Optimization: D-336
-   A racks dispatch
    -   Grouping and sorting: D-349
    -   Number ranges: D-350
    -   Production sequence: D-349
    -   Size categories: D-348
    -   Standard production organization: D-348
-   A+W Continuous Cutting: J-1172
    -   Overview of planned batches: J-1172
-   A+W Pattern Viewer: J-1156
-   A+W Residual Stock Manager: J-1147
-   Action for BOM configuration: E-604
-   Add box
    -   Added depth: 1-1097
    -   Added height: 1-1097
    -   Added width: 1-1097
-   Add elements (default time): E-644
-   Add order to items: C-196
-   Add rack
    -   Depth: 1-1095
    -   Height: 1-1095
    -   Width: 1-1095
-   Added depth
    -   Add box: 1-1097
-   Added height
    -   Add box: 1-1097
-   Added width
    -   Add box: I-1097
-   Additional condition: G-777
    -   Select: G-861
-   Additional sorting
    -   Additional sorting: D-392
    -   Key: D-392
    -   Tab: D-392
    -   Value: D-392
-   Addup
    -   Define quantity: F-751
-   Adjust shifts: E-594
-   AIR
    -   Input value (numeric): F-745
-   All
    -   Define conditions: F-738
    -   Define quantity: F-750
-   Allocation editor
    -   Dialog: F-760
    -   Formula: F-762
    -   Input field: F-761
    -   Property: F-761
    -   Quantity: F-762
    -   Transferred quantity: F-762
-   Alternative machines: E-450
-   And operation
    -   Formula editor: F-758
-   AND/OR relations: G-776
-   Any child
    -   Define quantity: F-750
-   Article number for missing processing
    -   Processing: D-403
-   Ascending
    -   Grouping: D-389
-   Assignment
    -   Level I: F-705
    -   Level II: F-708
-   Asynchronous processing: E-615
-   Automatic rescheduling: E-449

### B
-   Barcoding: C-215
-   Barcoding bookings
    -   Continuous booking: H-976
-   Basic idea
    -   cutting code creation: J-1108
    -   cutting optimization: J-1108
-   Batch
    -   cut: J-1137
    -   Select: J-1180
    -   select: J-1126
    -   sequence: J-1140
-   Batch creation: C-185
-   Batch number/Lot number
    -   Terminal IG: L-1307
-   Batch strategies: C-139
-   Batches: C-138, C-182
    -   Add order: C-142
    -   Batch strategies: C-139
    -   Change description: C-188
    -   Create: C-141
    -   Create special glass batch: C-187
    -   link: J-1133
    -   Manage: C-144
    -   Resolve: C-144
-   Behavior in detailed scheduling
    -   Lot type: D-401
-   BOM
    -   element chains: E-448
-   BOM configuration: E-603
-   Book whole furnace bed (Terminal TG-Out): L-1383
-   Bottleneck
    -   machine: E-462
    -   work shift: E-459
-   Bottom
    -   Define quantity: F-750
-   Boxes: H-924
-   Bucket creation: C-178
-   Buckets: C-132, C-168
    -   Add buckets: C-135
    -   Create: C-134, C-178
    -   Edit description: C-180
    -   Purchase parts: C-175
    -   Reservation orders: C-171
    -   Resolve: C-137
-   Buffer rack: D-384
    -   Rack settings: D-384
-   Buttons: A-90
    -   Close: A-92
    -   Find: A-93
    -   New: A-92
    -   OK: A-92
    -   Save: A-93
-   Buttons in MA: G-837

### C
-   Calculation sequence: E-642
    -   default time formula: E-544
-   Calendar
    -   creating non-working days: E-504
    -   deleting non-working days: E-506
    -   editing non-working days: E-505
-   Campaign
    -   creating: E-479
    -   creating individual date: E-480
    -   creating individual dates: E-480
    -   creating weekly date: E-482
    -   delete date: E-484
    -   deleting: E-485
    -   disable: E-485
    -   edit: E-484
-   Campaign days: E-621
-   Campaigns: E-620
    -   Campaign days: E-621
    -   Individual dates: E-621
    -   individual dates, weekly dates: E-477
    -   scheduling: E-479
    -   Weekly dates: E-623
-   Capacity planning: C-109
-   Change batch description: C-188
-   Change default times: C-206
-   Change language: L-1414
-   Change minimum number of A racks
    -   Dialog: D-437
-   Change procurement type: C-165
-   Change program language: L-1315
-   Change rack name
    -   PackView: 1-1094, I-1095, 1-1097
-   Changes to scheduled orders: E-616
-   Check number
    -   Harp racks: D-396
-   Check quantity
    -   Fixed rack: D-397
    -   Harp racks: D-395
-   Child
    -   Define quantity: F-750
-   Close
    -   Buttons: A-92
-   Cluster view: J-1244
-   Coated lites: G-775
-   Column definition: C-227
-   Columns
    -   Definition: C-227
-   Comparison
    -   Level I: F-701
    -   Level II: F-706
-   Condition
    -   Conditions: F-740
    -   Invert: F-742
    -   Level I: F-701
    -   Level II: F-706
    -   Lower input field: F-740
    -   Middle selection field: F-739
    -   Normal: F-740
    -   Transferred quantity: F-743
    -   Upper input field: F-739
    -   Value: F-740
-   Condition editor
    -   Graphic version: G-876
    -   Text version: G-880
-   Condition name
    -   Dialog: F-741
    -   New name: F-741
    -   Old name: F-741
-   Conditions
    -   Condition: F-740
-   Conditions and formulas: G-819, G-873
    -   in MA: G-820
    -   Processing time: G-822, G-866
-   Configure columns: C-117
-   Configure filters: C-124
-   Configure tabs: C-115
-   Configure totals row: C-119
-   Context menus: C-234
-   Continue
    -   cutting: J-1142
-   Control
    -   Table: J-1230
-   Control unit: J-1134
-   correct data: H-976
-   Cost calculation: E-675
    -   definition: E-521
-   Costs: E-675
    -   creating: E-522
    -   deleting: E-524
    -   edit: E-523
-   Create
    -   cutting code: J-1230
    -   Table optimization: J-1180
    -   table optimization: J-1127
-   Create additional sorting
    -   Dialog: D-393
    -   Do not check value: D-393
    -   Sorting: D-391
    -   Value: D-393
-   Create batches: C-141, C-185
-   Create buckets: C-134
-   Create new filter (Production monitor): E-591
-   Create special glass batch: C-187
-   Creating individual dates in campaigns: E-480
-   Creating work shifts: E-510
-   Creation
    -   Implicit processing: D-404
-   Creation of Processings: E-633
-   Creation of processings
    -   Add condition: E-636
    -   Sequence: E-634
-   Cut
    -   Job: J-1230
-   Cutting
    -   continue: J-1142
    -   interrupt: J-1142
    -   repeat: J-1137, J-1220
    -   sequence: J-1140, J-1232
    -   skip: J-1138
    -   start: J-1140, J-1230
-   Cutting code
    -   create: J-1230
    -   do not create: J-1138
-   Cutting table: J-1134

### D
-   Damaged lites: L-1311
-   Data import
    -   A+W Production: J-1113
    -   method: J-1112
    -   stand-alone system: J-1114, J-1253
-   Data input
    -   filler orders: J-1118
    -   rejects: J-1118
    -   rush order lites: J-1118
-   Data processing
    -   table optimization: J-1126
-   Data relevant to the system
    -   Barcode options: H-985
    -   Barcode types: H-986
    -   Column assignment: H-1002
    -   Columns: H-1003
    -   Registration point types: H-987
    -   Status types: H-997
-   Date optimization
    -   rules: E-447
-   Dates
    -   campaigns: E-477
    -   creating a campaign: E-480
    -   creating campaign: E-482
-   Default Time Formula: E-640
-   Default time formula: E-540, E-545
    -   Add elements: E-644
    -   Calculation sequence: E-642
    -   calculation sequence: E-544
    -   condition for arcs: E-547
    -   condition for shape: E-548
    -   condition for threshold: E-548
    -   Copy formula: E-657
    -   creating vector: E-554
    -   defining: E-551
    -   Enter time formula element: E-649
    -   example: E-546
    -   Factors: E-645
    -   factors: E-541
    -   fixed elements: E-541
    -   Formula: E-657
    -   Formula evaluation process: E-658
    -   Formula object properties: E-653, E-655
    -   Input help for vectors: E-543, E-646
    -   Limit for table: E-652
    -   Select formula: E-648
    -   Show formula: E-657
    -   table: E-542
    -   test time formula: E-556
    -   time formula object: E-549
    -   Time formula test: E-653
    -   User-defined table elements: E-651
    -   Vectors: E-645
    -   vectors: E-542
-   Default time formulas
    -   copy syntax: E-561
    -   deleting: E-555
    -   test calculation: E-557
    -   testing: E-556
    -   time surcharges: E-543
-   Default Times: E-638
-   Default times
    -   definition: E-539
-   Defect Optimizer: J-1178
-   Defective orders: E-614
-   define: G-870
-   Define column: C-121
-   Define conditions
    -   All: F-738
    -   Condition
        -   Define conditions: F-739
    -   Dialog: F-736
    -   Menu: F-737
    -   One: F-738
    -   Tool bar: F-737
    -   Zero: F-738
-   Define quantity
    -   Addup: F-751
    -   All: F-750
    -   Any child: F-750
    -   Bottom: F-750
    -   Child: F-750
    -   Dialog: F-748
    -   Master: F-750
    -   Menu: F-749
    -   Parent: F-750
    -   Self: F-750
    -   Tool bar: F-750
    -   Up: F-750
-   Define totals row: C-121
-   Delete
    -   high-priority lite: J-1120
    -   Rejects: J-1121, J-1122
    -   Select allocation: F-760
    -   Select conditions: F-735
    -   Select formulas: F-756
    -   Select quantities: F-747
-   Deleting expired reservation: E-493
-   Denso scanners: H-939
-   Depth
    -   Add rack: 1-1095
-   Descending
    -   Grouping: D-390
-   Description
    -   Formula editor: F-758
    -   Select allocation: F-760
    -   Select formulas: F-756
    -   Select quantities: F-747
-   Detailed scheduling for batch...
    -   Tab Breakage: D-422
    -   Tab Filler Orders: D-419
    -   Tab Free optimization: D-427
    -   Tab Glass thickness: D-425
    -   Tab Nesting: D-417
    -   Tab Options: D-434
    -   Tab Organization: D-430
    -   Tab Organization options: D-432
    -   Tab Partial quantities: D-428
    -   Tab Rack load: D-410
    -   Tab Residue plates: D-421
    -   Tab Results: D-415
    -   Tab Rush Orders: D-424
    -   Tab Special: D-417
    -   Tab Stocksize selection: D-436
-   Detailed scheduling for batch...
    -   Dialog: D-406
    -   Tab Glass types: D-407
-   Detailed view
    -   Item no.: 1-1029
    -   Order no.: 1-1029
    -   P group: 1-1029
    -   Production line: 1-1029
    -   Quantity: 1-1029
    -   Rack ID: I-1029
    -   Rack name: 1-1028
    -   Rack#: 1-1026
    -   Row: 1-1029
    -   Side: 1-1026
    -   Size: 1-1029
    -   Stack: 1-1026
    -   Surface: 1-1029
    -   Type: 1-1029
    -   Vert. stack: 1-1029
    -   Weight: 1-1029
-   Details: C-211
-   Dialog
    -   Allocation editor: F-760
    -   Condition name: F-741
    -   Define conditions: F-736
    -   Define quantity: F-748
    -   Formula editor: F-757
    -   Info: F-742, F-754
    -   Input value (numeric): F-744
    -   Quantity name: F-752
    -   Select allocation: F-760
    -   Select condition: F-734
    -   Select formulas: F-755
    -   Select quantities: F-746
-   Digit
    -   Input value (numeric): F-745
-   Direct objects: H-912
-   Distance of axis

### E
-   Edge deletion: C-232
-   Edit
    -   Select allocation: F-760
    -   Select conditions: F-735
    -   Select formulas: F-756
    -   Select quantities: F-747
-   Edit bucket description: C-180
-   Editor-Grouping
    -   Tab: D-389
-   Editor-Sorting
    -   Tab: D-391
-   Element ID: G-777
-   Empty weight harp rack: D-397
-   End
    -   Breakage, Master organization: D-378
    -   Filler, Master organization: D-377
    -   Residue plate, Master organization: D-378
    -   Test sequence: D-373
-   Enter
    -   high-priority lite: J-1119, J-1191
    -   Rejects: J-1241
    -   rejects: J-1120
-   ERP System: A-24
-   Error
    -   scheduling: E-473
-   Error rack: H-916
-   Error report: J-1115, J-1254
-   Exercises
    -   Views: C-128
-   Existing allocation
    -   Select allocation: F-760
-   Existing conditions
    -   Select conditions: F-735
-   Existing formulas
    -   Formula editor: F-759
    -   Select formulas: F-756
-   Existing property
    -   Formula editor: F-759
-   Existing quantity
    -   Select quantities: F-747
-   Expert mode
    -   Overview: H-968
-   Expired reservations: E-624
-   Export
    -   Log entries: L-1314
    -   Work plan: E-466
-   Export log entries: L-1414
-   Export/Import item view: C-201

### F
-   Factors: E-645
-   Factors (default time formula): E-541
-   Features: J-1109
-   Field definition: C-199
-   Filled harp racks
    -   Grouping and sorting: D-358
    -   Number ranges: D-359
    -   Optimization: D-359
    -   Production sequence: D-358
    -   Standard production organization: D-358
-   Filler condition
    -   Master organization: D-377
-   Filler order
    -   use: J-1128
-   Filler orders: C-160
-   Filter
    -   Define: C-229
    -   Edit: C-228
-   Filter definition: C-229
-   Filter function
    -   Pool view: 1-1080
-   Find
    -   Buttons: A-93
    -   Online help: A-99
-   Fixed elements (default time formula): E-541
-   Flag test
    -   Test flag: D-256
-   Flags: D-256
-   Formula
    -   Allocation editor: F-762
    -   Formula editor
        -   Grouping: D-390
        -   Level I: F-700
        -   Level II: F-705
-   Formula editor
    -   And operation: F-758
    -   Description: F-758
    -   Dialog: F-757
    -   Existing formulas: F-759
    -   Existing property: F-759
    -   Formula: F-758
    -   Graphic version: G-876
    -   Input field: F-758
    -   Maximum: F-758
    -   Middle value: F-758
    -   Minimum: F-758
    -   Number of results: F-758
    -   Or operation: F-758
    -   Quantity: F-758
    -   Text version: G-880
    -   Total: F-758
    -   Transferred quantity: F-758
-   formula editor: E-545
-   Formula evaluation: E-658
-   Formula evaluation process: E-658
-   Formula object properties: E-655
-   formula structure: E-540
-   Formulas and conditions: G-819, G-873
    -   in MA: G-820
    -   Processing time: G-822, G-866
-   Free edit mode: 1-1037
-   From/to
    -   Tab Application, dialog Rack Settings: D-384

### G
-   General buttons
    -   Produce: L-1306
    -   Rejects: L-1307
-   Glass type
    -   select: J-1202
-   Glass types: C-208
-   Global settings
    -   Functional principle: D-327
-   Group formation
    -   Organization groups: D-381
    -   Presettings: D-387
    -   Rack settings: D-383
-   Grouping
    -   Ascending: D-389
    -   Descending: D-390
    -   Formula: D-390
    -   Lot type: D-400
    -   Property: D-390
-   Grouping and sorting
    -   A racks: D-343
    -   A racks dispatch: D-349
    -   Filled harp racks: D-358
    -   Harp racks, no filling up: D-354
    -   Grouping and sorting: D-354
    -   Number ranges: D-354
    -   Optimization: D-354
    -   Production sequence: D-353
    -   Standard production organization: D-353

### H
-   Height
    -   Add rack: 1-1095
-   Help topics
    -   Online help: A-96
-   High-priority lite
    -   delete: J-1120
    -   enter: J-1119, J-1191
    -   show: J-1189
-   High-priority order: E-607
-   Handling of
    -   damaged lites: L-1311
    -   Machine statuses: L-1310
-   Harp racks, no filling up

### I
-   Icon
    -   Pool view: 1-1019
-   Icons
    -   overview: J-1187
    -   PackView: 1-1090
-   ID for Stack Opti
    -   Harp rack: D-396
-   Image of the unit in color: L-1318
-   Implicit processing
    -   Creation: D-404
    -   Lot type: D-404
    -   Name: D-404
    -   Tab: D-404
    -   Type: D-404
-   Import
    -   batch: J-1114
    -   Data: J-1253
    -   switch off: J-1115
    -   switch on: J-1114
-   Index
    -   Online help: A-98
-   Indirect objects: H-912
-   Individual dates (campaign): E-621
-   Individual filters (Production monitor): E-590
-   Info
    -   Dialog: F-742, F-754
    -   Info fields: L-1306
-   Input field
    -   Allocation editor: F-761
    -   Formula editor: F-758
-   Input help for vectors: E-646
-   Input value (numeric)
    -   AIR: F-745
    -   Dialog: F-744
    -   Digit: F-745
    -   Length: F-745
    -   New value: F-744
    -   Old value: F-744, F-745
    -   Text: F-745
-   Interrupt
    -   cutting: J-1142
-   Invert
    -   Condition: F-742
-   Item no.
    -   Detailed view: 1-1029
-   Items: C-145, C-193
    -   Add order: C-196
    -   Field definition: C-199
    -   Import/export view: C-201
    -   Split: C-146, C-197

### J
-   Job
    -   cut: J-1230
    -   reset: J-1220
    -   select: J-1226

### K
-   Key
    -   Additional sorting: D-392

### L
-   L rack
    -   Dialog Rack: D-395
-   Lager: J-1269, L-1461
-   Length
    -   Input value (numeric): F-745
-   Link: J-1133
    -   table optimization: J-1131
-   Linked documents: L-1307
-   Links to documents: C-231
-   List: C-119
-   List current unit
    -   Terminal IG-In: L-1305
-   Lite
    -   enter: J-1119
-   Lite format: G-776
-   Load another production number: L-1312
-   Load Distribution: E-679
-   Load distribution
    -   definition: E-570
    -   deleting: E-574
    -   editing: E-573
    -   set-up: E-571
-   Load lot
    -   Terminal IG-In: L-1309
-   Load remakes
    -   Terminal IG-In: L-1313
-   Local optimization
    -   Number of stockplates: J-1219
    -   overview: J-1207
    -   Parameters: J-1210, J-1216
    -   Stockplate: J-1212
-   Logical machine: G-789, G-790, G-845
    -   create costs: E-522
    -   default time: E-539
    -   Define: G-792, G-863
    -   Delete: G-795
    -   Edit: G-794, G-864
    -   Enter: G-792, G-863
    -   Formula selection: G-866, G-882
    -   Manage: G-792
    -   Processing time: G-866, G-882
    -   Shift group: E-672
-   Logical machine see also machine
-   Lot type
    -   Behavior in detailed scheduling: D-401
    -   Grouping: D-400
    -   Implicit processing: D-404
    -   Machine type: D-400
    -   Name: D-400
    -   Name/Type/Procurement type: D-400
    -   Number: D-400
    -   Processing: D-403
    -   Production sequence: D-400
    -   Reverse sorting: D-400
-   Lot types
    -   Tab: D-399
-   Lots: C-219
-   Lower input field
    -   Condition: F-740

### M
-   MA: G-770
    -   Elements: G-768
-   MA editor
    -   Logical machines: G-845
    -   Machine types: G-851
    -   Machines: G-843
    -   Work process allocation: G-849
    -   Work processes: G-847
-   Machine: A-52, G-771, G-772, G-843
    -   Additional condition: G-777
    -   AND/OR relations: G-776
    -   bottleneck: E-462
    -   Coated glass: G-784
    -   Coated lites: G-775
    -   creating costs: E-522
    -   Define: G-778, G-853
    -   Delete: G-781
    -   deleting costs: E-524
    -   Edit: G-779, G-782, G-854
    -   Edit properties: G-779
    -   Element ID: G-777
    -   Enter: G-778, G-853
    -   Lite format: G-776
    -   Manage: G-778
    -   Maximum thickness: G-782
    -   maximum thickness: G-775
    -   Minimum thickness: G-782
    -   minimum thickness: G-775
    -   Names and numbers: G-774
    -   Patterned glass: G-775, G-784
    -   rescheduling: E-469
    -   Restrictions: G-774
    -   setting display type: E-465
    -   Shapes: G-775, G-784
    -   Size restrictions: G-776, G-786, G-787, G-859
    -   Spacer restrictions: G-776, G-786, G-787, G-860
    -   Stepped IG: G-776, G-784
    -   work shift: E-461
    -   X-, Y-, Z-,W cuts: G-856
-   Machine costs
    -   edit costs: E-523
-   Machine paths
    -   alternative machines: E-450
    -   processing chains: E-449
-   Machine restrictions: G-774
    -   Edit: G-782
-   Machine see also logical machine
-   Machine shifts: E-580
-   Machine status: L-1310
-   Machine type: G-870
    -   Edit: G-871
    -   Lot type: D-400
-   Machine types: G-851
-   Machinery allocation: G-770
    -   Buttons: G-837
    -   Elements: G-768
    -   logical machine: G-789
    -   Machine: A-52, G-771, G-772
    -   Work process: G-797
    -   Work process allocation: G-808
-   Machinery group
    -   creating: E-565
    -   deleting: E-567
    -   editing: E-567
-   Machinery groups: E-677
    -   definition: E-564
-   Machines
    -   Display in Production monitor: E-584
    -   display in Production Monitor: E-463
-   Machine status dialog: L-1414
-   Main packing group: 1-1076
-   Manage batches: C-144
-   Master
    -   Define quantity: F-750
-   Master data: J-1114
    -   Capacity planning: E-446
    -   Machine allocation: E-446
    -   protection, data back-up: E-500
-   Master organization
    -   Dialog: D-375
    -   End of breakage: D-378
    -   End of filler: D-377
    -   End of residue plate: D-378
    -   Filler condition: D-377
    -   Minimum quantity: D-376
    -   Name: D-375
    -   Production groups: D-376
    -   Pseudo parts: D-377
    -   Pseudo series: D-376
    -   Quick organization: D-375
    -   Script: D-377
    -   Stack XOPT together: D-375
    -   Start breakage: D-378
    -   Start filler: D-377
    -   Start residue plate: D-378
    -   Tab: D-369
    -   Use breakage: D-378
    -   Use filler: D-377
    -   Use residue plates: D-377
    -   Use rush orders: D-378
-   Matrix for transition times: E-533
-   Max
    -   Number of groups (tab Application), dialog Rack Settings: D-385
    -   Number of harp racks, dialog Rack: D-395, D-396
-   Max. number of slots/rack
    -   Racks: D-395
-   Maximum
    -   Formula editor: F-758
-   Maximum load
    -   Harp rack: D-397
-   Maximum thickness: G-775
-   Maximum weight
    -   A rack: D-395
    -   Fixed rack: D-398
-   Menu
    -   Define conditions: F-737
    -   Define quantity: F-749
    -   Software: J-1186
-   Menu bar: L-1304
-   Menu File
    -   Load order: L-1449
    -   Preview dialog: L-1414
-   Menu file
    -   Batch: L-1414
    -   Go to ProdNo.: L-1414
    -   Reregister: L-1414
-   Method
    -   data import: J-1112
    -   overview: J-1110, J-1116, J-1124, J-1135
    -   table control: J-1134
-   Middle selection field
    -   Condition: F-739
-   Middle value
    -   Formula editor: F-758
-   Minimum
    -   Formula editor: F-758
-   Minimum quantity
    -   Master organization: D-376
-   Minimum thickness: G-775
-   Module
    -   function: H-906
-   Modules
    -   connected: J-1146
    -   Defect Optimizer: J-1178
    -   PlanEditor: J-1171

### N
-   Name
    -   Implicit processing: D-404
    -   Lot type: D-400
    -   Master organization: D-375
    -   Organization groups: D-381
    -   Processing: D-402
    -   Rack settings: D-383
    -   Select conditions: F-735
-   Name of organization type
    -   Organization: D-379
-   Name/Type/Procurement type
    -   Lot type: D-400
-   New
    -   Buttons: A-92
    -   Production sequence: D-371
-   New allocation
    -   Select allocation: F-760
-   New condition
    -   Production sequence: D-371
-   New conditions
    -   Select conditions: F-735
-   New formular
    -   Select formulas: F-756
-   New logical machine: G-863
-   New machine: G-778, G-853
-   New machine type: G-870
-   New name
    -   Condition name: F-741
    -   Quantity name: F-753
-   New quantity
    -   Select quantities: F-747
-   New value
    -   Input value (numeric): F-744
-   New work process: G-867
-   No allocation
    -   Select allocation: F-760
-   No conditions
    -   Select conditions: F-735
-   No formula
    -   Select formulas: F-756
-   No quantity
    -   Select quantities: F-747
-   No splitting of..if rack load is over...percent
    -   Organization: D-379
-   Non-working days
    -   creating: E-504
    -   deleting: E-506
    -   editing: E-505
-   Normal
    -   Condition: F-740
-   Number
    -   Lot type: D-400
-   Number of results
    -   Formula editor: F-758
-   Number of slots for...
    -   Rack: D-396
-   Number ranges
    -   A racks: D-344
    -   A racks AIR: D-336
    -   A racks dispatch: D-350
    -   Filled harp racks: D-359
    -   Harp racks, no filling up: D-354

### O
-   Offline scanners: H-940
-   OK
    -   Buttons: A-92
-   Old name
    -   Condition name: F-741
    -   Quantity name: F-753
-   Old value
    -   Input value (numeric): F-744, F-745
-   One
    -   Define conditions: F-738
-   Online help
    -   Content: A-97
    -   Find: A-99
    -   Help topics: A-96
    -   Index: A-98
-   Online scanners: H-939
-   Open processing step Terminal TG-In: L-1375
-   Operating sequence
    -   Terminal Edit: L-1403
    -   Terminal IG-Assembly: L-1320
    -   Terminal IG-Out: L-1326
    -   Terminal LG-Assembly: L-1395
    -   Terminal LG-In: L-1389
    -   Terminal Manual Cutting: L-1340, L-1349
    -   Terminal Order: L-1357
    -   Terminal Processing: L-1366
    -   Terminal TG-In: L-1375
    -   Terminal TG-Out: L-1383
-   Optimization
    -   A racks: D-344
    -   A racks AIR: D-336
    -   check: J-1140
    -   Currently changed settings: J-1224
    -   cut: J-1140
    -   Filled harp racks: D-359
    -   Harp racks, no filling up: D-354
    -   import: J-1114
    -   Pausing glass types: J-1222
    -   select: J-1226
    -   select stockplate: J-1128
-   Optimization behavior
    -   Rack settings: D-384
-   Optimize
    -   rejects: J-1126
    -   residual plate: J-1154
    -   Rush order lite: J-1126
-   optimize
    -   Local optimization: J-1210
    -   Select glass type: J-1202
-   Or operation
    -   Formula editor: F-758
-   Order
    -   post-processing scheduling: E-474
    -   rescheduling: E-469
    -   reservation: E-487
    -   Schedule: E-468
    -   Select (Production monitor): E-588
-   Order no.
    -   Detailed view: 1-1029
-   Order overview: C-157
-   Orders: C-129, C-154
    -   Capacity planning: C-131
    -   Faulty information: C-131
-   Organization
    -   Dialog: D-369, D-379
    -   Functional principle: D-269
    -   Name of organization type: D-379
    -   No splitting of...if rack load is over...percent: D-379
    -   Presettings: D-387
    -   Production: D-379
    -   Stacking mode: D-379
    -   Type: D-379
-   Organization groups
    -   Dialog: D-381
    -   Group formation: D-381
    -   Name: D-381
    -   Sorting of groups: D-381
    -   Sorting within the groups: D-381
-   Overlapping dialogs: C-222
-   Overview
    -   Expert mode: H-968
    -   icons: J-1187
    -   Local optimization: J-1207
    -   method: J-1110, J-1116, J-1124, J-1135
    -   Software: J-1186
-   Overview dialogs: C-111

### P
-   P group
    -   Detailed view: 1-1029
-   Packing group: I-1077
-   Packing groups
    -   Description: 1-1077
    -   Exclude items from optimization: I-1077
    -   Main packing group: 1-1076
    -   Pack production lines together: 1-1077
    -   Packing group: 1-1077
    -   Packing rule: 1-1077
-   Packing rule: 1-1077
-   PackView
    -   Automatic backup: 1-1086
    -   Change rack name: I-1094, I-1095, I-1097
    -   Close file: 1-1086
    -   Icons: 1-1090
    -   Menu: I-1086, I-1100
    -   Open file: 1-1086
    -   Print: 1-1086
    -   Print preview: I-1086
    -   Printer setup: I-1086
    -   Terminate program: I-1087
-   Parent
    -   Define quantity: F-750
-   Patterned glass: G-775
-   Pausing glass types: J-1222
-   Personnel: H-1000
-   PlanEditor: J-1171
-   Plate
    -   cut again: J-1145
    -   do not cut: J-1138
-   Pool: C-129
-   Pool view
    -   Filter function: 1-1080
    -   Hotkey: 1-1080
    -   Total: 1-1080
-   Post-processing of scheduling: E-611
    -   Changes to scheduled orders: E-616
    -   Defective orders: E-614
-   Prerequisite knowledge: A-22, L-1297
-   Presetting
    -   Dialog: D-387
    -   Group formation: D-387
    -   Organization: D-387
    -   Processing sequence: D-387
    -   Sorting on the rack: D-387
-   Preview list: L-1306
-   Print
    -   List of orders: L-1314
-   Process
    -   Residual plate: J-1233
-   Processing
    -   adding: E-497
    -   Article number for missing processing: D-403
    -   creating: E-497
    -   Lot type: D-403
    -   Name: D-402
    -   Procurement type: D-403
    -   rescheduling: E-470
    -   resolving: E-498
    -   Tab: D-401
    -   Type: D-402
-   Processing articles: G-825
    -   Define: G-832
    -   Delete: G-835
    -   Edit: G-834
    -   Enter: G-832
    -   in MA: A-55, G-827
    -   Manage: G-832
    -   Undo allocation to processing type: G-835
-   Processing quality: C-240
-   Processing creation: E-496
-   removing processing: E-498
-   Processing sequence
    -   Presettings: D-387
-   Processing time see default times
-   Processing types: G-825, G-884, G-885
    -   Define: G-829
    -   Delete: G-831
    -   Edit: G-830
    -   Enter: G-829
    -   in MA: A-55, G-826
    -   Manage: G-829
-   Processings: C-203
    -   Change default times: C-206
    -   rescheduling: E-471
    -   Split items: E-617
-   Procurement type
    -   Change: C-165
    -   Processing: D-403
-   Produce lite
    -   Terminal IG-In: L-1309
-   Product range: A-24
-   Production
    -   Organization: D-379
-   Production dates
    -   evaluation: E-451
-   Production groups: D-376
    -   Master organization: D-376
-   Production line
    -   Detailed view: 1-1029
-   Production Monitor
    -   adjustments: E-456
    -   detailed view: E-456
    -   display machines: E-463
    -   set display: E-464
-   Production monitor: E-454, E-580
    -   Adjust shifts: E-594
    -   Create new filter: E-591
    -   creating work shifts: E-510
    -   Displayed machines: E-584
    -   Filter by batch: E-589
    -   Filter by order: E-588
    -   Individual filters: E-590
    -   Machine: E-592
    -   Presentation of shifts: E-585
    -   Select batch: E-588
    -   Select order (Production monitor): E-588
    -   Settings: E-585
    -   Shift properties: E-595
-   Production scheduling: C-108
-   Production sequence
    -   A racks: D-342
    -   A racks dispatch: D-349
    -   Filled harp racks: D-358
    -   Harp racks, no filling up: D-353
    -   Lot type: D-400
    -   New: D-371
    -   New condition: D-371
    -   Settings: D-372
    -   Tab: D-371
-   Production status
    -   reset: J-1145
-   Properties of tabs: C-226
-   Property

### Q
-   Quantity: D-395
    -   Allocation editor: F-762
    -   Detailed view: 1-1029
    -   Formula editor: F-758
    -   Level I: F-704
    -   Level II: F-708
    -   Level III: F-709
    -   Slot number, dialog Rack: D-396
-   Quantity name
    -   Dialog: F-752
    -   New name: F-753
    -   Old name: F-753
-   Quick organization
    -   Master organization: D-375

### R
-   Rack: D-395
    -   Center of gravity from middle: D-397
    -   Check number (of harp racks): D-395, D-396
    -   Check quantity (fixed rack): D-397
    -   Dialog: D-394
    -   Distance of axis: D-397
    -   Empty weight (harp rack): D-397
    -   ID for Stack Opti: D-396
    -   L rack: D-395
    -   Max. number of harp racks: D-395, D-396
    -   Max. number of slots/rack: D-395
    -   Maximum load (harp rack): D-397
    -   Maximum weight (A rack): D-395
    -   Maximum weight (fixed rack): D-398
    -   Number of slots: D-396
    -   Number of slots for...: D-396
    -   Quantity: D-395
    -   Robot: D-395
    -   Sortjet: D-395, D-397
    -   Stacking depth (A rack): D-395
    -   Stacking depth (fixed rack): D-397
    -   Stacking width (A rack): D-395
    -   Stacking width (fixed rack): D-396, D-397
    -   Start=0: D-396
    -   Two slots/number: D-396
-   Rack filter
    -   Company-owned racks: H-996
    -   Rack base type: H-996
    -   Rack name from ... to: H-996
    -   Rack type: H-996
    -   Reg. point type: H-996
    -   Registration point: H-996
-   Rack ID
    -   Detailed view: 1-1029
-   Rack mode: D-385
-   Rack name
    -   Detailed view: 1-1028
-   Rack settings
    -   Buffer rack: D-384
    -   Dialog: D-383
    -   Group formation: D-383
    -   Max. number of groups (tab Application): D-385
    -   Name: D-383
    -   Optimization behavior: D-384
    -   Rack type (tab Application): D-385
    -   Sorting within the groups: D-383
    -   Stacking mode: D-385
    -   Stacking mode for groups: D-384
    -   Tab Application, from/to: D-384
-   Rack type
    -   Rack settings (tab Application): D-385
-   Rack#
    -   Detailed view: 1-1026
-   Racks: H-923
    -   Base reg. point: H-994
    -   BC start value: H-993
    -   Create multiple racks: H-992
    -   Current reg. point: H-994
    -   Current status: H-994
    -   Customer name: H-994
    -   Customer number: H-994
    -   Delivery location: H-995
    -   End value: H-993
    -   Filter: H-923
    -   Last reg. point: H-994
    -   Last status: H-994
    -   Prefix: H-993
    -   Rack base type: H-993
    -   Rack type: H-993
    -   Route number: H-995
    -   Slot number from ... to: H-993
    -   Start value: H-993
-   Temporary rack: H-994
-   Register
    -   Terminal IG-In: L-1308
-   Registration Point
    -   Grouping: H-989
    -   Grouping for shifts: H-989
    -   Restrictions: H-989
    -   Unit feedback: H-991
-   Registration point
    -   Barcode: H-988
    -   Current status: H-989
    -   Description: H-989
    -   Machine for order entry: H-991
    -   Name: H-989
    -   Number: H-988
    -   Over quantities: H-990
    -   Processing feedback: H-991
    -   Produced parts: H-990
    -   Production feedback: H-991
    -   Rack feedback: H-991
    -   Registration point type: H-989
    -   Report rack load: H-991
    -   Subrow for labels: H-989
    -   Text for customer lists: H-989
    -   Text for production lists: H-989
-   Truck: H-921
-   Registration points
    -   Manage: H-919
-   Reject
    -   enter: J-1241
-   Rejects
    -   delete: J-1121, J-1122
    -   enter: J-1120
    -   optimize: J-1126
    -   Pool: J-1239
    -   select: J-1126
-   Repeat
    -   Batch: J-1137
    -   cutting: J-1145, J-1220
-   Required knowledge: H-906
-   Rescheduling: E-605, E-610
    -   high-priority order: E-605
    -   lock date: E-605
    -   machine: E-469
    -   order: E-469
    -   Post-processing of scheduling: E-611
    -   processing: E-470
    -   Receipt of goods: E-607
    -   Rescheduling: E-610
-   Reservation
    -   capacities: E-487
    -   configuration: E-486
    -   creating: E-489
    -   deleting: E-492
    -   deleting expired reservation: E-493
    -   editing: E-491
    -   expired: E-488
    -   order: E-487
    -   Per shift: E-627
    -   Select project: E-631
-   Reservation for Machine: E-629
-   Reservation orders bucket: C-171
-   Reservations: E-626
    -   by day, by week: E-627
    -   Expired reservations: E-624
    -   Per customer: E-627
    -   Per machine: E-627
-   Reserve capacity: E-487
-   Reserve sorting
    -   Lot type: D-400
-   Reset
    -   status: J-1145, J-1220
-   Residual plate
    -   optimize: J-1154
    -   process: J-1233
    -   show: J-1140
    -   use: J-1128
-   Residue plate slot: J-1213
-   Resolve
    -   table optimization: J-1129
-   Resolve batches: C-144
-   Resolve buckets: C-137
-   Right-click: C-234
-   Robot
    -   Functional principle: D-295
    -   Rack: D-395
-   Rough Scheduling
    -   Terms: C-109
-   Row
    -   Detailed view: 1-1029
-   Rules
    -   Load.RUL file: I-1071
    -   Name of.RUL file: I-1071
    -   RUL file: I-1071
    -   date optimization: E-447
    -   Description of the RUL file: I-1071
    -   scheduling: E-448
-   Rush order lite
    -   optimize: J-1126
    -   select: J-1126

### S
-   Save
    -   Buttons: A-93
-   Scan
    -   Units: H-945
-   Scan units: H-945
-   Scanner
    -   Configuration: H-940
-   Scheduling: E-448, E-579, E-602
    -   Asynchronous processing: E-615
    -   BOM: E-448
    -   BOM configuration: E-603
    -   campaigns: E-479
    -   Changes to scheduled orders: E-616
    -   Defective orders: E-614
    -   Error: E-611
    -   error: E-473
    -   machine paths: E-449
    -   post-processing: E-474
    -   Processing creation: E-496
    -   production dates: E-451
    -   Schedule orders: E-468
    -   Split items: E-617
    -   transition times: E-527
-   Scheduling rules: E-446
-   Script
    -   Master organization: D-377
-   Search for document: C-148
-   Select
    -   Batch: J-1126, J-1137, J-1180
    -   Glass type: J-1202
    -   job: J-1226
    -   Optimization: J-1202, J-1226
    -   rejects: J-1126
    -   Rush order lite: J-1126
    -   stockplate: J-1212
-   Select allocation
    -   Delete: F-760
    -   Description: F-760
    -   Dialog: F-760
    -   Edit: F-760
    -   Existing allocation: F-760
    -   New allocation: F-760
    -   No allocation: F-760
-   Select batch (Production monitor): E-588
-   Select condition: G-821, G-861
    -   Dialog: F-734
-   Select conditions
    -   Delete: F-735
    -   Edit: F-735
    -   Existing conditions: F-735
    -   Name: F-735
    -   New condition: F-735
    -   No condition: F-735
-   Select customer for reservation Reservation
    -   Select customer: E-630
-   Select formula: E-648, G-821, G-861
-   Select formulas
    -   Delete: F-756
    -   Description: F-756
    -   Dialog: F-755
    -   Edit: F-756
    -   Existing formulas: F-756
    -   New formula: F-756
    -   No formula: F-756
-   Select project (reservation): E-631
-   Select quantities
    -   Delete: F-747
    -   Description: F-747
    -   Dialog: F-746
    -   Edit: F-747
    -   Existing quantity: F-747
    -   New quantity: F-747
    -   No quantity: F-747
-   Self
    -   Define quantity: F-750
-   Sequence
    -   batch: J-1140
    -   cutting: J-1140, J-1232
-   Sequence (creation of processings): E-634
-   Sequence of checks
    -   Functional principle: D-324
-   Sequence of machines
    -   Dialog: D-438
    -   Down: D-438
    -   Up: D-438
-   Serial scanners: H-940
-   Set status: C-109
-   Settings
    -   Production sequence: D-372
    -   Table optimization: J-1251
    -   Tables: J-1249
-   Shape: J-1243
-   Shape input: J-1193
-   Shape view: L-1304
-   Shapes: G-775
-   Shift
    -   special case for change: E-530
-   Shift calendar: E-665
-   Shift change special case: E-530
-   Shift group: E-670
    -   creating: E-515
    -   deleting: E-519
    -   editing: E-518
-   Shift plan: E-666
    -   creating: E-508
    -   deleting: E-510
    -   editing: E-509
-   Shift plans: E-502
-   Shift properties: E-595
-   Shift reservations: E-627
-   Shift rule: E-668
    -   creating: E-511
    -   deleting: E-514
    -   editing: E-513
-   Shifts: E-663
    -   Logical machine: E-672
    -   Shift calendar: E-665
    -   Shift group: E-670
    -   shift group: E-515
    -   Shift plan: E-666
    -   shift plan: E-509
    -   Shift rule: E-668
    -   shift rule: E-513
    -   Transition time: E-660
-   Shipping: H-947
-   Shop floor data collection: C-215
-   Short description of the standard production organization: D-334
-   Show
    -   high-priority lite: J-1189
-   Side
    -   Detailed view: 1-1026
-   Size
    -   Detailed view: 1-1029
-   Size categories A racks dispatch: D-348
-   Size restrictions: G-776, G-859
-   Skip
    -   cutting: J-1138
-   Software
    -   Menu: J-1186
    -   Overview: J-1186
-   Software terms: A-89
-   Sorting
    -   Create additional sorting: D-391
-   Sorting of groups
    -   Organization groups: D-381
-   Sorting on the rack
    -   Presettings: D-387
-   Sorting within the groups
    -   Organization groups: D-381
    -   Rack settings: D-383
-   Sortjet
    -   Harp rack: D-395, D-397
-   Spacer restrictions: G-776, G-860
-   Split items: C-197, E-617
-   Stack
    -   Detailed view: 1-1026
-   Stack XOPT together
    -   Master organization: D-375
-   Stacking depth
    -   A rack: D-395
    -   Rack (fixed rack): D-397
-   Stacking mode
    -   Organization: D-379
    -   Rack settings: D-385
-   Stacking mode for groups
    -   Rack settings: D-384
-   Stacking width
    -   A rack: D-395
    -   Fixed rack: D-396, D-397
-   Stand alone system
    -   Data import: J-1253
-   Standard production organization
    -   A racks: D-342
    -   A racks dispatch: D-348
    -   Harp racks, no filling up: D-353
    -   Short description: D-334
-   Standard production organizations
    -   Filled harp racks: D-358
-   Standard report
    -   Booking history: H-973
    -   Loading list: H-971
    -   Order overview: H-970
    -   Order status: H-971
    -   Rack load per item: H-973
    -   Rack load per lite: H-972
    -   Unit list: H-970
-   Start
    -   =0, rack: D-396
    -   Breakage, Master organization: D-378
    -   cutting: J-1230
    -   Filler, Master organization: D-377
    -   Residue plate, Master organization: D-378
    -   Test sequence: D-373
-   Start help function: L-1414
-   Status
    -   Action barcode: H-934
    -   Rack: H-933
    -   Registration point: H-933
    -   Unit/group: H-933
-   Status barcode
    -   Scan: H-957
-   Status values
    -   AWRack info: H-999
    -   AWRack status: H-999
    -   Barcode: H-999
    -   Description: H-999
    -   Status name: H-998
    -   Status number: H-998
    -   Text for lists: H-999
-   Stepped IG: G-776
-   Stock: C-239, E-681, G-893
-   Stockplate
    -   select: J-1128, J-1212
-   Surcharges on default time: E-543
-   Surface: L-1303
    -   Detailed view: 1-1029
-   Surplus Editor: C-163
-   Switch off
    -   import: J-1115
-   Switch on
    -   import: J-1114

### T
-   Table
    -   control: J-1230
    -   table (default time formula): E-542
-   Table optimization: J-1126
    -   check result: J-1128
    -   Create: J-1180
    -   create: J-1127
    -   link: J-1131
    -   Resolve: J-1129
    -   Settings: J-1251
-   Tables
    -   Settings: J-1249
-   Tabs
    -   Properties: C-226
-   Terminal Edit
    -   Work steps: L-1403
-   Terminal IG
    -   Batch number/Lot number: L-1307
    -   Georgian bar view: L-1307
    -   Production instructions: L-1307
    -   Production number/Name: L-1304
-   Terminal IG buttons
    -   Skip: L-1307
-   Terminal IG Georgian bar view: L-1307
-   Terminal IG production instructions: L-1307
-   Terminal IG-In: L-1303
    -   List of current unit: L-1305
    -   Load another production number: L-1312
    -   Load lot: L-1309
    -   Load remakes: L-1313
    -   Preview list: L-1306
    -   Produce lite: L-1309
    -   Register: L-1308
    -   Surface: L-1303
    -   Work steps: L-1307
-   Terminal IG-In buttons
    -   Load lot: L-1306
-   Terminal IG-Out
    -   Work steps: L-1326
-   Terminal LG-Assembly
    -   Work steps: L-1395
-   Terminal LG-In
    -   Work steps: L-1389
-   Terminal Order
    -   Work steps: L-1357
-   Terminal Processing
    -   Work steps: L-1366
-   Terminal TG-In
    -   List unloading sequence: L-1381
    -   Open processing step: L-1375
    -   Work steps: L-1375
-   Terminal TG-Out
    -   Book whole furnace bed: L-1383
    -   Work steps: L-1383
-   Terminal TG-Out buttons: L-1381
-   Terms in Rough Scheduling: C-109
-   Test sequence
    -   Down: D-373
    -   End: D-373
    -   Start: D-373
    -   Tab: D-372
    -   Up: D-373
-   Test time formula: E-556
-   Text
    -   Input value (numeric): F-745
    -   Threshold value (default time formula): E-548
-   Time formula element: E-649
-   Time formula object: E-549
-   Time formula test: E-556, E-653
    -   Formula object properties: E-653, E-655
-   Tool bar
    -   Define conditions: F-737
    -   Define quantity: F-750
-   ToolTV IG-In buttons
    -   Remakes: L-1307
-   Topic: A-96
-   Total
    -   Formula editor: F-758
    -   Pool view: 1-1080
-   Transferred quantity
    -   Allocation editor: F-762
    -   Condition: F-743
    -   Formula editor: F-758
-   Transition
    -   hours: E-529
    -   in hours or shift: E-527
    -   shifts: E-528
-   Transition time
    -   creating: E-534
    -   deleting: E-536
    -   editing: E-536
    -   hours: E-529
    -   shifts: E-528
    -   special case: E-530
    -   type: E-532
-   Transition Times: E-525
-   Transition times: E-659
    -   definition: E-531
    -   matrix: E-533
    -   scheduling: E-527
    -   Shifts: E-660
-   Two slots/number
    -   Rack: D-396

### U
-   Type
    -   Detailed view: 1-1029
    -   Implicit processing: D-404
    -   Organization: D-379
    -   Processing: D-402
-   Unloading sequence (Terminal TG-In): L-1381
-   Up
    -   Define quantity: F-750
    -   Sequence of machines: D-438
    -   Test sequence: D-373
-   Upper input field
    -   Condition: F-739
-   Use
    -   Breakage, dialog Master Organization: D-378
    -   filler order: J-1128
    -   Filler, Master organization: D-377
    -   residual plate: J-1128
    -   Residue plates, dialog Master Organization: D-377
    -   Rush orders, dialog Master Organization: D-378
-   User-defined table elements: E-651

### V
-   Value
    -   Additional sorting: D-392
    -   Condition: F-740
    -   Create additional sorting: D-393
-   Values: 1-1073
-   .VAL file: I-1074
    -   Description of the.VAL file: 1-1075
    -   Load.VAL file: 1-1073
    -   Maximum value of.VAL file: 1-1075
    -   Minimum value of.VAL file: 1-1075
    -   Name of.VAL file: I-1075
    -   Packing parameter number: 1-1074
-   Vectors: E-645
    -   input help: E-543
    -   using in default time formulas: E-554
-   Vectors (default time formula): E-542
-   Vert. stack
    -   Detailed view: 1-1029
-   View
    -   Rejects: J-1239
-   Views: C-111
    -   Configurable components: C-112
    -   Configure: C-115
    -   Configure columns: C-117
    -   Configure filters: C-124
    -   Configure tabs: C-115
    -   Configure totals row: C-119
    -   Context menu for tagged entries: 1-1082
    -   Define column: C-121
    -   Define totals row: C-121
    -   Exercises: C-128
    -   White screen: C-127
    -   Working with the list: C-119

### W
-   Weekly dates (campaign): E-623
-   Weight
    -   Detailed view: 1-1029
-   White screen: C-127
-   Width
    -   Add rack: 1-1095
-   Work
    -   continue: J-1142
    -   interrupt: J-1142
-   Work plan: C-223
    -   Export: E-466
-   Work process: A-53, G-797, G-798, G-847
    -   Additional condition: G-802
    -   Based on processing article: G-803
    -   Define: G-804, G-867
    -   Delete: G-806
    -   Edit: G-805, G-868
    -   Enter: G-804, G-867
    -   Exact definition: G-800
    -   Manage: G-804
    -   not allocated: G-801
    -   Priority: G-801
    -   Several work processes: G-801
-   Work process allocation: G-808, G-849
    -   Additional condition: G-809
    -   Allocate logical machine and work process: G-814
    -   Change priority: G-817
    -   flexibly adapted: A-54, G-809
    -   Separate logical machine and work process: G-816
-   Work shift
    -   adjustments: E-456
    -   bottleneck: E-459
    -   extending, shortening: E-459
    -   locking: E-458
    -   machine: E-461
    -   reserving: E-459
    -   setting up additional: E-457
-   Work shifts: E-454, E-580
    -   display: E-464

### X
-   XOPT-ON Plus
    -   Cluster view: J-1244
    -   general: J-1179
    -   Import: J-1179
    -   Optimization: J-1179

### Z
-   Zero
    -   Define conditions: F-738
