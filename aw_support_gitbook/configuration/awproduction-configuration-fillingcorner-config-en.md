---
description: "EN-CONFIG-AW_Production_Filling_Corner"
---


# A+W Configuration
---
## A+W Production: Filling corners and capillary tubes
-INTERNAL-

---

## 1. Contents

### Change history

| Date       | Author        | Comment                             | Version |
| :--------- | :------------ | :---------------------------------- | :------ |
| 2021-02-11 | D. Dreier     | AWP installation and configuration  | 1.0     |
| 2021-03-17 | D. Dreier     | A+W Production Terminal Setup       |         |
| 2021-03-23 | E. Tempelfeld | Document formatting, publication    | 1.1     |

### Contents

1.  **Contents**
2.  **General Information**
    *   2.1. New A+W processing types
    *   2.2. Extensions in A+W Enterprise
        *   2.2.1. Filling corner (A+W type 1661)
        *   2.2.2. Capillary tube (A+W type 1662)
3.  **Program update**
4.  **A+W Designer (Shapes)**
    *   4.1. Adjustment of the SN.INI
    *   4.2. Display of the filling corner in SN
5.  **A+W Production**
    *   5.1. Article master data
    *   5.2. Processing master data
        *   5.2.1. Creating the processing type
        *   5.2.2. Creating the processing article
        *   5.2.3. Generation of the processing 1661 – filling corner by the BOM configurator
    *   5.3. Machine assignment
        *   5.3.1. Create work process
        *   5.3.2. Assignment of a machine to the work process: set filling corner
    *   5.4. Scheduling - Orders4Production
        *   5.4.1. Activate work step
    *   5.5. Flow (results)
        *   5.5.1. Data for use for the batch formation
        *   5.5.2. Data for Production Terminal
        *   5.5.3. General data for the filling corner
        *   5.5.4. Examples
6.  **Contact Address**

---

## 2. General Information

A robot is used in operations to fill IG and LAMI glasses with gel. For this Pressure compensation (capillary tubes and filling corners) processing, the following parameters are required:
*   Corner
*   Distance to the corner
*   Edge
*   Angle of rotation

Whereby the angle of rotation is primarily required for robot control.
Basis for the development is the processing *Pressure compensation = awtyp 1660*.

### 2.1. New A+W processing types
- **1661** Filling corner
- **1662** Capillary tubes

These A+W processing types are described precisely in the normal A+W processing catalog.

### 2.2. Extensions in A+W Enterprise

#### 2.2.1. Filling corner (A+W type 1661)
To affix a filling corner, only the parameter corner is required.

#### 2.2.2. Capillary tube (A+W type 1662)
For capillary tubes, the dimensioning by corner/edge is supported. The distance to the corner has to be input. Optionally, an angle depending on an edge can be entered if the capillary tubes should have a special orientation. Furthermore, it is possible to enter a type for the capillary tube if there are several types.

**External standard interface**
The B1 records have to be scheduled as follows:

**Filling corner (1661)**

| Parameter | Meaning |
| :-------- | :------ |
| 1         | Corner  |

**Capillary tube (1662) (only AWE status as of: 25.01.21)**

| Parameter | Meaning                       |
| :-------- | :---------------------------- |
| 1         | Corner                        |
| 2         | Distance to corner            |
| 3..10     | Edge 1-8                      |
| 11        | Angle of rotation             |
| 12        | Reference edge                |
| 13        | Type no. (different articles) |

**Transfer to production and creation of sketches:**
For the transfer to production and the creation of the sketches, the appropriate modules have to be updated (see the additional chapter).

---

## 3. Program update
In order to be able to use the new A+W processing type 1661 - Filling corner to the fullest extent, the following programs have to be updated:

1.  The processing type 1661 is available starting with the OrderXML version 5.5.0006.
2.  A+W Production - Version 13. QR: 2/21
3.  A+W CAD-Designer (Shapes) – Version 13. QR: 2/21
4.  A+W Production Terminal
    > **[For installation, please consult the Automation Team in advance!]**
    > `http://tfs2012.a-w.intra:8080/tfs/glasssuite/Production/Production%20Team/versionControl?path=%24%2FProduction%2FDevMaps%2FClarity%2FCIM%2FPanorama%2FMCJobInsertTV%2FVetrotech&_a=contents`
5.  A+W Production Monitor (`\\jupiter\SW_Install\v6\Diskset\A+W Production Monitor`)

When executing from the SetupLauncher, make sure that **A+W Production** and **A+W CAD Designer (Shape)** are selected.

*(The document shows two screenshots of the 'A+W SetupLauncher' and 'Component Selection' dialogs. In the Component Selection, 'A+W Production 6...' and 'A+W CAD Designer (Shapes)' are highlighted as components to be selected for installation/update.)*

---

## 4. A+W Designer (Shapes)

### 4.1. Adjustment of the SN.INI
In the sn.ini file `((TRANS)P:\SN\SN.INI)`, the following sections have to be adjusted:

