---
description: "EN CONFIG A+W Production Filling Corner"
---



# EN CONFIG A+W Production Filling Corner

      Configuration


A+W Production: Filling corners and
capillary tubes




                                   english




                          - -INTERNAL-
1. Contents
Change history


Date            Author                Comment                                 Version
2021-02-11      D. Dreier             AWP installation and configuration      1.0
2021-03-17      D. Dreier             A+W Production Terminal Setup
2021-03-23      E. Tempelfeld         Document formatting, publication        1.1




Contents

1.   Contents                                                                                 3
2.   General Information                                                                      4
     2.1. New A+W processing types                                                            4
     2.2. Extensions in A+W Enterprise                                                        4
          2.2.1. Filling corner (A+W type 1661)                                               4
          2.2.2. Capillary tube (A+W type 1662)                                               4
3.   Program update                                                                           6
4.   A+W Designer (Shapes)                                                                    7
     4.1. Adjustment of the SN.INI                                                            7
     4.2. Display of the filling corner in SN                                                 7
5.   A+W Production                                                                         8
     5.1. Article master data                                                               8
     5.2. Processing master data                                                            8
          5.2.1. Creating the processing type                                               8
          5.2.2. Creating the processing article                                            9
          5.2.3. Generation of the processing 1661 – filling corner by the BOM configurator 9
     5.3. Machine assignment                                                               10
          5.3.1. Create work process                                                       10
          5.3.2. Assignment of a machine to the work process: set filling corner           11
     5.4. Scheduling – Orders4Production                                                   12
          5.4.1. Activate work step                                                        12
     5.5. Flow (results)                                                                   12
          5.5.1. Data for use for the batch formation                                      13
          5.5.2. Data for Production Terminal                                              13
          5.5.3. General data for the filling corner                                       13
          5.5.4. Examples                                                                  14
6.   Contact Address                                          Fehler! Textmarke nicht definiert.




A+W Software GmbH            EN-CONFIG-A+W Production Filling Corner.docx                          3
2. General Information
A robot is used in operations to fill IG and LAMI glasses with gel. For this Pressure compensation
(capillary tubes and filling corners) processing, the following parameters are required:
    • Corner
    • Distance to the corner




    •   Edge

    • Angle of rotation
Whereby the angle of rotation is primarily required for robot control.
Basis for the development is the processing Pressure compensation = awtyp 1660


2.1. New A+W processing types
1661    Filling corner
1662    Capillary tubes
These A+W processing types are described precisely in the normal A+W processing catalog.


2.2. Extensions in A+W Enterprise
2.2.1. Filling corner (A+W type 1661)
To affix a filling corner, only the parameter corner is required.


2.2.2. Capillary tube (A+W type 1662)
For capillary tubes, the dimensioning by corner/edge is supported. The distance to the corner has
to be input. Optionally, an angle depending on an edge can be entered if the capillary tubes
should have a special orientation. Furthermore, it is possible to enter a type for the capillary tube
if there are several types.
External standard interface
The B1 records have to be scheduled as follows:
Filling corner (1661)
Parameter       Meaning
1               Corner
Capillary tube (1662) (only AWE status as of: 25.01.21)


A+W Software GmbH            EN-CONFIG-A+W Production Filling Corner.docx                            4
Parameter      Meaning
1              Corner
2              Distance to corner
3..10          Edge 1 – 8
11             Angle of rotation
12             Reference edge
13             Type no. (different articles)
Transfer to production and creation of sketches:
For the transfer to production and the creation of the sketches, the appropriate modules have to
be updated (see the additional chapter)




A+W Software GmbH          EN-CONFIG-A+W Production Filling Corner.docx                            5
3. Program update
In order to be able to use the new A+W processing type 1661 - Filling corner to the fullest extent,
the following programs have to be updated:
    1. The processing type 1661 is available starting with the OrderXML version 5.5.0006.
    2. A+W Production – Version 13. QR: 2/21
    3. A+W CAD-Designer (Shapes) – Version 13. QR: 2/21
    4. A+W Production Terminal
       [For installation, please consult the Automation Team in advance!]

        http://tfs2012.a-
        w.intra:8080/tfs/glasssuite/Production/Production%20Team/_versionControl?path=%24
        %2FProduction%2FDevMaps%2FClarity%2FCIM%2FPanorama%2FMCJobInsertTV%2FVetr
        otech&_a=contents


    5. A+W Production Monitor (\\jupiter\SW_Install\v6\Diskset\A+W Production Monitor )


When executing from the SetupLauncher, make sure that A+W Production and A+W CAD Designer
(Shape) are selected.




A+W Software GmbH           EN-CONFIG-A+W Production Filling Corner.docx                              6
4. A+W Designer (Shapes)
4.1. Adjustment of the SN.INI
In the sn.ini file ((TRANS)P:\SN\SN.INI), the following sections have to be adjusted:
[Customer]
FileVersion= 13.4.2194


4.2. Display of the filling corner in SN
The size of the corner filling in the SN sketch is determined by the settings FillingCornerWidth and
FillingCornerHeight.
The standard sketch is provided with the A+W CAD Designer (Shapes) SetUp in
SNInstallationFolder\SurfaceImage.
The title of the image file has to be FillingCorner. The extension can be EMF, PNG, BMP, JPG or
JPEG.
In order to display the image in SN sketch, this image has to be copied to the configured motif
folder, typically a subfolder of the trans/SN network folder (this can be configured in A+W
Enterprise via environment variable).
Whether a corner is suitable for the automatic placement of filling corners is defined by the
setting MaximumHorizontalFillDistance.
The SN tool for inserting a filling corner has the name FILLCORN. It can be added to the tools in
the INCONT view (setting INCONTadditionalTools).




