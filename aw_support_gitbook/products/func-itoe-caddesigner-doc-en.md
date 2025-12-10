---
description: "A+W Business - iTOE Functional Description"
---


# A+W Functional Description
---
## A+W Business - iTOE

A+W - Software for Glass

---

## 2. Notes on this document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. Third party copyrights must be observed.

### 2.2. Copyrights

© 2021, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions that have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| Product | A+W Business / A+W Business Pro |
| :--- | :--- |
| **Module number** | 210019 / 230019 |
| **Module** | iTOE |
| **Brief description** | Integrated CAD in A+W Business |
| **Available** | Starting with A+W Business v6 (13.04.0637); A+W CAD Designer (Shapes) v6 |

### 3.2. Description

The goal of the technical order entry with iTOE is to be able to enter geometries and processing both in the A+W Business order entry as well as in A+W CAD Designer (Shapes) and if possible, to receive a harmonized BOM.

In the iTOE, the A+W CAD Designer (Shapes) is integrated into the order/quotation entry in A+W Business. This enables:

- The entry and import of geometric data with the help of the A+W CAD Designer (Shapes).
- The generation of geometric data (SN files) from the A+W Business order data.
- The harmonization of information between the two systems.

The standard processing and geometry entry in A+W Business enables the input and visualization of standard shapes and standard processings in the sense of the shape catalog and the A+W standard processing type catalog. The iTOE also offers support for free shapes and non-standard processings.

### 3.3. Requirements

- A license for the A+W CAD Designer (Shapes) is required. Depending on the desired functionality in the CAD (e.g. DXF import), it may be necessary to license additional options.
- The user must be trained in the operation of the CAD.
- A+W Business Version 6 (13.04.0637) is assumed.
- Module 159 has to be released in A+W Business.
- The use of the A+W processing type catalog is assumed (described below as STD processing).
- In this document there is a distinction between STD shapes (shapes from the A+W shape catalog) and free shapes. Other catalogs are not currently supported.

### 3.4. List of functions

- The entry of STD geometries and STD processings in A+W Business with subsequent further processing in the A+W CAD Designer (Shapes).
- Assignment of existing SN files to order items with subsequent comparison of the STD geometries and processings in the A+W Business BOM.
- In the A+W CAD Designer (Shapes), STD geometries and STD processings can be added and changed and returned to A+W Business. Here, new STD processings are added to the A+W Business BOM, removed processings are deleted, and changed processings adjusted. Here, it is not absolutely necessary to save a SN file and link it with the item.
- For the geometric entry of processings in the A+W CAD Designer (Shapes) there are also other input possibilities. (e.g. dimensioning via chain dimensions)
- If the file is saved, the following information can also be stored there:
    - Change of the display (additional or changed dimensions, additional text, etc.)
    - Technological changes (adjustment for cutting or the processing centers)
- In particular, via A+W CAD Designer (Shapes), geometric data that describes free shapes can be incorporated (e.g. via the DXF import).
- DXF files can be imported directly into A+W Business and there is an immediate synchronization of the BOM.
- On the A+W CAD Designer (Shapes) menu, it is possible to select whether or not an SN file is stored in the item. Insofar as no CAD-specific additions to the sketch are made, this may not be necessary. Insofar as changes were made in the CAD that cannot be stored in the A+W Business BOM (e.g. chain dimensions of drillings, etc.), the SN file should be transferred.

### 3.5. Restrictions

#### 3.5.1. General

When calling the iTOW from the processing entry, the complete glass structure is transferred to the A+W CAD Designer (Shapes). Any existing *.SN file is considered here and also transferred. After the processing in the A+W CAD Designer (Shapes), the user can choose whether or not an SN file should be created in A+W Business. If changes were made in A+W CAD Designer (Shapes) that could not be mapped in the A+W Business BOM (e.g. chain dimensions), the user should always select transfer with SN file to prevent losing any data.

