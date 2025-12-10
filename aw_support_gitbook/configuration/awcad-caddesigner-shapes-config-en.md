---
title: "EN-CONFIG-AW_CAD_Designer_Shapes"
source: "EN-CONFIG-AW_CAD_Designer_Shapes.pdf"
tags: ["A+W", "CAD Designer", "Shapes", "Configuration", "SN.INI", "Drawing Configurator", "Profile View", "Software for Glass", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "An internal configuration guide for the A+W CAD Designer (Shapes) software. This document details how to configure the software using the SN.INI file, including adding tools to views, using the Drawing Configurator for layout adjustments, and setting up the Profile View feature."
long_description: "This document serves as a technical configuration guide for the A+W CAD Designer (Shapes) application, specifically for internal use. It provides instructions on how to customize the software's behavior and appearance. The guide focuses on modifications made through the `SN.INI` configuration file. Key topics covered include the 'General Information' section, which explains how to add extra tools to different views within the application. The 'Drawing Configurator' section introduces a dedicated tool for modifying the layout of SN drawings, explaining its location and usage, with a warning to back up configurations. Finally, the 'Profile View' section details the extensive set of parameters available in the `[Picture]` section of the `SN.INI` file to control the display of a unit's profile view, covering aspects like size, position, appearance, and the visibility of specific features such as drillings, coatings, and miters. The document is intended for technicians and developers responsible for setting up and maintaining the A+W CAD Designer software."
---

# A+W Configuration
# A+W CAD Designer (Shapes)

**- INTERNAL -**

**A+W - Software for Glass**

---

---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2018-09-11 | Dirk Langwald | Original version | 1.0 |

---

## Content

1.  **General information** - 4
    1.1. Tools - 4
2.  **Drawing Configurator** - 5
3.  **Profile View** - 6
4.  **Table of Figures** - 8

---

## 1. General information

A+W CAD Designer Shapes is largely configured with the configuration file **SN.INI**. A description of the individual switches is here:
`\\jupiter\Doku_DocuWare\Shaping_Nesting\!General\Installation_Configuration\SNINI_XML_Doku\SNINI-Doku.xml`

Other important documentation is the manual that can be reached in the application directly via the ? menu.

### 1.1. Tools

In A+W CAD Designer (Shapes) there are many tools for recording and processings. Each view has a default selection of tools. If additional tools are required in a view, they can be added via the configuration file. For this, in the **[View]** section, there is an individual switch for each view: **<Name of the view>additionalTools**

The tools are assigned to the parameter in a list separated by spaces:

**Example:**
`GEOMETRYadditionalTools = JOINSHP RoundEdge RndAll CUTCORNR`

A list of the available tools and their application is in the manual.

