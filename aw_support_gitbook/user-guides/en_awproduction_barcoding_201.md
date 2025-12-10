---
title: "EN AWProduction Barcoding 2.01"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["EN_AWProduction_Barcoding_2.01"]
version: "1.0"
last_updated: "2025-12-10"
description: "Barcoding              H                             English                 A+W Production                                                                                                           Introduction                                           Introduction                                       This part of the documentation contains editorial notes.                                         Revision overview                                       Part"
source_file: "EN_AWProduction_Barcoding_2.01.pdf"
---


# EN AWProduction Barcoding 2.01

Barcoding              H




                        English




            A+W Production
                                                                                                          Introduction




                                      Introduction
                                      This part of the documentation contains editorial notes.


                                      Revision overview
                                      Part
                                      Version / Date

                                      1.00 / 03-2007             Original version

                                      1.01 / 07-2013             Layout adapted to CI 2013.

                                      2.0 / 06-2014              Complete revision

                                      2.01 / 1-2017              Product and company names adjusted.



                                      Editorial
                                      The editorial provides information on the following topics:
                                      •   Notes on this document
                                      •   Copyrights
                                      •   Trademarks
                                      •   Contact

                                      Notes on this document
                                      This publication is written exclusively for end users of A+W Production in mind.
                                      The documentation and software described therein are licensed only and must
                                      be used or copied only in accordance with the terms of our license agreement.
                                      The contents of the documentation are for information purposes only and are
                                      subject to changes without prior notice.
                                      The text and illustrations were compiled with the utmost care. Still, errors can-
                                      not be totally excluded. A+W Software GmbH cannot be held liable for errors
                                      or inaccuracies, unless they can be attributed to intentional or grossly negli-
                                      gent behavior.
                                      The descriptions in this document are based on the full program level of A+W
                                      Production.

                                      Copyrights
                                      © 2017, A+W Software GmbH, all rights, including the right of reprint, produc-
                                      tion of copies and translation, are reserved.
                                      The documentation may be copied, completely or in part, saved in an archiving
2.01 / 07-2017




                                      system, or transferred in any other form only in accordance with our license
                                      agreement. This documentation may not be transmitted, neither electronically,
                                      nor mechanically, nor by recording or in any other way, without the prior written
                                      permission from A+W Software GmbH.


                 A+W Production Barcode Manager                                                                   H-3
                 Introduction




                                Trademarks
                                All hardware and software names mentioned in this documentation might also
                                be registered trademarks or other property rights of third parties. Copyrights of
                                third parties must be complied with.

                                Contact
                                A+W Software GmbH

                                Am Pfahlgraben 4-10

                                D-35415 Pohlheim

                                   +49 6404 2051-0

                                   +49 6404 2051-877

                                Zentrale@a-w.com

                                http://www.a-w.com
2.01 / 07-2017




                 H-4                                                       A+W Production Barcode Manager
                                                                                                                                                      Contents




                                      Contents
                                      Introduction ............................................................................................................. H-3
                                        Revision overview ............................................................................................... H-3
                                        Editorial ............................................................................................................... H-3

                                      Tutorial                                                                                                             H-7
                                      Overview ................................................................................................................. H-9
                                       Documentation .................................................................................................. H-10
                                          Tutorial Structure ........................................................................................... H-10
                                          Display Conventions ...................................................................................... H-11
                                      Basic Ideas ........................................................................................................... H-12
                                       Barcoding .......................................................................................................... H-13
                                       Purpose of A+W Production .............................................................................. H-13
                                      Booking Elements ................................................................................................. H-14
                                       Products ............................................................................................................ H-15
                                          Basics ............................................................................................................ H-16
                                             Direct objects .............................................................................................. H-16
                                             Indirect objects ........................................................................................... H-16
                                          Lites or Units .................................................................................................. H-16
                                             Booking types ............................................................................................. H-17
                                       Booking Places .................................................................................................. H-18
                                          Registration Points ......................................................................................... H-19
                                             Error rack .................................................................................................... H-20
                                             Correct booking .......................................................................................... H-22
                                          Managing Registration Points ........................................................................ H-23
                                             Truck registration point ............................................................................... H-25
                                       Racks ................................................................................................................ H-26
                                          Racks ............................................................................................................. H-27
                                          Boxes ............................................................................................................. H-28
                                          Managing Racks ............................................................................................ H-29
                                       Staff ................................................................................................................... H-32
                                          Employees ..................................................................................................... H-33
                                          Managing Employees .................................................................................... H-34
                                       Status ................................................................................................................ H-36
                                          Status values ................................................................................................. H-37
                                             Unit/group ................................................................................................... H-37
                                             Rack ........................................................................................................... H-37
                                             Registration point ........................................................................................ H-37
                                             Action barcode ............................................................................................ H-38
                                          Managing Status Values ................................................................................ H-39
                                      Data Entry ............................................................................................................. H-41
                                       Scanner ............................................................................................................. H-42
                                          Scanner Types ............................................................................................... H-43
                                             Online scanners .......................................................................................... H-43
                                             Denso scanners (WLAN) ............................................................................ H-43
                                             Serial scanners ........................................................................................... H-44
                                             Offline scanners .......................................................................................... H-44
                                             The scanner configurations ........................................................................ H-44
                                          Barcodes ........................................................................................................ H-45
                                      Booking Examples ................................................................................................ H-46
                                       Scanning Sequence .......................................................................................... H-47
2.01 / 07-2017




                                       Scanning Units .................................................................................................. H-49
                                       Scanning in Dispatch ......................................................................................... H-51
                                       Scanning Registration Points ............................................................................ H-53



                 A+W Production Barcode Manager                                                                                                              H-5
                 Contents




                              Truck Registration Point .................................................................................... H-56
                                   Exercises: ................................................................................................... H-57
                                   Exercise 1: Loading an empty and a partly loaded truck ............................ H-57
                              Scanning Racks and/or Boxes .......................................................................... H-59
                              Scanning the Status .......................................................................................... H-61
                              Correcting Erroneous Entries ............................................................................ H-62
                            Production Terminals ............................................................................................ H-63
                              Production Terminals ........................................................................................ H-64
                                 Introduction .................................................................................................... H-65
                            Reject Management .............................................................................................. H-67
                              Overview ........................................................................................................... H-68
                                 Reject Handling (Internal) .............................................................................. H-69
                            Statistics, Reporting and Monitoring ..................................................................... H-71
                              Overview ........................................................................................................... H-72
                              Barcode Reporting ............................................................................................ H-73
                                 Loading the Reports ....................................................................................... H-73
                                 Examples of Standard Barcode Reports ........................................................ H-73
                                   Unit list ........................................................................................................ H-74
                                   Order overview ........................................................................................... H-74
                                   Order status ................................................................................................ H-75
                                   Loading list ................................................................................................ H-76
                                   Rack load per lite ........................................................................................ H-77
                                   Rack load per item ...................................................................................... H-78
                                   Booking history ........................................................................................... H-78
                              Monitoring: A+W Dashboard ............................................................................. H-79
                                 Overview ........................................................................................................ H-80
                              Statistics: A+W Discovery ................................................................................. H-82
                                 Overview ........................................................................................................ H-83

                            Software Reference                                                                                               H-85
                            Overview ............................................................................................................... H-87
                            Master Data .......................................................................................................... H-88
                             Barcode Options ................................................................................................ H-89
                             Barcode Types .................................................................................................. H-90
                             Registration Point Types ................................................................................... H-91
                             Registration Points ............................................................................................ H-92
                             Racks ................................................................................................................ H-96
                             Rack Filter ......................................................................................................... H-99
                             Status Types ................................................................................................... H-100
                             Status Values .................................................................................................. H-101
                             Employees ....................................................................................................... H-103
                             Column Assignment ........................................................................................ H-105
                             Columns .......................................................................................................... H-106
                             Post-Processing .............................................................................................. H-107

                            Partindex                                                                                                           H-1
                            Index Barcoding ...................................................................................................... H-3
2.01 / 07-2017




                 H-6                                                                           A+W Production Barcode Manager
Barcoding               H

                    Tutorial




            A+W Production
                 Tutorial                                                                                      Overview




                                      Overview
                                      The target group of this training session concerning the A+W Production mod-
                                      ule are employees who are working at different stations (machines and regis-
                                      tration points) within production.
                                      The benefit for the customers is that they can directly control their machines.
                                      There are no downtimes due to having to digitalize a shape at a processing
                                      machine. It is furthermore not necessary to enter any NC codes at the machine
                                      which also means continuous machine deployment.

                                          The functions depend on the enabled modules
                                          Please note that the individual functions are available only if the corre-
                                          sponding modules and interfaces have been installed and enabled.

                                          If you detect functions in this description that are not available in your ver-
                                          sion, please contact A+W Software GmbH.

                                      Subjects
                                      This tutorial offers the following subjects:
                                      •   Basic Ideas
                                      •   Booking Elements
                                      •   Data Entry
                                      •   Statistics, Reporting and Monitoring

                                      Required knowledge
                                      This tutorial addresses participants who work at different stations (areas, ma-
                                      chines and registration points) within Production. The participants must be fa-
                                      miliar with the concepts of production terminals and scanners.

                                          Required knowledge
                                          Basic IT knowledge and/or Windows knowledge are prerequisites for using
                                          A+W Production.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                     H-9
                 Overview                                                                                 Tutorial




                            Documentation
                            For your training on the Barcode Manager, the following documents are avail-
                            able:

                            HTML                       Tutorial and Software Reference

                            Handout                    Printout of training document for participants

                            PDF                       Complete documentation
                                                       Tutorial
                                                       Software Reference

                            Online help <F1>           Context-sensitive dialog help in the A+W Production
                                                       Software Reference.


                            Tutorial Structure
                            This tutorial consists of subjects with several training modules each. Each
                            module consists of the following elements:

                            Overview                  Each training module starts with an overview of the
                                                      major topics:
                                                       • Objectives: What shall be conveyed?
                                                       • Benefit: What can this knowledge be used for?
                                                       • Maxims: Which correlations are to be remembered?

                            Concepts                   First, the concepts and terms of the corresponding
                                                       training module will be explained. This is followed by
                                                       examples and instructions.

                            Exercises                  • For some of the training modules, exercises with
                                                         certain tasks and suggested solutions are available.
                                                       • These exercises will help you to understand and
                                                         learn to apply A+W Production.

                            Cross reference section    At the end of each training module there is a section
                                                       with cross references pointing to corresponding
                                                       descriptions in the software reference.
                                                       This will help you to extend your newly acquired
                                                       knowledge.

                            Reading tip               The contents of a training module are based on the
                                                      knowledge conveyed in the previous module. We
                                                      therefore recommend not to skip any training modules.
                                                       If you are already familiar with a subject you should at
                                                       least read the summary at the start of a training module
                                                       in order to bring the main details to mind.


                            In the practice section of each training unit, the software reference and the ex-
2.01 / 07-2017




                            ercise section are systematically included by means of cross references. This
                            results in a central theme throughout the entire documentation.




                 H-10                                                    A+W Production Barcode Manager
                 Tutorial                                                                                   Overview




                                      Display Conventions
                                      Certain parts of sentences are specially marked. The meanings are:

                                      Italics                 Marks character strings referring to software elements,
                                                              e.g. the Global Shape Data dialog.

                                      Bold                    Marks phrases to be entered via the keyboard, e.g. the
                                                              number 0.

                                      >                       The so-called breadcrumb path shows how to open a
                                                              dialog, e.g. File > Import > Transfer file.

                                      []                      Square brackets mark buttons in a dialog, e.g. [OK] to
                                                              save the entries.

                                      <>                      Angle brackets refer to keys or shortcuts on the
                                                              keyboard, e.g. <F1> is used to open the online help.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                  H-11
                 Basic Ideas                                                                          Tutorial




                               Basic Ideas
                               This documentation shall give you an idea of Barcoding process and module
                               in A+W Production and a basic understanding of this subject. Moreover, we
                               will explain the basics of A+W Production, the tools used, and the general pos-
                               sibilities and limits.
                               We strongly recommend to refer to detailed documentation on control stations
                               (production terminals), internal A+W Production installation and configuration
                               instructions, scanner installation, configuration, etc. These subjects will be
                               mentioned in this documentation, but not handled in detail. A clear restriction
                               of the areas is not always possible, and not required either.
                               These instructions are not a substitute for basic knowledge about production
                               structures, the production terminals used, scanners or other A+W software.

                               Document structure
                               This documentation describes general knowledge on A+W Production. What
                               is A+W Production, the most important components, registration points, which
                               scanner types are used, procedures, etc.
2.01 / 07-2017




                 H-12                                                    A+W Production Barcode Manager
                 Tutorial                                                                                   Basic Ideas




                                      Barcoding
                                      A+W Production is a general term for collecting current data about statuses
                                      and processes in companies.
                                      It gathers the flow of production at the most important places within production,
                                      the so-called registration points and thus maps the process flow of your pro-
                                      duction. This is achieved by means of, e.g. barcodes, scanners, Production
                                      Terminals (control stations), etc. Directly or indirectly, the gathered data is
                                      transferred to an appropriate collection point (AWPort) and saved in the data-
                                      base (A+W Production DB).


                                      Purpose of A+W Production
                                      First of all, A+W Production is used to display the current situation. Starting
                                      from determining the production status of an order, and tracking the product
                                      through production to displaying the performance.
                                      In the case of rejects, apart from the registration point, the reject reason is en-
                                      tered. Corresponding subsequent parts can be created automatically, depend-
                                      ing on the configuration. Machine control is also executed automatically based
                                      on barcode readings.
                                      Another important aspect of A+W Production are the statistical analyses. You
                                      can analyze the productivity and machine times, monitor production mistakes
                                      (e.g. reject) and are provided with quality assurance thanks to the batch data
                                      collection.
                                      A+W Discovery enables you to create long-term analyses that are available for
                                      future planning.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                    H-13
                 Booking Elements                                                                        Tutorial




                                    Booking Elements
                                    This subject shows you how to handle the different objects of A+W Production.
                                    This includes the following training modules:
                                    •   “Products” on page H-15
                                    •   “Booking Places” on page H-18
                                    •   “Racks” on page H-26
                                    •   “Staff” on page H-32
                                    •   “Status” on page H-36
