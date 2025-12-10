---
title: "EN FUNC A+W Enterprise iTOE"
category: "functional_descriptions"
product: "A+W Enterprise iTOE"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Enterprise iTOE"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Enterprise - iTOE                                   english 1. Contents 1.   Contents                                                          3 2.   Notes on this Document                                            4      2.1. Trademarks                                                   4      2.2. Copyrights                                                   4      2.3. Exclusion of liability                                       4 3.   Performance Descriptio"
source_file: "EN-FUNC-A+W Enterprise iTOE.pdf"
---


# EN FUNC A+W Enterprise iTOE

     Functional Description


A+W Enterprise - iTOE




                              english
1. Contents
1.   Contents                                                          3
2.   Notes on this Document                                            4
     2.1. Trademarks                                                   4
     2.2. Copyrights                                                   4
     2.3. Exclusion of liability                                       4
3.   Performance Description                                           5
     3.1. Data                                                         5
     3.2. Description                                                  5
     3.3. Requirements                                                 5
     3.4. List of functions                                            6
     3.5. Limitations                                                  7
          3.5.1. General                                               7
          3.5.2. CAD                                                   8
     3.6. Notes                                                        9
4.   Contact Address                                                  10




A+W Software GmbH                  EN-FUNC-A+W Enterprise iTOE.DOCX        3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The greatest care was used in
compiling the texts and figures. However it is not possible to exclude errors completely. A+W
Software GmbH assumes no liability for errors or imprecise statements unless these can be traced
back to intentional or negligent actions.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2015, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation may only be copied whole or in part, stored in an archiving
system or transmitted in any other form in accordance with the license agreement. The
documentation may not be transmitted electronically, by recording or in any other form without
the prior written permission of A+W Software GmbH.


