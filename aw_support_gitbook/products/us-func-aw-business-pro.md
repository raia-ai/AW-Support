---
title: "US FUNC A+W Business Pro"
category: "functional_descriptions"
product: "A+W Business Pro"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Business Pro"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Specification   A+W Business Pro 6                                     english 1. Notes about this Document This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The greatest care was used in compiling the texts and figures. However it is not possible to exclude errors completely"
source_file: "US-FUNC-A+W Business Pro.pdf"
---


# US FUNC A+W Business Pro

     Functional Specification


A+W Business Pro 6




                                english
1. Notes about this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The greatest care was used in
compiling the texts and figures. However it is not possible to exclude errors completely. A+W
Software GmbH assumes no liability for errors or imprecise statements unless these can be traced
back to intentional or negligent actions.


1.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


1.2. Copyrights
© 2015, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation may only be copied whole or in part, stored in an archiving
system or transmitted in any other form in accordance with the license agreement. Without the
prior written permission of A+W Software GmbH, the documentation may not be transmitted
electronically, by recording or in any other form.


1.3. Exclusion of liability
A+W Software GmbH assumes no liability for data errors that rely on basic principles of the
standard functions made available by Microsoft, Unix or other software and hardware suppliers.
A+W reserves the right to change software data, structure, and interfaces as part of program
expansions without prior announcement. All adjustments, expansions, database queries, reports,
analyses, and interface expansions that were created individually for our customers and/or
machines and software partners as well as all costs and efforts associated with these were borne
by the client (customers, machine and software partners). This includes also any necessary long-
term costs and efforts for the expansion and adjustment of subsequent program versions. This is
necessary in order to ensure that the adjustments/expansions commissioned that were
undertaken/developed for a version will also work perfectly and be used in the subsequent
version.




                                                                                                 3/19
2. Table of Contents
Notes about this Document                                   3
 Trademarks                                                 3
 Copyrights                                                 3
 Exclusion of liability                                     3
Table of Contents                                           4
Description of the product                                  5
Characteristics in the Organization Area                    6
Features in the Optimization                                9
Coupling/Expansion with other A+W Products/Modules         13
 Production Software                                       13
 A+W Business Capacity Planning                            14
 A+W Business Stock Connection                             14
Machine Activation Features                                16
Functionality A+W Business Pro and A+W Business Pro (EL)   17
Contact Address                                            19




                                                           4/19
3. Description of the product
A+W Business Pro is an integrated ERP-PPS solution for small and medium-sized companies for
use in order processing and production planning.
The A+W commercial solution enables not just the entry of quotations, orders, credits,
complaints, delivery notes, and the management of purchase orders and inquiries, but also the
control of other company areas (e.g. stock, purchasing, dispatch, etc.).
The integrated production solution offers comprehensive technical support for the processing and
planning of orders and quotations. Thanks to the intelligent wizard function, the process of batch
formation, optimization, on through to production release can be completed with a mouse-click.
The user can switch to "expert mode" at any time and can influence individual planning and
optimization steps manually and explicitly there and thus change the result.
The target group of A+W Business Pro is small and medium-sized companies who organize their
production mostly manually and using production papers.
A+W Business Pro should be regarded as independent of earlier A+W products. In particular, A+W
Business Pro is not an upgrade product from earlier production solutions (such as ALFERT or
XOPT2000). Thus there is also no guarantee that all functional characteristics of earlier products
are available in this product. Required features that are not listed in these technical specifications
must be clarified on request.




In this document, only the services and characteristics of the production area (master data and
production manager) are specified in order to delimit them as compared to other A+W products
and other production solutions available on the market.



                                                                                                 5/19
4. Characteristics in the Organization Area
Supported features/processes                      Non-supported features/processes
Pre-defined lot types                             Lot types cannot be defined freely
   •   100 = simple glass, processed simple          •   Pre-defined lot types cannot be
       glass                                             changed.
   •   200 = LSG                                     •   No new or additional lot types can be
                                                         defined.
   •   300 = IGU
