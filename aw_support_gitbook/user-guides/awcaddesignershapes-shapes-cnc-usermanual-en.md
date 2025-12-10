---
description: "EN-UM-AWCADDesignerShapes_11"
---


---
## Tools & Fixed Questions

7.  Go to the shape view. Click on the magnifier. A+W Business shows the shape and the corresponding list of variables in a separate dialog.
    A+W Business will show only the variables saved in the SN file under a name starting without an underscore (_).
    Variables the names of which start with two underscores, can be automatically assigned values by A+W Business. A+W Business needs to be configured for this.
8.  Enter the required order item values for the variables.
9.  Press [OK]. The item will be recalculated with the current values; a new drawing is displayed.
10. Quit the shape view by clicking on [END]. In the field for the file name, the name of the template file has been replaced by the name of the file created with the new values.
11. Save the item.

> **Changes can be made in the SN file!**
> If you save an item then load it again to change the values of the variables, A+W Business will also update the SN file.

### Create automatic variables

Variables have to be entered in the following fashion in SN templates you want to dimension automatically in A+W Business:

`__XXXX_YY_ZZ`
(2 underscores, 4 numbers, 1 underscore, 2 numbers, 1 underscore, 2 numbers)

*   **XXXX** = four-digit product number for the processing in A+W Business.
*   **YY** = how often does this processing step occur in the glass to be processed.
*   **ZZ** = processing size to be analyzed.

To use automatic variables, proceed as follows:

1.  Create a SN file with the required contour.
2.  Dimension the contour using variables.
    Use variable names acc. to pattern described above.
3.  Enter the A+W Business product number (XXXX) in the variable.
4.  In the variable, which of the existing processing steps (in the A+W Business BOM for the glass) shall be used to preset the dimension (YY).
5.  In the variable, define the processing parameter to be used for entering a value for the variable (ZZ). The parameters will be analyzed based on the processing type:

    **Processing type Drilling:**
    *   00 = X value hole 1
    *   01 = Y value hole 1
    *   02 = diameter hole 1
    *   03 = X value hole 2
    *   04 = Y value hole 2
    *   05 = diameter hole 2
    *   06 = X value hole 3
    *   07 = Y value hole 3
    *   08 = diameter hole 3
    *   09 = X value hole 4
    *   10 = Y value hole 4
    *   11 = diameter hole 4

    You can allocate the sizes of four holes as A+W Business allows to position four holes with identical diameter for the processing step Drilling.

    **Processing type Notch:**
    *   00 - 07 = Edge number
    *   08 = Width of notch
    *   09 = Height of notch
    *   18 = Distance of the notch

    **Example**
    Variable name: `__9610_03_02`
    *   **9610** could e.g. be the processing step Drilling.
    *   **03** is the third processing Drilling for glass.
    *   **02** is the diameter of the (first) hole of the third processing step Drilling.

6.  Save the SN file and use it like other template files.

> **SN file can be created without sketch view!**
> If the SN template includes only automatic variables apart from the supplementary shape sizes, you can dimension the entire contour with A+W Business and save it without accessing the sketch view (in A+W Business). If the template includes other variables, you have to complete the variables in the sketch view.
>
> In sn.ini you can define if the name of the automatic variable shall appear in the sketch view.

## Interaction with A+W Production

The link between A+W CAD Designer (Shapes) and A+W Production is mainly used to create the machinery codes via A+W CAD Designer (Shapes) and to create the graphics to be displayed at different terminals.

The following graphic shows a couple of examples of how A+W Production uses A+W CAD Designer (Shapes) functions:

**Fig. A-242 CAD Designer – Interaction with A+W Production**
*(A flowchart shows A+W Production importing items via an SN file into CAD Designer. CAD Designer then produces a Drawing, a BLOCK.IND file, and a CNC code. The CNC code is sent to CNC machines.)*

A+W Production loads A+W CAD Designer (Shapes) in the background and creates the necessary CNC or CAMDXF code.

If you import items with an attached SN file, A+W CAD Designer (Shapes) will be started in the background; the system checks if the articles and processing steps in the SN file match the A+W Production BOM.

### Via CNC files

CNC is a standard export/import format to control CNC machines. A+W CAD Designer (Shapes) can export data to this format. Some CNC machines will understand more CNC commands than defined in the standard. A+W CAD Designer (Shapes) therefore offers various options for creating CNC codes:

*   Standard CNC code can be created via File > Export > CNC.
*   To create machine-specific CNC codes, you have to install the corresponding driver first. When you have installed the driver, A+W CAD Designer (Shapes) will create the specific CNC code in menu Machine > Export to...

> **Specific drivers for machines are necessary!**
> For information on the available drivers and the corresponding A+W CAD Designer (Shapes) configuration, please contact A+W.
>
> When you install machine drivers, you define the view from which the geometry shall be exported. This makes sure that the grinding machine will be supplied with data from the Grinding view, and the drill from the Drilling view.

### Via DXF files

Everyone working with CAD and sketching programs, will know DXF as the standard export / import format that allows to exchange CAD files between different application programs. The DXF file contains the graphic-geometrical data of the sketched objects in an internationally applied code. This information can be read by every CAD program.

Because of its CAM elements, A+W CAD Designer (Shapes) has to be able to recognize and manage contour connections. Unlike for conventional CAD systems, segment relations are important. It is not enough for A+W CAD Designer (Shapes) to manage a collection of individual segments; these segments have to form a coherent contour.

**Standard DXF**

The DXF format contains geometrical data, i.e. it defines parameters such as contour and number of sketched elements, size, colour, line thickness, drilling positions, etc. A+W CAD Designer (Shapes) can read and process these DXF files and can also save contours in this format.

DXF files contain no information on machinery processes required to produce the sketched element. This includes the cutting path, the breakout sequence, and other information that can be entered and predefined in A+W CAD Designer (Shapes).

To make sure that DXF files can be read correctly by other CAD programs without much editing in A+W CAD Designer (Shapes), you have to obey some instructions. Example: only one line is usually drawn between two adjacent lites although A+W CAD Designer (Shapes) needs two segments to limit the lites. The end points of adjacent segments often do not match exactly. A+W CAD Designer (Shapes) will use so-called "catch areas" in this case. If segment ends are within the same catch area, A+W CAD Designer (Shapes) can link them automatically.

You should follow these guidelines when you create files in a CAD program and want to process the data in A+W CAD Designer (Shapes):

*   The contour to be imported should be complete and be the only one on a DXF layer. If several contours are imported from a DXF file, each of them should sit on a separate layer. Labelling, sizes, legends, etc. should be kept in separate layers.
*   The contour to be imported has to be closed. Open contours have to be edited in A+W CAD Designer (Shapes).
*   The contour to be imported should consist of ARC-, LINE- and CIRCLE entities. A+W CAD Designer (Shapes) can import POLYLINE entities to a certain extent; this is best avoided however. A+W CAD Designer (Shapes) will convert SOLID- and TRACE entities into several LINE entities to be able to import them. You should use CIRCLE entities only to define the position of drilled holes.
*   The DXF header will not be interpreted. DXF files become smaller if you omit the header. Importing into A+W CAD Designer (Shapes) only requires the SECTION ENTITIES. This means that ARC entities cannot be entered in clockwise order because this setting is defined by the variable $ANGDIR in SECTION HEADER.
*   INSERT entities will not be expanded. This means that the entire contour has to be defined in SECTION ENTITIES and cannot be constructed from blocks.
*   The separating points of adjacent segments of a contour should match.
*   If several contours have to be put into a layer, you should avoid branches. Otherwise, the wrong segments might be formed into a contour.

