---
title: "AUW_Configuration_ExtendedEdgeDeletion"
source: "AUW_Configuration_ExtendedEdgeDeletion.docx"
tags: ["AUW", "Configuration", "Extended Edge Deletion", "Data Management", "Graph Operations", "Deletion Rules", "Admin Guide", "Procedures", "Settings"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides configuration guidance for the Extended Edge Deletion feature in AUW. It is organized into the following main sections: What is Extended Edge Deletion?, Configuration A+W Production, Configuration cutting code driver, Entry A+W Production, Entry A+W Business."
long_description: "This document details how to configure and operate the Extended Edge Deletion capability within AUW. It is intended for administrators and advanced users responsible for maintaining data integrity and managing edge relationships. The content is structured into major sections, including: What is Extended Edge Deletion?; Configuration A+W Production; Configuration cutting code driver; Entry A+W Production; Entry A+W Business; Entry A+W Enterprise; Appendix 1 - Overview IG; Appendix 2 - Troubleshooting; Appendix 3 - Specials. Key sub-sections cover topics such as: How are deletion sizes entered?; How to calculate automatically deletion sizes?; Where are the deletion sizes stored?; Technical Requirements; Activate automatic calculation; Size of the grinding wheel; Edge individual cutbacks; Edge work and extended edge deletion; Enable and disable extended edge deletion; Minimum width of extended edge deletion. It outlines prerequisites and environmental requirements needed before enabling the feature. Procedural guidance explains configuration steps, parameter options, and sequencing to ensure correct behavior. Illustrative examples and use cases demonstrate expected outcomes and edge conditions. Throughout the document, each section begins with a clear header and uses bullet lists and tables where appropriate to present parameters and outcomes. Terminology and definitions are preserved from the source, and any tables are rendered using GitHub Flavored Markdown for consistency. Where the original formatting implied groupings or hierarchies, these have been normalized into consistent sections and sub-sections to improve readability in text-based interfaces."
---

History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
|  | TS-Service | Issue | 1.0 |
| 07.2012 | DLA | Dokument in AUW Standard transferiert und erweitert. | 1.1 |
| 07.2013 | DLA | Kapitel 3.6 | 1.2 |
| 09.2013 | DLA | Erweiterungen 3.6, 6 – Neu 6.1, 3.7, 3.8 | 1.3 |
| 01.2014 | DLA | Anpassungen | 1.4 |
| 05.2014 | DLA | Enter SQLServer SP for edge work | 1.5 |
| 06.2014 | DLA | Erweiterung  Troubleshooting | 1.6 |
| 01.2015 | DLA | Fehlerkorrektur [dbo].[cu_correct_area_deletion] | 1.7 |
| 02.2015 | DLA | Kleinere Erweiterungen | 1.8 |
| 04.2015 | DLA | Erweiterung BOTTERO | 1.9 |
| 08.2016 | DLA | Change name „area deletion“ to „extended edge deletion” | 2.0 |
| 06.2017 | DLA | Shapeopt is supported now | 2.1 |
| 02.2018 | DLA | Struktur angepasste | 2.2 |
|  |  |  |  |

Content

## What is Extended Edge Deletion?
We distinguish two types of deletion. Technically, the coating of a soft coated glass is removed in both. This can happen automatically when cutting or on an IG line, or manually by a worker. This is done in the IG production, so that the frame is located directly on the glass and not on the coating.
One is the normal **edge deletion**. Here the cutting code gets the information to decoat the edges of this glass type. While the cutting a grinding wheel moves over the planned cut. This wheel typically has a diameter of 20mm; it means each sheet has decoated a strip of 10 mm at the edge. This is not quite cutback (glass outer edge to inner edge of spacer), but it is in the tolerance range.
The type described in this document is the **extended edge**** deletion**. In contrast to the edge deletion, the size of the area to be decoate will be described for each edge of each sheet and the coordinates are transferred to the cutting code. This allows an exact decoating of cutback or of a step in a stepped IGU. Decoating of the normal edges with the function of extended edge deletion is rarely used, because an exact decoating slows down the cutting process considerably (the grinding wheel has to move more the once over the scheduled cut).
This both kind describe a deletion which starts at an edge of the glass. It also exist an **area deletion**, which decorates an area in the middle of the glass. This process will not be done during cutting.
The informations are provided in both cases only for soft coated glass and when the decoating option at the cutting table is configured in A+W Production.
### How are deletion sizes entered?
In A+W Production (since version 2.28) you can enter values manually at sheets that meet the technical requirements.
For IGU an **automatic calculation** of the sze is possible during import process (POOLASC interface since version 2.28 and ORDERXML interface since version 2.29).
In order entry you can add a processing of **processing type 1025** (edge deletion) to a sheet. In the processing the edge deletion size is described. This is need e.g. if you produce soft coated glass with a right decoating and deliver this to an IGU factory.
### How to calculate automatically deletion sizes?
For the cutting parts to be decoated, several values are calculated for each edge. The result is the depth of the decoated strip.
- **Edge work *****(not supported!)***
e.g. polishing; a solution can be done with a customizing function (see example in chapter 2.8)
- **Steps**
The value of a step on on the next sheet of an stepped IGU.
- **Backcut**
In A+W Production the value of backcut is stored in the shape record (table POOL_MODELL) number 1000 (BEARB_NR) of the spacer. The values for each edge are stored in the fields STUFENEINZUGx of this record.
*In older systems with A+W Business the value for **backcut** is transferred to AW Production in text record 3600.** With this no edge individual **backcuts** are possible. ALCIM uses this text record until version 2011 SP1 + Hotfix.*
If the diameter of the defined grinding wheel is smaller than the double result, then the deletion size is stored in table POOL_ENTSCHICHTUNG.
E.g. if you use a grinding wheel with 20mm diameter the deletion size is stored on a cutback of 11mm (20<2x11=True), but not stored on a cutback of 10mm (20<2x10=False).
The status of automatic calculation is stored for each line item in database field **POOL_POS.ENTSCHICHT_STATUS**:
*-1 **	**= Position has not being processed yet**
**0 **	**= Position has been processed already (no matter if the position is being de-coated or not)**
**> 0 **	**= Position caused an error during processing*
### Where are the deletion sizes stored?
In A+W Production for each sheet with extended edge deletion information you have one record in table **POOL_ENTSCHICHTUNG**. The table is linked to table POOL_TEILE across the field **ENTSCHICHT_I****D**.
During creation of optimization files (detailed scheduling or XOPTON) the deletion size is stored as additional shape record (OPT2FA) with shape number -1 behind the original shape record and the record. Because there is no shape record for rectangles (shape number 0), a original shape records with shape number 98 is generated in this case.
### Technical Requirements
Only soft coated sheets will be decoated: *POOL_TEILE.BESCHICHT_TYP in (1, 2, 10-19)*
The cutting table and our cutting code driver must support this function. Which of the driver supports it, can be found in the driver documentation. Drivers for HEGLA, LISEC and Bystronic support the function.
Free shapes (shape no. 99) or shapes with round edges are not supported. Nested FRM files aren’t supported.
Shapes nested with ShapeOpt are supported since A+W Production version 6.3.
## Configuration A+W Production
Where deletion size were recognized only to A+W Production about the editor, no further configuration is necessary. The automatic calculation function must be activated. The calculation happens during import process after machine assignment.
### Activate automatic calculation
The switch can be found in the configuration of the respective import function.
POOLASC interface: **[ALCIMPRT_SETTINGS / CALCULATE_GRINDINGAREA]**** = 1**
*(ALCIM **à** Former Data Import (ALCIMPRT) **à** ALCIMPORT Special **à** Surface deletio**n)*
OrderXML interface:* ***[ITEMS4ALCIM_SPECIAL / CALCULATE_GRINDINGAREA]**** = 1**
*(**ALCIM **à** Data Import (Items4Alcim) **à** Customer **Settings **à** Surface deletion)*
### Size of the grinding wheel
The size of the grinding wheel is defined in 1/10mm, default is 200 (20mm). This setting is global and applies to all cutting tables. It can be found in the configuration of the respective import function.
POOLASC interface*: ***[ALCIMPRT_SETTINGS / ****DIM_OF_GR****DHEAD]**** = 200****
***(**ALCIM** **à** Former Data Import (ALCIMPRT) **à** ALCIMPORT Special **à** Deletion Head**)*
OrderXML interface*: ***[****ITEMS4ALCIM_SPECIAL / DIM_OF_GR****DHEAD]**** = 200**
*(**ALCIM **à** Data Import (Items4Alcim) **à** Customer Settings **à** Deletion Head**)*
### Edge individual cutbacks
Edge individual cutbacks will be used for calculation since ALCIM 2011 SP1+Hotfix or A+W Production 5.2. With a hidden parameter the behavior can be changed. If the parameter doesn’t exist, it is active: **[****ITEMS4ALCIM_SETTINGS / CUTBACK****] = 1**
### Edge work and extended edge deletion
At coated sheets existing edge works are not included in the calculation of extended edge deletion. They can be entered manually afterwards in A+W Production, but the editor does not show the cutting dimensions.
Another option would be to add the edge work with a CU stored procedure which can be execute during import process and after reassignment.

**INFORMIX example of a SP which is in use at ****customer ISOSKLO**** (create by DLA)****:**
**BEGIN** **WORK**;
**DROP** **PROCEDURE** "alcimdb".cu_correct_ex_edge_deletion;
**CREATE** **PROCEDURE** "alcimdb".cu_correct_ex_edge_deletion (spAuftNr INTEGER, spPos INTEGER, spU_Pos INTEGER)
*-------------------------------------------------------------------------------------------------*
*--- A+W 06.2013*
*-------------------------------------------------------------------------------------------------*
*--- SP korrigiert die Werte der **erweiterten **Randentschichtung** **in Tabelle POOL_ENTSCHICHTUNG*
*--- * Auf die **Entschichtung** werden Kantenbearbeitungen addiert. **
**---   **Kantenbearbeitung muss auf dem **beschichteten** Teil selbst hängen*
*-------------------------------------------------------------------------------------------------*
  DEFINE spTeile_nr INTEGER;
  DEFINE spKantenmatrix CHAR(15);
  DEFINE spMassZuschlagFound INTEGER;
  DEFINE spMassZuschlag INTEGER;
  DEFINE spMassZuschlag_1 INTEGER;
  DEFINE spMassZuschlag_2 INTEGER;
  DEFINE spMassZuschlag_3 INTEGER;
  DEFINE spMassZuschlag_4 INTEGER;
  DEFINE spMassZuschlag_5 INTEGER;
  DEFINE spMassZuschlag_6 INTEGER;
  DEFINE spMassZuschlag_7 INTEGER;
  DEFINE spMassZuschlag_8 INTEGER;

  *--- Alle Teile mit **Entschichtungen** durchlaufen*
  FOREACH **SELECT** teile_nr **INTO** spTeile_nr **FROM** pool_entschichtung 
          **WHERE** auftnr=spAuftNr **AND** pos=spPos **AND** u_pos=spU_Pos 
          **AND** einzug_1_p1 > 0 
    LET spMassZuschlagFound = 0;
    LET spMassZuschlag = 0;
    LET spMassZuschlag_1 = 0;
    LET spMassZuschlag_2 = 0;
    LET spMassZuschlag_3 = 0;
    LET spMassZuschlag_4 = 0;
    LET spMassZuschlag_5 = 0;
    LET spMassZuschlag_6 = 0;
    LET spMassZuschlag_7 = 0;
    LET spMassZuschlag_8 = 0;
  
    *--- Alle **kantenbearbeitungen** durchlaufen*
    FOREACH **SELECT** mass_zuschlag, kantenmatrix **INTO** spMassZuschlag, spKantenmatrix 
            **FROM** pool_bearbeit 
            **WHERE** auftnr=spAuftNr **AND** pos=spPos **AND** u_pos=spU_Pos 
            **AND** teile_nr = spTeile_nr **AND** mass_zuschlag > 0
      LET spMassZuschlagFound = spMassZuschlagFound + 1;
      **IF** SUBSTRING(spKantenmatrix **FROM** 1 **FOR** 1) = 1 **THEN**
        LET spMassZuschlag_1 = spMassZuschlag_1 + spMassZuschlag;
      **END** **IF**;
      **IF** SUBSTRING(spKantenmatrix **FROM** 2 **FOR** 1) = 1 **THEN**
        LET spMassZuschlag_2 = spMassZuschlag_2 + spMassZuschlag;
      **END** **IF**;
      **IF** SUBSTRING(spKantenmatrix **FROM** 3 **FOR** 1) = 1 **THEN**
        LET spMassZuschlag_3 = spMassZuschlag_3 + spMassZuschlag;
      **END** **IF**;
      **IF** SUBSTRING(spKantenmatrix **FROM** 4 **FOR** 1) = 1 **THEN**
        LET spMassZuschlag_4 = spMassZuschlag_4 + spMassZuschlag;
      **END** **IF**;
      **IF** SUBSTRING(spKantenmatrix **FROM** 5 **FOR** 1) = 1 **THEN**
        LET spMassZuschlag_5 = spMassZuschlag_5 + spMassZuschlag;
      **END** **IF**;
      **IF** SUBSTRING(spKantenmatrix **FROM** 6 **FOR** 1) = 1 **THEN**
        LET spMassZuschlag_6 = spMassZuschlag_6 + spMassZuschlag;
      **END** **IF**;
      **IF** SUBSTRING(spKantenmatrix **FROM** 7 **FOR** 1) = 1 **THEN**
        LET spMassZuschlag_7 = spMassZuschlag_7 + spMassZuschlag;
      **END** **IF**;
      **IF** SUBSTRING(spKantenmatrix **FROM** 8 **FOR** 1) = 1 **THEN**
        LET spMassZuschlag_8 = spMassZuschlag_8 + spMassZuschlag;
      **END** **IF**;        
    **END** FOREACH;  
  
    **IF** spMassZuschlagFound > 0 **THEN**
      **UPDATE** pool_entschichtung **SET**
einzug_1_p1 = einzug_1_p1 + spMassZuschlag_1, einzug_1_p2 = einzug_1_p2 + spMassZuschlag_1, 
      einzug_2_p1 = einzug_2_p1 + spMassZuschlag_2, einzug_2_p2 = einzug_2_p2 + spMassZuschlag_2, 
      einzug_3_p1 = einzug_3_p1 + spMassZuschlag_3, einzug_3_p2 = einzug_3_p2 + spMassZuschlag_3, 
      einzug_4_p1 = einzug_4_p1 + spMassZuschlag_4, einzug_4_p2 = einzug_4_p2 + spMassZuschlag_4, 
      einzug_5_p1 = einzug_5_p1 + spMassZuschlag_5, einzug_5_p2 = einzug_5_p2 + spMassZuschlag_5, 
      einzug_6_p1 = einzug_6_p1 + spMassZuschlag_6, einzug_6_p2 = einzug_6_p2 + spMassZuschlag_6, 
      einzug_7_p1 = einzug_7_p1 + spMassZuschlag_7, einzug_7_p2 = einzug_7_p2 + spMassZuschlag_7, 
      einzug_8_p1 = einzug_8_p1 + spMassZuschlag_8, einzug_8_p2 = einzug_8_p2 + spMassZuschlag_8, 
      lastmodzeit = **CURRENT**, lastmodstation = "AUW_SP" 
      **WHERE** auftnr=spAuftNr **AND** pos=spPos **AND** u_pos=spU_Pos **AND** teile_nr = spTeile_nr 
      **AND** lastmodstation <> "AUW_SP"; 
    **END** **IF**;
  **END** FOREACH;

**END** **PROCEDURE**;
**COMMIT** **WORK**;

**SQLServer**** ****example****:**
CREATE PROCEDURE [dbo].[cu_correct_ex_edge_deletion]
@spAuftNr INTEGER,
@spPos INTEGER,
@spU_Pos INTEGER
AS
--------------------------------------------------------------------------------------------- A+W 05.2014
------------------------------------------------------------------------------------------
--- SP korrigiert die Werte der erweiterten Randentschichtung in Tabelle POOL_ENTSCHICHTUNG
--- * Auf die Entschichtung werden Kantenbearbeitungen addiert.
--- Kantenbearbeitung muss auf dem beschichteten Teil selbst hängen
------------------------------------------------------------------------------------------
BEGIN
DECLARE @spTeile_nr INTEGER;
DECLARE @spKantenmatrix CHAR(15);
DECLARE @spMassZuschlagFound INTEGER;
DECLARE @spMassZuschlag INTEGER;
DECLARE @spMassZuschlag_1 INTEGER;
DECLARE @spMassZuschlag_2 INTEGER;
DECLARE @spMassZuschlag_3 INTEGER;
DECLARE @spMassZuschlag_4 INTEGER;
DECLARE @spMassZuschlag_5 INTEGER;
DECLARE @spMassZuschlag_6 INTEGER;
DECLARE @spMassZuschlag_7 INTEGER;
DECLARE @spMassZuschlag_8 INTEGER;

--- Alle Teile mit Entschichtungen durchlaufen
DECLARE select_cursor1 CURSOR FOR
SELECT teile_nr FROM pool_entschichtung
WHERE auftnr=@spAuftNr AND pos=@spPos AND u_pos=@spU_Pos AND einzug_1_p1 > 0;
OPEN select_cursor1;
FETCH NEXT FROM select_cursor1 INTO @spTeile_nr;
WHILE @@FETCH_STATUS = 0
BEGIN
SELECT @spMassZuschlagFound = 0;
SELECT @spMassZuschlag = 0;
SELECT @spMassZuschlag_1 = 0;
SELECT @spMassZuschlag_2 = 0;
SELECT @spMassZuschlag_3 = 0;
SELECT @spMassZuschlag_4 = 0;
SELECT @spMassZuschlag_5 = 0;
SELECT @spMassZuschlag_6 = 0;
SELECT @spMassZuschlag_7 = 0;
SELECT @spMassZuschlag_8 = 0;
--- Alle Kantenbearbeitungen durchlaufen
DECLARE select_cursor2 CURSOR FOR
SELECT mass_zuschlag, kantenmatrix
FROM pool_bearbeit
WHERE auftnr=@spAuftNr AND pos=@spPos AND u_pos=@spU_Pos
AND teile_nr = @spTeile_nr AND mass_zuschlag > 0;
OPEN select_cursor2;
FETCH NEXT FROM select_cursor2 INTO @spMassZuschlag, @spKantenmatrix;
WHILE @@FETCH_STATUS = 0
BEGIN
SELECT @spMassZuschlagFound = @spMassZuschlagFound + 1;
IF SUBSTRING(@spKantenmatrix, 1 , 1) = 1
SELECT @spMassZuschlag_1 = @spMassZuschlag_1 + @spMassZuschlag;
IF SUBSTRING(@spKantenmatrix,  2 , 1) = 1
SELECT @spMassZuschlag_2 = @spMassZuschlag_2 + @spMassZuschlag;
IF SUBSTRING(@spKantenmatrix, 3 , 1) = 1
SELECT @spMassZuschlag_3 = @spMassZuschlag_3 + @spMassZuschlag;
IF SUBSTRING(@spKantenmatrix , 4 , 1) = 1
SELECT @spMassZuschlag_4 = @spMassZuschlag_4 + @spMassZuschlag;
IF SUBSTRING(@spKantenmatrix , 5 , 1) = 1
SELECT @spMassZuschlag_5 = @spMassZuschlag_5 + @spMassZuschlag;
IF SUBSTRING(@spKantenmatrix , 6 , 1) = 1
SELECT @spMassZuschlag_6 = @spMassZuschlag_6 + @spMassZuschlag;

IF SUBSTRING(@spKantenmatrix , 7 , 1) = 1
SELECT @spMassZuschlag_7 = @spMassZuschlag_7 + @spMassZuschlag;
IF SUBSTRING(@spKantenmatrix , 8 , 1) = 1
SELECT @spMassZuschlag_8 = @spMassZuschlag_8 + @spMassZuschlag;
FETCH NEXT FROM select_cursor2 INTO @spMassZuschlag, @spKantenmatrix;
END
CLOSE select_cursor2;
DEALLOCATE select_cursor2;
IF @spMassZuschlagFound > 0
BEGIN
UPDATE pool_entschichtung SET
einzug_1_p1 = einzug_1_p1 + @spMassZuschlag_1,
einzug_1_p2 = einzug_1_p2 + @spMassZuschlag_1,
einzug_2_p1 = einzug_2_p1 + @spMassZuschlag_2,
einzug_2_p2 = einzug_2_p2 + @spMassZuschlag_2,
einzug_3_p1 = einzug_3_p1 + @spMassZuschlag_3,
einzug_3_p2 = einzug_3_p2 + @spMassZuschlag_3,
einzug_4_p1 = einzug_4_p1 + @spMassZuschlag_4,
einzug_4_p2 = einzug_4_p2 + @spMassZuschlag_4,
einzug_5_p1 = einzug_5_p1 + @spMassZuschlag_5,
einzug_5_p2 = einzug_5_p2 + @spMassZuschlag_5,
einzug_6_p1 = einzug_6_p1 + @spMassZuschlag_6,
einzug_6_p2 = einzug_6_p2 + @spMassZuschlag_6,
einzug_7_p1 = einzug_7_p1 + @spMassZuschlag_7,
einzug_7_p2 = einzug_7_p2 + @spMassZuschlag_7,
einzug_8_p1 = einzug_8_p1 + @spMassZuschlag_8,
einzug_8_p2 = einzug_8_p2 + @spMassZuschlag_8,
lastmodzeit = CURRENT_TIMESTAMP, lastmodstation = 'AUW_SP'
WHERE auftnr=@spAuftNr AND pos=@spPos AND u_pos=@spU_Pos
AND teile_nr = @spTeile_nr AND lastmodstation <> 'AUW_SP';
END
FETCH NEXT FROM select_cursor1 INTO @spTeile_nr;
END
CLOSE select_cursor1;
DEALLOCATE select_cursor1;
END
GO
## Configuration cutting code driver
For configuration of extended edge deletion you have several records in OPT2TXT configuration file. The most driver looks on record 118, XCEDICUT looks on record 98. In the AUW base configuration extended edge deletion is disabled, but there are DL files for activating.
An exact documentation of the configuration you will find in the OPT2TXT documentation.
A cutting code driver only generates extended edge deletion information in the cutting code, if this information are stored in OPT2 files. The detailed scheduling of A+W Production writes this information into OPT2 files, if the flag deletion is active in the master data of the cutting table.
### Enable and disable extended edge deletion
If not specified in another record, use record [118:1-5] (00000 = disabled).
HEGLA – XCEDICUT: 	[98:37] (0 = enabled / 1 = disabled)
BOTTERO – XCBOTHPS: 	[53:37] (0 = enabled / 1 = disabled); *since version 1.72 (28.04.2015)*
### Minimum width of extended edge deletion
Not every width should be written into cutting code interface. In order not to slow down the cutting process, a strip of 11mm should be processed with normal edge deletion and not with the extended edge deletion.
This parameters describes the width until the extended edge deletion should be suppressed.
If not specified in another record, use record [118:71-75] (format 1/10mm).
HEGLA – XCEDICUT: 	[98:38-41] (0.1 mm)
LISEC – XCLICUT: 	[104:12-15] (full mm); *since version 1.70 (11.06.2012)**; **use 118 as fallback*
BOTTERO – XCBOTHPS: 	[53:33-36] (0.1 mm); *since version 1.72 (28.04.2015)*
### Specials
For **XCEDICUT** it could be necessary to set OPT2TXT [98:47] to one, this suppress shape 98 in the cutting code (F records) which can make the cutting slow (e.g. on a lami cutting table). The parameter is available since XCEDICUT version 2.24.
For **LISEC** in the LISEC converter the licensed option “Stepped for Opt.Conv” is need to activate. If not, the extended edge deletion information will be ignored.
## Entry A+W Production
An editor for extended edge deletion can be open in rough scheduling **[Reentry / Edge Deletion]**.  The editor shows each soft coated sheet of the selection.

## Entry A+W Business
For IGU line items nothing special is need for order entry. In the master data for the spacer articles you have to define the cutback…

… and the spacer thickness.

This is need for A+W production to configure the right area.
Edge individual cutbacks are set manually during order entry in the BOM directly to the frame part.
Via a corresponding processing you can add an individual decoating on a coated glass. Add processing from processing group “decoating” at the cutting part which you want decoate.
The entered width will be decoted from each selected edge. If you want have different widths for different edges, you have to add one processing for each width.
### Change cutback with customizing
If a customer wants different cutbacks according to specific parameters (e.g., by area), this can be done via a customizing directly in A + W Business.
At customer ISOSKLO we have such a formula, which increases the cutback from master data for items with a big area (< 4m² + 0; < 6m² + 2; < 12m² + 4; >= 12m² + 6) and add values for an U-profil if exist (for U-profil no standard processing exist).
!**************************************************************************************;
!** Rückschnitt verändern nach Vorgaben von SGG ISOSKLO	**;
!** Formel wird als Eingabeprüfung in der Auftragsposition eingebunden **;
!**************************************************************************************;
!** Used Variables;
!** g_sqlUdv[0] = Handle to main database;
!** g_nUdv[0] => The current line item index;
!** g_nUdv[1] => Index for BOM;
!** g_nUdv[2] => Zähler für 1. oder 2. Abstandhalter;
!** g_nUdv[3] => Manueller Rückschnitt vorhanden, ;
!** g_nUdv[4] => Merker für 3-fach ISO;
!** g_nUdv[5] => BOM_Produkt;
!** g_nUdv[6] => Merker für Erhöhung Grenze 1;
!** g_nUdv[7] => Merker für Erhöhung Grenze 2;
!** g_nUdv[8] => Merker für Erhöhung Grenze 3;
!** g_nUdv[9] => Rückschnitt aus Stammdaten;
!** g_nUdv[10] => QM der Position;
!** g_nUdv[11] => LFM der Position;
!** g_nUdv[12] => QM Grenze 1;
!** g_nUdv[13] => QM Grenze 2;
!** g_nUdv[14] => QM Grenze 3;
!** g_nUdv[15] => LFM Grenze 2;
!** g_nUdv[16] => mm Erhöhung Grenze 1;
!** g_nUdv[17] => mm Erhöhung Grenze 2;
!** g_nUdv[18] => mm Erhöhung Grenze 3;
!** g_nUdv[19] => Rückschnitt Basiswert =10;
!** g_nUdv[20-27] => Parameter für U-Profil, an welcher Kante;
!** g_nUdv[28] => Anzahl Kanten;
!** g_nUdv[29] => Laufvariable;
!** g_nUdv[30-37] => Stufen;
!** g_nUdv[38] => BOM_ID SZR1;
!** g_nUdv[39] => BOM_ID SZR2;
!** g_nUdv[40-47] => Rückschnitt pro Kante;
!** g_nUdv[48] => Profil Dicke;
!** g_nUdv[49] => Profil vorhanden;
!** g_nUdv[50] => Auftrag;
!** g_nUdv[51] => Fetch Status;
!** g_nUdv[52] => BOM_ID SZR1 IndexVar;
!** g_nUdv[53] => BOM_ID SZR2 IndexVar;
!** g_nUdv[54] => Modellnr;
!** g_nUdv[55] => Stufe Glas;
!** g_sUdv[1] => Produkt-Array für Erhöhung um 1 mm;
!** g_sUdv[2] => Produkt-Array für Erhöhung um 2 mm;
!** g_nUdv[60-67] => U-Profil,Dicke an Kante x;
!**************************************************************************************;
! Get the current line item index;
Set g_nUdv[0] = frmDocumentItems.w_nPosIdx;
Set g_nUdv[1] = 0;
Set g_nUdv[2] = 0 ;
Set g_nUdv[3] = w_fktDoc.m_Pos[g_nUdv[0]].m_nPOS_BIT & nBIT_POS_RUECKSCHNITT;
Set g_nUdv[4] = 0;
Set g_nUdv[5] = 0;
Set g_nUdv[6] = 0;
Set g_nUdv[7] = 0;
Set g_nUdv[8] = 0;
Set g_nUdv[55] = 0;
Set g_nUdv[19] = 10;
Set g_nUdv[28] = 4;
! Manuelle Vorgaben für die Funktion Rückschnitt;
! ************* Produkt Array 1 *************************************;
SET g_sUdv[1]='8000,8001,8002';
! ************* Produkt Array 2 *************************************;
SET g_sUdv[1]='9000,9001,9002';
! ************* QM Grenze 1 *************************************;
SET g_nUdv[12]=4;
! ************* QM Grenze 2 *************************************;
SET g_nUdv[13]=6;
! ************* QM Grenze 3 *************************************;
SET g_nUdv[14]=12;
! ************* LFM Grenze 2 *************************************;
SET g_nUdv[15]=999;
! ************* mm Grenze 1 *************************************;
SET g_nUdv[16]=2;
! ************* mm Grenze 2 *************************************;
SET g_nUdv[17]=4;
! ************* mm Grenze 3 *************************************;
SET g_nUdv[18]=6;
! ************* mm Zuschlag für 3-fach ISO **********************;
! Aufruf nur, falls der Rückschnitt nicht manuell vorgegeben wurde;
IF w_fktDoc.m_Pos[g_nUdv[0]].m_nPROD_PRODART=PRDART_ISO AND g_nUdv[3]=0;
SET g_nUdv[49]=0;
SET g_nUdv[29]=0;
While g_nUdv[29]<8;
SET g_nUdv[g_nUdv[29]+20]=0;
SET g_nUdv[g_nUdv[29]+30]=0;
SET g_nUdv[g_nUdv[29]+40]=0;
! Änderungsvorschlag Herr Krejca;
SET g_nUdv[g_nUdv[29]+60]=0;
SET g_nUdv[29]=g_nUdv[29]+1;
WEND;
WHILE g_nUdv[1] < w_fktDoc.m_Pos[g_nUdv[0]].m_nStuklAnz;
! 1. Abstandhalter gefunden, Rückschnitt aus Stammdaten einlesen;
IF w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_PRODART = 60 ;
SET g_nUdv[5]=w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nBOM_PRODUKT;
IF g_nUdv[2]=0;
! Rückschnitt aus Stammdaten einlesen;
IF DbMakeTempConnect ( g_sqlUdv[0] );
IF SqlPrepareAndExecute( g_sqlUdv[0], DbParse('select BA_REDUKTION from SYSADM.BA_EKKAL where BA_PRODUKT=:g_nUdv[5] INTO :g_nUdv[9]') );
IF SqlFetchNext ( g_sqlUdv[0], g_nUdv[30] ) ;
!SalMessageBox ( 'Rückschnitt  '\|\|SalNumberToStrX(g_nUdv[9],0), 'Hinweis', MB_IconExclamation \| MB_Ok );
ENDIF;
ENDIF;
DbDisconnect(g_sqlUdv[0]);
IF g_nUdv[9]=0;
SalMessageBox ( 'Kein Rückschnitt in Stammdaten eingetragen!', 'Hinweis', MB_IconExclamation \| MB_Ok );
ENDIF;
SET g_nUdv[38]=w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nBOM_ID;
SET g_nUdv[52]=g_nUdv[1];
!SalMessageBox ( 'RS pro Kante  '\|\|SalNumberToStrX(w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_MOD.m_nRUECKSCHNITT[0],0)\|\|' Bomid '\|\|SalNumberToStrX(g_nUdv[38],0), 'Hinweis', MB_IconExclamation \| MB_Ok );
ENDIF;
ENDIF;
! 2. Abstandhalter vorhanden;
IF g_nUdv[2]>0;
SET g_nUdv[4]=1;
SET g_nUdv[39]=w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nBOM_ID;
SET g_nUdv[53]=g_nUdv[1];
ENDIF;
SET g_nUdv[2]=g_nUdv[2]+1;
ENDIF;
! Prüfen ob U-Profil in Stückliste vorhanden;
IF w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_PRODART = 20 AND w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_PRODGRP = 31 AND w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_DICKE >0 ;
SET g_nUdv[29]=0;
SET g_nUdv[48]=w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_DICKE;
SET g_nUdv[49]=1;
While g_nUdv[29]<8;
IF w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_BEARB.m_nBEA_PARAM[g_nUdv[29]]>0;
SET g_nUdv[g_nUdv[29]+20]=w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_BEARB.m_nBEA_PARAM[g_nUdv[29]];
SET g_nUdv[g_nUdv[29]+60]=g_nUdv[48];
ENDIF;
SET g_nUdv[29]=g_nUdv[29]+1;
WEND;
!SalMessageBox ( 'U-Profil gefunden  '\|\|SalNumberToStrX(g_nUdv[20],0)\|\|'param7 '\|\|SalNumberToStrX(g_nUdv[27],0), 'Hinweis', MB_IconExclamation \| MB_Ok );
ENDIF;
! Prüfen ob Stufe in Stückliste vorhanden;
!		IF w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_PRODART = 12 AND w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_PRODGRP = 50 ;
!			SET g_nUdv[29]=0;
!			While g_nUdv[29]<8;
!				SET g_nUdv[g_nUdv[29]+30]=w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_MOD.m_nMOD_STUFE[g_nUdv[29]];
!				SET g_nUdv[29]=g_nUdv[29]+1;
!			WEND;
!			SET g_nUdv[55]=w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_MOD.m_nSTUFE_GLAS;
!SalMessageBox ( 'Stufe gefunden  '\|\|w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_sSTL_BEZ, 'Hinweis', MB_IconExclamation \| MB_Ok );
!		ENDIF;
! Prüfen ob Modell in Stückliste vorhanden;
IF w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_PRODART = 12 AND w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_PRODGRP != 50 ;
SET g_nUdv[54]=w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_MOD.m_nMOD_NUMMER;
IF g_nUdv[54]=3 or g_nUdv[54]=4 or g_nUdv[54]=7 or g_nUdv[54]=8 or g_nUdv[54]=21 or g_nUdv[54]=37 or g_nUdv[54]=38 or g_nUdv[54]=53 or g_nUdv[54]=54 or g_nUdv[54]=110 or g_nUdv[54]=111 or g_nUdv[54]=112;
SET g_nUdv[28]=5;
ENDIF;
IF g_nUdv[54]=9 or g_nUdv[54]=10 or g_nUdv[54]=22 or g_nUdv[54]=43 or g_nUdv[54]=44 or g_nUdv[54]=55 or g_nUdv[54]=91 or g_nUdv[54]=129 or g_nUdv[54]=130;
SET g_nUdv[28]=6;
ENDIF;
IF g_nUdv[54]=19 or g_nUdv[54]=24 or g_nUdv[54]=90;
SET g_nUdv[28]=8;
ENDIF;
IF g_nUdv[54]=20 or g_nUdv[54]=25 or g_nUdv[54]=26 or g_nUdv[54]=41 or g_nUdv[54]=42 or g_nUdv[54]=45 or g_nUdv[54]=46 or g_nUdv[54]=51 or g_nUdv[54]=70 or g_nUdv[54]=71 or g_nUdv[54]=72 or g_nUdv[54]=73 or g_nUdv[54]=113 or g_nUdv[54]=115 or g_nUdv[54]=116 or g_nUdv[54]=117 or g_nUdv[54]=118 or g_nUdv[54]=134;
SET g_nUdv[28]=3;
ENDIF;
IF g_nUdv[54]=23;
SET g_nUdv[28]=7;
ENDIF;
IF g_nUdv[54]=60 or g_nUdv[54]=61 or g_nUdv[54]=81;
SET g_nUdv[28]=1;
ENDIF;
IF g_nUdv[54]=62 or g_nUdv[54]=63;
SET g_nUdv[28]=2;
ENDIF;
!SalMessageBox ( 'Modell gefunden  '\|\|w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_sSTL_BEZ, 'Hinweis', MB_IconExclamation \| MB_Ok );
ENDIF;
! BOM Index erhöhen;
Set g_nUdv[1] = g_nUdv[1] + 1;
WEND;
! Ergebnis auswerten;
SET g_nUdv[10]=w_fktDoc.m_Pos[g_nUdv[0]].m_nPP_QM_FAKT;
SET g_nUdv[11]=w_fktDoc.m_Pos[g_nUdv[0]].m_nPP_LFM_FAKT;
! qm > Grenze 1;
IF g_nUdv[10]>=g_nUdv[12];
SET g_nUdv[6]=1;
ENDIF;
! qm > Grenze 2;
IF g_nUdv[10]>=g_nUdv[13];
SET g_nUdv[6]=0;
SET g_nUdv[7]=1;
ENDIF;
! qm > Grenze 3;
IF g_nUdv[10]>=g_nUdv[14];
SET g_nUdv[6]=0;
SET g_nUdv[7]=0;
SET g_nUdv[8]=1;
ENDIF;
! lfm > Grenze 2;
IF g_nUdv[11]>g_nUdv[15];
SET g_nUdv[6]=0;
SET g_nUdv[7]=1;
ENDIF;
! Rückschnitt um x mm Grenze 1 erhöhen;
IF g_nUdv[6]>0;
SET g_nUdv[19]=g_nUdv[19]+g_nUdv[16];
ENDIF;
! Rückschnitt um x mm Grenze 2 erhöhen;
IF g_nUdv[7]>0;
SET g_nUdv[19]=g_nUdv[19]+g_nUdv[17];
ENDIF;
! Rückschnitt um x mm Grenze 3 erhöhen;
IF g_nUdv[8]>0;
SET g_nUdv[19]=g_nUdv[19]+g_nUdv[18];
ENDIF;
!SalMessageBox ( 'Udv19  '\|\|SalNumberToStrX(g_nUdv[19],0)\|\|' Udv6  '\|\|SalNumberToStrX(g_nUdv[6],0), 'Hinweis', MB_IconExclamation \| MB_Ok );
! Neuen Rückschnitt zurückschreiben;
IF g_nUdv[19]>g_nUdv[9];
SET g_nUdv[9]=g_nUdv[19];
ENDIF;
SET w_fktDoc.m_Pos[g_nUdv[0]].m_nRUECKSCHNITT=g_nUdv[9];
! Rückschnitt pro Kante zurückschreiben falls Profil vorhanden;
! Änderungsvorschlag Herr Krejca;
!IF g_nUdv[49]=1;
! An beiden SZR zurückschreiben;
IF g_nUdv[55]=2 OR g_nUdv[55]=5 OR g_nUdv[55]=6 OR g_nUdv[55]=0;
SET g_nUdv[29]=0;
While g_nUdv[29]<8;
IF g_nUdv[29]<g_nUdv[28];
SET g_nUdv[48]=g_nUdv[g_nUdv[29]+60];
SET g_nUdv[g_nUdv[29]+40]=g_nUdv[g_nUdv[29]+20]*g_nUdv[48]+g_nUdv[g_nUdv[29]+30]+g_nUdv[9];
SET w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[52]].m_MOD.m_nRUECKSCHNITT[g_nUdv[29]]=g_nUdv[g_nUdv[29]+40];
! 3-fach ISO;
IF g_nUdv[4]=1;
SET w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[53]].m_MOD.m_nRUECKSCHNITT[g_nUdv[29]]=g_nUdv[g_nUdv[29]+40];
ENDIF;
ENDIF;
SET g_nUdv[29]=g_nUdv[29]+1;
WEND;
ENDIF;
! Nur SZR1 mit Stufe, SZR2 ohne Stufe zurückschreiben;
IF g_nUdv[55]=1;
SET g_nUdv[29]=0;
While g_nUdv[29]<8;
IF g_nUdv[29]<g_nUdv[28];
SET g_nUdv[48]=g_nUdv[g_nUdv[29]+60];
SET g_nUdv[g_nUdv[29]+40]=g_nUdv[g_nUdv[29]+20]*g_nUdv[48]+g_nUdv[g_nUdv[29]+30]+g_nUdv[9];
SET w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[52]].m_MOD.m_nRUECKSCHNITT[g_nUdv[29]]=g_nUdv[g_nUdv[29]+40];
! 3-fach ISO;
IF g_nUdv[4]=1;
SET g_nUdv[48]=g_nUdv[g_nUdv[29]+60];
SET g_nUdv[g_nUdv[29]+40]=g_nUdv[g_nUdv[29]+20]*g_nUdv[48]+g_nUdv[9];
SET w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[53]].m_MOD.m_nRUECKSCHNITT[g_nUdv[29]]=g_nUdv[g_nUdv[29]+40];
ENDIF;
ENDIF;
SET g_nUdv[29]=g_nUdv[29]+1;
WEND;
ENDIF;
! Nur SZR2 mit Stufe, SZR1 ohne Stufe zurückschreiben;
IF g_nUdv[55]=4;
SET g_nUdv[29]=0;
While g_nUdv[29]<8;
IF g_nUdv[29]<g_nUdv[28];
SET g_nUdv[48]=g_nUdv[g_nUdv[29]+60];
SET g_nUdv[g_nUdv[29]+40]=g_nUdv[g_nUdv[29]+20]*g_nUdv[48]+g_nUdv[9];
SET w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[52]].m_MOD.m_nRUECKSCHNITT[g_nUdv[29]]=g_nUdv[g_nUdv[29]+40];
! 3-fach ISO;
IF g_nUdv[4]=1;
SET g_nUdv[48]=g_nUdv[g_nUdv[29]+60];
SET g_nUdv[g_nUdv[29]+40]=g_nUdv[g_nUdv[29]+20]*g_nUdv[48]+g_nUdv[g_nUdv[29]+30]+g_nUdv[9];
SET w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[53]].m_MOD.m_nRUECKSCHNITT[g_nUdv[29]]=g_nUdv[g_nUdv[29]+40];
ENDIF;
ENDIF;
SET g_nUdv[29]=g_nUdv[29]+1;
WEND;
ENDIF;
!ENDIF;
ENDIF;
## Entry A+W Enterprise
…
## Appendix 1 - Overview IG