```ini
[Customer]
FileVersion=13.4.2194
```

### 4.2. Display of the filling corner in SN
The size of the corner filling in the SN sketch is determined by the settings `FillingCornerWidth` and `FillingCornerHeight`.

The standard sketch is provided with the A+W CAD Designer (Shapes) SetUp in `SNInstallationFolder\SurfaceImage`.

The title of the image file has to be `FillingCorner`. The extension can be EMF, PNG, BMP, JPG or JPEG.

In order to display the image in SN sketch, this image has to be copied to the configured motif folder, typically a subfolder of the trans/SN network folder (this can be configured in A+W Enterprise via environment variable).

Whether a corner is suitable for the automatic placement of filling corners is defined by the setting `MaximumHorizontalFillDistance`.

The SN tool for inserting a filling corner has the name `FILLCORN`. It can be added to the tools in the INCONT view (setting `INCONTadditionalTools`).

---

## 5. A+W Production
To support setting the filling corner on the fire protection glass unit, an appropriate processing article on the article type of the unit is required.
It can be provided by the ERP system or generated in the production system (BOM configurator).

### 5.1. Article master data
Fire protection glass is mapped to the article type 9 - cast resin.

*(A screenshot of the 'Artikelstammdaten' (Article master data) window is shown. The article '220005 BSG FM' is selected, and its 'Artikeltyp' (Article type) is set to '9 Gießharzeinheit' (Cast resin unit).)*

### 5.2. Processing master data
In the processing master data, the processing article is assigned a processing type. This corresponds to the A+W processing type of the filling corner.

#### 5.2.1. Creating the processing type
*(A screenshot of the 'Bearbeitungtypen' (Processing types) window is shown. A new processing type is created with the following details:)*
- **Bearbeitungstyp-Nr. (Processing type no.):** 1661
- **Bezeichnung (Description):** Füllecke setzen (Set filling corner)
- **Sequenz (Sequence):** 101

#### 5.2.2. Creating the processing article
The type 1661, created in advance, has to be selected as type. The A+W processing type cannot yet be selected here.

*(A screenshot of the 'Bearbeitungsartikel' (Processing article) window is shown. A new processing article is created with the following details:)*
- **Artikel-Nr. (Article no.):** 3991566
- **Bezeichnung (Description):** Füllecke
- **Bearbeitungstyp (Processing type):** 1661 Füllecke setzen

#### 5.2.3. Generation of the processing 1661 – filling corner by the BOM configurator
To generate the processing, go to `Master Data > Capacity Planning > Processing Generation` as follows:

*(A screenshot of the 'Bearbeitungserzeugung' (Processing Generation) window is shown. This configures the automatic creation of the 'Füllecke' processing.)*
- **Processing selected:** `3991566 Füllecke` (from processing type `1661 Füllecke setzen`)
- **Assigned to part type:** `Gießharzeinheit` (Cast resin unit)
- **Condition:** A condition is added to associate this processing with the specific fire protection glass article.
  - **Name:** `CAP_PTTYPE_PROCTYPE_ADD_3991566_TO_9_`
  - **Property:** `Parts_ARTNR`
  - **Value:** `220005`

Via an additional condition, it has to be ensured that the processing is only generated if it does not yet exist (transfer from the ERP system).

### 5.3. Machine assignment

#### 5.3.1. Create work process
The master data of the machine assignment has to be expanded to include the work process **Set filling corner**.
Navigate to `Master Data > MA Editor > Tab: work processes`.

*(A screenshot of the 'MZO-Editor' is shown. A new work process is created with the following details:)*
- **ID:** 16610
- **Name:** Füllecke setzen (Set filling corner)
- **A+W Types:** `1661 / Füllecke setzen` is added as a restriction.

#### 5.3.2. Assignment of a machine to the work process: set filling corner
In principle, here you can create a new machine with handling in the capacity planning. It is also sufficient if the dummy machine is used for information processings. However, this depends on the structure of the whole organization.

*(A screenshot of the 'MZO-Editor', tab 'Arbeitsgangzuordnung' (Work process assignment) is shown. The work process `16610 / Füllecke setzen` is assigned to a machine, in this case `9999 / Dummy für Informationsbearbeitungen`.)*

### 5.4. Scheduling – Orders4Production
The handling of the filling corner was implemented in a separate work step: `Proc1661RelData_23734`.

#### 5.4.1. Activate work step
Navigate to `Master Data > Configuration > Parameters > Order Import (Orders4Production) > Sequence for Order Import`:

*(A screenshot of the Parameter configuration window is shown. In the 'String Collection Editor' for the 'Reihenfolge für Auftragsimport' (Sequence for Order Import), a list of active work steps is displayed.)*

**List of the active work steps:**
The new work step must be added to the sequence.
```
Enumerate; 8
SNCreation; 8
CheckUp1; 8
BomConfigurator; 8
CheckUp2; 8
Label; 8
MachineryAllocation; 6
Capacity; 4
AlcimWorks; 6
SPCall; 8
Proc1661RelData_23734; 1
GrindArea; 8
...
```