Basically, we recommend that the supplier of the DXF files should adapt his file for the import into A+W CAD Designer (Shapes) using the above guidelines.

For the operator of a CNC machine, receiving the DXF file means only the start of his actual work. The operator has to convert all the details of the DXF file required for the processing on hand in a predefined process. He must define the tools to be used as well as all processing parameters. This is how the processing (CAM) program is created, to be transferred to the machine.

A+W CAD Designer (Shapes) offers an extended DXF, CAMDXF. This format includes the machinery control information. The CAMDXF format offers the following advantages:

*   Controlling the machines with the processing data becomes faster, more elegant, and safer.
*   Apart from the geometrical data, CAMDXF includes the information for several machines in the processing chain.
*   The format can be used to control machines of the manufacturers Z. Bavelloni, Intermac, and Forvet.
*   The processing machines „understand“ the information provided by the CAM-DXF files without further programming.
*   The information includes all details such as the necessary tools and settings, reference points for positioning the suckers, etc.
*   CAMDXF can be supported by all machinery manufacturers.

It does not replace the CAD/CAM program at the machine, however. This is still required to process the CAM-DXF files.

The CAMDXF file can be created in A+W CAD Designer (Shapes) and can be directly sent to production scheduling or to the producer's IT system. No tedious training of machine operators is required. Through times are reduced and potential sources for errors are eliminated.

To write this format by A+W CAD Designer (Shapes) you have to install the corresponding machine driver. The export function is available in menu Machine.

The CAMDXF export is available from A+W CAD Designer (Shapes) version 5.02 and can only be accessed via view Edge processing.

### Via CAMXML files

CAMXML is an xml-based format.

Parts of a product (e.g. toughened lites for IG or for laminated glass units) are often purchased. The complete product structure is defined in A+W CAD Designer (Shapes) but - for obvious reasons - cannot or must not be passed on to the supplier.

With the function CAMXML, A+W CAD Designer (Shapes) allows to export data of individual BOM elements. These exported elements are fully described and can be imported by the recipient as a new product into another A+W CAD Designer (Shapes) installation. The function is available starting in A+W CAD Designer (Shapes) version 5.02.

### Data export

Data of contours and processing steps defined in A+W CAD Designer (Shapes) can be exported to many data formats. There are the following options:

*   Export data to a standard format
*   Export data to a special machinery format
*   Exporting part of a BOM

For a short description of the data formats, please see:
⇨ Software Reference, "Save file in (export)" on page A-171
⇨ "Via CNC files" on page A-503
⇨ "Via DXF files" on page A-504
⇨ “Via CAMXML files" on page A-506

**Export data to a standard format**

1.  Save the processing status of the SN file you want to export. Enter a suitable file name if necessary.
2.  Go to the view the display of which shall be exported.
3.  Open menu File > Export. A+W CAD Designer (Shapes) shows several valid standard export formats.
4.  Select the format in which the data shall be saved. A+W CAD Designer (Shapes) shows the dialog Save as.
5.  Select the required storing place and enter a file name.
6.  Confirm your entries by <OK>. A+W CAD Designer (Shapes) saves the data in the defined format with the corresponding suffix.

> **Additional information**
> ⇨ Software Reference, "Save file in (export)" on page A-171

**Export data to a special machinery format**
A+W CAD Designer (Shapes) can create CNC machinery control code.

> **SN can handle special machinery formats only if they have been installed!**
> To be able to create specific machinery code, first install the corresponding machine driver and configure A+W CAD Designer (Shapes) accordingly. If you need support, please contact A+W.

1.  Save the processing status of the SN file you want to export. Enter a suitable file name if necessary.
2.  Open menu File. A+W CAD Designer (Shapes) shows all installed machines for which data can be exported.
3.  Select the machine for which data shall be created. A+W CAD Designer (Shapes) shows further options.
4.  Select the data format (e.g. NC code) to load the data export. A+W CAD Designer (Shapes) saves the data in the place you have defined when installing the machine driver.
5.  Confirm your entry by [OK]. A+W CAD Designer (Shapes) saves the data in the defined format with the corresponding suffix.
    A+W CAD Designer (Shapes) exports the data from the view defined for the selected machine.

**Exporting part of a BOM**
A+W CAD Designer (Shapes) provides the data exchange format CAMXML. This allows to save complete SN files as well as only parts of a unit and transfer it e.g. to a supplier.

1.  Save the processing status of the SN file you want to export. Enter a suitable file name if necessary.
2.  Go to view Edgework. Only from there can you export to the CAMXML format. If you start this function in another view, A+W CAD Designer (Shapes) will switch to the right view.
3.  Click on the level part of which you want to export. Select Level 0 to export the entire product structure.
4.  Click on a segment of the contour to be exported. A+W CAD Designer (Shapes) will export the tagged element with all the levels below.
5.  Select menu File > Export > CAMXML. A+W CAD Designer (Shapes) shows the dialog Save as.
6.  Select the required storing place and enter a file name.
7.  Confirm your entry by [OK]. A+W CAD Designer (Shapes) will save the selected element in the defined file with the suffix .xml. The saved file can be opened in any A+W CAD Designer (Shapes) version from 5.02 upwards, to be processed as a common SN file. To check the information included in the CAMXML file, open the file via A+W CAD Designer (Shapes).

> **Additional information**
> ⇨ Software Reference, "Save file in (export)" on page A-171

## Change display of the drawing

Use menu View to define the way in which A+W CAD Designer (Shapes) shall display the drawing and sizes in the different views. These settings will change the display of the drawing, its background or sizes. Basic settings which do not change during program operation, are fixed in the configuration file sn.ini.

You can use the following functions to change the display of the drawing on screen:

*   Select measure
*   Extend display

Apart from that, there is a Segment input for experts which shall be explained below.

### Select measure

You can work in millimeter (mm) or Inch. For the latter, you can choose decimals or fractions.