## Appendix 2 - Troubleshooting
LOG files are generated with the ALCIM.EXE.CONFIG in module **Albwir.Basis**.
### Cutting code produce ERROR: doshp: error 314
This happens with XCLICUT, maybe with other driver too. The driver describes how the de-coating wheel does the edge deletion. If there is no 90° corner the wheel drive into the corner and delete so an area on the sheet aside too. If there is no shape trim, it could happen that the wheel delete more than the standard edge deletion does on the sheet aside.
How much is allowed it is defined in OPT2TXT [118:46-50] (StripOffPrimitivZone). The value -1000 is 10mm.
If you get the error there is a sheet in the optimisation where more area will be delete as defined in the value. You can increase the value. If the cutting code works with a higher value, take care about the sheet aside.
Another solution is to make the sheet bigger, to add a shape trim to the edge where the problem happens. This can be done with XRECALC. If XFRECALC is running before optimisation and the record 118 is filed in OPT2TXT, XRECALC add a shape trim to the shapes which have the problem.
This works if the standard KVALUE in OPT2FA is filled (this will not be done in ALCIM, detailed scheduling writes a 0 into the field).
A Problem could happen if you have different cutting tables with different values in record 118. So you have to fill always the right value into OPT2TXT record 118 before optimisation.
### Size of cutting rectangle increases
It could happens, that XRECALC increase the size of cutting rectangle. This can happen with a bad angle that forces the grinding wheel into the sheet beside.
To disable this check set in OPT2TXT [118:51-55] (StripOffPrimitivZoneCheck) to 0. 0 is the favored setting.
### Bad optimization result with extended edge deletion function
If in shape master data of A+W Production the TRIMs for shape 0 (rectangle) are set, the TRIM values will be used for optimization with extended edge deletion and increase the rectangle. This happens through the OPT2FA records which exist for shape 0 too. If the extended edge deletion function isn’t in use, the detailed scheduling don’t create OPT2FA records for rectangle. Solution: disable the TRIM for shape 0.
### Edge Deletion isn’t calculated – wrong Shape master data
In the A+W production Shape-Catalog you must be able to set information about round arcs on the shape. If this is not possible, a re-initialization of the Shape-Catalog is necessary.
All shapes with *RUNDBOGEN_FLAG = 0* are not initialized. Re-initialization for these shapes has to be done through shape master data in *ALCIM **à** Master Data **à** Shape **Masterdata** **à** Import Catalog*
**SELECT** **DISTINCT** rundbogen_flag,* **FROM** modellstamm **WHERE** rundbogen_flag = 0;