2.01 / 07-2017




                 H-14                                                         A+W Production Barcode Manager
                 Tutorial                                                                               Booking Elements




                                      Products
                                      Objectives

                                      • Getting familiar with objects of A+W Production.
                                      • What can and what cannot be tracked


                                      Definitions

                                      Direct objects              Have a barcode and are booked directly.

                                      Indirect objects            Do not have a barcode because they are automatically
                                                                  included when booked.


                                      Note

                                      Traceable products          All parts of a bill of materials onto which a barcode can
                                                                  be applied.

                                      Single lite A+W Production Every BOM element is identified by its own barcode.

                                      Quantity A+W Production     All parts of a BOM element have the same barcode.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                        H-15
                 Booking Elements                                                                             Tutorial




                                    Basics
                                    A+W Production differentiates between two object types:
                                    •   Direct objects
                                    •   Indirect objects

                                    Direct objects
                                    Direct objects are those that have a barcode and can be booked directly. They
                                    include:
                                    •   Registration points (places, trucks and machines)
                                    •   Racks and boxes
                                    •   Lites and units
                                    •   Status values / statuses
                                    •   Employees

                                    Indirect objects
                                    Indirect objects are those that are automatically included when booked. They
                                    include:
                                    •   Processing
                                    •   Batch information


                                    Lites or Units
                                    Lites and units are traceable products. These are always all the parts of a bill
                                    of materials onto which a barcode can be affixed. Example: Single lite, IG, LA-
                                    MI, frame, muntin, etc.
                                    In single lite A+W Production (default), every BOM element is identified by a
                                    unique barcode. This enables you to determine the exact location and status
                                    of a part.
                                    In quantity A+W Production, all parts of a BOM element have the same bar-
                                    code. As a result, it is no longer possible to determine the exact location and
                                    status of a part. Here, quantity statements are only made in relation to produc-
                                    tion statuses. Accordingly, the booking effort is a lot less.
                                    In contrast to the aforementioned parts, there are parts that cannot be tracked.
                                    These include, e.g. gas, butyl, silicone, foils, etc.
                                    To get an optimum data basis, it is therefore essential to book single lites/units
                                    to the corresponding registration point or rack in Production.
2.01 / 07-2017




                 H-16                                                           A+W Production Barcode Manager
                 Tutorial                                                                            Booking Elements




                                      Booking types
                                      We distinguish between three booking types:
                                      •   Movement bookings:
                                          Movement bookings record the change of location of a rack, unit or lite.
                                          This may be a rack (e.g. unit on rack) or a registration point (rack or unit on
                                          registration point).
                                      •   Processing bookings:
                                          Processing bookings register processing steps (e.g. drilling) for units.
                                      •   Status bookings (e.g. rejects, maintenance):
                                          Status bookings represent the change of status of an object.
                                      Processing and status bookings can also be triggered implicitly, through move-
                                      ment bookings.
                                      Naturally, reject registration is important in this connection. Apart from the reg-
                                      istration point and other information, the reject reason is entered. Subsequent
                                      parts can be generated automatically, depending on the configuration.
                                      The gathered data can be used for analysis, statistics, and inventory purpos-
                                      es, among other things (e.g. barcode reports, MS-Excel, etc.). It is used for
                                      production control, lite/unit and rack tracking and many other purposes.


                                      Additional information
                                       “Reject Management” on page H-67
                                       “Barcode Reporting” on page H-73
                                       “Scanning Units” on page H-49
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                    H-17
                 Booking Elements                                                                                  Tutorial




                                    Booking Places
                                    Objectives

                                    • Acquire knowledge about the Registration Points dialog.
                                    • Getting familiar with and understanding the Error Rack registration point.
                                    • Getting familiar with and understanding the Dispatch registration point.


                                    Benefits

                                    In order to avoid booking mistakes, it is necessary to observe the correct booking
                                    order.


                                    Definitions

                                    RP                          Short for registration point

                                    Registration points         Stations within production or dispatch.

                                    Error rack                  An internal registration point with the registration point
                                                                number 12 and is filled automatically. This registration
                                                                point will include all units which – because of errors –
                                                                have lost their allocation to a physical rack or a physical
                                                                registration point.

                                    Trigger time                The time defined in the system which determines the
                                                                point in time from which the truck load is considered to
                                                                be shipped. It is enabled by the status booking <Start>
                                                                <Truck>. The time can be configured in the system.


                                    Note

                                    Registration points         Have a unique number and a name.
2.01 / 07-2017




                 H-18                                                             A+W Production Barcode Manager
                 Tutorial                                                                         Booking Elements




                                      Registration Points
                                      All stations within production (production areas, trucks, machines) that are
                                      equipped with scanners and/or Production Terminals are called registration
                                      points (RP). They have a unique number and a name.
                                      A machine does not necessarily have to be one registration point. It can also
                                      be subdivided into several registration points.
                                      Example: IG line
                                      •   1611 > machine entry,
                                      •   1610 > the machine itself and
                                      •   1612 > machine exit.
                                      Splitting machines into several registration points allows detailed production
                                      tracking and analysis.
                                      You can book racks, products and statuses to these registration points. The
                                      more registration points you have, the more detailed your analyses will be.




                                      Fig. H-1     Registration points


                                      The table above shows which registration points have already been created.
                                      You can create new registration points or change already created registration
                                      points.
                                      The checkboxes in the Feedback of Bookings section are for production feed-
                                      back that are used to update the current order status in the upper-level order
                                      processing system.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                H-19
                 Booking Elements                                                                              Tutorial




                                    You will find a detailed description of the individual fields in the software refer-
                                    ence.

                                        Column headers can be configured as desired
                                        The headers of the individual columns can be configured as desired. It is
                                        therefore possible that the headers shown here do not correspond to the
                                        headers in your installation.

                                    Error rack
                                    The error rack is an internal registration point. This registration point will in-
                                    clude all units which – because of errors – have lost their allocation to a phys-
                                    ical rack or a physical registration point.
                                    The internal registration point Error Rack has registration point number 12.
                                    Registration point 12 follows the same rules as any other registration point (re-
                                    ports, bookings, corrections, etc.).
                                    Basically, there are two rules for the Error Rack registration point:
                                    •   Rule 1: The error rack should always be empty!
                                    •   Rule 2: If the error rack is not empty, there must be an operation or scanner
                                        error.

                                    How do units get onto the error rack?
                                    There are several reasons. Apart from a defective scanner/label, this is usually
                                    due to operating errors by the staff.
                                    The error rack is used whenever a registration point or rack is scanned with
                                    the status <Start> while according to A+W Production, this object still holds
                                    units. These units are automatically assigned to the Error Rack registration
                                    point.

                                    Possible causes:
                                    Example 1:
                                    Several racks are being used at a registration point. A physical rack has been
                                    registered with the scanner; units are booked to this rack <Rack 1> <Unit 1>
                                    <Unit 2>. When changing to the second rack, the user forgets to scan/register
                                    this rack. The units are actually placed onto rack 2 but booked to the wrong
                                    rack, namely rack 1.
                                    If rack 1, which has been correctly loaded, is processed as usual during the
                                    production process, this rack will be empty and ready for other tasks.
                                    According to the scanning rules, rack 1 will be scanned with <Start> <Rack1>
                                    next time. This resets the rack in barcoding to empty.
                                    Internally (according to bookings), rack 1 still held the erroneously scanned
                                    (allocated) units from rack 2 (see above). These units are automatically
                                    booked to the Error Rack registration point.
2.01 / 07-2017




                                    Example 2:
                                    A truck is loaded correctly. When all units, racks, and boxes have been loaded,
                                    the truck should get the status Shipped <Shipped><Truck1>.


                 H-20                                                            A+W Production Barcode Manager
                 Tutorial                                                                           Booking Elements




                                      This is omitted. The truck delivers the goods and is available (empty) for the
                                      next transport on the next day.
                                      According to the scanning rules, it is registered for loading by
                                      <Start><Truck1>, and reset (empty).
                                      As the truck is still considered loaded (according to bookings) because of the
                                      missing <Shipped> booking of the previous day, its entire load is booked to
                                      registration point 12 (Error Rack) by the <Start> status booking.
                                      Example 3:
                                      A loaded rack is unloaded without being scanned, or scanned by a defective
                                      scanner. Physically, the rack is empty, but according to barcoding, it is still
                                      loaded. The next time the rack is used, in adherence to the scanning rules
                                      <Start><Rack>, these units will be booked to registration point 12, Error Rack.

                                      Removing units from the error rack
                                      The error rack is an internal registration point. As on any other registration
                                      point, units on this rack can be changed by new bookings.
                                      There are two methods of booking units from one registration point (in this
                                      case the error rack) to another registration point/rack.
                                      The manual method is carried out via the Production Terminal Edit. You must
                                      execute the changes to the registration point (of the rack) manually by using
                                      the Production Terminal Edit.
                                      The automatic method corrects an error automatically by another correct
                                      booking during the production process.

                                         Tip
                                         Check the internal registration point 12 (Error Rack) regularly, and make
                                         corrections right away. Apart from the Production Terminal Edit, the Bar-
                                         code Manager reports are available for checking purposes.
                                          “Barcode Reporting” on page H-73
                                         Please remember: from the barcoding point of view, this is a registration
                                         point. You can use the same functions and tools for analyses and correc-
                                         tions as for any other registration point!
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                  H-21
                 Booking Elements                                                                            Tutorial




                                       Check why the units were booked to the error rack and prevent these errors
                                       if possible.

                                       Many units on the error rack
                                       If there are many units on the internal registration point 12 Error Rack,
                                       please contact the A+W customer service. A+W will analyze the reasons
                                       together with you and work out a customized and practical solution.

                                    Correct booking
                                    Units moved to the internal registration point 12, Error Rack, will be automati-
                                    cally removed from the Error Rack with the next correct booking of these units
                                    at another registration point. They will be assigned to this registration point/
                                    rack and vanish from the Error Rack registration point.
                                    Example:
                                    A loaded rack is unloaded without being scanned, or scanned by a defective
                                    scanner. Physically, the rack is empty, but according to barcoding, it is still
                                    loaded.
                                    The next time the rack is used complying with the scanning rules <Start>
                                    <Rack>, these units will be booked to the Error Rack (only applies to units
                                    which have not been registered again in the meantime, see below!).
                                    Prerequisite for automatic correction is that the units are still being produced
                                    and will be scanned during further processing.
                                    Every scan allocates the unit to the corresponding registration point/rack; the
                                    unit automatically vanishes from the internal registration point 12, Error Rack.


                                    Additional information
                                     “Scanning in Dispatch” on page H-51
                                     “Scanning Registration Points” on page H-53
2.01 / 07-2017




                 H-22                                                          A+W Production Barcode Manager
                 Tutorial                                                                            Booking Elements




                                      Managing Registration Points
                                      This module will show you how to create new registration points and edit or
                                      delete them.
                                      The following instructions exist for this training module:
                                      •   “How to create a new registration point” on page H-23
                                      •   “How to delete a registration point” on page H-24
                                      •   “How to make changes to registration points” on page H-24


                                       How to create a new registration point
                                      1 Open the Registration Points dialog.
                                      2 Press the icon button [New].
                                      3 Enter a unique registration point number in the Registration Point Number
                                        field.
                                      4 Enter the barcode number for the registration point in the Barcode field.
                                      5 Enter the registration point name in the Name field.
                                      6 The Description field allows you to enter information regarding the registra-
                                        tion point.
                                      7 Enter the text that is to be displayed in the production lists in the Text for
                                        Production Lists field.
                                      8 Enter the text that is to be displayed in the customer lists in the Text for Cus-
                                        tomer Lists field.
                                      9 Enter the text that is to be displayed underneath the barcode in the Subrow
                                        for Barcode Labels field.
                                      10 Select the type of the registration point from the Registration Point Type
                                         combo box.
                                      11 Using the Grouping field, you can define a different grouping to be used for
                                         analyses apart from the registration point type.
                                      12 In the Grouping for Working Shifts field you can group individual registra-
                                         tion points for working shifts.
                                      13 Select the corresponding status from the combo box in the Current Status
                                         field.
                                      14 If a restriction check has been defined for the registration point, it will be
                                         activated and controlled via the Restriction combo box.
                                      15 The Over Quantities field is in direct connection with the Restriction field.
                                         You can define the corresponding value in percentage only if the Restric-
                                         tion field has one.
                                      16 Activate the Show Produced Parts checkbox if completely produced lites
                                         should be shown on the Production Terminal.
2.01 / 07-2017




                                      17 If the registration point deviates from the registration point from order entry,
                                         please overwrite the entry.




                 A+W Production Barcode Manager                                                                    H-23
                 Booking Elements                                                                          Tutorial




                                    18 Activate the Processing Feedback checkbox if the processing progress
                                       should be reported to the order processing system precise to the lite.
                                    19 Activate the Rack Feedback checkbox if the rack load should be reported
                                       to the order processing system.
                                    20 Activate the Report Rack Load to Rack Server checkbox if the rack load
                                       should be reported to the rack server.
                                    21 Activate the Unit Feedback checkbox.
                                    22 Activate the Production Feedback checkbox if feedback on the order items
                                       should be sent to the order processing system.
                                    23 Click on the icon button [Save] to save the entries.


                                     How to delete a registration point
                                    1 Open the Registration Point dialog.
                                    2 Select the registration point that is to be deleted from the list.
                                    3 Press the icon button [Delete].
                                    4 The system queries whether the record shall actually be deleted.
                                    5 Click on [Yes]. The record will be deleted.


                                     How to make changes to registration points
                                    1 Open the Registration Point dialog.
                                    2 Select the registration point that is to be changed from the list.
                                    3 Press the icon button [Change]. The dialog will be released for editing.
                                    4 Carry out the required changes.
                                    5 Click on the icon button [Save] to save the entries.


                                    Additional information
                                     Software Reference, “Registration Points” on page H-92
