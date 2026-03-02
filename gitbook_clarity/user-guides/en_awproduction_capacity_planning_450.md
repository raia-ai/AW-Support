---
description: "EN AWProduction Capacity Planning 4.50"
---



# EN AWProduction Capacity Planning 4.50

Capacity Planning          E




                            English




                A+W Production
                                                                                                                 Introduction




                                        Introduction
                                        In this part of the documentation you can find editorial notices.


                                        Revision Overview
                                        Section                    Edition
                                        Version / Date

                                        4.50 / 01-2023             Export work plan added.

                                        4.00 / 11-2017             Revision

                                        3.01 / 01-2017             Product and company names adjusted.

                                        3.00 / 08-2013             Initial creation of Tutorial and complete revision of
                                                                   Software Reference.

                                        2.00 / 04-2008             Revision

                                        1.20 / 11-2007             Change of name (AWCapacity/Capacity Planning)

                                        1.10 / 2007                Change of chapter Work Plan

                                        1.00 / 2007                Original version



                                        Editorial
                                        The editorial contains the following themes:
                                        •   Notes on this Document
                                        •   Copyrights
                                        •   Trademarks
                                        •   Contact

                                        Notes on this Document
                                        This document is intended for end users of A+W Production.
                                        The documentation and software described are licenses that must be used or
                                        copied only in accordance with the conditions of our license agreement. The
                                        contents of the documentation are only informative and are subject to changes
                                        without prior notice. The text and illustrations were compiled with the utmost
                                        care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be
                                        held liable for errors or inaccuracies, unless they can be attributed to wilful or
                                        grossly negligent action.
                                        This document describes the full scope of the master data.

                                        Copyrights
4.50 / 01-2023




                                        © 2023,A+W Software GmbH, all rights reserved, including the right of reprint,
                                        the production of copies and of the translation.



                 A+W Production Capacity Planning                                                                          E-3
                 Introduction




                                The documentation must be copied, completely or in part, saved in an archiv-
                                ing system, or transferred in any other form only in accordance with our license
                                agreement. Transmission of the documentation is not allowed, neither elec-
                                tronically, nor mechanically, nor by recording or in any other way, without A+W
                                Software GmbH's prior written approval.

                                Trademarks
                                Any designation of hardware and software being mentioned in the documen-
                                tation can also be registered trademarks or other commercial rights of third
                                parties being protected by law. Rights of third parties being protected by law
                                are to be observed insofar.

                                Contact
                                A+W Software GmbH
                                Am Pfahlgraben 4 - 10
                                D-35415 Pohlheim
                                Germany
                                   +49 6404 2051 0
                                   +6404 2051 877
                                Zentrale@a-w.com
                                http://www.a-w.com
4.50 / 01-2023




                 E-4                                                      A+W Production Capacity Planning
                                                                                                                                                        Contents




                                        Contents
                                        Introduction ............................................................................................................. E-3
                                          Revision Overview ............................................................................................... E-3
                                          Editorial ............................................................................................................... E-3
                                        Contents ................................................................................................................. E-5

                                        Tutorial                                                                                                             E-9
                                        Overview ............................................................................................................... E-11
                                          Documentation .................................................................................................. E-12
                                            Tutorial Structure ........................................................................................... E-12
                                            Display Conventions ...................................................................................... E-13
                                        Basic Principles .................................................................................................... E-14
                                          Date Optimization .............................................................................................. E-15
                                          Scheduling ......................................................................................................... E-16
                                        Planning and Scheduling ...................................................................................... E-20
                                          Production Monitor ............................................................................................ E-21
                                            Daily Adjustments of the Work Shifts ............................................................. E-23
                                            Setting up Production Monitor ........................................................................ E-30
                                          Export work plan ................................................................................................ E-33
                                          Scheduling and Rescheduling ........................................................................... E-34
                                            Scheduling of Orders ..................................................................................... E-35
                                            Rescheduling ................................................................................................. E-36
                                            Rescheduling Processings ............................................................................. E-38
                                            Incorrect Scheduling ...................................................................................... E-40
                                            Post-Processing of Scheduled Orders ........................................................... E-41
                                          Campaign Planning ........................................................................................... E-43
                                            Definition of the Campaigns ........................................................................... E-44
                                            Campaigns in Scheduling .............................................................................. E-46
                                            Definition and Management of Campaigns .................................................... E-46
                                            Exercises on Campaigns ............................................................................... E-52
                                          Reservations ..................................................................................................... E-53
                                            Reservation of Capacities .............................................................................. E-54
                                            Definition and Management of Reservations ................................................. E-55
                                            Exercises on Reservations ............................................................................ E-61
                                          Creating Processings ........................................................................................ E-62
                                            Creation of Processings for Scheduling ......................................................... E-63
                                            Creation of Processings ................................................................................. E-64
                                        Master Data of Capacity Planning ........................................................................ E-67
                                          Shifts ................................................................................................................. E-68
                                            Shift Plans ...................................................................................................... E-69
                                            Definition of non-working Days ...................................................................... E-71
                                            Create a Shift Plan ......................................................................................... E-74
                                            Defining a Shift Rule ...................................................................................... E-77
                                            Creating a Shift Group ................................................................................... E-82
                                            Exercises ....................................................................................................... E-86
                                          Cost Calculation ................................................................................................ E-87
                                            Definition of the Cost Calculation ................................................................... E-88
                                            Definition and Management of Costs ............................................................. E-89
                                            Exercises ....................................................................................................... E-91
                                          Transition Times ................................................................................................ E-92
                                            Transition Times in Shifts or Hours ................................................................ E-94
4.50 / 01-2023




                                            Definition of Transition Times ........................................................................ E-98
                                            Definition and Management of Transition Times ......................................... E-101
                                            Exercises ..................................................................................................... E-104
                                          Default Times ................................................................................................. E-105


                 A+W Production Capacity Planning                                                                                                               E-5
                 Contents




                                 Definition of the Default Times ..................................................................... E-106
                                 Structure of Default Time Formulas ............................................................. E-107
                                 Calculation of Time Surcharges ................................................................... E-110
                                 Editor for Formula Elements ........................................................................ E-112
                                 Example – Default Time for the Logical Machine Cutting ............................ E-113
                                 Time Formula Objects .................................................................................. E-116
                                 Definition and Management of Default Time Formulas ................................ E-117
                                 Testing Time Formulas ................................................................................ E-124
                                 Exercises ..................................................................................................... E-130
                               Machinery Groups ........................................................................................... E-131
                                 Definition of the Machinery Groups .............................................................. E-132
                                 Definition and Management of Machinery Groups ....................................... E-133
                                 Exercises ..................................................................................................... E-136
                               Load Distribution ............................................................................................. E-137
                                 Definition of Load Distribution ..................................................................... E-138
                                 Definition and Editing of Load Distribution ................................................... E-139
                                 Exercises ..................................................................................................... E-142

                            Software Reference                                                                                            E-143
                            Overview ............................................................................................................. E-145
                            Scheduling .......................................................................................................... E-146
                              Production Monitor .......................................................................................... E-147
                              Displayed Machines ........................................................................................ E-151
                              Settings ........................................................................................................... E-152
                              Please Select an Order/Batch ......................................................................... E-155
                                Filter – Orders .............................................................................................. E-155
                                Filter – Batches ............................................................................................ E-156
                                Filter – Individual Filters ............................................................................... E-157
                              Create New Filter ............................................................................................ E-158
                              Machine (Name) .............................................................................................. E-159
                              Adjust Shifts for Machine ................................................................................. E-160
                              Shift Properties ................................................................................................ E-161
                              Reservation Display ........................................................................................ E-162
                              Workplan from Production Monitor .................................................................. E-163
                                Work Plan - Details ...................................................................................... E-164
                                Work Plan - Overview .................................................................................. E-165
                              Scheduling ....................................................................................................... E-166
                              BOM Configuration .......................................................................................... E-167
                              Action .............................................................................................................. E-168
                              Rescheduling ................................................................................................... E-169
                              Machine Reallocation ...................................................................................... E-173
                              Post-Processing Booking ................................................................................ E-174
                              Defective Orders ............................................................................................. E-177
                              Asynchronous Processing ............................................................................... E-178
                              Changes to Scheduled Orders ........................................................................ E-179
                              Split Items ........................................................................................................ E-180
                            Campaigns and Reservations ............................................................................. E-182
                              Campaigns ...................................................................................................... E-183
                                Campaigns – Individual Dates ..................................................................... E-183
                                Campaigns – Weekly Dates ......................................................................... E-185
                              Expired Reservations ...................................................................................... E-186
                              Reservations ................................................................................................... E-187
                              Reservation for Machine ................................................................................. E-189
4.50 / 01-2023




                              Select a Customer ........................................................................................... E-190
                              Select Project .................................................................................................. E-191
                            Processings ........................................................................................................ E-192
                              Creation of Processings .................................................................................. E-193


                 E-6                                                                          A+W Production Capacity Planning
                                                                                                                                                       Contents




                                          Add an Existing Condition ............................................................................... E-195
                                        Time Master Data ............................................................................................... E-196
                                          Default Times ................................................................................................. E-197
                                          Default Time Formula ...................................................................................... E-199
                                          Add elements .................................................................................................. E-203
                                          Tabelle, Vector (Name) ................................................................................... E-204
                                          Input Help for Vectors ...................................................................................... E-205
                                          Select Formula ................................................................................................ E-207
                                          Entering a Formula Element ............................................................................ E-208
                                          User-defined Table Elements .......................................................................... E-210
                                          Select Limit ...................................................................................................... E-211
                                          Time Formula Test .......................................................................................... E-212
                                          Formula Object Properties .............................................................................. E-214
                                          Formula (Name) .............................................................................................. E-215
                                          Course of Formula Evaluation ......................................................................... E-216
                                          Transition Times .............................................................................................. E-217
                                        Master Data for the Shifts ................................................................................... E-220
                                          Shifts ............................................................................................................... E-221
                                          Shift Calendar .................................................................................................. E-223
                                          Shift Plan ......................................................................................................... E-224
                                          Shift Rule ......................................................................................................... E-226
                                          Shift Group ...................................................................................................... E-228
                                          Machine ........................................................................................................... E-229
                                        Machines and Costs ........................................................................................... E-231
                                          Cost Calculation .............................................................................................. E-232
                                          Machinery Groups ........................................................................................... E-234
                                          Load Distribution ............................................................................................. E-235

                                        Section Index                                                                                                 E-237
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                                                              E-7
                 Contents
4.50 / 01-2023




                 E-8        A+W Production Capacity Planning