2.3. Exclusion of liability
A+W Software GmbH assumes no liability for data errors that rely on basic principles of the
standard functions made available by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All adjustments, expansions, database
queries, reports, analyses, and interface expansions that were created individually for our
customers and/or machines and software partners as well as all costs and efforts associated with
these were borne by the client (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary in order to ensure that the adjustments/expansions commissioned that
were undertaken/developed for a version will also work perfectly and can be used in the
subsequent version.




A+W Software GmbH                 EN-FUNC-A+W Enterprise iTOE.DOCX                                      4
3. Performance Description
3.1. Data
Product                  A+W Enterprise
Module number            200019
Module                   iTOE
Brief description        Integrated CAD in A+W Enterprise
Available                Starting with A+W Enterprise v6 / A+W CAD Designer
                         (Shapes) v6

3.2. Description
The goal of the technical order entry with iTOE is to be able to enter geometries and processing
both in the A+W Enterprise order entry as well as in A+W CAD Designer (Shapes) and if possible,
to receive a harmonized BOM.
In the iTOE, the A+W CAD Designer (Shapes) is integrated into the order/quotation entry in A+W
Enterprise. This enables:
    •   The entry and import of geometric data with the help of the A+W CAD Designer (Shapes).
    •   The generation of geometric data (SN files) from the A+W Enterprise order data.
    •   The harmonization of information between the two systems.
The standard processing and geometry entry in AWE enables the input and visualization of
standard shapes and standard processings in the sense of the shape catalog and the A+W
standard processing type catalog. The iTOE also offers support for free shapes and non-standard
processings.


3.3. Requirements
    •   A license for the A+W CAD Designer (Shapes) is required. Depending on the desired
        functionality in the CAD (e.g. DXF import), it may be necessary to license additional
        options.
    •   The user must be trained in the operation of the CAD.
    •   A+W Enterprise Version 6.3 is assumed.
    •   The module variable in A+W Enterprise must be activated.
    •   The use of the A+W processing type catalog is assumed (described below as STD
        processing).
    •   In this document there is a distinction between STD shapes (shapes from the A+W shape
        catalog) and free shapes. Other catalogs are not currently supported.



A+W Software GmbH                EN-FUNC-A+W Enterprise iTOE.DOCX                                  5
3.4. List of functions
   •       The entry of STD geometries and STD processings in A+W Enterprise with subsequent
           further processing in the A+W CAD Designer (Shapes).
   •       Assignment of existing SN files to order items with subsequent comparison of the STD
           geometries and processings in the A+W Enterprise BOM.
   •       In the A+W CAD Designer (Shapes), STD geometries and STD processings can be added
           and changed and returned to A+W Enterprise. Here, new STD processings are added to
           the A+W Enterprise BOM, removed processings are deleted, and changed processings
           adjusted. Here, it is not absolutely necessary to save a SN file and link it with the item.
   •       For the geometric entry of processings in the A+W CAD Designer (Shapes) there are also
           other input possibilities. (e.g. dimensioning via chain dimensions)
   •       If the file is saved, the following information can also be stored there:
           o Change of the display (additional or changed dimensions, additional text, etc.)
           o Technological changes (adjustment for cutting or the processing centers)
   •       Inn particular, via A+W CAD Designer (Shapes), geometric data that describes free shapes
           can be incorporated (e.g. via the DXF import).
   •       The synchronization status of the item is managed via a status value:


       SN           Description
       status
       0            All CAD processings were taken over into the A+W Enterprise BOM and no
                    associated CAD file was saved
       1            The associated CAD file is saved at the request of the person making the entry.
                    (-> SN menu element: Exit TOE and save file)
       2            The associated CAD file is saved because it contains information that could not
                    be returned as AWType to A+W Enterprise.
       3            The associated CAD file is saved because for a reported AWType, no
                    appropriate processing was found in the master data.
       4            2+3
       5            The associated CAD file is saved because status 1,2,3 or 4 was reached and in
                    addition, this is a free shape or a fixed geometry (shape dimensions may no
                    longer be changed).
       100          A+W Enterprise BOM and CAD file are in a non-synchronized state. In
                    particular free shapes and shapes from SN with shape change
                    ("cadShapeTransfomation") receive the status 100 after initial transfer and
                    must be adjusted manually in case of further adjustments.
       101/102 Special status for steps (step changes in the SN are not taken over into the
               A+W Enterprise)




A+W Software GmbH                    EN-FUNC-A+W Enterprise iTOE.DOCX                                    6
3.5. Limitations
3.5.1. General
Synchronization for free shape (shape 99)
For entry of a free shape (shape 99) with processings in the A+W CAD Designer (Shapes) via iTOE
and subsequent reporting to A+W Enterprise, if all processings could be mapped, the associated
item is set to SN status 5. That is, you can no longer change the geometry of the sheet (external
shape) in A+W Enterprise. This is only possible in the A+W CAD Designer (Shapes).
    •   In this state, however, additional processings can be added in the A+W CAD Designer
        (Shapes) and transferred to A+W Enterprise.
    •   In A+W Enterprise, processings added will be added to the SN file, insofar as they were
        dimensioned absolutely (with respect to the circumscribing rectangle). If there is an
        attempt to add a processing with another dimensioning type to the AWE BOM, then a
        warning will appear in the processing entry that this change will cause a non-synchronized
        state.
    •   A change of the processing parameters in A+W Enterprise is also still possible in this state.
        Such a change also means that the corresponding parameter change will be made via the
        iTOE in the SN file.
Edge processing can be reported back from the A+W CAD Designer (Shapes) to the A+W
Enterprise BOM if all edges of the shape should be processed. Here, several edge processings are
also possible assuming that all edges are always processed.
On reporting to A+W Enterprise, edge processings that are not done on all edges cause the item
to be set to the SN status 100.
Processings that cannot be mapped to A+W standard types
These processings cannot be transferred back to A+W Enterprise. Here it is necessary to save the
SN file and link it with the item.
In general, in A+W Enterprise, you must add this processing to the BOM manually (price
calculation, production planning). This processing may not have any assignment to an A+W
processing type, otherwise it would be added to the SN file if necessary.
Macros (also parametric macros)
The addition of processing macros to A+W CAD Designer (Shapes) means that macros are resolved
into their individual processings and these are reported back to A+W Enterprise.
However, if the macro is entered in A+W Enterprise, it can be retained. In this state, however, no
change should be made to the processings assigned to the macro in the A+W CAD Designer
(Shapes). If this is absolutely necessary, at least the SN file must be saved.
Shape change for items with link to a SN file
    •   In the A+W CAD Designer (Shapes) it is possible to change the associated geometry and to
        perform a new shape detection, which means that a new A+W shape can arise. This shape
        change is then reported back to A+W Enterprise, whereby the shape parameters are
        synchronized appropriately in A+W Enterprise. The item is thus put into the status 5.




A+W Software GmbH                 EN-FUNC-A+W Enterprise iTOE.DOCX                                      7
    •   When entering the shape dialog in A+W Enterprise, with this status a query appears
        whether the existing SN file should be removed and replaced with the new geometry. If
        the answer to this query is "No," then the user has the opportunity to make the geometry
        change nevertheless and to to continue working non-synchronized (with SN status 100) or
        to leave the shape information unchanged in A+W Enterprise.
Shapes whose number of segments deviate from the number of XOPT edges
Shapes with a different number of segments in the A+W CAD Designer (Shapes) in comparison to
the number of edges in A+W Enterprise cannot currently be mapped. The consequence of this is
that the associated item is currently set to the SN status 100. Affected by this are the shapes 60,
61, 62, 63, 74, 75, 78, 81, 123, 124, 125, 133
Assign SN file
As soon as a SN file was assigned to an item, for performance reasons, the synchronization of the
data in A+W Enterprise and the data within the A+W CAD Designer (Shapes) is not undertaken as
often. This shows up in the application, among other things, in that a changed drilling diameter is
only updated after exiting the order BOM in the SN Live view.
Step changes
Step changes in the TOE file are not yet supported. Here, the item goes into the special status
101/102.
Templates
The selection of a template and corresponding entry of all corresponding parameters in an order
item of the order entry is not possible.
However, a template like any other SN file can be used for synchronization. For this, the template
file is added as SN file to the appropriate item (CTRL+E) and then "synchronization" is selected. In
the CAD program, the dimensions can then be adjusted and after that, the template information
taken over into the A+W Enterprise BOM by exiting the TOE.
Ordered subparts for items with SN file
If an order item contains an ordered subpart and a SN file was attached to the item, then this file
is also taken over into the order item for the subpart. The SN file still contains the glass structure
of the entire order item and not just of the ordered item. From this it follows that in the SN file
(through inheritance from the header part), processings can be contained on the ordered glass
(e.g. drillings) that should not be made. When printing out the order via the A+W Enterprise Print
Service, the CAD sketch is also printed according to the attached SN file.


3.5.2. CAD
The CAD offers a relatively great degree of freedom for the generation and changing of shapes. In
the course of the iTOE, in particular the geometry, inner contours, and edge processing views
must be used according to their definition. The data for the reporting to A+W Enterprise is gained
from these views. This way of working will be explained through the standard configuration of the
tools in the CAD. For combined products (IG, LSG), the processings must be done on the header
part. If a processing refers to a subpart, this must be stored in the BOM of the corresponding
processing. This is also the standard procedure, with which an appropriately trained user should
be familiar. Changes on the level of the subparts are possible, however they will not be reported
back to the A+W Enterprise.



A+W Software GmbH                  EN-FUNC-A+W Enterprise iTOE.DOCX                                      8
3.6. Notes




A+W Software GmbH   EN-FUNC-A+W Enterprise iTOE.DOCX   9
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Enterprise iTOE.DOCX   10