Pre-defined storage space organizations
   •   The system is delivered with two pre-
       defined storage space organizations: A-
                                                  4.1.
       rack and IGU harp racks
   •   Within these two standard orgas, the
       following production/organization
       forms are mapped: processed simple
       glass, IGU, LSG production
Self-defined storage space organizations
   •   The set-up and management of self-
       defined organizations is possible - with
                                                  4.2.
       adherence to the pre-defined
       parameters and basic conditions
       mentioned here (lot types, for
       example)
   •   Multi-level production organizations
       can be mapped
   •   A-rack and harp rack organizations are
       supported. Mixed forms are also
       possible
Pre-defined storage mode (stacking mode)          No changes/additions to stacking mode
   •   The system supports/includes the              •   Other stacking modes, such as unit,
       stacking mode production with split               glass or Vabgla, are not supported
       groups
                                                     •   In case of frame-break (new
For details about the stacking mode described            generation when the maximum load
here, please consult the manual about detailed           is reached), groups cannot be kept
scheduling.                                              together
                                                     •   Change to stacking modes and split
                                                         modes are not possible
                                                  For details about the stacking modes
                                                  described here, please consult the manual
                                                  about detailed scheduling.


                                                                                              6/19
Self-defined rack numbers
    •   The number ranges for storage spaces
        and storage space groups can be
        defined freely in the master data
Sequential rack numbers                           No permanent reset of the rack numbers
    •   With reaching of the maximum load of          •   A reset of the rack numbers is only
        a storage space, the system                       done with reaching of the self-
        automatically generates a new storage             defined number limit
        space with a new logical number
                                                  No splitting of order items in the detailed
                                                  scheduling
                                                      •   The A+W Business Pro detailed
                                                          scheduling does not support the
                                                          splitting of order items
Pre-defined rough scheduling and detailed         No freely-definable rough and detailed
scheduling views                                  planning views
    •   The system offers pre-defined rough           •   No additional information can be
        scheduling and detailed scheduling                displayed or configured (for example
        views                                             additional, new columns or filters)
    •   In the rough scheduling area, it is           •   Customizing is not possible
        possible using pre-defined columns to
        create individual filter structures and
        to save them depending on the user
Output of production papers and bar codes
    •   The system supports the manual
        organization of production processes
        using pre-defined production papers
        and bar codes
    •   Production papers and bar codes
        already integrated into the system can
        be adjusted in format and layout
        (Crystal Reports)
Creation of self-defined reports                  No incorporation of self-defined/additional
                                                  production papers in the printing process
    •   The system permits the creation of
        self-defined queries and reports              •   It is not possible to define additional
        according to the A+W Business (CR)                production papers and to incorporate
        database description                              these in the standard process flow
Pre-defined criteria for storage space            No support of self-defined formulas
organization
                                                      •   It is not possible to define new
    •   A+W Business receives a set of pre-               variables or operators yourself and
        defined formula building blocks                   add them to the system
        (variables and operators) in order to
        define filter criteria for sorting and
                                                                                                7/19
       groupings in the area of storage space   •   There is no possibility for form-based
       organization                                 criteria/filter definition (SQL)
                                                    provided
Item split in the AWB Capacity Planning
   •   Is supported since V6 and thus split
       items can be scheduled in the
       Production Manager.




                                                                                       8/19
5. Features in the Optimization
Supported features/processes                      Non-supported features/processes
Supported yield and sequence optimization         No explicit selection of the optimization
modes                                             modes
   •   Sequence optimization XOPTS 6.2                •   Setting of the optimization mode not
       (strict sequence)                                  explicitly possible; instead, controlled
                                                          by the system via setting of the
   •   Sequence optimization XOPTS 6.1
                                                          grouping and sorting parameters
       (keep customers together)
   •   Sequence optimization XOPTS 5.2
       (standard)
   •   Sequence optimization XOPTS 5.1 (IGU
       on harp racks or many A-racks)
   •   XOPT (chaotic optimization)
   •   Setting of the optimization mode
       implicitly, via the grouping and sorting
       parameters