2.01 / 07-2017




                 H-24                                                          A+W Production Barcode Manager
                 Tutorial                                                                            Booking Elements




                                      Truck registration point
                                      Each truck is a registration point which follows the same rules as any other
                                      registration point. An exception is the emptying of a truck via barcodes. Ob-
                                      jects (racks/boxes, etc.) usually leave a registration point by being registered
                                      at another registration point. This does not make sense for trucks, for practical
                                      reasons. It would have to be scanned when the units are unloaded, e.g. at the
                                      construction site.
                                      The objects must be booked off this registration point and transferred to the
                                      internal registration point 11 (Off Site) by means of another barcode mecha-
                                      nism. However, this booking must be made only after the truck has been re-
                                      turned fully unloaded!
                                      To avoid a complex technical structure with scanners at the gates, the booking
                                      to registration point 11 (Off Site) is made after a time period defined in the sys-
                                      tem, when the truck is registered after its return by <Start><Truck>.
                                      The time period is triggered by scanning the status <Shipped> <Truck> for the
                                      corresponding truck and/or its load.
                                      Within this time period, the load is considered as not shipped and is still
                                      booked to registration point <Truck> with status <Shipped>. Only after a
                                      START registration, AFTER a defined period, the registration point changes to
                                      11.
                                      The status booking <Start><Truck> would reset the truck and/or the racks, and
                                      move the units involved to the error rack!
                                      After the defined time period, all units are considered to be shipped, and are
                                      booked to the internal registration point 11 with status <Shipped>; the racks
                                      and/or the truck can be used again in the production process.


                                      Additional information
                                       Software Reference, “Registration Points” on page H-92
                                       “Truck Registration Point” on page H-56
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                    H-25
                 Booking Elements                                                                                 Tutorial




                                    Racks
                                    Objectives

                                    • Acquire knowledge about the Racks dialog.
                                    • Getting familiar with and understanding the booking process.


                                    Benefits

                                    In order to understand barcoding, you must know what can be booked to the racks.


                                    Definitions

                                    Rack types                 Rack types in barcoding include A racks, L racks, harp
                                                               racks, boxes and the specific racks for furnace beds and
                                                               autoclaves.


                                    Note

                                    Book rack                  When a rack is booked to a registration point, all units on
                                                               the rack will be automatically booked to this registration
                                                               point as well.

                                    Create racks               Racks can be created in the master data manually or
                                                               automatically.

                                    Book                       You can book products or statuses to racks.

                                    Where is a rack located    A rack is always located at one location (registration
                                                               point)

                                    Boxes                      Boxes are not returned to the production cycle.
2.01 / 07-2017




                 H-26                                                            A+W Production Barcode Manager
                 Tutorial                                                                            Booking Elements




                                      Racks
                                      Use this section to create racks for A+W Production. The following rack types
                                      are available:
                                      •   A racks
                                      •   L racks
                                      •   Harp racks
                                      •   Boxes
                                      At some registration points, special racks are required. These are usually the
                                      furnaces and autoclaves.
                                      You can book products or statuses to the racks. A rack is always located at
                                      one location in production (registration point).




                                      Fig. H-2     Racks


                                      The screenshot above shows which racks have already been created. You can
                                      create new racks or change already created racks.

                                      Filter racks
                                      If you have a large quantity of racks, you can create filters to restrict the dis-
                                      played racks. You can see in the upper section of the dialog whether a filter
                                      has been set.
                                      If a filter has been set, the following is displayed:



                                      Fig. H-3     Rack filter is set
2.01 / 07-2017




                                      If no filter has been set, the following is displayed:




                 A+W Production Barcode Manager                                                                    H-27
                 Booking Elements                                                                                Tutorial




                                    Fig. H-4      No rack filter set


                                    In order to activate a filter, click on the button [Filter]. The Rack filter dialog
                                    opens in which you can define and activate the corresponding filter.
                                    You will find a detailed description of the individual fields in the software refer-
                                    ence.

                                       Column headers can be configured as desired
                                       The headers of the individual columns can be configured as desired. It is
                                       therefore possible that the headers shown here do not correspond to the
                                       headers in your installation.


                                    Boxes
                                    At first, boxes are treated like racks but they are not returned to the production
                                    cycle. It is therefore useful to use a separate number area for the barcodes.
                                    This barcode area should always be printed and used up completely. This en-
                                    sures that a barcode cannot be used several times in Production simultane-
                                    ously.
                                    You can, of course, also print and use up a succession of several smaller ar-
                                    eas, e.g. 9000-9099 followed by 9100-9199, 9200-9299, etc., but you should
                                    always use the entire number area up to 9999.
                                    The booking history for the boxes still remains expressive if the area is used
                                    to its full extent and barcodes repeat themselves after quite a long time.

                                       Creating barcodes
                                       Always use the report for barcode creation. Alternatively, barcodes can be
                                       supplied by a Microsoft Word document.


                                    Additional information
                                     Software Reference, “Racks” on page H-96
                                     Software Reference, “Rack Filter” on page H-99
                                     “Barcode Reporting” on page H-73
                                     “Scanning Racks and/or Boxes” on page H-59
2.01 / 07-2017




                 H-28                                                             A+W Production Barcode Manager
                 Tutorial                                                                          Booking Elements




                                      Managing Racks
                                      This module will show you how to create new racks and to edit or delete them.
                                      The following instructions exist for this training module:
                                      •   “This is how you create one new rack” on page H-29
                                      •   “This is how you create several new racks at once” on page H-29
                                      •   “How to delete a rack” on page H-30
                                      •   “How to make changes to a rack” on page H-30


                                       This is how you create one new rack
                                      1 Open the Racks dialog.
                                      2 Press the icon button [New].
                                      3 Enter a unique name for the rack in the Name field.
                                      4 Enter the barcode for the rack in the Barcode field.
                                      5 Select from the Rack Base Type combo box to define whether the rack is
                                        a regular rack, a tray rack or a box.
                                      6 Select Rack Type from the combo box to define whether the rack is a A
                                        rack, a harp rack or special rack.
                                      7 If the rack is a tray rack, enter the first and last number to be used in the
                                        Slot Number from to field.
                                      8 Assign the base registration point to the rack in the Base Reg. Point field.
                                      9 Activate the Temporary Rack checkbox if the rack is a temporary rack.
                                      10 Click on the icon button [Save] to save the entries.


                                       This is how you create several new racks at once
                                      1 Open the Racks dialog.
                                      2 Press the icon button [New].
                                      3 Activate the Create several racks checkbox. Underneath the checkbox, the
                                        fields Prefix, Start Value, End Value and BC Start Value are displayed.
                                      4 In the Prefix field you can enter a letter or letter combination that precedes
                                        the start value.
                                      5 Enter the first number for the racks in the Start Value field.
                                      6 Enter the last number for the racks in the End Value field.
                                      7 In the BC Start Value field, enter the barcode number that should be started
                                        with.
                                      8 Select from the Rack Base Type combo box whether the racks are regular
                                        racks, tray racks or boxes.
                                      9 Select from the Rack Type combo box whether the racks are A racks, harp
2.01 / 07-2017




                                        racks or special racks.




                 A+W Production Barcode Manager                                                                 H-29
                 Booking Elements                                                                            Tutorial




                                    10 If the racks are tray racks, enter the first and last number to be used in the
                                       Slot Number from to field.
                                    11 Assign the base registration point to the racks in the Base Reg. Point field.
                                    12 Activate the Temporary rack checkbox if the racks are temporary racks.
                                    13 Click on the icon button [Save] to save the entries.
                                    14 A query is displayed asking you if you really want to insert the correspond-
                                       ing number of racks.


                                     How to delete a rack
                                    1 Open the Racks dialog.
                                    2 Select the rack that is to be deleted from the list.
                                    3 Press the icon button [Delete].
                                    4 The system queries whether the record shall actually be deleted.
                                    5 Click on [Yes]. The record will be deleted.


                                     How to make changes to a rack
                                    1 Open the Racks dialog.
                                    2 Select the rack that is to be changed from the list.
                                    3 Press the icon button [Change]. The dialog will be released for editing.
                                    4 Carry out the required changes.
                                    5 Click on the icon button [Save] to save the entries.


                                     How to set a rack filter
                                    1 Open the Racks dialog.
                                    2 Click on the button [Filter]. The Rack Filter dialog opens.
                                    3 You can filter by the following criteria:
                                       •   Registration point types
                                       •   Registration points
                                       •   Rack name
                                       •   Rack base type
                                       •   Rack type
                                    4 Carry out the required settings.
                                    5 Click on the button [Accept] to save the entries.
                                    6 Click on [X] to close the dialog.
2.01 / 07-2017




                 H-30                                                             A+W Production Barcode Manager
                 Tutorial                                                                         Booking Elements




                                       How to delete a rack filter
                                      1 Open the Racks dialog.
                                      2 Click on the button [Filter]. The Rack Filter dialog opens.
                                      3 Click on the button [Reset] to clear set filters.
                                      4 Click on [X] to close the dialog.
                                      5 All racks are shown again.


                                      Additional information
                                       Software Reference, “Racks” on page H-96
                                       Software Reference, “Rack Filter” on page H-99
                                       “Scanning Racks and/or Boxes” on page H-59
2.01 / 07-2017




                 A+W Production Barcode Manager                                                              H-31
                 Booking Elements                                                                               Tutorial




                                    Staff
                                    Objectives

                                    • Acquire knowledge about the Employees dialog.
                                    • Getting familiar with and understanding how to manage employees.
                                    • Create and edit employees


                                    Benefits

                                    You can define different cost rates for each employee. This enables you to take a
                                    closer look at personnel costs. In addition, you can analyze how many employees
                                    were involved in processing.


                                    Note

                                    Create employees            An employee must first be created before he can log on
                                                                at a station.

                                    Registered person           Is included with the booking. This is the employee
                                                                responsible for the booking. The registered person
                                                                remains registered until another name barcode is
                                                                scanned.

                                    Registration mandatory      The scanner and A+W Production date can be set so
                                                                that user registration is mandatory.
2.01 / 07-2017




                 H-32                                                            A+W Production Barcode Manager
                 Tutorial                                                                             Booking Elements




                                      Employees
                                      All employees in your company who work with A+W Production must be reg-
                                      istered. After an employee has been registered, he can log on at the individual
                                      stations. His name is then automatically included in the individual bookings
                                      and he is the employee responsible for this booking.




                                      Fig. H-5      Employees


                                      The table above shows which employees have already been created. You can
                                      create new employees or change already created employees.
                                      You can define different cost rates for each employee. This enables you to
                                      take a closer look at the respective personnel costs.
                                      In addition, it is possible that several employees are registered for one station.
                                      Accordingly, you will know how many employees were involved in processing.
                                      You will find a detailed description of the individual fields in the software refer-
                                      ence.

                                         Column headers can be configured as desired
                                         The headers of the individual columns can be configured as desired. It is
                                         therefore possible that the headers shown here do not correspond to the
                                         headers in your installation.


                                      Additional information
                                       Software Reference, “Employees” on page H-103
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                    H-33
                 Booking Elements                                                                        Tutorial




                                    Managing Employees
                                    This module will show you how to create new employees and edit or delete
                                    them.
                                    The following instructions exist for this training module:
                                    •   “How to create a new employee” on page H-34
                                    •   “How to delete an employee” on page H-34
                                    •   “How to make changes to employee data” on page H-35


                                     How to create a new employee
                                    1 Open the Employees dialog.
                                    2 Press the icon button [New].
                                    3 Enter a unique number for the employee in the Number field.
                                    4 Enter the name of the employee in the Name field.
                                    5 The Description field allows you to enter information about the employee.
                                    6 Enter the employee's personnel number in the Personnel No. field. This
                                      number can be requested from the Payroll office or Accounting.
                                    7 Enter the barcode number for the employee in the Barcode field. In the
                                      case of a 9-digit barcode, this might be the combination of the Number and
                                      Personnel No. fields. Example: the employee has number 60, the person-
                                      nel number is 51 – this results in the barcode 600000051.
                                    8 Click on the icon button [Save] to save the entries.


                                     How to delete an employee
                                    1 Open the Employees dialog.
                                    2 Select the employee who is to be deleted from the list.
                                    3 Press the icon button [Delete].
                                    4 The system queries whether the record shall actually be deleted.
                                    5 Click on [Yes]. The record will be deleted.
2.01 / 07-2017




                 H-34                                                          A+W Production Barcode Manager
                 Tutorial                                                                         Booking Elements




                                       How to make changes to employee data
                                      1 Open the Employees dialog.
                                      2 Select the employee who is to be changed from the list.
                                      3 Press the icon button [Change]. The dialog will be released for editing.
                                      4 Carry out the required changes.
                                      5 Click on the icon button [Save] to save the entries.


                                      Additional information
                                       Software Reference, “Employees” on page H-103
2.01 / 07-2017




                 A+W Production Barcode Manager                                                              H-35
                 Booking Elements                                                                                Tutorial




                                    Status
                                    Objectives

                                    • Acquire knowledge about the Status Values dialog.
                                    • Getting familiar with and understanding different status values


                                    Benefits

                                    In order to obtain meaningful analyses, a certain booking discipline must be adhered
                                    to.


                                    Definitions

                                    Status values               Describe the status of an object

                                    Machine status              Ready, off, malfunction, maintenance, break, …

                                    Product status              Reject, deficiency, …

                                    Rack status                 Empty, ready, shipped, …

                                    Registration point status   Ready, shipped, empty, …

                                    Action status               OK, abort, accept, …


                                    Note

                                    Interruptions               Work interruptions must always be logged.
