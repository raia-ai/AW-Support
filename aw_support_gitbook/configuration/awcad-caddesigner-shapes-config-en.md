---
description: "EN-CONFIG-AW_CAD_Designer_Shapes"
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