Capacity Planning           E

                        Tutorial




                A+W Production
                 Tutorial                                                                                     Overview




                                        Overview
                                        The tutorial on the Capacity planning module deals with the planning of your
                                        production process and the optimum use of your machine capacity. The main
                                        goals of capacity planning are the adherence to delivery dates, using the ma-
                                        chinery to the best effect, and being able to react flexibly to unforeseeable
                                        events. Optimal capacity planning is always a balancing act between the
                                        greatest possible efficiency and greatest possible flexibility.
                                        This tutorial describes how you can intervene manually in the planning and
                                        how the master data for capacity planning is set up.
                                        This tutorial includes the following subjects:
                                        •   “Basic Principles” on page E-14
                                        •   “Planning and Scheduling” on page E-20
                                        •   “Master Data of Capacity Planning” on page E-67

                                        Prerequisite knowledge
                                        This tutorial is meant for persons in charge of production scheduling in A+W
                                        Production who are responsible for organizing the optimum production pro-
                                        cess. Participants must be familiar with the master data concept in A+W Pro-
                                        duction. Knowledge of rough and detailed scheduling are also useful.

                                            Protecting master data against access
                                            The master data of A+W Production and especially of A+W Capacity Plan-
                                            ning are highly sensitive data. Uncontrolled or unintentional interventions
                                            and changes can bring production to a complete standstill. Therefore, set
                                            up the workstations so that only the administrators or employees with ap-
                                            propriate functions have access to the master data.

                                            Data back-up
                                            Create a full back-up of the master data before beginning any processing
                                            of the master data. The backup tool is located under: C:\Programs
                                            (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe.
                                            Shift the saved back-up out of your user directory into a directory to which
                                            support also has access. Discuss the upcoming changes in advance with
                                            your planner at A+W Software GmbH.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-11
                 Overview                                                                                Tutorial




                            Documentation
                            The following documents are available for the Capacity planning module:

                            Format                    Scope

                            PDF                       Complete documentation
                                                      • Tutorial
                                                      • Software reference
                                                      • Index

                            Online help <F1>          Dialog help


                            Tutorial Structure
                            This tutorial consists of subjects with several training modules each. Each unit
                            consists of the following elements:

                            Overview                  Each training unit starts with an overview of the major
                                                      topics:Each training unit starts with an overview of the
                                                      major topics:
                                                      • Objectives: What shall be conveyed?
                                                      • Benefit: What can this knowledge be used for?
                                                      • Maxims: Which correlations are to be remembered?

                            Concepts                  Concepts and terms of the corresponding training
                                                      session will be explained first. This is followed by
                                                      examples and operating instructions.

                            Exercises                 There are exercises featuring special tasks for some of
                                                      the training units.
4.50 / 01-2023




                 E-12                                                  A+W Production Capacity Planning
                 Tutorial                                                                                          Overview




                                        Display Conventions
                                        Certain parts of the sentences are specially marked. The meanings are:

                                        Italics                   mark character strings describing the software
                                                                  elements, e.g. the dialog Campaign planning.

                                        Bold                      marks character strings to be entered via keyboard, e.g.
                                                                  Enter 0.

                                        >                         The so-called 'breadcrumb trail' shows how to open a
                                                                  dialog, e.g. Master data > Capacity planning >
                                                                  Campaign planning > Add campaign.

                                        []                        Square brackets mark the buttons in the dialog, e.g.
                                                                  [OK] to save the data.

                                        <>                        Pointed brackets refer to keys or shortcuts on the
                                                                  keyboard, e. g. <F1> is used to open the online help.


                                        Reading instructions
                                        The contents of a training unit are based on the knowledge conveyed in the
                                        previous unit. We therefore recommend not to skip any unit.
                                        If you are already familiar with a subject you should at least read the summary
                                        at the beginning of the unit in order to bring the main details to mind.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                     E-13
                 Basic Principles                                                                                  Tutorial




                                    Basic Principles
                                    A+W Capacity Planning is designed so that even for products with unusually
                                    deep BOMs, usually several secure paths from the start technology to dis-
                                    patch are found. The capacity planning accesses the work processes that the
                                    lites run through from cutting to delivery.

                                    Master data for machine allocation
                                    The machine allocation (MA) establishes the connection between work pro-
                                    cesses and machines and maps the assessment according to preferred ma-
                                    chines. So that the machines valid for the lites to be produced are found, the
                                    machines must be described precisely. In the machine allocation, there is a
                                    distinction between physical restrictions and logical machines with additional
                                    restrictions, cost rates and transition times.
                                    Since the steps for setting up the capacity planning rely on the logical ma-
                                    chines, the machine park must be described completely. The information for
                                    this is in the Machine Allocation section.

                                    Master data for capacity planning
                                    For the date determination, shift plans, transition times, and times for the pro-
                                    cessing duration are required.
                                    •   So that a simple picture for the utilization arises for testing the data, it is rec-
                                        ommended that you specify the processing durations across the board in
                                        seconds per piece, e.g. 1 - 5 minutes per lite depending on the machine.
                                    •   For the transition times, the optimal and realistic production throughput
                                        should be described. The specification of the times in whole shifts ensures
                                        a simple, predictable date determination. On machines that can also work
                                        unattended, the transition time (storage time) in hours can be specified,
                                        e.g. heat soak, autoclave, or hardening of silicon seals. In the exercises,
                                        ensure that you have the needed space in the operation in order to store
                                        the glass quantity of a shift.
                                    •   The scheduling bottlenecks can be determined from the times for the pro-
                                        cessing duration.

                                    Scheduling rules
                                    The scheduling rules are specified as configuration parameters for A+W Ca-
                                    pacity Planning. They influence the program behavior, the message culture,
                                    and the possible user reactions. This affects, for example:
                                    •   May delivery dates be shifted.
                                    •   When is the earliest production start for a scheduled order.
                                    •   How are quotations scheduled and do they have to be canceled again.
                                    •   How are rush orders put through.
                                    •   Starting with what quantity do items need to be split.
4.50 / 01-2023




                 E-14                                                              A+W Production Capacity Planning
                 Tutorial                                                                                        Basic Principles




                                             Date Optimization
                                             The date optimization begins with the last machine on or before the delivery
                                             date: the loading. With a view to the Production Monitor, the date optimization
                                             can be depicted as follows.


                                                  Wednesday             Thursday            Friday               Monday

                  Float cutting

                  Sorting for TG

                  Coating machine

                  Sorting for IG

                                                                                      1
                  Spacer bender 1
                                                                                                     0
                  IG line 2
                                                                                                     0
                  IG sealing
                                                                                                             2
                                                                                                                          0
                  Packing
                                                                                                         2
                  Vehicle fleet



                                         F                              E                                D   C    B       A
                 A Vehicle fleet – loading             C Calculation path 2                E Conflict
                 B Calculation with optimal transition D Transition time in shifts         F Production beginning cutting
                   time
                 Fig. E-1      Scheduling paths with and without conflicts


                                             Starting from the drive date, after deducting the customer handling time (in
                                             working days), the production end is specified. From the end of the last possi-
                                             ble work shift (A), the scheduling searches backwards for the latest possible
                                             production beginning.
                                             The transition times from one processing to the next are counted in shifts (D),
                                             whereby 0 is the immediately following processing in the same shift. Locked
                                             shifts, which are marked with an X, are counted too.
                                             The calculation always checks all possible cost-effective paths. In case of date
                                             conflicts, transition times are kept and there is a buffer at the end of production.
                                             If in the process storage times that are too long result, the buffer times must
4.50 / 01-2023




                                             be distributed manually. The solutions arising this way are much more expen-
                                             sive, however.




                 A+W Production Capacity Planning                                                                             E-15
                 Basic Principles                                                                                         Tutorial




                                                  The Production Monitor is described in detail in a separate unit.
                                                   “Production Monitor” on page E-21



                                                  Scheduling
                                                  This section summarizes the technical background information for the sched-
                                                  uling.
                                                  Scheduling and interactive rescheduling uses the A+W Capacity Planning
                                                  functions for allocating valid processing dates and machines to the bills of ma-
                                                  terial.
                                                  Scheduling runs through five phases:
                                                  •   Analysis of the BOM.
                                                  •   Definition of machine paths.
                                                  •   Definition of feasible production dates.
                                                  •   Evaluation of feasible production dates.
                                                  •   Selection of the most favorable solution.

                                                  BOM analysis
                                                  The BOM is broken down into element chains; those are the BOM sections
                                                  whose first processing has no preceding processing or that unites several
                                                  BOM parts. The individual element chains are calculated independently and in
                                                  parallel. The individual results are matched to the final BOM at the conclusion
                                                  of the calculation.




                                             IG                                                    IG           LAMI

                                                                                 Element
                                           Spacer                                                         PVB           Spacer
                             TG                           LAMI


                                                          PVB
                                            HSG                         HSG                       Temp.     HSG        HSG


                            Float



                                            Float                       Float                     Float     Float      Float


                 Fig. E-2           Formation of element chains from the BOM
4.50 / 01-2023




                                                  While the BOM for the scheduling is being constructed, it is checked for plau-
                                                  sibility at the same time. Here, errors in the BOM are detected and reported:




                 E-16                                                                       A+W Production Capacity Planning
                 Tutorial                                                                                            Basic Principles




                                                 •   Abandoned BOM elements and processing steps will be detected and
                                                     skipped. A warning is written in the logfiles.
                                                 •   Processing sequences are checked and adjusted. Defining processings re-
                                                     ceive the sequence 100; processings with smaller sequence are arranged
                                                     according to the defining processing.
                                                 •   Any missing defining processings will be detected and reported.
                                                 •   Any missing logical machines will be detected and reported.
                                                 •   Inconsistencies between the processing data and machine allocation mas-
                                                     ter data will be detected

                                                 Definition of machine paths
                                                 For the calculation of the machine paths, there are two features available in
                                                 A+W Capacity Planning: best technology and automatic machine reschedul-
                                                 ing.
                                                 If only best technology is used, there is precisely one machinery path. Alterna-
                                                 tive machines are not used.




                 A
                        Cutting       Grinding       Polishing   Shape       Drilling   Drilling       Cut-out   Tempering      Silk
                                                                 corners                                                     screening
                 B



                                        C              C           D           E          E                                     F
                 A Processing                               C No machine change                    E No machine change
                 B Defined machines                         D Informative processing               F Screen printing + subsequent
                                                                                                     screen printing
                 Fig. E-3         Machinery path with best technology


                                                 By forming processing chains on a machine, subsequent processings can be
                                                 summarized insofar as the machine alternatives are the same. Subsequent
                                                 processings (C, E) without machine change are done on the same date. To
                                                 prevent this, e.g. with two screen printings one after another (F), a transition
                                                 time must be defined so that the first printing can dry before the second is ap-
                                                 plied. Informative processings (D) are assigned to the preceding processing.

                                                     Processing chains and automatic rescheduling
                                                     The settings for processing chains and automatic rescheduling are speci-
                                                     fied in the machine properties. The machines are described in the Machine
                                                     Allocation (MA) part.

                                                 For automatic machine rescheduling, all machine alternatives are determined
                                                 and connected to one another for each processing in the element chain. The
4.50 / 01-2023




                                                 number of machine paths can thus get so large that no solution is possible.
                                                 Therefore, the number of alternative machines must be limited.




                 A+W Production Capacity Planning                                                                               E-17
                 Basic Principles                                                                                          Tutorial




                        Cutting     Grinding       Polishing   Shape       Drilling   Drilling       Cut-out   Tempering      Silk
                                                               corners                                                     screening

                 A


                 B


                 C


                 A Preferred machines                     B Alternative machines                 C Manual production
                 Fig. E-4     Automatic machine rescheduling


                                               In this example, you see that the alternative machines are limited: all machines
                                               where manual work is done are not included in the determination of the ma-
                                               chine paths.
                                               For each processing in an element chain, the quantity of valid alternative ma-
                                               chines is loaded and transition times are assigned.
                                               •   For each processing, the machine specified by rescheduling determined by
                                                   the MA or by earlier rescheduling applies.
                                               •   Subsequent processings without machine change are done on the same
                                                   date.
                                               •   Machines that form processing chains can combine successive process-
                                                   ings provided that their processing alternatives are identical.
                                               •   Machines that are not assigned to any registration point process only infor-
                                                   mative processings, e.g. Shape corners. These processings are assigned
                                                   to the preceding processing and planned with it. The first processing of an
                                                   element chain may therefore not be an informative processing.
                                               All machines found are associated with their preceding machines insofar as
                                               the transitions are permitted. Thus the set of all machine paths with start points
                                               and end points will be created for an element chain. All processing steps of the
                                               element chain must not be included more than once in every path of the set.

                                                   Keep the number of alternative machines small
                                                   For each processing in the element chain, all machine alternatives are de-
                                                   termined and connected to one another. The number of machine paths can
                                                   thus get so large that no solution is possible. Therefore, limit the number of
                                                   machine alternatives. Also form processing chains. This increases perfor-
                                                   mance significantly.

                                               Definition of feasible production dates
4.50 / 01-2023




                                               Using the machine paths, the shift plans, and the transitions between the par-
                                               ticipating logical machines, the possible production dates for the individual
                                               processings steps are determined. For this, their (virtual) costs are calculated



                 E-18                                                                       A+W Production Capacity Planning
                 Tutorial                                                                                 Basic Principles




                                        and the scheduling rights determined, which are required for the use of the
                                        transitions.
                                        Random transitions are permitted below the last processing step in the BOM,
                                        below each joining processing steps, and below campaigns, rescheduling tar-
                                        gets, and date locks.
                                        This makes sure that valid production dates are available even if the schedul-
                                        ing variance has been extremely restricted.
                                        The result is a set of all scheduled machine paths from which the following
                                        evaluation can determine the most favorable paths.

                                        Evaluation of feasible production dates
                                        The set of all production dates found will be checked and evaluated. This re-
                                        sults in solution sets for start and end dates of the machine paths and their (vir-
                                        tual) costs. This supports
                                        •   A production flow that is as fast as possible
                                        •   Priority use of the transition type Normal.
                                        •   Scheduling for the preferred machine.
                                        •   Buffer times at the end of production.
                                        •   Use of the transition type Rush at the start of production.
                                        If the production needs to be brought forward because of date conflicts, over-
                                        load, locked shifts or for other reasons, this is done by moving the entire pro-
                                        cessing chain forward.
                                        The result of this step is for every element chain a set of the most favorable
                                        solutions for every completion date of the next step

                                        Finding the optimal solution
                                        The individual solutions for the element chains are linked with the transition
                                        costs to the next steps to achieve the optimal result for the entire BOM.
                                        For every start date of a laminated sheet or IG unit, the most favorable solu-
                                        tions for all sub-elements are combined and passed on to the next step for ev-
                                        ery completion date.

                                        Reporting to the ERP system
                                        The calculated time and personnel costs and material consumption are report-
                                        ed in the order and the storage management of the ERP system. In connection
                                        with the ERP integration, the following data is transmitted:
                                        •   Scheduling state.
                                        •   Machine and personnel cost determination.
                                        •   Calculation of earliest possible delivery date.
                                        •   Query of the driving dates for route planning.
                                        •   Query of the receipt of goods dates.
                                        •   Fileless completion reporting via webservices.
4.50 / 01-2023




                                        •   Online progress display from ERP via webservices.




                 A+W Production Capacity Planning                                                                    E-19
                 Planning and Scheduling                                                                           Tutorial




                                           Planning and Scheduling
                                           In this section, you will find information about how the scheduled orders are
                                           displayed and edited in the Production Monitor. In addition, you can correct in-
                                           correct schedulings and reserve production times.
                                           This section provides information on the following subjects:
                                           •   “Production Monitor” on page E-21
                                           •   “Scheduling and Rescheduling” on page E-34
                                           •   “Campaign Planning” on page E-43
                                           •   “Reservations” on page E-53
                                           •   “Creating Processings” on page E-62
4.50 / 01-2023




                 E-20                                                                A+W Production Capacity Planning
                 Tutorial                                                                            Planning and Scheduling




                                            Production Monitor
                                            The Production Monitor is the central capacity and order control desk and en-
                                            try point for work preparation, e.g. batch formation, rescheduling.
                                            On the Production Monitor dialog, you check and edit production planning.
                                            Here, the capacity utilization of the machines is displayed per work shift.




                     A                  B      C           D    E           F    G                    H
                 A   Displayed machines                               E   Bottleneck
                 B   Work shift per date                              F   Disabled
                 C   Scheduling                                       G   Reserved for rush orders
                 D   Work shift shortened                             H   Undefined processings
                 Fig. E-5      Production Monitor


                                            In this example, you see that for most machines, there are 2 work shifts avail-
                                            able. For some machines, 3 work shifts are displayed and can be booked.
                                            These work shifts are set up and generated via the master data for the capac-
                                            ity planning.
                                             “Master Data of Capacity Planning” on page E-67
4.50 / 01-2023




                                            The orders are scheduled from the point of view of date optimization. Here, the
                                            rules of A+W Capacity Planning, the times of the work shifts, the locking of
                                            shifts, the defined bottlenecks, and the (virtual) costs are considered.



                 A+W Production Capacity Planning                                                                      E-21
                 Planning and Scheduling                                                                             Tutorial




                                           The details of how the scheduling is calculated is described in a separate unit.
                                            “Date Optimization” on page E-15
                                           Generally, the orders from the ERP system are scheduled automatically. The
                                           work processes (processings) are scheduled accordingly on the machines'
                                           work shifts so that the delivery date promised in the order is adhered to. In spe-
                                           cial situations, you must intervene in this planning:
                                           •   Shift orders to other machines or dates.
                                                “Rescheduling” on page E-36
                                                “Rescheduling Processings” on page E-38
                                           •   Eliminate missing information from the orders.
                                                “Incorrect Scheduling” on page E-40
                                                “Post-Processing of Scheduled Orders” on page E-41
                                                “Creation of Processings” on page E-64
                                           •   Lock, reserve or set up additional work shifts.
                                                “Campaign Planning” on page E-43
                                                “Reservations” on page E-53
                                           •   Eliminate missing information from the orders.
                                                “Creating Processings” on page E-62
                                           •   Adjust utilization on a daily basis
                                                “Daily Adjustments of the Work Shifts” on page E-23
                                           •   Furthermore, you can set up the colored display of the work shifts as you
                                               wish.
                                                “Setting up Production Monitor” on page E-30
4.50 / 01-2023




                 E-22                                                                  A+W Production Capacity Planning
                 Tutorial                                                                       Planning and Scheduling




                                          Detail view




                 Fig. E-6   Production Monitor - detailed view


                                          In the detailed view, you can check the scheduling for individual days. In order
                                          to edit the schedulings, you must change back tot he main view.


                                          Daily Adjustments of the Work Shifts
                                          The work shifts in the Production Monitor are generated from the capacity
                                          planning master data. They apply for the assigned machines on particular
                                          days of the week and in a defined period of time. Changes to the master data
                                          therefore apply regardless of the current planning.
                                          You can control the planning day by day by adding individual work shifts for a
                                          machine, for example; by disabling machines to exclude them from the sched-
                                          uling; equalizing the planning by defining machines or work shifts as bottle-
                                          necks.
                                          In order to adjust individual work shifts to current needs for ongoing orders,
                                          you have the following possibilities:
                                          •   “Here's how to create an additional work shift” on page E-24
                                          •   “Here's how to lock a work shift completely” on page E-25
                                          •   “Here's how to reserve a work shift” on page E-26
                                          •   “Here's how to edit the working hours for a work shift” on page E-26
4.50 / 01-2023




                                          •   “Here's how to define a work shift as bottleneck” on page E-27
                                          •   “Here's how to set up the work shifts for a machine” on page E-28
                                          •   “Here's how to define a machine as bottleneck machine” on page E-29


                 A+W Production Capacity Planning                                                                   E-23
                 Planning and Scheduling                                                                          Tutorial




                                            Here's how to create an additional work shift

                                              No automatic rescheduling
                                              If you set up an additional shift in the Production Monitor, already sched-
                                              uled orders are not rescheduled automatically.

                                           1 Select A+W Production > Production Monitor.
                                           2 Open the context menu for the machine and the day on which you need an
                                             additional work shift.




                                           3 Select the Enter new shift menu.




                                              A                                        B



                                              A Date of the work shift              B Time of the work shift


                                           4 Select the start and end time (B).
                                           5 Select the date (A) of the start and end times.
                                              The end date of a night shift must be on the following day.
                                           6 Save the setting with [OK].




                                              The new work shift is displayed in the Production Monitor.
4.50 / 01-2023




                 E-24                                                                A+W Production Capacity Planning
                 Tutorial                                                                      Planning and Scheduling




                                         Here's how to lock a work shift completely
                                        1 Select A+W Production > Production Monitor.

                                               A


                                               B


                                           A Marked work shift                     B Context menu
                                           Fig. E-7      Work shift - Properties


                                        2 Mark the work shift (A) that you want to lock.
                                        3 Select Shift properties from the context menu (B).




                                           A                                               B




                                           A Status of the work shift              B Selection of the status


                                        4 Set the status to Disabled.
                                        5 Save the setting with [OK].




                                           The locked shift is marked in the Production Monitor with an X.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-25
                 Planning and Scheduling                                                                              Tutorial




                                            Here's how to reserve a work shift
                                           1 Open the Shift Properties dialog as shown in the previous action sequence.
                                           2 Set the status to Active for rush orders.
                                           3 Save the setting with [OK].




                                              The reserved work shift is marked in the Production Monitor with a !.


                                            Here's how to edit the working hours for a work shift
                                           1 Open the Shift Properties dialog as shown in the previous action sequence.




                                              A                                             B




                                              A Capacity of the work shift          B Specification of the duration


                                           2 Enter the duration of the time in hours and minutes.
                                           3 Save the setting with [OK].




                                              Shortening of the work shift is indicated with cross-hatching in the Produc-
                                              tion Monitor.
4.50 / 01-2023




                 E-26                                                                A+W Production Capacity Planning
                 Tutorial                                                                      Planning and Scheduling




                                         Here's how to define a work shift as bottleneck
                                        1 Open the Shift Properties dialog as shown in the previous action sequence.




                                           A                                              B




                                           A Bottleneck                           B Changing the setting


                                        2 Change the setting for the Bottleneck entry (A) to Yes (B).
                                        3 Save the setting with [OK].
                                           The setting applies only for the current work shift. It prevents the work shift
                                           from being booked beyond its capacity.

                                           Setting several work shifts to bottleneck
                                           You can mark several work shifts by pressing <Ctrl> and marking the shift.
                                           When you're holding the <Ctrl> key down, you can also drag a rectangle
                                           across all shifts that should be marked. Then you can mark all highlighted
                                           shifts together as Bottleneck.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                   E-27
                 Planning and Scheduling                                                                        Tutorial




                                            Here's how to set up the work shifts for a machine
                                           1 In the Production Monitor, open the context menu for the desired machine
                                             and select Shift properties.




                                              A
                                              B



                                                                                                    C




                                              A Shift number                         C Days of the week
                                              B Duration of the work shift
                                              Fig. E-8     Days of the week for the machine shift


                                           2 Mark the days of the week (C) on which the machine is available in the work
                                             shift.
                                           3 Enter the number (A) of the shift to which the changes refer.
                                           4 Enter the duration (B) in which the machine is available on the marked days
                                             of the week.
                                           5 Save the setting with [OK].
                                           6 If necessary, update the Production Monitor so that the changes to the ma-
                                             chine shifts are displayed.
4.50 / 01-2023




                 E-28                                                                 A+W Production Capacity Planning
                 Tutorial                                                                     Planning and Scheduling




                                         Here's how to define a machine as bottleneck machine
                                        1 In the Production Monitor, open the context menu for the desired machine
                                          and select Properties.




                                           A                                             B




                                           A Bottleneck                           B Change setting


                                        2 Change the setting for the Bottleneck entry (A) to Yes (B).
                                           The setting only applies for the current machine and only until it is reset
                                           again manually. This way, the machine cannot be booked beyond its ca-
                                           pacity.

                                           Defining bottleneck machines at the very start of the process
                                           To equalize production, bottleneck machines must be defined as far toward
                                           the beginning of the production process as possible. This setting should be
                                           specified at the beginning of the start-up of the Production Monitor via the
                                           setting of the machines displayed.

                                            “Here's how to display the machines in the Production Monitor” on page E-30
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-29
                 Planning and Scheduling                                                                               Tutorial




                                           Setting up Production Monitor
                                           In order to adjust the display to your planning needs, you have the following
                                           possibilities:
                                           •   “Here's how to display the machines in the Production Monitor” on
                                               page E-30
                                           •   “Here's how to set the display of the colors” on page E-31
                                           •   “Here's how to set the display type for all machines” on page E-32
                                           •   “Here's how to set the display type for one machine” on page E-32


                                            Here's how to display the machines in the Production Monitor
                                           1 Select A+W Production > Production Monitor.
                                           2 Click [Selected machines].




                                               A




                                               B




                                               A Displayed Machines                     B Machines are not displayed
                                               Fig. E-9     Selection of the machines


                                               On this dialog, all machines from the MA are listed. The red font marks ma-
                                               chines that are defined as bottleneck machines. These machines cannot
                                               be booked beyond their capacity.
                                           3 Check whether the settings as bottleneck machines are correct.
                                               Via the context menu for a machine, you can change the setting.
4.50 / 01-2023




                                           4 Mark the machines that should be displayed in the Production Monitor.




                 E-30                                                                   A+W Production Capacity Planning
                 Tutorial                                                                      Planning and Scheduling




                                        5 Save the setting with [OK].
                                           The dialog closes.
                                        6 If necessary, update the Production Monitor so that the changes to the ma-
                                          chines are displayed.


                                         Here's how to set the display of the colors
                                        1 Click [Settings].




                                                                                                 A

                                                                                                 B
                                                                                                 C




                                                                                                 D




                                           A Days before start date               C Specification of the color values
                                           B Selection of the color                 (RGB)
                                                                                  D Selection from combo box
                                           Fig. E-10    Settings for the Production Monitor


                                        2 Specify the settings with which the work shifts and scheduling should be
                                          displayed in the Production Monitor, e.g.:
                                           •   Number of days (A) that are displayed before the start date.
                                           •   Color (B, C) in which the times are displayed, e.g. assigned times, res-
                                               ervations.
                                           •   Specification (D) whether particular information is displayed, e.g. the
                                               time, planned work processes.
4.50 / 01-2023




                                        3 Save the settings with [OK].
                                           The dialog closes.



                 A+W Production Capacity Planning                                                                   E-31
                 Planning and Scheduling                                                                          Tutorial




                                           4 If necessary, update the Production Monitor so that the changes to the ma-
                                             chines are displayed.


                                            Here's how to set the display type for all machines
                                           1 Click [Change display type for all machines].




                                           2 Select with which values the scheduling in the Production Monitor should
                                             be displayed.
                                           3 Save the setting with [OK].
                                              The dialog closes.
                                           4 If necessary, update the Production Monitor so that the changes to the ma-
                                             chines are displayed.


                                            Here's how to set the display type for one machine
                                           1 In the Production Monitor, open the context menu for the desired machine.




                                                                                         B

                                              A




                                              A Logical machine                   B Display type of the machine


                                           2 Specify whether the assigned logical machines (A) should also be dis-
                                             played for the machine.
                                           3 Select with which values (B) the scheduling of the machine in the Produc-
                                             tion Monitor should be displayed.
4.50 / 01-2023




                                           4 Save the setting with [OK].
                                              The dialog closes.



                 E-32                                                              A+W Production Capacity Planning
                 Tutorial                                                                   Planning and Scheduling




                                        5 If necessary, update the Production Monitor so that the changes to the ma-
                                          chines are displayed.


                                        Export work plan




                                        Abb. E-11    Export work plan


                                        If you have opened the work plan in the production monitor via the context me-
                                        nu, you can export the data to a CSV file. Select the desired entries and open
                                        the Display menu. There you select Export. The dialog Save as ... opens. En-
                                        ter an appropriate name and click on [Save].
4.50 / 01-2023




                 A+W Production Capacity Planning                                                               E-33
                 Planning and Scheduling                                                                                Tutorial




                                           Scheduling and Rescheduling
                                           Objectives

                                           • What is scheduling and how are orders scheduled?
                                           • How can you react to problems which occur during scheduling?
                                           • What is rescheduling and how is it done?


                                           Benefit

                                           • During scheduling, order and quotation data transferred by the ERP system are
                                             processed and calculated. Based on these data, dates are calculated and
                                             restrictions relevant for production are checked to make sure that your order is
                                             produced efficiently.
                                           • Rescheduling can be used to allocate processing steps to other dates and
                                             machines.


                                           Note

                                           Scheduling                  Scheduling means the processing and calculation of
                                                                       data after an order or a quotation has been transferred
                                                                       by the ERP system. The orders or quotations are
                                                                       generally scheduled automatically.
                                                                       You can re-work a failed scheduling.

                                           Bottleneck machine          A bottleneck machine cannot be booked beyond its
                                                                       capacity.

                                           Scheduling                  Scheduling start with the selection of processings.The
                                                                       target dates are binding. They are treated like
                                                                       processings with a single campaign date. Delivery dates
                                                                       are protected - exception: The processing Shipping can
                                                                       be shifted.

                                           Processing sequences        Processing sequences in ascending order define the
                                                                       sequence of processing steps.

                                           Rescheduling mode           Possibilities for rescheduling:
                                                                       •   Complete BOM.
                                                                       •   Only predecessor processing.
                                                                       •   Only successor processing
                                                                       •   Individual processing.
                                                                       Rescheduling mode and direction are independent.
                                                                       Processings that do not participate are excepted from
                                                                       the scheduling.

                                           Rescheduling of orders      • Date rescheduling
                                                                         Orders are shifted to other dates.
                                                                       • Machine rescheduling:
                                                                         Orders are produced on other machines than
                                                                         originally planned.
4.50 / 01-2023




                 E-34                                                                    A+W Production Capacity Planning
                 Tutorial                                                                      Planning and Scheduling




                                        Scheduling of Orders
                                        Generally, automatic scheduling of orders is set up in A+W Production. The
                                        data import runs as background process. You can trace the process of sched-
                                        uling in the A+W ServiceMonitor. Manual interventions are only required if in-
                                        dividual orders or order items could not be scheduled. The processing of these
                                        orders is described in a separate unit.
                                         “Incorrect Scheduling” on page E-40
                                        You can check and edit the scheduled orders that cannot be processed further
                                        on the Orders dialog. This topic is discussed in the Rough Scheduling section.
                                        If manual scheduling has been configured in A+W Production you will have to
                                        use the Scheduling dialog. When scheduling has been successful, field Status
                                        will show the actual time.




                                        Fig. E-12    Scheduling


                                        The scheduling is calculated in A+W Production until a solution is found that
                                        corresponds to the scheduling rules. If no acceptable solution was found, you
                                        must control the scheduling manually. For this, for example, large items can
                                        be split. The position split is described in detail in the Rough Planning section.

                                           Settings for the data transfer
                                           Please check the settings for the data transfer from the ERP system to
                                           A+W Production with the A+W Software GmbH customer service team.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                   E-35
                 Planning and Scheduling                                                                          Tutorial




                                           Rescheduling
                                           You can reschedule orders if they cannot be put through production as origi-
                                           nally planned. Here, you can either select another machine or shift the pro-
                                           cessing to another date.
                                           •   Scheduling begins with the selection of processings.
                                           •   With the various rescheduling modes, you have the following possibilities
                                               for rescheduling:
                                               Complete BOM, only predecessor, only successor, individual processing.
                                           •   The target dates are binding: The target dates are assigned and locked.
                                               They are handled like processings with a single campaign date.
                                           •   Delivery dates are protected:
                                               This does not apply for the processing Shipping.
                                           •   Rescheduling mode and direction are independent.
                                               Processings that do not participate are excepted from the scheduling. If
                                               due to the rescheduling an invalid processing sequence would arise, all
                                               successors are rescheduled if this achieves a valid result.
                                               An invalid rescheduling would be, for example, the rescheduling Only pre-
                                               decessors in the direction later than the successors.

                                           Machine reallocation
                                           With a machine reallocation, the production of an order is shifted to other ma-
                                           chines. This can be necessary, for example, if a machine is not available due
                                           to repairs.




                                           A
                                                                                           B




                                           A Currently scheduled machines         B Available machines
                                           Fig. E-13    Machine reallocation
4.50 / 01-2023




                 E-36                                                                A+W Production Capacity Planning
                 Tutorial                                                                            Planning and Scheduling




                                            Processing rescheduling
                                            For the rescheduling of a production date, a processing is shifted to another
                                            date so that the order is completed earlier or later. This can be necessary, for
                                            example, if the priority of an order changes.




                 A


                                                                                                                           D




                 B




                                                                     C
                 A Processings                                           C Rescheduling mode
                 B Date and machine selection                            D Specifications for the scheduling
                 Fig. E-14   Rescheduling


                                            You can reschedule a processing (A) for another date (B) or another machine.
                                            For this, you can specify how the transition times (D) should be considered.
                                            The dates recalculated by a rescheduling can then be locked. Thus, they are
                                            protected against further rescheduling.
                                            The following modes are available for rescheduling (C):
                                            •   Reschedule complete BOM: The complete parts list to which the process-
                                                ing belongs is rescheduled.
                                            •   Only marked processing:
                                                Only the marked processing is rescheduled.
                                            •   Selected processing and all following processings:
                                                The selected processing and all following processing steps for the lite will
4.50 / 01-2023




                                                be rescheduled.
                                            •   Marked and all previous processings: The marked and all previous pro-
                                                cessings of the lite are rescheduled.


                 A+W Production Capacity Planning                                                                      E-37
                 Planning and Scheduling                                                                                Tutorial




                                            •       Unconditional allocation of dates for selected processing: Scheduling of the
                                                    selected processing will be forced on the selected date irrespective of the
                                                    machine capacities.
                                            With all these options, shipping and delivery date will be kept unless they are
                                            explicitly rescheduled. If you permit the shifting of the delivery date (D, you
                                            should also send the new delivery date back to the ERP system.


                                            Rescheduling Processings
                                            This unit will teach you how you can shift the processings to another date.


                                             Here's how to reschedule a processing
                                            1 Go to Display > Orders > Context menu for selected orders > Processings
                                              > Context menu for selected processings > Work schedule > Reschedul-
                                              ing.


                                                                                                 E




                 A




                 B




                                                C           D
                 A Processings                                             C Reservation
                 B Available machines for the selected processing          D Mode
                                                                           E Time pattern
                 Fig. E-15    Reschedule date


                                            2 Choose the processings (A) to be rescheduled.
4.50 / 01-2023




                                                    If you select several processings, you can only shift the date.
                                            3 Select the setting for the scheduling (E):


                 E-38                                                                       A+W Production Capacity Planning
                 Tutorial                                                                     Planning and Scheduling




                                           •   Force rescheduling:
                                               With this setting, the capacity limits of bottleneck machines are not con-
                                               sidered. Therefore, it is possible to overbook the work shifts.
                                           •   Allow Express Grid:
                                               For rescheduling, the transition times of the type Rush are used.
                                           •   Reschedule as High-Priority Order:
                                               The processing is rescheduled with the minimum transition times.
                                               Caution: Here, the times for campaigns can also be used. Use this set-
                                               ting only in emergencies.
                                        4 Mark the shift in which the processing should be rescheduled.




                                        5 Choose the rescheduling mode (D).
                                           The button to start the rescheduling is enabled.
                                        6 Click [Reschedule] to start the rescheduling.
                                           The times are recalculated. The result is displayed on a dialog. If the re-
                                           scheduling was not successful, you must change the conditions and try re-
                                           scheduling again.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-39
                 Planning and Scheduling                                                                            Tutorial




                                           Incorrect Scheduling
                                           The scheduling of orders can fail for various reasons, e.g. in the following cas-
                                           es:
                                           •   Undefined articles in orders.
                                           •   Undefined production articles in orders.
                                           •   Undefined processing steps in orders.
                                           •   Invalid order data.
                                           •   Shift restrictions cannot be met.
                                           •   Shifts do not exist, e.g. because the shift plans have expired.
                                           You can rework these orders and then repeat the scheduling.




                 A




                 B




                 A Defective Orders                                   B Selection criteria for the display
                 Fig. E-16   Incorrect scheduling


                                           To filter the orders, you can select one of the possible error causes (B). The
                                           display of the corresponding orders (A) is updated automatically. You can se-
                                           lect per order how the orders are handled. For this, you have the following op-
                                           tions:
                                           •   Take over data again
                                               The order data is scheduled again and unchanged. For this, you must cor-
                                               rect the master data, e.g. extend shift plans, and then schedule without re-
                                               newed transfer of the data from the ERP system.
                                           •   Force scheduling:
                                               The scheduling is forced. Here, the capacity of bottleneck machines is not
                                               considered. Therefore, the work shifts can be overbooked.
                                           •   Ignore scheduling:
4.50 / 01-2023




                                               The production dates are determined without consideration of transfer
                                               times, capacity limits, and campaign dates. All other orders and their deliv-
                                               ery dates are pushed back.



                 E-40                                                                  A+W Production Capacity Planning
                 Tutorial                                                                           Planning and Scheduling




                                             •   Delete invalid orders:
                                                 The corresponding orders are deleted. Speak to your colleagues in order
                                                 entry so that the orders will be corrected and re-entered into A+W Produc-
                                                 tion.
                                             •   Confirm determined delivery date:
                                                 The delivery date proposed by A+W Production is accepted. The new de-
                                                 livery date is reported back to the ERP system.


                                             Post-Processing of Scheduled Orders
                                             This unit will teach you how you can manually re-work the orders that could
                                             not be scheduled.


                                              Here's how to re-work a scheduling
                                             1 Go to Master data > Post-processing of scheduling.




                 A




                                                                                                             C



                 B




                 A List of orders                                         C Display by
                 B Selection criteria
                 Fig. E-17     Post-processing of invalid scheduling


                                             2 Select the filter criterion (B) for the display of the orders and sorting (C).
                                                 The list of orders is filtered.
                                             3 Select the order (A) to be edited.
                                             4 Click [Edit].
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                        E-41
                 Planning and Scheduling                                                                            Tutorial




                                              Depending on the filter criterion, you have the following possibilities:
                                              •   If you must change articles, the dialog for the corresponding master
                                                  data opens. Eliminate the error and then reschedule the order.
                                              •   For the other errors, one of the following dialogs opens:




                                           Fig. E-18    Defective Orders and Changes to Scheduled Orders


                                           5 Select the option with which you can eliminate the error.
                                              There is a description of the options in the Software Reference.
                                               Software Reference, “Defective Orders” on page E-177
                                               Software Reference, “Asynchronous Processing” on page E-178
                                               Software Reference, “Changes to Scheduled Orders” on page E-179
                                           6 Click [OK] to adopt the changes.
                                              The order is treated according to the options selected.
4.50 / 01-2023




                 E-42                                                                 A+W Production Capacity Planning
                 Tutorial                                                                           Planning and Scheduling




                                        Campaign Planning
                                        Objectives

                                        •   What is a campaign?
                                        •   How are campaigns defined, edited, and deleted?
                                        •   What are Individual dates?
                                        •   What are Weekly dates?


                                        Benefit

                                        • Campaigns are processes that are executed only on certain days, in certain shifts,
                                          and on certain machines, e.g. blue screen printing every Friday in shift 2.


                                        Note

                                        Campaigns                     Campaigns will help you process specific orders for
                                                                      customers or projects and plan them in due time.
                                                                      Campaigns are fixed, repeating dates for particular
                                                                      processes, which are largely untouchable. However,
                                                                      they can be overridden by "High-priority orders" or in the
                                                                      rescheduling editor with date assignments.

                                        Individual dates              Individual dates are campaigns which are executed just
                                                                      once.

                                        Weekly dates                  Weekly dates are campaigns which are run on a regular
                                                                      basis.

                                            Prerequisite
                                            Campaigns can be defined only if the appropriate work processes and
                                            shifts have been defined and if the corresponding shift plan is active.

                                             “Shifts” on page E-68
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                         E-43
                 Planning and Scheduling                                                                               Tutorial




                                             Definition of the Campaigns
                                             Campaigns serve especially to set up a machine correctly, e.g. for coatings
                                             that require long set-up times. This means that the machine is used in different
                                             modes.
                                             With campaigns, you can plan capacities for particular work processes, e.g. for
                                             screen printing in a different color for each day of the week. From this, e.g.
                                             campaigns Blue on Monday or Green on Tuesday are created. The advantage
                                             of reserving the screen printing capacities in this way is that the cleaning and
                                             set-up work can be minimized.
                                             Campaigns can also be set up so that particular work processes are done in a
                                             particular shift, e.g. all the cutting of special glass types in the first shift.
                                             The time reserved for a campaign can only be overridden by high-priority or-
                                             ders.




                                                                                                                   E


                 A




                 B




                                         C             D
                 A Work process of the campaign                         C Available shifts
                 B Day of the campaign                                  D Day of the planned campaign
                                                                        E Activated campaign
                 Fig. E-19   Campaigns
4.50 / 01-2023




                                             A campaign always applies for a particular work process (A). It is either spec-
                                             ified as individual date or as weekly date on a particular day of the week (B).
                                             If on the day there are several shifts available *C, the respective shifts must be
                                             specified.


                 E-44                                                                   A+W Production Capacity Planning
                 Tutorial                                                                          Planning and Scheduling




                                        Campaigns are used exclusively for work processes. The machine on which
                                        the processing is done plays no role here.
                                        For this, the work processes may not be bound to a particular machine.

                                           Example

                                           If two different screen printings are defined, during scheduling it must be
                                           detected which of the screen printings is the one in question. Here it plays no
                                           role on which machine the screen printing is done.
                                           A work process Screen printing for campaign X must be set up in the MA so
                                           that it is only used for campaigns. This work process must be assigned to the
                                           logical machine to which the campaigns are allocated.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                        E-45
                 Planning and Scheduling                                                                            Tutorial




                                           Campaigns in Scheduling
                                           For the scheduling for campaigns, all dates are hidden for which the work pro-
                                           cess does not apply.


                                                         Monday          Tuesday       Wednesday        Thursday




                                           A



                                                             B    C             D     E
                                           A Hidden work shifts                     D Flexible transition time
                                           B Flexible transition time               E Optimal solution
                                           C Second campaign of the BOM
                                           Fig. E-20     Scheduling for campaigns


                                           In this example, you see that the optimal solution (E) has a transition from one
                                           shift apiece. If the scheduling finds no result, it is checked whether there is a
                                           solution if campaign dates are ignored. If necessary, a corresponding mes-
                                           sage indicates that campaign dates are missing.
                                           Work processes with campaigns automatically receive a flexible transition time
                                           at entry. If in the BOM there are several campaigns (C), then the system
                                           searches for earlier start dates (B, D) in order to avoid conflicts.


                                           Definition and Management of Campaigns
                                           This unit will show you how to define, edit, or delete campaigns.
                                           For instructions on this subject, please see:
                                           •   “Here's how to define a campaign as an Individual date” on page E-47
                                           •   “Here's how to define a campaign as a weekly date” on page E-49
                                           •   “Here's how to edit a campaign” on page E-51
                                           •   “Here's how to delete a campaign” on page E-52

                                               Prerequisite
                                               Campaigns can be defined only if the appropriate work processes and
                                               shifts have been defined and if the corresponding shift plan is active.
4.50 / 01-2023




                                                “Here's how to draw up a shift plan” on page E-75




                 E-46                                                                  A+W Production Capacity Planning
                 Tutorial                                                                         Planning and Scheduling




                                         Here's how to define a campaign as an Individual date

                                            Prerequisite
                                            On the Individual dates tab, only activated shift plans are displayed. If nec-
                                            essary, activate the shift plans that are required for the campaign.

                                        1 Go to Master data > Capacity planning > Campaign planning.




                                        A




                                        B




                                        C




                                        A Work process                             C Duration of the campaign
                                        B Date of the campaign
                                        Fig. E-21     Creating a campaign


                                        2 Mark the work process (A) for the campaign.
                                            The buttons are enabled.
                                        3 Click the arrow to the right.
                                            The work process is displayed in the Campaigns field.
                                        4 Check the checkbox of this work process in the Campaigns field.
                                            The Individual dates tab is active now.
                                        5 Mark the date for the campaign (B) on the calendar.
                                            The Available shifts field lists the shifts that are available for this date.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                      E-47
                 Planning and Scheduling                                                                           Tutorial




                                           6 Choose the shift in which the campaign shall be run.
                                              If the shifts are not displayed, you must check in the corresponding shift
                                              rule whether the days of the week are marked on which the shift is avail-
                                              able.
                                               “Here's how to define a shift rule” on page E-78
                                           7 Specify how many days or weeks (B) the campaign should last.
                                           8 Click [+].
                                              The new campaign is displayed in the Individual dates field. If the campaign
                                              should run through several shifts, repeat the steps 6 - 8 for each individual
                                              shift.




                                           9 Click [OK] to save the campaign.
                                              The campaign is saved, the dialog closed.
4.50 / 01-2023




                 E-48                                                                  A+W Production Capacity Planning
                 Tutorial                                                                     Planning and Scheduling




                                         Here's how to define a campaign as a weekly date

                                            Prerequisite
                                            On the Weekly dates tab, only activated shift plans are displayed. If neces-
                                            sary, activate the shift plans that are required for the campaign.

                                        1 Go to Master data > Capacity planning > Campaign planning.




                                        A




                                        B




                                        C




                                        A Work process                          C Duration of the campaign
                                        B Date of the campaign
                                        Fig. E-22    Creating campaigns


                                        2 Mark the work process for the campaign.
                                            The buttons are enabled.
                                        3 Click the arrow to the right.
                                            The work process is displayed in the Campaigns field.
                                        4 Check the checkbox of this work process in the Campaigns field.
                                            The Weekly dates tab is enabled.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                 E-49
                 Planning and Scheduling                                                                                 Tutorial




                                           5 Change to the Weekly dates tab.




                                           A
                                           B




                                           A Campaign days                            B Shifts
                                               Fig. E-23     Weekly campaigns


                                           6 Mark the day of the week for the campaign (A) on the calendar.
                                               The Available shifts field lists the shifts that are available for this day of the
                                               week.
                                           7 Choose the shift in which the campaign shall be run.
                                           8 Click [+].




                                               The new campaign appears in the Weekly dates field. If the campaign
                                               should run through several shifts, repeat the steps 6 - 8 for each individual
                                               shift.
                                           9 Click [OK] to save the campaign.
                                               The campaign is saved, the dialog closed.
4.50 / 01-2023




                 E-50                                                                    A+W Production Capacity Planning
                 Tutorial                                                                  Planning and Scheduling




                                         Here's how to edit a campaign
                                        1 Go to Master data > Capacity planning > Campaign planning.
                                        2 In the Campaigns field, mark the campaign that you want to change.
                                           The tabs Individual dates and Weekly dates show the dates for which cam-
                                           paigns have been defined.




                                           Fig. E-24   Edit campaign


                                        3 Mark the date that you want to change.
                                        4 Click [Delete].
                                           The date is deleted.
                                        5 Select a new date or day or the week and the shift.
                                        6 Click [+].
                                           The new date is displayed.
                                        7 Click [OK] to save the changes.
                                           The change is saved, the dialog closed.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                              E-51
                 Planning and Scheduling                                                                            Tutorial




                                            Here's how to disable a campaign
                                           1 Go to Master data > Capacity planning > Campaign planning.
                                           2 In the Campaigns field, mark the campaign that you want to disable.
                                               The fields are locked.
                                           3 Click [OK] to save the changes.
                                               The change is saved, the dialog closed.
                                               The campaign is not included in the capacity planning. The campaign re-
                                               tains all of its properties. This way, you can switch campaigns on and off on
                                               short notice.


                                            Here's how to delete a campaign
                                           1 Go to Master data > Capacity planning > Campaign planning.
                                           2 Mark the campaign that you want to delete.
                                           3 Click the arrow to the left.
                                               The campaign including all its dates is deleted.
                                           4 Click [OK] to save the changes.
                                               The change is saved, the dialog closed.


                                           Exercises on Campaigns
                                           Create the data so that it is available in all subsequent exercises. If the data
                                           for the capacity planning is thus complete, you can test the planning for your
                                           own orders in the Production Monitor.
                                           •   Decide which work processes on your shop floor should be organized in
                                               campaigns.
                                           •   What is best for these work processes: A campaign as an individual date
                                               or a campaign as a weekly date?
                                           •   Create the appropriate campaigns.
                                           •   Edit the individual campaigns.
                                           •   Delete dates from campaigns.
                                           •   Delete campaigns.


                                           Additional information
                                            Software Reference, “Campaigns” on page E-183
4.50 / 01-2023




                 E-52                                                                 A+W Production Capacity Planning
                 Tutorial                                                                        Planning and Scheduling




                                        Reservations
                                        Objectives

                                        • What are reservations?
                                        • How are reservations defined, edited, and deleted?


                                        Benefit

                                        • Reservations can be used to keep capacities free for certain customers or projects.


                                        Note

                                                                    Reservations can be made only for bottleneck machines.

                                                                    Reservations are made for customers and projects.

                                           Prerequisite
                                           Reservations can be made only for machines defined as bottleneck ma-
                                           chines.

                                           Reservations in shifts, days or weeks
                                           Generally, capacities are reserved by the week. Depending on the setting
                                           under Master Data > Configuration > A+W Production > Capacity Planning
                                           > Type of Reservation, the reservation can also be specified for days or
                                           work shifts. If you change the setting, the old reservations are lost.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                      E-53
                 Planning and Scheduling                                                                            Tutorial




                                           Reservation of Capacities
                                           For individual customers or projects, you can reserve capacities on a particular
                                           machine. Generally, you reserve the capacity across the entire week, so that
                                           you are not dependent on when the order arrives.
                                           This way, capacities are held free so that the orders can be channeled through
                                           the bottlenecks without delay. Therefore, capacities can only be reserved for
                                           the work processes and machines for which bottlenecks can arise and which
                                           therefore are defined as bottleneck machines.
                                            “Here's how to define a machine as bottleneck machine” on page E-29.

                                               Reservations for individual orders
                                               Reservations for times for individual orders must be entered by the ERP
                                               system and transferred. The orders marked as Reserved order and re-
                                               leased for production reserve appropriate times on all machines required
                                               for the production.




                                           A




                                           B




                                           C




                                           A Machine for which the capacities are   B Detailed information
                                             displayed                              C Information about the reservation
                                               Fig. E-25   Reservations


                                           The capacities of the machines (A) are depicted graphically. Per day, all shifts
                                           are displayed that correspond to the selected period. For this, detailed infor-
                                           mation (B) is available.
                                           The reservations are displayed in a list (C) if a day is marked.
4.50 / 01-2023




                                           The daily capacity of a machine is defined by the shifts entered for this ma-
                                           chine.



                 E-54                                                                 A+W Production Capacity Planning
                 Tutorial                                                                      Planning and Scheduling




                                        When an order is transferred to A+W Production, the software checks whether
                                        there is a reservation for the customer or project in question.
                                        •   If so, A+W Production will allocate the order to the reserved capacity pro-
                                            vided there is enough free capacity left.
                                        •   If no reservation has been made for the customer or project yet, or if there
                                            is nothing left of the reserved capacity, the order will be allocated to non-
                                            reserved capacities.

                                        Expired reservations
                                        If there are expired reservations, the dialog Expired reservations will open
                                        when you open the Reservations dialog. You can delete expired reservations
                                        or take over future reservations by changing the expiration date.


                                        Definition and Management of Reservations
                                        This part of the tutorial will show you how to enter, edit, and delete reserva-
                                        tions.
                                        For instructions on this subject, please see:
                                        •   “Here's how to delete an expired reservation” on page E-60
                                        •   “How to enter a reservation” on page E-56
                                        •   “Here's how to edit a reservation” on page E-58
                                        •   “Here's how to delete a reservation” on page E-59

                                            Condition
                                            Reservations can only be made for machines defined as bottleneck ma-
                                            chines.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-55
                 Planning and Scheduling                                                                            Tutorial




                                            How to enter a reservation
                                           1 Go to Master data > Capacity planning > Reservations.
                                              If necessary, close the Expired Reservations dialog to open the Reserva-
                                              tions dialog.
                                               “Here's how to delete an expired reservation” on page E-60




                                              A
                                              B
                                              C




                                              A Machine                              C Number of days displayed
                                              B Start date
                                              Fig. E-26      Reservations


                                           2 Select the machine (A) on which you want to enter the reservation, e.g.
                                             Grinding.
                                           3 Select the start date (B) from which the reservation should apply.
                                           4 Specify the number of days (C) that should be displayed, e.g. 5.
                                              In the Shift reservations area, the shifts for the days are displayed on which
                                              the selected machine is available.
                                           5 Click [New].
4.50 / 01-2023




                 E-56                                                                 A+W Production Capacity Planning
                 Tutorial                                                                     Planning and Scheduling




                                           A

                                           B
                                           C




                                           D



                                           A Customer                             C Shift
                                           B Start date                           D Percentage reservation
                                           Fig. E-27      Create reservation


                                        6 Select a customer (A) or a project.
                                        7 Select the start date (B) and the shift (C) for the reservation.
                                        8 Specify the reservation in % (D).
                                           You can also click in the field above to specify the reservation visually.




                                        9 Click [OK] to save the reservation.
                                           The dialog closes. The data appears on the Reservations dialog.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-57
                 Planning and Scheduling                                                                               Tutorial




                                           10 In the Shift reservations field, select the day with the reservation.




                                              The reservations for the shift are listed in the List of reservations.
                                           11 Click [OK] to adopt the changes.
                                              The changes are saved and the dialog closed.


                                            Here's how to edit a reservation
                                           1 Go to Master data > Capacity planning > Reservations.
                                           2 Choose the machine for which you want to edit a reservation, e.g. Grinding.
                                           3 Select the start date from which the reservations should apply.
                                           4 Specify the number of days that should be displayed, e.g. 5.
                                              In the Shift reservations area, the shifts for the selected days are displayed
                                              on which the selected machine is available.
4.50 / 01-2023




                 E-58                                                                 A+W Production Capacity Planning
                 Tutorial                                                                     Planning and Scheduling




                                           Fig. E-28    Edit reservations


                                        5 Select the field to be edited from the List of reservations.




                                        6 Change the percentage value of the reservation.
                                        7 Click [OK] to adopt the changes.
                                           The changes are saved and the dialog closed.


                                         Here's how to delete a reservation
                                        1 Go to Master data > Capacity planning > Reservations.
                                        2 Choose the machine for which you want to edit a reservation, e.g. Grinding.
                                        3 Select the start date from which the reservations should apply.
                                        4 Specify the number of days that should be displayed, e.g. 5.
                                           In the Shift reservations area, the shifts for the selected days are displayed
                                           on which the selected machine is available.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-59
                 Planning and Scheduling                                                                      Tutorial




                                           5 Select the line with the reservation that should be deleted.




                                           6 Click [Delete].
                                              The selected reservation is deleted from the list.
                                           7 Click [OK] to adopt the changes.
                                              The changes are saved and the dialog closed.


                                            Here's how to delete an expired reservation
                                           1 Go to Master data > Capacity planning > Reservations.




                                              Fig. E-29    Expired reservations


                                           2 Select the reservations to be deleted from the list.
                                           3 Click [Delete].
                                              The reservations are deleted.
                                           4 Click [OK] to save the changes.
                                              The Expired Reservations dialog closes and the Reservations dialog
                                              opens.
4.50 / 01-2023




                 E-60                                                                A+W Production Capacity Planning
                 Tutorial                                                                      Planning and Scheduling




                                        Exercises on Reservations
                                        •   Enter a reservation for several days and shifts for a customer or a project.
                                        •   Enter a test order for a customer or a project with a delivery date at the end
                                            of the two weeks.
                                        •   Schedule the order.
                                        •   Check the results.
                                        •   Make a new reservation and enter a new order which exceeds the reserved
                                            capacities.
                                        •   Schedule the order and check the results.
                                        •   Edit the reservations.


                                        Additional information
                                         Software Reference, “Reservations” on page E-187
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                   E-61
                 Planning and Scheduling                                                                                  Tutorial




                                           Creating Processings
                                           Objectives

                                           • What does creation of processings mean?
                                           • How are processing steps created and added to the BOM?


                                           Benefit

                                           • The PPS system needs a more detailed BOM that includes all work steps in order
                                             to calculate the individual production dates and production costs. This is created by
                                             creating processings within the course of scheduling.


                                           Note

                                           Processings                  Processing steps define the product's need to be
                                                                        processed, e.g. arrissing.

                                           Work processes               Work processes define the way in which the need for
                                                                        processing shall be served, e.g. a special type of
                                                                        arrissing.

                                              Prerequisite
                                              Processing steps can be created only by allocating processing articles to
                                              element types. The definition of processing types, processing articles, and
                                              element types is described in the Master Data section.
                                              Please agree any changes in the creation of processings with the A+W
                                              Software GmbH customer service because these are relevant for produc-
                                              tion.
4.50 / 01-2023




                 E-62                                                                    A+W Production Capacity Planning
                 Tutorial                                                                    Planning and Scheduling




                                        Creation of Processings for Scheduling
                                        The BOM of the ERP system includes the end product to be produced with its
                                        sub-elements and price-relevant processings, e.g. arrissing of the edges. Oth-
                                        er production steps are only included implicitly in this BOM, e.g. cutting.
                                        For the calculation of the individual production dates and costs, A+W Capacity
                                        Planning needs a more detailed BOM with all steps for which expenditures of
                                        time and costs are required.Therefore, in the course of scheduling, production-
                                        relevant steps are added to the production BOM. The creation of processings
                                        thus ensures that for each BOM element it is described how it arises in pro-
                                        duction.

                                                                                       B




                                        A




                                        A Processings with the assigned        B Element types with assigned
                                          processing articles                    processings
                                        Fig. E-30    Creation of processings


                                        So that the processings can be created for the elements of the BOM, these
                                        processings must be permitted on the corresponding element types. By as-
                                        signing the processing (A) to an element type (B), the production BOM can be
                                        created so that all time and cost-relevant calculations can be made.
                                        Therefore, for the capacity planning, processing must be defined at least for
                                        all stock removals, purchased and cut elements and for the assembly of LAMI
                                        and IG.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-63
                 Planning and Scheduling                                                                         Tutorial




                                           Creation of Processings
                                           This unit will show you how to complete the BOM by processing steps which
                                           are relevant for production.
                                           For instructions on this subject, please see:
                                           •   “Here's how to add a processing” on page E-64
                                           •   “Here's how to remove a processing step from the creation of processings”
                                               on page E-65


                                            Here's how to add a processing

                                               Adding processings
                                               When processings are added, changes will be applied as soon as they are
                                               made in the dialog.
                                               They cannot be undone.

                                               Please contact the A+W Software GmbH customer service if you want to
                                               change processings.

                                           1 Go to Master data > Capacity planning > Creation of processings.




                                           Fig. E-31    Assigning processing article
4.50 / 01-2023




                                           2 Go to field Processings and select the processing article you want to assign
                                             to an element type.


                 E-64                                                                  A+W Production Capacity Planning
                 Tutorial                                                                     Planning and Scheduling




                                        3 Go to the Element types field and select the processing article you want to
                                          assign to the processing article.
                                        4 Click the arrow to the right.
                                           The processing article is assigned to this article type.
                                        5 Click [OK] to save the data.
                                           The assignment will be saved.


                                         Here's how to remove a processing step from the creation of
                                          processings

                                           Add processings
                                           When processings are added, changes will be applied as soon as they are
                                           made in the dialog. They cannot be undone.
                                           Please contact the A+W Software GmbH customer service if you want to
                                           change processings.

                                        1 Go to Master data > Capacity planning > Creation of processings.




                                        Fig. E-32    Removing an assignment


                                        2 In field Part types, select the processing article to be removed.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                               E-65
                 Planning and Scheduling                                                                    Tutorial




                                           3 Click the arrow to the left.
                                              The assignment will be removed from the article type.
                                           4 Click [OK] to save the data.
                                              The change is saved.
4.50 / 01-2023




                 E-66                                                              A+W Production Capacity Planning
                 Tutorial                                                            Master Data of Capacity Planning




                                        Master Data of Capacity Plan-
                                        ning
                                        In order to be able to work with A+W Capacity Planning, the master data for
                                        the capacity planning must be set up. This master data forms, together with
                                        the master data for the machine allocation (MA) and the master data for the
                                        article, the basis for the scheduling of orders and planning by A+W Capacity
                                        Planning.
                                        Before you set up or edit the master data for capacity planning, the machines
                                        and work processes must be described completely. Information about this top-
                                        ic is in the Machine Allocation section.

                                            Protecting master data against access
                                            The master data of A+W Production and especially of A+W Capacity Plan-
                                            ning are highly sensitive data. Uncontrolled or unintentional interventions
                                            and changes can bring production to a complete standstill.
                                            Therefore, set up the workstations so that only the administrators or em-
                                            ployees with appropriate functions have access to the master data.

                                        This section provides information on the following subjects:
                                        •   “Shifts” on page E-68
                                        •   “Cost Calculation” on page E-87
                                        •   “Transition Times” on page E-92
                                        •   “Default Times” on page E-105
                                        •   “Machinery Groups” on page E-131
                                        •   “Load Distribution” on page E-137

                                            Data back-up
                                            Before you begin editing the master data, create a complete data back-up
                                            of the master data. The back-up tool is under
                                            C:\Programs (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe.Move
                                            the saved back-up from your user directory into a directory to which support
                                            also has access.
                                            Discuss the upcoming change in advance with your planner atA+W Soft-
                                            ware GmbH
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                 E-67
                 Master Data of Capacity Planning                                                                            Tutorial




                                         Shifts
                                         Objectives

                                         •   What's the calendar for?
                                         •   What is a shift?
                                         •   What details are required for a shift?
                                         •   How are shifts defined, edited, and deleted?


                                         Benefit

                                         • With shifts, you define in which period work is done on particular machines.


                                         Note

                                         Calendar                     With the calendar, you define non-working days, e.g.
                                                                      legal holidays or company holidays.

                                         Work shift                   Work shifts are displayed in the Production Monitor. A
                                                                      work shift is defined as a shift plan with shift rules and
                                                                      shift groups.

                                         Shift plan                   In the shift plan, you define with shift rules and shift
                                                                      groups:
                                                                      • In how many shifts work is done.
                                                                      • On which days the shift is available.
                                                                      • For which machines the rules apply.

                                         Shift rule                   A shift rule defines the details of a shift, e.g. the shift
                                                                      duration.
                                                                      For each shift rule, only one shift group can be defined.
                                                                      All shift rules of a shift plan must have this same shift
                                                                      group.

                                         Shift group                  In a shift group, the machines are specified that work in
                                                                      this shift. All shift rules of a shift must have the same
                                                                      machine groups.
4.50 / 01-2023




                 E-68                                                                    A+W Production Capacity Planning
                 Tutorial                                                               Master Data of Capacity Planning




                                         Shift Plans
                                         With shift plans, you define work shifts that are displayed in the Production
                                         Monitor. In the shift plan, you specify in which period the machine works in your
                                         production. An individual work shift can be changed or deleted in the Produc-
                                         tion Monitor without having the change taken over in the shift plan.




                 A
                   B
                 C
                   D                                                                                     E



                                                                                                         F




                 A Calendar                                          D Shift rule with assigned machines
                 B Shift plan                                        E Shift plan is available
                 C Shift rule                                        F Generate data for the Production Monitor
                 Fig. E-33      Shifts


                                         The calendar (A) forms a general basis, on which you specify the non-working
                                         days, e.g. the public holidays or company holidays.
                                         You define the shifts in A+W Production with the shift plan (B) with shift rules
                                         (C) and shift groups (D).
                                         •   The shift plan (B) defines the general conditions. You can e.g. create a shift
                                             plan called Two-shift which specifies two-shift operation. The Two-shift shift
                                             plan specifies whether this shift plan is active, when it comes into effect and
                                             for how long, and whether you will be using an individual shift calendar or
                                             if the shift calendar will be imported from the ERP system.
                                         •   For each shift plan, there is at least one shift rule (C) with which you specify
                                             on which days and at what times work is done, e.g. in two-shift operation
                                             from Monday to Friday, from 6AM to 2PM for the early shift and from 2PM
4.50 / 01-2023




                                             to 10PM for the late shift.
                                         •   The shift rule applies for a shift group (D) in which you define which ma-
                                             chines work in which shifts. Thus, for example, you can specify that one of
                                             your cutting tables is always only active in the early shift or that the CNC


                 A+W Production Capacity Planning                                                                      E-69
                 Master Data of Capacity Planning                                                                  Tutorial




                                            center is also in operation on Saturdays. Only one shift group can be added
                                            to each shift rule. If you are using several shift rules, all of them must in-
                                            clude the same shift group.
                                            With the shift rules, you can set up the planning so that, e.g. the machines
                                            on which bottlenecks can arise work in several shifts, but all others work in
                                            only one shift.
                                         Each shift plan can initially be defined regardless of the capacity planning. This
                                         way, you can create shift plans that you activate only at particular times (E),
                                         e.g. for special shifts.
                                         Furthermore, each shift plan can only be valid to a limited extent. Thus, for ex-
                                         ample, you can create a shift plan for a planned construction project that is
                                         only valid for the time in which the lites must be delivered. This way, these
                                         times are not included in the planning outside the validity period.
                                         When you create or change a shift plan, the shift is only taken over as work
                                         shift into the Production Monitor if it is generated explicitly with (F). The new
                                         work shifts are consider for the scheduling in A+W Capacity Planning for the
                                         new orders; already scheduled orders are unaffected by this.
                                         You can display an overview of the work shifts and their utilization on the Pro-
                                         duction Monitor dialog.
                                          Software Reference, “Scheduling” on page E-146
4.50 / 01-2023




                 E-70                                                                A+W Production Capacity Planning
                 Tutorial                                                            Master Data of Capacity Planning




                                        Definition of non-working Days
                                        This unit will show you how to define, edit, or delete non-working days.

                                            Setting up the calendar
                                            You must set up the calendar before you define shift plans. Non-working
                                            days are only considered for new shifts.

                                        For instructions on this subject, please see:
                                        •   “Here's how to define non-working days” on page E-71
                                        •   “Here's how to edit non-working days” on page E-72
                                        •   “Here's how to delete non-working days” on page E-73


                                         Here's how to define non-working days
                                        1 Go to Master data > Capacity planning > Shifts.

                                                    A                               B




                                        A Select calendar                       B Non-working days
                                        Fig. E-34       Shift Calendar
4.50 / 01-2023




                                        2 In the Shift editor field, select the Calendar entry (A).



                 A+W Production Capacity Planning                                                                  E-71
                 Master Data of Capacity Planning                                                                Tutorial




                                         3 Click [New].
                                            A new line is added in the Shift calendar area.
                                         4 In the Day and Comment fields, enter the data, e.g. a national holiday.
                                         5 Click [Accept].
                                            The data is saved. When creating new shifts, the non-working days are
                                            skipped.


                                          Here's how to edit non-working days
                                         1 Go to Master data > Capacity planning > Shifts.
                                         2 In the Shift editor field, select the Calendar entry.




                                         Fig. E-35    Edit calendar


                                         3 In the Shift calendar field, select the date that you want to edit.
                                         4 Change the values.
                                         5 Click [Accept].
                                            The data is saved.
4.50 / 01-2023




                 E-72                                                               A+W Production Capacity Planning
                 Tutorial                                                            Master Data of Capacity Planning




                                         Here's how to delete non-working days
                                        1 Go to Master data > Capacity planning > Shifts.
                                        2 In the Shift editor field, select the Calendar entry.
                                        3 In the Calendar area, in the first column, select the day that you want to de-
                                          lete.

                                                A                          B




                                        A Calendar                               B Selection
                                        Fig. E-36    Deleting non-working days


                                        4 Click [Delete].
                                           The day with the arrow in the first column is deleted.
                                        5 Click [Accept].
                                           The data is saved.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                 E-73
                 Master Data of Capacity Planning                                                                Tutorial




                                         Create a Shift Plan
                                         This unit will show you how to define, edit, or delete shift plans.
                                         A new work shift can only be created if you have created at least one shift rule
                                         and a shift group with machines for the new shift plan.
                                         For instructions on this subject, please see:
                                         •   “Here's how to draw up a shift plan” on page E-75
                                         •   “Here's how to edit a shift plan” on page E-76
                                         •   “Here's how to delete a shift plan” on page E-77

                                             Import data
                                             When you create or change a shift plan, a shift rule or a shift group, you
                                             must click [New] so that the changed shift data is created in the Production
                                             Monitor. If the changed shift is not created, A+W Production plans produc-
                                             tion with the old shift data.
4.50 / 01-2023




                 E-74                                                               A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                         Here's how to draw up a shift plan
                                        1 Go to Master data > Capacity planning > Shifts.
                                        2 In the Shift editor field, select the Calendar entry.

                                                     A




                                                                                   B
                                        A Select context menu                   B Select button
                                        Fig. E-37    New shift plan


                                        3 With a right-Click the calendar, open the context menu (A) and select the
                                          New shift plan entry.
                                           Alternatively, you can open the selection list (B) on the [New] button and
                                           select New shift plan.
4.50 / 01-2023




                                        4 In the Shift plan area, in the Name field, enter a name, e.g. Two-shift nor-
                                          mal.


                 A+W Production Capacity Planning                                                                E-75
                 Master Data of Capacity Planning                                                                Tutorial




                                         5 Click [Accept].
                                            The data is saved. The new shift plan is displayed in the shift editor.
                                            Next, you must set up the shift rules and assign the machines. Only after
                                            that is the [Create] button enabled.
                                             “Defining a Shift Rule” on page E-77


                                          Here's how to edit a shift plan
                                         1 Go to Master data > Capacity planning > Shifts.
                                         2 Select the shift plan to be edited in the Shift editor area.




                                         3 Edit the values for the shift plan.
                                            A typical application case is the extension of a shift plan.
                                         4 Check whether the Active checkbox is checked so that the shift plan can
                                           be used in the capacity planning.
                                         5 Click [Accept].
                                            The data is saved.
                                         6 Click [Create] to create the changed data in the Production Monitor.
4.50 / 01-2023




                 E-76                                                                A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                         Here's how to delete a shift plan

                                            Deleting a shift plan
                                            If you delete a shift plan, the corresponding shift rule and shift group will be
                                            deleted as well! The deleted shift will still be displayed in the Production
                                            Monitor. To delete it from the Production Monitor, you must first reschedule
                                            the scheduled processings.

                                        1 Go to Master data > Capacity planning > Shifts.
                                        2 Select the shift plan to be deleted in the Shift editor area.
                                        3 Click [Delete].
                                            The shift plan is deleted from the shift editor.
                                        4 Click [Accept].
                                            The data is saved.


                                        Defining a Shift Rule
                                        This unit will show you how to define, edit, or delete shift rules.
                                        For instructions on this subject, please see:
                                        •   “Here's how to define a shift rule” on page E-78
                                        •   “Here's how to edit a shift rule” on page E-80
                                        •   “Here's how to delete a shift rule” on page E-81

                                            Import data
                                            When you create or change a shift plan, a shift rule or a shift group, you
                                            must click [New] so that the changed shift data is created in the Production
                                            Monitor. If the changed shift is not created,A+W Production plans produc-
                                            tion with the old shift data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                     E-77
                 Master Data of Capacity Planning                                                               Tutorial




                                          Here's how to define a shift rule
                                         1 Go to Master data > Capacity planning > Shifts.
                                         2 Select the shift plan to which the shift rule will be assigned.

                                                        A




                                                                                    B
                                         A Select context menu                   B Select button
                                         Fig. E-38    New shift rule


                                         3 Open the context menu for the shift plan (A) and select the New shift plan
                                           entry.
                                            Alternatively, you can open the selection list (B) on the [New] button and
                                            select New shift plan.
4.50 / 01-2023




                 E-78                                                               A+W Production Capacity Planning
                 Tutorial                                                                 Master Data of Capacity Planning




                                                                                              A
                                                                                              B



                                                                                              C




                                                                                              D


                                           A Name of the shift rule                    C Shift number
                                           B Start and end date                        D Calendar – selection
                                           Fig. E-39    Definition of the shift rule


                                        4 Enter a name (A) and a shift number (C), e.g. Early shift and number 1.
                                        5 Select the time for shift beginning and shift end (B), e.g. beginning at 6AM
                                          and end at 2PM.
                                        6 Select the weekdays on which this shift shall be run, e.g. Mon-Fri for a five-
                                          day working week.
                                        7 Select whether you want to use your own calendar (D) or if the calendar
                                          shall be imported from the ERP system, e.g. from A+W Enterprise.
                                           You must only specify the validity period if you are setting up a special shift.
                                        8 Click [Accept].
                                           The data is saved. The new shift plan is displayed in the shift editor.
                                           Next, you must set up the shift groups and assign the machines. Only after
                                           that will the [Create] button be enabled.
                                            “Creating a Shift Group” on page E-82
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                    E-79
                 Master Data of Capacity Planning                                                                 Tutorial




                                          Here's how to edit a shift rule
                                         1 Go to Master data > Capacity planning > Shifts.
                                         2 Select the shift rule you want to edit.




                                                                                         A            B          C
                                         A Changing the validity period          B Saving shift data
                                                                                 C Creating data for planning
                                         Fig. E-40    Editing a shift rule


                                         3 Change the entries in the Shift rule section.
                                            A typical change is to extend a shift plan. For this, change the time period
                                            (A). The fields for the period are only enabled if at least one shift group is
                                            assigned.
                                         4 Click [Accept] (B).
                                            The data is saved.
                                         5 Click [Create] (C) to create the shift with the changed data in the Production
                                           Monitor.
                                            The shift is displayed with the changed data in the Production Monitor.
4.50 / 01-2023




                 E-80                                                                A+W Production Capacity Planning
                 Tutorial                                                               Master Data of Capacity Planning




                                         Here's how to delete a shift rule
                                        1 Go to Master data > Capacity planning > Shifts.
                                           Before you delete a shift rule, you should restrict the validity. This way, the
                                           shifts are no longer displayed in the Production Monitor and they can no
                                           longer be booked.
                                        2 Select the shift rule that you want to delete.




                                                                                               A           B
                                        A Deleting a shift rule                   B Deleting a shift rule for shift plan
                                        Fig. E-41     Deleting a shift rule


                                        3 Click [Delete] (A).
                                           The shift rule is deleted from the editor.
                                        4 Click [Delete] (B).
                                           The shift is deleted from the Production Monitor.

                                           Deleting a shift
                                           You can delete a work shift in the Production Monitor. Here, only the indi-
                                           vidual shift is deleted. If you want to delete shifts by deleting the shift rules,
                                           you should first check the shifts in the Production Monitor. Under some cir-
                                           cumstances, you must shift orders that are still scheduled.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                          E-81
                 Master Data of Capacity Planning                                                                Tutorial




                                         Creating a Shift Group
                                         This unit will show you how to define, edit, or delete shift groups.
                                         For instructions on this subject, please see:
                                         •   “How to create a shift group” on page E-82
                                         •   “Here's how to edit a shift group” on page E-85
                                         •   “How to delete a shift group” on page E-86

                                             Import data
                                             When you create or change a shift plan, a shift rule or a shift group, you
                                             must click [New] so that the changed shift data is created in the Production
                                             Monitor.
                                             If the changed shift is not created, A+W Production plans the production
                                             with the old shift data.


                                          How to create a shift group
                                         1 Go to Master data > Capacity planning > Shifts.
                                         2 Go to section Shift editor and select the shift rule to which the shift group
                                           will be allocated.

                                                          A




                                                                                    B
4.50 / 01-2023




                                         A Select context menu                   B Select button
                                         Fig. E-42    New shift group




                 E-82                                                               A+W Production Capacity Planning
                 Tutorial                                                               Master Data of Capacity Planning




                                        3 Open the context menu for the shift rule (A) and select the New shift group
                                          entry.
                                           Alternatively, you can open the selection list (B) on the [New] button and
                                           select New shift group.


                                                                                           A




                                                                                          B




                                           A Name of Shift Group                    B Assigning the shift group
                                           Fig. E-43    Definition of the shift group


                                        4 Select a shift group in the Name field (A) or enter a name.
                                           Section Edit shift group lists the available machines.
                                        5 Click [Accept] to save the data.
                                        6 For all machines you want to assign the new shift group, select the name
                                          of this shift group (B) in the Shift group column.
4.50 / 01-2023




                                        7 Assign every machine to a shift group this way.
                                        8 Click [Accept].


                 A+W Production Capacity Planning                                                                 E-83
                 Master Data of Capacity Planning                                                                   Tutorial




                                            The data is saved. The new shift group is displayed in the shift editor with
                                            all assigned machines.




                                            After you have completely defined the shift plan, you can create the shift in
                                            the Production Monitor. To do this, proceed as follows:
                                         9 Select the new shift plan in the shift editor.
                                            The Shift plan area is displayed.
                                         10 Check the Active checkbox and enter the date starting on which the shift
                                            plan is valid.
                                         11 Click [Create].
                                            This creates the shift and so the shift is available for capacity planning start-
                                            ing on the validity date and if necessary for the specified time period.
4.50 / 01-2023




                 E-84                                                                A+W Production Capacity Planning
                 Tutorial                                                            Master Data of Capacity Planning




                                         Here's how to edit a shift group
                                        1 Go to Master data > Capacity planning > Shifts.
                                        2 Select the shift group to be edited from section Shift editor.




                                        Fig. E-44    Edit shift group


                                        3 In the Edit shift group area, change the dates, e.g.:
                                           •   Assign machines to other shift groups.The change of the assignment of
                                               a machine to a machinery group is a typical application case for moving
                                               a machine to a different shift operation.
                                           •   Changing the name of a shift group.
                                        4 Click [Accept] to save the data.
                                           The data is saved.
                                        5 Select the current shift rule.
                                           The Shift rule area is displayed with the current data.
                                        6 Check the data and if necessary, adjust the settings, e.g. the validity period.
                                           After you have edited the shift plan, you can create the changed shift in the
                                           Production Monitor. To do this, proceed as follows:
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-85
                 Master Data of Capacity Planning                                                                 Tutorial




                                         7 Click [Create].
                                             This needs to be done for all shifts.


                                          How to delete a shift group
                                         1 Go to Master data > Capacity planning > Shifts.
                                         2 Select the shift group to be deleted from section Shift editor.
                                         3 Click [Delete].
                                             The shift group is deleted.
                                         4 Click [Accept] to save the data.
                                             The data is saved.


                                         Exercises
                                         Create the data so that it is available in all subsequent exercises. If the data
                                         for the capacity planning is thus complete, you can test the planning for your
                                         own orders in the Production Monitor.
                                         •   Plan your production on paper. Which shifts will be worked on which days,
                                             and which machines will be used for the individual shifts?
                                         •   Transfer your results to A+W Production by defining the shifts.
                                         •   Check your results in the Production Monitor.
                                              Software Reference, “Scheduling” on page E-146
                                         •   Change the shift plan for a machine, e.g. from two-shift to three-shift oper-
                                             ation.
                                         •   Extend an existing shift plan.


                                         Additional information
                                          Software Reference, “Shifts” on page E-221
4.50 / 01-2023




                 E-86                                                                A+W Production Capacity Planning
                 Tutorial                                                                Master Data of Capacity Planning




                                        Cost Calculation
                                        Objectives

                                        • What is cost calculation in capacity scheduling?
                                        • How are the costs for logical machines entered, edited, or deleted?
                                        • Which data are exchanged between A+W Production and the ERP system in
                                          connection with cost calculation?


                                        Benefit

                                        • With cost calculation, a cost optimization can be achieved. Together with the
                                          transition times, first the more economical machines are utilized for the scheduling.
                                        • The exact breakdown and reporting of costs offers the following advantages:
                                          - Exact cost calculation for quotation and order entry in the ERP system.
                                          - Scheduling on more economical machines.
                                          - Cost-cased statistical analysis.


                                        Note

                                                                     With the cost calculation, you can determine personnel
                                                                     costs, machine costs, and other costs.

                                                                     Labor and machine costs are stored in A+W Capacity
                                                                     Planning per machine.

                                                                     Material costs are stored and calculated in the ERP
                                                                     system.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                        E-87
                 Master Data of Capacity Planning                                                                    Tutorial




                                         Definition of the Cost Calculation
                                         For logical machines, you can specify the costs that arise for production, If an
                                         order or a quotation is scheduled, A+W Production reports the costs back to
                                         the ERP system. This way, the person entering the order can query the pro-
                                         duction costs that arise for production. The material costs are stored and cal-
                                         culated in the ERP system.

                                                      A         B




                                         A Physical machine                        B Assigned logical machine
                                         Fig. E-45    Cost calculation


                                         Enter the costs per hour and logical machine. This way, you can weight the
                                         costs of a physical machine differently, depending on which logical machine is
                                         addressed. You specify machine costs, labor costs, and other costs separately
                                         per logical machine.

                                            Example

                                            Various edge processings can be executed on your single-sided grinding
                                            machine, e.g. grinding, polishing, and mitering.
                                            The various work processes are created not just as different processings, but
                                            also as different logical machines.
                                            The machine tools for possible processings have different costs for the tool
                                            downtime and reprocurement. You map these differences via the costs of the
                                            logical machine that are defined for the physical machine.
                                            At the same time, you can consider the different speeds for the processing in
                                            different specified times.
4.50 / 01-2023




                 E-88                                                                 A+W Production Capacity Planning
                 Tutorial                                                                Master Data of Capacity Planning




                                        Definition and Management of Costs
                                        This unit will tell you how to enter, edit, and delete the costs for logical ma-
                                        chines.
                                        For instructions on this subject, please see:
                                        •   “How to define the costs for a logical machine” on page E-89
                                        •   “How to edit the costs for a logical machine” on page E-90
                                        •   “How to delete the costs for a logical machine” on page E-91


                                         How to define the costs for a logical machine
                                        1 Go to Master data > Capacity planning > Cost calculation.
                                            The Cost Calculation dialog opens.
                                        2 Click [New].
                                            A line with the machine -1 is inserted into the list.

                                                        A                           B




                                            A Machine                               B Costs
                                            Fig. E-46    New line for cost calculation


                                        3 Double-Click the -1 field (A).
                                            The Please select a machine dialog appears.
                                        4 Select the desired machine with a double-click.
                                        5 Double-Click the empty field Log. Machine.
                                            The Please select a machine dialog appears. It lists all logical machines de-
4.50 / 01-2023




                                            fined for the selected machine.
                                        6 Select the desired logical machine with a double-click.
                                        7 Enter the labor costs per hour for a worker.


                 A+W Production Capacity Planning                                                                    E-89
                 Master Data of Capacity Planning                                                                Tutorial




                                            If two people are required for the work process, you must enter twice the
                                            costs.
                                         8 Repeat step 7 for the fields Machine costs and Other costs (B).
                                            You can enter a comment, e.g. in order to explain the labor costs.
                                         9 Click [OK].
                                            The data is saved and the dialog closed.


                                          How to edit the costs for a logical machine
                                         1 Go to Master data > Capacity planning > Cost calculation.




                                            Fig. E-47    Edit cost calculation


                                         2 Change the value of the field in question, e.g. Other Costs.
                                         3 Repeat step 2 for all costs whose entries are outdated.
                                         4 Click [OK].
                                            The data is saved and the dialog closed.
4.50 / 01-2023




                 E-90                                                             A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                         How to delete the costs for a logical machine
                                        1 Go to Master data > Capacity planning > Cost calculation.
                                        2 Mark the line that you want to delete.
                                        3 Click [Delete].
                                            The entry will be deleted from the list.
                                            If you have deleted the entry by accident, cancel the process with [End].
                                        4 Click [OK].
                                            The data is saved and the dialog closed.


                                        Exercises
                                        Create the data so that it is available in all subsequent exercises. If the data
                                        for the capacity planning is thus complete, you can test the planning for your
                                        own orders in the Production Monitor.
                                        •   Select your machine and formulate the costs for the associated logical ma-
                                            chines:
                                            Which labor costs, machinery costs, and other costs are incurred for the
                                            logical machine.
                                        •   Enter the costs for the logical machine on the Cost calculati-on dialog.
                                        •   Enter a test order or test quotation and schedule it for this machine. Check
                                            the reported prices.
                                        •   Edit the costs for the logical machines in dialog Cost calculation.


                                        Additional information
                                         Software Reference, “Cost Calculation” on page E-232
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-91
                 Master Data of Capacity Planning                                                                       Tutorial




                                         Transition Times
                                         Objectives

                                         • What are transition times?
                                         • How are transition times defined, edited, and deleted?


                                         Benefit

                                         • Transition times shape the time movement of the lites through production.


                                         Note

                                         Transition Time             A transition time describes the span between the end
                                                                     points of sequential processings.
                                                                     If two sequential work processes are done on the same
                                                                     machine, there are no transition times, e.g. drilling and
                                                                     washing.
                                                                     Transition times are defined exclusively for logical
                                                                     machines.

                                         Transition type             Transition times are defined as three different types:
                                                                     normal, rush transition, minimal transition.

                                         Normal transition           Normal transitions describe the optimal production
                                                                     process, e.g. without absences of personnel or machine
                                                                     breakdowns, breakage, etc.

                                         Rush transition             Rush transitions describe accelerated processing, e.g. in
                                                                     that the dwell times are shortened. However, these
                                                                     transition times increase the costs.

                                         Minimal transition          Minimal transitions are the most expensive transition
                                                                     times.

                                         Transition time 0           Processings that follow one another directly have no
                                                                     transition times, e.g. spacer bending - IG line - IG edge
                                                                     sealing.
                                                                     For these processings, all three types of transition times
                                                                     are identical.

                                         Explicit transition         You define the transition from machine x to machine y as
                                                                     an explicit transition.

                                         Hierarchical evaluation     The stored transition times are evaluated in the following
                                                                     sequence:
                                                                     •   Machine x -> Machine y.
                                                                     •   Machine x -> All machines.
                                                                     •   All machines -> machine x.
                                                                     •   All machines -> all machines.
4.50 / 01-2023




                 E-92                                                                  A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                        Note

                                        Dwell times              Dwell times refer to times that pass without any
                                                                 processing, e.g. for lite sorting, wait time for remakes,
                                                                 drying times.
                                                                 Required dwell times cannot be sped up, e.g. the times
                                                                 for heat soak.
                                                                 Dwell times are calculated into the transition times.

                                        Set-up time              Set-up times are calculated into the transition times.

                                        Customer handling time   This refers to the time that is required to load the
                                                                 packaged goods. Generally one working day is set for
                                                                 this. For loading a container, however, several days may
                                                                 be required.
                                                                 This time is not calculated into the date optimization and
                                                                 it is therefore not defined as transition time. It is stored in
                                                                 the ERP in the customer's master data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                         E-93
                 Master Data of Capacity Planning                                                                             Tutorial




                                              Transition Times in Shifts or Hours
                                              With transition times, you define the time between two processings or two (log-
                                              ical) machines. These time vary depending on from which machine a lite
                                              comes and to which machine it is going.
                                              The simplest form of the transition time is the time for the path that a lite re-
                                              quires from one (logical) machine to the next one, e.g. the transition from cut-
                                              ting to the next processing. These times are defined as optimal transitions with
                                              the type Normal. If the transition can be sped up, times with the type Rush and/
                                              or Minimal are created.
                                               “Transition types” on page E-99


                                                   Wednesday            Thursday                Friday             Monday


                  Float cutting

                  Sorting for

                  Coating system

                  Sorting for IG

                                                                                          1
                  Spacer bender 1

                  IG line 2
                                                                                                         0

                  Seal IG
                                                                                                             2                0
                  Packing

                  Vehicle fleet



                                                                                     A            B                       C
                 A Alternative - with or without       B Transition time within a shift        C Transition of 2 shifts
                   coating
                 Fig. E-48      Backwards calculation with normal transition times


                                              In this example, you see the optimal flow with the normal transition times for
                                              an IG lite with a coated lite. If in the IG only one lite is coated (A), the cutting
                                              is divided across two shifts so that the lite to be coated is cut earlier. Since
                                              Spacer bender - IG line - Seal IG (B) must always be done one after another,
                                              these processings are done in the same shift.
4.50 / 01-2023




                                              The transition is regarded in each case from the end of a shift. The transition
                                              from packing to sealing (C) is specified with 2 shifts, for example, This way,
                                              there is enough room for play within the shift in which the processing is sue.



                 E-94                                                                         A+W Production Capacity Planning
                 Tutorial                                                               Master Data of Capacity Planning




                                        Each transition to another shift generates virtual costs, which are higher the
                                        more the transition deviates from optimal transition. From this point of view, the
                                        transitions must be designed optimally.

                                        Transition times in shifts
                                        Maximum transition times are only evaluated for Normal transitions. The other
                                        transitions are filled out automatically as minimal. If there is an entry of the type
                                        Minimal, faster transitions are forbidden. For Rush transitions, it is enough to
                                        specify the minimum number of shifts.


                                               Wednesday          Thursday          Friday           Monday




                                                                              A                B          C
                                        A Optimal and maximal                     B Rush transition time
                                          transition time                         C Minimum transition time
                                        Fig. E-49     Transitions in shifts


                                        In this example, the normal transition time (A) is specified across five shifts,
                                        which can be extended to a maximum of seven. The rush transition (B) is de-
                                        fined with three shifts. The program can thus automatically also calculate four
                                        shifts.
                                        With the minimum transition time of precisely one shift (C), the transition in the
                                        same shift is forbidden automatically. The transition of two shifts is calculated
                                        in automatically.
                                        This means that you must only make four specifications: Normal with 5 + 2,
                                        Rush with 3 shifts, and Minimal with 1 shift. This way, seven possible shift tran-
                                        sitions can be calculated.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                      E-95
                 Master Data of Capacity Planning                                                                     Tutorial




                                         Transition times in hours
                                         The transition time in hours does not refer to work time, but to the calendar
                                         time and is also evaluated with the virtual costs. The program specifies the
                                         transition times in hours in general in the work time.
                                         Processing dates always refer to the shift end. With a transition time of 00:00
                                         hours, the lites are automatically passed to the next machine, that is, they are
                                         processed further in the same shift.
                                         If you specify the transition time in hours, you must specify a maximum time.
                                         The selection of the maximum time determines whether weekends are includ-
                                         ed in the planning.

                                            Each time specification means a change of the shift
                                            With the first minute, which you specify as transition time in hours, there is
                                            a change to the next shift.


                                               Wednesday            Thursday        Friday          Monday




                                                     A     B                         C          D
                                         A Transition time = 0                    C Transition time to the next day
                                         B Transition time to the next shift      D Transition time to the weekend
                                         Fig. E-50       Transitions in hours


                                         The shift times of the various machines can vary in their length; that is, the TG
                                         furnace can be specified with a shift time of 6 hours, the IG line, by contrast,
                                         has 8 hours.
                                         If you are working with such changeable shift ends, the time may not be spec-
                                         ified with more than 8 hours. To avoid this problem, you can simply specify 6
                                         hrs. (B).
                                         From Friday at 10PM to Monday at 2PM, you need a transition time of at least
                                         64 hours (D) for the optimal transition. Only with this transition time is it worth
                                         letting the glass stand over the weekend.
                                         From this example, you can see that the definition of transition times in shifts
                                         is much easier than the transition in hours.
4.50 / 01-2023




                 E-96                                                                A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                        Shift change - special case
                                        The grinding machine in the following example works in a single shift. Further-
                                        more, it works very slowly. If it is fitted in the morning, the lites can be trans-
                                        ferred to the subsequent machine at the shift end.
                                        The transition times are therefore defined with the following details:
                                        •   Normal = 0 shift
                                        •   Max. = 1 shift
                                        •   Rush = 1 shift
                                        •   Min. = 0 shift


                                                                           Monday               Tuesday


                                               Grinding
                                               special edges

                                               Tempered glass




                                        Fig. E-51    Shift change with regard to machine


                                        The transition time of 1 shift refers to the shifts of the grinding machine. From
                                        this, it follows that the transition to the next shift is always calculated for the
                                        following day regardless of the transition type.
                                        In this case, it is necessary to define the transition times for the grinding ma-
                                        chine in hours:
                                        •   Normal = 0 hrs.
                                        •   Max. = 8 hrs.
                                        •   Rush = 4 hrs.
                                        •   Min. = 4 hrs.


                                                                           Monday               Tuesday


                                               Grinding
                                               special edges

                                               Tempered glass




                                        Fig. E-52    Transition in hours


                                        As a result of these settings, the maximum transition leads to the end of the
4.50 / 01-2023




                                        subsequent shift on the subsequent machine. The times for the rush transition
                                        and the minimal transition lead to the middle of the following shift.




                 A+W Production Capacity Planning                                                                    E-97
                 Master Data of Capacity Planning                                                                      Tutorial




                                               Definition of Transition Times
                                               For the individual logical machines, you specify transition times of all types
                                               with the corresponding time specifications in shifts. In exceptional cases, you
                                               can also use times with the specification in hours, e.g. for drying times.
                                               In addition, there are a series of production-conditioned transition times that
                                               cannot be sped up, e.g. for heat soak or drying times after screen printing.
                                               For the case that a transition does not result in a change of machine and if no
                                               explicit transition between two logical machines has been defined, an auto-
                                               matic transition with a transition time of 0 will be used. This guarantees that
                                               unnecessary transitions between machines will be avoided even if no explicit
                                               transitions have been defined.
                                                “Definition of machine paths” on page E-17


                             A                      B                    C          D         E              F




                 A Station from which the lite comes                      D Normal transition times in hours
                 B Station to which the lite is going                     E Normal transition time in shifts
                 C Type of transition                                     F Maximum transition time in hours, shifts
                 Fig. E-53       Transition times


                                               Transition times are generally defined in shift (E); in exceptional cases they
                                               can also be specified in hours (D). Handling and set-up times must be consid-
                                               ered in the transition times.
4.50 / 01-2023




                 E-98                                                                     A+W Production Capacity Planning
                 Tutorial                                                                    Master Data of Capacity Planning




                                        •   Transition times in shifts are defined in whole shifts.
                                        •   Transition times in hours are defined in blocks of four or eight hours. This
                                            is adjusted to the shifts in your production and is clear. The transition times
                                            also include the non-working time, e.g. for the hardening of silicone sealing
                                            over the weekend.
                                        The transition times are processed hierarchically. Here, it applies that:
                                        •   Machine x -> Machine y describes the explicit transition between two ma-
                                            chines.
                                        •   Machine x -> All machines describes the transition at the end of machine x.
                                        •   All machines -> Machine x describes the transition at the entry to machine
                                            x.
                                        •   All machines -> All machines describes the general transition and is eval-
                                            uated last if no other transition time was found.

                                        Transition types
                                        In order to specify the transition times correctly, you must know the optimal
                                        throughput of your production. This means that you need to know exactly how
                                        long it takes until the next processing can be done. Starting from the normal
                                        (optimal) transition, you can then determine by how much time a transition can
                                        be shortened.
                                        The various types of transition times are used as follows:
                                        •   In the Normal type, the lites go through production in the regular, scheduled
                                            time. These times apply for the optimal production process, e.g. without ab-
                                            sences of personnel or machine breakdowns, breakage, etc.
                                        •   In the Rush type, the production of individual lites is sped up, e.g. by short-
                                            ening the dwell time. However, these transition times increase the costs.
                                        •   In the Minimal type, the so-called high-priority orders are pushed through
                                            production. Here, only the transition times are considered that are indis-
                                            pensable for production, e.g. dwell times in the LAMI autoclave, drying of
                                            adhesions. Minimal transition times are the most expensive transition
                                            times.
                                        •   With the Illegal type, a transition from or to a machine is locked, e.g. be-
                                            cause internal transport paths are required.

                                            Example

                                            With a grinding drilling line with the setting Illegal, you can specify that only
                                            such lites will reach the drilling station that were previously at the grinding
                                            station. For this, you would set up the following transitions:
                                            • Illegal: All machines – drilling station
                                            • Normal: Grinding station -> drilling station
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                               E-99
                 Master Data of Capacity Planning                                                                                                                Tutorial




                                         Preparation for defining transition times
                                         In order to determine the transition times for your production, you can create
                                         a matrix. The matrix helps to visualize the transition times between the logical
                                         machines.
                                         Distinguish the time between departure and the time for arrival:
                                         •   The departure after the work process can mean, e.g. that a lite is waiting to
                                             be repacked after a processing.
                                         •   The arrival at the start can refer to preliminary work.




                                                                  to




                                                                                                                            IG - Muntin
                                                                                            Heat Soak
                                                                       Arrissing




                                                                                                                                          IG Line
                                                                                   Bender




                                                                                                                 Drilling
                                                                                                        LAMI
                                              from
                                              Receipt of goods            4          4                   4        4           4            4

                                              Cutting                                                             4
                                                                                                                                                    Legend:
                                              Arrissing                   0          0                   0                                 0
                                                                                                                                                    • Number:
                                              Bender                                                                                       4
                                                                                                                                                      Transition time in
                                              Heat Soak                                                  8                                 8          hours
                                                                                                                  8                                 • Green:
                                              LAMI                                                                                         8
                                                                                                                                                      Transition time
                                              Drilling                                                                                     4          upon departure
                                                                                                                                           4        • Red:
                                              IG - Muntin
                                                                                                                                                      Transition time
                                              IG Line                                                                                      0          upon arrival



                                         Fig. E-54        Sample matrix for transition times


                                         In this example, you see, for example, that the glass in heat soak always
                                         dwells for eight hours. Therefore, the transition time from heat soak to all other
                                         workstations is always 16 hours. The times determined this way for your pro-
                                         duction must be converted into shifts.
                                         Such a matrix shows that you must only define a few transition times between
                                         the workstations. All others can be defined with the setting From all machines
                                         -> machine x or From machine x -> All other machines.
                                         We recommend creating the matrix and entering it in the dialog together with
                                         the A+W Software GmbH service team.
4.50 / 01-2023




                 E-100                                                                                         A+W Production Capacity Planning
                 Tutorial                                                                  Master Data of Capacity Planning




                                            Definition and Management of Transition Times
                                            This unit will show you how to define, edit, or delete transition times. Consider
                                            that set-up and handling times must also be considered in the transition times.
                                            For instructions on this subject, please see:
                                            •   “How to enter a transition time” on page E-101
                                            •   “How to edit a transition time” on page E-103
                                            •   “How to delete a transition time” on page E-103

                                                Prerequisite
                                                Before entering transition times you have to define the corresponding log-
                                                ical machines in machine allocation.


                                             How to enter a transition time
                                            1 Go to Master data > Capacity planning > Transition times.
                                            2 Click [New].


                      A        B                     C                       D         E                   F




                 A New line                                            D Type of transition time
                 B Machine from which the part is departing            E Normal transition time in hours or shifts
                 C Machine at which the part is arriving               F Maximum transition time in hours or shifts
4.50 / 01-2023




                 Fig. E-55    Setting up transition times


                                                A new line is added at the top of the list of machines.


                 A+W Production Capacity Planning                                                                     E-101
                 Master Data of Capacity Planning                                                                     Tutorial




                                         3 Double-click in the field (B) in order to open the dialog for selecting the ma-
                                           chine.




                                         4 Select the desired machine with a double-click.
                                         5 Repeat the step for the machine (C) for which you are specifying the tran-
                                           sition.
                                            Also use the options All machines to machine X and Machine X to all ma-
                                            chines.
                                         6 Select the type (D) for the transition time and enter the appropriate time (E).
                                            Use shifts if possible. In exceptional cases, you can also use time periods,
                                            e.g. drying times.
                                         7 Enter the maximum transition time (F).
                                            This way, you allow the system to extend the transition time. Here, you can
                                            also use hours or shifts.

                                            Tip
                                            For the transition to the last process, e.g. Packing or Dispatch, specify the
                                            longest transition time possible. This will give you greater flexibility in criti-
                                            cal situations.

                                         8 Repeat steps 2 and 7 for the next transition type (D) of the same machine
                                           combination.
                                         9 Click [OK] to save the data.
                                            You have thus created the transition times in the various transition types for
                                            a transition.
4.50 / 01-2023




                 E-102                                                                A+W Production Capacity Planning
                 Tutorial                                                                 Master Data of Capacity Planning




                                            How to edit a transition time
                                           1 Go to Master data > Capacity planning > Transition times.
                                           2 Correct the transition times for the desired machines.
                                               Activate the fields with a double-click.
                                           3 If necessary, add a machine combination by creating data for another tran-
                                             sition type.
                                               To do this, follow the description in the action sequence for creating transi-
                                               tion times.
                                           4 Click [OK] to save the changes.
                                               With that, you have changed the transition time.


                                            How to delete a transition time
                                           1 Go to Master data > Capacity planning > Transition times.
                                           2 In the first column, select the transition time to be deleted.
                                               The whole line for this transition time is highlighted.




                 Fig. E-56   Deleting transition times


                                           3 Click [Delete].
                                               The transition time is deleted from the list.
                                               In case you have deleted a transition time from the list by mistake: Click the
                                               [End] button.
                                               If you confirm the message with [No], the dialog closes without saving the
                                               changes. The transition time is displayed in the list again when you open
                                               the dialog.
4.50 / 01-2023




                                           4 Click [OK] to close the dialog.
                                               The changes will be taken over in the database.


                 A+W Production Capacity Planning                                                                     E-103
                 Master Data of Capacity Planning                                                                 Tutorial




                                         Exercises
                                         Create the data so that it is available in all subsequent exercises. If the data
                                         for the capacity planning is thus complete, you can test the planning for your
                                         own orders in the Production Monitor.
                                         •   Work with your trainer to create a new machine in the machine allocation
                                             completely, which you mark clearly as test machine for the capacity plan-
                                             ning.
                                         •   Define the transition times for this machine in the rush and common grid.
                                         •   Create transition times between two machines for all types of transition
                                             times that are required for the transitions.
                                         •   Change the transition times.
                                         •   Check the results in the production monitor by means of a test order.


                                         Additional information
                                          Software Reference, “Transition Times” on page E-217
4.50 / 01-2023




                 E-104                                                              A+W Production Capacity Planning
                 Tutorial                                                               Master Data of Capacity Planning




                                        Default Times
                                        Objectives

                                        •   What are default times?
                                        •   How are default times defined, edited, and deleted?
                                        •   Which elements do the default times consist of?
                                        •   How are elements included in default times?
                                        •   How does the formula test work?


                                        Benefits

                                        • You can use default times to define the duration of a work step on a machine for a
                                          lite. Together with the transition times, the times through the production stations
                                          are calculated this way.


                                        Note

                                        Default time = processing    Default times in define how long a certain work process
                                        time                         takes on a certain machine.
                                                                     The processing time is calculated using formulas.
                                                                     Default times are called processing times in machine
                                                                     allocation (MA).

                                        Logical machines             Default times are created for the logical machines.

                                        Default Times                The default times are used for capacity planning and
                                                                     cost calculation.

                                        Formula                      Default times can be calculated with formulas in order to
                                                                     consider various influencing variables, e.g. area, linear
                                                                     meters, quantity, thickness.
                                                                     Complex default times are entered as formulas in
                                                                     machine allocation.

                                        Element                      A line in a default time formula, e.g. a thickness
                                                                     dependency, the time for the production of a cut-out on a
                                                                     machining center or a time surcharge for heavy lites.
                                                                     Elements can be entered separately and tested. There
                                                                     are fixed elements, conditioned expressions, threshold
                                                                     values, weighted expressions (so-called free elements),
                                                                     and vectors. Tables and three-dimensional
                                                                     dependencies (so-called cubes) can also be processed
                                                                     as user-defined elements.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                        E-105
                 Master Data of Capacity Planning                                                                Tutorial




                                         Definition of the Default Times
                                         With a default time, you define how the duration of a work process is calculat-
                                         ed on a logical machine. The basis of the calculation is the respective area or
                                         edge length of the individual order item.




                                         Fig. E-57    Default Times


                                         This dialog lists the logical machines via which processings are controlled. De-
                                         fault ties are specified in A+W Production with default tie formulas. You define
                                         the default time formulas on the Formula for Default Time dialog.

                                            Default Times
                                            The default times are called processing times in machine allocation (MA).
                                            Since the default times are assigned to logical machines you can also enter
                                            formulas for default times in machinery allocation. This is done by means
                                            of the machine allocation editor, Logical machine tab in the Processing time
                                            field. These formulas from the A cannot be changed on the Default Times
                                            dialog.
4.50 / 01-2023




                 E-106                                                             A+W Production Capacity Planning
                 Tutorial                                                               Master Data of Capacity Planning




                                        Structure of Default Time Formulas
                                        Each default time formula is based on a basis time that is specified in seconds.
                                        Default time formulas can be defined with specified elements. In addition, you
                                        can also create your own elements and use them in the formula.

                                                      A                                            B          C        D




                                         E
                                        A Elements of the default time formula     D Sorting sequence of the elements
                                        B Basis time in seconds                    E Multiplier for the processing quantity
                                        C Selection of the calculation operation
                                        Fig. E-58     Default Time Formula


                                        With each line, a time surcharge is specified, which is either calculated as a
                                        formula or determined as value of a table.
                                        You can use several different elements (A) in a default time formula. For this,
                                        select the desired element, specify a value in seconds, and specify how the
                                        value should be used in the calculation operation (C). Important here is that
                                        the sequence (D) is sorted correctly. This is especially true if the next calcula-
                                        tion operation builds on the intermediate result of the previous operation.
                                        The basis time counts as start value. All other elements of the formula are
                                        therefore surcharges on the start value. If you do not enter a basis time, all cal-
                                        culations build on the result of the first entry (A).
                                        By default, various elements are offered for selection, to which you can add
                                        with your own definitions:
4.50 / 01-2023




                                         “Editor for Formula Elements” on page E-112




                 A+W Production Capacity Planning                                                                     E-107
                 Master Data of Capacity Planning                                                                           Tutorial




                                            Example gas and shape

                                            Basis time                          23 s
                                            Factor for size                     23 * size factor
                                            Factor for gas                      Intermediate result * gas factor
                                            Constants for shape                 Intermediate result + shape constant


                                         With this default formula, you can calculate times for lites with gas filling and
                                         for shapes. If, however, you want to calculate LAMI, the formula must be struc-
                                         tured as follows:

                                            Example LAMI, size and gas

                                            Basis time                          23 s
                                            Factor LAMI                         + LAMI factor
                                            Factor for size                     Intermediate result 1 * size factor
                                            Factor for gas                      Intermediate result 2 + (23 * gas factor)


                                         Fixed elements
                                         Fixed elements are not assigned a value; instead, it is only specified how the
                                         elements affect the default formula. For calculation, the actual values of the
                                         glass are used. Thus, for example, for the Fixed element 'thickness' with a lite
                                         that is 4.00 mm thick, the value 4 is determined. For the Fixed element 'quan-
                                         tity', the number of lites and for a Fixed element 'area' the area of the lites is
                                         determined.
                                         With the selection of the calculation operation, you specify on the Formula for
                                         Default Time dialog how the value determined is used in the default time for-
                                         mula.

                                         Factors
                                         With a factor, you can specify a time surcharge that is always calculated if the
                                         prerequisite for the use of the factor is fulfilled.

                                            Example

                                            With the Value for 'Size of lite' you specify a surcharge on the basic time that
                                            is always calculated for oversized lites. When a lite counts as oversized is
                                            specified for the factor.


                                         With the selection of the calculation operation, you specify on the Formula for
                                         Default Time dialog how the value determined is used in the default time for-
                                         mula.
4.50 / 01-2023




                 E-108                                                                  A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                        Vectors – tables and cubes
                                        Vectors permit an exact planning of default times based on the properties of
                                        the workpiece. Vectors can be used to take into account the default time, e.g.
                                        for the glass thickness, area to be processed, the edge structure, and the as-
                                        pect ratio of a lite.




                                        Fig. E-59    Vector ’Thickness -> factor’ – time surcharges depending on the lite
                                                     thickness


                                        Different lite thicknesses are e.g. allowed for by the vector ’Thickness  fac-
                                        tor’. This way, you specify time surcharges depending on the thickness of a li-
                                        te.
                                        If you specify the value in the Vector ’Thickness factor’ as table, you can
                                        scale the value of the vector, e.g. from 4.00 - 5.99 mm thickness, the value 0.1
                                        applies; for 6.00 - 7.99, the value 0.2 applies, etc.
                                        With the selection of the calculation operation, you specify on the Formula for
                                        Default Time dialog how vectors are used in the default time formula.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                    E-109
                 Master Data of Capacity Planning                                                                       Tutorial




                                         Input help for vectors
                                         Vectors are entered on the Factor/vector (name) dialog. This table contains
                                         one surcharge value per limit value (scale level). To create such a table, there
                                         are two procedures available:
                                         •   You specify the values individually in the table. Here, for example, you
                                             specify several levels of thicknesses, lengths or weights and assign each
                                             of these a value.
                                         •   You can have the scale levels and scaled values calculated.




                                         Fig. E-60     Input help for vectors - result


                                             For this calculation, you specify a start and end value, e.g. 4.00 - 20.00 mm
                                             for the thickness. If you specify 2.00 mm as step size, a step is inserted ev-
                                             ery 2.00 mm between the start and end values.
                                             If you specify 0.1 as start value for the surcharge and 0.1 as the step size,
                                             then the value 0.1 applies for the first step, and for all further levels, this val-
                                             ue is increased by 0.1.
                                             For the table, the result is: lites with a thickness of 4.00 - 5.99 mm have the
                                             value 0.1; from 6.00 - 8.00 mm, the value 0.2, etc.


                                         Calculation of Time Surcharges
                                         In the simplest case, a default time formula only consists of a basic time. You
                                         can e.g. define a basic time of 30 seconds for a logical machine. This means
                                         that any process on this logical machine will take 30 seconds.
                                         In practice, the duration of such a process depends on various factors howev-
                                         er, e.g. on the lite thickness and on the length of the edge to be processed.
                                         The thicker the lite and the longer the edge to be processed, the more time will
4.50 / 01-2023




                                         a process take.
                                         To consider these dependencies, you can specify time surcharges. There are
                                         fixed elements and/or vectors available in the default time formula.


                 E-110                                                                   A+W Production Capacity Planning
                 Tutorial                                                                    Master Data of Capacity Planning




                                        For the default time formula, you can select from the following elements:
                                        •   Basic time or start time.
                                        •   Time surcharge as fixed element, e.g. the glass thickness.
                                        •   Time surcharge as fixed value, e.g. for large lites.
                                        •   Time surcharge as vector, e.g. scaling by weight.
                                        •   Time surcharge as table for matrix, e.g. edge length.
                                        Basic time and time surcharges are specified in seconds.

                                        Sequence of the calculations
                                        For the calculation, you must consider the operator sequence of mathematics:
                                        multiplication and division are calculated before addition and subtraction un-
                                        less parentheses specify the sequence.

                                            Example

                                            1+2*4                     =9                      Multiplication first

                                            (1 + 2) * 4               = 12                    Brackets first

                                            1 + (2 * 4)               =9

                                            4 * (1 + 2)               = 12

                                            6 + (9 / 3)               =9

                                            (6 + 9) / 3               =5


                                        For calculation of the time surcharges, the following settings are available:

                                        Setting                Meaning

                                        + Table                The value from the table is added to the intermediate result.

                                        + b * value            The basic time is multiplied by the value. The result of the
                                                               multiplication is added to the intermediate result.

                                        + value                The value is added to the intermediate result.

                                        * (1 + value)          The value is added to 1 and the result multiplied by the
                                                               intermediate result from the previous line.

                                        * Vector               The result of the previous line is multiplied by the value of the
                                                               vector.

                                        Tab. E-1          Possible settings for the default time formula

                                        If the calculation begins with the determination from a formula, specify 0 as
                                        start value, e.g. the calculation of an area before the first screen printing is ap-
                                        plied.
                                        If the calculation is based on the result of the previous line, the sequence of
                                        entries is important.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                             E-111
                 Master Data of Capacity Planning                                                                  Tutorial




                                         Editor for Formula Elements
                                         For the definition of individual formula elements, there is an editor in which you
                                         can create your own formulas or select a pre-defined formula.



                                         A
                                         B                                                                    E

                                         C                                                                    C
                                                                                                              F
                                         D




                                         A Name of the formula element            D Calculation formula
                                         B Selection of the type                  E Input format
                                         C Labeling                               F Independent parameter
                                         Fig. E-61    Entering time formula elements


                                         You give the formula element a name (A), which is displayed in the selection
                                         of formula elements and a label (C) that is displayed on the Formula for Default
                                         Time dialog. The second label is displayed before the calculation value.
                                         You use the various element types (B) for the following calculations:
                                         •   Fixed element:
                                             Expressions without user input, e.g. long edge. This setting should no lon-
                                             ger be used for new definitions; it has been replaced by Free element.
                                         •   Condition:
                                             Expressions with a user input that is used if the condition is true.
                                         •   Free element:
                                             Expressions for which the result is weighted with the user input (e.g. sec-
                                             onds per meter ground).
4.50 / 01-2023




                 E-112                                                                 A+W Production Capacity Planning
                 Tutorial                                                             Master Data of Capacity Planning




                                        •   Threshold value:
                                            Expressions for which the threshold value for the condition can be set with-
                                            out changing the formula definition (e.g. quantity surcharge starting with
                                            user input)
                                        •   Vector:
                                            Expressions for which a table with value pairs of minimum values and co-
                                            efficients to be used is maintained.
                                        You can write the actual formula definition (D) of the element as a formula or
                                        select a pre-defined formula and adjust it. For vectors, you cannot change the
                                        definition, therefore, the field is grayed out.


                                        Example – Default Time for the Logical Machine
                                        Cutting
                                        You have determined the area dependency of your cut from production statis-
                                        tics. Furthermore, you 'know' that the arc shapes take 20 seconds longer on
                                        average and the table requires 10% more time for edge deletion of insulated
                                        glass components
                                        In order to be able to react quickly to production changes, you want to be able
                                        to set the complete default time formula to faster or slower with a control pa-
                                        rameter.




                                        Fig. E-62    Example – default time formula
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-113
                 Master Data of Capacity Planning                                                                        Tutorial




                                         Line                     Definition    Explanation

                                         Basic time               0.95          The control parameter is 95% of the default
                                                                                time, that is, it is set to faster.

                                         Edge stripping           * (1 + 0.1)   The surcharge is only calculated for a coated
                                                                                lite for IG.

                                         Area cut                 * Vector      The result is multiplied by the times for the
                                                                                sheet area.

                                         Arc shape                + 20          For a shape with round arcs, 20 seconds are
                                                                                added.

                                         Tab. E-2     Example – conditions of calculation

                                         The actual times are maintained in the vector for the cut area, e.g.:

                                          Area (qm)          Val.

                                          0.1                70          up to 0.99 sq m, 70 seconds are calculated

                                          0.5                45          for 0.1 - 0.499 sq m, 45 seconds are calculated

                                          1.0                60          for 0.5 - 0.999 sq m, 60 seconds are calculated

                                          2.0                150         for 1.5 - 1.999 sq m, 150 seconds are calculated

                                          3.0                210         for 1.999 - 2.999 sq m, 150 seconds are calculated


                                         In this example, you see that for very small and for large lites, more time is re-
                                         quired for cutting. Thus, there is another size surcharge for cutting. For area
                                         processings, such a surcharge may be necessary and must be defined on the
                                         appropriate logical machine.

                                         Condition: shape with arcs
                                         The condition should only supply the user input as result if it is true.

                                            Definition (example)

                                            IF (($Parts_MODELL_NR >= 60 AND $Parts_MODELL_NR <= 81) OR
                                            ($Parts_MODELL_NR >= 113 AND $Parts_MODELL_NR <= 118) OR
                                            ($Parts_MODELL_NR >= 123 AND $Parts_MODELL_NR <= 125) OR
                                            ($Parts_MODELL_NR >= 133 AND $Parts_MODELL_NR <= 199))
                                            THEN 20 END

                                            Length specification in the formula
                                            Note that the length values in a formula must be specified in µm.
4.50 / 01-2023




                 E-114                                                                  A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                          Condition: threshold value
                                          With more than 11 pieces, the default time should be 10% smaller.

                                               Definition (example)

                                               IF ($Parts_MENGE > 11) THEN - 0.1 END


                                          Condition: vector for shape cutting
                                          Vectors can depend on units or depict non-linear situations. If the simple sur-
                                          charge for shapes with arcs is not precise enough for you, define a vector, with
                                          help of which you can query the required coefficients easily and very precisely.
                                          On the dialog for entering a shape element, you can create a new element with
                                          the element type Vector. For a valid vector, select a formula for the indepen-
                                          dent parameter, e.g. AWF_ShapeNumber.




                                           A
                                                                      B



                 A Vector with independent parameters                 B Table for shape numbers
                 Fig. E-63   Vector for shape-dependent time surcharges


                                          The table permits the shape-dependent scaling of the surcharges. The entry
                                          for the left column always provides the start value of the validity range. It's
                                          good practice to define a value pair for 0 so that the value range is described
                                          completely.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-115
                 Master Data of Capacity Planning                                                                      Tutorial




                                         Time Formula Objects
                                         You can map the BOM or elements of the BOM as formula objects in order to
                                         depict the chain of processings. This display serves to test the dependencies
                                         of the processings in the default time formula, e.g. to check how the process-
                                         ing depends on what is done in the counter-lite. Formula objects are used for
                                         testing formulas with logical quantities.
                                         Formula objects always refer to a particular default time formula. They cannot
                                         be used across the boards. You can save the formula objects if you want to
                                         have proof that the formula is applied correctly.




                                                                                                                E




                                                                                                                D




                                                          A          B                    C
                                         A Save whole object                       D Delete selected object
                                         B Delete object                           E Objects
                                         C Add object
                                         Fig. E-64     BOM tree from the point of view of the individual processings


                                         In this example, you see the processing BOM of an IG lite. When adding, the
                                         formula objects (E) are numbered. With a double-click, you can open each for-
                                         mula object and rename it, e.g. the first object to IG. This makes sense to clar-
                                         ify the structure. When adding (C), a new object is created below the selected
                                         object. When deleting (D), the selected object and all sublevels are deleted.

                                            Loading a saved object for testing
                                            A saved formula object can only be used for the formula for which it was
                                            created, e.g. to test changes in the default time formula. Therefore, it
                                            makes sense to give meaningful names when saving.

                                         There is an example of a formula object under the test of the default time for-
                                         mula.
4.50 / 01-2023




                                          “Here's how to test the calculation of the time formula” on page E-125




                 E-116                                                                A+W Production Capacity Planning
                 Tutorial                                                             Master Data of Capacity Planning




                                        Definition and Management of Default Time Formu-
                                        las
                                        This unit will tell you how to define, edit, or delete default time formulas.
                                        In the first line on the Formula for Default Time dialog, you can define formula
                                        elements as templates for all machines. If for the machine 0 you define a time
                                        formula, this is saved in the database, however the formula is not used since
                                        the machine 0 is not assigned a processing in the MA.

                                            Prerequisite
                                            Default time formulas are defined for the logical machines that execute a
                                            particular work process. Therefore, the appropriate logical machines must
                                            be defined in the machine allocation.

                                        For instructions on this subject, please see:
                                        •   “Here's how to define a default time formula” on page E-118
                                        •   “Here's how to create a vector with the input help” on page E-121
                                        •   “Here's how to delete a default time formula” on page E-123

                                            Complexity of default time formulas
                                            A+W Production allows defining default time formulas of any complexity re-
                                            quired. This permits the handling of all sorts of special cases. Keep default
                                            time formulas as simple as possible. If in your production it is necessary to
                                            use complex default time formulas, please contact theA+W Software
                                            GmbH customer service.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-117
                 Master Data of Capacity Planning                                                               Tutorial




                                          Here's how to define a default time formula
                                         1 Go to Master data > Capacity planning > Default times.




                                         Fig. E-65    Default Times


                                         2 Select the logical machine for which you want to define a default time for-
                                           mula.
                                         3 Click [Edit].
                                            The Formula for Default time dialog opens.
                                            A warning will be issued if a formula for the processing time has already
                                            been entered for this logical machine in machine allocation. If you proceed,
                                            the formula entered in machine allocation will be overwritten.
4.50 / 01-2023




                 E-118                                                             A+W Production Capacity Planning
                 Tutorial                                                                  Master Data of Capacity Planning




                                                                                                    A




                                         B                 C                       D                                 E
                                        A Basic Time                                   D Add a formula element
                                        B Multiplier for the processing quantity       E Add a pre-defined formula
                                        C Current logical machine
                                        Fig. E-66     Default Time Formula


                                        4 Enter the basic time (A) in seconds.
                                             You can either add a predefined formula (E) and save the data or build a
                                             formula with formula elements. The following steps will demonstrate the
                                             building with formula elements.
                                        5 Click [New] (D) to select an element.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                        E-119
                 Master Data of Capacity Planning                                                                 Tutorial




                                         6 Select the element, e.g. a vector, and take over the selection with [OK].
                                            The selected element now appears on the list in the Formula for Default
                                            time dialog.

                                                                                                 A        B




                                         A Specify values                        B Specify calculation
                                         Fig. E-67    Default time formula with new element
4.50 / 01-2023




                                         7 Click [...] (A) in order to open the dialog for entering the values.




                 E-120                                                              A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                           If you are creating a vector, you can specify limit values and the time values
                                           manually or using the input help.
                                            “Here's how to create a vector with the input help” on page E-121
                                        8 Select the operator (B) for the calculation.
                                        9 Repeat the steps 5 - 8 to add additional elements.
                                        10 Check the sequence of the formula elements.
                                           The sequence is important for the calculation if the surcharge refers to the
                                           intermediate total of the previous element.
                                        11 Click [OK] to apply the data.
                                           The dialog closes. Thus, you have compiled a default time formula. You
                                           can check the calculation and start a calculation with sample values with a
                                           formula object.
                                            “Testing Time Formulas” on page E-124
                                            “Time Formula Objects” on page E-116


                                         Here's how to create a vector with the input help
                                        1 Go to Master data > Capacity planning > Default times > Default time for-
                                          mula.
                                        2 Enter the basic time in seconds.
                                        3 Click [New] and select an element, e.g. Vector 'thickness -> factor'.




                                           Tab. E-3     Vector 'thickness -> factor'


                                        4 Click [Input help].
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                 E-121
                 Master Data of Capacity Planning                                                                 Tutorial




                                            A



                                            B




                                            A Limit values for the scaling         B Values for the time surcharge
                                            Tab. E-4      Input help for vectors


                                            First the limit values for the scaling (A) and then the values for the factor
                                            (B) are entered. The table is created using these inputs.
                                         5 Enter the start and end values, e.g. 4.00 and 20.00.
                                            These values specify the smallest and largest thickness.
                                         6 Enter the step size, e.g. 2.00.
                                            This value specifies at what steps the limit values for the scaling are calcu-
                                            lated between the start and end values.
                                         7 Enter the start value and the step size for the factor, e.g. 0.1.
                                            This value specifies by what size the factor is increased per limit value.
                                            Thus, you have entered all necessary values.
                                         8 Click [OK] to start the calculation of the table.
                                            The Input help for vectors dialog closes. The tables are calculated and tak-
                                            en over on the Vector -> thickness dialog.
                                            You can correct and complete the data.
4.50 / 01-2023




                 E-122                                                              A+W Production Capacity Planning
                 Tutorial                                                           Master Data of Capacity Planning




                                        9 Click [OK] to save the data.
                                           The Vector thickness -> factor dialog closes. The scaling created is taken
                                           over in the default time formula.


                                         Here's how to delete a default time formula
                                        1 Go to Master data > Capacity planning > Default times > Default time for-
                                          mula.
                                        2 Select the element that you want to delete.
                                        3 Click [Delete].
                                        4 Repeat the steps 2 and 3 until all elements that are no longer needed have
                                          been removed from the list.
                                        5 Set the basic time to zero.
                                        6 Click [OK] to save the data.
                                           The dialog closes.
                                           To delete a default time formula completely, select the default time on the
                                           Default times dialog and click [Delete].
4.50 / 01-2023




                 A+W Production Capacity Planning                                                              E-123
                 Master Data of Capacity Planning                                                                  Tutorial




                                         Testing Time Formulas
                                         On the Time formula test dialog, you can test formulas and check the values
                                         and calculation settings. You can either test the formula you are currently ed-
                                         iting on the Formula for Default time dialog or load a saved formula into the
                                         dialog in order to test it.
                                         The formula test outputs a result that specifies the time for the work process
                                         in question in seconds.
                                         For instructions on this subject, please see:
                                         •   “Here's how to test the time formula” on page E-124
                                         •   “Here's how to test the calculation of the time formula” on page E-125
                                         •   “Here's how to create a copy of the time formula syntax” on page E-129
                                         In addition, you can define formula objects that you can use to test all formulas.
                                         You specify the specific case there in which you want to test the formula, e.g.
                                         the thickness and width of a lite. Thus, you always have the same defaults for
                                         the test. This function is described in a separate unit.
                                          “Time Formula Objects” on page E-116


                                          Here's how to test the time formula
                                         1 Go to Master data > Capacity planning > Default times > Default time for-
                                           mula.




                                         Fig. E-68    Default Time Formula
4.50 / 01-2023




                                         2 Select the formula element that you want to test:




                 E-124                                                               A+W Production Capacity Planning
                 Tutorial                                                             Master Data of Capacity Planning




                                           If you want to test the entire default time formula, you must select the Basic
                                           Time element. However, you can also test each element individually by se-
                                           lecting it and performing the following steps.
                                        3 Click [Formula test].




                                                                           A                 B
                                           A Test result                           B Start evaluation
                                           Fig. E-69       Time formula test


                                        4 Click [Evaluate] (B).
                                           The calculation result (A) is displayed. If necessary, you can edit and cor-
                                           rect the formula.
                                        5 Click [OK] to save the data.
                                           To test the formula with lite data, you can create a formula object for the test
                                           and enter values.


                                         Here's how to test the calculation of the time formula
                                        1 Go to Master data > Capacity planning > Default times > Default time for-
                                          mula.
                                           Dialog Default time formula appears.
                                        2 Click [Formula test].
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                   E-125
                 Master Data of Capacity Planning                                                                 Tutorial




                                                                                                              A




                                                                                                              B




                                            A Select object                         B Add object
                                            Fig. E-70    Time formula object


                                         3 Double-click on the formula object (A) to open the dialog for entering the
                                           properties.

                                                              A                                    B
4.50 / 01-2023




                                            A Freely selectable name                B Selection of the type
                                            Fig. E-71    Properties of the formula object



                 E-126                                                               A+W Production Capacity Planning
                 Tutorial                                                              Master Data of Capacity Planning




                                        4 Enter a name (A) and select the type (B), e.g. element.
                                        5 Click [Add].
                                           The fields in the Properties column are pre-populated with the elements
                                           that are included in the current default time formula.




                                           Fig. E-72     Entering values for formula objects


                                        6 Enter the appropriate values for each property, e.g. the dimensions for
                                          height and width.
                                           Note that you must specify the dimensions in micrometers μm.
                                        7 Click [Close] to save the data and close the dialog.
                                           The Formula test dialog is displayed in the foreground.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                               E-127
                 Master Data of Capacity Planning                                                                  Tutorial




                                            Fig. E-73    Calculation with time formula objects


                                         8 Select the formula object for which the calculation should be started.
                                         9 Click [Formula test].
                                            The result of the calculation with the values input is displayed. If the calcu-
                                            lation does not do what you want it to, you can check the calculated values.
4.50 / 01-2023




                 E-128                                                               A+W Production Capacity Planning
                 Tutorial                                                          Master Data of Capacity Planning




                                         Here's how to create a copy of the time formula syntax
                                        1 Test the time formulas as specified in the previous action sequence.




                                           A



                                           A Display formula
                                           Fig. E-74   Time formula test


                                        2 Check the Display formula checkbox (A).




                                           Fig. E-75   Formula syntax


                                           On this dialog, you can check the syntax of the whole formula. To correct
4.50 / 01-2023




                                           the syntax with the help of A+W service, copy the syntax and send the text
                                           to A+W.




                 A+W Production Capacity Planning                                                             E-129
                 Master Data of Capacity Planning                                                               Tutorial




                                         Exercises
                                         •   Select a logical machine from your test machines and plan the default
                                             times for this logical machine on paper:
                                             – Which lites are going to be processed on this logical machine?
                                             – Which factors are necessary to define the default times for these lites?
                                             – How shall these factors be included in the default time formula?
                                         •   Create the default time formula based on the necessary elements.
                                         •   For the entry 0 - all machines, enter various formula elements, e.g. a spe-
                                             cific vector, a table, a threshold value.
                                         •   Create a formula object for a formula and test the default time formula in
                                             order to check whether the result meets your expectations.


                                         Additional information
                                          Software Reference, “Default Times” on page E-197
                                          Software Reference, “Default Time Formula” on page E-199
                                          Software Reference, “Tabelle, Vector (Name)” on page E-204
                                          Software Reference, “Input Help for Vectors” on page E-205
                                          Software Reference, “Entering a Formula Element” on page E-208
4.50 / 01-2023




                 E-130                                                             A+W Production Capacity Planning
                 Tutorial                                                             Master Data of Capacity Planning




                                        Machinery Groups
                                        Objectives

                                        • What are machinery groups in capacity planning?
                                        • How are machine groups defined, edited, and deleted?


                                        Benefits

                                        • Machine groups are used for combining the machines of an area and for
                                          controlling the capacity of the group by means of the number of employees.


                                        Note

                                        Machinery groups           Machinery groups combine the machines in certain
                                                                   areas, e.g. cutting or edgework.

                                        Persons                    Assign a number of persons to a machinery group and
                                                                   thus define the capacity of the corresponding machinery
                                                                   group.

                                        Shifts                     The shifts of the machines belonging to the same
                                                                   machinery group have to match.

                                        Bottleneck machine         A bottleneck machine cannot be booked beyond its
                                                                   capacity.
                                                                   Machines become a bottleneck machine when they are
                                                                   allocated to a machinery group.

                                           Prerequisite
                                           The shifts of the machines belonging to the same machinery group have to
                                           match. This includes the start and end time of the shifts.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                     E-131
                 Master Data of Capacity Planning                                                                   Tutorial




                                         Definition of the Machinery Groups
                                         You can combine machines into groups. Machinery groups make sense for
                                         machines in the same area. Thus, e.g. you could create a machine group Cut-
                                         ting to which you assign all machines in cutting. A specified capacity then ap-
                                         plies for the entire machinery group, that is, for cutting.
                                         You can only combine machines into a group whose shifts match; that is, that
                                         are available for the same time. Machines that you add to a machinery group
                                         automatically become bottleneck machines.




                                         A                                                                                C




                                         B
                                                                                                                          D




                                         A Machinery Group                        C Number of people in the group
                                         B Available machines                     D Allocated machines
                                         Fig. E-76     Machinery groups


                                         You must assign each of the machinery groups a number of people (C). A+W
                                         Production basically assumes that one person is working on each machine. If
                                         you reduce the number of employees in the group, the available time per ma-
                                         chine decreases.

                                             Example

                                             In the Cutting machinery group with four machines, there are four people
                                             assumed. If the 4 employees work 40 hours per week, 4 x 40 = 160 working
                                             hours per week available.
                                             With 3 employees, only 3 x 40 working hours = 120 hours per week are
                                             available.
4.50 / 01-2023




                 E-132                                                               A+W Production Capacity Planning
                 Tutorial                                                            Master Data of Capacity Planning




                                        Definition and Management of Machinery Groups
                                        This unit will tell you how to define, edit, or delete machinery groups.
                                        For instructions on this subject, please see:
                                        •   “Here's how to create a machinery group” on page E-133
                                        •   “Here's how to edit a machinery group” on page E-135
                                        •   “Here's how to delete a machinery group” on page E-135


                                         Here's how to create a machinery group
                                        1 Go to Master data > Capacity planning > Machinery groups.




                                        Fig. E-77    Machinery groups


                                        2 Click [New].




                                        3 Enter a name for the machinery group, e.g. Cutting.
                                        4 Click [OK].
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-133
                 Master Data of Capacity Planning                                                              Tutorial




                                            The Machinery groups field shows the new machinery group.
                                         5 Select the new machinery group.
                                            The list Machines for group shows all available machines.




                                         6 Select the machine that you want to add to the group, e.g. 180 Cutting table
                                           8.
                                         7 Click the arrow to the right and confirm the message
                                            The machine was added to the group.
                                         8 Repeat the steps 5 to 7 to add more machines.




                                         9 Go to field Machinery groups and double-Click column Persons.
4.50 / 01-2023




                                         10 Enter the number of persons working in this machinery group.

                 E-134                                                            A+W Production Capacity Planning
                 Tutorial                                                           Master Data of Capacity Planning




                                        11 Click [OK] to save the data.
                                           The dialog closes. That done, you have defined the machinery group.


                                         Here's how to edit a machinery group
                                        1 Go to Master data > Capacity planning > Machinery groups.




                                           Fig. E-78    Selected machinery group


                                        2 Go to the Machinery groups field and select the machinery group to be ed-
                                          ited.
                                           The right side of the list Machines for group lists all machines that have
                                           been added to the group. The left side lists the available machines.
                                        3 Select a machine to be removed from or added to the group.
                                        4 Click the [Arrow left] or [Arrow right] button to remove a machine from the
                                          group or add a machine to the group.
                                        5 Repeat the steps 3 to 4 to remove more machines from the group or add
                                          more machines to the group.
                                        6 In the Machinery groups field, correct the number of people.
                                        7 Click [OK] to save the data.
                                           The changes are saved and the dialog closed.


                                         Here's how to delete a machinery group
4.50 / 01-2023




                                        1 Go to Master data > Capacity planning > Machinery groups.
                                        2 In the Machinery groups field, select the machinery group to be deleted.



                 A+W Production Capacity Planning                                                               E-135
                 Master Data of Capacity Planning                                                                 Tutorial




                                         3 Click [Delete].
                                             The machinery group is removed from the list. This way, you change the
                                             available capacity for scheduling.
                                         4 Click [OK] to save the data.
                                             The changes are saved and the dialog closed.


                                         Exercises
                                         Create the data so that it is available in all subsequent exercises. If the data
                                         for the capacity planning is thus complete, you can test the planning for your
                                         own orders in the Production Monitor.
                                         •   Decide which machines you want to be arranged in a group.
                                         •   Create at least one machinery group on the Machinery groups dialog.
                                         •   Edit your machinery group.
                                         •   Delete one of your machinery groups.


                                         Additional information
                                          Software Reference, “Machinery Groups” on page E-234
4.50 / 01-2023




                 E-136                                                              A+W Production Capacity Planning
                 Tutorial                                                                Master Data of Capacity Planning




                                        Load Distribution
                                        Objectives

                                        • What does load distribution mean in connection with capacity planning?
                                        • How can the load distribution be defined, edited, or deleted?


                                        Benefits

                                        • Load distribution makes sense for machines with a special qualification. If this
                                          qualification is not called for, the machine is used for standard processing.


                                        Note

                                        Physical machine             Load distribution can only be defined for machines that
                                                                     have been specified as bottleneck machines.
                                                                     For example, you can keep 30% free for shapes on the
                                                                     machine that may be used for rectangles if no shapes
                                                                     are scheduled.

                                        Logical machines             The load distribution is made among the logical
                                                                     machines that have been defined for a physical machine.
                                                                     This way, you can break down the load distribution of a
                                                                     CNC center as percentages with the three logical
                                                                     machines Special edges, Cut-outs, and Drillings.

                                        Bottleneck machine           A bottleneck machine cannot be booked beyond its
                                                                     capacity.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                      E-137
                 Master Data of Capacity Planning                                                                       Tutorial




                                         Definition of Load Distribution
                                         The load distribution is specified among the logical machines that have been
                                         defined for a physical machine. This way, you specify the percentage share of
                                         the logical machines of the total capacity of the physical machine.
                                         You use load distribution to guarantee that a machine holds free a guaranteed
                                         minimum capacity for special tasks, e.g. for shape cutting. If the capacity held
                                         free is not used for shapes, rectangles can also be processed. This load dis-
                                         tribution is only possible and makes sense for machines that are defined as
                                         bottleneck machines.




                                         A
                                         B

                                         C                                                                                    D




                                         A Physical machine                          C Logical machines
                                         B Enable processing                         D Share of total capacity
                                         Fig. E-79     Load distribution


                                         You break down the capacity of a machine by allocating percentage shares (D)
                                         to the associated logical machines (C).

                                             Example

                                             A machine can process shapes, that is, rectangles and shapes. So that this
                                             special qualification is not occupied by the simpler rectangles, keep 30% free
                                             for shapes, for example. This load distribution is considered during
                                             scheduling.
                                             If this 30% is not needed for shapes, rectangles can also be processed.
4.50 / 01-2023




                 E-138                                                                  A+W Production Capacity Planning
                 Tutorial                                                                Master Data of Capacity Planning




                                        Definition and Editing of Load Distribution
                                        This unit will show you how to define, edit, and delete load distributions.
                                        For instructions on this subject, please see:
                                        •   “Here's how to set up load distribution” on page E-139
                                        •   “Here's how to edit load distribution” on page E-141
                                        •   “How to delete load distribution” on page E-142

                                            Prerequisite
                                            Load distribution can only be defined for machines that have been speci-
                                            fied as bottleneck machines.


                                         Here's how to set up load distribution
                                        1 Go to Master data > Capacity planning > Load distribution.




                                            A
                                            B




                                            A Machine                                 B Release fields
                                            Fig. E-80    Defining load distribution


                                        2 Select the machine (A) whose capacity you want to break down.
                                            The selection list includes only the machines that are defined as bottleneck
                                            machines.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                 E-139
                 Master Data of Capacity Planning                                                                 Tutorial




                                            Fig. E-81    Logical machines


                                            The corresponding logical machines are listed.
                                         3 Check the Enable check checkbox (B to enable the fields.
                                            The fields for the logical machines are enabled. If there is no load distribu-
                                            tion specified, Unlimited will appear in the right column.
                                         4 Double-Click the right column.




                                         5 Enter the percentage for the capacity.
                                         6 Repeat steps 4 and 5 in order to set up the percentage of total capacity of
                                           the physical machine for all logical machines.
                                         7 Uncheck the Enable check checkbox to prevent inadvertent changes.
                                         8 Click [OK] button to save the data and close the Load distribution dialog.
                                            The data is saved and the dialog closed.
4.50 / 01-2023




                 E-140                                                              A+W Production Capacity Planning
                 Tutorial                                                               Master Data of Capacity Planning




                                         Here's how to edit load distribution
                                        1 Go to Master data > Capacity planning > Load distribution.




                                           A
                                           B




                                           A Machine                                 B Enable fields
                                           Fig. E-82    Defining load distribution


                                        2 Select the machine (A whose load distribution you want to edit.
                                           The selection list includes only the machines that are defined as bottleneck
                                           machines.
                                        3 If necessary, check the Enable check checkbox ()B.
4.50 / 01-2023




                                           Fig. E-83    Load distribution of the selected machine




                 A+W Production Capacity Planning                                                                E-141
                 Master Data of Capacity Planning                                                                 Tutorial




                                         4 For all logical machines, change the percentage value for the capacity.
                                         5 If necessary, uncheck the Enable check checkbox.
                                         6 Click [OK] to save the data.
                                             The changes are saved and the dialog closed.


                                          How to delete load distribution
                                         1 Go to Master data > Capacity planning > Load distribution.
                                         2 Go to field Physical machine and select the machine the load distribution
                                           of which you want to delete.
                                             The corresponding logical machines are listed.
                                         3 Check the Enable check checkbox.
                                             The fields will be enabled.
                                         4 For all logical machines, change the percentage value for the capacity to
                                           000%.
                                             Unlimited is displayed in the fields.
                                         5 If necessary, uncheck the Enable check checkbox.
                                         6 Click [OK] to save the data.
                                             The changes are saved and the dialog closed. You have deleted the load
                                             distribution for this machine.


                                         Exercises
                                         Create the data so that it is available in all subsequent exercises. If the data
                                         for the capacity planning is thus complete, you can test the planning for your
                                         own orders in the Production Monitor.
                                         •   Check for which machines a load distribution makes sense.
                                             If necessary, create logical machines for your test machines beforehand.
                                         •   Set up at least one load distribution.
                                         •   Edit the load distribution.
                                         •   Delete the load distribution.


                                         Additional information
                                          Software Reference, “Load Distribution” on page E-235
4.50 / 01-2023




                 E-142                                                               A+W Production Capacity Planning
Capacity Planning                  E

                    Software Reference




                A+W Production
                 Software Reference                                                                            Overview




                                        Overview
                                        The Production Monitor dialog is available for planning and organizing the ca-
                                        pacities of your production. It displays the work shifts per machine.
                                        The orders are scheduled item by item, whereby the scheduling per item must
                                        be successful. If an order item cannot be scheduled successfully, the whole
                                        order is not scheduled.
                                        So that the calculation in the Production Monitor are done correctly, the capac-
                                        ity planning master data must be set up. The description of the dialogs is
                                        grouped in topics. It does not follow the arrangement of the dialogs in the soft-
                                        ware reference.
                                        The software reference provides information on the following subjects:
                                        •   “Scheduling” on page E-146
                                        •   “Campaigns and Reservations” on page E-182
                                        •   “Processings” on page E-192
                                        •   “Time Master Data” on page E-196
                                        •   “Master Data for the Shifts” on page E-220
                                        •   “Machines and Costs” on page E-231
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-145
                 Scheduling                                                             Software Reference




                              Scheduling
                              The Production Monitor is the central capacity and order control desk and en-
                              try point for work preparation, e.g. batch formation, rescheduling.
                              This section provides information on the following subjects:
                              •   “Production Monitor” on page E-147
                              •   “Displayed Machines” on page E-151
                              •   “Settings” on page E-152
                              •   “Please Select an Order/Batch” on page E-155
                              •   “Create New Filter” on page E-158
                              •   “Machine (Name)” on page E-159
                              •   “Adjust Shifts for Machine” on page E-160
                              •   “Shift Properties” on page E-161
                              •   “Reservation Display” on page E-162
                              •   “Workplan from Production Monitor” on page E-163
                              •   “Scheduling” on page E-166
                              •   “BOM Configuration” on page E-167
                              •   “Action” on page E-168
                              •   “Rescheduling” on page E-169
                              •   “Machine Reallocation” on page E-173
                              •   “Post-Processing Booking” on page E-174
                              •   “Defective Orders” on page E-177
                              •   “Asynchronous Processing” on page E-178
                              •   “Changes to Scheduled Orders” on page E-179
                              •   “Split Items” on page E-180
4.50 / 01-2023




                 E-146                                                 A+W Production Capacity Planning
                 Software Reference                                                                                 Scheduling




                                           Production Monitor
                                           Display > Production Monitor
                                           Details View > Context Menu > Production Monitor




                 Fig. E-84    Production Monitor


                                           This dialog displays the current state of production and the use of machine ca-
                                           pacity per work shift. This makes the Production Monitor the capacity and or-
                                           der control desk and the entry point for work preparation, e.g. batch formation,
                                           rescheduling.
                                            Tutorial, “Production Monitor” on page E-21

                                           Buttons

                 Icon        Function                                  Description

                             Selected machines                          “Displayed Machines” on page E-151


                             Settings                                   “Settings” on page E-152


                             Change display type for all machines      Selection of the display for all machines:
                                                                       •   Time
4.50 / 01-2023




                                                                       •   Quantity
                                                                       •   Area
                                                                       •   Weight



                 A+W Production Capacity Planning                                                                       E-147
                 Scheduling                                                                                   Software Reference




                 Icon         Function                                     Description

                              Change display (shift, day, week)            Changes the display. The machine capacity is shown
                                                                           per shift, per day, or per week

                              Change view                                  Changes the view.
                                                                           • Main view:
                                                                             All shifts in the specified time period are displayed.
                                                                           • Detail view:
                                                                             Only the shifts for the day specified are displayed.

                              Zoom in, zoom out                            Enlarges or reduces the display of the steps.


                              Refresh view                                 Refreshes the view.


                              Given number of days back, forward           Shifts the time period displayed back or forward by the
                                                                           number of days that is specified in the Days field.

                              Filter view, remove filter                    “Please Select an Order/Batch” on page E-155



                                              Start date Opens the calendar to select the start day for the display of work
                                              shifts.

                                              Days Specification of by how many days the display with the buttons should
                                              be scrolled forward or back.

                                              Filter input field Specification of the filter criterion, to filter the display by or-
                                              ders or batches.

                                                  Display
                                                  The display can be adapted individually. This affects the colors, a time grid,
                                                  status information, etc.

                                                   “Settings” on page E-152

                                              Work shifts
                                              The Production Monitor displays the work shifts for all selected machines. Ma-
                                              chines that are defined as bottleneck machines are displayed in red. A bottle-
                                              neck machine cannot be booked beyond its capacity.
4.50 / 01-2023




                 E-148                                                                     A+W Production Capacity Planning
                 Software Reference                                                                           Scheduling




                                        The following information is available via the context menu:
                                        •   Properties:
                                            Opens a dialog on which you can change the machine properties.
                                             “Machine (Name)” on page E-159
                                        •   Shift properties:
                                            Opens a dialog on which you can adjust shift times of the machine.
                                             “Adjust Shifts for Machine” on page E-160
                                        •   Display logical machines:
                                            With this entry the display of the logical machines can be activated and de-
                                            activated. Until now you had to change the corresponding switch in the
                                            master data dialog. When using the context menu, the value stored in the
                                            master data is not changed, only the display is adapted, so that the change
                                            is only temporary.
                                             “Misc” on page E-160

                                        Status of the planning
                                        The colored dots indicate the backlogs:
                                        •   Green: No backlog.
                                        •   Yellow: Backlog that can be made up on the same day by using the free
                                            capacities.
                                        •   Red: Backlog that cannot be made up for on the same day.

                                        Display of the work shifts
                                        Brief information about the status is displayed in the tooltip for a work shift.
                                        The following information is available via the context menu:
                                        •   Work plan:
                                            Opens the Work plan: Selection from A+W Production Monitor dialog with
                                            the overview of the batches and orders of the machine and shift.
                                             “Workplan from Production Monitor” on page E-163
                                        •   Delete:
                                            Deletes a selected work shift from the Production Monitor.
                                        •   Shift properties:
                                            Opens the Shift properties dialog where you can change the properties of
                                            a shift.
                                             “Shift Properties” on page E-161
                                        •   Display reservations:
                                            Opens the Display reservation dialog in order to check the reservations for
                                            a shift.
                                             “Reservation Display” on page E-162

                                        Hatched The duration of the work shift is reduced.

                                        X The work shift is deactivated.
4.50 / 01-2023




                                        ! The shift was set to Active for rush orders and is therefore only available for
                                        rush orders.

                                        ? Undefined processings are scheduled in the work shift.


                 A+W Production Capacity Planning                                                                  E-149
                 Scheduling                                                         Software Reference




                              Frame The shift is defined as a bottleneck.
                               “Shift Properties” on page E-161
4.50 / 01-2023




                 E-150                                                A+W Production Capacity Planning
                 Software Reference                                                                         Scheduling




                                        Displayed Machines
                                        Display > Production Monitor > [Selected machines].




                                        Fig. E-85    Displayed machines


                                        On this dialog, you select the machines that will be displayed on the Produc-
                                        tion Monitor dialog. Here, you can also specify the order. Machines that are de-
                                        fined as bottleneck machines will be displayed in red in the list. A bottleneck
                                        machine cannot be booked beyond its capacity.

                                        Checkbox Specification of whether a machine is displayed on the Production
                                        Monitor dialog.
                                         The machine is not displayed.
                                         The machine is displayed.

                                        [Arrow up], [Arrow down] Shifts the selected machine by one place up or
                                        down.

                                        [OK] Saves and applies the selection and closes the dialog.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-151
                 Scheduling                                                              Software Reference




                              Settings
                              Display > Production Monitor > [Settings].




                              Fig. E-86    Settings - fields displayed by category


                              On this dialog, you can set the display on the Production Monitor dialog, e.g.
                              whether machine groups and backlogs are displayed. Furthermore, you can
                              specify the display of the colors for work shifts, bottlenecks or overloads.

                              [Categories] Sorts the elements by categories.

                              [Alphabetically] Sorts the elements alphabetically.

                              [Properties] Not currently used.

                              Other settings
                              •   Number of Days before the Start Date:
                                  Specification how many days before the current start are displayed.
                              •   Treatment of Machine Groups:
                                  Specification whether machine groups are displayed.
                              •   Treatment of Backlogs:
4.50 / 01-2023




                                  Specification whether backlogs are displayed.




                 E-152                                                     A+W Production Capacity Planning
                 Software Reference                                                                         Scheduling




                                        Display
                                        •   Processed:
                                            Color in which processed orders are displayed.
                                        •   Update Time:
                                            Specification of the interval in seconds at which the display on the Produc-
                                            tion Monitor dialog is updated.
                                        •   Selected Shifts:
                                            Color in which the selected work shift is displayed.
                                        •   Display Capacity Graphically:
                                            Specification whether the capacity is displayed as text.
                                        •   Automated Updates:
                                            Specification whether the display is updated automatically.
                                        •   Scheduled:
                                            Color in which the scheduled orders are displayed.
                                        •   Bottleneck:
                                            Color in which bottlenecks are displayed.
                                        •   Bottleneck Color:
                                            Font color for bottleneck machines.
                                        •   Color of Indication Icons:
                                            Color in which the indication icons are displayed.
                                        •   Free Reservation Time:
                                            Color in which the unbooked reservations are displayed.
                                        •   Intensity of 3D Effects:
                                            Selection of the intensity with which the 3D effects are displayed.
                                        •   Shift:
                                            Color in which the work shifts are displayed.
                                        •   Display Hours:
                                            Specification whether an hour grid is placed behind the shifts.
                                        •   Overload:
                                            Color in which an overload is displayed.
                                        •   Scheduled:
                                            Color in which scheduled work shifts are displayed.
                                        •   Scheduled Work Processes:
                                            Color in which scheduled work processes are displayed.
                                        •   Display Time :
                                            Specification of whether a time grid is displayed.
                                        •   Time Color:
                                            Color in which the time is displayed.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-153
                 Scheduling                                                              Software Reference




                              Detailed display
                              •   Work processes with finished primary products:
                                  Specification whether work processes with finished primary products are
                                  displayed.
                              •   Intensity of 3D Effects:
                                  Specification of the intensity of the 3D effect for graphic elements in the
                                  Production Monitor.
                              •   Production Release (quantity-based):
                                  Color in which quantity-based production releases are displayed.
                              •   Production Release (time-based):
                                  Color in which time-based production releases are displayed.
                              •   Display Stati:
                                  Selection whether in addition to the machine the status for backlogs is dis-
                                  played.
                              •   Unscheduled (quantity-based):
                                  Color in which unscheduled work shifts are displayed. The display is quan-
                                  tity-based.
                              •   Unscheduled (time-based):
                                  Color in which unscheduled work shifts are displayed. The display is time-
                                  based.
                              •   Scheduled (quantity-based):
                                  Color in which scheduled work shifts are displayed. The display is quantity-
                                  based.
                              •   Scheduled (time-based):
                                  Color in which scheduled work shifts are displayed. The display is time-
                                  based.
                              •   Primary products finished (quantity-based):
                                  Color in which the finished primary products are displayed. The display is
                                  quantity-based.
                              •   Primary products finished (time-based):
                                  Color in which the finished primary products are displayed. The display is
                                  time-based.

                              [OK] Saves and applies the selection and closes the dialog.
4.50 / 01-2023




                 E-154                                                   A+W Production Capacity Planning
                 Software Reference                                                                         Scheduling




                                        Please Select an Order/Batch
                                        Display > Production Monitor > [Filter view]
                                        Use this dialog to select orders, batches, and self-defined filters by which the
                                        view in the Production Monitor will be filtered.
                                        The dialog offers the following tabs:
                                        •   “Filter – Orders” on page E-155
                                        •   “Filter – Batches” on page E-156
                                        •   “Filter – Individual Filters” on page E-157


                                        Filter – Orders
                                        Display > Production Monitor > [Filter view] > Orders




                                        Fig. E-87     Please select an order/batch – orders


                                        The defined orders are displayed on this tab. You can select one order at a
                                        time. The display in the Production Monitor is restricted to the selected order.

                                        Order number Order number by which filtering should be done.

                                        Customer Customer name by which filtering should be done. The list of or-
                                        ders is restricted to the customer.

                                        Number of records Defines the number of orders to be listed.

                                        [OK] Saves the data.

                                        [Reject] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-155
                 Scheduling                                                              Software Reference




                              Filter – Batches
                              Display > Production Monitor > [Filter view] > Batches




                              Fig. E-88    Please select an order/batch – batches


                              The defined batches are displayed on this tab. You can select one batch at a
                              time. The display in the Production Monitor is restricted to the selected batch.

                              Batch Number Batch number by which filtering should be done.

                              Batch Description Batch description by which filtering should be done. The
                              list of batches is restricted to the batch.

                              Number of Records Defines the number of batches to be listed.

                              [OK] Saves the data.

                              [Reject] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-156                                                   A+W Production Capacity Planning
                 Software Reference                                                                         Scheduling




                                        Filter – Individual Filters
                                        Display > Production Monitor > [Filter view] > Individual Filters




                                        Fig. E-89    Please select an order/batch – individual filters


                                        The individually defined filters are displayed on this tab.

                                        [New] Opens the dialog Create new filter where you can define your own fil-
                                        ters.
                                         “Create New Filter” on page E-158

                                        [OK] Saves the data.

                                        [Reject] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                               E-157
                 Scheduling                                                               Software Reference




                              Create New Filter
                              Display > Production Monitor > [Filter view] > tab Individual Filters > [New]




                              Fig. E-90    Create new filter


                              On this dialog, you can create individual filters for searching in the Production
                              Monitor. You create the filters in the SQL database language.

                                 Creating individual filters
                                 Please contact the A+W Software GmbH customer service should you
                                 need special filters for searching in the Production monitor.

                              Name Name of the filter.

                              Description Description of the filter.

                              SQL Definition of the filter in SQL.

                              [OK] Saves the data.

                              [Reject] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-158                                                   A+W Production Capacity Planning
                 Software Reference                                                                         Scheduling




                                        Machine (Name)
                                        Display > Production Monitor > Machine > Context Menu > Properties




                                        Fig. E-91    Machine (Name)


                                        On this dialog, you change the properties of the machine in the Production
                                        Monitor.

                                        [Categories] Sorts the elements by categories.

                                        [Alphabetical] Sorts the elements alphabetically.

                                        [Properties] Not currently used.

                                        Machine properties
                                        •   ID:
                                            Identification number of the machine.
                                        •   Registration point:
                                            Identification number of the registration point.
                                        •   Name:
                                            Machine name.
                                        •   Bottleneck:
                                            Defines whether the machine is a bottleneck machine. Bottleneck ma-
                                            chines appear in red letter on the List of machines in the production moni-
                                            tor.
                                        •   Display type:
                                            Selection of the unit in which the shift info displays the status Completed.
                                            Available for selection are:
                                            – Percent
                                            – Quantity
                                            – Area
4.50 / 01-2023




                                            – Weight
                                            – Linear meters
                                            – Processing


                 A+W Production Capacity Planning                                                                E-159
                 Scheduling                                                                Software Reference




                              •   Group:
                                  Machine group to which the machine belongs.
                              •   Change performance per type of display:
                                  Specification of the unit in which the performance of the machine is dis-
                                  played.

                              Misc
                              •   Display logical machines:
                                  Selection of whether the logical machines for the selected machine are
                                  also displayed in the Production Monitor, e.g. for the machine Drilling (Drill-
                                  ing machine).

                              [OK] Saves the data.

                              [Reject] Closes the dialog without saving the data.


                              Adjust Shifts for Machine
                              Display > Production Monitor > Machine > Context Menu > Shift Properties




                              Fig. E-92     Adjust shifts for machine


                              On this dialog, you can adjust the work shifts for the machine in question with
                              regard to weekdays.

                              Days Specification of the weekdays for which the change applies.
                               The work shift is not changed for this day.
                               The work shift is changed for this day.

                              Shift number Specification of the shift number.

                              Capacity Enter the shift capacity for the selected weekdays.
4.50 / 01-2023




                              [OK] Saves the data.

                              [Reject] Closes the dialog without saving the data.


                 E-160                                                    A+W Production Capacity Planning
                 Software Reference                                                                         Scheduling




                                        Shift Properties
                                        Display > Production Monitor > Display Shifts > Context Menu > Shift Proper-
                                        ties




                                        Fig. E-93    Shift properties


                                        On this dialog, you can display the properties of a work shift with regard to a
                                        machine.

                                        [Categories] Sorts the elements by categories.

                                        [Alphabetical] Sorts the elements alphabetically.

                                        [Properties] Not currently used.

                                        Shift properties
                                        •   Date:
                                            Date of the selected work shift.
                                        •   Shift number:
                                            Number of the selected work shift.
                                        •   Start, End:
                                            Start and end time from the master data for the selected work shift.
                                        •   Capacity:
                                            Time in hours that are available in the work shift. You can change the ca-
                                            pacity of a work shift. The reduced capability is displayed hatched in the
                                            Production Monitor.
                                        •   Comment:
                                            Comment about manual changes to the current work shift.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-161
                 Scheduling                                                                                Software Reference




                                           •   Status:
                                               Status of a work shift. On the selection menu, you select from among the
                                               following options:
                                               – Active: The work shift is available for the machine in question.
                                               – Deactivated: The work shift is not available for the machine in question.
                                                   The shift is selected in the Production Monitor with an X.
                                                   “Display of the work shifts” on page E-149
                                               – Active for rush orders: The shift is available only for rush orders for the
                                                  machine in question. The shift is selected in the Production Monitor with
                                                  an !.
                                           •   Bottleneck:
                                               Selection of whether the shift is a bottleneck. A bottleneck machine cannot be
                                               booked beyond its capacity.

                                           [OK] Saves the data.

                                           [Reject] Closes the dialog without saving the data.


                                           Reservation Display
                                           Display> Production Monitor > Shift > Context Menu > Show Reservations




                 Fig. E-94    Reservations - overview


                                           This dialog displays all reservations for the current shift. You should delete ex-
                                           pired or cancelled reservations.
                                            Tutorial, “Here's how to delete a reservation” on page E-59
4.50 / 01-2023




                 E-162                                                                 A+W Production Capacity Planning
                 Software Reference                                                                              Scheduling




                                        Workplan from Production Monitor
                                        Display > Production Monitor > Shift > Context Menu > Work Plan
                                        On this dialog, you can get an overview for a particular shift.
                                        The dialog offers the following tabs:
                                        •   “Work Plan - Details” on page E-164
                                        •   “Work Plan - Overview” on page E-165

                                        Context menu
                                        Via the context menu for the batches, you can open other dialogs in order to
                                        display details about the selected batch.
                                        You can select the following entries via the context menu for the columns:

                                        Entry                   Function

                                        Resort                  Sort column in ascending or descending order. Affects the
                                                                first three columns.

                                        Formatting              Select format or unit for the columns, e.g. date format or
                                                                length unit.

                                        Insert                  Opens the selection for columns that can be inserted in
                                                                the various categories.

                                        Delete                  Deletes the selected column.

                                        Display Definition      Opens the Column Definition dialog that shows details
                                                                concerning the column in question.


                                        Buttons
                                        The functions of the buttons are described in detail in the Rough Scheduling
                                        section.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                     E-163
                 Scheduling                                                                             Software Reference




                                            Work Plan - Details
                                            Display > Production Monitor > Shift > Context Menu > Work Plan > Details




                 Fig. E-95    Work plan: Selection from Production Monitor - Details


                                            On this tab, you can get an overview of the planned batches in a particular
                                            shift. You can check the glass types for the selected entries, check details, and
                                            start batches. These functions are described in detail in the Rough Planning
                                            section.

                                            Columns
                                            With the context menu, you can select the columns in order to display the de-
                                            sired information, e.g.:
                                            •   Batch:
                                                Specifies the batch.
                                            •   Order:
                                                Order number.
                                            •   Item (int Itm):
                                                Number of the item.
                                            •   Part No:
                                                Part number.
                                            •   Sequence:
                                                Sequence number for the processing.
                                            •   Proc. No:
                                                Article number of the processing.
4.50 / 01-2023




                                            •   MA Machine:
                                                Number of the machine, used for this processing.



                 E-164                                                                 A+W Production Capacity Planning
                 Software Reference                                                                         Scheduling




                                          Total line
                                          You can display different totals in the totals row, e.g.:
                                          •   Total Quantity T:
                                              Total quantity and quantity in the selected batches.
                                          •   Total Duration:
                                              Total processing time of the selected batches in hours.

                                          Filter

                                          [Add filter] Adds a filter.

                                          Drop-down menu Select a filter:
                                          • Click: Opens the drop-down menu from which you select a filter.
                                          • Right-click: Opens the dialog to edit the current filter.


                                          Work Plan - Overview
                                          Display > Production Monitor > Shift > Context Menu > Work Plan > Overview




                 Fig. E-96   Work plan: Selection from Production Monitor - Overview


                                          On this tab, you can get an overview of the processing types that are done on
                                          a machine in the selected shift.
                                          You can set up the display of the columns in the same way as on the Details
                                          tab.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                               E-165
                 Scheduling                                                             Software Reference




                              Scheduling
                              Display > Scheduling




                              Fig. E-97    Scheduling


                              Dialog Scheduling is used for importing orders as XML data from A+W Busi-
                              ness or A+W Enterprise. When you open the Scheduling dialog, the orders will
                              be imported automatically; after completion, the actual time is shown in field
                              Status.
                              If the automatic import of orders is configured in A+W Production, you do not
                              have to open the Scheduling dialog. Data import will be run as a background
                              process in this case. You can trace the scheduling process in the A+W Service
                              Monitor.
4.50 / 01-2023




                 E-166                                                 A+W Production Capacity Planning
                 Software Reference                                                                      Scheduling




                                        BOM Configuration
                                        Master Data > Scheduling > BOM Configuration




                                        Fig. E-98   BOM configuration


                                        This dialog can be used to analyze the BOM configuration.

                                           No changes of BOM configuration
                                           Changes in the BOM configuration dialog are a severe interference with the
                                           structure of A+W Production. You must never change the BOM configura-
                                           tion. In case of questions please contact the A+W Software GmbH custom-
                                           er service.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                             E-167
                 Scheduling                                                           Software Reference




                              Action
                              Master data > Scheduling > BOM Configuration > [New], [Change]




                              Fig. E-99   BOM configuration - action


                              On this dialog, you can analyze the individual actions for BOM manipulation.
                              Each action consists of at least one condition, with occurrence of which the
                              stored function is executed.

                                 No changes of BOM configuration
                                 Changes in the BOM configuration dialog are a severe interference with the
                                 structure of A+W Production. You must never change the BOM configura-
                                 tion. In case of questions please contact the A+W Software GmbH custom-
                                 er service.
4.50 / 01-2023




                 E-168                                                 A+W Production Capacity Planning
                 Software Reference                                                                            Scheduling




                                             Rescheduling
                                             Display > Production Monitor > Double-click on Shift > Context Menu > Work
                                             Plan > Rescheduling
                                             Display > Orders > Context Menu > Processings > Context Menu > Work Plan
                                             > Rescheduling
                                             Display > Batches > Context Menu > Processings > Context Menu > Work
                                             Plan > Rescheduling




                 Fig. E-100   Rescheduling


                                             In this dialog you can reschedule processing steps for orders or batches to
                                             other dates and machines.
                                              Tutorial, “Rescheduling” on page E-36

                                             1. Select the processing steps to be rescheduled
                                             List of processing steps, that can be rescheduled.
                                             •   Order:
                                                 List of processing steps sorted by date and machine.
                                             •   Item:
                                                 Item number of the processing step in question.
                                             •   Production Date:
4.50 / 01-2023




                                                 Former date for which the processing step has been scheduled..
                                             •   Shift:
                                                 Former shift for which the processing step has been scheduled..


                 A+W Production Capacity Planning                                                                  E-169
                 Scheduling                                                               Software Reference




                              •   Protected:
                                  Display, whether the date is protected.
                              •   Work Process:
                                  Work process scheduled for the processing in question.
                              •   Logical Machine:
                                  Logical machine used for this processing.
                              •   Quantity:
                                  Quantity produced by means of this processing step.
                              •   Machine:
                                  Machine used for this processing.
                              •   Part Number:
                                  Number of the BOM element.
                              •   Sequence:
                                  Processing sequence.
                              •   ProcNo:
                                  Processing number of the processing step.
                              •   Purchase Information:
                                  Defines whether purchased elements are involved.

                              Force Scheduling You can force scheduling on a particular date.
                              Re-scheduling will not be forced.
                               Re-scheduling will be forced. With this setting, the capacity limits of bottle-
                              neck machines are not considered. Therefore, the shifts may be overbooked.

                              Allow express grid For the rescheduling, you can specify that transition
                              times of the type Rush are used.
                               Re-scheduling will be done in the normal grid.
                               Re-scheduling will be done in express grid.

                              Combo box (protection) Selection whether dates are protected against re-
                              scheduling. The protection is usually set after a successful re-scheduling.
                              • Keep Protected Processing Dates:
                                 Protected processing dates will not be rescheduled.
                              • Protect Rescheduling Dates:
                                 The new dates calculated after the rescheduling will be protected against
                                 further rescheduling.
                              • Protect all processing dates:
                                 All processing dates of the selected batches are protected.
                              • Lift processing protection:
                                 The protection for all processing dates of the selected batches is lifted.

                              Reason If you want to permit a date in the past for the rescheduling, you
                              have to enter a reason. With this, the appropriate checkbox is enabled.
                               “Permitted Target Dates in the Past” on page E-171

                              Days for Automatic Postponement of Delivery Date Specification of by
                              how many days the delivery date may be moved.
4.50 / 01-2023




                 E-170                                                   A+W Production Capacity Planning
                 Software Reference                                                                         Scheduling




                                           Re-scheduling and shipping date
                                           The shipping date is protected during re-scheduling to meet the require-
                                           ments of the ERP system. The shipping date will be kept unless it is explic-
                                           itly changed.
                                           Please check with person who entered the order if you want to change the
                                           shipping date.

                                        Reschedule as High Priority Order You can reschedule the processing
                                        with the highest priority.
                                         The priority is rescheduled with normal priority.
                                         The priority is rescheduled with the highest priority. The orders are sched-
                                        uled with minimum transfer times. Here, the times of campaigns can also be
                                        used. Use this setting only in emergencies.

                                        Ignore Dates for Receipt of Goods Some processings depend on having
                                        purchased parts delivered, e.g. the production of an IG lite with a TG that is
                                        not produced in-house.
                                         Goods receipt is expected for production. Goods receipt will be checked be-
                                        fore rescheduling.
                                        Goods receipt will be not checked before rescheduling.

                                        Report Delivery Date Postponement The rescheduling of an item can af-
                                        fect the delivery date.
                                         In case of a delivery date postponement for an item, the delivery date from
                                        the order header will be reported back.
                                         A delivery date postponement of an item will be reported to the order. The
                                        delivery date in the order header will be adjusted. However, this is only possi-
                                        ble if the data is transferred online.

                                        Permitted Target Dates in the Past For rescheduling, you can also permit
                                        dates in the past. The checkbox is only enabled if you have entered a reason.
                                         Dates are not postponed in the past.
                                         The processing can also be postponed in the past. For this, a reason must
                                        be specified.
                                         “Reason” on page E-170

                                        2. Select Date, Shift, and Machine
                                        This section lists the machines and the corresponding shifts per workday.

                                        [Update view] Updates the list.

                                        [Given number of days backwards] Shifts the time period of the shifts dis-
                                        played in the past by the number of days that is specified in the Days field.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-171
                 Scheduling                                                              Software Reference




                              Start date Specification of the start date from which the time period should be
                              displayed.

                              Days Specification of by how many days the display of the shifts with the but-
                              tons should be scrolled forward or back.

                              [Given number of days forward] Shifts the time period of the shifts dis-
                              played in the future by the number of days that is specified in the Days field.

                              3. Execute Re-scheduling

                              Select the mode to start re-scheduling Choose the mode in which re-
                              scheduling will be executed.
                              • Reschedule complete parts list: The complete parts list to which the pro-
                                 cessing belongs is rescheduled.
                              • Only selected processing:
                                 Only the selected processing is rescheduled.
                              • Selected processing and all following:
                                 The selected processing and all following processings on the list will be re-
                                 scheduled.
                              • Selected and all previous processings:
                                 The selected and all previous processings of the lite are rescheduled.
                              • Unconditional allocation of date for selected processing:
                                 The selected processing is rescheduled on the selected date for the ma-
                                 chine selected. The plausibility is not checked and the machine capacities
                                 are not considered.

                              [Re-schedule] Starts the rescheduling with the selected parameters. The
                              button is only enabled if a rescheduling mode is selected.

                              [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-172                                                  A+W Production Capacity Planning
                 Software Reference                                                                      Scheduling




                                        Machine Reallocation
                                        Orders > Context Menu > Work Schedule > Rescheduling
                                        Batches > Context Menu > Work Schedule > Rescheduling




                                        Fig. E-101   Machine reallocation


                                        On this dialog you can reschedule processings for orders or batches to other
                                        logical machines. For the machine rescheduling, the processing duration will
                                        not be recalculated. The costs and scheduling rules are not checked.
                                        A rescheduling via this dialog only makes sense if you can reschedule on an
                                        identical logical machine.

                                        Logical routes Machines and logical machines from which a processing
                                        should be rescheduled.

                                        Alternatives for reassignment Display and selection of the possible alter-
                                        natives to the selected logical machine.

                                        [Apply] Saves the data.

                                        [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                            E-173
                 Scheduling                                                                            Software Reference




                                           Post-Processing Booking
                                           Master Data > Post-Processing Booking




                 Fig. E-102   Post-processing booking


                                           On this dialog, you can rework orders that were not scheduled successfully
                                           and schedule them again.
                                            Tutorial, “Post-Processing of Scheduled Orders” on page E-41

                                           [Edit] Opens the dialog Defective orders which enables you to handle sched-
                                           uling problems.
                                            “Defective Orders” on page E-177

                                           [Update] Updates the displayed data.

                                           Orders overview
                                           The display of the columns depends on the option that is selected in the Post-
                                           Processing of... field.
                                           •   Order Number:
                                               The order number is displayed if the Undefined Articles option is selected.
                                           •   Article No., Article Name.:
                                               Number and name of the article that is not defined are displayed if the Un-
                                               defined Articles or Undefined Processings option is selected.
                                           •   Production Article Number, Production Article: Number and name of the
                                               production article that is not defined are displayed if the Undefined Produc-
4.50 / 01-2023




                                               tion Article/Thickness Combinations option is selected.




                 E-174                                                                A+W Production Capacity Planning
                 Software Reference                                                                           Scheduling




                                        •   Thickness:
                                            The thickness in mm is displayed if the Undefined Production Article/Thick-
                                            ness Combinations option is selected.
                                        •   Message:
                                            The text of the report is displayed if the Report Problems option is selected.
                                        •   Status:
                                            The status of the orders is displayed if the Defective Order Data option is
                                            selected.
                                        •   Number of orders:
                                            The number of orders with the same status is displayed if the Defective Or-
                                            der Data option is selected.
                                        •   Time stamp of the import file:
                                            Date and time at which the order was scheduled.
                                        •   Item:
                                            The number of the order item is displayed if the Changes of Scheduled Or-
                                            ders option is selected.
                                        •   ItemRef:
                                            The reference number of the order item is displayed if the Changes of
                                            Scheduled Orders option is selected.
                                        •   Packing Group:
                                            The packing group that is assigned to the batch is displayed if the Changes
                                            of Scheduled Orders option is selected.
                                        •   Qty. Items:
                                            The number of items belonging to the batch is displayed if the Changes of
                                            Scheduled Orders option is selected.
                                        •   Change Text:
                                            The text from the ERP system is displayed if the Changes of Scheduled Or-
                                            ders option is selected. For this, the text has to be transferred.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                 E-175
                 Scheduling                                                               Software Reference




                              Post-Processing of
                              With the selection of the option, you specify according to which criteria the or-
                              ders in the list should be displayed. In brackets is a number indicating how
                              many orders with the criterion are present.
                              For undefined articles, thickness combinations, and/or processings, you can
                              open and correct the order with a double-click.
                              •   Undefined Articles (n orders):
                                  Orders with undefined articles.
                              •   Undefined Production Article/Thickness combinations (n orders):
                                  Orders with undefined production article combinations and undefined thick-
                                  ness combinations.
                              •   Undefined Processings (n orders):
                                  Orders with undefined processings.
                              •   Report Problems (n orders):
                                  Orders with report problems. Report problems can occur with the data
                                  transfer between an ERP system and A+W Production.
                                   “Asynchronous Processing” on page E-178
                              •   Changes of Scheduled Orders (n Orders):
                                  Orders that were changed after scheduling.
                                   “Changes to Scheduled Orders” on page E-179
                              •   Defective Order Data (n orders):
                                  Orders with defective order data.
                                   “Defective Orders” on page E-177
                              •   Orders with reference status (n orders):
                                  Orders with reference status.

                              Display by
                              With the selection of the option, you specify how the orders in the list are sort-
                              ed.
                              •   Order number:
                                  Sorting by order numbers.
                              •   Reason for post-processing:
                                  Sorting by reasons for post-processing.

                              Detailed Display for Batches and Packing Groups
                              The field is displayed if the Changes of Scheduled Orders option is selected.
                              •   Batch:
                                  Number of the batch.
                              •   Batch status:
                                  Status of the batch.
                              •   Packing group:
                                  Packing group that is assigned to the batch.
4.50 / 01-2023




                 E-176                                                   A+W Production Capacity Planning
                 Software Reference                                                                            Scheduling




                                        Defective Orders
                                        Master Data > Post-Processing Booking > [Edit]




                                        Fig. E-103    Defective Orders


                                        On this dialog, you can select how orders that are not scheduled should be
                                        processed.
                                         Tutorial, “Post-Processing of Scheduled Orders” on page E-41
                                        You can choose one of the following options:
                                        •   Repeat data import:
                                            The selected orders are rescheduled. You can use this option e.g. in case
                                            of master data errors, e.g. if A+W Production has failed to find a shift for the
                                            orders. This gives you the chance of correcting the error in master data,
                                            e.g. by adjusting the shifts. After that, you can reschedule the orders with-
                                            out importing the data again from the ERP system.
                                        •   Force scheduling. Free capacity at bottleneck machines will not be consid-
                                            ered:
                                            The order is rescheduled without taking the capacity into account. This may
                                            affect your production because the existing capacity could be exceeded,
                                            and other orders might be postponed.
                                        •   Ignore scheduling. The production dates are determined without consider-
                                            ation of transfer times, capacity limits, and campaign dates. You must cre-
                                            ate valid workplans via manual scheduling.
                                        •   Delete invalid orders: The system will NOT be able to schedule these or-
                                            ders. Please check with order entry first!
                                            The orders are deleted from A+W Production. To repeat scheduling, the or-
                                            ders have to be imported once more from the ERP system.
                                        •   Confirm calculated delivery date:
                                            Accepts the new delivery date A+W Production suggests for the selected
                                            orders. The orders are scheduled based on the new delivery date condi-
4.50 / 01-2023




                                            tions; the calculated delivery date is reported to the ERP system.
                                            Delivery dates should be changed only after checking with production
                                            scheduling!


                 A+W Production Capacity Planning                                                                   E-177
                 Scheduling                                                              Software Reference




                              Asynchronous Processing
                              Master Data > Post-Processing Booking > Report Problems Option > [Edit]




                              Fig. E-104   Asynchronous processing


                              On this dialog, you can select how orders with reporting problems should be
                              processed.
                              You can choose one of the following options:
                              •   Try again:
                                  The selected orders were scheduled again. Use this option, e.g. in case of
                                  errors during data transfer.
                              •   Cancel item:
                                  The item is cancelled. The remaining order is scheduled. With this option,
                                  you should consult the customer so that the data is transferred again.
                              •   Ignore error:
                                  The production dates are determined. The item is taken over, however the
                                  report is not written. That's why you may only select this option if you are
                                  absolutely sure that you can ignore the error.
4.50 / 01-2023




                 E-178                                                   A+W Production Capacity Planning
                 Software Reference                                                                          Scheduling




                                        Changes to Scheduled Orders
                                        Master Data > Post-Processing Booking > [Edit].




                                        Fig. E-105    Changes to scheduled orders


                                        On this dialog, you can select how scheduled orders should be handled for
                                        which changes were transferred.
                                        You can choose one of the following options.
                                        •   Create new line item:
                                            Cancellation of the previous item and takeover of the change as new item
                                            into the pool.:
                                            The order is scheduled again with a new item number.
                                        •   Try again:
                                            Takeover of the change into the pool. Resolve the affected batches/PMO
                                            master groups beforehand.:
                                            First resolve the affected batches and then select this option. The order is
                                            then rescheduled.
                                        •   Ignore modification:
                                            Delete the modification. The previous item remains unchanged.:/
                                            The modification is deleted and the original data retained.
                                        •   (not recommended):
                                            Takeover of the change into the previous batches. Before this, make sure
                                            that the modification is not production-relevant.:
                                            Not currently used.

                                        [Analyze change] Not currently used.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-179
                 Scheduling                                                                 Software Reference




                              Split Items
                              Display > Orders > Context menu > Split items




                              Fig. E-106    Split items


                              On this dialog, you can split items from orders. If for a large item the process-
                              ing time of the slowest machine exceeds the configured threshold, this item is
                              split by A+W Capacity Planner in the course of scheduling. Generally the items
                              are split automatically so that scheduling runs at optimal speed even for larger
                              items.
                              The item split is described in the Rough Planning - Tutorial section.
                               Rough Scheduling: Tutorial, “How to split an item” auf Seite C-52

                              Selected items
                              The list contains the processing steps you have selected in dialog Process-
                              ings.
                              •   Order:
                                  Order that you have selected for splitting.
                              •   Item:
                                  Number of the order item.
                              •   Subitem:
                                  Number of subitems in the order.
                              •   Quantity:
                                  Number of lites in the item.

                              [Remove] Deletes a selected item.
4.50 / 01-2023




                 E-180                                                    A+W Production Capacity Planning
                 Software Reference                                                                           Scheduling




                                        Splitting options
                                        With the selection of the option, you specify how the items are split:
                                        •   Split per item in...:
                                            Specification of into how many new items will be split. The field for specify-
                                            ing the number is enabled.
                                        •   Create items with maximum...:
                                            Specification of the maximum number of lites a new item may contain. The
                                            field for specifying the number is enabled.
                                        •   Create per item one item with:
                                            Specification of the number of lites for which a new item is generated. The
                                            field for specifying the number is enabled.
                                        •   Split according to PMO result:
                                            Specification that the items are split according to the packing optimization.

                                        New Items
                                        The list shows the split items as subitems.
                                        •   Order:
                                            Order number.
                                        •   Item:
                                            Number of the order item.
                                        •   Subitem:
                                            Number of subitems in the order.
                                        •   New item:
                                            Number of the new items after the split. The number is counted per split or-
                                            der item.
                                        •   Quantity:
                                            Number of lites in the new item.

                                        [Split] Splits the selected item. The new items are only saved if they have
                                        been confirmed with [Accept].

                                        [Accept] Saves the new items. This action cannot be undone.

                                        [Reject] Restores the original item. Then you can split the item with other
                                        specifications.

                                        [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                 E-181
                 Campaigns and Reservations                                                      Software Reference




                                       Campaigns and Reservations
                                       You can define campaigns and reserve capacities for particular work process-
                                       es.
                                       This section provides information on the following subjects:
                                       •   “Campaigns” on page E-183
                                       •   “Expired Reservations” on page E-186
                                       •   “Reservations” on page E-187
                                       •   “Reservation for Machine” on page E-189
                                       •   “Select a Customer” on page E-190
                                       •   “Select Project” on page E-191
4.50 / 01-2023




                 E-182                                                          A+W Production Capacity Planning
                 Software Reference                                                        Campaigns and Reservations




                                           Campaigns
                                           Master Data > Capacity Planning > Campaign Planning
                                           On this dialog, you can define campaigns as individual dates or weekly dates.
                                           With campaigns, you can plan capacities for particular work processes, e.g. for
                                           screen printing in a different color for each day of the week.

                                               Prerequisite
                                               Only the processings are schedule in campaign dates that are defined as
                                               campaign processings.

                                            Tutorial, “Campaign Planning” on page E-43
                                           The Campaigns dialog offers the following tabs:
                                           •   “Campaigns – Individual Dates” on page E-183
                                           •   “Campaigns – Weekly Dates” on page E-185


                                           Campaigns – Individual Dates
                                           Master data > Capacity Planning > Campaign Planning > Individual Dates tab
4.50 / 01-2023




                 Fig. E-107   Campaigns – individual dates




                 A+W Production Capacity Planning                                                                  E-183
                 Campaigns and Reservations                                                        Software Reference




                                       On this tab, you manage individual campaigns. With individual campaigns, you
                                       conduct campaigns that occur once.
                                        Tutorial, “Campaign Planning” on page E-43

                                       Work process Work processes you have defined in machine allocation. A
                                       work process is grayed out on the list when it has been added to a campaign.

                                       Campaigns Work processes you have added which are valid for campaigns.
                                       If you select a work process from the Campaigns list, the tabs Individual dates
                                       and Weekly dates show the corresponding dates.
                                       The campaign is inactive.
                                       The campaign is active.

                                       [Allocate] Moves a selected element to the other side.

                                       Individual dates

                                       Calendar Choose a date for the campaign.

                                       Shifts Available shifts on the selected date.

                                          Display shifts
                                          Only the active shift plans are displayed. If necessary, activate the shift
                                          plans that are required for the campaign.

                                       Individual dates Display of the campaign for the selected date.
                                       • Date:
                                          Dates for which campaigns have been defined.
                                       • Shift:
                                          Work shift during which the corresponding campaign will be run.

                                          Delete campaigns
                                          Deleting campaigns at short notice will affect the production. Processings
                                          may not be executed for instance, or production dates may change.
                                          Please contact the customer service of A+W Software GmbH should you
                                          want to delete campaigns and if orders have already been scheduled at this
                                          point.

                                       Add for the next The period of time for which the campaign is defined.
                                       You can use this option to define whether the duration of the date is specified
                                       in days or in weeks.

                                       [Add campaign] Adds a campaign. For this, the following elements have to
                                       be selected:
                                       • a work process valid for campaigns
                                       • a date
                                       • a shift
4.50 / 01-2023




                                       [Delete] Deletes a selected campaign.

                                       [OK] Saves the data.


                 E-184                                                            A+W Production Capacity Planning
                 Software Reference                                                        Campaigns and Reservations




                                          [Cancel] Closes the dialog without saving the data.


                                          Campaigns – Weekly Dates
                                          Master data > Capacity Planning > Campaign Planning > Weekly Dates tab




                 Fig. E-108   Campaign days – Weekly dates


                                          On this tab, you manage individual campaigns. Serial campaigns serve to han-
                                          dle periodically recurring campaigns.
                                           Tutorial, “Definition and Management of Campaigns” on page E-46
                                          A description of the fields in dialog Campaigns can be found in:
                                           “Campaigns – Individual Dates” on page E-183

                                          Weekly dates Display of the campaigns for the selected day of the week.
                                          • Weekday:
                                            Workdays for which you have created campaigns.
                                          • Shift:
                                            Work shift during which the corresponding campaign will be run.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                              E-185
                 Campaigns and Reservations                                                     Software Reference




                                       Expired Reservations
                                       Master data > Capacity Planning > Reservations




                                       Fig. E-109   Expired reservations


                                       This dialog presents the reservations that have expired. This dialog appears
                                       automatically when you open the Reservations dialog and there are any ex-
                                       pired reservations.

                                       List
                                       •   Machine:
                                           Machine of which capacity has been reserved.
                                       •   Customer:
                                           Customer for whom the capacity has been reserved.
                                       •   Project:
                                           Project for which the capacity has been reserved.
                                       •   Week:
                                           Calendar week in which the capacity has been reserved.
                                       •   Year:
                                           Year for which the capacity has been reserved.
                                       •   Date:
                                           Date on which the reservation begins.
                                       •   Shift:
                                           Work shift for which the capacity has been reserved.
                                       •   Percentage:
                                           Capacity in percentage that was reserved on the machine.
                                       •   Used:
                                           Shows the percentage of the reservation which has already been used up.
                                       •   Process:
                                           Date on which the reservation ends.
4.50 / 01-2023




                 E-186                                                          A+W Production Capacity Planning
                 Software Reference                                                      Campaigns and Reservations




                                        [Delete] Deletes the selected reservation.

                                        [OK] Saves the data and closes the Reservations window


                                        Reservations
                                        Master data > Capacity Planning > Reservations




                                        Fig. E-110    Reservations


                                        On this dialog, you manage reservations of machine capacities. Reservations
                                        are only possible on the individual machines that are defined as bottleneck
                                        machines. They are temporally limited. A bottleneck machine cannot be booked
                                        beyond its capacities.

                                        The reservations are either created for specific customers or construction proj-
                                        ects.
                                        The reserved times are marked in the respective shifts in the Production Mon-
                                        itor.
                                         Tutorial, “Reservations” on page E-53

                                           Reservations for individual orders
                                           Reservations of times for individual orders must be entered and transferred
                                           by the ERP system. The orders marked as Reservation order and released
                                           for production reserve appropriate times on all machines required for the
4.50 / 01-2023




                                           production.




                 A+W Production Capacity Planning                                                                E-187
                 Campaigns and Reservations                                                        Software Reference




                                       Reservations

                                           Reservations in shifts, days or weeks
                                           Generally, capacities are reserved by the week. Depending on the setting
                                           under Master Data > Configuration > A+W Production > Capacity Planning
                                           > Type of Reservation, days or shifts can be specified for the reservation.
                                           If you change the setting, the old reservations are lost.

                                       Machine Choose the machine the reservations of which are displayed. The
                                       list includes all machines that have been defined as bottleneck machines.

                                       Start date Start of the reserved period. By default, the current day is dis-
                                       played.

                                       Days Defines the number of days shown in the preview.

                                       Shift reservations
                                       In the Shift reservations area, the reservations starting from the selected date
                                       are displayed graphically.

                                       Free Free capacity of the machine.

                                       Reserved Reserved capacity of the machine.

                                       Used Actually used share of the reservation.

                                       Reservations per customer
                                       If a day is selected in the Shift reservations area, an overview with all reserva-
                                       tions is displayed.
                                       •   Customer:
                                           Customer for whom the capacities have been reserved.
                                       •   Project:
                                           Project for which the capacities have been reserved.
                                       •   Reservation:
                                           Reserved machine capacities in percent.
                                       •   Used:
                                           Actually used share of the reservation in percent.
                                       •   Expiry date:
                                           Date on which the reservation ends.
                                       •   Date:
                                           Date on which the reservation was entered.
                                       •   Shift:
                                           Work shift for which the reservation applies.

                                       [New] Opens the dialog to reserve machine capacities.
                                        “Reservation for Machine” on page E-189
4.50 / 01-2023




                                       [Delete] Deletes the selected reservation.

                                       [OK] Saves the data.


                 E-188                                                             A+W Production Capacity Planning
                 Software Reference                                                        Campaigns and Reservations




                                        [Quit] Cancels the processing and closes the dialog.


                                        Reservation for Machine
                                        Master data > Capacity Planning > Reservations > [New]




                                        Fig. E-111   Reservation for customer or project


                                        On this dialog, you reserve machine capacities for a particular customer or
                                        project.

                                           Reservations in shifts, days or weeks
                                           Generally, capacities are reserved week by week. Depending on the set-
                                           ting under Master Data > Configuration > A+W Production > Capacity Plan-
                                           ning > Type of Reservation, however, days or shifts can also be specified
                                           for the reservation. If you change the setting, the old reservations are lost.

                                        Customer Customer for whom the machine capacity is reserved. The [Zoom]
                                        opens the dialog Select customer.
                                         “Select a Customer” on page E-190

                                        Project Project for which machine capacity shall be reserved. The [Zoom]
                                        icon opens the Select project dialog.
                                         “Select Project” on page E-191

                                        Date Start of the reserved period.

                                        Shift Shift in which the machine is reserved.

                                        Expiry date End of the reserved period.

                                        Reservation in % Machine capacity in percent that should be reserved.
                                        You can enter the reservation as a number or by dragging the bar in the field
4.50 / 01-2023




                                        with the mouse.

                                        [OK] Saves the data.



                 A+W Production Capacity Planning                                                                E-189
                 Campaigns and Reservations                                                       Software Reference




                                       [Close] Closes the dialog without saving the data.


                                       Select a Customer
                                       Master data > Capacity Planning > Reservations > [New] > Customer




                                       Fig. E-112   Select a customer


                                       On this dialog, you select the customer for whom you want to reserve machine
                                       capacities.

                                       Overview
                                       •   ID:
                                           Customer number.
                                       •   Name:
                                           Customer name.
                                       •   Matchcode:
                                           Matchcode assigned to the customer.

                                       Matchcode Enter a matchcode to search for a customer.

                                       Name Enter a name to search for a customer.

                                       Quantity Number of customers to be displayed in the overview.

                                       [Find] Starts the search if you have entered the wild card % in the filter crite-
                                       rion.

                                       [OK] Takes over the selected customer into the Reservation for machine dia-
                                       log.

                                       [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-190                                                            A+W Production Capacity Planning
                 Software Reference                                                      Campaigns and Reservations




                                        Select Project
                                        Master data > Capacity Planning > Reservations > [New] > Project




                                        Fig. E-113    Select project


                                        This dialog serves to select the project for which a reservation shall be made.

                                        Overview
                                        •   ID:
                                            Project ID.
                                        •   Description:
                                            Description of the project.

                                        Name Enter a name to search for the project.

                                        Quantity Number of projects to be displayed in the overview.

                                        [Find] Starts the search if you have entered the wild card % in the filter crite-
                                        rion.

                                        [OK] Takes over the selected project into the Reservation for machine dialog.

                                        [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-191
                 Processings                                                             Software Reference




                               Processings
                               The processings describe the steps for producing the parts. The processing
                               generation ensures that for each BOM part, it is described how it is created in
                               production. This information is indispensable for A+W Capacity Planner and it
                               makes sense otherwise, e.g. to see the whole creation of the products on the
                               papers.
                               This section provides information on the following subjects:
                               •   “Creation of Processings” on page E-193
                               •   “Add an Existing Condition” on page E-195
4.50 / 01-2023




                 E-192                                                   A+W Production Capacity Planning
                 Software Reference                                                                          Processings




                                           Creation of Processings
                                           Master data > Capacity Planning > Creation of Processings




                 Fig. E-114   Creation of Processings


                                           On this dialog, you assign the processing articles to the part types that are
                                           stored in the master data. This assignment is necessary, for example, if your
                                           ERP system does not transfer these processings.
                                           Using the assignments, work processes can be determined. These details are
                                           required for production planning and cost determination.
                                           Creation of processing means that processings are created for the parts of the
                                           BOM, the part types, and the procurement types. The processings describe
                                           how the parts are created. So that the capacity planning can work, processings
                                           must be defined, at least for all stock removals, ordered and cut parts and as-
                                           sembly processings such as LAMI and IG.
                                           Heed additional processings such as Pack and Send, insofar as these are not
                                           transferred by your ERP system.
                                            Tutorial, “Creation of Processings” on page E-64
4.50 / 01-2023




                                           Creation of processings

                                           Processings Production-relevant processing types and allocated process-
                                           ing articles.

                 A+W Production Capacity Planning                                                                  E-193
                 Processings                                                               Software Reference




                               Part types Part types with allocated processing articles.

                               [Allocate] Assigns a selected processing article to the selected part type.

                               Details Information on the selected processing type or processing article.
                               •   Article number:
                                   Article number of the selected processing article.
                               •   Processing type:
                                   – If a processing article has been selected: allocated processing type.
                                   – If a processing type has been selected: ID of the processing type.
                               •   Procurement type:
                                   Procurement type for this processing type.
                               •   Class:
                                   Defines the processing class to which the selected processing article be-
                                   longs, e.g. arrissing.
                               •   Name:
                                   Name of the selected element.
                               •   Sequence/sequence number:
                                   This is the sequence defined for the selected element. The higher the se-
                                   quence number, the later will be processing be applied to the glass.
                                   – If a sequence has been defined for a processing article, this will be
                                       obeyed.
                                   – If no sequence has been defined for a processing article, the sequence
                                       defined for the processing type will be applied.
                                   For all defining processings like e.g. insulating, annealing, or packing, the
                                   sequence 100 can be set. For all other processings like e.g. arrissing and
                                   drilling, the sequence has to be ascending.

                                   Sequence and sequence number
                                   The sequence defines the sequence of processing steps and is therefore
                                   relevant for production.
                                   Please contact the customer service of A+W Software GmbH if you want
                                   to change any sequences.

                               • Part type:
                                 This is the number allocated to the part type, e.g. 2 for Trade glass.
                                 The part type is defined by A+W Software GmbH.
                               The field below shows a description of the selected element.

                               [Categories] Sorts the elements by categories.

                               [Alphabetical] Sorts the elements alphabetically.

                               [Properties] Not currently used.

                               Conditions Formulas that are assigned to the processing article that is se-
                               lected in the Part types area.
4.50 / 01-2023




                 E-194                                                    A+W Production Capacity Planning
                 Software Reference                                                                       Processings




                                           Formulas and conditions
                                           Formulas have have a massive impact on the properties and planning ef-
                                           fects of processing types and part types under some circumstances. You
                                           must understand what effects the stored formula has.
                                           There is a separate manual about the topic formulas and restrictions in
                                           A+W Production.

                                        [New] Opens the Add existing condition dialog in order to assign a formula to
                                        the processing article.

                                        [Delete] Deletes the selected formula in field Conditions.

                                        [OK] Saves the data.


                                        Add an Existing Condition
                                        Master Data > Capacity Planning > Creation of Processings > [New drop-down
                                        menu] > [Add Existing Condition]




                                        Fig. E-115   Add an existing condition


                                        On this dialog you select the condition that you want to assign to a processing
                                        on the Creation of Processings dialog.

                                        [OK] Imports a selected formula into the dialog Creation of processings.

                                        [Close] Closes the dialog without importing a condition into the Creation of
                                        processings dialog.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                               E-195
                 Time Master Data                                                             Software Reference




                                    Time Master Data
                                    You have to enter times for all processing steps as a basis for calculating the
                                    duration per processing item.
                                    This section provides information on the following subjects:
                                    •   “Default Times” on page E-197
                                    •   “Default Time Formula” on page E-199
                                    •   “Add elements” on page E-203
                                    •   “Tabelle, Vector (Name)” on page E-204
                                    •   “Input Help for Vectors” on page E-205
                                    •   “Select Formula” on page E-207
                                    •   “Entering a Formula Element” on page E-208
                                    •   “User-defined Table Elements” on page E-210
                                    •   “Select Limit” on page E-211
                                    •   “Time Formula Test” on page E-212
                                    •   “Formula Object Properties” on page E-214
                                    •   “Formula (Name)” on page E-215
                                    •   “Course of Formula Evaluation” on page E-216
                                    •   “Transition Times” on page E-217
4.50 / 01-2023




                 E-196                                                        A+W Production Capacity Planning
                 Software Reference                                                                   Time Master Data




                                        Default Times
                                        Master data > Capacity Planning > Default Times




                                        Fig. E-116   Default times


                                        On this dialog, you manage the calculation formulas for the processings on
                                        one of the logical machines. With a formula, you define how the duration of a
                                        work process is calculated. Basis of the calculation is, e.g. the respective area
                                        or edge length in the individual order item.
                                         Tutorial, “Default Times” on page E-105
                                        There are two different editors available for the creation of formulas. For a de-
                                        tailed description, see the Formula editor section.
                                        In the line 0 – All machines, you can define formula elements as templates for
                                        all machines.

                                        Default time formulas
                                        In the overview, all machines defined in A+W Production are displayed. This
                                        data is imported from the machine assignment and cannot be edited.
                                        •   No.:
                                            Number of the logical machine.
                                        •   Log:
4.50 / 01-2023




                                            Logical ID of the logical machine.
                                        •   Machine:
                                            Name of the machine.


                 A+W Production Capacity Planning                                                                 E-197
                 Time Master Data                                                              Software Reference




                                    •   Log. Machine:
                                        Name of the logical machine.
                                    •   Bottleneck:
                                        Indication whether the machine is defined as a bottleneck machine.
                                    •   Individual:
                                        Indication whether the machine forms processing chains. If no processing
                                        chains should be formed, the processings are worked through individually,
                                        that is, scheduled one after another in separate steps.
                                        This setting makes sense for screen printing, surface processings, etc.
                                        For drilling, grinding, etc., the checkbox should not be checked since pro-
                                        cessing chains make sense for these processings.
                                    •   Manual:
                                        Indication whether the machine is operated manually. Manual machines
                                        are not included in the automatic machine scheduling. They are also locked
                                        for the automatic item split.
                                    •   Type:
                                        Machine type of the corresponding machine.
                                    •   ID:
                                        Number of the logical machine. This ID is important for technical support.

                                    [Edit] Opens the Default time formula dialog so that the default time formula
                                    can be edited.
                                     “Default Time Formula” on page E-199

                                        Existing default time formula
                                        If you click Edit and a formula-based default time formula is assigned, a
                                        message will be displayed. Contact A+W Software GmbH customer ser-
                                        vice if you want to change the default time.

                                    [Delete] Deletes the selected entry.

                                    [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-198                                                        A+W Production Capacity Planning
                 Software Reference                                                                         Time Master Data




                                            Default Time Formula
                                            Master data > Capacity Planning > Default Times > [Edit]




                 Fig. E-117   Default time formula, example showing all selection options


                                            Use this dialog to edit the cycle times of a logical machine.

                                               Change default time formula
                                               Please change or define default time formulas only in agreement with A+W
                                               Software GmbH customer service.

                                               Complex default time formulas are a profound operation in A+W Produc-
                                               tion and should only be defined by the A+W Software GmbH customer ser-
                                               vice. A default time formula is considered to be complex e.g. if it includes
                                               two or more factors/vectors.

                                             Tutorial, “Definition and Management of Default Time Formulas” on page E-117
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                     E-199
                 Time Master Data                                                                   Software Reference




                                    Default time formula
                                    List of the elements that belong to the formula.

                                    Basic time Specification of the basic time for the default time formula in sec-
                                    onds.
                                    If the calculation begins with the determination from a formula, specify 0 as
                                    start value, e.g. the calculation of an area before the first screen printing is ap-
                                    plied.
                                    You can define the following time allowances for the calculation:
                                    • Factor ’Gas’:
                                         Time required for filling an IG unit with gas.
                                    • Factor 'Muntins’:
                                         Time required based on the number of muntins.
                                    • Shape Factor:
                                         Time required depending on the selected shape.
                                    • Factor ’Large lite', 'Small lite':
                                         Time allowance depending on the sheet size. Please also enter the sheet
                                         size.
                                    • Factor ’TGH’:
                                         Time allowance for the handling of toughened glass.
                                    • Factor ’LAM’:
                                         Time allowance for the handling of laminated glass.
                                    • Factor ’at least triple IG':
                                         Time allowance for the handling of triple IG.
                                    • Coating factor:
                                         Time allowance for taking in to account the handling of coated
                                         sheets.
                                    • Vector ’Weight -> Factor’:
                                         Time allowance based on the sheet weight.
                                    • Vector ’Length -> Factor’:
                                         Time allowance based on the edge length to be processed.
                                    • Vector ’Qty. -> Factor’:
                                         Time allowance based on the number of sheets to be processed.
                                    • Vector ’Thickness -> Factor’:
                                         Time allowance depending on the sheet thickness.
                                    • Vector ’Sqft -> Factor’:
                                         Time allowance based on the surface to be processed.
                                    • Vector ’Edge Matrix -> Factor’:
                                         Time allowance based on the edge matrix of the sheets.
                                    • ’Free’ element 1 … 10:
                                         Free elements for further time allowances.

                                    + value, + vector, + table Selection of the calculation operation for a con-
                                    stant value, a vector or a table:

                                    Setting            Meaning
4.50 / 01-2023




                                    + Table            The value from the table is added to the intermediate result.

                                    Tab. E-5      Possible settings for the default time formula


                 E-200                                                            A+W Production Capacity Planning
                 Software Reference                                                                           Time Master Data




                                        Setting              Meaning

                                        + b * value          The basic time is multiplied by the value. The result of the
                                                             multiplication is added to the intermediate result.

                                        + value              The value is added to the intermediate result.

                                        * (1 + value)        The value is added to 1 and the result multiplied by the
                                                             intermediate result from the previous line.

                                        * Vector             The result of the previous line is multiplied by the value of the
                                                             vector.

                                        Tab. E-5        Possible settings for the default time formula

                                           Calculation sequence
                                           For the calculation, you must consider the operator sequence of mathemat-
                                           ics: multiplication and division are calculated before addition and subtrac-
                                           tion unless parentheses specify the sequence.
                                           Furthermore, you must heed the sequence of the lines if a calculation
                                           should build on the result of the previous line.

                                        […] Opens the dialog Vector (Name) where you can edit the properties of the
                                        vector.
                                         “Tabelle, Vector (Name)” on page E-204

                                        [Sort] Moves a selected element in the default time formula. The sequence
                                        of factors is essential if you choose the option Factor multiplied by subtotal.

                                        [Multiplication of formula result by the processing quantity per part]
                                        You can multiply the result of the formula by the quantity to be processed per
                                        part.
                                        The result of the formula will not be multiplied by the processing quantity per
                                        part.
                                        The result of the formula will be multiplied by the processing quantity per
                                        part.

                                        Own formula
                                        Display of the assigned formula.

                                        [Zoom] Opens the dialog Generic Select Form where you can select self-de-
                                        fined formulas.
                                         “Select Formula” on page E-207

                                        [Cross] Removes a formula from the field Own formula.

                                        [Formula editor] Opens the Enter a formula element dialog on which you
                                        can create a formula.
                                        There is a separate manual on the topic of the Formula editor.
4.50 / 01-2023




                                         “Entering a Formula Element” on page E-208




                 A+W Production Capacity Planning                                                                           E-201
                 Time Master Data                                                          Software Reference




                                    Formula test Opens the dialog Time Formula Test which is used to analyze
                                    formulas for time calculation.
                                     “Time Formula Test” on page E-212

                                    [New] Opens the dialog Add Elements in which you can select elements.
                                     “Add elements” on page E-203

                                    [OK] Saves the data.

                                    [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-202                                                       A+W Production Capacity Planning
                 Software Reference                                                                   Time Master Data




                                        Add elements
                                        Master data > Capacity planning > Default times > [Edit] > [New]




                                        Fig. E-118   Add elements


                                        On this dialog, you can apply elements for time allowances on the Default time
                                        formula dialog.
                                         Tutorial, “Definition and Management of Default Time Formulas” on page E-117

                                        [Delete] Deletes the selected entry.

                                        [OK] Takes over the selected entry into the Default time formula dialog.

                                        [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-203
                 Time Master Data                                                                 Software Reference




                                    Tabelle, Vector (Name)
                                    Master data > Capacity planning > Default times > select logical machine >
                                    [Edit] > [...]




                                    Fig. E-119   Value entry – entry into table, matrix display


                                    On this dialog, you edit the properties of a time allowance. You can edit the
                                    values depending on type in the table entry.
                                     Tutorial, “Definition and Management of Default Time Formulas” on page E-117

                                    Columns The display of the columns depends on the formula element for
                                    which the dialog is opened, e.g. thickness, weight, height, and width.

                                       Example of thickness

                                       If you enter 4.00 mm, 8.00 mm, and 10.00 mm for the thickness in the table,
                                       the allocated factors will apply to the thicknesses 4.00 to 7.99 mm, 8.00 to
                                       9.99 mm, etc.


                                    Value Factor (value) per thickness, weight, length, quantity, surface, or edge
                                    matrix.

                                    [Input help] Opens the Input help for vectors dialog.
                                     “Input Help for Vectors” on page E-205

                                    [OK] Takes over the selected entry into the Default time formula dialog.

                                    [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-204                                                            A+W Production Capacity Planning
                 Software Reference                                                                     Time Master Data




                                        Input Help for Vectors
                                        Master data > Capacity planning > Default times > select logical machine >
                                        Edit > [...] > insert vector > [Input help]




                                        Fig. E-120   Input help for vectors


                                        On this dialog, you can have the table on the Vector... dialog filled out auto-
                                        matically by specifying values.
                                         Tutorial, “Definition and Management of Default Time Formulas” on page E-117

                                        Default values
                                        In this area, you specify the limit values for the calculation of the table.

                                        Start Value Start value with which the table begins.
                                        The start value refers to the table column Thickness, weight, length, quantity,
                                        surface, or edge matrix on the Factor/Vector (Name) dialog. For example, for
                                        Vector Length -> Factor enter 100 mm as start value to start the calculation at
                                        100 mm.

                                        End Value End value with which the table closes.
                                        The end value refers to the table column Thickness, weight, length, quantity,
                                        surface, or edge matrix on the Factor/Vector (Name) dialog.
                                        For example, for Vector Length -> Factor enter 2000 mm as end value to end
                                        the calculation at 2000 mm.

                                        Step Size Size with which the limit value is created between start and end
                                        value.
                                        The step size refers to the table column Thickness, weight, length, quantity,
                                        surface, or edge matrix on the Factor/Vector (Name) dialog.
                                        Enter for example for a vector Vector ’Length -> Factor’ a step size of 100 mm.
                                        This means that a different value will be assigned to the vector every 100 mm,
4.50 / 01-2023




                                        e.g. 100.00 to 199.00 mm, 200.00 to 299.99 mm, etc.




                 A+W Production Capacity Planning                                                                      E-205
                 Time Master Data                                                              Software Reference




                                    Values
                                    In this area, you specify the values for the calculation of the time allowances
                                    per limit value.

                                    Start Value Value with which the time allowance for the smallest of the spec-
                                    ified limit values is calculated.
                                    The start value refers to the table column Factor on the Fac-tor/Vector (Name)
                                    dialog.
                                    Enter for example for a vector Vector ’Length -> Factor’ a start value of 1. This
                                    means that the vector will be assigned the value 1 for a length between 100
                                    mm and 199.99 mm.

                                    Step Size Value by which the calculation value per limit value is increased.
                                    The step size refers to the table column Factor on the Factor/Vector (Name)
                                    dialog.
                                    Enter for example for a vector Vector ’Length -> Factor’ a step size of 2. This
                                    means that the value of the vector will be increased by the value 2 ever 100
                                    mm, e.g. the values 1, 3, 5, etc.

                                    [OK] Saves the data.

                                    [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-206                                                         A+W Production Capacity Planning
                 Software Reference                                                                   Time Master Data




                                        Select Formula
                                        Master data > Capacity planning > Default times > Edit > Own formula




                                        Fig. E-121   Select Formula


                                        On this dialog, you can select defined formulas and insert them on the Default
                                        time formula dialog.
                                         Tutorial, “Definition and Management of Default Time Formulas” on page E-117

                                           Own formulas
                                           Additional formulas may have a massive impact on the behavior and the
                                           properties of default time formulas.
                                           Please contact A+W Software GmbH customer service if you need your
                                           own formulas or to change existing formulas!

                                        ID Formula ID.

                                        Formula Formula name.

                                        Description Description of the formula.

                                        Language Choose the language in which the formula has been written. If
                                        you choose English, for instance, you will see only the formulas that have been
                                        defined in this language.

                                        Text Search for a formula by means of its name.

                                        [OK] Saves the data.

                                        [Reject] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                E-207
                 Time Master Data                                                              Software Reference




                                    Entering a Formula Element
                                    Master data > Capacity planning > Default times > [Edit] > [Formula Editor],
                                    [New]




                                    Fig. E-122   Time formula – entering element


                                    On this dialog, you can enter an individual element for calculating a time for-
                                    mula.
                                     Tutorial, “Editor for Formula Elements” on page E-112

                                    Name Name that is displayed in the selection of formula elements.

                                    Element Type Selection of the element type.
                                    • Fixed element:
                                       Expressions without user entry, e.g. long edge. You should no longer use
                                       this setting for new definitions. It has been replaced by Free Element.
                                    • Condition:
                                       Expressions with a user input that is used if the condition is true.
                                    • Free element:
                                       Expressions for which the result is weighted with the user input (e.g. sec-
                                       onds per meter ground)
                                    • Threshold value:
                                       Expressions for which the threshold value for the condition can be set with-
                                       out changing the formula definition (e.g. quantity surcharge starting with
                                       user input)
                                    • Vector:
                                       Expressions for which a table with value pairs of minimum values and co-
                                       efficients to be used is maintained.

                                    Labeling Designation that is displayed on the Default time formula dialog.

                                    Definition Formula for the calculation for the element types Fixed element,
4.50 / 01-2023




                                    Condition, and Free element.




                 E-208                                                         A+W Production Capacity Planning
                 Software Reference                                                                 Time Master Data




                                        Input format Format of the dimension unit for the element types Threshold
                                        value and Vector:
                                        • No unit:
                                           No dimensional unit.
                                        • Thickness, Length:
                                           Millimeter, inch.
                                        • Area:
                                           Square meter, square foot.
                                        This setting guarantees that the inputs for the parameters are interpreted in
                                        the unit that is configured in A+W Production.

                                        Labeling Designation that is displayed on the Default time formula dialog be-
                                        fore the calculation value, e.g. sec. for a time value.

                                        Definition Display of the formula for an independent parameter that is select-
                                        ed for a vector or threshold value.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                               E-209
                 Time Master Data                                                                Software Reference




                                    User-defined Table Elements
                                    Master data > Capacity planning > Default times > [Edit] > [New] > <New ta-
                                    ble...>




                                    Fig. E-123   User-defined table elements


                                    On this dialog, you define a new table element for default time formulas.
                                     Tutorial, “Structure of Default Time Formulas” on page E-107

                                    Properties

                                    Name Name of the table element.

                                    Type Type of the formula element.
                                    The following options are available for New table:
                                    • Vector (one-dimensional)
                                    • Table (two-dimensional)
                                    • Cube (three-dimensional)

                                    Value 1, Value 2, Value 3 Opens the Select limit dialog where you can se-
                                    lect a value. The number of fields depends on the table type selected.
                                     “Select Limit” on page E-211

                                    Description Description of the table elements.

                                    [Delete] Deletes the selected element.

                                    [Save] Saves the data.

                                    [New] Creates a new table element.
4.50 / 01-2023




                                    [Close] Closes the dialog without saving the data.




                 E-210                                                          A+W Production Capacity Planning
                 Software Reference                                                                 Time Master Data




                                        Select Limit
                                        Master data > Capacity planning > Default times > [Edit] > [New] > <New ta-
                                        ble...> select




                                        Fig. E-124   Limits for table elements


                                        On this dialog, you can select limit values for a new table element. The table
                                        element is used for the formula for calculation of default times.
                                         “User-defined Table Elements” on page E-210

                                        [OK] Applies the data.

                                        [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                               E-211
                 Time Master Data                                                               Software Reference




                                    Time Formula Test
                                    Master data > Capacity planning > Default times > [Edit] > [Formula -test]




                                    Fig. E-125   Time formula test


                                    On this dialog, you can check formulas for time calculation. The test always
                                    affects the element selected on the Default time formula dialog. If the whole
                                    default time formula should be tested, you must select the Basic Time entry.
                                     Tutorial, “Testing Time Formulas” on page E-124

                                    Formula object

                                    Formula object (name) Graphic display of the formula objects. With a dou-
                                    ble-click, you open a dialog on which you can enter the values for the test, e.g.
                                    the lite dimensions.
                                     “Formula Object Properties” on page E-214

                                    [New] Saves a new formula object.

                                    [Load] Loads a saved formula object.

                                    [Save] Saves the changed formula object.

                                    [Add] Adds an element below the selected element.

                                    [Delete] Deletes the selected element.
4.50 / 01-2023




                 E-212                                                         A+W Production Capacity Planning
                 Software Reference                                                                     Time Master Data




                                        Diagnosis Tool

                                        Show formula You can have the formula syntax displayed.
                                        The formula syntax will not be shown.
                                        Opens the Formula (name) dialog where the syntax of the formula is shown
                                        and can be copied.
                                         “Formula (Name)” on page E-215

                                        Protocol evaluation You can create a record of the formula evaluation.
                                        The evaluation will not be recorded.
                                        The evaluation of the formula is shown on the Course of Formula Evaluation
                                        dialog.
                                         “Course of Formula Evaluation” on page E-216

                                        Result Result of the time calculation in seconds. An arrow up or down indi-
                                        cates that the result of the default time formula is higher or lower than the basic
                                        time.

                                        [Evaluate] Starts the formula analysis.
                                        Analysis always starts from the selected formula object. If you have not select-
                                        ed an element, the evaluation begins on the header.
                                        The result of the analysis is displayed in the Result field. If you have selected
                                        the Protocol Evaluation checkbox, the Course of Formula Evaluation dialog
                                        opens.
                                         “Course of Formula Evaluation” on page E-216

                                        [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                   E-213
                 Time Master Data                                                                 Software Reference




                                    Formula Object Properties
                                    Master data > Capacity planning > Default times > Edit > Formula test > Dou-
                                    ble-click on the formula object




                                    Fig. E-126    Time formula test - formula object properties


                                    On this dialog, you enter the data for the formula test, e.g. a lite with the thick-
                                    ness 4 mm and a width of 2500 mm. On this dialog, lengths and thicknesses
                                    are specified in the unit micrometers µm.
                                     Tutorial, “Time Formula Objects” on page E-116

                                    Formula Object Properties

                                    Name Name of the formula object.

                                    Type Selection of the option Part or Processing.

                                    Overview
                                    •   Property:
                                        Assigned property. In the selection list, all factors are available that you
                                        have added to the default time formula and their properties can be edited.
                                    •   Value:
                                        Value for the test calculation in question. Length and thickness specifica-
4.50 / 01-2023




                                        tions in micrometers.




                 E-214                                                           A+W Production Capacity Planning
                 Software Reference                                                                    Time Master Data




                                        [Add] Adds a new element to the Property list. The display of the properties
                                        depends on the elements that are added to the default time formula.

                                        [Delete] Deletes the selected element.

                                        [Close] Closes the dialog without saving the data.


                                        Formula (Name)
                                        Master data > Capacity planning > Default times > [Edit] > [Formula -test] >
                                        check Display Formula checkbox




                                        Fig. E-127   Formula syntax


                                        On this dialog, the formula is displayed in natural syntax in order to find errors
                                        in a default time formula.
                                         Tutorial, “Definition and Management of Default Time Formulas” on page E-117

                                        [Copy] Copies the formula e.g. to add it to an editor.

                                        [Close] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-215
                 Time Master Data                                                              Software Reference




                                    Course of Formula Evaluation
                                    Master data > Capacity planning > Default times > [Edit] > [Formula -test] >
                                    check Protocol Evaluation checkbox > [Evaluate]




                                    Fig. E-128   Course of formula evaluation


                                    This dialog displays the course of formula evaluation. This evaluation is re-
                                    quired by A+W Software GmbH support to analyze a formula calculation.
                                     Tutorial, “Definition and Management of Default Time Formulas” on page E-117

                                    [Close] Closes the dialog.
4.50 / 01-2023




                 E-216                                                          A+W Production Capacity Planning
                 Software Reference                                                                      Time Master Data




                                            Transition Times
                                            Master data > Capacity planning > Transition times




                 Fig. E-129   Transition times


                                            On this dialog, you specify transition times between (logical) machines. You
                                            can define transition times for optimal transfer and for accelerated transfers.
                                            With the specification of minimum and maximum times, you specify a time
                                            span in which the transition can take place. For the planning, the transition is
                                            always regarded from the end of a shift.
                                             Tutorial, “Transition Times” on page E-92
                                            The transition times are processed hierarchically.
                                            •    Machine x -> Machine y describes the explicit transition between two ma-
                                                 chines.
                                            •    Machine x -> All machines describes the transition at the end of machine x.
                                            •    All machines -> Machine x describes the transition at the entry to machine
                                                 x.
                                            •    All machines -> All machines describes the general transition and is eval-
                                                 uated last.
4.50 / 01-2023




                                             Tutorial, “Transition Times” on page E-92




                 A+W Production Capacity Planning                                                                    E-217
                 Time Master Data                                                                Software Reference




                                        Transition times in shifts
                                        Generally, transition times are defined in shifts. Only in exceptional cases
                                        do you use the duration in hours and minutes, e.g. for drying times.

                                    Machines
                                    •   Machine 1:
                                        Logical machine from where the transition starts.
                                        Double-click on a field to open the dialog to select a logical machine.
                                    •   Machine 2:
                                        Logical machine to which the transition is made.
                                        Double-click on a field to open the dialog to select a logical machine.
                                    •   Type:
                                        Type of transition time:
                                        – Normal:
                                            Normal transition time. It describes the optimal throughput through pro-
                                            duction, e.g. without breakdowns of personnel or machines, breakage,
                                            etc.
                                        – Rush:
                                            Reduced transition time for rush orders, e.g. without dwell times. With
                                            this time, the (virtual) costs increase. These transition times are used
                                            automatically for orders that have the priority Rush in the ERP system.
                                            These orders also use the work shifts reserved for rush orders.
                                        – Minimal:
                                            Reduced transition time for top priority orders. You may only use this
                                            setting if another reduction is technically possible. In general, this set-
                                            ting is only used if a minimum time must be adhered to, e.g. after the
                                            autoclave.
                                            Only the transition time from the Transition time 'h:m' is used.
                                        – Prohibited:
                                            Maschine 2 may not be activated after machine 1. With this setting, you
                                            can map, for example, that a machine cannot be reached without inter-
                                            nal transport.
                                    •   Transition time 'h:m':
                                        Minimal transition time in hours and minutes. This setting is used if the time
                                        is also calculated across non-working days.You can specify the minimal
                                        transition time and maximum transition time in mixed units, e.g. an optimal
                                        transition time of 2 hours and a maximum transition time of 2 shifts.
                                    •   Shifts:
                                        Minimum transition time in shifts.
                                    •   Maximum transition time 'h:m':
                                        Maximum transition time in hours and minutes. Here, a value must be
                                        specified that describes at least one weekend since the machine will oth-
                                        erwise not be used on Friday, for example.
                                    •   Maximum shifts:
                                        Maximum transition time in shifts. The value of the maximum transition time
                                        is added to the minimum transition time. With a minimum transition time of
                                        1 shift and a maximum transition time of 3 shifts, this produces a transition
4.50 / 01-2023




                                        time of 1 to 4 shifts.
                                        You can specify the minimum transition time and maximum transition time




                 E-218                                                          A+W Production Capacity Planning
                 Software Reference                                                                        Time Master Data




                                           in mixed units, e.g. a minimum transition time of 2 hours and a maximum
                                           transition time of 2 shifts.

                                           Example

                                           Transition type        Shifts       Maximum shifts    Time in shifts

                                           Normal                   2                 2                4
                                                                    2                 1                3

                                           Rush                     1                                  1

                                           Minimum                  1                                  1

                                           Tip
                                           For the transition to the last process, e.g. Packing or Dispatch, specify the
                                           longest transition time possible. This will give you greater flexibility in criti-
                                           cal situations.

                                        [New] Adds a new line in order to define a transition time.

                                        [Delete] Deletes the selected entry.

                                        [OK] Takes over the selected entry into the Default time formula dialog.

                                        [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                    E-219
                 Master Data for the Shifts                                                                  Software Reference




                                              Master Data for the Shifts
                                              In addition to the default and transition times, it is also possible to define shifts
                                              in which the work times can be defined in production per day.
                                              This section provides information on the following subjects:
                                              •   “Shifts” on page E-221
                                              •   “Shift Calendar” on page E-223
                                              •   “Shift Plan” on page E-224
                                              •   “Shift Rule” on page E-226
                                              •   “Shift Group” on page E-228
                                              •   “Machine” on page E-229
4.50 / 01-2023




                 E-220                                                                     A+W Production Capacity Planning
                 Software Reference                                                           Master Data for the Shifts




                                        Shifts
                                        Master data > Capacity planning > Shifts
                                        The following chapters deal with the Shifts dialog:
                                        •   “Shift Calendar” on page E-223
                                        •   “Shift Plan” on page E-224
                                        •   “Shift Rule” on page E-226
                                        •   “Shift Group” on page E-228
                                        •   “Machine” on page E-229




                 Fig. E-130   Shifts


                                        Manage shift plans on this dialog.

                                            Changing of shifts
                                            Changing shifts is a major operation in capacity planning. Check in the Pro-
                                            duction Monitor whether changes are implemented correctly in work shifts.
                                            Orders already scheduled will not be rescheduled automatically. Therefore,
                                            change shifts only so that they only become available at a time when no
                                            orders are scheduled.
                                            For last-minute changes, there are various functions available in the Pro-
                                            duction Monitor. In case of questions, please contactA+W Software GmbH
                                            customer service.
4.50 / 01-2023




                                         Tutorial, “Shifts” on page E-68




                 A+W Production Capacity Planning                                                                E-221
                 Master Data for the Shifts                                                             Software Reference




                                              Shift editor
                                              In the Shift editor area, the calendar and shift plans are displayed. Using the
                                              context menu or the buttons, you can open the various views for the definition
                                              of the shift plans:
                                              •   Shift Calendar
                                              •   Shift Plan
                                              •   Shift Rule
                                              •   Shift Group
                                              •   Machine

                                              [New] Opens the Shift calendar view in order to define a new calendar.

                                              [Delete] Deletes the selected entry.

                                              [Apply] Saves the data.

                                              [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-222                                                                  A+W Production Capacity Planning
                 Software Reference                                                                Master Data for the Shifts




                                            Shift Calendar
                                            Master data > Capacity planning > Shifts > Calendar




                 Fig. E-131   Shifts – calendar


                                            In this view of the dialog, you define the non-working days.
                                             Tutorial, “Definition of non-working Days” on page E-71

                                            Shift calendar Specification of the non-working days, for example, holidays.

                                            Day Date of the non-working day.

                                            Comment Description of the non-working day, e.g. Christmas day.

                                            [New] Adds a new line to the shift calendar in order to define a non-working
                                            day.
                                            Use the selection list to create a new shift plan.
                                             Shift Plan

                                            [Delete] Deletes the selected day from the shift calendar.

                                            [Apply] Saves the data.

                                            [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                     E-223
                 Master Data for the Shifts                                                              Software Reference




                                              Shift Plan
                                              Master data > Capacity planning > Shifts > Shift plan




                 Fig. E-132   Shifts, shift plan


                                              In this view of the dialog, you manage the shift plans with which you define the
                                              shifts.
                                               Tutorial, “Create a Shift Plan” on page E-74

                                              Shift plan
                                              In this area, you create and manage a shift plan, e.g. a two-shift plan or a
                                              three-shift plan.

                                              ID ID of the shift plan.

                                              Name Freely selectable name of the shift plan.

                                              Active You can specify whether the shift plan can be used for the planning of
                                              weekly campaigns.
                                              The shift plan is available for Weekly dates. It cannot be selected on the
                                              Campaigns dialog.
                                              The shift plan is available for Weekly dates.
4.50 / 01-2023




                                              Valid from Specification of the date starting on which the shift plan is valid.
                                              This way, you can set up the shift plan without making the shift available im-
                                              mediately, e.g. for special shifts on a weekend.


                 E-224                                                                    A+W Production Capacity Planning
                 Software Reference                                                            Master Data for the Shifts




                                        Generate shifts
                                        By selecting this option, you specify which calendar is used for the shift plan:
                                        •   Use own shift calendar:
                                            Uses the calendar you have defined in the shifts calendar.
                                             “Shift Calendar” on page E-223
                                        •   Use calendar from ERP system:
                                            Imports a calendar from an ERP system, e.g. from A+W Business.

                                        From ... to Specification of the start and end date. Shifts according to this
                                        shift plan will only be generated in the Production Monitor for the specified time
                                        period.

                                        [Create] Creates a new shift in the Production Monitor with the new data that
                                        you have entered.
                                        The button is only active if you have assigned a shift rule and a shift group with
                                        machines.

                                        [New] Creates a new shift plan.
                                        The list box is used to create a new shift rule.
                                         Shift Rule

                                        [Delete] Deletes a selected shift plan.

                                        [Apply] Saves the data.

                                        [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-225
                 Master Data for the Shifts                                                               Software Reference




                                              Shift Rule
                                              Master data > Capacity planning > Shifts > Shift rule




                 Fig. E-133   Shifts – Shift rule


                                              In this view of the dialog, you manage the shift rules of a shift plan.
                                               Tutorial, “Defining a Shift Rule” on page E-77

                                              Shift rule
                                              Shift rules apply for an individual shift plan. You can assign a shift group to
                                              each shift rule.

                                              Name Freely definable name of the shift rule, e.g. Early shift normal.

                                              Start of shift, End of shift Specification of the time at which the shift begins
                                              and ends.

                                              Capacity Display of the capacity of the shift in hours. This is calculated from
                                              the shift beginning and shift end.

                                              Shift number Input of the shift number.
4.50 / 01-2023




                 E-226                                                                     A+W Production Capacity Planning
                 Software Reference                                                            Master Data for the Shifts




                                        Days Specification of the weekdays on which the shift can be worked.
                                         The shift is not created.
                                         The shift can be created in the Production Monitor.

                                        Generate shifts
                                        By selecting this option, you specify which calendar is used for the shift plan:
                                        •   Use own shift calendar:
                                            Uses the calendar you have defined in the shifts calendar.
                                             “Shift Calendar” on page E-223
                                        •   Use calendar from ERP system:
                                            Imports a calendar from an ERP system, e.g. from A+W Business.

                                        From ... to Specification of the start and end date. Shifts according to this
                                        shift plan will only be generated in the Production Monitor for the specified time
                                        period.

                                        [Delete] Deletes the selected shift rule with all assigned machines. This way,
                                        the associated shifts are deleted from the Production Monitor.

                                        [Create] Creates shifts in the Production Monitor with the new data that you
                                        have entered.
                                        The button is only active if you have assigned a shift rule and a shift group with
                                        machines.

                                        [New] Creates a new shift rule. The list box is not used at present.

                                        [Delete] Deletes a selected shift rule.

                                        [Apply] Saves the data.

                                        [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                  E-227
                 Master Data for the Shifts                                                                Software Reference




                                              Shift Group
                                              Master data > Capacity planning > Shifts > Shift group




                 Fig. E-134   Shifts – Edit shift group


                                              In this view of the dialog, you assign the registration points to a shift group.
                                              One shift group can be created per shift rule.
                                               Tutorial, “Creating a Shift Group” on page E-82

                                              Edit shift group

                                              Name of Shift Group Name of the shift group to which the registration points
                                              are assigned.

                                              Registration Point Number Registration point number.

                                              Name Name of the registration point.

                                              Shift group Shift group that has been assigned to the registration point for
                                              the current shift plan. You can select another shift group.

                                              [New] Creates a new shift group. Each shift rule can only be assigned one
                                              shift group.
4.50 / 01-2023




                                              [Delete] Deletes a selected shift group.




                 E-228                                                                    A+W Production Capacity Planning
                 Software Reference                                                             Master Data for the Shifts




                                           [Apply] Saves the data.

                                           [Quit] Closes the dialog without saving the data.


                                           Machine
                                           Master data > Capacity planning > Shifts > Shift group > Machine




                 Fig. E-135   Shifts – Machine


                                           In this view of the dialog, you assign the logical machines to a registration
                                           point.
                                            Tutorial, “Creating a Shift Group” on page E-82

                                           Registration point
                                           Properties of the selected registration point and the logical machines assigned
                                           to the registration point.

                                           Number (number) ID of the machine.

                                           Name Machine name.

                                           Barcode Barcode of the machine.
4.50 / 01-2023




                                           Machines Logical machines assigned to the registration point.




                 A+W Production Capacity Planning                                                                   E-229
                 Master Data for the Shifts                                                          Software Reference




                                              [Delete] Deletes the selected logical machine.

                                              [Apply] Saves the data.

                                              [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-230                                                                 A+W Production Capacity Planning
                 Software Reference                                                              Machines and Costs




                                        Machines and Costs
                                        Machines can be arranged in groups to help planning the available times. The
                                        costs are also stored on the machines.
                                        This section provides information on the following subjects:
                                        •   “Cost Calculation” on page E-232
                                        •   “Machinery Groups” on page E-234
                                        •   “Load Distribution” on page E-235
4.50 / 01-2023




                 A+W Production Capacity Planning                                                            E-231
                 Machines and Costs                                                               Software Reference




                                      Cost Calculation
                                      Master data > Capacity planning > Cost calculation




                                      Fig. E-136   Cost calculation


                                      On this dialog, you specify costs that arise on logical machines.
                                      If your PPS- and ERP systems, e.g. A+W Enterprise and A+W Business, have
                                      been completely set up, the costs will be reported back to the ERP system.
                                       Tutorial, “Cost Calculation” on page E-87
4.50 / 01-2023




                 E-232                                                              A+W Production Capacity Planning
                 Software Reference                                                                 Machines and Costs




                                        Costs
                                        In the overview, all machines defined are displayed.
                                        •   Machine:
                                            Number and name of the physical machine for which the costs are defined.
                                            A double-click opens a dialog to select a machine.
                                        •   Log. Machine:
                                            Assigned logical machine for which the costs are defined.
                                            A double-click opens a dialog to select a logical machine.
                                        •   Labor Costs:
                                            Labor costs of the logical machine in the local currency.
                                        •   Machine Costs:
                                            Machine costs for the logical machine in the local currency.
                                        •   Other Costs:
                                            Other costs of the logical machine in the local currency. With these costs,
                                            for example, you can consider that additional protective clothing is required
                                            on a machine and its costs have to be considered.
                                        •   Comment:
                                            Comments about the logical machine.

                                        [New] Adds a new line to create additional machine costs.

                                        [Delete] Deletes the selected entry.

                                        [OK] Takes over the selected entry into the Default time formula dialog.

                                        [Quit] Closes the dialog without saving the data.
4.50 / 01-2023




                 A+W Production Capacity Planning                                                                 E-233
                 Machines and Costs                                                              Software Reference




                                      Machinery Groups
                                      Master data > Capacity planning > Machinery groups




                                      Fig. E-137   Machinery groups


                                      On this dialog, you can combine machines into groups and assign a number
                                      of people. This way, there is a specified capacity for the entire machine group,
                                      e.g. for work areas such as cutting, IG, and dispatch.
                                      Machines can be arranged in a machinery group only if the shifts of all ma-
                                      chines in the group match.
                                      When a machine is added to a machinery group, it automatically becomes a
                                      bottleneck machine. The overload settings for the logical machine will be
                                      adapted to the overload settings of all logical machines in the group.
                                       Tutorial, “Machinery Groups” on page E-131

                                      Machinery groups

                                      Group List of defined machinery groups.

                                      Staff Number of staff members who work on the respective machinery group.
4.50 / 01-2023




                 E-234                                                          A+W Production Capacity Planning
                 Software Reference                                                                Machines and Costs




                                        Machines for group
                                        The field on the left lists the logical machines that can be added to a selected
                                        machinery group. The list on the right shows the logical machines that have
                                        been added to the machinery group.

                                        [Allocate] Moves a selected element to the other side.

                                        [New] Opens a dialog to create a new machine group.

                                        [Delete] Deletes the selected entry.

                                        [OK] Saves the data.

                                        [Quit] Closes the dialog without saving the data.


                                        Load Distribution
                                        Master data > Capacity Planning > Load Distribution




                                        Fig. E-138   Load distribution


                                        The Load Distribution dialog defines the loads of the logical machines as a
                                        percentage of the physical machines. If two logical machines have been de-
                                        fined for a machine, the 100% of the machine load can be distributed to the
                                        logical machines, e.g. 50% each.
                                        You use load distribution to guarantee that a machine holds free a guaranteed
4.50 / 01-2023




                                        minimum capacity for special tasks, e.g. for shape cutting. If the capacity held
                                        free is not used for shapes, rectangles can also be processed. This load dis-



                 A+W Production Capacity Planning                                                                E-235
                 Machines and Costs                                                             Software Reference




                                      tribution is only possible and makes sense for machines that are defined as
                                      bottleneck machines.
                                       Tutorial, “Load Distribution” on page E-137

                                      Load Distribution

                                      Physical machines Choose the machines to edit the load distribution.

                                      Enable check The load distribution is locked to prevent accidental changes.
                                      The load distribution of the logical machines on the list cannot be edited.
                                      The load distribution of the logical machines on the list can be edited.

                                      [OK] Saves the data.

                                      [Cancel] Closes the dialog without saving the data.
4.50 / 01-2023




                 E-236                                                            A+W Production Capacity Planning
Capacity Planning             E

                    Section Index




                A+W Production
                 Section Index                                                        Index: Capacity Planning




                 Index: Capacity Planning
                 A                                              Creating work shifts E-77
                 Action for BOM configuration E-168             Creation of Processings E-193
                 Add elements E-203                             Creation of processings
                 Adjust shifts E-160                            – Add condition E-195
                 Alternative machines E-18                      – Sequence E-194
                 Asynchronous processing E-178
                 Automatic rescheduling E-17                    D
                                                                Date optimization
                 B                                              – rules E-15
                 BOM                                            Dates
                 – element chains E-16                          – campaigns E-44
                 BOM configuration E-167                        – creating a campaign E-47
                 Bottleneck                                     – creating campaign E-49
                 – machine E-29                                 Default Time Formula E-199
                 – work shift E-27                              Default time formula E-107, E-112
                                                                – Add elements E-203
                                                                – Calculation sequence E-201
                 C
                                                                – calculation sequence E-111
                 Calculation sequence E-201
                                                                – condition for arcs E-114
                 – default time formula E-111
                                                                – condition for shape E-115
                 Calendar
                                                                – condition for threshold E-115
                 – creating non-working days E-71
                                                                – Copy formula E-215
                 – deleting non-working days E-73
                                                                – creating vector E-121
                 – editing non-working days E-72
                                                                – defining E-118
                 Campaign
                                                                – Enter time formula element E-208
                 – creating E-46
                                                                – example E-113
                 – creating individual date E-47
                                                                – Factors E-204
                 – creating individual dates E-47
                                                                – factors E-108
                 – creating weekly date E-49
                                                                – fixed elements E-108
                 – delete date E-51
                                                                – Formula E-215
                 – deleting E-52
                                                                – Formula evaluation process E-216
                 – disable E-52
                                                                – Formula object properties E-212, E-214
                 – edit E-51
                                                                – Input help for vectors E-110, E-205
                 Campaign days E-184
                                                                – Limit for table E-211
                 Campaigns E-183
                                                                – Select formula E-207
                 – Campaign days E-184
                                                                – Show formula E-215
                 – Individual dates E-183
                                                                – table E-109
                 – individual dates, weekly dates E-44
                                                                – test time formula E-124
                 – scheduling E-46
                                                                – time formula object E-116
                 – Weekly dates E-185
                                                                – Time formula test E-212
                 Changes to scheduled orders E-179
                                                                – User-defined table elements E-210
                 Cost calculation E-232
                                                                – Vectors E-204
                 – definition E-88
                                                                – vectors E-109
                 Costs E-232
                                                                Default time formulas
                 – creating E-89
                                                                – copy syntax E-129
                 – deleting E-91
                                                                – deleting E-123
4.50 / 01-2023




                 – edit E-90
                                                                – test calculation E-125
                 Create new filter (Production monitor) E-158
                                                                – testing E-124
                 Creating individual dates in campaigns E-47
                                                                – time surcharges E-110


                 A+W Production Capacity Planning                                                      E-239
                 Index: Capacity Planning                                                             Section Index




                 Default Times E-197                               – setting display type E-32
                 Default times                                     – work shift E-28
                 – definition E-106                                Machine costs
                 Defective orders E-177                            – edit costs E-90
                 Deleting expired reservation E-60                 Machine paths
                 Dwell time see transition times                   – alternative machines E-18
                                                                   – processing chains E-17
                 E                                                 Machine see also logical machine
                 Error                                             Machine shifts E-147
                 – scheduling E-40                                 Machinery group
                 Expired reservations    E-186                     – creating E-133
                 Export                                            – deleting E-135
                 – Work plan E-33                                  – editing E-135
                                                                   Machinery groups E-234
                                                                   – definition E-132
                 F                                                 Machines
                 Factors E-204                                     – Display in Production monitor E-151
                 Factors (default time formula) E-108              – display in Production Monitor E-30
                 Fixed elements (default time formula) E-108       Master data
                 formula editor E-112                              – Capacity planning E-14
                 Formula evaluation E-216                          – Machine allocation E-14
                 Formula evaluation process E-216                  – protection, data back-up E-67
                 Formula object properties E-214                   Matrix for transition times E-100
                 formula structure E-107
                                                                   N
                 H                                                 Non-working days
                 High-priority order   E-171                       – creating E-71
                                                                   – deleting E-73
                 I                                                 – editing E-72
                 Individual dates (campaign) E-183
                 Individual filters (Production monitor)   E-157   O
                 Input help for vectors E-205                      Order
                                                                   – post-processing scheduling    E-41
                 L                                                 – rescheduling E-36
                 Load Distribution E-235                           – reservation E-54
                 Load distribution                                 – Schedule E-35
                 – definition E-138                                – Select (Production monitor)   E-155
                 – deleting E-142
                 – editing E-141                                   P
                 – set-up E-139                                    Post-processing of scheduling E-174
                 Logical machine                                   – Changes to scheduled orders E-179
                 – create costs E-89                               – Defective orders E-177
                 – default time E-106                              Processing
                 – Shift group E-229                               – adding E-64
                 Logical machine see also machine                  – creating E-64
                                                                   – rescheduling E-37
                 M                                                 – resolving E-65
                 Machine                                           Processing chains E-17
4.50 / 01-2023




                 – bottleneck E-29                                 Processing creation E-63
                 – creating costs E-89                             – removing processing E-65
                 – deleting costs E-91                             Processing time see default times
                 – rescheduling E-36                               Processings


                 E-240                                                          A+W Production Capacity Planning
                 Section Index                                                         Index: Capacity Planning




                 – rescheduling E-38                           Rules
                 – Split items E-180                           – date optimization E-15
                 Production dates                              – scheduling E-16
                 – evaluation E-19
                 Production Monitor                            S
                 – adjustments E-23                            Scheduling E-16, E-146, E-166
                 – detailed view E-23                          – Asynchronous processing E-178
                 – display machines E-30                       – BOM E-16
                 – set display E-31                            – BOM configuration E-167
                 Production monitor E-21, E-147                – campaigns E-46
                 – Adjust shifts E-160                         – Changes to scheduled orders E-179
                 – Create new filter E-158                     – Defective orders E-177
                 – creating work shifts E-77                   – Error E-174
                 – Displayed machines E-151                    – error E-40
                 – Filter by batch E-156                       – machine paths E-17
                 – Filter by order E-155                       – post-processing E-41
                 – Individual filters E-157                    – Processing creation E-63
                 – Machine E-159                               – production dates E-18
                 – Presentation of shifts E-152                – Schedule orders E-35
                 – Select batch E-155                          – Split items E-180
                 – Select order (Production monitor)   E-155   – transition times E-94
                 – Settings E-152                              Scheduling rules E-14
                 – Shift properties E-161                      Select batch E-155
                                                               Select customer for reservation Reservation
                 R                                             – Select customer E-190
                 Rescheduling E-169, E-173                     Select formula E-207
                 – high-priority order E-169                   Select project (reservation) E-191
                 – lock date E-169                             Sequence (creation of processings) E-194
                 – machine E-36                                Shift
                 – order E-36                                  – special case for change E-97
                 – Post-processing of scheduling E-174         Shift calendar E-223
                 – processing E-37                             Shift change special case E-97
                 – Receipt of goods E-171                      Shift group E-228
                 – Rescheduling E-173                          – creating E-82
                 Reservation                                   – deleting E-86
                 – capacities E-54                             – editing E-85
                 – configuration E-53                          Shift plan E-224
                 – creating E-56                               – creating E-75
                 – deleting E-59                               – deleting E-77
                 – deleting expired reservation E-60           – editing E-76
                 – editing E-58                                Shift plans E-69
                 – expired E-55                                Shift properties E-161
                 – order E-54                                  Shift reservations E-188
                 – Per shift E-188                             Shift rule E-226
                 – Select project E-191                        – creating E-78
                 Reservation for Machine E-189                 – deleting E-81
                 Reservations E-187                            – editing E-80
                 – by day, by week E-188                       Shifts E-221
                 – Expired reservations E-186                  – Logical machine E-229
4.50 / 01-2023




                 – Per customer E-188                          – Shift calendar E-223
                 – Per machine E-188                           – Shift group E-228
                 Reserve capacity E-54                         – shift group E-82



                 A+W Production Capacity Planning                                                        E-241
                 Index: Capacity Planning                                                       Section Index




                 – Shift plan E-224                             – extending, shortening E-26
                 – shift plan E-76                              – locking E-25
                 – Shift rule E-226                             – machine E-28
                 – shift rule E-80                              – reserving E-26
                 – Transition time E-218                        – setting up additional E-24
                 Split items E-180                              Work shifts E-21, E-147
                 Surcharges on default time    E-110            – display E-31

                 T
                 table (default time formula) E-109
                 Test time formula E-124
                 Threshold value (default time formula) E-115
                 Time formula element E-208
                 Time formula object E-116
                 Time formula test E-124, E-212
                 – Formula object properties E-212, E-214
                 Transition
                 – hours E-96
                 – in hours or shift E-94
                 – shifts E-95
                 Transition time
                 – creating E-101
                 – deleting E-103
                 – editing E-103
                 – hours E-96
                 – shifts E-95
                 – special case E-97
                 – type E-99
                 Transition Times E-92
                 Transition times E-217
                 – definition E-98
                 – matrix E-100
                 – scheduling E-94
                 – Shifts E-218

                 U
                 User-defined table elements    E-210

                 V
                 Vectors E-204
                 – input help E-110
                 – using in default time formulas E-121
                 Vectors (default time formula) E-109

                 W
                 Weekly dates (campaign)      E-185
                 Work plan
                 – Export E-33
4.50 / 01-2023




                 Work shift
                 – adjustments E-23
                 – bottleneck E-27



                 E-242                                                      A+W Production Capacity Planning

