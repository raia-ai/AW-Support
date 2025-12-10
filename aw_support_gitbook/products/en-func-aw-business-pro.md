---
description: "EN FUNC A+W Business Pro"
---



# EN FUNC A+W Business Pro

     Functional Description


A+W Business Pro 6




                              english
1. Content
1.   Content                                                                         3
2.   Notes on this Document                                                          4
     2.1. Trademarks                                                                 4
     2.2. Copyrights                                                                 4
     2.3. Disclaimer of liability                                                    4
3.   Product Presentation                                                            5
     3.1. Notes                                                                      6
          3.1.1. A+W Business Pro in connection with A+W Realtime Optimizer          6
          3.1.2. A+W Business Pro in connection with A+W Production Terminal (EL)    6
4.   Features in the Organization Area                                               7
5.   Features in Optimization                                                       10
6.   Coupling / expansion with other A+W products / modules                         14
     6.1. Production software                                                       14
     6.2. A+W Business Capacity Planning                                            16
     6.3. A+W Business stock connection                                             16
7.   Features of Machine Control                                                    18
8.   Contact Address                                                                19




A+W Software GmbH                   EN-FUNC-A+W Business Pro.docx                        3
2. Notes on this Document
This documentation and the software described in it are only licensed and may only be used and
copied pursuant to this license. The contents of the documentation are for information purposes
only and are subject to changes without prior notice. The text and illustrations were compiled
with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH
cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly
negligent action.


2.1. Trademarks
All hardware and software names mentioned in this documentation may also be registered
trademarks or other industrial property rights held by third parties. Copyrights of third parties
must be complied with.


2.2. Copyrights
© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation can be copied, completely or in part, saved in an
archiving system, or transferred in any other form only in accordance with our license agreement.
Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by
recording or in any other way, without the written prior approval of A+W Software GmbH.


2.3. Disclaimer of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions which have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions which
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH                   EN-FUNC-A+W Business Pro.docx                                     4
3. Product Presentation
A+W Business Pro is an integrated ERP PPS solution for small and medium-sized businesses in the
sector of order processing and production planning.
The business solution from A+W not only makes it possible to enter quotations, orders, credit
notes, complaints and delivery notes as well as to manage orders and inquiries, but also facilitates
controlling of other company areas (e.g. warehouse, purchasing, dispatch, etc.).
The integrated production solution offers comprehensive technical support for the processing and
planning of orders and quotations. Thanks to the intelligent wizard function, the process of batch
formation, optimization, on through to production release can be completed with a mouse-click.
The user has the option to switch to the so-called "expert" mode at any time, where he/she can
manually and explicitly directly influence the individual planning and optimization steps, and
consequently the result.
The target group for A+W Business Pro are small and medium-sized companies that mainly
organize their production manually and by means of production documents.
A+W Business Pro should be regarded as independent of earlier A+W products. In particular, A+W
Business Pro is not an upgrade product from earlier production solutions (such as ALFERT or
XOPT2000). Thus there is also no guarantee that all functional characteristics of earlier products
are available in this product. Required features that are not listed in these technical specifications
must be clarified on request.




In this document only the services and functional characteristics of the production area (master
data and production manager) are specified in order to distinguish them from other A+W
products and other production solutions available on the market.


A+W Software GmbH                   EN-FUNC-A+W Business Pro.docx                                    5
3.1. Notes
3.1.1. A+W Business Pro in connection with A+W Realtime
    Optimizer
If A+W Business Pro is used together with the A+W Realtime Optimizer, the waste statistics refer
only to plan values. All manual changes or changes due to the influence of the A+W Realtime
Optimizer are not considered here. If an A+W Realtime Optimizer standalone is used, the actual
consumption data can be drawn from the A+W Realtime Optimizer database.


3.1.2. A+W Business Pro in connection with A+W Production
    Terminal (EL)
If A+W Business Pro is used together with the A+W Production Terminal (EL), the Partial Delivery
functionality is not available since rack bookings are not supported.
The same applies for the Reject Handling for Purchased Orders functionality (item number
210015). In this environment, the required service is not available.




A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx                                   6
4. Features in the Organization Area
Supported features / processes                   Features / processes that are not
                                                 supported
Predefined lot types                             Lot types that cannot be defined as desired
    •   100 = single glass, processed single        •   Predefined lot types cannot be
        glass                                           changed.
    •   200 = LAMI                                  •   New or additional lot types cannot be
                                                        defined.
    •   300 = IG
