---
description: "AUW_Configuration_Lasermarking"
---


## Configuration laser marking
### History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 2014.06 | DLA | Issue | 1.0 |
| 2016.05 | DLA | Enhancement | 1.1 |
| 2017.03 | PK | Translation of chapter 3 | 1.3 |

## Content

## What is laser marking?
During the cutting process a laser burns a logo on the sheet. The position of the logo is defined in the cutting code.
In the BOM the logo is defined in a processing of standard A+W processing type 1255. The processing has to be attached at the cutting part and contains information about position, rotation angle or logo id.
## Variant [45:24] – without SN file
You activate this variant with OPT2TXT parameter [45:24]. This only applies for rectangles and is supported by EDICUT cutting code interface. A record in the BLOCK file isn’t necessary.
A+W Realtime Optimizer is necessarily required. Before generating the cutting code the logo information will be stored in the OPT2DAT (CHRHOST filed, LABEL.SET) if they are not filled (detailed scheduling doesn’t fill the fileds).
The processing with the laser marking information has to be allocated in machinery allocation to the cutting table. If not, the XOPTON doesn’t write the information into OPT2 file.
### Configuration: XOPTON.CFG:
[Laser]
Mode=1
AdditionalTextMode=0

### Configuration: OPT2TXT:
[45:24] =	1	 for „XOPTB –e“ to generatet he info records
2	 for mirrored coordinates

### Configuration: LABEL.SET:
The following fields has to be defined in LABEL.SET for laser marking.
| **Field** | **Length** | **Description** | **Used** |
| --- | --- | --- | --- |
| CUTMIRROR | 1 | FEIN_UNIT.CUTMIRROR | Yes |
| AWTYPE_LOGO_LAYER | 1 | POOL_BEARBEIT.MASS1 | Yes |
| AWTYPE_LOGO_IDENT | 8 | POOL_BEARBEIT.MASS2 (Logo ID) | Yes |
| AWTYPE_LOGO_CORNER | 1 | POOL_BEARBEIT.MASS3 | Yes |
| AWTYPE_LOGO_XPOS | 5 | POOL_BEARBEIT.MASS4 (X - position of the mark) | Yes |
| AWTYPE_LOGO_YPOS | 5 | POOL_BEARBEIT.MASS5 (Y  - position of the mark) | Yes |
| AWTYPE_LOGO_WIDTH | 5 | POOL_BEARBEIT.MASS6 | No |
| AWTYPE_LOGO_HEIGHT | 5 | POOL_BEARBEIT.MASS7 | No |
| AWTYPE_LOGO_REFPOINT | 1 | POOL_BEARBEIT.MASS10 | No |
| AWTYPE_LOGO_REFEDGE | 2 | POOL_BEARBEIT.MASS11 | No |
| AWTYPE_LOGO_ANGLE | 3 | POOL_BEARBEIT.MASS12 (rotation angle 0-360) | Yes |
| AWTYPE_LOGO_DATA | 24 | ? | Yes |

## Variant [45:25] – with SN file
This variant is activated via the OPT2TXT switch [45:25]. It also applies to shapes and is currently supported by the EDICUT cutting code.
### Requirement
- BLOCK Entry of the sheet (thus also an SN drawing is required) which is also used during optimization.
- A + W Realtime Optimizer for cutting code output (OPT2BAR is absolutely necessary to accurately identify individual sheets).
- Release >= 5.4

### Configuration SN.INI
In the machine section ([ALCIM2000] Import in A + W Production), the switch:
**ExportSurfaceProcessing = 1** must be set to activate the LOGO export

### Configuration A+W Production [ALCIM_SHAPE / SNCUTASSTANDARDFRM]
To optimize the sheets (rectangles and standard models) with SN drawing,and use the BLOCK entry during optimization
### EDICUT: Cutting Code:
The laser marking is transferred in the info fields of the EDICUT code, i. XOPTB -E must be called and the EDICUT code must be set to read the EDICUT.TMP
- Call LaserMarkWriter.exe (currently without parameters, will be improved if the details of the machine are known). The program reads OPT2DAT and BLOCK and extracts the data from the laser marking. The program creates a file LaserMark.TXT. Previously, the old file should be deleted.
- XOPTB reads the file LaserMark.TXT (if the laser marking is activated) and fills the corresponding info data in the EDICUT.TMP.
- XCEDICUT reads the EDICUT.TMP and creates the code

### Datarecord for laser marking: The data set is accommodated in the T information of each sheet. The structure is as follows
IMarkierungNNNXXXX.XXXYYYY.YYYLLLLLLLLWWWWTTTTTTTTTTTTTTTTTTTTTTTT
Example: IMarkierung0010030.0000373.00000000001000033.1F
- Identification ("Markierung")
- 3 digits for Identification number (Datatyp: Integer)
- 8 digits for the X-Position of the marking  (e.g.: 1234.567 mm)
- 8 digits fort he Y-Position of the marking (e.g.: 1234.567 mm)
- 8 digits for the logoID (Datentyp: Integer)
- 4 digits for the angle of rotation (0-360)
- 24 digits User data (Zahlen 0…9, Buchstaben)
### Customer: Installed at SPRINZ.