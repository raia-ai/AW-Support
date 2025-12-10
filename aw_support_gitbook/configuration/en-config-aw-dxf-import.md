---
description: "EN CONFIG A+W DXF Import"
---



# EN CONFIG A+W DXF Import

     Configuration Instructions


DXF files in A+W Programs




                                  english
Change history


Date             Author                    Comments                                 Version
2021-04-19 EB                              Original version                         1.0
2021-05-10 BH                              Correction
2023-02-02 SVH                             [AW-82801] – Rotated shapes




Content

1.         General                                                                             4
2.         DFX import                                                                         5
  2.1.     A+W CAD Designer(Shapes)                                                           5
     2.1.1. Function                                                                           5
     2.1.2. Import dialog in the A+W CAD Designer                                              6
     2.1.3. Configuration (SN.ini):                                                            6
     2.1.4. Detection in DXF import                                                            7
     2.1.5. Templates, macros, and DXF files in setup                                          7
     2.1.6. AUTOCAD 2018 files                                                                 8
 2.2.      A+W Business                                                                       8
     2.2.1. Expanded DXF import dialog                                                         8
 2.3.      A+W Enterprise                                                                      8
     2.3.1. DXF import dialog                                                                  8
     2.3.2. Detailed information                                                              10
 2.4.      A+W Production                                                                     10
     2.4.1. Geometry calculation uses the configured view for DXF export                      10
     2.4.2. Geometry calculation: expansion of the automated DXF generation                   10
 2.5.      Troubleshooting                                                                    11
     2.5.1. Importing DXF file with layouts                                                   11
     2.5.2. Import of DXF files with layers, which have a blank space in the name             11
     2.5.3. Improved file selection when importing DXF files                                  11




A+W Software GmbH                        EN-CONFIG-A+W DXF-Import.docx                             3
1. General
Files in DXF format can be imported into the A+W CAD Designer (Shapes) The individual
functions for the topic DFX import are collected in this document.




A+W Software GmbH              EN-CONFIG-A+W DXF-Import.docx                            4
2. DFX import
2.1. A+W CAD Designer(Shapes)
2.1.1. Function
A+W CAD Designer (Shapes) can import shapes from DXF files. The geometric data is interpreted
as outlines of glass products (exterior shapes, drillings, and cut-outs). The data in the DXF files can
be extremely varied; depending on the type of the file, the data import can run nearly
automatically, require manual reworking or possibly not be possible. There is no standard for how
objects of different quality are described in DXF; for example, glass contours in comparison to
surface processings. During the import into A+W CAD Designer (Shapes), all data is interpreted as
glass contours.


The following guidelines should help design DXF files so that they can be imported from
A+W CAD Designer (Shapes) without a problem.
    1.   A shape to be imported should be complete and only on one DXF layer. If several
         shapes should be imported by a DXF file, it is best if each shape is on its own
         layer. If in the DXF file there are labels, dimensions, legends, etc., then it is best if
         these elements are on layers separate from the shapes. During the import, it is
         possible to select one or several layers on a selection dialog.
    2.   The shape to be imported should be closed. Open shapes require reworking in the
         A+W CAD Designer (Shapes).
    3.   The separating points of adjacent segments of a shape (e.g. lines or arcs) should
         match. During the import, seamless curves have to be generated. There is a
         configurable capture radius for the chaining. However, if the gaps are too large,
         manual reworking is required. It is possible that the result of the import is not
         clear.
    4.   Only 2-dimensional data is imported. The geometric objects have to be on one
         level. (the third coordinate z has to be equal to 0 or constant).
    5.   Only particular geometric data (entities) are imported. The rest of the entities are
         ignored. Imported are: ARC, LINE, CIRCLE, POLYLINE, LWPOLYLINE, ELLIPSE,
         SPLINE. Internally, A+W CAD Designer (Shapes) works with lines and arcs. Ellipses
         and splines are converted in sequences of lines and arcs. Depending on the
         configuration, polylines are also converted. This is the case, e.g. if they consist of
         a lot of segments.
    6.   No texts or dimensioning objects are imported.
    7.   Blocks are read and inserted according to the INSERT entities. In case of several
         insertions, the data is duplicated. The block structure itself is not taken over. A
         scaling factor is heeded for INSERTs, not supported, however are non-
         homogeneous scalings (different scaling factors in x and y)