For details about the optimization modes
described here, please consult the manual
about detailed scheduling.
Synchronous optimization
   •   In the optimization, the system
       considers the dependencies of sheet
       and countersheet for IGU and LSG in
       the sequence orientation of the
       optimization (depending on the
       organizational form selected and the
       grouping and sorting keys set)
                                                  No dynamic optimization
                                                      •   A+W Business Pro does not include or
                                                          support a dynamic optimization mode
                                                      •   Expansions such as A+W Dynopt and
                                                          A+W Dynopt Compact cannot be
                                                          coupled to the system
Optimization of quotations and/or                 Optimization of quotations and/or
reservation orders                                reservation orders
   •   Quotations or reservation orders               •   Except for the PDF, no data is saved.
       entered in the ERP area can be
                                                      •   Costs determined are not written
       optimized in the production manger
                                                          back.
       for calculation purposes. The results
       are saved as PDF in the quotation.             •   There is no reservation of stock plates

                                                                                              9/19
Decoating
    •   We write the decoating widths for the
        shape into the Opt2 files if:
        -   We are using the A+W catalog
        -   The shape does not have any
            circular arc segments
        -   Decoating is possible on the
            machine and the decoating width
            is greater than or equal to the
            minimum on the machine.
        -   For individual sheets or LSG, the
            processing edge decoating (1025)
            from the A+W processing catalog
            is heeded and evaluated
            accordingly.
Manual insertion of additional sheets (fillers)   No automatic filler dimensions
    •   Fillers can be added manually in the         •   The system does not generate any
        A+W Planeditor (after optimization has           fillers automatically in the course of
        been performed and stored)                       optimization
    •   Entry of sheet parameters possible:
        height, width, shape number, storage
        space number
                                                  No bar codes or production papers for
                                                  manually-added sheets
                                                     •   No bar codes are generated for
                                                         manually-added sheets.
                                                     •   Manually-added sheets are not
                                                         considered/displayed on production
                                                         papers.
Graphic display of shapes in the quick display    No modification of the optimization results
    •   The quick display (detail view in the        •   The optimization results (cutting
        process of optimization) cannot                  patterns) cannot be edited manually
        display any shape geometries                     in the A+W Planeditor
        graphically.
                                                     •   If changes are necessary, then
Displayed instead are the circumscribed                  changes must be made to
rectangles. This is the preview that can be              optimization parameters (shape
generated more quickly                                   break edges, orga, etc.) in the process
                                                         of optimization - before saving the
                                                         optimization
Optimizing shapes




                                                                                            10/19
   •   In the optimization, A+W Business Pro
       considers the shape parameters stored
       in the system and the order
Integration of A+W Shape Opt
   •   If the add-on A+W Shape Opt should
       be activated, then 2 shape geometries
       apiece are combined in the
       optimization
Graphic display of shapes on printout and in
the A+W Planeditor
   •   In A+W Planeditor (after saving the
       optimization results) and on printouts
       (work sheets), the system displays
       shapes correctly
Display of the most important information on    No editing of the graphic display in the A+W
printouts and displays                          Planeditor and the quick display
   •   The quick display provides the               •   The information displayed in the
       following information: dimensions,               quick display (detail view) and in the
       cutting dimensions, storage space no.,           A+W Planeditor cannot be changed or
       breakage sequence                                expanded. Thus, for example, no
                                                        order numbers or item numbers can
   •   Printouts and the A+W Planeditor also
                                                        be displayed.
       provide the following information:
       shape image
Free shapes for IGU or LSG
   •   The processing of free shapes (shape
       99) is supported for insulated glass
       and/or LSG glass
Surcharges for edge processings (rectangle,     Surcharges for edge processings (free shape
default shape)                                  [F99])
   •   For dimension-changing edge                  •   For free shapes, surcharges are not
       processings such as grinding, the                added automatically to the geometry.
       surcharges can be managed in                     The user must create the contour as it
       Business Pro. For rectangles and                 should be cut.
       default shapes, these surcharges are
                                                The exception to this are drilling hole
       added to the cutting contour.
                                                markings in the cutting code. The shapes are
                                                written here as F99 to the block file and the
                                                edge surcharges are calculated in advance.
Number of stock plates
   •   The number of stock plates and/or
       residual sheets per optimization can
       be 10 or 30.
