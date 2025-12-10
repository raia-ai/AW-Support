---
title: "EN-CONFIG-AW_Enterprise_6"
source: "EN-CONFIG-AW_Enterprise_6.pdf"
tags: ["A+W Enterprise", "Software Configuration", "Glass Manufacturing", "BOM", "iTOE Rules", "Environment Variables", "Technical Documentation", "Order Processing", "Release Pool", "Limit Check"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical configuration guide for the A+W Enterprise software, detailing rules for processing laminated glass (LAMI), inheritance logic for bill of materials (BOM), iTOE (interface to external systems) rules, and various environment variables that control system behavior. It covers specific configurations for drilling, edge polishing, order release procedures, and customer limit checks."
long_description: "This document is an excerpt from a comprehensive configuration manual for A+W Enterprise, a specialized software solution for the glass manufacturing industry. It provides in-depth guidance on configuring specific processes related to laminated (LAMI), tempered (TG), and insulated (IG) glass units. A significant portion is dedicated to defining 'inheritance' rules, which dictate how processing steps (like drilling or polishing) applied to a composite product (e.g., a LAMI unit) are managed in relation to its individual components (lites). This includes both passing processes down to sub-components and inheriting them upward for pricing or flagging. The guide extensively details the setup for different processing types, such as stepped and countersunk drilling, using iTOE (Interface To External Systems) exchange rules. It is rich with practical examples, including screenshots from the A+W CAD Designer and various configuration dialogs. Furthermore, the document serves as a reference for numerous environment variables that control system behavior, such as 'INTAUF_BEARBCOPY_BA_HALTEN', 'VBEA_KUNR', and others affecting order processing, limit checks, and the automatic generation of text for production documents. It also explains the functionality of the 'Release Pool,' where orders are held for review, and the 'Limit Check' feature for managing customer credit."
---

| | | | |
| :--- | :--- | :--- | :--- |
| 150 | 1 | 499003 | 399003 Senkbohrung |
| 150 | 2 | 499003 | 399005 Bohrung 4-20mm DurchmesserET |
| 100 | 1 | 499003 | 199003 Senkbohrung |
| 100 | 2 | 499003 | 199002 Bohrung bis 10mm Durchmesser |
| 100 | 3 | 499003 | 199003 Senkbohrung |
| 110 | 1 | 499003 | 199003 Senkbohrung |
| 110 | 2 | 499003 | 199002 Bohrung bis 10mm Durchmesser |
**Figure: Rules with indication of glass number**

Here, by entering the glass number, you can enter various articles for the inheritance that are determined by the left/top parameter of the countersunk drilling (D+D1+angle top +depth top) (glass = 1), the part that should eventually be taken over as drilling (glass = 2) and as countersunk drilling, which are determined by the right/bottom parameters of the countersunk drilling (D+D2+angle bottom and + depth bottom) (glass = 3). The inputs for glass number = 3 are not absolutely necessary if it is the same article as the countersunk drilling for glass number = 1.

This rule does not mean that for glass=1 that the countersunk drilling is always exchanged in for LAMI, but only if both diameters (and depth top) is specified for this side. If the input for the sinking on the side is missing, then the rule for glass = 2 (drilling) is applied. The same also applies for 2nd glass. If the sink depth is greater than for the previous glass, then for the 2nd depth, the rule for the countersunk drilling is also applied.

Maintenance of the master data is only possible if the switch VBEA_KUNR is active and as value contains the number of a pseudo customer. Only then can you maintain the master data.

Because it depends on diameter/depth which processings are inherited, the functionality from the background process was taken over in the foreground. Intaufart -22 (BOM structure) for the foreground entry of orders is omitted.

The inheritance starts if you insert an inheritable LAMI processing in the BOM manually or via ITOE. If in ITOE the processing is only distributed to individual lites, the processings will come separately for individual lites and are not linked with one another in the AW Enterprise BOM.

If the LAMI processing was inherited, then it is marked on the BOM dialog and also on the processing dialog and the parameters cannot be changed.

---
## 37.4.7. Environment variables

### INTAUF_BEARBCOPY_BA_HALTEN (client reference: no)
If the system has been configured so that distribution defines how laminated glass is going to be produced and/or processed, you can now pass on these decisions for inherited processings via site.

If the switch is active, the processing steps marked as 'can be passed on' in master data will adopt the processing type from distribution instead of loading it from the production site's master data as for all other elements.

### INTAUF_VSGLM_BA_HALTEN (client reference: no)
If it is already decided in the trade whether LAMI SD is produced or comes from stock, this decision can be passed on to production.

If this switch is active, the processing steps marked as 'can be passed on' in master data will adopt the processing type from distribution instead of loading it from the production site's master data as for all other elements.

### ORDERXML_IGNORIERE_BEARB_BESTELLKZO (client reference: no)
In the standard system, the OrderXML service transfers all BOM processing to the OrderXML file. This switch can be set if you want to ignore the processing of the BOM. Then it is sufficient in the A+W Enterprise BOM to set the procurement type of the processing concerned to "None", and the processing is not taken over.

### VBEA_KUNR (client reference : no)
The customer number for E/A for the inherited processing is defined in the variable. Also activates the possibility to create one.

Otherwise is always applies that: the same article as in the header is inherited.

### VSG_VERERBEN_MIT_DRUCKKZ (client reference: no)
Switch for intauf. Novak. For inheritance of the processing from LAMI, DRUCK-KZ is set for the sub-elements according to BA.

If BA=PROD, then druckkz = P (inheritance without iTOE)

AWDesk 451313: complete description

## 37.5. Definition of the iTOE rules for inheritance upward
This section describes which parameters a SN file must contain for the entry so that the ITOW rules take effect. This section will describe how you must define the iTOE rules so that they take effect.

**Package processing:** processing on header article or on the LAMI after combination. For example, a drilling in LAMI, edges polished on LAMI. The individual lites of the LAMI are not drilled before the combination of the LAMI. Only possible if the LAMI does not contain any TG. This processing is not inherited upward or downward in AWE.

**Individual processing:** processing on the individual lites of the LAMI before combination. For example, a drilling in both TGs. This processing is inherited upward in AWE for prices and print flag.

These examples are subdivided into:
*   Part 1 for normal processing such as edge processing, normal drilling and notches
*   Part 2 for stepped drilling
*   Part 3 for countersunk drilling

### 37.5.1. Part 1 - for normal processing such as edge processing, normal drilling and notches

**LAMI with 2xFloat – package processing**

How you must define an edge processing, drilling, section if this is a package processing.
For this processing, the following level must be activated in the SN file:

| Titel | Wert | In |
| :--- | :--- | :--- |
| 0 | ☑ | |
| 1 | | |
| 2 | | |
**Figure 79: Excerption from A+W CAD Designer (Shapes)**

The processing should not be inherited downward in AWE, so LAMI/CR inheritance must be set to 'N' in the article master data.

In the iTOE rules in order to find the article for header articles, the system searches by product type = 170 LAMI article FD and intermediate level art-type empty.

Example for edge processing polishing (A+W processing type = 1010):