A+W Software GmbH                   EN-CONFIG-A+W DXF-Import.docx                                     5
Handling of edge cut-outs
In A+W CAD Designer (Shapes), a shape is described by a basic form and additional edge cut-
outs. The basic form is usually cut, the edge cut-outs are milled out in subsequent steps.
This breakdown is important for production. The shape can exist differently in DXF files:
    1. As closed curve in which the cut-outs are already included
    2. As closed basic form with additional closed interior contours, which describe the
        cut-outs
    3. As closed basic form with additional open interior contours, which describe the
        cut-outs
Variant 2 corresponds to the display in the A+W CAD Designer (Shapes), the import is
then especially unproblematic.
The variants 1 and 3 are also supported starting with Version 6 of the A+W CAD Designer.
With Variant 1, it has to be noted that the breakdown into outer form and edge cut-out is
not always completely clear. At the customer, this is oriented according to what should
be cut (what is breakable). There are configuration settings for this.



2.1.2. Import dialog in the A+W CAD Designer
During import, first the user is presented with a dialog for selecting the layer. Here the DXF file is
displayed, as it would look in a DXF viewer. Dimensions, symbols, and segments are displayed in
the colors stored in the file. This simplifies the interpretation of the data for the user and the
correct selection of the relevant layer with the glass data. After the selection, the selected layer is
taken over into the 2D view of the A+W CAD Designer (Shapes). A+W CAD Designer (Shapes)
displays the imported segments. Closed curves are highlighted in red. With open curves or curves
with gaps, the problematic points are highlighted. In the 2D import view, a complete view of the
DXF file is displayed in grayed-out color in the background. This enables the user to make
purposeful corrections. During the change to the GEOMETRY view, the closed curves are taken
over.


2.1.3. Configuration (SN.ini):
In the DXFImport partition
MeasurementsInMM: The units in the DXF file. The default value 1 stands for mm; with 0, all
                  values are interpreted as INCH.
CreateCounterbore:       Circles are converted to cylindrical drillings (0, standard) or countersunk
                         drillings (1).
In the user partition
ImportDrillholeMaxDiameter: Circles up to this radius are converted to drillings.
Additional configuration possibilities (DXFImport partition)
 CaptureRadiusStartingValue:                Capture radius for the chaining of segments (default
                                            value 0.01).
 MinimumEntityExtendForShapeConstr          Segments with smaller lengths are ignored; default
 uction:                                    value is 0.01 mm.


A+W Software GmbH                   EN-CONFIG-A+W DXF-Import.docx                                      6
 USEXTREAM:                                Curve smoothing with XTREAM, the default value 1
                                           activates this option.
 USETANGENTXTREAM:                         Tangents on the end of splines and ellipses are
                                           considered in XTREAM (default value 1)
 SmoothPolylinesMinEntries:                Automatic smoothing for POLYLINES and
                                           LWPOLYLINES with many segments. The whole-
                                           number value determines the minimum number of
                                           segments with which the smoothing is activated.
 PointResolution:                          Resolution of SPLINES and ELLIPSES in points
 UseCADImage:                              Preview with viewer (CADImage) activated
 ShowFrozenOrInvisibleLayers:              Default 0, display only active layer
 SmoothPolylinesPointResolution:           Resolution of polylines in points
 ConsiderRotatedShapes                     [AW-82801] - Deactivate (=0) the detection of
                                           rotated shapes starting with SN Version 13.4.2769


MAXCORNERANGLE, MINIINTERIORRADIUS, NORMACCURACY: Configuration curve smoothing.


2.1.4. Detection in DXF import
Cut-outs and roundings
The detection of cut-outs and roundings on the DXF import dialog can now be deactivated with a
switch (SN.ini, section DXFImport, EnableFeatureRecognition = 0). This way, it is easier to restore
the behavior of Version 5. (AwDesk: 394165)


Rotated shapes [AW-82801]
The deactivateion of the rotated detection ConsiderRotatedShapes = 0 is the recommended
configuration. Otherwise with the attachment/reporting of processings with dimension type 0
(reference to the circumscribing rectangle) there are amibiguities. If a customer imports and
produces only simple shapes (without drillings/cut-outs), ConsiderRotatedShapes = 1 can also be a
sensible option.
See also:
SN.ini, Abschnitt StandardShapes, ConsiderSmallerRectanglesOnly = 1.
In general, several standard shapes are detected for a shape. Which of these is selected will be
determined using different criteria; e.g. non-rotated shapes are preferred. If only a rotated shape
is detected, the circumscribing rectangle for the rotated shape (of the shape) can be larger than
the circumscribing rectangle in the initial position. This is awkward (e.g. more waste). With a
switch, these shapes can now be ignored, if necessary, no shape at all is detected.



