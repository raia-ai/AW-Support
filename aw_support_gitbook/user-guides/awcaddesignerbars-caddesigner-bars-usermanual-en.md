---
title: "EN-UM-AWCADDesignerBars"
source: "EN-UM-AWCADDesignerBars.pdf"
tags: ["A+W", "CAD Designer", "Bars", "Muntins", "Software Manual", "Glass", "Windows", "Doors", "Tutorial", "Software Reference"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is the official user manual for the A+W CAD Designer (Bars) software, a program designed for creating muntin patterns for glass, windows, and doors. It provides comprehensive guidance on using the software, from basic operations to advanced features. The manual includes a detailed tutorial, a complete software reference, and quick-access help cards to assist users in mastering the design and configuration of muntin bars."
long_description: "This is the complete English manual for the A+W CAD Designer (Bars) software, intended for end users who design and manufacture windows and doors with muntin bars. The document is structured into several key parts to facilitate learning and quick reference. The 'Editorial' section outlines the document's scope, copyright information, and display conventions. A main 'Overview' section introduces the software's purpose and structure. The core of the manual is the 'Tutorial' section, a step-by-step guide that walks users through the entire process of using the software. This includes navigating the user interface, managing settings, defining master data for different muntin types (glass-dividing, internal, fitted), creating new designs, positioning muntins, and working with special patterns like diamonds, suns, and stars. It also covers the creation and use of macros for recurring patterns and explains data exchange processes. Following the tutorial, the 'Software Reference' provides an exhaustive A-Z guide to every menu, dialog, tool, and function within the application, serving as a detailed technical dictionary for users. Finally, the 'Help Cards' section offers task-oriented, quick-reference guides for the most common operations, such as creating a house front, loading a macro, or protecting master data. This manual equips users with the knowledge to efficiently create both simple and complex, true-to-scale muntin patterns for production."
---
# A+W CAD Designer (Bars) Manual

---
## Editorial

### Revision overview of the documentation

| Date | Description |
| :--- | :--- |
| 10-2024 | Update of complete manual for PDF and HTML5 format. |

### Notes
This document is intended only for end users of A+W CAD Designer (Bars).

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of A+W CAD Designer (Bars).

### Copyrights
© 2024, A+W Software GmbH all rights reserved, also those for reprinting, the making of copies and translation.

The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Display conventions
Individual elements of the sentences are displayed in a special form. The meanings are:

- **Italics**: marks character strings describing the software elements, e.g. the *Buckets* dialog.
- **Bold**: marks character strings to be entered via keyboard, e.g.: Enter **0**.
- **>**: shows the way to open a dialog, e.g. *Display > Filler orders > Context menu - List > Order overview*.
- **[]**: square brackets mark the buttons in the dialog, e. g. [OK] to save the data.
- **< >**: pointed brackets refer to keys or shortcuts on the keyboard, e. g. <F1> is used to open the online help

### Contact
**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Deutschland

**Tel.:** +49 641 96620 0
**E-Mail:** info@a-w.com
**Web:** http://www.a-w.com

## A - A+W CAD Designer (Bars) Overview

### Revision overview of the module:

| Date | Description |
| :--- | :--- |
| 01-2017 | Product and company names adjusted. |
| 03-2013 | Revision as part of the product realignment |
| 10-2010 | Original version |

This module provides information on the following subjects:
- Tutorial
- Software Reference

## A - A+W CAD Designer (Bars) Tutorial

This section provides information on the following subjects:
- Overview
- A+W CAD Designer (Bars) introduces itself
- Working with A+W CAD Designer (Bars)
- Muntins
- Special patterns
- Data exchange
- Configuration
- Annex - Macro Catalog

### Overview
The A+W CAD Designer (Bars) training is meant for users who create simple as well as complex muntin patterns. You will learn how to enter master data and create muntin patterns.

For frequently occurring patterns, you will be taught how to create and use macros. With the help of these macros it is quite easy to create one's own catalogue of patterns.

**Subject areas**
This tutorial offers the following subject areas:
- A+W CAD Designer (Bars) introduces itself
- Working with A+W CAD Designer (Bars)
- Settings
- Master data in A+W CAD Designer (Bars)
- Muntins
- Cutting and measuring
- Special patterns
- Data exchange
- Configuration
- Annex - Macro Catalog

> **Required knowledge**
> Basic knowledge of EDP or Windows are prerequisite for using A+W CAD Designer (Bars).

### Tutorial Structure
This tutorial consists of subject areas with several learning units each. Each learning unit consists of the following elements:

- **Overview**: Each learning unit starts with an overview of the major subjects:
    - Objectives: What shall be taught?
    - Benefit: What can this knowledge be used for?
    - Maxims: Which connections are to be remembered?
- **Concepts**: Concepts and terms of the corresponding learning unit will be explained first. This is followed by examples and operating instructions.
- **Exercises**: For some learning units, exercises with certain tasks and suggested solutions are available. These exercises shall help you understand and use A+W CAD Designer (Bars).
- **Cross references**: At the end of each learning unit there is a section with cross reference pointing out the corresponding descriptions in the software reference. This shall help you to extend your new-found knowledge.
- **Reading instructions**: The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend that you do not skip any learning units. If you are already familiar with this subject you should at least read the summary at the beginning of the learning unit in order to visualize the main details.

The practical part of each training unit automatically includes the software reference and the exercises on the cross references. This will provide a central thread through the entire documentation.

### A+W CAD Designer (Bars) introduces itself
Inventive architecture and individual taste are more and more expressed in extraordinary muntin patterns. The increasing number of special muntin constructions requires a powerful construction program also capable of editing the required pattern true to scale, on screen, via printer or plotter.

A+W CAD Designer (Bars) is a Windows-based muntin construction program with a graphic user interface that allows to arrange most of the common grid types in the required pattern on rectangular or shaped lites. You can add muntin of different width to a construction and also use different muntin types in a pattern. A+W CAD Designer (Bars) allows the construction of patterns with rectangular, curved, and angled muntins.

Please obey the customary specifications. In Germany for instance, inward-opening tilt/turn windows are mainly used. In America, by contrast, sliding or winding windows opening to the outside are the custom.

#### Muntin pattern
A+W CAD Designer (Bars) provides an automatism for the most frequent muntin patterns such as clear fields. Apart from that, free designs can be created easily by means of auxiliary points. As it is the custom in CAD programs, these auxiliary points can be created by a number of geometrical operations (e.g. intersection or distance). In addition, individual muntins or groups of muntins can be manipulated in many different ways. Details can be made visible with the help of enlarged sections.

#### Muntin alignment
The muntins are aligned on a work surface on which lites can be positioned and displayed at random. At the same time, the muntin pattern can be adapted to the house front. This means that the optically correct progress of the bars can be continued over all lites of the house front.

#### Output
A true-to-scale sketch will be printed which also includes the list of profiles to be cut. This sketch also shows all relevant information for the muntin crosses like e.g. the milling angle. There are no restrictions as to the creation of production papers; these can be shown on screen or printed, as required. True-to-scale edition via plotter.

#### Macros
Macros can be applied to frequently used patterns. Macros are easy to create. Only the actual sizes need to be entered. With the help of these macros it is quite easy to create one's own catalogue of patterns.

#### Dimensioning
The size of the finished design can be adapted to the individual production requirements. It is possible for example to define drill point information referring to the inside edge or referring to the outside edge of the spacer.

#### Other details
The integrated interface allows quick and easy import of data. Additionally, NC codes for various machinery (e.g. Hegla muntin saw, Rottler & Ruediger saw and assembly center) can be created.

## Working with A+W CAD Designer (Bars)

This subject area explains A+W CAD Designer (Bars)'s user interface and its use.

### The A+W CAD Designer (Bars) user interface

**Objectives**
- Introducing the user interface of A+W CAD Designer (Bars)
- Introduction and explanation of catch points
- Introduction and explanation of tools
- Description of the input window
- Introducing the different cursor shapes

**The benefit**
A+W CAD Designer (Bars) can be used to the best effect only if you are capable of applying the tools available. The better you know the A+W CAD Designer (Bars) tools, the more efficient your work will be.

**Definitions**

| Term | Definition |
| :--- | :--- |
| **Icon bar** | is the horizontal bar containing small buttons with symbols (icons). |
| **Tools** | will help you design muntin patterns. |
| **The input window** | Based on your selection you will get information on the materials used and the corresponding quantities. |
| **Design area** | This is where the muntin patterns are designed. |
| **Catch points** | will help you position the muntins. |

> **Note**
> - Icon bar, tools, input windows, and catch points can be moved to any position by means of the mouse.
> - The functions can be shown or hidden as required in menu *View*.
> - Depending on your actions, the cursor will change its shape in A+W CAD Designer (Bars).

### Program presentation
When you start A+W CAD Designer (Bars), it will look as follows:
(A description of the user interface components)
- **A** Menu bar
- **B** Icon bar
- **C** Standard muntin (as defined)
- **D** Tools
- **E** The input window
- **F** Design area
- **G** Catch points

The top section includes - from left to right - the menu bar (A), the icon bar (B), and the standard muntin (C). Below the standard muntin are the tools (D) and the input window (E). The catch points (G) appear on the side of the screen. The large central area is the design area (F).

> **Moving elements**
> Apart from the menu bar, you can move all elements as required. This allows to adapt the design area to your needs.

### The menu bar
The menu bar offers the main functions for the user. The individual menus can be opened by a mouse-click. Some of the menus are directly accessible by hotkeys.
(*File Edit Macro Info Database View Help*)

### The icon bar
The functions that can be executed with an icon are also accessible via the menus. A+W CAD Designer (Bars) offers the following icons.

#### Description of the individual icons
At the end you will find a list of buttons/icons and their meaning.

| Icon | Explanation |
| :--- | :--- |
| New | New design (lite, macro, house front). Press this button to create a new file. If there is still a design on your workspace, the program will want to know if this shall be saved. After that, the workspace will be emptied. |
| Open | Open a design. Press this button to open the file. The dialog *Open file...* appears. |
| Save | Save a design. Press this button to save the file. |
| Print | Print a design. Press this button to print the design. Please make sure that the required printer has been installed/configured. |
| Import | Import a transfer file. Press this icon to import the files which have been transferred to A+W CAD Designer (Bars) by other systems. |
| Print Transfer | Print a transfer file. Press this icon to print a file which has been transferred by another system. Please make sure that the required printer has been installed/configured. |
| Scale Up | Scale up section. There are two versions: A click of the mouse enlarges the design by 10%. Keep pressing the mouse key while extending a section. |
| Scale Down | Scale down section. A click of the mouse reduces the design by 10%. |
| All | All. The design is enlarged or reduced so that it can be displayed completely. |
| Undo | Undo the last action. |
| Redo | Restore the last, cancelled action. |
| Help | Load help. |
| Master Data | Open master data. Press this icon to open the dialog *Master data*. |

> **Moving the icon bar**
> You can tag the icon bar and position it elsewhere.

### The input window
The contents of the input window change depending on your selection. When you select a bar or a segment from a design, A+W CAD Designer (Bars) shows the corresponding article, width, colour, and the continuous bar. The field ID appears only in connection with A+W Business, in which case it will be filled in automatically.

Example of input window values:
- Muntin Article: 0002
- Muntin Width: 8.00
- Milling: 2.00
- Color of Muntin: gold
- Uninterrupted: Milling
- Muntin Length: 158.00
- Cross Thickness: 8.00

> **Sizes for dimensioning**
> If dimensioning is active, you can click on it to display the sizes in the input window. The sizes can be easily changed in the input window.

When you press [Quantities], A+W CAD Designer (Bars) will come up with the number of design characteristics. These characteristics are relevant for pricing.

### The standard muntin
This bar is the so-called standard muntin, i.e. unless you select another muntin, this one will be used for all designs. This muntin is active whenever you start the program. You can change the muntin temporarily anytime by selecting another muntin from the combo box.
(*0001 [Helima 2000 (26)] - 26 mm unknown*)

You can define the standard muntin in dialog *Master data editor*.

### The cursor
The cursor can change its shape in A+W CAD Designer (Bars) depending on your current action. The cursor can take the shapes listed below:

- **Arrow Cursor**: The cursor for common operation. It can be used to tag individual elements, or activate tools or catch points.
- **Crosshairs Cursor**: When you position the cursor on a catch point, the cursor takes the shape of crosshairs. Crosshairs will make your work easier. Whenever the cursor takes the shape of crosshairs, you have nearly hit the catch point.
- **Continuity Cursor**: When you change the continuous muntin, the cursor changes its shape.
- **Extend Cursor**: For extending muntin, the cursor changes its shape.

### The catch points
A+W CAD Designer (Bars) permits you to position auxiliary points, so-called catch points, on the design. The catch points can be added at random and help to position segments (bars, curves, etc.) correctly. When you point the cursor on the lite and press the right mouse key, A+W CAD Designer (Bars) will automatically set a catch point in each corner and in the center of the surface. These automatically positioned catch points are shown in green. Manually positioned catch points are shown in red.

#### Working with catch points
The following table provides a list of the catch points available in A+W CAD Designer (Bars).

| Icon | Name | Explanation |
| :--- | :--- | :--- |
| Delete | Delete | Deletes a catch point. |
| Delete All | Delete all | Deletes all catch points. |
| Division | Division | Enter the number of interval divisions for object, distance, and parallel. |
| Intersection | Intersection | Creates catch points wherever two objects cross. |
| Relative | Relative | Creates a catch point in relation to any defined point. |
| Object | Object | Creates catch point on a muntin, spacer, or the lite edge. |
| Rectangle | Rectangle | Creates four catch points at the corners of a rectangle defined by two mouse-clicks. |
| Row | Row | Creates catch points at all intersections with other muntins. |
| Distance | Distance | Creates catch points on a straight line. |
| Length of arc I | Length of arc I | Creates a catch point on an arc in a defined distance. |
| Center I | Center I | Creates catch points in all feasible centers of circles (two points). |
| Parallel | Parallel | Creates catch points with a parallel shift from a straight line. |
| Length of arc II | Length of arc II | Creates a catch point in a defined distance along the arc. |
| Center II | Center II | Creates catch points in the center of a circle (three points). |
| Direction | Direction | Creates catch points in an adjustable angle from the reference point. |
| Vector | Vector | Creates a catch point on a straight line in a defined distance from the starting point. |

#### Catch points - examples

**Creates catch point(s)**
This tool can be used to set catch points by defining intervals.
1. Choose the tool. The dialog *Enter intervals for catch points* opens.
2. Enter the number of intervals (areas between the catch points), e. g. 3.
3. Four catch points will be set.

**Creates a catch point at an intersection**
This tool can be used to set catch points at intersections of muntins.
1. Choose the tool.
2. Click on the first muntin, e. g. the horizontal one.
3. Click on the second muntin, e. g. the vertical one.
4. The catch point will be set at the intersection of the two selected muntins.

**Creates a relative catch point**
Use this tool to set a catch point in relation to a certain point.
1. Choose the tool.
2. Click on the reference point, e. g. intersection of two muntins.
3. The dialog *Enter - Relative distance* opens.
4. Enter the horizontal distance from the reference point in field dx, e. g. 80 mm.
5. Enter the vertical distance from the reference point in field dy, e. g. 40 mm.
6. Press [OK] to close the dialog.
7. The catch point will be set in accordance with the defined coordinates.

**Creates catch points on objects**
Objects can be muntins, spacers, or the lite edge.
1. Choose the tool.
2. Click on the object on which catch points shall be positioned, e. g. the horizontal muntin.
3. The catch points will be positioned on the muntin.
> **Number of catch points**: The number of catch points you are going to position can be set with the tool *Number?*.

**Creates four catch points on the corners of a rectangle**
This tool allows you to set four catch points on a cross. Just enter two catch points; A+W CAD Designer (Bars) will add the other two automatically.
1. Choose the tool.
2. Click on the first catch point.
3. Click on the second catch point.
4. The two missing catch points are positioned.

**Creates catch points on intersections**
This tool can be used to set catch points on intersections.
1. Choose the tool.
2. Click on the object on which catch points shall be positioned, e. g. the horizontal muntin.
3. The catch point is positioned on the intersection.

**Create a number of catch points from (starting point) to (end point)**
You can use this tool to set the desired number of catch points on a muntin. Just enter the start and end point.
1. Choose the tool.
2. Click on a starting point on the object, e. g. the horizontal muntin.
3. Click on the end point on the object.
4. The catch points will be positioned on the muntin.
> **Number of catch points**: The number of catch points you are going to position can be set with the tool *Number?*.

**Positioning catch points along an arc**
This tool is used to position a catch point on an arc in a defined distance (radius).
1. Choose the tool.
2. Click on the center of the arc.
3. Click on a point on the arc. The dialog *Enter segment length of arc* opens. Enter **-45**. Close the dialog using the [OK] button.
4. The catch point is positioned accordingly.
> **Setting catch points**: As the tool icon shows, the catch point will be set clockwise. Entering a negative 45 means that the catch point will be set counterclockwise.

**Position catch point in feasible center**
This tool is used to position a catch point in the center of a circle.
1. Choose the tool.
2. Click on the first point on the arc.
3. Click on the second point on the arc. Dialog *Enter radius* opens. Enter **200**. Close the dialog using the [OK] button.
4. The catch points will be positioned accordingly. This entry permits setting two catch points, corresponding to the two intersection points of circles with the entered radius (200) drawn from the two clicked points.

**Creates catch points parallel with a straight line**
This tool can be used to position catch points parallel with a muntin.
1. Choose the tool.
2. Click on the starting point of the object parallel with which the catch points shall be positioned, e.g. the horizontal muntin.
3. Click on the end point of the object. Dialog *Enter parallel distance* opens. Enter **100** mm. Close the dialog with [OK].
4. The catch points are positioned.

**Position catch point in defined distance along an arc**
This tool is used for positioning a catch point on an arc, in a defined distance.
1. Choose the tool.
2. Click on the center of the circle.
3. Click on a point on the arc. Dialog *Enter length of arc* opens. Enter **100** mm. Close the dialog using the [OK] button.
4. The catch point is positioned. (This corresponds to an arc length of 100).

**Creates a catch point in the center of a circle (three points)**
You can use this tool to position a catch point in the center of an arc defined by three points.
1. Choose the tool.
2. Click on the first point on the arc.
3. Click on the second point on the arc.
4. Click on the third point on the arc.
5. The catch point is positioned.

**Creates catch points at a defined angle**
This tool can be used to position catch points parallel with a muntin.
1. Choose the tool.
2. Click on the reference point. Dialog *Enter direction of angle (degrees)*. Enter the degrees of the angle, e. g. **45°**. Another dialog opens, *Enter length of direction (in mm)*, e. g. **200**.
3. The catch points will be positioned accordingly.
> **Number of catch points**: The number of catch points you are going to position can be set with the tool *Number?*.

**Creates a catch point on a straight line in a defined distance from the starting point**
Use this tool to position a catch point on a straight line.
1. Choose the tool.
2. Click on the reference point.
3. Click on a point in the desired direction. Dialog *Enter distance* appears. Enter the distance, e. g. **200**.
4. The catch point is positioned accordingly.

**Deletes the catch point**
This tool serves to delete a single catch point by clicking on it.
1. Choose the tool.
2. Click on the catch point you want to delete.
3. The catch point is deleted.

**Deletes all catch points**
This tool is used to delete all catch points by just one mouse-click.
1. Choose the tool.
2. All catch points are deleted.

### The tools
A+W CAD Designer (Bars) offers a number of tools to make your task easier. The tools are also available in the menus.

#### Using the tools
The following table shows the tools available in A+W CAD Designer (Bars).

| Icon | Explanation |
| :--- | :--- |
| Select | Select an element. |
| Straight Muntin | Creates a straight muntin between two catch points. |
| Horizontal Muntin | Creates a straight (horizontal) muntin between two catch points. |
| Vertical Muntin | Creates a straight (vertical) muntin between two catch points. |
| Angled Muntin | Creates a straight muntin between two catch points at a defined angle. |
| Curved Muntin | Creates a curved muntin between three catch points. |
| Circular Muntin | Creates a circular muntin between two catch points. |
| Sun | Creates a sun in a clear field. |
| Crescent | Creates a crescent. |
| Arc | Creates an arc in a clear field. |
| Change Continuity | The uninterrupted direction will be changed for a 90° cross. |
| Extend | Muntin will be extended up to a selected object. |
| Divide All | Divides all muntins. |
| Connect All | Connects all muntins. |
| Set/Delete Muntin | Sets or deletes a muntin in a clear field. |
| New Lite | Creates a new lite. Activate the tool then click on the lite to open the dialog. |
| Macro Pattern | Creates a muntin pattern in the lite from a macro. |
| V/H Muntins | Opens the dialog for entering vertical and horizontal muntins. |
| Quantities | Shows the corresponding quantities in the input area. |
| YT Cutting | Changes the YT cutting. |

Apart from the tools which are available as icons, A+W CAD Designer (Bars) offers the following tools (menu *Edit*):
- **Rotate**: Turning a muntin
- **Reflect**: Reflecting a muntin
- **Move**: Moving a muntin

#### Tools - examples

**Creates a straight bar between two catch points**
This tool is used to position a straight bar at a free angle.
1. Set the required catch points.
2. Choose the tool.
3. Click on the starting (catch) point of the straight line.
4. Click on the end (catch) point of the straight line.
5. The muntin is set.

**Creates a horizontal muntin**
This tool can be used to position a horizontal muntin.
1. Set the required catch points.
2. Choose the tool.
3. Click on the starting (catch) point of the straight line.
4. Click on the end point on the straight line.
5. The muntin is set.

**Creates a vertical muntin**
Use this tool to position a vertical muntin.
1. Set the required catch points.
2. Choose the tool.
3. Click on the starting (catch) point of the straight line.
4. Click on the end point on the straight line.
5. The muntin is set.

**Creates a straight muntin by means of a mouse-click and definition of the angle**
This tool can be used to position a straight muntin, defining any angle required.
1. Set the required catch points.
2. Choose the tool.
3. Click on the starting (catch) point of the straight line.
4. Click on the end point on the straight line. The end point also marks the length of the muntin.
5. The dialog *Enter angle* opens. Enter the required angle, e. g. **-45**.
6. The muntin is set.
> **Negative entries**: As the tool icon shows, the catch point is set counterclockwise. Enter a negative 45 to set the muntin clockwise.

**Creates a curved muntin by means of three mouse-clicks**
This tool offers two different procedures:
1. Click on the center of the arc, then on the starting point, and next on the end point.
2. Click on the starting point of the arc, then on the end point, and finally on any point on the arc.

Procedure 1 works as follows:
1. Set the required catch points.
2. Choose the tool.
3. Click on the center of the circle.
4. Click on the starting point of the circle.
5. Click on the end point of the circle.
6. The muntin is set.

**Creates a circle by means of two mouse-clicks**
This tool serves to create a circle of muntins, defined by its center and any point on the circle.
1. Set the required catch points.
2. Choose the tool.
3. Click on the center of the circle.
4. Click on any (catch) point on the circle.
5. The circle of muntins is set.

**Creates a sun in a clear field**
This tool can be used to create a radial pattern in a clear field.
1. Define the lite.
2. Choose the tool.
3. Click on the lite (clear field) in which the radial pattern shall be positioned.
4. The *Sun and stars* dialog opens. Activate the radio button **Same angles**. From the combo box *Number of rays*, select **5**. Quit the dialog by pressing [OK].
5. The radial pattern is positioned. (Other options include *Rays in corners* and different *cutting methods* like *Cut to corner*, *Cut to vertical spacer*, etc., which produce different results).

**Creates a crescent**
This tool is used where a radial pattern has been positioned. The crescent can be positioned where the rays of the sun meet.
1. Create the lite with the radial pattern.
2. Choose the tool.
3. Move the cursor to the point where the crescent shall be positioned. The cursor will change its shape into a crescent.
4. You can make the necessary settings in the *Input window* for *Radius* and *Orientation* (from bottom to top, top to bottom, right to left, left to right).

**Creates an arc in a clear field**
This tool is used to position an arc in a clear field.
1. Define the lite.
2. Choose the tool.
3. Click on the lite (clear field) in which the arc shall be placed.
4. In the *Input window*, you can make the necessary settings. The field *Mode* offers options like *Intersects vertical spacer*, *Meets corner*, *Radius measured from bottom*, etc. The *Orientation* field defines alignment.

**Changes the continuity of muntins**
This tool can be used to change the continuous muntin.
1. Starting position (e.g., the vertical muntin is continuous).
2. Choose the tool.
3. Click on the muntin crossing.
4. The continuity of muntins is changed (the horizontal muntin is now continuous).

**Extends a muntin**
This tool can be used to extend or shorten a muntin.
1. The muntin shall be extended/cut.
2. Choose the tool. The cursor changes shape.
3. Click on the muntin you want to extend/cut. It is shown in red.
4. Click on the object up to which the muntin shall be extended/cut.
5. The muntin is extended/cut.

**Divide all muntins**
This tool can be used to divide all muntins by a mouse-click.
1. Starting point: Two vertical muntins are continuous.
2. Choose the tool. The muntins will be split.

**Connect all muntins**
This tool can be used to connect all muntins by a mouse-click.
1. Starting point: All muntins are split.
2. Choose the tool. The muntins will be connected.

**Creates or deletes a muntin in a clear field**
This tool can be used to delete individual muntins or reposition them.
1. Starting position.
2. Choose the tool and position the cursor on the muntin to be removed.
3. Click on the left muntin.
4. The muntin is removed.
5. Move the cursor to the point where the muntin was deleted; it will change shape, allowing you to re-set the muntin.

**Change YT cut**
This tool determines the cut for Y muntins at a cross intersection.
1. Starting point: Tool is inactive, all muntins at the intersection are cut symmetrically.
2. Disable the tool: The intersection is calculated normally, only the two Y muntins are cut to meet the cross.

**Turning a muntin**
This tool is used to copy and turn a muntin by means of three mouse-clicks. (*Edit > Rotate*)
1. Starting point: The muntin to be rotated has been marked.
2. Select the menu item. Click on the center of rotation.
3. Click on the first reference point for the rotation.
4. Click on the second reference point for the rotation.
5. The muntin will be copied and turned.

**Reflecting a muntin**
This menu is used to reflect a muntin horizontally or vertically by just two mouse-clicks. (*Edit > Reflect*)
1. Starting point: The muntin to be reflected has been marked.
2. Select the menu item. Click on the first point on the reflection line.
3. Click on the second point on the reflection line.
4. The muntin is copied and reflected.

**Moving a muntin**
This menu is used to move a tagged muntin. (*Edit > Move*)
1. Starting point: The muntin to be moved has been marked.
2. Select the menu item. Press the left mouse key and keep pressing it. Move the muntin.

### Dimensioning tools
A+W CAD Designer (Bars) offers two dimensioning tools. These tools permit switching between dimensioning of absolute and relative drill points and defining whether the lite or the spacer is the reference point.
- **Absolute/Relative Drill Holes Tool**: Switches between absolute and relative dimensioning.
- **Lite/Spacer Reference Tool**: Defines whether measuring refers to the spacer or the lite.

> **Tick Dimensioning checkbox**
> You have to tick the checkbox *Dimensioning* in dialog *Settings...* to use the icons.

## Settings

**Objectives**
- Introduction and explanation of dimensioning.
- Understanding numbering of muntins.
- Understanding differences in dimensioning of drill points (absolute/relative, spacer/lites).
- Introduction of measurement systems.
- Starting the program in another language.

**The benefit**
The efficient use of A+W CAD Designer (Bars) requires correct settings. The software can be set to different languages during operation without a reboot.

> **Note**
> - **Dimensioning**: Can be enabled or disabled.
> - **Units of measurement**: Can display imperial or metric measurements.
> - **Changing the language**: Can be adjusted during operation.
> - **Digits, milling points, and arrows**: Can be displayed only if checkbox *Dimensioning* has been ticked.

### Showing and hiding dimensions
A+W CAD Designer (Bars) allows you to decide whether and how dimensioning shall be made.

#### How to enable dimensioning
1. Select menu *View > Settings*.
2. Dialog *Settings...* appears. Tab *Dimensioning* opens automatically.
3. Tick the checkbox **Dimensioning**.

#### Dimensioning by means of arrows
1. Select menu *View > Settings*.
2. Tick the checkbox **Dimensioning**.
3. Tick the checkbox **Arrows**.

#### How to apply digits to muntins
1. Select menu *View > Settings*.
2. Tick the checkbox **Dimensioning**.
3. Tick the checkbox **Digits at muntins**.

#### How to display milling points
1. Select menu *View > Settings*.
2. Tick the checkbox **Dimensioning**.
3. Tick the checkbox **Milling points**.

### Displaying the drill hole dimensions
You can define how sizes shall be presented. The program offers the following options:
- **Absolute drill holes**
- **Relative drill holes**

The display is always connected to the settings in section **Refer to**, where you define if dimensioning refers to the spacer or the lite.
- **Relative drill holes** require less space but provide less information.
- **Absolute drill holes** provide more detailed distance information.

### Input of sizes
A+W CAD Designer (Bars) permits to define the unit of measurement. Sizes can be shown in:
- mm
- Inches (with further options for fractions or decimals)

> **Conversion of measures**
> A+W CAD Designer (Bars) can use different measures. It is even possible to change the defined measure during operation. Existing master data will be converted in this case!

#### How to define the measure you want to use
1. Select menu *View > Settings*.
2. Dialog *Settings...* appears. Go to tab **Sizes**.
3. To use mm, activate the radio button **Size input in mm**.
4. To use inches (fractions), activate **Size input in inches (fractions)** and enter the denominator.
5. To use inches (decimals), activate **Size input in inches (decimals)** and enter the decimal accuracy.

### Choose program language
A+W CAD Designer (Bars) can be operated in seven languages. The language can be changed during operation without rebooting.

#### How to select another language
1. Select menu *View > Settings*.
2. Dialog *Settings...* appears. Go to tab **Choose language**.
3. Select the desired language from the combo box.
4. Close the dialog using [OK]. The program appears in the selected language.

## Master data in A+W CAD Designer (Bars)

**Objectives**
- Introducing different muntin types.
- Understanding differences in muntin types.
- Defining new muntins.
- Defining the standard muntin.
- Protecting master data by a password.

**The benefit**
Using A+W CAD Designer (Bars) requires defining the master data (i.e., the muntins) first.

**Definitions**

| Term | Definition |
| :--- | :--- |
| **Glass-dividing muntins** | Real muntins splitting a lite into several smaller ones. |
| **Internal muntins** | Fitted into the airspace. |
| **Fitted muntins** | Consist of integrated spacer profiles and are connected with the surface. |
| **Auxiliary muntins** | Muntins or parts thereof required to create a muntin pattern. |
| **Edge connection** | Closes the muntin and serves as a link with the surrounding spacer. |
| **Uninterrupted** | Defines continuous muntins transferred via files. |

> **Note**: Master data can be configured by the user.

### Muntin types
There are different types of muntins. Basically, we distinguish:
- Glass-dividing muntins
- Internal muntins
- Fitted muntins

#### Glass-dividing muntins
Glass-dividing muntins are real muntins. Not just one lite is set into the window frame but four or more small lites are fitted, with wooden or PVC-U muntins which form the window as such.
- **Advantages**: Stabilize the element, three-dimensional effect, can be produced up to a width of 138 mm.
- **Disadvantages**: Higher heat loss, very narrow muntins impossible, not easy to clean.

#### Internal muntins
For bigger glass surfaces, internal muntins may be ideal. They are easy to clean because of the uninterrupted surface.
- **Advantages**: Reasonably priced, lites can be cleaned easily, less heat loss.
- **Disadvantages**: No three-dimensional effect, rattling noises may occur, does not go with every kind of spacer.

#### Fitted muntins
Fitted or glued-on muntins are narrow strips of wood which are glued to the outside of the lite to make it look like a window with genuine muntins.
- **Advantages**: Very narrow muntins are feasible with a proper three-dimensional effect, less heat loss.
- **Disadvantages**: More expensive than internal muntins, rattling noises may occur, can be produced only up to a certain narrow width, not easy to clean.

### Muntins
Muntins usually come in the shape of rods (normal length 6000 mm) and can be made from different materials (Aluminium, PVC-U, Wood) in different widths, curves, and profiles.

### Auxiliary muntins
Auxiliary muntins are required for designing a muntin pattern after which they are deleted, completely or in part. For example, to create a radial pattern that ends at a curved arc muntin, the radial bars are first created to the edge of the lite, then the parts beyond the arc are marked and deleted. These deleted parts are the auxiliary muntins.

### Master data input
A+W CAD Designer (Bars)'s master data consist solely of muntin data. Open the master data editor by *Master data > Master data editor*.

#### How to enter a new muntin
1. To enter a new muntin, press [Add]. Dialog *Enter new article* appears.
2. Enter the required article number and press [OK].
3. Field *Name* will be automatically preset. You can replace this entry.
4. Enter the width of the muntin in field *Width*.
5. Enter the milling depth in field *Milling depth*.
6. Field *Offset* is for special treatment of drills with offset sizes.
7. *Edge reduction*: The connection with the spacer may use stoppers; the bar will be automatically reduced by the stopper thickness.
8. The fields *Special cross* and *Cross width* are for non-continuous, plug-in cross connections.
9. Enter the length of the muntin in field *Rod length*.
10. Field *T-allowance* is used if a bar is cut at right angles to another.
11. The radio buttons in the *Continuous* section define continuous muntins for transferred files.
12. The *Double cutting* checkbox automatically doubles the quantity for certain muntin systems (e.g., fitted muntins).
13. Enable the *L fields with reduction* checkbox to exclude edge stoppers from dimensioning.
14. The *Line number* field is for companies with several production lines.
15. Allocate a color code to the muntin in the *Color code* section.
16. The [Start] button defines the standard muntin.

### Protect master data
To keep the risk of production errors to a minimum, A+W CAD Designer (Bars) allows you to protect the master data by a password.

#### How to protect your master data by means of a password
1. Open the master data editor using *Master data > Master data editor*.
2. Tick the checkbox **Password protection**.
3. Press [OK] to close the dialog. Answer the security check by [Yes]. Dialog *Password* opens.
4. Enter the desired password in the *Password* field.
5. Repeat the password in field *1*.
6. Press [OK]. The dialogs will be closed.

### Exercises

#### Exercise 1: Entering a muntin article
**Task**: Enter a muntin article with the following specifications, set it as standard, and protect master data with a password.
- Product code: 8500
- Muntin name: Fitted muntin
- Color code: RAL 1004
- Color name: Yellow-gold
- Width: 26 mm
- Milling depth: 6.5 mm
- Trim: 3 mm
- Muntin length: 6000 mm
- Double cutting
- Password: 1111

**Solution**:
1. Open dialog *Master data editor*.
2. Press [Add], enter **8500**, press [OK].
3. Enter **Fitted muntin** in field *Name*.
4. Press [Start] to define the muntin as standard.
5. Enter **26** mm in field *Width*.
6. In field *Milling depth*, enter **6.5** mm.
7. Enter **3** mm in field *Trim*.
8. In field *Muntin length*, enter **6000** mm.
9. Tick the checkbox **Double cutting**.
10. Press [Add] in section *Color code*, enter **RAL 1004** mm, press [OK].
11. Tag the entry RAL 1004 in field *Name* and change it to **Gold-yellow**.
12. Tag the entry RAL 1004 and press [Change] to select the color.
13. Press [Start] to assign the standard color.
14. Tick the checkbox **Password protection**.
15. Press [OK], then [OK] again. Dialog *Password* opens.
16. Enter **1111** in field *Passwort*.
17. Repeat in field *Confirm* and press [OK].

## Muntins
This section shows you how to create your own muntin patterns. This is necessary if the order processing system does not transfer any data, or if you do not want to use a standard pattern.

### New designs
**Objectives**
- Understanding the process of creating new muntin patterns.
- Introduction and explanation of shape restrictions.
- Introduction and explanation of muntin patterns.
- Exchanging muntins in existing patterns.

**The benefit**: Designing the muntin patterns required by the customers.

#### General procedure
Muntin patterns are created in three steps:
1. Define the shape of the pattern
2. Define the properties
3. Position the muntins (horizontal/vertical pattern, free positioning, or macros)

#### Define the shape of the pattern
This task starts with the selection of the required pattern, the so-called shape. The selection depends on the shape catalog you are using. The *Shape input* dialog shows a parameter list (A) and a shape preview window (C).

#### Defining the lite properties
The next step is the definition of properties for the lite and order/customer data. The *Lite Properties* dialog opens automatically after the shape input. Here you define the X and Y position, alignment, order details, etc.

#### Positioning of muntins
Simple patterns consist of one or more vertical and/or horizontal muntins. The *Pattern: Vertical/horizontal* dialog helps position these automatically. Options include:
- **Identical clear fields**: Positions muntins so all fields have the same size.
- **Same drill hole distance**: Positions muntins so all drill holes have the same distance from the spacer.
- **Same drill hole distance (referring to the lite)**: Positions muntins based on drill point distances on the lite.
- **Same muntin length**: Positions muntins to have the same length.
- **Customized**: Allows for fixed values or distances to be entered manually.

#### Exchange muntin
A+W CAD Designer (Bars) permits exchanging muntins in existing patterns without creating a new pattern.
1. Tag the muntin to be replaced.
2. In menu *Edit*, open *Change article...*
3. Dialog *Master data* appears.
4. Choose the desired muntin.
5. Press [OK]. The muntin will be replaced.

### Demos and exercises
This section provides demos and exercises for creating muntin patterns.

- **Trainer demo: Explaining the shapes**: Shows different shapes and restrictions via the *Dialog Shape input*.
- **Trainer demo: Defining the lite properties**: Demonstrates necessary entries for positioning the lite via *Dialog Lite properties*.
- **Trainer demo: Adding a simple muntin pattern**: Shows how to create a simple grid pattern using *Dialog Vertical/horizontal pattern*.
- **Exercise 1: Create a design by means of a muntin pattern**: A step-by-step guide to creating a pattern with two horizontal and one vertical muntin on shape no. 65.
- **Exercise 2: Create a free pattern**: Shows how to create a free design manually using catch points and muntin tools.
- **Exercise 3: Copying a muntin pattern**: A guide to creating a more complex pattern with a sun element, using a combination of V/H pattern tools and manual cutting.

## Cutting and measuring
This section explains how to view cutting information and measure distances.

### Show cutting information
The dialog *Info > cutting info...* provides all essential cutting information for the present muntin pattern.
- It shows the lite and master data details.
- It calculates the total material quantity required.
- It lists each muntin piece (A, B, C...) with its quantity, length, start/end cutting angles, and milling points.

#### Cutting the start and end of a muntin
The sizes behind S: (start) and E: (end) show how the muntin will be cut.
- **One number** (e. g. -- 0° --): The muntin is cut at the defined angle at that end.
- **Two numbers** (e. g. 45° 0° -45°): The muntins are cut at defined angles starting from the center of the side.
- **Three numbers** (e. g. 56 22-68): The bar meets another muntin at the average angle (22°), with the outer angles for saw milling.
- **Numbers in brackets** (e. g. 68 (15,4) -22(4.1) -56(6,5)): Several muntins meet at one point; numbers in brackets define the width of each cut.

#### Milling points
Indicated by `M:` in the line, followed by the relative milling size from the start of the muntin and a direction (R for right, L for left).

### Measuring distances or lengths
The tool *Info > Measuring* measures the distance between two mouse clicks. The *Distance* dialog appears, showing Absolute, X, and Y distances.
> **Precise measuring**: Use catch points for precise measurements.

## Special patterns
This section tells you how to create and handle special patterns, house fronts, and macros.

### Creating a special pattern
A+W CAD Designer (Bars) allows positioning special patterns automatically.
1. Position a lite on the desktop.
2. Select menu *Macro > Special pattern > Special pattern*.
3. Click on the lite. The *Diamonds and rectangles...* dialog appears.
4. Choose the pattern type (Diamond or Rectangle), enter Width and Height.
5. Choose the distribution: Diamond/Rectangle-symmetrical or Muntin-symmetrical.

### House fronts
This feature allows positioning up to four lites on the desktop to give a customer an idea of a house front.
- **Define the sizes of the individual lites**: Use the *Macro > Special pattern > House front* dialog.
- **Defining the lite properties**: After defining sizes, the lite properties dialog opens for further details.
- **Demos and exercises** are provided to guide through creating and copying a house front.

## Macros
Macros are useful for frequently occurring designs. They are patterns that are created once and can be used time and again.

### General
An existing macro is loaded in the following way:
1. Define the shape of the pattern.
2. Define the lite properties.
3. Load macro.

### Load macro
Open menu *Macro > Free pattern* and click on the lite. This opens the *Select macro* dialog, which lists all available macros.

### Demos and exercises
- **Trainer demo: Explaining existing macros**: Explains how to use pre-existing macros.
- **Trainer demo: Changing an existing macro**: Shows how an existing macro can be edited.
- **Trainer demo: Create your own macro**: Shows how to create a new macro from scratch.
- **Exercises**: A series of exercises guide the user through positioning, changing, creating, and saving macros, including using reference points for precise placement.

## Data exchange
This subject area tells you how to import and export data from and to other programs.

### Data Import
If you are using A+W CAD Designer (Bars) in connection with another system (e.g. A+W Business), you need to know how to import files.

#### Transfer files
Data is imported from an order processing system. In the corresponding mode, A+W CAD Designer (Bars) imports all *.xml files at once. When imported successfully, the file is moved to an 'Archives' directory.

#### File import - New
1. Select menu *File > Import > Transfer file*.
2. The *Select - Order/item* dialog appears, listing transferred items.
3. Status *Designed* shows the record is complete. You can view patterns by tagging an item and pressing [OK].

### Data export
This includes printing/plotting patterns, cutting lists, and exporting graphics.

#### Patterns and transfer files
A true-to-scale sketch can be printed, including a list of profiles to be cut and milling angles.

#### Printer setup
Before printing, you must install the printer via *File > Printer setup...*. You can define two different printers, for example, a standard printer and a plotter.

#### Printing the patterns
Use *File > Print > Pattern* to print on the configured printers.

#### Print transfer file
This is for printing files transferred from other systems. It can be printed as a 'Transfer file' (sketch with order details) or 'Transfer file list' (cutting list).

#### Export image
A pattern can be exported as an image (JPG, BMP, PNG) via *File > Export image...*.

#### Send messages
A pattern can be emailed as an .awd file via *File > Email*. This requires the recipient to have A+W CAD Designer (Bars) installed.

## Configuration
The program is configured by the A+W team on site. If you need to change the configuration, you can access it via *Master data > Edit configuration*.
> **Changing the configuration**: You should be careful when changing the configuration. If you are not sure about the changes to be made, please check with A+W Software GmbH to avoid undesirable results!

## Annex – Macro Catalog
A+W Software GmbH provides a multitude of predefined macros to save time and effort. This section provides a list and visual examples of available macros.
- **Macro 2S2W**: 2 vertical and 2 horizontal muntins.
- **Macro 2S3W**: 2 vertical and 3 horizontal muntins, with user input for edge distance.
- **Macro 2SX4W**: 3 vertical and 4 horizontal muntins.
- **Macro Crowder**: 21 vertical and 13 horizontal muntins.
- **Macro Cumbria**: 4 diamond shapes, with user input for edge distance and diamond size.
- **Macro Diamond1**: 5 horizontal and 3 vertical muntins with 3 diamond shapes.
- **Macro Dumfries**: 4 horizontal and 4 vertical muntins in a frame pattern.
- **Macro Durham**: An octagon with connecting legs.
- **Macro Galloway**: An octagon with semi-circles and a rectangle.
- **Macro Kent1-5**: Various combinations of vertical/horizontal muntins with diamond shapes.
- **Macro Multi**: 8 horizontal and 5 vertical muntins at a fixed distance.
- **Macro NewVersi**: 5 horizontal and 5 vertical muntins.
- **Macro QueenAnn**: 5 horizontal and 3 vertical muntins with diamond shapes on the sides.
- **Macro Sun**: A semi-circle with 5 rays.
- **Macro Sun 1**: A curved muntin with 3 rays.
- **Macro York0Add1**: A vertical muntin with one diamond shape.
- **Macro York3H1S**: A horizontal and three vertical muntins with a central diamond shape.

## Z - Software Reference
This section provides detailed information on all functions, menus, and dialogs.

### Operation of A+W CAD Designer (Bars)
This section explains general terms and how to terminate the program.

#### Software terms
- **Buttons**: [OK], [Cancel], etc.
- **Hot key**: Underlined letters in menus/buttons indicate a keyboard shortcut with Alt.
- **Radio button**: Select one option from a group.
- **Combo box**: A drop-down list of options.
- **Checkbox**: Tick to enable/disable an option.
- **Tab**: Switches between different subjects in a dialog.
- **Menu bar/menu item**: The main navigation bar at the top.
- **Table/column header**: Click to sort the table data.

#### Key combinations
- **<Ctrl> + <N>**: File New
- **<Ctrl> + <O>**: Open
- **<Ctrl> + <S>**: Save
- **<Ctrl> + <A>**: Select all
- **<Ctrl> + <X>**: Cut
- **<Ctrl> + <C>**: Copy
- **<Ctrl> + <V>**: Paste

#### Terminate program
End the program by clicking the [Close] button or using *File > End*. The program will prompt you to save any unsaved changes.

### Handling of Files
The *File* menu offers options for creating, opening, saving, importing, and exporting files, as well as printing.

- **New lite**: *File > New > Icon New Lite*. Opens the *Lite properties* dialog to define a new lite.
- **Import of the transfer file**: *File > Import > Transfer file*. Shows items transferred from a superior system.
- **New lite position**: *File > Import > Transfer file > Alignment*. Used to combine items into a house front.
- **Print**: *File > Print > Construction*. Prints the current design(s).
- **Printing of Lists**: *File > Print > Transfer file list*. Prints a cutting list for transferred items.
- **Printer Setup**: *File > Print > Printer setup*. Configures printers for output.

### The Use of Tools
The *Edit* menu provides access to various tools for manipulating designs. Many of these have corresponding icons. These include Undo, Repeat, Catchpoints, Add, Copy, Rotate, Reflect, Move, and more.

### Working with Special Patterns
The *Macro* menu provides tools for creating special and predefined patterns.

- **Vertical/Horizontal Patterns**: Creates grid patterns based on various division rules.
- **Customer Defined V/H Pattern**: Allows for custom spacing of grid patterns.
- **Enter distances between muntins**: A dialog to position muntins by defining distances.
- **Diamond pattern...**: Automatically positions diamond shapes or rectangles.
- **Glass Fronts...**: Creates a house front with up to four lites.
- **Sun and stars**: Creates a radial "sun" pattern in a clear field.
- **Select Macro**: Positions a predefined macro on a lite.
- **Macro parameters**: A dialog that appears for macros requiring user input.
- **Relative distance**: A sub-dialog for entering specific values for macro parameters.

### Measuring and cutting
The *Info* menu provides tools for inspection.

- **Distance**: *Info > Measuring*. Measures the distance between two points.
- **Cutting Information**: *Info > cutting info...*. Provides a detailed breakdown of all cuts and material requirements for a pattern.

### Master data
The *Master data* menu is for managing muntin articles and colors.

- **Master data**: *Master data > Master data*. Provides an overview and allows exchanging muntins.
- **Master Data Editor**: *Master data > Master data editor*. The main dialog for adding, deleting, and modifying muntin articles, colors, and properties.
- **Password**: *Master data > Master data editor > Tick checkbox password protection*. Protects master data from unauthorized changes.

### View
The *View* menu controls the visibility of various UI elements and settings.

- **Scale up/down/Full**: Adjusts the zoom level of the design.
- **Settings**: Opens a dialog with tabs for *Dimensioning*, *Size*, and *Language Selection*.
- **Show/Hide Elements**: Toggles the visibility of Tools, Status line, catchpoints, Muntin article, etc.

### How to use the help function
- **Help topics**: Starts the help function.
- **Program information**: *Help > Info on A+W CAD Designer*. Shows version and release information.

## Help Cards
This chapter provides quick, task-oriented information for common workflows.

### Master data Help Cards
- **Bar 01-001: Tools**: An overview of the tools palette.
- **Bar 01-002: Catch points**: An overview of the catch points palette.
- **Bar 01-003: Create muntins**: Workflow for creating a new muntin article in the Master Data Editor.
- **Bar 01-004: Protect master data**: Workflow for protecting master data with a password.

### Muntins Help Cards
- **Bar 02-001: Lite properties**: Workflow for defining lite properties.
- **Bar 02-002: Position simple muntin pattern**: Workflow for creating a simple 2x2 grid pattern.
- **Bar 02-003: Positioning muntins by means of values**: Workflow for positioning muntins using fixed distance values.
- **Bar 02-004: Positioning a shape with muntins**: Workflow for adding a grid pattern to a shaped lite.
- **Bar 02-005: Creating a free muntin pattern**: Workflow for creating a complex pattern with a sun element manually.

### Special patterns Help Cards
- **Bar 03-001: Create a house front**: Workflow for positioning a multi-lite house front.
- **Bar 03-002: Load macro**: Workflow for loading and positioning an existing macro.
- **Bar 03-003: Changing and saving a macro**: Workflow for modifying an existing macro and saving the changes.
- **Bar 03-004: Create an individual macro**: Workflow for creating a new macro from scratch.
