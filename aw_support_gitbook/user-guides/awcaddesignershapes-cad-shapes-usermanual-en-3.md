---
description: "EN-UM-AWCADDesignerShapes_8"
---


# The Use of Tools

If you change contours (i.e. the glass edge or the position of the contour changes) after entering the auxiliary cut, the auxiliary cut will automatically keep the defined distances and alignment.

1.  Choose the tool. Click on the corresponding icon.
2.  Select the segment from which the auxiliary cut shall start, to be extended with the same gradient. The selected segment is shown in red.
3.  Select the edge of the pattern in the direction of which the auxiliary cut shall run. The contour points of the selected edge are highlighted in green.
4.  Confirm your entry by `<ENTER>` or [OK].

**Example:**

*Fig. A-199 Define an auxiliary cut by extending a segment*
*   **A**: Tagging sequence (1. select red line, 2. select green line)
*   **B**: Result of extension

The zoomed display of the bottom left corner of the pattern shows the auxiliary cut, from the contour to the glass edge (dotted line). You can see the distance that is kept between auxiliary cut and contour/pattern.

5.  To change these two distances, click on the segment. Two input fields appear:
    *   `_`: Distance between contour and auxiliary cut.
    *   `[`: Distance between edge and auxiliary cut.
6.  Enter the required value and confirm by `<ENTER>` or [OK].

Both defaults can also be set permanently to another value in sn.ini.

---
### Defining an auxiliary cut by extending a segment

This tool serves to create an integrated auxiliary cut which results in an extension of the selected segment; the formerly adjacent segment is separated from the extended segment by a small gap. The distance between the two segments after the separation is set when A+W CAD Designer (Shapes) is installed (in sn.ini).

The auxiliary cut, i.e. the extension of the selected segment, is extended as a straight line with the same gradient the selected segment shows in the corresponding end point. This means that the cut is extended and ends in a short distance from the edge of the primitive. To change the two distances, tag the auxiliary cut or the connecting auxiliary line. Two input fields appear:

*   `(`: Distance between the extended segment and the originally adjacent segment.
*   `[`: Distance between edge and auxiliary cut.

Both defaults can also be set permanently to another value in sn.ini.

If you change contours (i.e. the glass edge or the position of the contour changes) after entering the auxiliary cut, the auxiliary cut will automatically keep the defined distances and alignment.

1.  Choose the tool. Click on the corresponding icon.
2.  Tag the segment to be extended. Click on the segment half in the direction it shall be extended towards the surrounding rectangle. The segment is marked by an arrow pointing in the direction of the extension.
3.  Confirm your entry by `<ENTER>` or [OK]. The integrated auxiliary cut will be calculated and displayed.

**Example:**

*Fig. A-200 Defining an auxiliary cut by extending a segment*
*   **A**: Starting position
*   **B**: Result

In this example, an auxiliary cut is made from the bottom right corner, ending shortly before the surrounding rectangle.

The zoomed display in the bottom right corner of the surrounding rectangle shows the auxiliary cut from the contour to the glass edge (dotted line). You will see the distance d which is kept between auxiliary cut and surrounding rectangle. Additionally, the original corner of the contour opens around distance D (this makes breaking the glass easier). The dotted connection between the left contour segment and the end point of the auxiliary line does not influence the cutting process. The program establishes this connection only to keep the contour closed which is essential for further calculations.

### Enter auxiliary cut to split the trim

Use this tool to define an auxiliary cut that lies in the center of an arc, and vertical to the arc (vertical to the secant). The auxiliary cut runs from the contour to the surrounding rectangle. The auxiliary cut ends in a defined distance from the segment and the edge. These values are defined during installation, in sn.ini. To change the two distances, tag the auxiliary cut. Two input fields appear:

*   `_`: Distance between contour and auxiliary cut.
*   `[`: Distance between edge and auxiliary cut.

Both defaults can also be set permanently to another value in sn.ini.

If you change contours (i.e. the glass edge or the position of the contour changes) after entering the auxiliary cut, the auxiliary cut will automatically keep the defined distances and alignment. To change the position and distances of auxiliary cuts, you can dimension them against the contour or move them by means of menu Transform.

1.  Choose the tool. Click on the corresponding icon.
2.  Click on the segment in the center of which the auxiliary cut shall start.
3.  Confirm your entry by `<ENTER>` or [OK]. The auxiliary cut will be computed and appears on the sketch.

**Example:**

*Fig. A-201 Auxiliary cut splitting the trim*

In this example, the auxiliary cut is marked by the letter c. The glass edge is identified by the letter d. The arrows a and b represent the secant of the arc segment.

### Enter auxiliary cut to split two contours

If you have nested two or more contours inside a surrounding rectangle to minimize the waste, the contours are easier to cut (because of the breaking properties of glass) if they are separated by an auxiliary cut. This is what this tool is for. The distance between contour and auxiliary cut has to be entered together with the cut.

If you change the contours (glass edge or position of the contour changes) after entering the auxiliary cut, the auxiliary cut will automatically keep the defined distances from the surrounding rectangle. The lateral distance from the contour will not be forced to remain flexible when nesting contours. To change the position and distances of auxiliary cuts, you can dimension them against the contour or move them via menu Transform.

1.  Choose the tool. Click on the corresponding icon.
2.  Select the segment where the separating cut shall be applied. The segment colour changes (normally to red) and the segment is shown in bold.
3.  Enter in `||` the distance between the selected segment and the separating cut.
4.  Confirm your entry by `<ENTER>` or [OK]. The separating cut will be computed and appears on the sketch.

**Example:**

*Fig. A-202 Separating cut*

In this case, two triangles are nested within a surrounding rectangle. To be able to break these contours without damage, we have added the auxiliary cut X.