2.01 / 07-2017




                 H-36                                                             A+W Production Barcode Manager
                 Tutorial                                                                           Booking Elements




                                      Status values
                                      Recording the actual object status within production is the basic principle of
                                      A+W Production.
                                      In order to obtain meaningful data analyses, the master data must be main-
                                      tained and it is absolutely necessary to book data (quantities and objects) cor-
                                      rectly and promptly.
                                      Status values affect the following A+W Production objects:
                                      •   Unit/group
                                      •   Rack
                                      •   Registration points
                                      •   Staff

                                      Unit/group
                                      The purpose of this is to enter the status of a lite and/or unit or a product.
                                      The following status values are available for example:
                                      •   Not yet produced
                                      •   Reject
                                      •   Defect
                                      •   Ready for shipment

                                      Rack
                                      The purpose of this is to enter the status of a rack.
                                      Racks can have the following statuses, for example:
                                      •   Empty
                                      •   Full
                                      •   Off site
                                      •   Ready for shipment

                                      Registration point
                                      The purpose of this is to enter the status of a registration point.
                                      Registration points can have the following statuses for example:
                                      •   Start
                                      •   To
                                      •   Off
                                      It may be necessary to interrupt work at a registration point during an ongoing
                                      production process. These interruptions must always be logged.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                   H-37
                 Booking Elements                                                                              Tutorial




                                    Possible reasons for an interruption:
                                    •   Machine maintenance
                                    •   Machine failure
                                    •   Breaks
                                    •   Set-up times

                                    Action barcode
                                    Apart from entering the aforementioned status values, it is also possible to
                                    scan different actions.
                                    They include, e.g.:
                                    •   OK
                                    •   Cancel
                                    •   Rotate
                                    •   Next row




                                    Fig. H-6       Status values


                                    The table above shows which status values have already been created. You
                                    can create new status values or change already created status values.
                                    You will find a detailed description of the individual fields in the software refer-
                                    ence.

                                        Column headers can be configured as desired
                                        The headers of the individual columns can be configured as desired. It is
                                        therefore possible that the headers shown here do not correspond to the
                                        headers in your installation.


                                    Additional information
                                     Software Reference, “Status Types” on page H-100
2.01 / 07-2017




                                     “Scanning the Status” on page H-61




                 H-38                                                            A+W Production Barcode Manager
                 Tutorial                                                                             Booking Elements




                                      Managing Status Values
                                      This module will show you how to create new status values and edit or delete
                                      them.
                                      The following instructions exist for this training module:
                                      •   “How to create a new status value” on page H-39
                                      •   “How to delete a status” on page H-39
                                      •   “How to make changes to status data” on page H-40


                                       How to create a new status value
                                      1 Open the Status Values dialog.
                                      2 Press the icon button [New].
                                      3 Enter a unique number for the status value in the Status Value Number
                                        field.
                                      4 Enter the name of the status value in the Name field.
                                      5 Enter information about the status value in the Description field, e.g. tool
                                        change.
                                      6 Enter the text that is to be displayed in the lists in the Text for Lists field.
                                      7 Enter the 9-digit barcode number for the status in the Barcode field.
                                      8 Select the required type from the Status Type combo box.
                                      9 Activate the AWRack Info checkbox if the rack server should be notified in
                                        the event of a change of this status.
                                      10 Select the required status from the AWRack Status combo box.
                                      11 Click on the icon button [Save] to save the entries.


                                       How to delete a status
                                      1 Open the Status Values dialog.
                                      2 Select the status that is to be deleted from the list.
                                      3 Press the icon button [Delete].
                                      4 The system queries whether the record shall actually be deleted.
                                      5 Click on [Yes]. The record will be deleted.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                     H-39
                 Booking Elements                                                                        Tutorial




                                     How to make changes to status data
                                    1 Open the Status Values dialog.
                                    2 Select the status that is to be changed from the list:
                                    3 Press the icon button [Change]. The dialog will be released for editing.
                                    4 Carry out the required changes.
                                    5 Click on the icon button [Save] to save the entries.


                                    Additional information
                                     Software Reference, “Status Types” on page H-100
                                     “Scanning the Status” on page H-61
2.01 / 07-2017




                 H-40                                                         A+W Production Barcode Manager
                 Tutorial                                                                               Data Entry




                                      Data Entry
                                      This subject shows you the methods and locations for entering data in produc-
                                      tion.
                                      This includes the following training modules:
                                      •   “Scanner” on page H-42
                                      •   “Barcodes” on page H-45
2.01 / 07-2017




                 A+W Production Barcode Manager                                                              H-41
                 Data Entry                                                                                 Tutorial




                              Scanner
                              Objectives

                              • Getting familiar with different scanners
                              • Getting to know and understanding their functionality
                              • The scanner configurations


                              Benefits

                              Using scanners will assist you in substantially reducing your workload and it saves
                              time.


                              Definitions

                              Online scanners             Do not have any memory and the scanner data must be
                                                          directly transmitted to the connected system. If the
                                                          connection is interrupted, scanned data will be lost.

                              Offline scanners            Have a memory which can temporarily save the scanned
                                                          data and transfers it when connected with the system.

                              Serial scanners             Are used at the terminals, for example. The scanner will
                                                          not save information temporarily, i.e. without connection
                                                          to the network, data will be lost.


                              Note

                              Configuration               Apart from their operating system, scanners need
                                                          software that performs the required functions.
2.01 / 07-2017




                 H-42                                                       A+W Production Barcode Manager
                 Tutorial                                                                                  Data Entry




                                      Scanner Types
                                      In barcoding, different scanner types are used. Basically, there are online and
                                      offline scanners.
                                      •   Online scanners:
                                      •   Offline scanners:
                                      Scanner selection is highly individual and depends on a variety of factors, e.g.:
                                      •   How many scanners with different logs shall be used?
                                      •   Where shall the scanners be used?
                                      •   Which operating radius do they have to cover?
                                      There are further factors that need to be discussed with the customer directly
                                      on site.

                                      Online scanners
                                      Online scanners include the line scanners and serial scanners which normally
                                      have no memory so that they have to transfer the scanned data directly to the
                                      connected system. If the connection is interrupted, scanned data will be lost.

                                      Denso scanners (WLAN)
                                      These scanners are WLAN-enabled and communicate directly with AWPort.
                                      They have a display and a buffer system for buffering data. Notifications to us-
                                      ers can be sent via the built-in display and the scanner's menu structure. If the
                                      data transfer is interrupted (e.g. outside the range of the receiving station),
                                      data will be temporarily saved in the scanner and transferred when the con-
                                      nection has been re-established. These scanners are used in the shipping ar-
                                      ea, for instance.




                                      Fig. H-7     Denso online scanner
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                  H-43
                 Data Entry                                                                             Tutorial




                              Serial scanners
                              The serial scanners are used at the Production Terminals or in connection with
                              AWPort-Light as free online scanners. In connection with the Production Ter-
                              minals, they are normally allocated to a fixed registration point (configurable)
                              and replace the keyboard. Bookings are made by the connected Production
                              Terminal.
                              With AWPort Light, these scanners can be used as free online scanners wher-
                              ever a Production Terminal is not required. These scanners are robust and
                              reasonably priced. However, they do not have a display or a temporary mem-
                              ory. Notifications to users can be issued only to a certain extent. As these
                              scanners normally do not have a buffer system, scanned data will be lost if the
                              data transfer is interrupted (e.g. outside the range of the receiving station).

                              Offline scanners
                              The use of offline scanners in an A+W Production environment is subject to
                              special restrictions. Offline scanners are barcode readers that collect barcode
                              registrations and transfer them together at a later stage. As the transfer usually
                              has to be released manually, data registered via offline scanners will be ana-
                              lyzed (much) later than that collected by online scanners.
                              These scanners require well-organized and disciplined working!

                              The scanner configurations
                              Scanner configurations are multi-layered. Apart from their operating system,
                              scanners need software that performs the required functions. This software is
                              supplied by A+W and has to be transferred to the scanner and configured
                              there.
                              Furthermore, scanners have to be registered with the A+W Production sys-
                              tem.
                              The necessary configuration steps are usually performed by A+W but can also
                              be executed by specially trained staff.

                                 Scanners in practice
                                 Currently, WLAN scanners type BHT800BW are deployed almost exclu-
                                 sively. The advantage of this type is that the collected data is always avail-
                                 able online.

                                 Documentation of configuration
                                 Documentation, including the customized configuration, is part of the proj-
                                 ect planning phase; it will be saved and kept on the customer’s computer.
2.01 / 07-2017




                 H-44                                                     A+W Production Barcode Manager
                 Tutorial                                                                                 Data Entry




                                      Barcodes
                                      Scanners usually require barcodes. Every person, registration point, rack, etc.
                                      gets a unique number which is encoded as a barcode for the scanner. These
                                      numbers are defined jointly by A+W Software GmbH and the customer during
                                      the project planning phase. These barcodes are provided, for example, by an
                                      A+W Production report.
                                      Should you need new barcodes for persons, registration points, or racks/box-
                                      es, start the report and print the required barcodes.


                                      Additional information
                                       Software Reference, “Barcode Options” on page H-89
                                       Software Reference, “Barcode Types” on page H-90
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                H-45
                 Booking Examples                                                                     Tutorial




                                    Booking Examples
                                    This subject shows you how to book correctly.
                                    This includes the following training modules:
                                    •   “Scanning Sequence” on page H-47
                                    •   “Scanning Units” on page H-49
                                    •   “Scanning in Dispatch” on page H-51
                                    •   “Scanning Registration Points” on page H-53
                                    •   “Truck Registration Point” on page H-56
                                    •   “Scanning Racks and/or Boxes” on page H-59
                                    •   “Scanning the Status” on page H-61
                                    •   “Correcting Erroneous Entries” on page H-62
2.01 / 07-2017




                 H-46                                                         A+W Production Barcode Manager
                 Tutorial                                                                           Booking Examples




                                      Scanning Sequence
                                      The following examples shall describe the scanning sequence to be obeyed.
                                      To keep the examples quite clear, we have refrained from showing the entire
                                      display chain, i. e. we assume that when units are scanned, the scanner has
                                      been registered at a registration point, the user has scanned his personal bar-
                                      code, etc. The total scanning sequence is the combination of the listed exam-
                                      ples, and depends on the registration point.
                                      When scanning, first of all, the scanner is always prepared for scanning by
                                      registering the person working with it (optional), registering the registration
                                      point at the scanner, followed by the other bookings, normally rack registration.
                                      Registration of the person, registration point, scanning the status, etc. only af-
                                      fects all future bookings such as scanning a unit which is then saved in the sys-
                                      tem with all this information by ALCIM Booking.


                                       Scanning sequence:
                                      1 The user operating the scanner should scan his personal barcode at the
                                        start of his shift/scanning. This information will be saved with every scan
                                        and serves for analysis purposes later. If this barcode is not scanned, a
                                        configurable default value will be saved in the database. A (new) name bar-
                                        code can be scanned anytime, even after the scanner has been registered
                                        at the registration point, e.g. when the operator at a registration point
                                        changes.
                                      2 The registration point where the scanner is used must always be known to
                                        the scanner. Every section, machine, truck registered as a registration
                                        point has its own barcode. These can be: cutting, IG line 1, IG line 2, fur-
                                        nace, dispatch, truck 1, truck 2, etc.
                                      3 The rack (box) where the units are stacked has to be scanned, i.e. regis-
                                        tered with the scanner. If there are several racks at the registration point,
                                        you always have to scan the rack to be currently loaded. Exception: In Dis-
                                        patch, units are also booked directly to the registration point (truck) (see
                                        also Special case truck).
                                      4 The units: After items 1-3 have been scanned, the units to be stacked or
                                        those whose status has changed (e.g. reject report) are scanned.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                   H-47
                 Booking Examples                                                                            Tutorial




                                    Description
                                    <Text> the text in pointed brackets shows the barcode to be scanned (regis-
                                    tration point, rack, status, unit, etc.).
                                    The row <Begin> <Rack> <Unit1> < Unit2> <Unit3 …> means: Scan the sta-
                                    tus <Begin>, then the rack <Rack> onto which the units should be placed and
                                    then all units <Unit> in the order in which they should be placed on this rack.

                                       Caution with barcode <Begin>
                                       The barcode <Begin> always resets the rack, box, truck, etc. to empty on
                                       the barcode side (reset)! If there were still units present according to bar-
                                       coding, e.g. on the rack, they will be assigned to the Error Rack registration
                                       point (see Error Rack, page 50)!

                                       These remaining units according to barcoding can only occur because of
                                       forgotten scans, incorrect labels (incorrect readings), etc.!
2.01 / 07-2017




                 H-48                                                          A+W Production Barcode Manager
                 Tutorial                                                                          Booking Examples




                                      Scanning Units
                                      This module shows you how to scan units.
                                      The following instructions exist for this training module:
                                      •   How to scan a unit to an empty rack (rack will be emptied by barcoding)
                                      •   How to scan a unit to a rack that already contains units
                                      •   How to scan reject report units
                                      •   How to scan delivery units
                                      •   How to scan units to an empty registration point: Special case Truck
                                      •   How to scan units to a registration point that already contains units


                                       How to scan a unit to an empty rack (rack will be emptied by
                                        barcoding)
                                      1 Register an empty rack with the scanner
                                          <Begin> <Rack>




                                      2 Scan the label of the unit.




                                          < Unit 1>
                                          < Unit 2>
                                          < Unit 3>
                                          < Unit 4>
                                          …
2.01 / 07-2017




                 A+W Production Barcode Manager                                                               H-49
                 Booking Examples                                                                    Tutorial




                                     How to scan a unit to a rack that already contains units
                                       <Rack> <Unit 1> <Unit 2> <Unit …>


                                     How to scan reject report units
                                       <Breakage> <Unit 1> <Breakage> <Unit 2> <Breakage> <Unit …>


                                     How to scan delivery units
                                       <Shipped> <Unit 1> <Shipped> <Unit 2> <Shipped> <Unit …>


                                     How to scan units to an empty registration point: Special case Truck
                                       <Begin> <RegPoint> <Unit 1> <Unit 2> <Unit …>


                                     How to scan units to a registration point that already contains units
                                       <RegPoint> <Unit 1> <Unit 2> <Unit …>


                                    Additional information
                                     “Lites or Units” on page H-16
2.01 / 07-2017




                 H-50                                                      A+W Production Barcode Manager
                 Tutorial                                                                           Booking Examples




                                      Scanning in Dispatch
                                      Dispatch needs special attention with regard to barcoding. There are units,
                                      racks, boxes, etc. at this registration point, but also trucks which are registra-
                                      tion points as well, and form the last link in the production chain. Usually, Den-
                                      so online scanners are used here.


                                       General procedure:
                                      1 First scan the name tag (it can be scanned again any time)
                                         •   <Schmidt>




                                      2 Register the registration point with the scanner. Then scan Dispatch Area
                                        from the list.
                                         •   <Dispatch Area>




                                      3 Scan the rack that the units should be placed on.
                                         •   <Rack 1>
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                   H-51
                 Booking Examples                                                                         Tutorial




                                    4 Scan the label of the unit.




                                       •   <Unit 1>
                                       •   <Unit 2>
                                       •   <Unit 3>
                                       •   <Unit 4>

                                       Note
                                       Please stick to the scanning sequence if you want or have to load units and
                                       racks/boxes at random!


                                    Additional information
                                     “Scanner” on page H-42
                                     “Truck registration point” on page H-25
                                     Software Reference, “Registration Points” on page H-92