2.1.5. Templates, macros, and DXF files in setup
In the SN program directory, in the AUW folder, there are the following new subdirectories:


A+W Software GmbH                  EN-CONFIG-A+W DXF-Import.docx                                      7
        • Macro
        • Templates
        • DXF

These directories contain appropriate files. (AwDesk: 327042)

The SN ConfigTool copies the new directory (Macro, DXF, Template) with content into the user's
server directory, but only if these directories have not yet been created.


2.1.6. AUTOCAD 2018 files
The DXF preview dialog in AWE/AWB/A+W CAD Designer (Shapes) now also supports the display
of AUTOCAD 2018 DXF files. (AwDesk: 418053)


2.2. A+W Business
2.2.1. Expanded DXF import dialog
With Version 6, there is a DXF import available in AW Business, which in standard cases (a simple
shape with processings) offers a very quick import of the data. In particular, processings (cut-outs,
drillings, roundings) are detected automatically. This dialog now opens in the CAD Designer when
opening a DXF file. In the CAD, the user has two possibilities for closing the dialog : Import shape
and Import data. With Import shape an import is started that is oriented toward detecting
precisely one shape with its processings. Here, cut-outs, drillings, and roundings are detected
automatically. The cutting form does not include the cut-outs. If the data is more general (e.g.
includes several shapes or additional objects), the data can be taken over via Import data. Then it
may be necessary to rework it more manually in the CAD.
The new dialog is displayed if you select File>Open from the menu. The old dialog is still available
via File>Import>DXF . With the switch UseFeatureDialog = 0 in the section DXFImport of the SN.ini
the new dialog can also be deactivated completely. In the course of the TOE in AWE it is also very
practical to use the new dialog viaFile>Import>DXF . For this, you can activate the dialog in this
case too with the switch UseFeatureDialogFileImport = 1. Here, however, you must heed that if
you exit the dialog with Import shape, all previous processings in the current document are
deleted.
For additional information, see A+W Business configuration instructions


2.3. A+W Enterprise
2.3.1. DXF import dialog
There is a new dialog available for DXF files, which can be started during the order entry. The new
dialog should allow that more DXF files can be imported into the A+W CAD Designer without
manual reprocessing.
The dialog offers better possibilities for
    •   Filtering DXF data


A+W Software GmbH                    EN-CONFIG-A+W DXF-Import.docx                                  8
      •   Detecting features
      •   Setting options
There is a preview of the DXF file. It is possible to select by levels (Layer) and colors (color index,
ACI). For this, a list of the existing levels and colors is displayed. The preview shows the currently-
selected objects.
After the selection, there is a detection of the objects. Especially the automatic detection of edge
and corner cutouts has been improved. The exterior contour is taken apart into a convex base
shape (that can be cut) and additional cutouts. Cutouts that are depicted by dotted lines within
the exterior shape are recognized.
Furthermore, options for the import can be set. This especially affects processings that may not
be depicted clearly in the DXF. For holes it is possible to select whether they should be sunk. The
sink depth and angle can be specified by the user. It is also possible to make the sinking only for
holes that are depicted with several concentric circles.
Roundings in the exterior shape are recognized as processings. A limit radius can be specified. All
roundings with larger radius are assigned to the base shape, all roundings with smaller radius are
evaluated as processings. Thus a rectangle with rounded corners can be imported as rectangle
with processing round corner or as shape 75 of the A+W shape catalog.
For cut-outs, additional rounding radii and an edge quality can be added.
The new DXF dialog offers no opportunity to select and manipulate individual object, that is, to
shift or delete a particular line or sink one hole and another not. For this, it is still necessary to
import the file with the A+W CAD Designer. On the other hand, the user does not need any
special CAD knowledge for the dialog and he can import DXF files very quickly and easily.
Master data
Under Keys -> System -> Document types a document of the type DXF must be created. Only one
document of this type may be present. Under this type, a copy of DXF file is backed up in the
position.