Predefined rack organization systems
    •   The system is delivered with two
        predefined rack organization systems:
        A racks and IG harp racks
    •   Within these two standard
        organization systems, the following
        production / organization types are
        shown: processed single glass, IG,
        LAMI production
Self-defined rack organization systems
    •   It is possible to set up and manage
        organization systems that were
        defined by yourself, provided that the
        predefined parameters and framework
        conditions that are specified here are
        met (e.g. lot types)
    •   Multi-level production organization
        systems can be mapped
    •   A rack and harp rack organization
        systems are supported. Mixed types
        are also possible
Predefined parking mode (stack mode)             No changes / supplements to the stack mode
    •   The system supports / includes the          •   Other stack modes, such as unit, glass
        stack mode Production with split                or Vabgla are not supported
        groups
                                                    •   In case of frame-break (new
You can read more about the stack mode that             generation when the maximum load
is described here in the Manual on the Process          is reached), groups cannot be kept
of Detailed Scheduling.                                 together
                                                    •   Changes to the stack modes or split
                                                        modes are not possible




A+W Software GmbH                 EN-FUNC-A+W Business Pro.docx                                  7
                                                You can read more about the stack modes
                                                that are described here in the Manual on the
                                                Process of Detailed Scheduling.
Self-defined rack numbers
    •   The number area for racks or rack
        groups can be defined in the master
        data as desired
Consecutive rack numbers                        No permanent reset of the rack numbers
    •   With reaching of the maximum load of        •   A reset of the rack numbers is only
        a storage space, the system                     done with reaching of the self-
        automatically generates a new storage           defined number limit
        space with a new logical number
                                                No splitting of order items in detailed
                                                scheduling
                                                    •   The A+W Business Pro detailed
                                                        scheduling does not support the
                                                        splitting of order items
Predefined rough and detailed scheduling        Rough and detailed scheduling views that
views                                           cannot be defined as desired
    •   The system offers predefined rough          •   It is not possible to show or configure
        scheduling and detailed scheduling              additional information (e.g.
        views                                           additional new columns or filters)
    •   In rough scheduling, you can create         •   Customizing is not possible
        your own filter structures with
        predefined columns and save these
        user-dependently
Output of production papers and bar codes
    •   The system supports the manual
        organization of production processes
        by means of predefined production
        papers and bar codes
    •   The format and layout of production
        papers and bar codes that are already
        integrated in the system can be
        adjusted (Crystal Reports)
Creation of self-defined reports                No integration of self-defined / additionally
                                                defined production papers in the printing
    •   The system enables the creation of
                                                process
        self-defined queries and reports in
        accordance with the database                •   It is not possible to define new
        description A+W Business (CR)                   additional production papers and
                                                        integrate those into the standard
                                                        process flow




A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx                                  8
Predefined criteria for rack organization          No support of self-defined formulas
systems
                                                      •   You cannot define new variables or
    •   A+W Business includes a set of pre-               operators yourself and add them to
        defined formula elements (variables               the system
        and operators) that are used to define
                                                      •   An option for formula-based criteria /
        filter criteria for sorting and grouping
                                                          filter definition (SQL) has not been
        in the sector of rack organization
                                                          provided for
        systems
Item split in the AWB Capacity Planning
    •   Is supported since V6 and thus split
        items can be scheduled in the
        Production Manager.




A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx                                   9
5. Features in Optimization
Supported features / processes                  Features / processes that are not
                                                supported
Supported waste and sequence optimization       No explicit selection of the optimization
modes                                           modes
    •   Sequence optimization XOPTS 6.2             •   Setting of the optimization mode not
        (strict sequence)                               explicitly possible; rather, it is
                                                        executed while controlled by the
    •   Sequence optimization XOPTS 6.1
                                                        system via setting of the grouping
        (keep customers together)
                                                        and sorting parameters
    •   Sequence optimization XOPTS 5.2
        (standard)
    •   Sequence optimization XOPTS 5.1 (IGU
        on harp racks or many A-racks)
    •   XOPT (chaotic optimization)
    •   Implicit setting of the optimization
        mode via the grouping and sorting
        parameters