A+W Software GmbH           EN-CONFIG-A+W Production Filling Corner.docx                            7
5. A+W Production
To support setting the filling corner on the fire protection glass unit, an appropriate processing
article on the article type of the unit is required.
It can be provided by the ERP system or generated in the production system (BOM configurator).


5.1. Article master data
Fire protection glass is mapped to the article type 9 - cast resin:




5.2. Processing master data
In the processing master data, the processing article is assigned a processing type. This
corresponds to the A+W processing type of the filling corner.


5.2.1. Creating the processing type




A+W Software GmbH            EN-CONFIG-A+W Production Filling Corner.docx                            8
5.2.2. Creating the processing article
The type 1661, created in advance, has to be selected as type. The A+W processing type cannot
yet be selected here.




5.2.3. Generation of the processing 1661 – filling corner by the BOM
    configurator
To generate the processing, go to Master Data > Capacity Planning > Processing Generation as
follows:




A+W Software GmbH          EN-CONFIG-A+W Production Filling Corner.docx                         9
Via an additional condition, it has to be ensure that the processing if only generated if it does not
yet exist (transfer from the ERP system).


5.3. Machine assignment
5.3.1. Create work process
The master data of the machine assignment has to be expanded to include the work process Set
filling corner.
Master Data > MA Editor > Tab: work processes




A+W Software GmbH            EN-CONFIG-A+W Production Filling Corner.docx                          10
5.3.2. Assignment of a machine to the work process: set filling
    corner
In principle, here you can create a new machine with handling in the capacity planning. It is also
sufficient if the dummy machine is used for information processings. However, this depends on
the structure of the whole organization.




A+W Software GmbH           EN-CONFIG-A+W Production Filling Corner.docx                             11
5.4. Scheduling – Orders4Production
The handling of the filling corner was implemented in a separate work step:
Proc1661RelData_23734.


5.4.1. Activate work step
Master Data > Configuration > Parameters > Order Import (Orders4Production) > Sequence for
Order Import:




List of the active work steps:
...
MachineryAllocation; 6
Capacity; 4
AlcimWorks; 6
SPCall; 8
Proc1661RelData_23734; 1
GrindArea; 8


5.5. Flow (results)
The work step is started after the set-up edge and the turning logic (implemented under SPCall)
have been run through.
As result, you get the following data:




A+W Software GmbH            EN-CONFIG-A+W Production Filling Corner.docx                         12
5.5.1. Data for use for the batch formation
POOL_BEARBEIT.MASS15:        Placement possible: 1 robot / 0 manual


5.5.2. Data for Production Terminal
   •   POOL_BEARBEIT.MASS12:          Parameter 1-> Offset
   •   POOL_BEARBEIT.MASS13:          Parameter 2-> Height
   •   POOL_BEARBEIT.MASS14:          Parameter 3-> Angle
   •   POOL_BEARBEIT.MASS15:                 Placement possible: 1 robot / 0 manual -> Parameter
       4: Implementation after: 1 = No data present / place filling corner manually (definition
       according to Bystronic)




   •   POOL_TEILE.AUSGANGSNR:         The unit is produced turned
   •   MZO_EINSTELLEN.WENDEN_IN:      The unit is produced turned on this machine
   •   MZO_EINSTELLEN.KANTE_IN:       The set-up edge on this machine


5.5.3. General data for the filling corner
   •   POOL_BEARBEIT.MASS1: Corner
   •   POOL_BEARBEIT.MASS2: Edge



A+W Software GmbH         EN-CONFIG-A+W Production Filling Corner.docx                       13
   •   POOL_BEARBEIT.MASS3: Angle
   •   POOL_BEARBEIT.MASS4: Edge
   •   POOL_BEARBEIT.MASS5: Angle
   •   POOL_BEARBEIT.MASS6: useAsSpecified by ERP
   •   POOL_BEARBEIT.MASS7: typeId - different articles


   •   MASS1: Corner [ENUM] gibt die Ecke an, in der die Füllecke zu platzieren ist. Element:
       ComponentOrientation serves to help you place the component relative to an edge. This can be
       necessary, for example, if a robot affixes the filling corner automatically.
   •   MASS2: Edge: [ENUM] specifies the edge to which the installation angle refers.
   •   MASS3: Angle [double] specifies the angle counter-clockwise – with respect to
       ComponentOrientation.Edge Element: FillingOrientation serves to help you specify the filling angle
       relative to an edge.
   •   MASS4: Edge: [ENUM] specifies the edge to which you refer the filling angle.
   •   MASS5: Angle [double] specifies the angle counter-clockwise – with reference to
       FillingOrientation.Edge.
   •   MASS6: useAsSpecified [boolean] serves so that the defined data and specified in the production
       system is taken over.
   •   MASS7: typeId [int] serves so that you can map different component variants (thickness
       dependent).


5.5.4. Examples




A+W Software GmbH           EN-CONFIG-A+W Production Filling Corner.docx                               14