2.01 / 07-2017




                 H-52                                                          A+W Production Barcode Manager
                 Tutorial                                                                          Booking Examples




                                      Scanning Registration Points
                                      Each registration point has its own barcode. Registration point examples:
                                      •   Cutting,
                                      •   IG line 1,
                                      •   IG line 2,
                                      •   Furnace,
                                      •   Dispatch,
                                      •   Truck1,
                                      •   Truck2
                                      •   etc.
                                      This module shows you how to scan registration points.
                                      The following instructions exist for this training module:
                                      •   “How to scan units to an empty registration point (registration point will be
                                          emptied by barcoding): Special case Truck” on page H-54
                                      •   “How to scan units to a registration point:” on page H-54
                                      •   “How to scan units to different registration points:” on page H-54
                                      •   “How to scan racks to a registration point:” on page H-55
                                      •   “How to scan racks to different registration points:” on page H-55
                                      •   “How to scan a registration point ready:” on page H-55
                                      •   “How to scan the delivery Truck or Trailer:” on page H-55
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                  H-53
                 Booking Examples                                                                    Tutorial




                                     How to scan units to an empty registration point (registration point
                                      will be emptied by barcoding): Special case Truck
                                    1 Register a new registration point with the scanner
                                       <Begin> <RegPoint>




                                    2 Scan the label of the lite/unit.




                                       <Unit 1>
                                       <Unit 2>
                                       <Unit 3>
                                       <Unit 4>
                                        …


                                     How to scan units to a registration point:
                                    1 Register the registration point with the scanner
                                       <RegPoint>
                                    2 Scan the label of the lite/unit
                                       <Unit 1> <Unit 2> <Unit …>


                                     How to scan units to different registration points:
                                       <RegPoint 1> <Unit 1> <Unit 2>
                                       <RegPoint 3> <Unit 3> <Unit 4> <Unit 5>
                                       <RegPoint 1> <Unit 6>
                                       <RegPoint 2> <Unit 7> <Unit 8> <Unit 9>
                                        …
2.01 / 07-2017




                 H-54                                                        A+W Production Barcode Manager
                 Tutorial                                                                        Booking Examples




                                       How to scan racks to a registration point:
                                         <RegPoint> <Rack 1> <Rack 2> <Rack …>


                                       How to scan racks to different registration points:
                                         <RegPoint 1> <Rack 1> <Rack 2>
                                         <RegPoint 2> <Rack 3>
                                         <RegPoint 1> <Rack 4>
                                         <RegPoint 2> <Rack 5> <Rack 6>
                                         <RegPoint 3> <Rack 7>
                                          …


                                       How to scan a registration point ready:
                                         <Ready> <RegPoint>


                                       How to scan the delivery Truck or Trailer:
                                         <Shipped> <RegPoint>


                                      Additional information
                                       Software Reference, “Registration Points” on page H-92
2.01 / 07-2017




                 A+W Production Barcode Manager                                                             H-55
                 Booking Examples                                                                      Tutorial




                                    Truck Registration Point
                                    This module shows you how to scan the Truck registration point.
                                    The following instructions exist for this training module:
                                    •   “General procedure:” on page H-56
                                    •   “Loading an empty and a partly loaded truck” on page H-57


                                     General procedure:
                                    1 First scan the name tag (it can be scanned again any time)
                                        <Schmidt>




                                    2 Register the new truck with the scanner.
                                        <Begin> <Truck1 >




                                    3 or register a partly loaded truck with the scanner.
                                        <Truck2>
                                    4 Scan the label of the unit.




                                        <Unit 1>
                                        <Unit 2>
                                        <Unit 3>
2.01 / 07-2017




                                        <Unit 4>
                                        …


                 H-56                                                          A+W Production Barcode Manager
                 Tutorial                                                                          Booking Examples




                                      Exercises:
                                      In this section we will show you how to load two trucks.

                                      Exercise 1: Loading an empty and a partly loaded truck
                                      Truck 1 (empty) and truck 2 (partly loaded) shall be loaded. The loading se-
                                      quence is free, i. e. the trucks, racks and units can be loaded at random.


                                       Loading an empty and a partly loaded truck
                                      1 Register truck 1 (RP) at the scanner
                                         <Begin> <Truck1>
                                      2 Book units directly to truck 1
                                         <Unit 1> <Unit 2> <Unit 3>
                                      3 Book racks to truck 1
                                         <Rack 1> <Rack 2>
                                      4 Register truck 1 again. Thus, the previous rack will be logged out and the
                                        following units can be booked directly on the truck. If this step does not take
                                        place, the following units will be booked to the previous rack (rack 2 on
                                        truck 1).
                                         <Truck1>
                                      5 Book units directly to truck 1
                                         <Unit 4> <Unit 5>
                                      6 Book racks to truck 1
                                         <Rack 3> <Rack 4> <Rack 5> <Rack 6>
                                      7 Register truck 2 (RP) at the scanner. This de-registers truck 1 automatically
                                         <Truck2>
                                      8 Book racks to truck 2
                                         <Rack 9> <Rack 10> <Rack 11>
                                      9 Register truck 2 again. Thus, the previous rack will be logged out and the
                                        following units can be booked directly on the truck. If this step does not take
                                        place, the following units will be booked to the previous rack (rack 11 on
                                        truck 2).
                                         <Rack 2>
                                      10 Book units directly to truck 2
                                         <Unit 6> <Unit 7> <Unit 8> <Unit 9>
                                      11 Book racks to truck 2
                                         <Rack 12><Rack 13>
2.01 / 07-2017




                                      12 Register truck 1 (RP) at the scanner. This de-registers truck 2 automatical-
                                         ly.
                                         <Truck1>


                 A+W Production Barcode Manager                                                                  H-57
                 Booking Examples                                                                              Tutorial




                                    13 Book racks to truck 1
                                       <Rack 14> <Rack 15>
                                    14 Register truck 1 again. Thus, the previous rack will be logged out and the
                                       following units can be booked directly on the truck.
                                       <Truck1>
                                    15 Book units directly to truck 1
                                       <Unit 10> <Unit 11>
                                       Loading will be continued …
                                    16 Loading of truck 1 is completed. The trigger time for truck 1 starts.
                                       <Shipped > <Truck 1>
                                    17 Register truck 2 at the scanner. This de-registers truck 1 automatically.
                                       <Truck2>
                                    18 Book racks to truck 21
                                       <Rack 9> <Rack 10> <Rack 11>
                                    19 Loading of truck 2 is completed. The trigger time for truck 2 starts.
                                       <Shipped> <Truck 2>

                                       Note
                                       Please stick to the scanning sequence if you want or have to load units and
                                       racks/boxes at random!

                                       When loading a truck, racks, boxes, and units can be allocated to the truck
                                       registration point. Please make sure that the units which are directly loaded
                                       onto the truck (registration point) are not booked to a previously loaded
                                       rack/box. Always finish loading a truck with the status booking <Shipped>
                                       <Truck>.
2.01 / 07-2017




                 H-58                                                          A+W Production Barcode Manager
                 Tutorial                                                                          Booking Examples




                                      Scanning Racks and/or Boxes
                                      Prerequisite:
                                      The employee's name and the current registration point must be scanned.
                                      The following instructions exist for this training module:
                                      •   “How to scan a unit to an empty rack (rack will be emptied by barcoding)”
                                          on page H-59
                                      •   “How to scan a transport rack ready for shipment” on page H-60
                                      •   “How to scan the delivery Racks/Transport Racks” on page H-60
                                      •   “How to scan racks to the truck” on page H-60


                                       How to scan a unit to an empty rack (rack will be emptied by
                                        barcoding)




                                      1 Scan an empty rack
                                          <Begin> <Rack>




                                      2 Scan the label of the unit.




                                          <Unit 1>
                                          <Unit 2>
                                          <Unit 3>
                                          <Unit 4>
2.01 / 07-2017




                                          …




                 A+W Production Barcode Manager                                                               H-59
                 Booking Examples                                                                    Tutorial




                                     How to scan a transport rack ready for shipment
                                       <Ready> < Rack 1> <Ready> <Rack 2> <Ready> <Rack …>


                                     How to scan the delivery Racks/Transport Racks
                                       <Shipped> <Rack 1> <Shipped> <Rack 2> <Shipped> <Rack …>


                                     How to scan racks to the truck
                                       <RegPoint> <Rack 1> <Rack 2> <Rack …>


                                    Additional information
                                     Software Reference, “Racks” on page H-96