You can read more about the optimization
modes that are described here in the Manual
on the Process of Detailed Scheduling.
Synchronous optimization
    •   For the optimization process, the
        system takes into account the
        dependencies of the pane and the
        counter pane for IG and LAMI for the
        sequential orientation of the
        optimization (dependent on the
        selected organization type and set
        grouping and sorting keys)
                                                No dynamic optimization
                                                    •   A+W Business Pro does not include or
                                                        support dynamic optimization modes
                                                    •   Extensions such as A+W Dynopt or
                                                        A+W Dynopt Compact cannot be
                                                        connected to the system
Optimization of quotations and/or               Optimization of quotations and/or
reservation orders                              reservation orders
    •   Quotations or reservation orders            •   Except for the PDF, no data is saved.
        entered in the ERP area can be
                                                    •   Costs determined are not written
        optimized in the production manger
                                                        back.


A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx                                10
         for calculational purposes. The results      •   There is no reservation of stock lites
         are saved as PDF in the quotation.
Decoat
    •    We write the decoating widths for the
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
Manual insertion of additional lites (fillers)     No automatic filler dimensions
    •    Fillers can be added manually in the         •   The system does not generate any
         A+W Planeditor (after optimization has           fillers automatically in the course of
         been performed and stored)                       optimization
    •    Entry of pane parameters possible:
         Height, width, model number, rack
         number
                                                   No bar codes or production papers for
                                                   manually added panes
                                                      •   Bar codes are not generated for
                                                          manually inserted panes.
                                                      •   Manually inserted panes are not
                                                          taken into account / shown on
                                                          production documents
Graphic display of shapes in the quick display     No modification of optimization results
    •    The quick display (detail view in the        •   The optimization results (sectional
         process of optimization) cannot display          views) cannot be manually edited in
         any shape geometries graphically.                A+W Planeditor
Displayed instead are the circumscribed               •   Any changes that may become
rectangles. This is the preview that can be               necessary must be carried out as
generated more quickly                                    changes to optimization parameters
                                                          (model trims, Orga, ...) during the
                                                          optimization process – prior to saving
                                                          the optimization
Optimization of shapes



A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx                                   11
    •   During the optimization process, A+W
        Business Pro takes the model
        parameters that are stored in the
        system and in the order into account
Integration of A+W Shape Opt
    •   If the extension A+W Shape Opt has
        been activated, 2 model geometries
        are combined at a time during the
        optimization process
Graphic display of shapes in printouts and in
A+W Planeditor
    •   The system shows shapes correctly in
        A+W Planeditor (after saving the
        optimization results) and on printouts
        (shop papers)
Display of the most important information on     No editing of the graphic display in the A+W
printouts and displays                           Planeditor and the quick display
    •   The quick display provides the               •   The information displayed in the
        following information: dimensions,               quick display (detail view) and in the
        cutting dimensions, storage space no.,           A+W Planeditor cannot be changed
        breakage sequence                                or expanded. Thus, for example, no
                                                         order numbers or item numbers can
    •   Printouts and the A+W Planeditor
                                                         be displayed.
        provided the following additional
        information: shape image
Free shapes for IGU or LSG
    •   The processing of free shapes (shape
        99) is supported for insulated glass
        and/or LSG glass
Surcharges for edge processings (rectangle,      Surcharges for edge processings (free shape
default shape)                                   [F99])
    •   For dimension-changing edge                  •   For free shapes, surcharges are not
        processings such as grinding, the                added automatically to the geometry.
        surcharges can be managed in                     The user must create the contour as
        Business Pro. These surcharges are               it should be cut.
        added for rectangles and default
                                                 The exception to this are drilling hole
        shapes to the cutting contour.
                                                 markings in the cutting code. The shapes are
                                                 written here as F99 to the block file and the
                                                 edge surcharges are calculated in advance.
Number of stock plates
    •   The number of stock plates and/or
        residual sheets per optimization can
        be 10 or 30.
Breakage


A+W Software GmbH                 EN-FUNC-A+W Business Pro.docx                                   12
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

        -   Tolerance for min. dist.X-X
        -   Tolerance for min. dist.Y-Y
        -   Tolerance for max. dist. X-X
        -   Tolerance for max. dist. Y-Y




A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx   13
6. Coupling / expansion with other A+W
  products / modules
6.1. Production software
Supported features / processes                     Features / processes that are not
                                                   supported
                                                   No coupling to external production software
                                                   or display systems
                                                      •   It is not possible to connect A+W
                                                          Business Pro to production software
                                                          or display / monitoring systems of
                                                          external software producers
                                                   No coupling to A+W Production
                                                      •   A+W Business Pro cannot be
                                                          connected to A+W Production
                                                   No coupling to / transfer of data to A+W
                                                   Production Terminal
                                                      •   It is not possible to transfer data for
                                                          the graphical display of production
                                                          steps to the A+W Production Terminal
