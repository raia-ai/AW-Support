---
title: "EN-UM-AWCADDesignerShapes_1"
source: "EN-UM-AWCADDesignerShapes_1.pdf"
tags: ["A+W CAD Designer", "Shapes", "Software Manual", "Glass Processing", "Window Design", "Door Design", "CAD Software", "Technical Documentation", "User Guide", "Architectural Glass"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "User manual for A+W CAD Designer (Shapes), a 2D CAD program for designing and managing free architectural or automotive glass shapes. This guide covers basic concepts, user interface, functions, and tutorials for creating and editing geometries."
long_description: "This document is the official user manual for A+W CAD Designer (Shapes), a specialized 2D CAD software solution for the glass, window, and door industry. The manual is intended for end-users who produce shapes and processed sheets, including mirror manufacturers, automotive glass suppliers, and producers of architectural glass. It provides a comprehensive guide to the software's functionalities, from basic ideas and terminology to advanced operations. The manual is structured into several key sections: an overview, a detailed tutorial, a software reference, and a guide to the various tools. The tutorial section offers step-by-step instructions and exercises for creating and editing geometries, handling edge cut-outs, drill holes, and using macros and templates. It explains the software's user interface, the concept of different 'views' (e.g., Sketch, Geometry, Cutting, Grinding), and how to manage the entire production process from a single program. The document also covers the specific features for both architectural (AT) and automotive (ATM) glass production, detailing how to handle technical information, control machinery, and optimize production workflows. Legal notices, copyright information, and display conventions are also included."
---

# A+W CAD Designer (Shapes) Manual

## Editorial

### Revision overview of the documentation

| Date | Description |
| --- | --- |
| 10-2024 | Update of complete manual for PDF and HTML5 format. |

### Notes
This document is intended only for end users of A+W CAD Designer (Shapes).
The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.
This document describes the full scope of A+W CAD Designer (Shapes).

### Copyrights
© 2024, A+W Software GmbH all rights reserved, also those for reprinting, the making of copies and translation.
The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Display conventions
Individual elements of the sentences are displayed in a special form. The meanings are:

| Convention | Description |
| --- | --- |
| *Italics* | marks character strings describing the software elements, e.g. the *Buckets dialog*. |
| **Bold** | marks character strings to be entered via keyboard, e.g.: Enter **0**. |
| > | shows the way to open a dialog, e.g. Display > Filler orders > Context menu - List > Order overview. |
| [] | square brackets mark the buttons in the dialog, e. g. [OK] to save the data. |
| < > | pointed brackets refer to keys or shortcuts on the keyboard, e. g. <F1> is used to open the online help. |

### Contact
A+W Software GmbH
Siemensstr. 3
D-35463 Fernwald
Germany

**Tel.:** +49 641 96620 0
**E-Mail:** info@a-w.com
**Web:** http://www.a-w.com

## Overview (Module A)

### Revision overview of the module:

| Date | Change |
| --- | --- |
| 09-2020 | New tools added. |
| 07-2019 | New tools added. |
| 03-2017 | Product and company names adjusted. New tools added. |
| 06-2013 | Complete revision |
| 09-2011 | Original version |

This module provides information on the following subjects:
- Tutorial
- Software Reference
- Tools

## Tutorial

This section provides information on the following subjects:
- Overview
- Basic Ideas
- Functions
- Defining and editing of geometries
- Edge Cut-outs, Drill Holes, and Internal Contours
- Macros and Templates

### Overview

The target group for the training on A+W CAD Designer (Shapes) includes all producers of shapes and/or processed sheets, shapes for building and furniture, mirror manufacturers, automotive glass for cars and utility vehicles.

The benefit for the customer is that he can control his machinery directly. There are no down times because shapes need to be digitised for a processing machine. No NC codes have to be entered at the machine either which means that the machines can be run constantly.

#### Sets of topics
This tutorial offers the following sets of topics:
- Basic Ideas
- Functions
- Defining and editing of geometries
- Edge Cut-outs, Drill Holes, and Internal Contours
- Macros and Templates

> **Required knowledge**
> Basic knowledge of EDP or Windows are prerequisite for using A+W CAD Designer (Shapes).

### Tutorial structure
This tutorial consists of sets of topics with several sessions each. Each session consists of the following elements:

- **Overview**: Each training session starts with an overview of the major topics:
  - Objectives: What shall be conveyed?
  - Benefit: What can this knowledge be used for?
  - Maxims: Which correlations are to be remembered?
- **Concepts**: First, the concepts and terms of the corresponding training session will be explained. This is followed by examples and operating instructions.
- **Exercises**:
  - For some of the sessions, exercises with certain tasks and suggested solutions are available.
  - These exercises shall help you understand and use A+W CAD Designer (Shapes).
- **Cross references**: At the end of each learning unit there is a section with cross reference pointing out the corresponding descriptions in the software reference. This shall help you to extend your new-found knowledge.

> **Reading instructions**
> The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any learning units. If you are already familiar with a subject you should at least read the summary at the beginning of the session in order to bring the main details to mind.
>
> The practical part of each training unit automatically includes the software reference and the exercises on the cross references. This will provide a central thread through the entire documentation.

### Basic Ideas
A+W CAD Designer (Shapes) is a 2D CAD program for entering and designing free architectural or automotive glass shapes. The program allows the simultaneous management of all processing steps for a sheet.

The basic idea of A+W CAD Designer (Shapes) is that all technical information (contour, geometry, processing steps) on a sheet can be entered and edited in one program which then controls all following, technical processes.

A+W CAD Designer (Shapes) provides geometric information on the operation of the (semi-) automatic production of automotive and processed glass. It manages the data for the individual processes and supports the user in fulfilling quality requirements and process restrictions.

A+W CAD Designer (Shapes) distinguishes the properties a certain glass shall have (operator's view, e.g. edgework, drilling, etc.) and the way in which it is produced (machine operator's view). A+W CAD Designer (Shapes) creates and manages several, different views of a glass product (points on digitised contours, contour, internal contours, edgework view, printing of sketches, views for cutting and grinding machinery, etc.).

A+W CAD Designer (Shapes)'s task is to define the properties of glass products and the (separate) technological realisation of these properties using processing machinery.

A+W Software GmbH offers two versions of A+W CAD Designer (Shapes):
- A+W CAD Designer (Shapes) ATM (automotive) for automotive glass
- A+W CAD Designer (Shapes) AT (architectural) for architectural glass

#### A+W CAD Designer (Shapes) ATM (automotive)
Producers of automotive glass are faced with the challenge of transferring a three-dimensional shape to a flat sheet, then apply the necessary processing steps before transforming it into the precise, curved shape. This complex contour development starts with A+W CAD Designer (Shapes) ATM. First, two-dimensional shapes, drill hole positions, machine axes, etc. are entered in A+W CAD Designer (Shapes). For contour input, you can import 3D CAD data from the vehicle producers in IGES or VDA-FS format, and convert them automatically to show them as a smoothed 2D contour if the files match certain requirements. For details on the requirements, please contact A+W Software GmbH. For cutting or processing of automotive glass sheets, A+W CAD Designer (Shapes) considers a multitude of machine-specific restrictions or options.

#### A+W CAD Designer (Shapes) AT (architectural)
The special challenge with regard to producing architectural glass is to enter a multitude of glass structures, shapes, and processing steps quickly and correctly, depict them clearly, and add notes, drilling, and edgework. The cooperation with an order entry system working with bills of material, is of special importance here. Processing, drilling, and notches can be returned as BOM elements to order processing for pricing purposes.

**Features**
A+W CAD Designer (Shapes)'s features:
- Graphic user surface
- No separation of:
  - SHAPING (input of contours)
  - NESTING (of contours)
  - CONTOUR (input of technical drawings)
- Input of contours by
  - Digitising of patterns (templates)
  - DXF file import
  - Standard shapes
  - Dimensioned sketches
  - Construction with coordinates
- Smoothing at digitising
- 3D to 2D conversion
- NC code creation for machinery control

Dimensions are shown on the edges of the sketch and can be edited as well. Incompletely dimensioned contours will be calculated as far as possible. Internal contours can be entered easily. For digitised shapes, a standard shape with the highest resemblance can be found. The minimum block size for a shape is defined by alignment.

A+W CAD Designer (Shapes) offers functions required for many applications. Data which up to now had to be stored in various places (order entry, production control, cutting, ...) can now be handled centrally.

#### Process optimisation
A+W CAD Designer (Shapes) offers solutions on three levels:
- **At order entry:** Describing the product by means of a sketch, geometry (technical drawing), digitising, input of coordinates, and CAD data. Drilling, notches, and edgework are entered separately.
- **At production scheduling:** Separate input of technology-dependent parameters and additional information (auxiliary cuts, grinding allowances, primitive sizes, etc.) referring to the same order geometry.
- **On the shop floor:** Converting the instructions into machine-readable information, tailored to the individual processing machines (e.g. NC cutting line, NC drill, NC grinder, processing centre).

A+W CAD Designer (Shapes) manages all defined parameters and additional information and will keep them even if the geometry is changed (error correction, size amendment). This allows to create, without much work, shape catalogues for the individual products, with all the necessary parameters.

#### Surface and control elements
The user interface and control elements of A+W CAD Designer (Shapes) are based on three main requirements:
- easy to learn and operate
- extended, glass-specific functions
- step-by-step extension

A+W CAD Designer (Shapes) shows different views of the sheet, with the appropriate information. A+W CAD Designer (Shapes) offers only the tools that are practical for the view in question. The major views and corresponding tool types are:
- **Import (2D and 3D)**
  - Complete segments
  - Close contour
- **Points**
  - Import data from digitiser
  - Creating straight lines, arcs, and holes by means of points
- **Sketch**
  - Drawing of lines and arcs
  - Dimensioning of distances and angles
- **Geometry**
  - Shift points
  - Linking and splitting of segments
  - Copy contours
  - Rotate contours
  - Reflect contours
  - Double contours (create symmetrical contour)
  - Smoothing transitions
  - Cutting off or rounding of corners
- **Revision**
  - Set dimensioning points (automotive glass)
- **Inside contours**
  - Define and dimension holes
  - Define and dimension one- and two-side counter-sunk holes
  - Define and dimension cut-outs
  - Add machine axis (automotive glass)
  - Positioning of stops (automotive glass)
- **Edgework**
  - Edge definition
  - Define edge quality
  - Cut off or round commercial corners (in A+W Enterprise TAB)
- **End product: drawing (printout)**
  - Complete dimensioning
  - Complete and format text
  - Highlight details
  - Complete cut display
- **Cutting**
  - Define trim
  - Set auxiliary cuts
  - Remove cut-outs
  - Rounding and sharpening of corners
  - Define start point for machine (automotive glass)
  - Copy contours
  - Determine surrounding rectangle
- **Grinding**
  - Rounding of corners
  - Define start point for machine (automotive glass)
  - Complete dimensioning
  - Align contour
- **Drilling**
  - Define and dimension production-relevant drilling
  - Define start point for machine (automotive glass)
  - Complete dimensioning
  - Add machine axis

### Terms
The following terms have a special meaning in this document:

- **Shaping & Nesting:** Shaping is the input or creation of the contour.
  - By entering a technical drawing
  - By digitising
  - By entering coordinates
  - By importing a DXF file
- **Nesting:** (Nesting = fitting) Nesting allows to fit contours into a rectangle to waste as little space as possible (optimising space, e.g. by fitting two triangles into a rectangle).
- **Segments:** Segments are arcs or straight lines (and other types such as drilled holes) with a start and end point.
- **View:** A view is the displayed sheet with part of the available information. The Drilling view for example shows only the sizes required by the drill.
- **SN object:** A SN object (drawing) consists of the contours in different views that are tailored to the individual steps of contour input and production.
- **Drawing:** Drawing means entering a new contour. If a contour is technically dimensioned, it is entered in the Sketch view. If the contour is described by coordinates (i.e. by its corners and radii), it can be entered in the Geometry view. The view Points is used to enter a contour (sketch or shape) by means of a digitising table, point by point, and have the closed contour calculated by A+W CAD Designer (Shapes).
- **Elastic band:** An elastic band is a blue line which appears when you press the mouse key. It shows the segment to be created or serves to measure distances.
- **Manual input:** When you define new segments, you can enter the approximate sizes (by means of the elastic band). When you release the mouse key, you can enter the exact coordinates via keyboard.
- **Primitive:** The primitive is the rectangle surrounding a contour which considers the distances (trim) from the contour.
- **Tool:** A tool in A+W CAD Designer (Shapes) is any icon that can be used to modify (edit) a segment or a contour.
> **Tools - help**
> The description of tools is also available in the online help. Use Shift+F1 in menu ? to enable the context-sensitive help function. The cursor changes into a question mark preceded by an arrow. Click on the tool icon. A+W CAD Designer (Shapes) displays help text on the corresponding tool.
- **Contour:** Contours consist of (any number of) segments. When you delete to non-adjacent segments from a closed contour, you will get two contours. You can join two contours by means of the appropriate tool. Minimal inaccuracies at the joint will be corrected automatically. If things are too inaccurate, the contours will not be joined.
- **Shape:** A shape is mostly a sheet (contour) with inside contour(s). In this manual, we will mainly use the term 'contour'.
- **Properties:** Apart from the geometry, the basis of an SN object is that defined properties will be kept even if changes (of the geometry or properties) are made. Properties can be: sizes, auxiliary cuts, processing sequences, etc. Properties cannot be changed even if the basic geometry changes (in practice). You can therefore change the geometry of a contour after defining auxiliary cuts. The function of the auxiliary cuts remains valid. Only their length may change for instance. You can also change a technical drawing with all its holes and edgework, then change the sizes, and you will still get the same product, only with a different size. Properties will be kept and will be passed on to the following views.

### Functions
This subject area introduces the functions of A+W CAD Designer (Shapes).

#### A+W CAD Designer (Shapes) User Interface
**Objectives**
- Introducing the user interface of A+W CAD Designer (Shapes)
- Introducing the tools
- Introducing the input window

**Benefit**
A+W CAD Designer (Shapes) can be used to the best effect only if you are capable of applying the tools available. The better you know the A+W CAD Designer (Shapes) tools, the more efficient your work will be.

**Definitions**
- **Icon bar:** is the horizontal bar containing small buttons with symbols (icons).
- **Tools:** Tools are used to create or amend a contour.
- **Input window:** Entries can be made or changed in the input window.
- **Drawing board:** This is where the actual work with the program is done.
- **Scroll bars:** can be found at the right and at the bottom edge of the drawing board. They can be used to define the position of the marked section in the system of coordinates.
- **Tape measure:** The horizontal tape measure shows the size of the visible area in x direction. The vertical tape measure shows the size of the visible area in y direction.
- **Views:** The different views have been optimised for certain tasks and are hierarchically connected.

> **Note**
> Icon bar, tools, input windows, and BOM can be moved to any position by means of the mouse. The functions can be shown or hidden as required in menu View.
>
> When you select a tool, the cursor adopts the appearance of this tool in A+W CAD Designer (Shapes).

#### Program Presentation
We are now going to describe the user interface of A+W CAD Designer (Shapes):

The user interface is composed of the following sections:
- **A** Menu bar
- **B** Icon bar
- **C** SN Tools
- **D** Input window
- **E** Drawing board
- **F** Tab (views) for input, construction, and editing
- **G** Dialogue
- **H** Scroll bar
- **I** Horizontal tape measure
- **J** Bills of material (BOM)
- **K** Tab: Steps on the bill of material level of an IG/laminated glass unit
- **L** Tab: SN/print version
- **M** Vertical tape measure
- **N** Status line

The top section includes - from left to right - the menu bar (A) and the icon bar (B). Below these are the tools (C), the input window (D), and the bill of materials (J). The large white area is the drawing board (E). The individual views appear on top of the drawing board in the shape of tabs (F). There is a special dialogue for lines and fillings (G). On the right and below the drawing board are the scroll bars (H) and the horizontal tape measure (I). The tabs Steps (K) and SN/print version (L) are found below the drawing board. The vertical tape measure (M) appears on the left side of the drawing board. The status line (N) is shown at the bottom of the screen.

**Menu bar (A)**
All program functions are accessible by the menus and menu items. Some of the menus are directly accessible by hotkeys. These are all the menus that can be opened by one mouse-click. Each of them offers several sub-menus. If you need direct help with a certain sub-menu, enable the context-sensitive help by pressing Shift+F1 in menu ?. The cursor changes into a question mark preceded by an arrow. Click on the menu. A+W CAD Designer (Shapes) will show the help text for the corresponding menu item.

**Icon bar (B)**
The icon bar offers the functions most frequently used in menus File and Edit as well as the zoom tools and the call for program information.

**Description of the individual symbols**

| Symbol | Explanation |
| --- | --- |
| 📄 | New file. |
| 📂 | Open an existing file. |
| 💾 | Save a file. |
| 📠 | Print a file. |
| 👀 | Show side view. |
| ✂️ | Cut selection. |
| 📋 | Copy selection. |
| 📥 | Paste selection. |
| ↩️ | Undo the last action. |
| ↪️ | Restore the last, cancelled action. |
| 🔍- | Gradual scale-down. |
| 🔍+ | Gradual scale-up. |

**SN tools (C)**
The first icon on any tool bar is the cursor. Select it to terminate or abort the previous function. You can use the cursor to select contour elements (e.g. for processing, transformation).

The tool bar offers the icons of frequently used functions for the view in question. The contents of the tool bar changes depending on the selected view (product, technology). You will see only the tools that can and should be used in the present mode. The tool bar can be positioned as a separate dialogue anywhere on the screen.

When you select a tool, the arrow will be replaced by the corresponding icon. Once selected, a tool remains active in the tool bar until the corresponding function is performed, or a new tool is selected.

If a view (Sketch, geometry, edit, etc.) contains more tool icons than can be shown in the dialogue, you can go to the next page (as in a book) to display more tools.

> **Adapting the tools**
> If you need additional tools in a view, or if too many tools are displayed, you can amend the view by means of the sn.ini file (section [View]). Please contact A+W if you need help.

> **Tools - help**
> The description of tools is also available in the online help. Use Shift+F1 in menu ? to enable the context-sensitive help function. The cursor changes into a question mark preceded by an arrow. Click on the tool icon. A+W CAD Designer (Shapes) displays help text on the corresponding tool.

**Input window (D)**
This is where entries are made and changed. You can position this section as a dialogue anywhere on the screen. Black fields only show input while red fields allow to select and edit the input.

You can allocate one of the following properties to a size:
- **active:** If a size is defined as being active, A+W CAD Designer (Shapes) will use this size as a basis for creating the sketch.
- **measuring:** If a size is defined as 'measured', A+W CAD Designer (Shapes) will calculate and display the actual value. If you change the drawing, this value will change automatically. Even dimensions like *Dimension two segments parallel to each other* can be defined as 'measuring'. The corresponding icon will appear if the segments are actually parallel. If the segments are not parallel, the icon will be crossed out.
- **fixed:** If a size is defined as fixed, A+W CAD Designer (Shapes) will show the size you have entered. This value does not depend on the actual size and will not change when the drawing is amended.

If you enter sizes, you will be able to use only properties that will make sense in connection with your input.
Depending on the context, you can use this dialogue to enter segment coordinates, distances, radii, and angles.

**Drawing board (E)**
This is where the actual work with the program is done. A+W CAD Designer (Shapes) displays the contours and their properties which can be edited by the user. The drawing board is white, the segments black. S/N shows the selected segments in red, green, and grey. Red marks the segments that are currently being handled. In case of dimensions, red means that these contours will be moved to keep the required size. Green and grey are the references created for the dimensions.

**Input, construction, and processing views (F)**
Click on a view to change the display on the drawing board.

**Dialogues (G)**
Certain functions are collected in dialogues. These can be displayed or hidden.

> **Dialogues - help**
> The online help provides a description of the dialogues. Open the dialogue and press `<F1>`. SN shows the help text available for this dialogue.

**Scroll bar (H)**
The scroll bars at the right and at the bottom edge of the drawing board can be used to adjust the position of the sketched segment on the coordinate system (spanning -10 m to +10 m). The scroll bars can also be operated by mouse wheel (if applicable). The mouse wheel can be moved horizontally or vertically. If the cursor is positioned on the top right section of the page, you can scroll the mouse wheel vertically and if the cursor is in the bottom left half, you can scroll horizontally.
- **Horizontal scroll bar:** This is used to move the visible area of the drawing board in direction x. Clicking on the arrow will move the screen in small steps. Clicking on the scroll bar will move the screen in bigger steps.
- **Vertical scroll bar:** Moves the visible area of the drawing board in direction y. Clicking on the arrow will move the screen in small steps. Clicking on the scroll bar will move the screen in bigger steps.

**Horizontal tape measure (I)**
Shows the size of the visible area in direction x, in the selected unit of measurement. The tape measure serves for orientation especially in zoomed display. The first visible number also shows the unit of measurement currently used.

**BOM (J)**
The BOM dialogue shows the individual sheets that form the unit.

**Tab Step (K)**
Tab Step handles the individual BOM levels of an IG/laminated glass unit. It is not about the step offset of an IG/laminated glass unit!
These tabs at the bottom edge of the drawing board are available if you are creating a multi-stepped contour (IG, laminated glass). The tabs allow to choose block view (all sheets, Step 0) and the display of further blocks or individual sheets (Step 1 to n).
If you have created a multi-step sketch using your own BOM editor, the program will display just these steps (levels).
Steps are available only if an appropriate BOM has been created at order entry, and has been transferred to A+W CAD Designer (Shapes).

**Tab SN/print version (L)**
At the bottom the drawing board, you can choose tab S&N or Drawing. Tab S&N shows the contour on A+W CAD Designer (Shapes)'s work surface. Tab Sketch shows how the contour is going to look when printed. Tab Drawing offers a number of tools for editing the printout.

> **Tab Sketch**
> Tab Sketch is available only when the contour has been calculated and is available in the Geometry view.

**Vertical tape measure (M)**
Shows the size of the visible area in direction y, in the selected unit of measurement. The tape measure serves for orientation especially in zoomed display.

**Status line (N)**
The status line offers information on the program or on the tools. When you point the cursor on a tool, A+W CAD Designer (Shapes) briefly displays explanatory text on this tool.

#### The Concept of Views in A+W CAD Designer (Shapes)
**Objectives**
- Individual views - introduction and description
- Understanding the difference between the views

**Benefit**
The individual views offer different functions. It is therefore necessary to know what is possible, and where.

**Definitions**
- **Product-related view:** These views offer all functions and tools for entering, creating, and designing glass products.
- **Technology-related view:** These views are used to select and edit the geometry created in the Product view, depending on the technology.

> **Note**
> The different views have been optimised for certain tasks and are hierarchically connected.

#### List of views
The different views available in A+W CAD Designer (Shapes) are optimized for certain tasks and are hierarchically linked. The view tree can be customized. A+W CAD Designer (Shapes) basically distinguishes between Product-related views and Technology-related views.

**View Hierarchy:**
- **Input Views** (Top Level)
  - 2D Import
  - 3D Import
  - Points
  - Sketch
- **Geometry** (derived from Input Views)
- **Revision**
- **Inside contours**
- **Edgework** (derived from Inside contours)
- **Technology Views** (derived from Edgework)
  - Unit
    - Cut unit
      - Break out unit
    - Multiple cutting
    - Breakout
  - Cutting
  - Grinding
  - Process
  - Drilling
  - End product
    - View without print view
    - View with print view

#### Product-related views
The product-related views offer all functions and tools for defining, creating, and designing glass products. The product-related views include:
- The Points view
- The Sketch view
- The Geometry view
- The Revision view (for automotive glass only)
- The Internal contours view
- The Edgework view
- The End product view

**The Points view**
Digitising is frequently used to describe a contour. A contour is calculated (by the program) based on a more or less dense cluster of points. The source of the points cannot only be a real digitising table but also other file formats supported by A+W CAD Designer (Shapes).

The segments entered in Points are marked as points. You can click on them to check for digitising irregularities. Points can be deleted if necessary. After entering a contour, you can proceed in two ways:
- **Automatic smoothing** by A+W CAD Designer (Shapes), either with the standard method (all points are kept and are linked by arcs and straight lines in the optimum way) or via XTREAM (based on the points, the system automatically creates the optimum contour). This is the easiest and best way to handle exact patterns and entering a large number of points.
- **Linking of points by optimum segments (best fit)** and display of the maximum and average error. This allows to enter even poor patterns in an exact way; you decide how many segments are necessary in a certain area to describe the contour. Segments can be linked in different ways:
  - **Pointed corners:** By leaving a gap between the adjacent segments.
  - **Random areas:** By leaving a point between adjacent segments. SN will calculate a transition between the segments (usually no smooth transition).
  - **Smooth transitions:** By means of a tool for entering the optimum connecting arc. This method is only required after an operating error.

The entered points will be saved with the object. You can change the points later, and thus change the product (contour).

**The Sketch view**
Create your free shape on paper, as you would do by hand. The contour will not be entered true to scale, and without the exact angles. Now add dimensions to the sketch so that A+W CAD Designer (Shapes) can calculate the geometry. If you have entered a sufficient number of correct sizes, it will display the contour in the Geometry view, true to scale. It is sufficient if the sketch matches the required contour only roughly.

The Sketch view offers tools for drawing and dimensioning.

A straight line or arc is always sketched from the start point to the end point. The mouse click always marks the end of a segment. The tool *Enter new start point* allows to start a new contour anywhere. The end point of a segment automatically becomes the start point of the following segment.

> **Please make sure to close the contour!**
> Only a closed and correctly dimensioned contour can be displayed and edited in the other views, Product or Technology. Close the contour by positioning the end point of the last segment on the green circle around the contour's start point. Start point and green circle will disappear; the arrow (mouse cursor) appears automatically.

> **Please make sure to change an already dimensioned contour correctly!**
> When you open a dimensioned contour for which processing has been defined to change the sizes, please make sure to enter correct sizes. You can check this in View > New sketch. When you leave the view Sketch and the contour cannot be calculated, A+W CAD Designer (Shapes) will delete all processing steps. Use Edit > Undo to return to the previous processing step, (re)dimension the contour correctly, keeping all processing steps.

Another way of creating a contour is to import an undimensioned sketch, and enter the required sizes.

**The Geometry view**
This view shows the basic geometry of a contour. Only after a contour designed in *Sketch* has been closed and correctly dimensioned, can it be displayed true to scale in *Geometry*. This allows to check the correct dimensioning in *Sketch*.

While menu *Sketch* still shows the sketch as it has been drawn, the contour appears with the right proportions in view *Geometry*. You can change the contour in view *Geometry* (e.g. add rounded or slanted corners). Likewise, a digitised shape will appear as a contour only in *Geometry*.

View *Geometry* offers essential functions for editing the geometry. Simple, basic geometries can be designed right in the *Geometry* view by entering coordinates and radii.

**The Revision view (for automotive glass only)**
*Revision* can be used to change a sheet, step by step. You can make technical changes as well as the contours. This menu allows to:
- Split segments and add further contour points.
- Delete obsolete contour points by joining two segments.
- Change contours by shifting existing contour points.
- Change the shape in defined areas according to your wishes and requirements.
Menu *Revision* also offers powerful functions to facilitate the smoothing of digitised contours.

**The Internal contours view**
Offers various options to position cut-outs and define holes to be drilled. In A+W CAD Designer (Shapes) ATM, the sheets to be produced are aligned with the suction cups, the centre, and the stoppers of the cutting and drilling machines. The technologies (cutting, drilling, etc.) consider the properties defined in this view.

**The Edgework view**
This view offers a multitude of symbols for adding edgework to your sketches. If you define a processing step for an edge, the correct grinding allowance will be automatically added to the cutting sizes. If you have a grinding or processing machine connected, the edgework symbols will tell the machines how the individual edges shall be treated.

**The End product view**
You can use a printout of the drawing as a work order or for your order confirmation. It shows edgework, inside contours, holes to be drilled, and all sizes. You can use this view to edit your contour prior to printing:
- Enter additional instructions.
- Zoom poorly visible areas.
- Show a sectional view of counter-sunk holes.
- Show narrow sheets in a wider perspective.
- Show flat surfaces in a steep perspective.

#### Technology-related views
The technology-related views allow to select and edit the geometry defined in the Product view. This is where restrictions and additional conditions are checked and automatically calculated if necessary. These views can be used to edit the designed geometry for various processing methods.

The separation of processing and the actual processing machine has two advantages:
- A technology can be used by several machines (drilling for drills and processing machines).
- The user creates the end product (the machine program) step by step in a logical sequence without having to handle too much information at once.

Technology-related views are:
- The Cutting view
- The Grinding view
- The Drilling view
- The Processing view
- The Unit view
- The Breakout view

**The Cutting view**
When you switch to the Cutting view, A+W CAD Designer (Shapes) will display the existing contours accordingly. Segments may be omitted or replaced by others. The processing sequence is determined by the technology, but you can set it by hand by defining starting points. The Cutting view shows all geometry elements from the Edgework view. The contour of the finished product is moved outward based on the edgework allowances. The following, cutting-related amendments can be made:
- Relief cut
- Separating cut
- Distribution cut
- Sharpen corner
- Round corner
- Set starting point.

**The Grinding view**
The Grinding view shows the contour(s) from the Edgework view. At transfer to processing machinery, several programs may be created for nested individual sheets. The processing direction can be determined by selecting starting points. The following tools can be used to define grinding-related amendments:
- Set starting point
- Round corner

**The Drilling view**
The Drilling view shows the contour(s) from the Edgework view. At transfer to processing machinery, several programs may be created for nested individual sheets. You can enter more holes here.

**The Processing view**
The Processing view shows the contour(s) from the Edgework view. You can visualise the individual processing steps. A processing machine offers the functions Drilling and Grinding as well as milling.

**The Unit view**
This view has been developed for the Lenhardt TPS IG line (among others), which means the NC-controlled application of spacers in an IG unit. The spacer consists of an organic sealant which can be applied to almost any required contour. Apart from automatic edge deletion, IG lines can handle stepped IG (sheets of different sizes). Enter for example two sheets in the Geometry view and edit them as usual. View Unit is used to assemble the sheets by means of dimensioning.

**The Breakout view**
The Breakout view only shows the contour from the Cutting view with its auxiliary cuts. These tools can be used to define - automatically or manually - the breakout path for the corresponding CNC machine for cutting and breaking the glass automatically.

> **Additional information**
> are provided by the online help, accessible by `<F1>`.

#### The production process - an example
The contour is displayed in five production views:
- Edgework
- Cutting
- Grinding allowance
- Drill holes
- Process

**Example Sheet Components:**
- **A:** Cut out arc
- **B:** Drill hole
- **C:** Edge cut-out
- **D:** Internal cut-out

**Cut out arc (A)**
Sketch the outside contour complete with the corner, define the arc as a cut-out, and align it with the corner edges in the Internal contour view. The contour is cut, including the corner, while the arc is cut by a processing machine (e.g. drilling/milling machine, processing center, etc.). This is why both cuts are shown.

**Drill hole (B)**
This is where the hole to be drilled has been defined. A hole is always displayed in the same way, in every view except in *Cutting*. In the *Cutting* view, holes can be shown as crosshairs or a circle. This allows to sketch the hole at cutting, depending on the configuration.

**Edge cut-out (C)**
A cut-out has been aligned to the edge in view *Inside contour*. The cut-out can be drawn in the *Sketch* view, or added as a complete contour in the *Geometry* or *Internal contour* view. The whole contour is cut at first after which the cut-out is produced by a processing machine. This is why both cuts are shown.

**Inside cut-out (D)**
A long hole has been positioned and aligned in the *Internal contour* view. The long hole can be drawn in the *Sketch* view, or added as a complete contour in the *Geometry* or *Internal contour* view. The cut-out for the oblong is not cut, but milled after the sheet has been cut. A hole is positioned in the machinery views *Drilling* or *Editing* to drill a hole for the milling machine.

**Edgework**
This view shows the contour like in *Inside contours*. Furthermore, you can allocate individual edgework to each outside edge. The edge then shows the corresponding symbol. For example, if the basic edge is marked with the symbol X (grinding), it might result in a 2 mm grinding allowance. This means that this edge will be moved 2 mm to the outside after cutting. This allowance will be removed in the Grinding process. The *Edgework* view is one of the views that create a contour according to the customer's wishes. These views always show the sheets with their final sizes.

**Cutting**
The *Cutting* view shows no drilling, edge-, corner- and inside cut-outs. If drilling is displayed (as crosshairs), this will be cut only as an option.

**Grinding allowance**
This view serves to define the exact cutting lines for the contour. The primitive from which the contour is cut, is shown as a broken line. Please note the corrected sizes resulting from the defined edgework, which will cause a cutting allowance.

**Backcut for trim**
A zoomed view might show that a cut ends slightly before the outside edge. This is necessary because of the breakout properties of glass. Otherwise, this cut might go through to the adjacent sheets, or break the glass prematurely.

**Drill holes**
Drilled holes can be marked in the production process *Cutting* (adjustable) by a cross smaller than the hole diameter, or by a circle.

**Grinding**
This view shows the contour as it would look after grinding. Only the segments relevant for grinding will be displayed (no inside contours). The contour has already been cut, the bottom edge has been reduced by the allowance to the size ordered by the customer.

**Drilling**
The *Drilling* view shows the entire contour. Unlike the *Cutting* view, it shows the actual sizes (grinding allowances have already been removed). Holes appear with their entire contour and all data. Drill holes may be added to an internal cut-out (long hole) in this view, meaning the inside cut-out will be drilled before milling.

**Process**
The *Processing* view shows the work steps required for the processing machine. This includes edging and milling. This is why the grinding allowance (for edgework) and the oblong as well as other inside contours are displayed.

> **The long hole can be milled and drilled!**
> With a processing machine, the long hole can be created by connecting two drill holes, or by milling it.
> - **Milled oblong:** At least one hole has to exist for milling so that the milling machine can penetrate the sheet.
> - **Oblong drilled and milled:** Even if you define two holes, you have to remove (mill) the remaining material.

> **Additional information**
> are provided by the online help, accessible by `<F1>`.

### Defining and editing of geometries
This section explains how geometries are defined and edited in A+W CAD Designer (Shapes).
This includes the following objectives:
- Sketching the shape
- Dimensioning the sketched shape
- Exercises

#### Creation and dimensioning of sketches
**Objectives**
- Learn the correct use of the tools in the *Sketch* view
- Creation of sketches
- Learn the correct use of the tools in the *Geometry*, *Internal contours*, and *Edgework* views
- Dimensioning of sketches
- Check your entries

**Benefit**
You will be able to use A+W CAD Designer (Shapes) efficiently only if you are familiar with the process and the tools.

**Definition**
- **Sketch:** This view is used to create a rough draft.
- **Reference line:** means the line with which dimensions are aligned, vertically or horizontally.

**Note**
- **Starting point:** Drawing always starts from a certain point, the starting point.
- **Reference line:** means the line with which dimensions are aligned, vertically or horizontally.
- **Curvature spread:** Please extend the arc only as far as necessary to avoid misinterpretations.
- **Close contour:** Please make sure to close the contour. Only a closed and correctly dimensioned contour can be displayed and edited in the other views.
- **Tools:** The description of tools is also available in the online help. Click on the tool icon and press `<F1>`. SN shows the help available for this tool.

#### Sketching the shape
In the first step, sketch the shape as you would do by hand on a piece of paper. This is done in the *Sketch* view. You do not have to draw the contour true to scale or with the proper angles. A straight line is sketched with the tool *New straight line*. To draw an arc, use the tool *New arc*.

**The starting point**
Drawing always starts from a certain point, the so-called starting point. By default, the starting point is the coordinate 0:0. You can position the starting point in any free space however. Setting out from the starting point, create a closed sequence of segments. In a closed contour, the last segments ends at the starting point.

**Tools for drawing straight lines and arcs**
A+W CAD Designer (Shapes) offers tools for drawing straight lines and arcs. Select *Straight line* or *Arc* and click the mouse to create the corresponding segment. The mouse click always marks the end of a segment. The end point of a segment automatically becomes the start point of the following segment.

> **Please make sure to close the contour!**
> Only a closed and correctly dimensioned contour can be displayed and edited in the other views, *Product* or *Technology*. Close the contour by positioning the end point of the last segment on the green circle around the contour's start point. Start point and green circle will disappear; the arrow (mouse cursor) appears automatically.

**How to enter a new straight line**
1. Choose the tool. Click on the corresponding icon.
2. Position the cursor at the point that shall become the end point of the line.
3. Press the left mouse key. A - preliminary - line now links the starting point with the end point.
4. To create the final straight line, press `<ENTER>` or [OK].
5. Another way of creating the final segment is drawing the next straight or arc segment.
6. When you position the mouse, and keep pressing the left mouse key, the actual coordinates are constantly displayed. Release the mouse key to draw the preliminary line.

**How to enter a new arc**
1. Choose the tool. Click on the corresponding icon.
2. Position the cursor and keep pressing the left mouse key. A+W CAD Designer (Shapes) constantly shows the actual coordinates and length.
3. Release the left mouse key when you have reached the required end point. A+W CAD Designer (Shapes) shows the chord as an auxiliary line (blue). Starting and end point of the arc are fixed.
4. Click on the chord and draw it into the required direction; keep pressing the mouse key. Release the mouse key when you have reached the desired radius. The radius is shown in the input field. The arc preliminarily appears as a continuous line.
5. To create the final arc segment, press `<ENTER>` or [OK].

> **Direction of the curve**
> When entering an arc, it is essential to be aware of the direction of the curve. It defines the direction of the radius later on.

> **Curvature spread**
> Please extend the arc only as far as necessary to avoid misinterpretations on Shaping & Nesting's part.

> **Tools - help**
> The description of tools is also available in the online help. Use Shift+F1 in menu ? to enable the context-sensitive help function. The cursor changes into a question mark preceded by an arrow. Click on the tool icon. A+W CAD Designer (Shapes) displays help text on the corresponding tool.

#### Dimensioning the sketched shape
When you have sketched the rough draft, dimensions have to be added to the individual segments so that A+W CAD Designer (Shapes) can calculate the geometry.

**Basics of dimensioning**
To find the correct tool for dimensioning any sketch, answer the following three questions:
1. Which line is the reference line for this sketch?
2. Is the corresponding size vertical or horizontal with the reference line?
3. Is the reference line involved?

**1. Which line is the reference line for this sketch?**
The reference line is the edge the sizes refer to. Some distancing tools require that you click on this line to inform the tool about how the sizes shall be aligned. The reference line defines how the displayed sizes shall be aligned to the reference edge. The reference line is the line with which dimensions are aligned, vertically or horizontally.

**2. Is the corresponding size vertical or horizontal with the reference line?**
This question helps determine which dimensioning tool to use, as tools are specific to horizontal or vertical measurements relative to the reference line.

**3. Is the reference line involved?**
This question clarifies whether the dimension is being applied directly to the reference line itself or between the reference line and another point/line.

#### Tools for dimensioning
A+W CAD Designer (Shapes) offers special tools for dimensioning. The icon shows which points and segments have to be tagged, and the resulting size type.

| Measurement Type | Vertical from reference line | Horizontal from reference line |
| --- | --- | --- |
| Point to Line | D | P |
| Point to Point | D | P |

If a tool requires clicking on two points, the program distinguishes the sequence. The first point is always red and the second, green. Based on the sizes entered for the green segment, the red segment will be adapted accordingly.

> **Clicking on the right point**
> Always click on the second half (seen from the starting point) of the reference line, or line to be dimensioned. Otherwise, A+W CAD Designer (Shapes) will fail to accept that the size belongs to the line in question.