2.01 / 07-2017




                 H-60                                                        A+W Production Barcode Manager
                 Tutorial                                                                           Booking Examples




                                      Scanning the Status
                                      Scanning a status barcode results in various barcoding activities in the back-
                                      ground that are important for the entire production controlling. If a truck is as-
                                      signed the <Shipped> status for example, this status will be applied to the
                                      entire load (racks, boxes, units, etc.); the load will be booked to the (system-)
                                      internal registration point 11 (Shipped).
                                      The status barcode describes the status of an object, e.g. a unit (broken etc.),
                                      a rack (empty, complete, shipped/<Begin>, <Shipped>, <Broken>, <Ready>,
                                      etc.).
                                      The status must always be scanned before the object (rack, unit, etc.). If sev-
                                      eral objects are to be assigned the same status, the status must be scanned
                                      separately for every object (<Status> <Object> <Status> <Object>).
                                      The following instructions exist for this training module:
                                      •   “How to scan the status Reject Report Units” on page H-61
                                      •   “How to scan the status Delivery Units” on page H-61
                                      •   “How to scan the status Delivery Units” on page H-61
                                      •   “How to scan the status Delivery Several Racks” on page H-61
                                      •   “How to register an empty rack (racks will be emptied by barcoding)” on
                                          page H-62
                                      •   “How to register an empty registration point (registration point will be emp-
                                          tied by barcoding): Special case Truck” on page H-62


                                       How to scan the status Reject Report Units
                                          <Breakage> <Unit 1> <Breakage> <Unit 2> <Breakage> <Unit …>


                                       How to scan the status Delivery Units
                                          <Shipped> <Unit 1> <Shipped> <Unit 2> <Shipped> <Unit …>


                                       How to scan the status Delivery Several Racks
                                          <Shipped> <Rack 1> <Shipped> <Rack 2> <Shipped> <Rack …>


                                       How to scan the status Delivery Truck/Trailer (complete the loading)
                                        and Start the Trigger Time
                                          <Shipped> <RegPoint>
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                   H-61
                 Booking Examples                                                                               Tutorial




                                     How to register an empty rack (racks will be emptied by barcoding)
                                       <Begin> <Rack>


                                     How to register an empty registration point (registration point will be
                                      emptied by barcoding): Special case Truck
                                       <Begin> <RegPoint>

                                       If the <Status> is scanned several times
                                       If the status is scanned several times in a row
                                       <Status1><Status2><Status3><Object>, the last scanned status will be ap-
                                       plied to the object, in this example <Status3><Object>. The barcode en-
                                       gine checks the bookings and will reject those that are not plausible, e.g.
                                       two status bookings in succession.

                                       Caution for setting status to <Begin>:
                                       The status <Begin> resets the object (rack, truck, etc) with respect to the
                                       registration point, i.e. to empty! If there were still units present according to
                                       barcoding, (e.g. on the truck or rack, they will be automatically assigned to
                                       the Error Rack registration point.
                                       Always finish loading a truck with the status booking <Shipped> <Truck>.


                                    Additional information
                                     Software Reference, “Status Types” on page H-100



                                    Correcting Erroneous Entries
                                    It is possible to correct erroneous entries with a new, correct booking! The ad-
                                    ditional booking is saved in the booking history but has no further effects apart
                                    from this correction.

                                    Example:
                                    If units have been booked to a rack instead of the registration point by mistake,
                                    this error can be corrected by first scanning the registration point and then the
                                    unit (to be repeated for every incorrectly scanned unit).
                                    <RegPoint> <Unit 1> <Unit 2> <Unit …>
2.01 / 07-2017




                 H-62                                                            A+W Production Barcode Manager
                 Tutorial                                                                       Production Terminals




                                      Production Terminals
                                      This subject will provide you with a brief overview concerning the different pro-
                                      duction terminals.
                                      This includes the following training modules:
                                      •   “Introduction” on page H-65
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                  H-63
                 Production Terminals                                                                                   Tutorial




                                        Production Terminals
                                        Objectives

                                        • Getting familiar with different terminals
                                        • Getting to know and understanding their functionality


                                        Benefits

                                        The Production Terminals support you when it comes to loading the lites of a unit from
                                        the rack to production (e.g. the line) in the correct sequence. To work efficiently, you
                                        have to understand the functioning of the terminals; you must also be capable of
                                        handling daily recurring situations.


                                        Definitions

                                        Production Terminal IG       Is used at the IG line.

                                        Production Terminal TG       Is used at the TG line.

                                        Production Terminal LG       Is used at the LG line.

                                        Production Terminal Order Is used wherever large quantities are booked.

                                        Production Terminal Manual Visualizes the work schedule for the lites to be cut at the
                                        Cutting                    manual cutting table.

                                        Production Terminal          Is used at the processing machines.
                                        Processing

                                        Production Terminal Edit     Is used in the shipping office.


                                        Note

                                        Prerequisite                 Prerequisite for the use of the production terminals is an
                                                                     installed barcode manager (A+W Production).
2.01 / 07-2017




                 H-64                                                                  A+W Production Barcode Manager
                 Tutorial                                                                                  Production Terminals




                                         Introduction
                                         Production Terminals are control stations for different work stations. Among
                                         other things, they are used to show and schedule the processing of lites ac-
                                         cording to various criteria, to book work performed, to report reject, to create
                                         subsequent parts automatically, or to create production statistics. Production
                                         terminals are typically used for:
                                         •   Cutting
                                         •   IG line
                                         •   TG furnace
                                         •   LAMI line
                                         •   Dispatch
                                         Control stations visualize and control individual processing steps and can be
                                         configured individually. A+W control stations can be used to print labels and
                                         reports online, and enter reject including all necessary information. Operation
                                         of the control stations is easy and uniform. These intelligent systems enable
                                         you to inform your customers of the current state of products at any time.
                                         Please see below for a diagram of a possible A+W Production landscape:




                                                                           Terminal Processing
                                             Terminal Manual
                                                 Cutting




                                                               Terminal TG-Out                   Terminal TG-In


                                                                Terminal LG-Out                        Terminal LG-In




                                                                       Terminal Bender
                                              Terminal
                                               IG-Out                                            Terminal IG-In
                                                         Terminal IG-Assembly




                 Fig. H-8   Overview of production terminals
2.01 / 07-2017




                                         As every workstation in production requires different information, there are
                                         standard terminals configured for the various processes and work flows.



                 A+W Production Barcode Manager                                                                          H-65
                 Production Terminals                                                                             Tutorial




                                        A brief explanation of the individual production terminals:

                                        Terminal Manual Cutting Visualizes the work schedule for the lites to be cut
                                        at the manual cutting table.

                                        Terminal Order Is used wherever large quantities are booked.

                                        Terminal Processing Is the control station version used with the processing
                                        machines, automatically controlling the machines. This module provides de-
                                        tailed information on the processing steps to be performed including true-to-
                                        scale production drawings.

                                        Terminal IG-In Is installed at the IG line entrance and visualizes the work
                                        schedule for the lites to be produced for a batch or a logical production rack/
                                        harp rack, in production sequence.

                                        Terminal IG-Assembly Is installed between the visual check of lites after the
                                        washing machine, and in front of the spacer applicator, visualizing the techni-
                                        cal data including the spacer data for each unit to be produced.

                                        Terminal IG-Out Installed at the IG line exit and shows the technical and
                                        shipping-related data for each unit produced.

                                        Terminal TG-In Is the display system at the furnace entry. It shows the fur-
                                        nace bed load and is controlled by the operator. All lites are registered at the
                                        scanner; their geometry is checked for completeness of processing.

                                        Terminal TG-Out This is the display system at the furnace exit. All lites reg-
                                        istered at the furnace entry are displayed based on the clock rate. If defined,
                                        the user will get information as to the further use or on stacking in the shipping
                                        area.

                                        Terminal Edit Is the control station version that is normally used in the ship-
                                        ping office for rebooking units, lites, or groups and for managing off-site racks.

                                        Terminal LG-In Installed at the LAMI line entrance, it visualizes the work
                                        schedule for the lites of a batch or a logical production rack/harp rack to be pro-
                                        duced, in production sequence.

                                        Terminal LG-Assembly Installed in the clean room, it shows the work sched-
                                        ule as soon as a lite or unit has been booked at Terminal LG-In. This leaves
                                        ample time for cutting the necessary film layers.

                                           Production terminals
                                           Please see the Production Terminal manual for detailed information on the
                                           individual terminals.
2.01 / 07-2017




                 H-66                                                               A+W Production Barcode Manager
                 Tutorial                                                                  Reject Management




                                      Reject Management
                                      This subject shows you how to handle broken lites.
                                      This includes the following training modules:
                                      •   “Reject Handling (Internal)” on page H-69
2.01 / 07-2017




                 A+W Production Barcode Manager                                                        H-67
                 Reject Management                                                                                   Tutorial




                                     Overview
                                     Objectives

                                     • Getting familiar with how to handle rejects.


                                     Benefits

                                     Manual input is not required and as a result the rejects are remade faster. Additional
                                     communication between the employees is also not required and thus are avoided.


                                     Definitions

                                     Rejects Pool                 You will find an overview of the rejects in the Rejects
                                                                  Pool.


                                     Note

                                     Rejects report               The rejects report is executed at each Production
                                                                  Terminal or via scanner.

                                     Labels                       Labels are printed automatically at a central printer.

                                     Automatic remake.            The automatic remake is executed on the residue plate
                                                                  or by table optimization in the A+W Realtime Optimizer.
2.01 / 07-2017




                 H-68                                                                 A+W Production Barcode Manager
                 Tutorial                                                                          Reject Management




                                      Reject Handling (Internal)
                                      When units are reported broken, various internal actions are triggered. After a
                                      reject report, all information on the original unit plus all subsequent parts and
                                      remakes of subsequent parts will be saved in the database.
                                      Subsequent parts will always be provided with the original barcode number.
                                      The barcode number of the original lite is provided with an index in the case of
                                      a reject report.
                                      The table shows the changes resulting from the reject reports with regard to
                                      the individual flags and barcode numbers.

                                      Barcode           Registration Rack        Reject   Subsequent       Description
                                                        point                             parts index

                                      012345678         Drilling       15        0        0                E1

                                      012345678 001     Drilling       15        1        0                E2
                                      Reject 1

                                      012345678         -              -         0        1                E3

                                      012345678 002     Furnace        20        1        1                E4
                                      Reject 2

                                      012345678         -              -         0        2                E5

                                      Tab. H-1     Barcoding Reject Handling

                                      Description of table


                                      E1   The lite with barcode 012345678 is at the Drilling registration point, on
                                           rack 15. The lite has not been reported broken; the reject flag is zero.
                                           This is the original lite as the subsequent parts index is zero.

                                      E2   The lite with barcode 012345678 is reported broken at the Drilling regis-
                                           tration point. The reject flag is set. A three-digit index is added to the bar-
                                           code number. Index 001 shows that this is the first reject.

                                      E3   A subsequent part is created and is provided the original barcode num-
                                           ber 012345678. In addition, the subsequent part index is increased by
                                           one (1). The subsequent part index distinguishes the subsequent part
                                           from the original lite. As the unit has not been entered, it is not allocated
                                           to a registration point.

                                      E4   The subsequent part has made its way in the production area up to the
                                           furnace where it is reported broken. The reject flag is set. A three-digit
                                           index is added to the barcode number. Index 002 shows that this is the
                                           second reject.

                                      E5   The second subsequent part is created and is provided with the original
                                           barcode number 012345678. In addition, the subsequent part index is in-
2.01 / 07-2017




                                           creased by one (2). The subsequent part index distinguishes the subse-
                                           quent part from the original lite. As the unit has not been entered, it is not
                                           allocated to a registration point.


                 A+W Production Barcode Manager                                                                     H-69
                 Reject Management                                                                           Tutorial




                                     Note
                                     When you print labels for the subsequent parts or at reporting, the above-
                                     mentioned values and flags can be analyzed and taken into account. This
                                     is usually defined during the project planning phase and can be adapted to
                                     the current needs if required. Please ask A+W Software GmbH for avail-
                                     able options.

                                     Tip
                                     You can use filters for the A+W Production views. Standard filters have
                                     been set for the barcode manager views which may not show units with a
                                     subsequent part index. To display these units, disable all filters (unfiltered).
                                     The name of the standard filter is Active!

                                     Views and filters
                                     For more information on the views and filters, please refer to the A+W Pro-
                                     duction manual.
2.01 / 07-2017




                 H-70                                                         A+W Production Barcode Manager
                 Tutorial                                                        Statistics, Reporting and Monitoring




                                      Statistics, Reporting and
                                      Monitoring
                                      This subject will introduce you to the reports and different analyses.
                                      This includes the following training modules:
                                      •   “Barcode Reporting” on page H-73
                                      •   “Monitoring: A+W Dashboard” on page H-79
                                      •   “Statistics: A+W Discovery” on page H-82
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                H-71
                 Statistics, Reporting and Monitoring                                                                   Tutorial




                                          Overview
                                          Objectives

                                          • Getting familiar with standard barcode reports.


                                          Benefits

                                          • Using the standard reports, you will have an overview of the current status of your
                                            production at any time. This will save you time and effort and you are always able
                                            to provide your customers with accurate answers.


                                          Definition

                                          Reports                     Are flexible tools to control and analyze the production.


                                          Note

                                          Standard reports            Are part of A+W Production

                                          Individual reports          Can be created at customers' requests at any time.
2.01 / 07-2017




                 H-72                                                                   A+W Production Barcode Manager
                 Tutorial                                                           Statistics, Reporting and Monitoring




                                      Barcode Reporting
                                      The described reports are standard barcode reports. It is possible to custom-
                                      ize reports and create new reports. The reports are a flexible and powerful pro-
                                      duction control and analysis tool.
                                      Please contact A+W Software GmbH; we are glad to advise you and to per-
                                      form the necessary changes, extensions and amendments or create new, cus-
                                      tomized reports.

                                         Note
                                         General reports analyzing a registration point usually show all units allocat-
                                         ed to this registration point! If a partly loaded rack is registered at the IG line
                                         exit (registration point 1612) for instance to load IG units, the units already
                                         existing on this rack will also be booked to registration point 1612! To run
                                         analyses which show only the throughput of the IG line, for example, you
                                         will require amended reports.


                                      Loading the Reports
                                      Reports can be loaded via the A+W Production menu structure. The individual
                                      Production Terminals provide reports depending on their function. Shortcuts to
                                      reports can be saved on the PC desktop.

                                         Note
                                         The A+W Production menu structure is dynamic. Menu entries for the Bar-
                                         code Manager are visible only if a Barcode Managerview is open.


                                      Examples of Standard Barcode Reports
                                      Depending on the report, you can enter or select individual parameters for the
                                      report. This can be the display time, the registration point to be analyzed, etc.

                                         Note
                                         The sectional display of reports will give you an overview of the A+W Pro-
                                         duction reports.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                      H-73
                 Statistics, Reporting and Monitoring                                                            Tutorial




                                          Unit list
                                          Lists > Unit list
                                          The unit list shows all parts that are selected in a A+W Production view exact
                                          to units. Depending on the filter in the A+W Production view, spacer bars, etc.
                                          are also shown.




                                          Fig. H-9      Unit list


                                          Order overview
                                          Lists > Order List
                                          The order overview shows you where the individual items (head sections) of
                                          the order are located.
2.01 / 07-2017




                 H-74                                                               A+W Production Barcode Manager
                 Tutorial                                                       Statistics, Reporting and Monitoring




                                      Fig. H-10    Order overview


                                      Order status
                                      Lists > Order status
                                      The list provides you with information about the order status.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                               H-75
                 Statistics, Reporting and Monitoring                                                           Tutorial




                                          Fig. H-11     Order status


                                          Loading list
                                          Lists > Loading list
                                          The loading list shows you the actual load. You can restrict content by using
                                          filters.
2.01 / 07-2017




                 H-76                                                               A+W Production Barcode Manager
                 Tutorial                                                       Statistics, Reporting and Monitoring




                                      Fig. H-12    Loading list


                                      Rack load per lite
                                      Lists > Rack load per lite
                                      The list shows you the load per lite for the entered rack number.




                                      Fig. H-13    Rack load per lite
2.01 / 07-2017




                 A+W Production Barcode Manager                                                               H-77
                 Statistics, Reporting and Monitoring                                                         Tutorial




                                          Rack load per item
                                          Lists > Rack load per item
                                          The list shows you the load per item for the entered rack number.




                                          Fig. H-14     Rack load per item


                                          Booking history
                                          Lists > Booking history
                                          This list shows you per order, which bookings have taken place and where.




                                          Fig. H-15     Booking history
2.01 / 07-2017




                 H-78                                                              A+W Production Barcode Manager
                 Tutorial                                                          Statistics, Reporting and Monitoring




                                      Monitoring: A+W Dashboard
                                      Objectives

                                      • Brief introduction to A+W Dashboard
                                      • Getting to know the options


                                      Benefits

                                      A+W Dashboard shows the important key figures of the crucial production points to
                                      ensure a high level of transparency.


                                      Definitions

                                      Traffic light              The traffic light shows the current status of a registration
                                                                 point. You can define the meaning of the colors yourself.


                                      Note

                                      Period of time             Database tables with the A+W Production bookings are
                                                                 used for analyses. Usually a time period of max. 24
                                                                 hours is taken into account.

                                      Correct display            You need complete A+W Production bookings for
                                                                 meaningful displays.

                                      Display                    A+W Dashboard can be used both on large monitors in
                                                                 various production departments and mobile terminals
                                                                 such as smartphones.

                                      Malfunctions               In the event of malfunctions, you can communicate the
                                                                 exact situation and in many cases even suggest your
                                                                 own solutions.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                        H-79
                 Statistics, Reporting and Monitoring                                                                Tutorial




                                             Overview
                                             A+W Dashboard shows the important key figures of the crucial production
                                             points to ensure a high level of transparency.
                                             You get information on specific production areas in real time such as cutting to
                                             size, ISO lines, processing and TG production: e.g. you will see the actual de-
                                             gree of utilization, the status of each machine, and the production progress.
                                             This program can be used both on large monitors in various production depart-
                                             ments and mobile terminals such as smartphones, tablet computers or PDAs.
                                             However, this requires an internet browser and access to this program (ad-
                                             dress and user account).
                                             This means that the display can be used as an online monitoring tool and de-
                                             cision-making tool if machine states change in the course of a shift or sched-
                                             uled quantities cannot be met.
                                             In case of malfunctions, the employees can communicate the situation exactly
                                             and in many cases suggest their own solution approaches.
                                             A+W Production contains predefined displays, although it can also be adapted
                                             to individual machines or departments. This enables you to keep an eye on the
                                             critical points of your production and take action wherever necessary.
                                             Database tables with the barcoding bookings are used for analysis. Usually a
                                             time period of max. 24 hours is taken into account. This is how A+W Dash-
                                             board differs from A+W Discovery which allows statistical analyses over longer
                                             periods of time.
                                             The analyses are visualized in different ways. You can zoom in and out of the
                                             displays and change pages by swiping.




                          A                B                        C                     D                   E
                 A Traffic light                      C Plot diagram                     E Speedometer
                 B Pie chart                          D Bar chart
                 Fig. 9        Types of visualization (examples)


                                             You can set up each of these display types to correspond with the demands of
                                             your production departments and monitoring.
2.01 / 07-2017




                 H-80                                                                  A+W Production Barcode Manager
                 Tutorial                                                         Statistics, Reporting and Monitoring




                                      Traffic light (A)
                                      The traffic light shows the current status of a registration point. You can define
                                      the meaning of the colors yourself. This display makes sense for status dis-
                                      plays over very short periods such as showing whether a machine is operating
                                      or has broken down.

                                      Pie chart (B)
                                      The pie chart shows the shares of machine statuses reported over a self-de-
                                      fined period. By default, this represents the past 24 hours. With it, the total of
                                      all downtimes of all shifts during the time period can be viewed.
                                      Furthermore, the operation of machines similar to one another can be com-
                                      pared with this display.
                                      Beyond this, the display can hide individual colors to make the relationship of
                                      the other two colors clearer.

                                      Plot diagram (C)
                                      This line shows the bookings of a past period of time spread out over a display
                                      period such as the bookings of the last hour spread over the display period.
                                      One point shows the total per grouping (such as per minute, hour or day).
                                      You can also show the targeted number of pieces along with the average by
                                      means of continuous horizontal lines for making the surpluses or shortfalls of
                                      the actual number of pieces visible.
                                      This display can show longer periods of time, although only a maximum of 24
                                      hours. A rapid drop in the curve might mean with an IG line that the individual
                                      lites were very large so that fewer units could be produced.

                                      Bar chart (D)
                                      The bar chart shows statistical data collected via SQL queries. These statistics
                                      have to be available for view configuration.

                                      Speedometer (E)
                                      The speedometer shows the present capacity utilization. For this purpose, the
                                      number of booked pieces during the past hour is analyzed. The red-yellow-
                                      green marking indicates how the number of pieces are assessed.
                                      The display is suited for short periods with a relatively high throughput.

                                         Correct display only if barcoding bookings are correct
                                         You need complete barcoding bookings for meaningful displays.

                                      A+W Dashboard links the production software A+W Production and the
                                      A+W Production Terminal. The Barcoding data is read out through the PPS
                                      Web Service.

                                         A+W Dashboard
2.01 / 07-2017




                                         Please see the A+W Dashboard manual for detailed information on this
                                         module.



                 A+W Production Barcode Manager                                                                    H-81
                 Statistics, Reporting and Monitoring                                                                     Tutorial




                                          Statistics: A+W Discovery
                                          Objectives

                                          • Brief introduction to A+W Discovery
                                          • Getting to know the options


                                          Benefits

                                          A+W Discovery is used to collect, edit, and visualize your business data.
                                          Management and controlling staff can analyze this information and use it for their
                                          business decisions.


                                          Definitions

                                          Pivot table                 Is a special type of table with the option to display data in
                                                                      different ways.

                                          Fiscal year                 Business year for which a company compiles the results
                                                                      of its business in an annual financial statement.


                                          Note

                                          A+W Discovery               Allows you to create long-term analyses of production
                                                                      data.

                                          Analyses                    Analyses can easily be created in the form of pivot tables
                                                                      using Microsoft Excel.

                                          Data provision              A+W Discovery can provide data from the ERP systems
                                                                      (A+W Enterprise, A+W Business) and the PPS system
                                                                      (A+W Production).

                                          Client-wide analyses        You can create client-wide analyses.
2.01 / 07-2017




                 H-82                                                                   A+W Production Barcode Manager
                 Tutorial                                                         Statistics, Reporting and Monitoring




                                      Overview
                                      Constantly growing demands on modern ERP and PPS systems require more
                                      and more powerful controlling and control mechanisms. On the one hand, this
                                      is due to tax and legal conditions while on the other hand there is the necessity
                                      of being able to analyze the product portfolio, productivity, and capacity utiliza-
                                      tion from different points of view and realign them accordingly.
                                      A+W Discovery is the state-of-the-art Business Intelligence System of A+W
                                      Software GmbH tailored to the special needs of modern glass producers and
                                      processors. Its setup and the integration with the PPS system A+W Production
                                      allows evaluating and offsetting statistical parameters and indices from differ-
                                      ent points of view and deducing the necessary strategic, commercial, or pro-
                                      duction-related decisions and steps.
                                      You can, for instance, collect data revealing the gross margin and the sales
                                      volume of certain locations or subsidiaries for a defined time frame (e.g. month
                                      or year). This enables you to adjust your cost structures accordingly if neces-
                                      sary, and motivate your staff and sales partners to achieve an increase in turn-
                                      over in the following year. Version 5.4 additionally implements the fiscal year
                                      and fiscal quarter.
                                      You will also be able to analyze key production figures like the quantity of reject
                                      per work station or machine downtimes within a defined time frame.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                    H-83
                 Statistics, Reporting and Monitoring                                                              Tutorial




                 Fig. 10     A+W Discovery


                                          Apart from that, A+W Discovery comes with predefined A+W standard reports
                                          which allow comparing and aggregating meaningful PPS data. This will put
                                          you in full control of all commercial and production-relevant data, products, re-
                                          sources, costs, times, and capacities.

                                              A+W Discovery
                                              Please see the A+W Discovery manual for detailed information on this
                                              module.
2.01 / 07-2017




                 H-84                                                                A+W Production Barcode Manager
Barcoding                  H

            Software Reference




            A+W Production
                 Software Reference                                                                       Overview




                                      Overview
                                      The software reference provides information on the following subjects:
                                      •   Master Data

                                          Dialogs are accessible from different points
                                          Please note that there are various ways of opening functions and dialogs.
                                          The corresponding dialogs will only be described once in this document.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                H-87
                 Master Data                                                              Software Reference




                               Master Data
                               Open menu Master Data > Barcoding
                               The Barcoding menu offers the following items:
                               •   Barcode Options:
                                   This section is maintained by A+W Software GmbH.
                               •   Barcode Types:
                                   This section is maintained by A+W Software GmbH.
                               •   Registration Point Types:
                                   This section is maintained by A+W Software GmbH.
                               •   Registration Points:
                                   Use this section to manage your registration points.
                                    “Registration Points” on page H-92
                               •   Racks:
                                   Use this section to manage your racks.
                                    “Racks” on page H-96
                               •   Rack Filters:
                                   Use this section to manage rack filters.
                                    “Rack Filter” on page H-99
                               •   Status Types:
                                   This section is maintained by A+W Software GmbH.
                               •   Status Values:
                                   Use this section to manage status values.
                                    “Status Values” on page H-101
                               •   Employees
                                   Use this section to manage your employees.
                                    “Employees” on page H-103
                               •   Column Assignment:
                                   This section is maintained by A+W Software GmbH.
                               •   Columns:
                                   This section is maintained by A+W Software GmbH.
                               •   Barcoding Post-Processing:
                                   This section includes post-processing for the event that problems have oc-
                                   curred during data processing.
                                    “Post-Processing” on page H-107
2.01 / 07-2017




                 H-88                                                     A+W Production Barcode Manager
                 Software Reference                                                                  Master Data




                                      Barcode Options
                                      Master Data > Barcoding > Barcode Options




                                      Fig. H-1    Barcode Options


                                      This section addresses the barcode options.

                                         Data relevant to the system
                                         This entire section is created and changed as required by A+W Software
                                         GmbH. Please do not change anything. The data in this dialog is relevant
                                         to the system.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                             H-89
                 Master Data                                                          Software Reference




                               Barcode Types
                               Master Data > Barcoding > Barcode Types




                               Fig. H-2    Barcode Types


                               This section determines the behavior of barcodes.

                                  Data relevant to the system
                                  This entire section is created and changed as required by A+W Software
                                  GmbH. Please do not change anything. The data in this dialog is relevant
                                  to the system.
2.01 / 07-2017




                 H-90                                                  A+W Production Barcode Manager
                 Software Reference                                                                  Master Data




                                      Registration Point Types
                                      Master Data > Barcoding > Registration Point Types




                                      Fig. H-3     Registration Point Types


                                      This section determines the behavior of registration points.

                                         Data relevant to the system
                                         This entire section is created and changed as required by A+W Software
                                         GmbH. Please do not change anything. The data in this dialog is relevant
                                         to the system.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                             H-91
                 Master Data                                                              Software Reference




                               Registration Points
                               Master Data > Barcoding > Registration Points




                               Fig. H-4     Registration points


                               This dialog is used to define new registration points, or change existing regis-
                               tration points.
                               Technical info: database table: AWBAR_STELLEN

                               List of status values

                               ID Unique number assigned to the registration point.

                               Name Name assigned to the registration point.

                               Description Description that you have given the registration point.

                               Type Type that you have assigned to the registration point.

                                  Column headers can be configured as desired
                                  The headers of the individual columns can be configured as desired. It is
                                  therefore possible that the headers shown here do not correspond to the
                                  headers in your installation.

                               Description of fields

                               Registration Point No. Enter the registration point number in this field.
                               Technical info: database field: Esnr
2.01 / 07-2017




                 H-92                                                    A+W Production Barcode Manager
                 Software Reference                                                                       Master Data




                                      Barcode Enter the registration point barcode in this field.
                                      Technical info: database field: Esbc

                                      Name Enter the registration point name in this field.
                                      Technical info: database field: Esname

                                      Description Enter a detailed description for the registration point in this field.
                                      Technical info: database field: Allgbez

                                      Text for Production Lists Enter a text in this field that is to be displayed in
                                      the production lists.
                                      Technical info: database field: Lst1bez

                                      Text for Customer Lists Enter a text in this field that is to be displayed in the
                                      customer lists.
                                      Technical info: database field: Lst2bez

                                      Subrow for Barcode Labels Enter a text in this field that is to be displayed
                                      underneath the barcodes.
                                      Technical info: database field: Barcbez

                                      Reg. Point Type The combo box shows all registration point types defined in
                                      your company. Select the corresponding type. If the requested registration
                                      point type is not included, you can switch to the Registration Point Type dialog
                                      by using the button […] and create the requested type there.
                                      Technical info: database field: Typ

                                      Grouping In this field you can group the registration points for analyses re-
                                      gardless of registration point types, e.g. all furnaces of a group.
                                      Technical info: database field: Gruppe

                                      Grouping for Working Shifts Use this field to group registration points to
                                      create working shifts. This combo box includes all created groupings. Select
                                      one grouping; the shifts for each of these groups is then generated.
                                      Technical info: database field: Shift_Group
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                   H-93
                 Master Data                                                                  Software Reference




                               Current Status Use this field to assign a current status to a registration point.
                               The combo box includes all the statuses defined in your company. Select the
                               corresponding status. If the requested status is not included, you can switch
                               to the Status Values dialog by using the button […] and create the requested
                               status there.
                               Technical info: database table: Zustandnr

                               Restrictions This value enables or disables the restriction check and defines
                               the quantity to which the restriction check refers. You can choose from the fol-
                               lowing values:
                               • 0: Restriction check is switched off. Any quantity can be booked in quantity
                                  barcoding.
                               • 1: The restriction check refers to the technical production quantity.
                               • 2: The restriction check refers to the quantity available. All lites which have
                                  completed the previous process, are available.
                               • 3: The restriction check refers to the quantity available. All lites which have
                                  completed all previous processes, are available.
                               Technical info: database field: Restriction

                               Over Exceeding Enter the quantities exceeded as a percentage in this field.
                               This value is analyzed only if the restriction check is enabled. It defines the
                               percentage by which an initial quantity can be exceeded. The initial quantity is
                               determined by the selection that has been made in the Restriction field. In
                               practice, the initial quantity for cutting is always the technical output (i.e. re-
                               striction = 1). For all following stations, it is always the available quantity (i.e.
                               restriction = 2 or 3).
                               Technical info: database field: Overbook

                               Show Produced Parts This checkbox controls whether produced parts are
                               shown or not. Possible values:
                                Completely produced lites are not shown on the Production Terminal.
                                Completely produced lites are shown on the Production Terminal.
                               Technical info: database field: Show_produced_parts
2.01 / 07-2017




                 H-94                                                        A+W Production Barcode Manager
                 Software Reference                                                                         Master Data




                                      Machine of the Order Entry This field shows the machine of the order entry.
                                      This field is reported back to order entry. This means that if you change the
                                      entry, the changed machine is reported back.
                                      Technical info: database field: Maschinennr

                                      Description of the fields in section Feedback of Bookings

                                      Processing Feedback This checkbox controls whether there will be feed-
                                      back regarding the processing. Possible values:
                                       No feedback.
                                       If a lite is booked to a registration point, the processing progress is written
                                      precisely to the lite into file ST-SD*.ASC in the form of a notification of change.

                                      Rack Feedback This checkbox controls whether there will be feedback re-
                                      garding the rack load. Possible values:
                                       No feedback.
                                       If a rack is booked to a registration point, the rack occupation is written pre-
                                      cisely to the lite into file ST-SG*.ASC in form of a snapshot.

                                      Register Rack Load to Rack Server This checkbox controls whether the
                                      rack load should be reported to the rack server. Possible values:
                                       No feedback to the rack server.
                                       The rack load is reported to the rack server.

                                      Unit Feedback (STSU*.asc) Use this checkbox to assign the A+W Produc-
                                      tion labels to A+W Business order items in A+W Business. Possible values:
                                       No feedback.
                                       If a unit is booked to a registration point, the processing progress is written
                                      precisely to the lite into file ST-SU*.ASC in form of a notification of change.

                                      Production Feedback Use this checkbox to update the current order status
                                      in A+W Business. Possible values:
                                       No feedback.
                                       The current order status in A+W Business is updated.


                                      Additional information
                                       Tutorial, “Registration Points” on page H-19
                                       Tutorial, “Error rack” on page H-20
                                       Tutorial, “Truck registration point” on page H-25
                                       “Status Values” on page H-101
                                       “Registration Point Types” on page H-91
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                    H-95
                 Master Data                                                              Software Reference




                               Racks
                               Master Data > Barcoding > Racks




                               Fig. H-5     Racks


                               This dialog is used to define new racks, or change existing ones.
                               Technical info: database table: AWBAR_GESTELLE

                               List of racks

                               Name Name assigned to the rack.

                               Rack Barcode assigned to the rack.

                               Type Rack type assigned to the rack.

                                  Column headers can be configured as desired
                                  The headers of the individual columns can be configured as desired. It is
                                  therefore possible that the headers shown here do not correspond to the
                                  headers in your installation.

                               Description of fields

                               Define Multiple Racks Activate this checkbox if you want to create several
                               racks at once. After you have activated the checkbox, the fields Prefix, Start
                               Value, End Value and BC Start Value are displayed underneath it.
2.01 / 07-2017




                               Prefix Activate this checkbox if you want to create several racks at once. After
                               you have activated the checkbox, the fields Prefix, Start Value, End Value and
                               BC Start Value are displayed underneath it.



                 H-96                                                     A+W Production Barcode Manager
                 Software Reference                                                                        Master Data




                                      Start Value Activate this checkbox if you want to create several racks at
                                      once. After you have activated the checkbox, the fields Prefix, Start Value, End
                                      Value and BC Start Value are displayed underneath it.

                                      End Value Activate this checkbox if you want to create several racks at once.
                                      After you have activated the checkbox, the fields Prefix, Start Value, End Value
                                      and BC Start Value are displayed underneath it.

                                      BC Start Value Activate this checkbox if you want to create several racks at
                                      once. After you have activated the checkbox, the fields Prefix, Start Value, End
                                      Value and BC Start Value are displayed underneath it.

                                      Description of the fields in the Properties section

                                      Rack Base Type This combo box allows to select the corresponding rack
                                      type. The following types are available:
                                      • 00 Normal
                                      • 01 Tray rack
                                      • 02 Crate
                                      Technical info: database table: Typ_KZ

                                      Rack Type This combo box allows to select the corresponding rack type. The
                                      following types are available:
                                      • 0000 Not Selected
                                      • 0001 Furnace bed
                                      • 0002 A-Rack
                                      • 0003 Harp rack
                                      • 0004 AutoClav rack
                                      Technical info: database table: Typ_KZ

                                      Slot Number from … to This field is used for tray racks and shows the num-
                                      ber of the 1st tray in the first field. In the second field, the number of the last
                                      occupied tray on the rack is displayed. If a rack is reported as Start, the num-
                                      ber that is displayed as the first slot number is -1.
                                      Technical info: database field: Erstfachnr / Lbelfach
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                    H-97
                 Master Data                                                              Software Reference




                               Base Reg. Point This combo box allows you to select the corresponding
                               base registration point. The combo box shows all registration points defined in
                               your company.
                               Technical info: database field: Basisesnr

                               Temporary Rack Use this checkbox to control whether the rack is a tempo-
                               rary rack or not.
                                The rack can be used as a temporary rack.
                                The rack cannot be used as a temporary rack.
                               Depending on the configuration, temporary racks are automatically created by
                               the booking logic.
                               Technical info: database field: Tempkz

                               Description of the fields in the Batch Data section

                               Current RP This field shows the registration point where the rack is currently
                               located.
                               Technical info: database field: Esnr

                               Last RP This field shows the registration point where the rack was previously
                               located.
                               Technical info: database table: Esnralt

                               Current Status This field shows you the current status of the rack (e.g. deliv-
                               ered, empty, etc.).
                               Technical info: database table: Zustandnr

                               Last Status This field shows the previous status.
                               Technical info: database table: Zustandnralt

                               Description of the fields in the Customer Data section

                               Customer Number In this field, enter the number of the customer (if avail-
                               able) who has been assigned with the rack in the case of an "off site" notifica-
                               tion.
                               Technical info: database table: Kundennr

                               Customer Name Enter the name of the customer for "off site" racks.
                               Technical info: database table: Kundenname

                               Delivery Location Enter the delivery location for "off site" racks
                               Technical info: database field: Lieferort

                               Route Number Enter the route number for "off site" racks.
                               Technical info: database field: Tournr
2.01 / 07-2017




                               Additional information
                                Tutorial, “Racks” on page H-26




                 H-98                                                    A+W Production Barcode Manager
                 Software Reference                                                                       Master Data




                                      Rack Filter
                                      Master Data > Barcoding > Rack Filter




                                      Fig. H-6     Rack filter


                                      In this dialog you can create filters yourself to limit the number of displayed
                                      racks. This is useful if you have a large quantity of racks.

                                      Description of fields

                                      Registration Point Type The combo box shows all registration point types
                                      defined in your company. Select the required type by which you intend to filter.

                                      Registration Point The combo box shows all registration points defined in
                                      your company. Select the required registration point by which you intend to fil-
                                      ter.

                                      Rack Name from to Enter a range by which you intend to filter.

                                      Rack Base Type This combo box includes all created rack base types. Se-
                                      lect the required rack base type by which you intend to filter.

                                      Rack Type This combo box includes all created rack types. Select the re-
                                      quired type by which you intend to filter.

                                      Company-Owned Racks Enable the checkbox if you intend to filter by com-
                                      pany-owned racks only.


                                      Additional information
                                       Tutorial, “Managing Racks” on page H-29
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                  H-99
                 Master Data                                                          Software Reference




                               Status Types
                               Master Data > Barcoding > Status Types




                               Fig. H-7    Status types


                               This section determines the behavior of a status.

                                  Data relevant to the system
                                  This entire section is created and changed as required by A+W Software
                                  GmbH. Please do not change anything. The data in this dialog is relevant
                                  to the system.
2.01 / 07-2017




                 H-100                                                  A+W Production Barcode Manager
                 Software Reference                                                                      Master Data




                                      Status Values
                                      Master Data > Barcoding > Status Values




                                      Fig. H-8     Status values


                                      This dialog is used to define new status values, or change existing ones.
                                      Technical info: database table: AWBAR_ZUSTAND

                                      List of status values

                                      ID Unique number assigned to the status.

                                      Name Name assigned to the status.

                                      Description Description that you have given the status.

                                      Type Type that you have assigned to the status.

                                         Column headers can be configured as desired
                                         The headers of the individual columns can be configured as desired. It is
                                         therefore possible that the headers shown here do not correspond to the
                                         headers in your installation.

                                      Description of fields

                                      Status Number A unique number assigned to the status. The system will
                                      suggest the next available number. You can overwrite this number.
                                      Technical info: database table: Zustandnr

                                      Name Assign a name for the status in this field.
                                      Technical info: database table: Zustandname

                                      Description Save a detailed description for the status in this field.
2.01 / 07-2017




                                      Technical info: database table: Beschreibung




                 A+W Production Barcode Manager                                                               H-101
                 Master Data                                                                 Software Reference




                               Text for Lists Enter a text in this field that is to be displayed in the lists.
                               Technical info: database table: Listenname

                               Barcode Enter the barcode for the status in this field.
                               Technical info: database table: Zustandbc

                               Status Type This combo box includes all created status types. Select the cor-
                               responding type. If the requested status type is not included, you can switch
                               to the Status Types dialog by using the button […] and create the requested
                               type there.
                               Technical info: database field: Typ

                               AWRack Info Use this checkbox to control whether or not the rack server
                               should be notified in the event of a change of this status.
                                Notification to the rack server.
                                No notification to the rack server.
                               Technical info: database field: Notify

                               AWRack Status This combo box includes all AWRack statuses. Select the
                               corresponding status from this combo box.
                               Technical info: database field: Awrackstate


                               Additional information
                                “Status Types” on page H-100
                                Tutorial, “Status” on page H-36
2.01 / 07-2017




                 H-102                                                      A+W Production Barcode Manager
                 Software Reference                                                                   Master Data




                                      Employees
                                      Master Data > Barcoding > Employees




                                      Fig. H-9    Employees


                                      This dialog is used to enter new employees, or change existing employee da-
                                      ta.
                                      Technical info: database table: AWBAR_PERSON

                                      List of employees

                                      Number Unique ID assigned to the employee.

                                      Name Name assigned to the employee.

                                      Personnel No. The employee key. It is identical with the ID.

                                      Description Description that you have given the employee.

                                      Barcode Barcode assigned to the employee.

                                         Column headers can be configured as desired
                                         The headers of the individual columns can be configured as desired. It is
                                         therefore possible that the headers shown here do not correspond to the
                                         headers in your installation.

                                      Description of fields

                                      Number Enter a unique number for the employee in this field.
                                      Technical info: database field: PersonNr

                                      Name Enter the name of the employee in this field.
2.01 / 07-2017




                                      Technical info: database field: PersonName




                 A+W Production Barcode Manager                                                             H-103
                 Master Data                                                              Software Reference




                               Description In this field you can enter additional information relating to the
                               employee.
                               Technical info: database table: Beschreibung

                               Employee No. Enter the employee number in this field. This number will be
                               provided to you by the payroll office or accounting.
                               Technical info: database table: PersonKey

                               Barcode Enter the barcode for the employee in this field. It is compiled from
                               the number and the employee number. Example: There is a 9-digit barcode,
                               the employee's number is 60 and the personnel no. is 51 – the barcode is then
                               600000051.
                               Technical info: database field: Personbc


                               Additional information
                                Tutorial, “Staff” on page H-32
2.01 / 07-2017




                 H-104                                                   A+W Production Barcode Manager
                 Software Reference                                                                  Master Data




                                      Column Assignment
                                      Master Data > Barcoding > Column Assignment




                                      Fig. H-10   Column assignment


                                      This section addresses the assignment of columns.

                                         Data relevant to the system
                                         This entire section is created and changed as required by A+W Software
                                         GmbH. Please do not change anything. The data in this dialog is relevant
                                         to the system.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                           H-105
                 Master Data                                                          Software Reference




                               Columns
                               Master data > Barcoding > Columns




                               Fig. H-11   Columns


                               This section addresses the columns.

                                  Data relevant to the system
                                  This entire section is created and changed as required by A+W Software
                                  GmbH. Please do not change anything. The data in this dialog is relevant
                                  to the system.
2.01 / 07-2017




                 H-106                                                 A+W Production Barcode Manager
                 Software Reference                                                                      Master Data




                                      Post-Processing
                                      Master Data > Barcoding > Post-Processing




                                      Fig. H-12    Post-processing


                                      Any problems that may occur during the processing of the barcoding data can
                                      be found here. The errors must be corrected!

                                      Description of fields

                                      Initialization Only If you activate this radio button, only errors that have oc-
                                      curred during the barcoding initialization are shown.

                                      Bookings Only If you activate this radio button, only errors that have oc-
                                      curred during booking are shown.

                                      All Use this radio button to display all parts that are pending post-processing.
                                      If the displayed quantity is too large, you can use the Not Processed radio but-
                                      ton to display only parts that have not been processed.

                                      Not Processed Use this radio button to limit the displayed data. If enabled,
                                      only parts that have not yet been processed are displayed.

                                      Description of buttons

                                      Repeat Use this button to reevaluate the booking record.

                                      Set Processed Press this button to clear the display.

                                      Update Press this button to update the display.
2.01 / 07-2017




                 A+W Production Barcode Manager                                                                H-107
                 Master Data                Software Reference
2.01 / 07-2017




                 H-108         A+W Production Barcode Manager
Barcoding                H

                   Partindex




            A+W Production
                 Partindex                                                             Index Barcoding




                 Index Barcoding
                 B                                  – Base reg. point H-98
                 Barcoding bookings                 – BC start value H-97
                 – Continuous booking        H-81   – Create multiple racks H-96
                 Boxes H-28                         – Current reg. point
                                                      – H-98
                                                    – Current status H-98
                 C
                                                    – Customer name H-98
                 correct data    H-81
                                                    – Customer number H-98
                                                    – Delivery location H-98
                 D                                  – End value H-97
                 Data relevant to the system        – Filter H-27
                 – Barcode options H-89             – Last reg. point H-98
                 – Barcode types H-90               – Last status H-98
                 – Column assignment H-105          – Prefix H-96
                 – Columns H-106                    – Rack base type H-97
                 – Registration point types H-91    – Rack type H-97
                 – Status types H-100               – Route number H-98
                 Denso scanners H-43                – Slot number from ... to H-97
                 Direct objects H-16                – Start value H-97
                 Dispatch H-51                      – Temporary rack H-98
                                                    Registration Point
                 E                                  – Grouping H-93
                 Error rack H-20                    – Grouping for shifts H-93
                 Expert mode                        – Restrictions H-94
                 – Overview H-72                    Registration point
                                                    – Barcode H-93
                                                    – Current status H-94
                 I
                                                    – Description H-93
                 Indirect objects     H-16
                                                    – Machine for order entry H-95
                                                    – Name H-93
                 M                                  – Number H-92
                 Module                             – Processing feedback H-95
                 – function     H-9                 – Produced parts H-94
                                                    – Production feedback H-95
                 O                                  – Quantities exceeding H-94
                 Offline scanners H-44              – Rack feedback H-95
                 Online scanners H-43               – Registration point type H-93
                 Overview                           – Report rack load H-95
                 – Expert mode H-72                 – Subrow for labels H-93
                                                    – Text for customer lists H-93
                                                    – Text for production lists H-93
                 R
                                                    – Truck H-25
                 Rack filter
                                                    Registration points
                 – Company-owned racks H-99
                                                    – Manage H-23
                 – Rack base type H-99
                                                    Required knowledge H-9
                 – Rack name from ... to H-99
2.01 / 07-2017




                 – Rack type H-99
                 – Reg. point type H-99
                 – Registration point H-99
                 Racks H-27


                 A+W Production Barcode Manager                                                   H-3
                 Index Barcoding                                   Partindex




                 S
                 Scan
                 – Units H-49
                 Scan units H-49
                 Scanner
                 – Configuration H-44
                 Serial scanners H-44
                 Staff H-103
                 Standard report
                 – Booking history H-78
                 – Loading list H-76
                 – Order overview H-74
                 – Order status H-75
                 – Rack load per item H-78
                 – Rack load per lite H-77
                 – Unit list H-74
                 Status
                 – Action barcode H-38
                 – Rack H-37
                 – Registration point H-37
                 – Unit/group H-37
                 Status barcode
                 – Scan H-61
                 Status values
                 – AWRack info H-102
                 – AWRack status H-102
                 – Barcode H-102
                 – Description H-101
                 – Status name H-101
                 – Status number H-101
                 – Text for lists H-102
2.01 / 07-2017




                 H-4                         A+W Production Barcode Manager