1.  Open the menu View.
2.  In sub-menu Settings, click on Sizes. This gives you the following options:
    *   Enter sizes in mm
    *   Enter sizes in inch (fractions)
    *   Enter sizes in inch (decimals)
    *   Mixed sizes

    The three top options define the measure in which numbers are entered: millimeter, inch (fractions, or inch (decimals). The measure of the ruler at the edge of the drawing board changes depending on your choice.

    If you enter just one number for a size (without mm or "), the measure for this number is defined by this option. Alternatively, you can directly enter the required measure (e.g. 12 mm or 25" 1/32). The input will be converted to the set measure. Click on mixed sizes to show all sizes with their original measure.

> **Define one measure!**
> For reasons of clarity, you should choose one measure before you start the dimensioning. You can of course dimension different parts of a sketch in different measures. In this case, you should activate mixed measures as the figures will be shown together with the measures (if this function is disabled, all sizes will be shown without measures).

3.  Choose one of the displayed optional measures to activate it. A+W CAD Designer (Shapes) now closes the menu. Next time you open the menu, the selected option will be ticked.

### Extend display

In addition to the sketch, you can display the following elements in certain views:
*   "Show critical points" on page A-510
*   "Show measuring points" on page A-511

### Show critical points

This setting allows to show (too) pointed angles between segments, (too) short segments, and (too) small inside radii of a contour. The ticked setting is valid.

1.  Open the menu View.
2.  In sub-menu Settings click on Show critical points. This offers the following options:
    *   **Mark critical segments in geometry and revision.**
        Critical segments will be shown only in the views Geometry and Revision.
    *   **Mark critical segments in every view.**
        Critical segments will be shown in every view.
    *   **Do not mark critical segments.**
        Critical segments will not be shown.
3.  Choose one of the displayed options to activate it. A+W CAD Designer (Shapes) now closes the menu. Next time you open the menu, the selected option will be ticked.

The file sn.ini defines the point from which on an angle is considered too pointed, or a segment or radius is considered too small. Section User in this file contains four entries which control the display of critical segments:

*   **MarkInsideRadiusBelow**
    This parameter defines up to which radius arc segments have to marked as critical (the entire segment will be shown in a special colour in this case).
*   **MarkOutsideAngleAbove**
    This parameter defines the point from which on the external transition angle (outward bend) between segments has to be marked as critical. This is marked by a small arrow pointing at the corresponding spot.
*   **MarkInsideAngleAbove**
    This parameter defines the point from which on the inside transition angle (inward bend) between segments becomes critical. This is marked by a small arrow pointing at the corresponding spot.
*   **MarkShortSegmentBelow**
    This parameter defines the maximum length up to which a segment has to marked as too short (the entire segment appears in a special colour).

### Show measuring points

This setting allows to restrict the display of measuring points to certain views. Measuring points can be entered in view Points by means of an appropriate digitizing tool.

These points serve as reference points for the original contour. We do not recommend to change the position of a reference point afterwards. Measuring points can be deleted from any view in which they are visible.

1.  Open the menu View.
2.  Click in sub-menu Settings on Show measuring points. This offers the following options:
    *   **Show measuring points only in view Points:**
        Measuring points will be displayed only in view Points.
    *   **Show measuring points in several views:**
        Measuring points will be shown in the views Points, Geometry, and Revision. The last view in which measuring points shall be shown, can be set in the configuration file sn.ini ([View] LastViewToDrawCheckpoints=, default is Revision).
    *   **Show measuring points in all views:**
        Measuring points will appear in all views.

### Show grid

This function allows to show raster points in the drawing. Depending on the display size, raster points are shown per millimeter, centimeter, decimeter, or meter.

1.  Open the menu View.
2.  Click in sub-menu Settings on Show raster. The raster is now active. A+W CAD Designer (Shapes) now closes the menu. Next time you open the menu, the selected option will be ticked.
    To switch off the raster, deselect the option.

### Background image (opacity)

This function allows you to set the visibility and opacity of the background image.

1.  Open the menu View.
2.  In sub-menu Settings, click on Background image and then on Opacity.
3.  Select the required opacity.

### Segment input for experts

This function allows to change the input window for segment input (manual input of straight and arc segments).
⇨ Tutorial, "Input window (D)" on page A-25

**Enter segments**

1.  Enable Segment input for experts by selecting it in menu View > Settings. A+W CAD Designer (Shapes) will tick the entry to show that the function is active.
2.  Enter segments by defining relative distances, length, angles, etc. Delete the input fields for unknown quantities (there must be no blank). Proceed as follows:
    *   **Straight segment (type 1):**
        Leave the fields for X2 and Y2 blank an enter for dx and dy the relative distance from the segment's start point. Alternatively you can enter X2, leave Y2 blank, and enter dy. A+W CAD Designer (Shapes) will calculate the line the end point of which has the x coordinate X2 and the Y coordinate Y1+dy.
    *   **Length and angles:**
        You can combine entries when defining length and angles. If you enter dx and dis for instance, A+W CAD Designer (Shapes) will calculate the end point with a horizontal distance dx from the start point, the length of the constructed segment being dis.
        When you enter angles, you can use <1 to define the angle towards the previous segment or _<_ for the angle to the horizontal axis, both in degrees and mathematically positive orientation (clockwise being negative, anti-clockwise positive).
    *   **Arcs:**
        The above instructions can be applied to arcs as well. First, define the end point of the arc. After that, you can enter the radius r, the height of the arc h or the length of the arc l to describe the arc.
3.  Confirm your entry by [OK].

## Help Cards

### This chapter provides information on:

*   Information on Help Cards
*   Creating geometries
*   Processings
*   Shape with bulge and edge cut-out

| Topic | Page |
| :--- | :--- |
| Information on Help Cards | A-515 |
| **Creating geometries** | **A-516** |
| Rectangle with cut-off corner | A-517 |
| Creating an arrow | A-518 |
| Modified parallelogram | A-519 |
| Rectangle slanted edge round corner | A-520 |
| Creating, dimensioning & saving shape | A-521 |
| Creating and saving a trapezoid | A-522 |
| Creating and mirroring a shape | A-523 |
| Creating and mirroring a shape | A-524 |
| **Processings** | **A-525** |
| Shape with missing corner and cut-out | A-526 |
| Shape with round corner and cut-out | A-527 |
| Rectangle with arc | A-528 |
| Shape with bulge and edge cut-out | A-529 |
| **Macros and templates** | **A-530** |
| Creating a symmetrical macro | A-531 |
| Creating a non-symmetrical macro | A-532 |
| Creating a template | A-533 |
| Inserting macro into template | A-534 |
| Parametric macro | A-535 |

### Information on Help Cards

The depictions in the Help Cards are based on the delivery version A+W CAD Designer (Shapes) 2014. Individual steps in the workflows may deviate depending on the configuration.

## Creating geometries

| Help Card | Topics |
| :--- | :--- |
| Rectangle with cut-off corner | Create and dimension a rectangle with cut-off corner. |
| Creating an arrow | Create and dimension the shape of an arrow |
| Modified parallelogram | Create and dimension the shape of a modified parallelogram. |
| Rectangle slanted edge round corner | Create and dimension the shape of a rectangle with a slanted edge and a round corner. |
| Creating, dimensioning & saving shape | Create, dimension, and save a rectangle with arc on top. |
| Creating and saving a trapezoid | Create, dimension, and save a trapezoid. |
| Creating and mirroring a shape | Create and mirror a shape halfway. |
| Creating and mirroring a shape | Create and mirror a shape halfway. |

### Help Card: Rectangle with cut-off corner (Shp 01-001)

**Goal of the action**
Create and dimension a rectangle with cut-off corner.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch the shape in the sketch view.
2.  Dimension the straight lines.
3.  Define the right angle. The symbol appears in the corner.
4.  For the corner cut-outs, select the tool for dimensioning the distance between a point and a line.
5.  With the Draw new function (View > Draw new or <Ctrl>+<D>), A+W CAD Designer (Shapes) checks whether or not the shape can be calculated.

### Help Card: Creating an arrow (Shp 01-002)

**Goal of the action**
Create and dimension the shape of an arrow.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch the shape in the sketch view.
2.  Dimension the individual straight lines.
3.  Define the right angle.
4.  Select the tool for dimensioning the interior angle between two segments.
5.  Let A+W CAD Designer (Shapes) recalculate the shape.

### Help Card: Modified parallelogram (Shp 01-003)

**Goal of the action**
Create and dimension the shape of a modified parallelogram.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch the shape in the sketch view.
2.  Dimension the individual straight lines.
3.  Select the tool for dimensioning the distance between two points parallel to a line.
    Mark the left point of the top straight line. This is displayed in red. Mark the bottom point of the left slope. This is displayed in green. Mark the bottom straight line. It is displayed in gray. A value window opens. Enter a length of 2099 for P= in the input window. A value window opens. Click the [OK] button.
4.  To dimension the right slant, select the tool for dimensioning the distance between a point and a straight line.
5.  Select the tool for dimensioning the interior angle between two segments.
6.  Let A+W CAD Designer (Shapes) recalculate the shape.

### Help Card: Rectangle slanted edge round corner (Shp 01-004)

**Goal of the action**
Create and dimension the shape of a rectangle with a slanted edge and a round corner.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch the shape in the sketch view.
2.  Dimension the individual straight lines.
3.  Dimension the slant.
4.  Select the tool in order to dimension the radius of an arc.
    Mark the arc. A value window opens. Enter a radius of 200 for R= in the input field. Click the [OK] button.
5.  Then select the tool to smooth out the arc segments.
    Mark the arc. This will be shown in red. Mark the left straight line. This will be colored green. Click the [OK] button. The segment will be connected smoothly. Repeat the procedure with the top straight line.
6.  Select the tool in order to specify a right angle (on both sides) between two straight segments.
7.  Let A+W CAD Designer (Shapes) recalculate the shape.

### Help Card: Creating, dimensioning & saving shape (Shp 01-005)

**Goal of the action**
Create, dimension, and save a rectangle with arc on top.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.
*   Study the Rectangle slanted edge round corner HelpCard.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch the shape with straight line and arc.
2.  Dimension the distance of the straight lines and of the arc.
3.  Connect all arc segments smoothly.
4.  Dimension the two vertical segments to one another.
5.  Change to the Final product view in order to check the result.
6.  From the File menu, select the Save as... menu element. The Global shape data dialog opens.
7.  Fill out the Name and Text fields.
8.  Close the dialog with the [OK] button. The Save as... dialog opens.
9.  Enter a file name and click the [Save] button.

### Help Card: Creating and saving a trapezoid (Shp 01-006)

**Goal of the action**
Create, dimension, and save a trapezoid.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.
*   Study the Creating, dimensioning & saving shape HelpCard.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch a trapezoid.
2.  Dimension the shape according to the task.
3.  Connect all arc segments smoothly.
4.  Save the shape as a file.

### Help Card: Creating and mirroring a shape (Shp 01-007)

**Goal of the action**
Create half of the adjacent shape and then mirror it.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.
*   Study the Rectangle slanted edge round corner HelpCard.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch the left half of the shape with straight line and arc.
2.  Dimension the bottom straight line with the value 75.
3.  Dimension the arc with the value 75.
4.  Connect the arc segments smoothly.
5.  Select the tool for dimensioning two segments parallel to one another.
    Mark the top straight line. This will be colored red. Mark the bottom straight line. This will be colored green. Click the [OK] button. The symbol = will appear below the top straight line.
6.  Dimension the two vertical segments to one another.
7.  Change to the Geometry view.
8.  Select the tool for doubling a shape by mirroring one segment.
    Mark the vertical straight line where the mirroring should be done. This will be colored red.
9.  Click the [OK] button. The contour is mirrored.

### Help Card: Creating and mirroring a shape (Shp 01-008)

**Goal of the action**
Create half of the adjacent shape and then mirror it.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.
*   Study the Rectangle slanted edge round corner HelpCard.
*   Study the Creating and mirroring a shape HelpCard.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch the left half of the shape with straight line and 3 arcs.
2.  Dimension the bottom straight line with the value 18.
3.  Dimension the bottom straight line with the value 30.
4.  Dimension the top straight line with the value 6.
5.  Dimension the three arcs with the value 75.
6.  Dimension the rest according to the adjacent values.
7.  Set three right angles.
8.  Connect both arc segments smoothly.
9.  Change to the Geometry view.
10. Select the tool for doubling a shape by mirroring one segment.
    Mark the vertical straight line where the mirroring should be done. This will be colored red.
11. Click the [OK] button. The contour is mirrored.

## Processings

| Help Card | Topics |
| :--- | :--- |
| Shape with missing corner and cut-out | Create a rectangle with cut-off corner and cut-out. |
| Shape with round corner and cut-out | Create a rectangle with rounded-off corners and edge cut-out. |
| Rectangle with arc | Create a rectangle with an arc on top. |
| Shape with bulge and edge cut-out | Create a shape with a bulge and two edge cut-outs. |

### Help Card: Shape with missing corner and cut-out (Shp 02-001)

**Goal of the action**
Create a rectangle with cut-off corner and cut-out.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.
*   Study the Rectangle slanted edge round corner HelpCard.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch and dimension a rectangle with a slanted corner.
2.  Change to the Inner contours view. From the File menu, select the Insert menu element. Select the file for the Shp 01-005 exercise that you saved. Click the [OK] button. The shape is placed.
3.  Select the tool for positioning cut-outs. In the inserted shape, mark the bottom horizontal straight line near the segment end point (red with small arrow in direction End). Now on the sketched rectangle, mark the top area of the right straight lines (green). Enter 200 for D2= in the input field. Click the [OK] button. Under D1 the value 0 remains since D1 is the parallel distance to the cut-out bottom edge and these should be one atop the other. The inserted file is placed in the shape of an inner cut-out.
4.  Select the tool for creating a drill hole with dimensioning. Mark the left straight line (red). Mark the bottom straight line (green). Enter a distance of 852 for D1= in the input field, 102 for D2= and a diameter of 34 for o=. Click the [OK] button. The drill hole is placed.
5.  For the next drill hole, mark the left straight line (red) again. Mark the bottom straight line (green). Enter a distance of 552 for D1= in the input field, 102 for D2= and a diameter of 34 for o=. Click the [OK] button. The drill hole is placed.
6.  Select the tool for creating a drill hole manually. Place the drill hole in the desired location.
7.  Select the tool for dimensioning. Dimension the drill hole.
8.  Select the tool for dimensioning two points parallel to a line. Mark the left drill hole (red). Mark the middle drill hole (green). Mark the bottom straight line (gray) and in the value window, enter D=150. Mark the left point of the slant and then the top horizontal straight line and enter D=450 in the value window.
9.  Check the result.

### Help Card: Shape with round corner and cut-out (Shp 02-002)

**Goal of the action**
Create a rectangle with rounded-off corners and edge cut-out.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.
*   Study the Rectangle slanted edge round corner Help-Card.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch and dimension a pentagon.
2.  Change to the Geometry view. Round off both corner points with the radius of 75.
3.  Change to the Sketch view. From the File menu, select the Insert menu element. Select the file for the Shp 01-006 exercise that you saved. Click the [OK] button. The shape is placed.
4.  Change to the Geometry view. In the shape you just placed, dimension the two upper arcs with the radius of 25 apiece.
5.  Change to the Inner contours view.
6.  Select the tool for positioning cut-outs. In the inserted shape, mark the bottom horizontal straight line near the segment start point (red with small arrow in direction Start). Now in the sketched pentagon, mark the bottom horizontal straight lines near the segment start point (green with small arrow in direction Start). In the value window under D1 and D2 enter the appropriate distances. Under R1 and R2 you can enter the radii of 25, so that the corners are rounded. Click the [OK] button. The shape is placed as inner contour.
7.  Change to the Geometry view. Select the tool for cutting an edge with different distances. Mark the start point and make the appropriate entries. Repeat the procedure with the bottom right corner.
8.  Select the tool for rounding corners. Dimension the still-missing arcs.
9.  Check the result.

### Help Card: Rectangle with arc (Shp 02-003)

**Goal of the action**
Create a rectangle with an arc on top.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.
*   Study the Rectangle slanted edge round corner Help-Card.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch half of the shape.
2.  Dimension the shape.
3.  Change to the Geometry view.
4.  Double the shape.
5.  Change to the Inner contours view.
6.  Check the result.
7.  Save the shape.

### Help Card: Shape with bulge and edge cut-out (Shp 02-004)

**Goal of the action**
Create a shape with a bulge and two edge cut-outs.

**Requirements**
*   Study the Rectangle with cut-off corner HelpCard.
*   Study the Creating an arrow HelpCard.
*   Study the Modified parallelogram HelpCard.
*   Study the Rectangle slanted edge round corner Help-Card.

**Additional info**
To create and dimension the shape shown, the following tools are required.

**Workflow**
1.  Sketch and dimension the shape.
2.  From the File menu, select the Insert menu element. Select the file for the Shp 02-003 exercise that you saved. Click the [OK] button. The shape is placed.
3.  Change to the Inner contours view. Select the tool for positioning cut-outs. If necessary, enlarge the view.
4.  In the inserted shape, mark the bottom horizontal straight line near the segment start point (red with small arrow in direction Start).
5.  Now in the sketched shape, mark the right straight lines near the segment start point (green with small arrow in direction Start). A value window opens. Under D1 enter the value 0 and D2 the value 205. R1 and R2 remain blank. Click the [OK] button. The shape is placed as inner contour.
6.  From the File menu, select the Insert menu element. Select the file for the Shp 02-003 exercise that you saved. Click the [OK] button. The shape is placed.
7.  Change to the Inner contours view. Repeat the steps 3, 4, and 5. Make sure the dimensions are correct.
8.  Check the result.

## Macros and templates

| Help Card | Topics |
| :--- | :--- |
| Creating a symmetrical macro | Create and save symmetrical edge cut-out macro. |
| Creating a non-symmetrical macro | Create and save non-symmetrical edge cut-out macro. |
| Creating a template | Create and save door template. |
| Inserting macro into template | Insert symmetrical macro. |
| Parametric macro | Create parametric macro. |

### Help Card: Creating a symmetrical macro (Shp 03-001)

**Goal of the action**
Create and save symmetrical edge cut-out macro.

**Requirements**
*   You know how a shape is drawn and dimensioned.
*   You know how processing are placed and dimensioned.

**Workflow**
1.  Drawing and dimensioning of the shape in the Sketch view.
2.  Place two drill holes in the Inner contours view with appropriate values.
3.  Group shape: mark both drill holes and a segment of the shape. Group the shape with Transform > Group. In order to make the grouping visible, enter 10 mm in the value window under <=, >=, ^=, and v=. A circumscribing rectangle is placed. The arrow that is visible on the bottom side of the circumscribing rectangle marks the reference point and the reference side.
4.  Place the reference point so that it is in the middle of one side and not in one corner. To do this, select the Halve segment tool, click the left side of the grouping rectangle, and click [OK]. After that, the segment is divided into two parts of equal length. Repeat the procedure for the right side.
5.  Then connect the two points with one another using a help line (tool: New help line).
6.  Activate the Set reference segment tool and click the top half of the segment near the halving point on the left side of the grouping rectangle. The segment will be colored red and has an arrow in the direction of the halving point. If you click [OK], the new reference segment is placed.
7.  In the next step, adjust the grouping rectangle to the shape again. To do this, mark any line in the grouping rectangle and change the values <=, >=, ^=, and v= from 10 mm to 0 mm in the value window. The reference point and the reference segment serve the later recording and dimensioning in the ERP system.
8.  Save the file under File > Save as... The Global shape data dialog opens. Please do not use any umlauts or blank spaces.

### Help Card: Creating a non-symmetrical macro (Shp 03-002)

**Goal of the action**
Create and save non-symmetrical edge cut-out macro.

**Requirements**
*   You know how a shape is drawn and dimensioned.
*   You know how processing are placed and dimensioned.

**Workflow**
1.  Drawing and dimensioning of the shape in the Sketch view.
2.  Place two drill holes in the Inner contours view with appropriate values.
3.  Group shape: mark drill hole and a segment of the shape. Group the shape with Transform > Group. In order to make the grouping visible, enter 10 mm in the value window under <=, >=, ^=, and v=. A circumscribing rectangle is placed. The arrow that is visible on the bottom side of the circumscribing rectangle marks the reference point and the reference side.
4.  Shift the reference point so that it is at the lower left in the corner. To do this, activate the Set reference segment tool and click the lower right corner of the grouping rectangle. The segment is colored red and it has an arrow in the direction of the corner point. If you click [OK], the new reference segment is placed.
5.  In the next step, adjust the grouping rectangle to the shape again. To do this, mark any line in the grouping rectangle and change the values <=, >=, ^=, and v= from 10 mm to 0 mm in the value window. The reference point and the reference segment serve the later recording and dimensioning in the ERP system.
6.  Save the file under File > Save as... The Global shape data dialog opens. Please do not use any umlauts or blank spaces.

### Help Card: Creating a template (Shp 03-003)

**Goal of the action**
Create and save door template.

**Requirements**
*   You know how a shape is drawn and dimensioned.
*   You know how processing are placed and dimensioned.

**Workflow**
1.  Drawing and dimensioning of the shape in the Sketch view.
2.  Place two drill holes (for edge hanging) in the Inner contours view with the following values.
    *   Distance from top and bottom edge: DrillHole-Height=150
    *   Distance from the left edge: 100
3.  Place a drill hole (for door handle) with the following values.
    *   Distance from the right edge: 100
    *   Distance from the lower edge: DoorHandle-Height=1000
4.  Seam all edges in the Edge processing view.
5.  In the Cutting (individual) view, remove all broken edges since these are stored in the master data in the production planning system. For this, click the dotted line, click the closed fist symbol on the values window. The fist opens into a hand. Then you can set the values in the ranges <=, >=, ^=, and v= to 0.
6.  Save the file under File > Save as... The Global shape data dialog opens. Names for template files must begin with T_ (for example, T_Tuer). Please do not use any umlauts or blank spaces. Save the file in the Templates folder, otherwise it will not be recognized as such!

### Help Card: Inserting macro into template (Shp 03-004)

**Goal of the action**
Insert symmetrical macro.

**Requirements**
*   You know how a shape is drawn and dimensioned.
*   A symmetrical edge cut-out macro is present.

**Workflow**
1.  Drawing and dimensioning of the shape in the Sketch view.
2.  Place the Symmetrical edge cut-out macro twice for the door attachment (File > Insert). Once for the upper door attachment and once for the lower.
3.  Change to the Inner contours view in order to place the edge cut-outs. Mark a segment of the edge cut-out, use Transform > Shift to position one edge cut-out top left and the other edge cut-out lower left. With respect to the subsequent dimensioning, it is recommended that you place the edge cut-outs to the left outside the shape and not inside it where they actually belong!
4.  To place the edge cut-outs, the Insert cut-out in shape tool is activated. Place the bottom edge cut-out by clicking the reference segment of the edge cut-out (arrow will be colored red) and the left edge of the door in the bottom area (arrow will be colored green). In the values window, enter the value 0 for D1 (horizontal) and the value 100 for D2 (vertical). Repeat this procedure for the top edge cut-out.
5.  Place a drill hole for the door handle.
6.  Seam all edges.
7.  Remove the broken edges.
8.  Save the file under File > Save as... The Global shape data dialog opens. Names for template files must begin with T_ (for example, T_DoorEdgeCutOut). Please do not use any umlauts or blank spaces. Save the file in the Templates folder, otherwise it will not be recognized as such!

### Help Card: Parametric macro (Shp 03-005)

**Goal of the action**
Create parametric macro.

**Requirements**
*   A+W CAD Designer (Shapes) Version 5.5 or higher.
*   You know how to group a form and relocate the reference point.

**Additional info**
*   Internal variables begin with an underscore, e.g. _D and serve to calculate the shape.
*   Restrictions begin with _TEST and serve to describe limits.

**Workflow**
1.  Drawing of the shape in the Sketch view.
2.  The dimensions are as follows:
    *   Height: H=100, Width: B=50, Chord: H=100 and Arc height: B/2
3.  Place two drill holes in the Inner contours view with the following values.
    *   Diameter: R=20
4.  To ensure that the drill hole edge is always at the height of the cord edge, a variable is recorded for this value. From the Edit menu, open the Edit variables entry. The Edit variables dialog opens. For this shape there are already three entries on the dialog (H, W and R). Click [New], then go to the next free line and enter _D in the Names area. Enter B/2+R/2 in the Output area. The area value is filled automatically after you have clicked [Apply]. For our example, this means that:
    *   Arc height = 50, B/2 = 25
    *   Radius = 20, R/2 = 10
    *   25 + 10 = 35.
    Activate the Parallel distance tool and specify_D for P=. Repeat the procedure for the second drill hole.
5.  In addition, we want to ensure that the height is always twice the width. The corresponding description is: height minus twice the width is equal to zero. To depict this, the formula is: H-2*W. Click [New] again. Since this is a restriction, in the Names area enter_TEST and in the Output area H-2*W. Since H=100 and B=50, the entry in the Value field is 0. Close the dialog.
6.  Group the shape. The value fix may not be active!
7.  Relocate the reference point as in the graphic.
8.  Adjust the grouping rectangle to the shape again.
9.  Save the file.

## Index

### A
*   **A+W Business**
    *   Interplay with TOP A-495
*   **A+W Enterprise**
    *   Interplay with TOP A-483
*   **A+W Production with CAD Designer** A-503
*   **Add auxiliary line** A-301
*   **Add Planar fixings** A-398
*   **Add roundings to a macro** A-320
*   **Adding a radius** A-454
*   **Adjust** A-429
*   **ALCIB**
    *   Link with Shaping&Nesting via AWBroke A-483
*   **ALFAK**
    *   Shape input A-496
*   **Align a contour** A-365
*   **Align laminated and IG lites** A-479
*   **Align lites** A-479
*   **Angle**
    *   dimension A-268
*   **Angle of an arc**
    *   dimension A-268
*   **Arc**
    *   dimension A-275
    *   dimension angle A-268
    *   Dimension height A-281
    *   dimension length A-286
    *   dimension secant length A-284
    *   enter A-231
    *   optimum A-225
*   **Arched notch**
    *   as BOM element A-333
    *   blend with contour A-334
*   **Architectural glass**
    *   process A-479
    *   Tools A-392
*   **Arrissing laminated** A-415
*   **Arrow** A-421
*   **Automatic dimensioning** A-288
*   **Auxiliary Cut** A-350
*   **AWBroke** A-483

### B
*   **Back cut** A-396
*   **Background image** A-512
*   **Bando cutting/grinding machine, Define starting point** A-376
*   **Basics**
    *   breakout A-35
    *   cutting A-34
    *   Edgework A-33, A-37
    *   Inside contour A-33
    *   Operation of Shaping&Nesting A-419
    *   Production process A-36
    *   Revision A-32
    *   unit A-35
*   **Bevel** A-409
*   **Block grinding of laminated edge** A-413
*   **BOM** A-480
    *   arched notch A-333
    *   cut-off corner A-310
    *   cut-out corner A-330
    *   notch A-329
    *   rounded corner A-316
*   **Breakout**
    *   basics A-35

### C
*   **CAD Designer**
    *   with A+W Production A-503
*   **CAMDXF** A-505
*   **CAMXML** A-506
*   **Catalog shape**
    *   enter via crosshairs A-221
    *   enter via measuring wheel A-220
*   **Change measure** A-509
*   **Changing a contour** A-241
*   **Close**
    *   contour A-247
    *   cut-out A-248
    *   gap A-248
*   **Close gap** A-248
*   **CNC** A-503
*   **Contour** A-18
    *   adjust A-194, A-431
    *   align A-365
    *   align with segment A-367
    *   change A-241
    *   close A-247, A-437
    *   complete A-435
    *   correct A-179
    *   create complex contour A-464
    *   create parts of A-465
    *   define direction A-373, A-378
    *   digitize A-217, A-438
    *   digitizing A-214
    *   distort A-393
    *   duplicate A-369
    *   edit A-444, A-476
    *   enter A-217, A-435
    *   export A-424
    *   flip horizontally A-194
    *   flip vertically A-194
    *   freeze A-195
    *   grouping A-194, A-195
    *   import A-228, A-424, A-435
    *   move A-193, A-243, A-429
    *   multiple grinding A-378
    *   notch A-325
    *   open A-424
    *   position like other contour A-377
    *   positioning A-193
    *   reflect A-244, A-430, A-466
    *   reflect horizontally A-193
    *   reflect vertically A-194
    *   replace group A-194
    *   rotate A-193, A-429, A-454
    *   rotate by 90 A-193
    *   save A-424
    *   sketch A-449
    *   smooth A-233
    *   stop freezing A-195
    *   stretch A-194, A-431
    *   with BOM A-480
*   **Contours**
    *   link A-241, A-466
*   **Convert**
    *   drill hole A-296
*   **Convert drill hole to countersunk** A-296
*   **Copy**
    *   contour A-369
    *   segments and contours A-428
*   **Copying a contour** A-244
*   **Corner**
    *   cut off A-304
    *   process A-478
    *   round A-312
    *   sharpen A-312
*   **Corner bevelling** A-304
*   **Correct a contour** A-179
*   **Correct contour** A-179
*   **Create**
    *   complex contour A-464
    *   door A-460
    *   section A-457
    *   shape A-468
    *   Sketch A-229
    *   sketch A-481
*   **Create an Ellipse** A-245
*   **Create cutting pattern** A-394
*   **Create partial contour** A-465
*   **Critical point**
    *   show A-510
*   **Crucial point**
    *   correct A-445
*   **Cut off corner** A-304
*   **Cut-off corner as BOM element** A-310
*   **Cut-out**
    *   as separate file A-317
    *   close A-248
    *   cut A-317
*   **Cut-out corner**
    *   as a BOM element A-330
    *   blend with contour A-332
*   **Cut-out macro** A-317
*   **Cutting**
    *   basics A-34
*   **Cutting path** A-360
*   **Cutting table control** A-363

### D
*   **Data export** A-506
*   **Data formats** A-435
*   **Data transfer**
    *   via CAMDXF A-505
    *   via CAMXML A-506
    *   via CNC A-503
    *   via DXF A-504
*   **Define breakout path** A-380
*   **Define cutting path** A-380
*   **Define direction of a contour** A-373, A-378
*   **Define edgework** A-478
*   **Define master and slave starting points** A-374
*   **Define surrounding rectangle** A-363
*   **Define trim** A-476
*   **Define units (IG and laminated)** A-418
*   **Delete dimensions** A-321
*   **Delete segments and contours** A-428
*   **Delete shape** A-321
*   **Design printout** A-463, A-481
*   **Digital camera** A-443
*   **Digitize** A-438
    *   contour A-217
    *   hole via crosshairs A-224
    *   hole with points A-222
    *   measuring point A-222
    *   via digitizer A-438
*   **Digitizer** A-214, A-438
*   **Digitizing**
    *   Contour A-214
    *   virtual A-227, A-443
    *   with digital camera A-227, A-443
*   **Dimension**
    *   angle (tools) A-268
    *   arc height A-281
    *   automatic A-288
    *   circle and arc A-275
    *   counter-sunk hole A-296
    *   distance between point and line A-256
    *   distance between points A-254
    *   distance between points, parallel with a line A-254, A-257
    *   distance between points, vertical to a line A-258
    *   distance of end points A-253
    *   distance of peaks A-280
    *   hole A-290
    *   horizontal distance between two points A-263
    *   inside angle of two segments A-270
    *   inside segment angle A-270
    *   length of a line A-264
    *   radius A-284
    *   secant length of an arc A-284
    *   segment A-252
    *   sketch A-451, A-455
    *   two parallel segments A-273
    *   two segments vertical to another A-273
    *   vertical distance between two points A-262
*   **Dimension aperture of an arc** A-268
*   **Dimension arcs of the same radius** A-286
*   **Dimension circle** A-275
*   **Dimension counter-sunk hole** A-296
*   **Dimension end point with X and Y coordinates** A-266
*   **Dimension inside angle between segments** A-270
*   **Dimension peaks with a distance** A-280
*   **Dimension secant length of an arc** A-284
*   **Dimension smooth transition** A-286
*   **Dimensions**
    *   check A-196
*   **Distance between**
    *   center and peak of two circles A-280
    *   Center of arc and end point, parallel A-282
    *   centers of two arcs A-281
    *   end points A-253
    *   line and arc A-278
    *   line and center of arc A-277
    *   peaks A-280
    *   point and center of arc A-276
    *   point and intersection, horizontal A-260
    *   point and intersection, parallel with a line A-260
    *   point and intersection, vertical A-259
    *   point and intersection, vertical to a line A-263
    *   point and line A-256
    *   points A-254
    *   points, horizontal A-263
    *   points, parallel with a line A-254, A-257
    *   points, vertical A-262
    *   points, vertical to a line A-258
*   **Distance from cut-off corner** A-267
*   **Distorted sketch** A-396
*   **Distorting a contour** A-393
*   **Drawing** A-18
    *   hatch A-395
*   **Drilling**
    *   cut A-317
*   **Cutting pattern** A-394
*   **DXF file** A-504

### E
*   **Edge** A-406
    *   arrissing A-406
    *   define A-416
    *   fine-adjusted A-403
    *   Laminated arrissing A-415
    *   laminated with mitre A-414
    *   move A-242
    *   of IG and laminated A-410
    *   polish A-405
    *   process A-403
    *   roughly adjusted A-404
    *   with mitre A-407
*   **Edge deletion** A-372
*   **Edge stripping** A-372
*   **Edgework**
    *   Basics A-33, A-37
    *   define A-478
*   **Edit**
    *   contour A-476
*   **Edit digitized contour** A-444
*   **Elastic band** A-18
*   **End points, dimension distance** A-253
*   **Enlarge**
    *   a view A-419
*   **Enlarge or reduce view** A-419
*   **Enter**
    *   arc A-231
    *   arc (optimum) A-225
    *   contour A-217, A-435
    *   line A-230
    *   line (optimum) A-225
*   **Enter a door** A-457, A-460
*   **Enter counter-sunk depth** A-297
*   **Enter machine starting points** A-375
*   **Enter optimum arc** A-225
*   **Enter optimum line** A-225
*   **Equalizing arc** A-444
*   **Equalizing line** A-444
*   **Establish production conformity** A-245
*   **Export standard format** A-506
*   **Exporting a contour** A-506

### F
*   **Features** A-15
*   **File**
    *   Closing a file A-158
    *   Creating a new file A-158
    *   Exit A-159
    *   export A-424
    *   Exporting files A-158
    *   import A-424
    *   Importing a transfer file A-158
    *   Inserting a contour A-158
    *   move to origin A-193
    *   open A-424
    *   Opening a file A-158
    *   Preview A-159
    *   Previous file A-159
    *   print A-172
    *   Print file A-159
    *   Return to order processing A-158, A-159
    *   save A-424
    *   Saving a file A-158
    *   Saving a new file A-158
    *   Send Email A-159
    *   Set password A-158
    *   Set up printer A-159
*   **Fluted Bevelling**
    *   Enter A-347
*   **Form a group** A-432
*   **Formatting a segment** A-395
*   **Free Shape**
    *   Edge shift A-396
*   **Functional principle**
    *   Tools A-249

### H
*   **Hatch surface** A-395
*   **Hatching a surface** A-395
*   **Hole**
    *   digitize via crosshairs A-224
    *   digitize with point A-222
    *   dimension A-290
    *   set A-457
*   **House front** A-189

### I
*   **Icon bar** A-21
*   **Icons**
    *   Help A-24
    *   Import A-23
    *   New pattern A-23
    *   Open A-23
    *   Open master data A-24
    *   Print A-23
    *   Print transfer file A-23
    *   Restore A-24
    *   Save A-23
    *   Undo A-23
    *   Zoom down section A-23
    *   Zoom up section A-23
*   **Identifying a shape** A-370
*   **IG**
    *   define unit A-418
    *   processing A-479
*   **Step** A-411
*   **Importing a contour** A-228
*   **Input window** A-21
*   **Inside contour**
    *   Basics A-33

### L
*   **LAMI**
    *   Pre-compound A-413
*   **Laminated**
    *   arrissing A-415
    *   edge block-grinding A-413
    *   edge with mitre A-414
    *   processing A-479
    *   Special edge A-410
    *   step A-411
    *   unit A-418
*   **Length of a line**
    *   dimension A-264
*   **Length of an arc**
    *   dimension A-286
*   **Line**
    *   dimension length A-264
    *   enter A-230
    *   optimum A-225
*   **Link**
    *   contours A-241
    *   segments A-226, A-239
    *   with AWBroke A-483
*   **Link edge deletion** A-372
*   **Linking**
    *   with AWBroke A-488
    *   Linking with SNAuto A-493
*   **Lite**
    *   enter as sketch A-449
    *   rotate A-365
*   **lite**
    *   digitize A-438
    *   with BOM A-480

### M
*   **Macro** A-317
    *   rounding A-320
*   **Manual input** A-18
*   **Measuring point**
    *   digitize A-222
    *   set A-390
    *   show A-511
*   **Merge contours** A-328
*   **Mitered edge** A-407
*   **Mitre on laminated edge** A-414
*   **Move** A-429
    *   contour A-243
    *   edge A-242
    *   point A-233, A-236, A-237
*   **Multiple grinding** A-378

### N
*   **Nesting** A-18
*   **Notch**
    *   add to contour A-325
    *   as BOM element A-329
    *   blend with contour A-329

### O
*   **Operation of Shaping&Nesting**
    *   Basics A-419
    *   Overview A-211
*   **Overview**
    *   tools A-212

### P
*   **Pattern**
    *   create print file in Word A-482
    *   digitize A-438
*   **Points**
    *   Dimension distance A-254
    *   dimension distance parallel with a line A-257
    *   dimension distance vertical to a line A-258
    *   dimension distance, parallel with a line A-254
    *   dimension horizontal distance A-263
    *   dimension vertical distance A-262
    *   dimension with X and Y coordinates A-265
    *   move A-233, A-236, A-237
*   **Position axis** A-384
*   **Position stops** A-384
*   **Position text on sketch** A-396
*   **Positioning a section** A-460
*   **Prepare cutting** A-476
*   **Primitive** A-18
*   **Print**
    *   a file A-172
    *   create pattern in Word A-482
    *   sketch A-481
    *   via Word A-481
*   **Process optimisation** A-16
*   **Processing**
    *   architectural glass A-479
    *   corner A-478
    *   laminated A-479
    *   toughened A-479
*   **Production process, Basics** A-36
*   **Properties** A-19

### R
*   **Radius**
    *   add A-454
    *   dimension A-284
    *   Tools A-304
*   **Reduce a view** A-419
*   **Reflect a contour** A-429
*   **Reflecting a contour** A-244
*   **Required knowledge** A-12
*   **Restore** A-428
*   **Revision, Basics** A-32
*   **Rotate a contour** A-365, A-429, A-454
*   **Rounded corner as BOM element** A-316

### S
*   **Section**
    *   add to door A-457
    *   create A-457
    *   position A-460
*   **Segment**
    *   caption A-232, A-395
    *   dimension A-252
    *   format A-395
    *   smooth transition A-269
    *   split A-238, A-327
*   **Segment caption** A-232, A-395
*   **Segments** A-18
    *   dimension inside angle A-270
    *   dimension vertical to another A-273
    *   group A-432
    *   link A-226, A-239
    *   parallel dimensioning A-273
*   **Select segment and contours** A-428
*   **Selection** A-421
*   **Set checkpoint** A-390
*   **Set transition angle to 0** A-239
*   **Shape** A-19
    *   create A-468
    *   enter in ALFAK A-496
    *   enter trim A-364
    *   identify A-370
    *   use A-469
*   **Shape edge**
    *   Edge overview A-416
    *   inside A-417
    *   outside A-417
    *   Special edge A-416
*   **Shape identification** A-370
*   **Shapes: see contours**
*   **Shaping & Nesting** A-18
*   **Shaping & Nesting AT** A-15
*   **Shaping & Nesting ATM** A-14
*   **Shaping&Nesting**
    *   Operation A-211
    *   Terms A-18
*   **Sharpen corner** A-312
*   **Show grid** A-511
*   **Sketch**
    *   add text A-396
    *   change layout A-509
    *   create A-229, A-449, A-481
    *   design A-463
    *   design with variables A-473
    *   dimension A-451, A-455
    *   distort A-396
    *   export A-424
    *   import A-424
    *   open A-424
    *   print A-481
    *   print via Word A-481
    *   save A-424
    *   set starting point A-229
*   **Smoothing a contour** A-233
*   **SN object** A-18
*   **Special bevel** A-409
*   **Special edge** A-405
*   **Special laminated edge** A-410
*   **Splitting a segment** A-238, A-327
*   **Standard bevel** A-408
*   **Staring point**
    *   set A-373
*   **Starting point**
    *   for Bando cutting/grinding machine A-376
    *   for master and slave A-374
    *   of sketch A-229
*   **Starting point for machine**
    *   enter A-375
*   **Stepped IG** A-411
*   **Stepped laminated** A-411
*   **Stretch** A-429
*   **Suckers** A-384
*   **Surface and control elements** A-16
*   **Surface Processing**
    *   Place A-335, A-345

### T
*   **Tag** A-421
*   **Technical order processing (TOP)**
    *   and A+W Business A-495
    *   and A+W Enterprise A-483
*   **Technologies, tools** A-350
*   **Terms in Shaping&Nesting** A-18
*   **Tool** A-18
*   **Tools** A-21
    *   Architectural glass A-392
    *   Define edge A-416
    *   dimension angle A-268
    *   for technologies A-350
    *   Functional principle A-249
    *   overview A-212
    *   round corner A-312
    *   Set starting point A-373
    *   smooth contour A-233
*   **Trim**
    *   define A-476
    *   for shape A-364

### U
*   **Undo** A-428
*   **Unit**
    *   basics A-35
*   **Units with BOM** A-480
*   **Using shapes** A-469

### V
*   **Variables**
    *   Define condition A-470
    *   List A-184
    *   use in sketch A-473
    *   using variables A-470
*   **View** A-18
    *   internal contours A-197
    *   redraw A-197
    *   settings A-198
    *   show all A-197
    *   show dimensions A-196
    *   show selection A-196
    *   tools A-198
    *   update BOM A-197
*   **Virtual digitizing** A-227, A-443

### W
*   **Window**
    *   arrange icons A-204
    *   list of file names A-204
    *   overlapping A-204
    *   tile horizontally A-204
*   **Word**
    *   file pattern A-482
    *   print sketch A-481
*   **Working with variables** A-470

### Z
*   **Zoom** A-419
*   **detail of a sketch** A-393
*   **Zoom detail** A-393
