---
title: "EN-FUNC-AW_Shape_Optimizer"
source: "EN-FUNC-AW_Shape_Optimizer.pdf"
tags: ["A+W", "Shape Optimizer", "Glass Manufacturing", "Software", "Functional Description", "Nesting", "Optimization", "Production", "Glass Cutting"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a functional description for the A+W Shape Optimizer, an add-on module for A+W's glass manufacturing software suite. It details how the software combines standard shapes to minimize waste and improve glass usage. The document covers its performance, requirements, functions, limitations, and provides contact information for A+W Software GmbH."
long_description: "This is a comprehensive functional description of the A+W Shape Optimizer, a software module designed to enhance glass cutting and production processes. The document is intended for users of A+W's software suite, including A+W Business Pro, A+W Production, A+W Realtime Optimizer, and A+W Standard Optimizer. It explains that the Shape Optimizer is an add-on module that intelligently combines two standard shapes into the smallest possible surrounding rectangle, improving material yield. The description outlines the technical requirements for implementation, such as specific parameter settings in the A+W Optimization configuration. It lists key functions, including automatic setting of trims and auxiliary cuts, placement of triangles, and pre-selection of the best results to save optimization time. The document also clearly states the limitations of the software, such as only combining two convex shapes at a time, not supporting shapes with circular arcs, and other specific restrictions. An example is provided to illustrate the efficiency gains, showing how the optimizer can fit more shapes onto a stock plate compared to previous methods. Finally, the document includes legal disclaimers, copyright information, and contact details for A+W Software GmbH."
---

# A+W Functional Description: A+W Shape Optimizer

**A+W - Software for Glass**

---

## 1. Content

1.  **Content**
2.  **Notes on this Document**
    - 2.1. Trademarks
    - 2.2. Copyrights
    - 2.3. Disclaimer of liability
3.  **Performance Description**
    - 3.1. Data
    - 3.2. Description
    - 3.3. Requirements
    - 3.4. List of functions
    - 3.5. Limitations
    - 3.6. Notes
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2018, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| Product | A+W Business Pro, A+W Production, A+W Realtime Optimizer, A+W Standard Optimizer |
| :--- | :--- |
| **Module number** | 220015, 220018, 220910, 230115 |
| **Module** | A+W Shape Optimizer |
| **Brief description** | Add-on module in the optimization for combining shapes |
| **Available** | From version 5 |

### 3.2. Description

The A+W Shape Optimizer combines two A+W standard shapes so that as small a rectangle as possible is created surrounding both shapes. Here if necessary auxiliary cuts and break edges and/or a certain distance is added between the two standard shapes. It is possible that the shapes are turned and rotated to improve the result. The sequence restriction is adhered to here, of course.

### 3.3. Requirements

The A+W Shape Optimizer is provided with A+W Optimization and requires this. In the configuration file of the optimization, there are some parameters that must be adjusted for the A+W Shape Optimizer:

- Angle between 2 segments in order to detect whether an auxiliary cut or trim is required.
- Trim size and thus also the auxiliary cut length
- Maximum height and width of the circumscribing rectangle
- Detection of a limit angle in degrees around a right triangle.
- The maximum size of a rectangular sheet that may be combined with a shape if necessary.

Since the A+W Shape Optimizer acts automatically in the background, no training is required for its use.

### 3.4. List of functions

The A+W Shape Optimizer replaces the standard combination of most catalog shapes completely (currently shapes that contain circular arcs are not supported). It results in better glass usage since a wide variety of shapes can be combined.
The A+W Shape Optimizer forms an optimization of all shapes using combinations of two shapes that utilize the glass better than the shapes individually. The combinations formed this way are then optimized in the rectangular optimization. Depending on the sequence restrictions and ability to combine the shapes, more or fewer shapes are processed this way.

In addition to the main function of combining two shapes, the algorithm includes the following functions:

- Automatic setting of the trims and auxiliary cuts
- Automatic setting of a distance to the common edge of the shapes, so that the shapes are not on an edge and the breakage is made easier.
- Placing of triangles in the free space or of a trapezoid or another square
- Automatic turning of nearly right triangles so that the right angle lies on the base side. Thus the result is better, for the right angle could be at the top point of the triangle.
- Automatic turning of triangles onto the longest side.
- Automatic pre-selection of the best results if the number of results becomes too large. This saves time for the optimization since the number of shapes to be optimized is reduced.
- Use possibility of turning and rotating for shapes and thus achieve a better result.
- Edge deletion of the individual shapes, insofar as the cutting code driver supports this.

### 3.5. Limitations

- Only 2 shapes are combined
- Only shapes from the A+W catalog
- Only convex shapes are combined; no concave ones (concave shapes have a bend to the inside)
  
  *[Image: Diagram showing a concave shape (Konkave Form) and a convex shape (Konvexe Form). The concave shape has an inward-facing angle, while the convex shape has all outward-facing angles.]*

- Rotating and turning of the shapes is only possible if the glass type permits this (coated glass, directional glass)
- No shapes with circular arcs
- No shape 99 or 98
- No shapes with more than 5 edges
- No shapes that are already combined (factor shapes). If a factor shape or two triangles are combined, the number of items is already divided by two in A+W Production and the shape is replaced by the combined shape. The number of sheets per item must therefore be even and >=2.
- No surface decoating

### 3.6. Notes

New feature since 2016: Two shapes may not be placed in the smallest circumscribing rectangle if with this more sheets fit on a plate.

**Example:** 100 triangles on the same side with a side length of 2400 mm should be produced. This is shape 20 in the A+W shape catalog. Previously 3 of these triangles were placed on a jumbo:

**Previous Method:**
- **Article:** Float 4
- **Pattern:** 1/2
- **Sheet Size:** 6000x3210
- **Result:** 66.44%
- **Description:** An image shows a large sheet with three triangles placed. Two triangles are combined to form a rectangle, and a third triangle is placed next to them, resulting in significant waste. The pieces are labeled `1 #1`, `1 #2`, and `1 #3`, with dimensions `2400` x `2079`.

**With the new feature, now 4 of these triangles fit on a stock plate:**

**New Feature Method:**
- **Pattern:** 1/25
- **Sheet Size:** 6000x3210
- **Result:** 94.77%
- **Description:** An image shows the same large sheet, but now it is cut into two large rectangular sections. Each section contains two triangles (`2 #1` and `2 #2` in one, `2 #3` and `2 #4` in the other) perfectly combined to fill the rectangular space with minimal waste. Each piece has dimensions `2400` x `2079`. This method fits 4 triangles on the plate.

---

## 4. Contact Address

**A+W Software GmbH**

Siemensstraße 3
35463 Fernwald
Germany

**Tel.** +49 641 96620-0

**E-mail:** info@a-w.com
**Internet:** http://www.a-w.com/