### Enter new tangential path for an offset cutting machine

1.  Choose the tool. Click on the corresponding icon.
2.  Click on the start of the segment on the contour in the tangential entry direction.
3.  Enter the following values:
    *   `d-`: Length of entry path in X direction.
    *   `d]`: Length in Y direction.
    *   `t`: Distance of auxiliary line and entry point.
    This auxiliary line is added to keep the contour closed.
4.  Confirm your entry by `<ENTER>` or [OK].

### Enter a new loop-like auxiliary cut

It is shaped like an oblong loop and is executed up to the edge of the cutting rectangle. The transitions are smooth so that the cutting wheel does not have to be upped. This permits very fast cutting. Two segments of equal direction are selected. In the direction of the first segment, the cut is extended up to the edge of the cutting rectangle. After a curve, the cutting path is retraced parallel with the first cut. At the final point of the second selected segment, the auxiliary cut meets up with the shape again. The width of the loop and the distance to the edge of the cutting rectangle can be changed.

1.  Choose the tool. Click on the corresponding icon.
2.  Select the first segment. The segment color changes to red.
3.  Select the second segment. The segment color changes to green.
4.  Confirm your entry by `<ENTER>` or [OK].
5.  The width of the loop and the distance to the edge are preset with (configurable) default values. To adjust the values, select one of the newly created lines. The input window served to adjust the parameters.

### Connecting two auxiliary cuts with one another

With this tool, you can connect two integrated auxiliary cuts with one another. This way, you can chain an area of the shape in order to cut it later.

The tool is available in the Cutting view.

In order to use this tool, you must first place the required auxiliary cuts.
⇨ "Defining an auxiliary cut by extending a segment" on page A-351

1.  Select the tool. Click on the corresponding icon.
2.  Select the first auxiliary cut. This will be shown in red.
3.  Select the second auxiliary cut. This will be shown in green.
4.  Enter the desired rounding radius (R) in the input field.
5.  Confirm your entry by `<ENTER>` or [OK].
6.  The two auxiliary cuts are connected to one another.

### Creating an auxiliary cut vertically to the contour

With this tool, you define an auxiliary cut that is continued vertically to the selected segment up to the edge of the glass. The auxiliary cut runs from the contour to the pattern (from which the contour is cut). The auxiliary cut ends in a defined distance from the segment and the edge. This value has been saved in sn.ini when the system was installed.

If you change contours (i.e. the glass edge or the position of the contour changes) after entering the auxiliary cut, the auxiliary cut will automatically keep the defined distances and alignment.

If there is no suitable segment end point for opening the shape, you first have to set a division point (SPLIT tool).

1.  Select the tool. Click on the corresponding icon.
2.  Click a segment at one of its end points. The selected segment is shown in red.
3.  Select the edge of the pattern in the direction of which the auxiliary cut shall run. The contour points of the selected edge are highlighted in green.
4.  Confirm your entry by `<ENTER>` or [OK].

**Example:**

*Fig. A-203 Auxiliary cut vertically to the contour*

The enlarged diagram shows the auxiliary cut and the rounding.

### Satellite for free breaking

During the manufacturing of auto glass lites, one of the important tasks is to break complex forms quickly and safely. In the past, breakage templates were used underneath the glass for this purpose. The breakage templates were slightly larger than the cut shape. The breakout wheel rolled largely parallel to the cutting shape. Thanks to the lever effect between breakage template, weight of the glass, and force of the breakout wheel, the cut was broken.

In particular, for small quantities, the manufacturing of breakage templates is unreasonably expensive.

This tool is a free satellite that provides the counter-force required from below the transport belt. In the cutting code, the coordinates for both tools are transmitted per movement command.

The tool is available in the Breakout view. In order to be able to use the tool, the following prerequisites must be fulfilled in A+W CAD Designer (Shapes):

*   The auxiliary cuts for breakout are present
*   The breakage path is generated
*   Additional paths for the satellites are generated. These paths are created like breakage paths (e.g. with the AUTOBRK tool). Thanks to the now subsequent marking with the SATELLITE tool, they are interpreted as path information for movement of the satellite.

By using the SATELLITE tool, one position on the breakage path is synchronized with one position on the satellite path. If the breakage tool is on the marked point of the breakage path, the satellite should be at the corresponding point on the satellite path. Thanks to the two-time use of the tool, a section of the breakage path can thus be synchronized with a section of the satellite path.

1.  Select the SATELLITE tool to synchronize the breakage path and the satellite path.
2.  First click a point on the breakage path to mark a position of the breakage tool. It is shown as a red dot.
3.  Then click a point on the satellite path to mark a position of the satellite. It is shown as a red dot. With the cuts 2 and 3 it is ensured that the satellite and breakage tool are at the selected point at the same time.
4.  Confirm your entry by `<ENTER>` or [OK]. The breakage path and the satellite path are connected at the start with a dotted line and the satellite path is shown in green.
5.  Repeat steps 2, 3, and 4 to determine an end point for the synchronization. The starting and end point of the satellite path can match; in this case, the satellite will not move on this section (fixed satellite).
6.  Repeat steps 2 to 5 to synchronize the movement of breakage tool and satellite on several sections.

The breakage sequence arises due to the starting points on the breakage paths. The sequence for the satellite path arises through the synchronization information stored with the SATELLITE tool. Therefore, no starting points are set on the satellite path.

> **Depending on the cutting table**
> This tool is not offered or supported by all cutting table manufacturers. That is, the use of the tool depends on whether your cutting table has this tool.

## Define cutting path at the corners

You can use the following tools to define cutting paths at the corners:

| Symbol | Short name | Description |
| :--- | :--- | :--- |
| 