Breakage

                                                                                         11/19
    •   Breakage can be reported in the
        Production Manager (starting with V6).
        With the broken sheets, the user can
        form a breakage run and then plan in
        detail, optimize, and produce as usual.
Marking drilling holes
    •   The drilling holes can be scored on the
        cutting table.
    •   Normal drilling holes and stepped
        drilling holes are heeded.
Offer optimization
    •   In addition to orders, quotations can
        also be planned. The quotation mode is
        only possible in standard mode. The
        quotation mode runs precisely like the
        order mode (detailed planning,
        optimization, and report output). For
        quotations, the user can change stock
        plate dimensions in the optimization
        and the purchase price of the stock
        plate (price per m²) and thus influence
        the optimization result. The results are
        3 reports (no cutting code) that depict
        the following:
        -   Optimization      result        with
            optimization parameters.
        -   Cross-sections
        -   List of the stock plates
        The reports are attached to the
        quotation.
Switchable tolerances for cuts in the
optimization in A+W Business Pro

    •   In A+W Business Pro it is now possible
        that the optimization ignores the
        minimum and maximum distances
        from XX and YY cuts if otherwise no
        result can be achieved. This applies for
        these tolerances:

        -   Tolerance for min. abs. X-X
        -   Tolerance for min. abs. Y-Y
        -   Tolerance for max. abs. X-X
        -   Tolerance for max. abs. Y-Y


                                                   12/19
6. Coupling/Expansion with other A+W
  Products/Modules
6.1. Production Software
Supported features/processes                      Non-supported features/processes
                                                  No coupling to external production software
                                                  or display systems
                                                     •   It is not possible to couple A+W
                                                         Business Pro to external software
                                                         producers' production software or
                                                         display/monitoring systems
                                                  No coupling to A+W Production
                                                     •   A+W Business Pro cannot be coupled
                                                         to A+W Production
                                                  No coupling to/transfer of data to A+W
                                                  Production Terminal
                                                     •   A data transfer for the graphic display
                                                         of production steps on A+W
                                                         Production Terminal is not possible
Coupling/data transfer to A+W Realtime            No feedback/data reporting from A+W
Optimizer                                         Realtime Optimizer
   •   It is possible to transfer the optimized      •   Reports from A+W Realtime Optimizer
       cutting patterns to the A+W Realtime              are not evaluated in A+W Business
       Optimizer in order to monitor and                 Pro
       control the cutting online there
                                                     •   Reports from the A+W Realtime
                                                         Optimizer are not evaluated in the
                                                         A+W Business Capacity Planning (in
                                                         the coupling A+W Business Pro - A+W
                                                         Business Capacity Planning - A+W
                                                         Realtime Optimizer)
Connection to A+W Business PDC                    PDC bookings only to the item
   •   The system supports the data transfer         •   The A+W Business PDC can only book
       to and from A+W Business PDC                      to the item
                                                     •   A precise booking of sheets or parts is
                                                         not possible
Incorporation of AWB Barcode Scanner              A+W Realtime Optimizer stock plate quantity
                                                  30
   •   With the AWB Barcode Scanner
       (starting with V6), breakage or defects       •   For the cutting process and the
       on the sheet can be reported. The                 existing optimization modes, only

                                                                                             13/19
       Production Manager can access the               optimizations with a maximum of 10
       reported sheets on the breakage                 different stock plate sizes or residual
       dialog and the user can form a                  sheet sizes are possible. The option 30
       breakage lot with these and additional          stock plates per optimization is not
       broken sheets.                                  supported.




6.2. A+W Business Capacity Planning
Supported features/processes                    Non-supported features/processes
Coupling to A+W Business Capacity Planning      Over-quantities
   •   The standard delivery version of A+W        •   No over-quantities possible, neither
       Business Pro already includes the               production-technically nor order-
       functions for machine assignment                technically
       (which are integrated into the
                                                Shortage
       capacity planning module)
                                                   •   No shortage possible, neither
   •   For the use of the capacity planning
                                                       production-technically nor order-
       functions (shifts, transition times,
                                                       technically
       default times, etc.) it is
       possible/necessary to expand the
       system with a complete A+W Business
       Capacity Planning (additional license)