Order entry
It is possible in the dimension fields of the item to import a DXF file analogous to the takeover of a
SN file. During the import, a SN file is generated from the information of the DXF file.
With Ctrl+B you use the file explorer to select an existing DXF file. This starts the DXF import
dialog on which the form to be imported is displayed. If the import is confirmed with OK and if the
import can be done without errors, then the user has the opportunity either to synchronize the
AWE BOM with the generated SN file or to take over the generated SN file directly without
synchronization.
The initially selected DXF file is added to the item as file attachment, so that it remains traceable
how the SN file was generated.The DXF file attachment has a fixed type (see master data) and can
only be present once per item.
The DXF file attachment has a fixed type (see master data) and can be present only once per item.
In addition to the method described above, the assignment of a DXF file can also be done directly
from the CAD file field in the item (Properties tab) via the selo (<F9>). Here, the user is initially
asked which file type (SN or DXF) he would like to select. In the file explorer, then only the files of
the selected file type are displayed.

EDI
In the external order scheduling, there is no logic available for the import of DXF files.


A+W Software GmbH                    EN-CONFIG-A+W DXF-Import.docx                                       9
Change of the BOM drillings in the DXF import view
It is now possible to adapt the BOM of the drillings in the DXF import view. This way,
the drillings can be distributed across different lites.

2.3.2. Detailed information
For additional detailed information regarding DXF import, please see the "Enterprise"
configuration instructions.




2.4. A+W Production
2.4.1. Geometry calculation uses the configured view for DXF export
During scheduling or on the occasion of the detailed scheduling, the geometry calculation
AlcimWorks generates output files for the optimization and the printing of forms. Since Version
5.4 a DXF file is also generated automatically insofar as a machine with the name ALCIMDXF is
configured in the configuration file in the CAD designer (Shapes) (aka SN.INI).
In the previous versions of the geometry calculation, the DXF export was generated from the
GRIND view (grind), regardless of which view was configured in the section [ALCIMDXF] in the
VIEW = entry.
This limitation is now eliminated so that any valid view can be used for the DXF export. There is no
validity check. (AWDesk: 361912)


2.4.2. Geometry calculation: expansion of the automated DXF
    generation
In the geometry calculation AlcimWorks for a while it has been possible to generate a DXF file for
the end product.

This possibility has now been expanded so that at the same time the cutting geometry is output,
another DXF file can be generated.

In order to activate the DXF output from the second view, a machine ALCIMDXF2 must be entered
in the [Customer] section of the SN.INI. The view from which the exporting is done is configured in
the section [ALCIMDXF2].

In contrast to the output ALCIMDXF, which only takes place for header parts, ALCIMDXF2 is
executed for all BOM levels.

Caution: the turning for cutting due to layer and structure changes is done using the mirror ID in
the BLOCK.ZIP; therefore, the machine output does NOT turn the machine output from the
geometry calculation. This also applies for the DXF files generated from the UNICUT view.

Caution: with use of the functionality in Version 2011, the driver installation for Shaping/Nesting
must also be executed in the directory %UserProfile%\A+W\Techsoft\SN\. (AwDesk: 364862)


A+W Software GmbH                  EN-CONFIG-A+W DXF-Import.docx                                  10
2.5. Troubleshooting
2.5.1. Importing DXF file with layouts
In a DXF file, there can be additional layouts in addition to the shape. These are views of the
shape with additional information (e.g. legend). If in these layouts there are additional geometric
objects (e.g. lines) and these objects are on the same DXF layers as the shape, then these objects
are also imported into the A+W CAD Designer under some circumstances. In connection with the
DXF import in AWB/AWE, it can happen that there were several shapes and a takeover of the data
was not initially possible. Now these additional objects are no longer imported. (AWDesk: 425138)


2.5.2. Import of DXF files with layers, which have a blank space in
    the name
Blank spaces in the names of layers were not permitted in earlier versions of the DXF format.
That's why there is an error in the DXF import if a DXF file is imported, which on the one hand
contains layers with blank spaces and on the other hand was written in an older version of the
DXF format. In the A+W CAD Designer, it is now also possible to import such files. (AwDesk:
431224)


2.5.3. Improved file selection when importing DXF files
For importing DXF files, the program suggests the directory from which the last DXF file was
imported. The program used to ignore, however, whether or not this directory was actually
available. The program therefore checks now whether the directory from which the last DXF file
was imported, is available at all. If it is not, the file selection dialog is started in a standard
directory that is sure to exist.

The standard directory in which the file selection dialog starts should the last used directory be
not available, is %AWALLUSERS%\Xopt. (AwDesk: 245325)




A+W Software GmbH                  EN-CONFIG-A+W DXF-Import.docx                                      11