Directly after transferring the sketch to A+W Business, the import dialog is displayed with all detected processings. Here, the article mapping can be added or taken over. As soon as changes are made to the mapping here, there is a new analysis of the processings. After the confirmation, the BOM is transferred to A+W Business according to the article assignments.

There is also still shape detection during the synchronization. If an A+W standard shape is detected, the user can change to the shape detected.

Additional processings can be added in the A+W CAD Designer (Shapes) and transferred to A+W Business.

In A+W Business, processings added will be added to the SN file, insofar as they were dimensioned absolutely (with respect to the circumscribing rectangle).

A change of the processing parameters in A+W Business is also possible. Such a change also means that the corresponding parameter change will be made via the iTOE in the SN file.

Edge processing can be reported back from the A+W CAD Designer (Shapes) to the A+W Business BOM if all edges of the shape should be processed. Here, several edge processings are also possible assuming that all edges are always processed.

**Processings that cannot be mapped to A+W standard types**

These processings cannot be transferred back to A+W Business. Here it is necessary to save the SN file and link it with the item.

In general, in A+W Business, you must add this processing to the BOM manually (price calculation, production planning). This processing may not have any assignment to an A+W processing type, otherwise it would be added to the SN file if necessary.

**Macros (also parametric macros)**

The addition of processing macros to A+W CAD Designer (Shapes) means that macros are resolved into their individual processings and these are reported back to A+W Business.

However, if the macro is entered in A+W Business, it can be retained. In this state, however, no change should be made to the processings assigned to the macro in the A+W CAD Designer (Shapes).

**Shape change for items with link to a SN file**

In the A+W CAD Designer (Shapes) it is possible to change the associated geometry and to perform a new shape detection, which means that a new A+W shape can arise. This shape change is then reported back to A+W Business, whereby the shape parameters are synchronized appropriately in A+W Business.

**Shapes whose number of segments deviate from the number of XOPT edges**

Shapes with a different number of segments in the A+W CAD Designer (Shapes) in comparison to the number of edges in A+W Business cannot currently be mapped. Affected by this are the shapes 60, 61, 62, 63, 74, 75, 78, 81, 123, 124, 125, 133

**DXF-Import**

The import DXF data is performed as usual. Then, however, the BOMs are synchronized. The DXF file is examined and the BOM is created in A+W Business using the article mapping, analogous to the synchronization with the A+W CAD Designer (Shapes).

**Step changes**

Step changes in iTOE are not yet supported.

**Ordered subparts for items with SN file**

If an order item contains an ordered subpart and a SN file was attached to the item, then this file is also taken over into the order item for the subpart. The SN file still contains the glass structure of the entire order item and not just of the ordered item. From this it follows that in the SN file (through inheritance from the header part), processings can be contained on the ordered glass (e.g. drillings) that should not be made. When printing out the order via the A+W Enterprise Print Service, the CAD sketch is also printed according to the attached SN file.

#### 3.5.2. A+W CAD Designer (Shapes)

A+W CAD Designer (Shapes) offers a relatively great degree of freedom for the generation and changing of shapes. In the course of the iTOE, in particular the geometry, inner contours, and edge processing views must be used according to their definition. The data for the reporting to A+W Business is gained from these views. This way of working will be explained through the standard configuration of the tools in the A+W CAD Designer (Shapes). For combined products (IG, LAMI), the processings must be done on the header part. If a processing refers to a subpart, this must be stored in the BOM of the corresponding processing. This is also the standard procedure, with which an appropriately trained user should be familiar. Changes on the level of the subparts are possible, however they will not be reported back to the A+W Business.

### 3.6. Notes

(This section is empty in the source document.)

---

## 4. Contact Address

**A+W Software GmbH**

Siemensstraße 3
35463 Fernwald
Germany

**Tel.** +49 641 96620-0

**E-mail:** info@a-w.com
**Internet:** http://www.a-w.com/