Coupling / data transfer to A+W Realtime           No feedback / data feedback from A+W
Optimizer                                          Realtime Optimizer
    •   It is possible to transfer the optimized      •   Feedback from A+W Realtime
        sectional views to A+W Realtime                   Optimizer is not analyzed in A+W
        Optimizer in order to monitor and                 Business Pro
        control cutting to size online there
                                                      •   Feedback from A+W Realtime
                                                          Optimizer is not analyzed in A+W
                                                          Business capacity planning (in the
                                                          coupling A+W Business Pro – A+W
                                                          Business capacity planning – A+W
                                                          Realtime Optimizer)
Connection of A+W Business BDE (barcoding)         Barcoding bookings only specific to the item
    •   The system supports data transfer to          •   A+W Business BDE can only make
        and from A+W Business BDE                         bookings specific to the item
        (barcoding)
                                                      •   A precise booking of lites or parts is
                                                          not possible
Incorporation of AWB Barcode Scanner               A+W Realtime Optimizer stock plate quantity
                                                   30
    •   With the AWB Barcode Scanner
        (starting with V6), breakage or defects


A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx                                   14
       on the sheet can be reported. The       •   For the cutting process and the
       Production Manager can access the           existing optimization modes, only
       reported sheets on the breakage             optimizations with a maximum of 10
       dialog and the user can form a              different stock plate sizes or residual
       breakage lot with these and                 sheet sizes are possible. The option 30
       additional broken sheets.                   stock plates per optimization is not
                                                   supported.




A+W Software GmbH              EN-FUNC-A+W Business Pro.docx                             15
6.2. A+W Business Capacity Planning
Supported features / processes                    Features / processes that are not
                                                  supported
Coupling with A+W Business Capacity               Excess quantities
Planning
                                                     •   No excess quantities possible, neither
    •   The standard delivery version of A+W             production-technically nor order-
        Business Pro already includes the                technically
        functions of the machine classification
                                                  Undersupply
        (integrated in the capacity planning
        module)                                      •   No undersupply possible, neither
                                                         production-technically nor order-
    •   In order to use the capacity planning
                                                         technically
        functions (shifts, transition periods,
        standard times, etc.), it is possible /
        necessary to expand the system with
        a full A+W Business capacity planning
        program (additional license)
Item split in the AWB Capacity Planning
    •   Is supported since V6 and thus split
        items can be scheduled in the
        Production Manager.



6.3. A+W Business stock connection
Supported features / processes                    Features / processes that are not
                                                  supported
Use of residual plates from the stock location
for residual plates
    •   The system offers the option to create
        and manage a stock for residual plates
    •   Residual plates that have been
        manually added to the booking can be
        used for the optimization
    •   Residual sheets can only be added
        manually to the residual stock
    •   Residual sheets are calculated and
        removed after the stock plates in the
        residual stock.
Use of stock sizes for the "best result"
    •   The optimization essentially uses the
        stock lites that provide the "best
        result" with respect to costs and yield



A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx                             16
    •   If it is mandatory that a residue plate
        is used despite worse waste or worse
        costs, the use of the residue plate can
        be manually controlled by means of
        the priority
                                                  Booking out a quantity of stock not possible
                                                  with A+W Realtime Optimizer
                                                     •   Since A+W Business Pro already
                                                         provides an option for manually
                                                         booking quantities out of stock within
                                                         the scope of the optimization, it is not
                                                         possible / allowed to carry out
                                                         automatic or manual booking of
                                                         quantities out of stock using A+W
                                                         Realtime Optimizer
                                                     •   The option to book quantities out of
                                                         stock must be deactivated in the
                                                         settings of A+W Realtime Optimizer




A+W Software GmbH                 EN-FUNC-A+W Business Pro.docx                                  17
7. Features of Machine Control
Supported features / processes                    Features / processes that are not
                                                  supported
Control of standard machines
    •   The system offers data transfer and
        control of cutting tables, IG lines and
        spacer benders
    •   Here, only commercially available
        standard machines are supported
    •   Please contact A+W Sales in advance
        of the project (during the quotation
        phase) to see whether the machine
        type you are using is supported.




A+W Software GmbH                  EN-FUNC-A+W Business Pro.docx                      18
8. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Business Pro.docx   19