### 5.5. Flow (results)
The work step is started after the set-up edge and the turning logic (implemented under SPCall) have been run through. As result, you get the following data:

#### 5.5.1. Data for use for the batch formation
- **POOL_BEARBEIT.MASS15:** Placement possible: 1 robot / 0 manual

#### 5.5.2. Data for Production Terminal
- **POOL_BEARBEIT.MASS12:** Parameter 1-> Offset
- **POOL_BEARBEIT.MASS13:** Parameter 2-> Height
- **POOL_BEARBEIT.MASS14:** Parameter 3-> Angle
- **POOL_BEARBEIT.MASS15:** Placement possible: 1 robot / 0 manual -> Parameter 4: Implementation after: 1 = No data present / place filling corner manually (definition according to Bystronic)

**Command Parameter 2: 1**
- **Parameter1:** Offset zum Umschreibenden Rechteck Vorderkante (0.1 mm) - *Offset to the bounding box front edge*
- **Parameter2:** Höhe für Roboter (0.1 mm) - *Height for robot*
- **Parameter3:** Winkel für Applikator (0.1° +- Im Uhrzeigersinn) - *Angle for applicator (clockwise)*
- **Parameter4:** 1 = Keine Daten vorhanden -> manuell Füllecke platzieren - *No data present -> place filling corner manually*
- **Parameter 5 to 16:** keine Funktion - *no function*

*(A diagram shows a pentagonal glass shape within its red rectangular bounding box. It illustrates the parameters:)*
- **Parameter1: Offset:** The vertical distance from the top edge of the bounding box to the corner where the filling is applied.
- **Parameter2: Höhe (Height):** A vertical dimension related to the filling corner itself.
- **Parameter3: Winkel (Angle):** The angle of the filling component.

- **POOL_TEILE.AUSGANGSNR:** The unit is produced turned
- **MZO_EINSTELLEN.WENDEN_IN:** The unit is produced turned on this machine
- **MZO_EINSTELLEN.KANTE_IN:** The set-up edge on this machine

#### 5.5.3. General data for the filling corner
- **POOL_BEARBEIT.MASS1:** Corner
- **POOL_BEARBEIT.MASS2:** Edge
- **POOL_BEARBEIT.MASS3:** Angle
- **POOL_BEARBEIT.MASS4:** Edge
- **POOL_BEARBEIT.MASS5:** Angle
- **POOL_BEARBEIT.MASS6:** useAsSpecified by ERP
- **POOL_BEARBEIT.MASS7:** typeId - different articles

**Parameter Definitions:**
*   **MASS1:** `Corner` [ENUM] gibt die Ecke an, in der die Füllecke zu platzieren ist. Element: ComponentOrientation serves to help you place the component relative to an edge. This can be necessary, for example, if a robot affixes the filling corner automatically.
*   **MASS2:** `Edge`: [ENUM] specifies the edge to which the installation angle refers.
*   **MASS3:** `Angle` [double] specifies the angle counter-clockwise - with respect to ComponentOrientation.Edge Element: FillingOrientation serves to help you specify the filling angle relative to an edge.
*   **MASS4:** `Edge`: [ENUM] specifies the edge to which you refer the filling angle.
*   **MASS5:** `Angle` [double] specifies the angle counter-clockwise – with reference to FillingOrientation.Edge.
*   **MASS6:** `useAsSpecified` [boolean] serves so that the defined data and specified in the production system is taken over.
*   **MASS7:** `typeId` [int] serves so that you can map different component variants (thickness dependent).

#### 5.5.4. Examples
*(The table shows example data from the `pool_bearbeit` table for processing type 1661)*

| aw_bearbtyp | auftnr  | pos | teile_nr | bearbeit_name | mass1 | mass2 | mass3 | mass4 | mass5 | mass6 | mass7 | robotermontage | offset | höhe | winkel |
| :---------- | :------ | :-: | :------: | :------------ | :---- | :---- | :---- | :---- | :---- | :---- | :---- | :------------- | :----- | :--- | :----- |
| 1661        | 4006590 |  1  |    0     | Füllecke      |   4   |   4   |  45   |  -1   |   0   |   0   |   0   | 1              | 700    | 45   | 0      |
| 1661        | 4006590 |  2  |    0     | Füllecke      |   4   |   4   |  31   |  -1   |   0   |   1   |   0   | 1              | 1200   | 31   | 0      |
| 1661        | 4006591 |  1  |    0     | Füllecke      |   4   |   4   |   0   |  -1   |   0   |   1   |   0   | 1              | 1200   | 31   | 0      |
| 1661        | 4006591 |  2  |    0     | Füllecke      |   4   |   4   |  31   |  -1   |   0   |   1   |   0   | 1              | 1200   | 31   | 0      |
| 1661        | 4006591 |  3  |    0     | Füllecke      |   4   |   4   |  -1   |  -1   |   0   |   1   |   0   | 1              |        |      |        |