Item split in the AWB Capacity Planning
   •   Is supported since V6 and thus split
       items can be scheduled in the
       Production Manager.




6.3. A+W Business Stock Connection
Supported features/processes                    Non-supported features/processes
Use of residual sheets from the residual
sheet stock
   •   The system offers the possibility for
       creating and managing a residual
       sheet stock
   •   Manually-added residual sheets can
       be used in the optimization
   •   Residual sheets can only be added
       manually to the residual stock




                                                                                         14/19
    •   Residual sheets are calculated and
        removed after the stock plates in the
        residual stock.
Use of stock sheets for the "best result"
    •   The optimization essentially uses the
        stock sheets that provide the "best
        result" with respect to costs and yield
    •   If a residual sheet should absolutely
        be used despite poorer yield or costs,
        then the use of the residual sheet can
        be controlled manually via the priority
                                                  No stock removals with the A+W Realtime
                                                  Optimizer
                                                     •   Since A+W Business Pro already offers
                                                         the possibility for manual stock
                                                         removal in the course of optimization,
                                                         it is not possible/permissible to make
                                                         automatic or manual stock removal
                                                         bookings with the A+W Realtime
                                                         Optimizer
                                                     •   The possibility for stock removal must
                                                         be deactivated in the settings of the
                                                         A+W Realtime Optimizer




                                                                                           15/19
7. Machine Activation Features
Supported features/processes                    Non-supported features/processes
Activation of standard machines
   •   The system offers data transfer to and
       the activation of cutting tables, IGU
       lines, and frame benders
   •   Here, only commonly-available
       machines are supported
   •   Please contact A+W Sales in advance
       of the project (during the quotation
       phase) to see whether the machine
       type you are using is supported.




                                                                               16/19
8. Functionality A+W Business Pro and A+W
  Business Pro (EL)




                                                                                 A+W Business Pro (EL)
                                                             A+W Business Pro
Functionality




Company Areas
Purchasing                                                                     1
Sales                                                                          
Production                                                                     
Stock                                                                          1
Dispatch                                                                       


Organization
Pre-defined lot types                                                          
Pre-defined storage space organizations                                        
Self-defined storage space organizations                                       
Pre-defined storage mode (stacking mode)                                       
Self-defined rack numbers                                                      
Sequential rack numbers                                                        
Pre-defined rough scheduling and detailed scheduling views                     
Output of production papers and bar codes                                      
Creation of self-defined reports                                               
Pre-defined criteria for storage space organization                            
Item split in the AWB Capacity Planning                                        
Technical order entry                                                          1


Optimization
Supported yield and sequence optimization modes                                


                                                                                                         17/19
 Synchronous optimization                                                 
 Optimization of quotations and/or reservation orders                     
 Decoating                                                                
 Manual insertion of additional sheets (fillers)                          
 Graphic display of shapes in the quick display                           
 Optimizing shapes                                                        
 Integration of A+W Shape Opt                                             
 Graphic display of shapes on printout and in the A+W PlanEditor          
 Display of the most important information on printouts and displays      
 Free shapes for IGU or LSG                                               
 Surcharges for edge processings (rectangle, default shape)               
 Number of stock plates                                                   
 Breakage                                                                 
 Marking drilling holes                                                   
 Offer optimization                                                       


 Expansion with other A+W Products / Modules
 Coupling/data transfer to A+W Realtime Optimizer                         
 Connection A+W Business EDI                                              1
 A+W CAD Designer                                                         2


 A+W Capacity Planning                                                    
 A+W Business Stock Connection                                            1


 Activation of Standard Machines
 Cutting Tables                                                           
 IG Lines                                                                 
 Spacer Benders                                                           


Legend:
         Included
    1
          Included in US Version
         Not available
 1
          Optionally available
 2
          Optionally available for US Version

                                                                                18/19
9. Contact Address
A+W Software GmbH

Am Pfahlgraben 4 - 10

35415 Pohlheim

Germany

Tel. +49 6404 2051 0

Fax. +49 6404 2051 877



E-Mail: zentrale@a-w.com

Internet: http://www.a-w.com/




                                19/19