**ATTENTION:** Reinitializing the Shape Catalog (also with the option: Maintain existing data) will set the T-values back to default. To avoid this, the values from RUNDBOGEN_FLAG can be read from a Reference-Database with the following SELECT-statement (the result of the statement creates UPDATE-statements which can be used on the customer database).
**SELECT** "UPDATE modellstamm SET rundbogen_flag = " \|\| rundbogen_flag \|\| " WHERE mod_kat = 1 AND mod_nr = " \|\| mod_nr \|\| ";" **FROM** modellstamm **WHERE** rundbogen_flag <> 0 **AND** mod_kat = 1;
## Appendix 3 - Specials
### Special Solution for POOLASC
In older versions of ALFAK a processing with type 1025 cannot be transferred to ALCIM. For those cases there is the Stored Procedure **cu_setEntschichtung**. This SP fills the respective fields in the POOL_BEARBEIT and returns the processing type (should be **1025,** default type). To make the extended edge deletion noticing this processing, a hidden switch must be activated:
**[ALCIMPRT_SETTINGS / AW_PROC_TYPE]**
*0 = processing is not considered by the **extended edge** deletion (default)*
*1 = SP is not executed; default processing type is used (1025)*
*2 = SP is executed; processing type the SP returns is used (should also be 1025)*
### Customizing on calculated results
If it is needed to manipulate the calculated result with a stored procedure during the import process (CU_PRT_ITEMWRT), the parameter **[ITEMS4ALCIM_SETTINGS / ALCIMPRT_MODE]** has to be set to 1. Value 0 executes the stored procedures before the extended edge deletion calculation.
### Enter the deletion size only via editor
Detailed Scheduling or XOPTON only writes the deletion size into optimisation files if the function for extended edge deletion in the import is activated. If Detailed Scheduling is also supposed to write them if the function is deactivated and the customer defines the deletion size manually through the editor in ALCIM, this is only possible with a hidden switch which is able to overwrite the settings from the import.
**	****[****FEIN_SPECIALS / CALCULATE_GRINDINGAREA****]**
* **0 **= take settings from import (standard)*
*1 = no matter what settings in import, write the deletion information*