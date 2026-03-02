---
description: "EN-CONFIG-AW_Continuous_Cutting"
---


# A+W Configuration: A+W Continuous Cutting

**A+W - Software for Glass**

---

---
## Change history

| Date       | Author         | Remarks | Version |
| :--------- | :------------- | :------ | :------ |
| 2021-07-12 | Anna Bremkamp  | Draft   | 1.0     |

---

## Content

1.  **General information**
2.  **A+W Realtime Optimizer configuration**
3.  **Configuration of A+W Continuous Cutting**
    3.1. Specifying standard values
    3.2. Add a filter
4.  **Use**
    4.1. Planning cutting
    4.2. Cutting

---

## 1. General information

The following documentation shows the steps for configuration of the A+W Realtime Optimizer - Continuous Cutting module.

The A+W Realtime Optimizer - Continuous Cutting module is a component of the A+W Realtime Optimizer and is currently available as a prototype.

Please make sure that you have downloaded the latest installation of the A+W Realtime Optimizer with all current hotfixes and that the database is up-to-date.

---

## 2. A+W Realtime Optimizer configuration

> **Important** - Make a backup of the current entries so they can be restored if needed - either by making a duplicate copy of the XOPTON.CFG (Example - $XOPTON.CFG) file or saving the original entry in the XOPTON.CFG.

Open the XOPTON.CFG file in the path:
`%appdata%\A+W\Techsoft\Xopton`

Find the section `[ContinuousCutting]` as shown below and make the following changes. If the section does not exist yet, insert it.

```ini
; ...... Section for Continuous Cutting ......
[ContinuousCutting]
ContinuousCuttingMode=0
ParameterStation=AUW_CONTINUOUS_CUTTING
```

*   **ContinuousCuttingMode:** `<INTEGER>` [0,1,2,3] default setting = 0
    Defines the mode for Continuous Cutting. The database table RTO_INTERFACE has to be present.
    *   **0** = Standard cutting process with batch selection dialog is used. No Continuous Cutting available.
    *   **1** = The dialog for overview of already-planned batches and the dialog for preparation of batches for Continuous Cutting is displayed (Office RTO). Continuous Cutting for production is not available.
    *   **2** = No dialog for overview and preparation of batches for Continuous Cutting is displayed (Shopfloor-RTO). Only Continuous Cutting for production is available.
    *   **3** = The dialogs for the overview and for preparation of batches for the Continuous Cutting are displayed. Continuous Cutting for production is also available.

*   **ParameterStation:** `<STRING>` default setting: AUW_CONTINUOUS_CUTTING
    Station name for loading user-specific configuration of the .NET Continuous Cutting.

---

## 3. Configuration of A+W Continuous Cutting

For the planning view, standard values can be specified in the parameter administrator and filters created. In the A+W Realtime Optimizer, open the "Continuous Cutting" menu element from the `Zuschnitt` (Cutting) menu.

After the new dialog has loaded successfully, press `CTRL+F9`. After entry of the password, the parameter administrator opens.

### 3.1. Specifying standard values

In the Parameter-Administrator, navigate to `ContinuousCutting > AUW_CONTINUOUS_CUTTING`. Enter the desired standard values in the `Standardwerte` section.

*   **Default Modus Postoptimierung:** 0
*   **Default mindestmenge Bruch für Postc:** 0
*   **Default Modus Verlinken:** 0
*   **Default Modus Reoptimierung:** 0
*   **Default mindestmenge Bruch für Reop:** 0
*   **Default Restblatt bearbeiten:** 0
*   **Default Mindestlänge des Restblattes:** 0

### 3.2. Add a filter

To add a new filter, click the button in the `Parametrisierbare SQL Filter` field.

An overview of all existing filters opens. Now you can insert a new filter or edit an existing filter.

**Example of Existing Filters:**

| Name                     | Filter                                                                  |
| :----------------------- | :---------------------------------------------------------------------- |
| AUW_FIL_BATCH            | `fein_los.job = [TTV1NUM]`                                              |
| AUW_FIL_BATCH_FROM_TO    | `fein_los.job >= [TTV1NUM] and fein_los.job <= [TTV2NUM]`                 |
| AUW_FIL_GLASTYPE         | `pool_teile.glasart = [TTV1NUM]`                                        |
| AUW_FIL_GLASTYPE_FROM_...| `pool_teile.glasart >= [TTV1NUM] and pool_teile.glasart <= [TTV2NUM]`     |
| AUW_FIL_GLASTYPE_THICK...| `pool_teile.glasart = [TTV1NUM] and pool_teile.dicke/1000 = [TTV2NUM]`    |

Click `Neu` (New) to create a new filter. Give the filter a meaningful name and make sure the syntax of the filter is correct. You can define a permanent filter or a filter with placeholders. For filters with placeholders, the user enters the desired value himself later on.

**Placeholders:**
*   `[TTV(1|2)NUM]`
*   `[TTV(1|2)NUMLIST]`
*   `[TTV(1|2)TEXT]`

**Filter Examples:**
*   **Permanent filter:** `pool_teile.glasart = 1004`
*   **Filter with placeholder:** `pool_teile.glasart = [TTV1NUM]`
*   **Filter with two placeholders:** `POOL_BEARBEIT.POS = [TTV1NUM] OR POOL_BEARBEIT.POS = [TTV2NUM]`

---

## 4. Use

### 4.1. Planning cutting

1.  Open the A+W Realtime Optimizer with the blue A+W Desktop shortcut.
2.  From the top menu, navigate to `Zuschnitt` (Cutting) > `Kontinuierlisches Schneiden...` (Continuous cutting...).
3.  This opens the "Freigegebene Lose" (Released Batches) overview, showing all cutting planned with A+W Continuous Cutting.
4.  Click the **"Planung" [F5]** button at the bottom right.

Now you are in the planning view where you can plan the cutting. This view shows a detailed list of batches with various parameters like due date, glass type, thickness, and quantities. You can use options at the bottom to perform actions like:
*   Nachoptimierung (Post-optimization)
*   Gruppieren (Grouping)
*   Verlinken (Linking)
*   Restplattenverwaltung (Remnant Management)
*   Click **Freigabe [F5]** (Release) to finalize the plan.

### 4.2. Cutting

1.  Open the A+W Realtime Optimizer with the blue A+W Desktop shortcut.
2.  From the top menu, navigate to `Einstellungen` (Settings) > `Zuschnitt` (Cutting).
3.  A dialog box will appear. Select **Automatisch** (Automatic) and confirm with **OK**.
4.  Now open the cutting overview by clicking the **Zuschnitt** (Cutting) button on the main menu bar.
5.  You will see an overview of the planned cutting groups, showing their status, job/lot numbers, and optimization details.
    *   If you click the **Options** button, you can reset the status of the batches if necessary.
6.  Click the **Start** button to start the cutting. The optimizations of the first group are transferred to the cutting table.
7.  The "Cutting Overview" screen will display the active cutting process, showing patterns, lites, and other details.

If the last pattern of the group has been sent to the cutting table and cut, the next group will be loaded into cutting automatically.
