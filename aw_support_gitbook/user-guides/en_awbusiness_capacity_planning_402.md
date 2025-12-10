---
description: "EN AWBusiness Capacity Planning 4.02"
---



# EN AWBusiness Capacity Planning 4.02

Capacity Planning          H




                            English




              A+W Business Pro
                                                                                                                  Introduction




                                        Introduction
                                        This part of the documentation contains editorial notes.


                                        Revision Overview
                                        Part              Description
                                        Version/Date

                                        1.00/12-2003      Initial creation

                                        1.01/08-2008      Spelling and grammar corrections, graphic tables converted,
                                                          figures and part numbering adjusted

                                        1.02/09-2010      Layout adjusted to document concept 2010

                                        2.00/05-2012      Initial creation of the tutorial, software reference completely
                                                          reworked

                                        3.00/08-2013      Adjustment of the ALFAK documentation to A+W Business Pro.

                                        4.00/04-2014      Complete revision.

                                        4.01/04-2015      Adjustment A+W Business Pro.

                                        4.02/01-2017      Product and company names adjusted.



                                        Editorial
                                        The editorial contains information about the following topics:
                                        •   Notes on this document
                                        •   Copyrights
                                        •   Trademarks
                                        •   Contacts

                                        Notes on this document
                                        This publication is conceived exclusively for end users of A+W Business Pro.
                                        This documentation and the software it describes is only distributed with a li-
                                        cense and may only be used and copied according to this license. The content
                                        of the documentation serves only as information and can be changed without
                                        prior notice at any time. The greatest care was used in compiling the texts and
                                        figures. However it is not possible to exclude errors completely. A+W Software
                                        GmbH assumes no liability for errors or imprecise statements unless these
                                        can be traced back to intentional or negligent actions.
                                        This document describes the complete stage of expansion of A+W Business
                                        Pro.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                         H-3
                 Introduction




                                Copyrights
                                © 2017, A+W Software GmbH, all rights reserved, also those for reprinting, the
                                making of copies and translation.
                                The documentation may only be copied whole or in part, stored in an archiving
                                system or transmitted in any other form in accordance with the license agree-
                                ment. Without the prior written permission of A+W Software GmbH, the docu-
                                mentation may not be transmitted electronically, by recording or in any other
                                form.

                                Trademarks
                                All hardware and software designations mentioned in the documentation can
                                also be registered trademarks or other industrial property rights of third parties.
                                The property rights of third parties must be observed.

                                Contacts
                                A+W Software GmbH

                                Am Pfahlgraben 4 - 10

                                D-35415 Pohlheim

                                Germany

                                    +49 6404 2051 0

                                    +6404 2051 877

                                Zentrale@a-w.com

                                http://www.a-w.com
4.02 / 01-2017




                 H-4                                                     A+W Business Pro Capacity Planning
                                                                                                                                                        Contents




                                        Contents
                                        Introduction ............................................................................................................. H-3
                                          Revision Overview ............................................................................................... H-3
                                          Editorial ............................................................................................................... H-3

                                        Tutorial                                                                                                             H-7
                                        Overview ................................................................................................................. H-9
                                         Documentation .................................................................................................. H-10
                                           Tutorial Structure ........................................................................................... H-10
                                           Display Conventions ...................................................................................... H-11
                                         Menu Overview ................................................................................................. H-12
                                           Capacity Planning Module ............................................................................. H-12
                                           Production Module ......................................................................................... H-14
                                         Basic Principles of Capacity Planning ............................................................... H-16
                                           Using Capacity Planning ................................................................................ H-17
                                        Master Data .......................................................................................................... H-18
                                         Machines and Production Areas ....................................................................... H-20
                                           Machine Types and Machines ....................................................................... H-21
                                           Work Types .................................................................................................... H-25
                                           Production Areas (Work Centers) .................................................................. H-27
                                           Define a Production Area ............................................................................... H-28
                                           Enter a Machine ............................................................................................. H-29
                                           Exercises ....................................................................................................... H-33
                                         Shift and Working Hours ................................................................................... H-34
                                           Working Hours ............................................................................................... H-35
                                           Workdays and Shifts ...................................................................................... H-35
                                           Maximum Capacity per Day ........................................................................... H-37
                                           Work Units ..................................................................................................... H-39
                                           Default Settings for Shift and Capacities ....................................................... H-43
                                           Adjust Calendar ............................................................................................. H-45
                                           Exercises ....................................................................................................... H-51
                                         Default Times .................................................................................................... H-52
                                           Basic Components of Time Planning ............................................................. H-53
                                           Default Times ................................................................................................. H-55
                                           Special Times ................................................................................................ H-58
                                           Work Types and Time Surcharges ................................................................ H-59
                                           Case Study IG and Shape ............................................................................. H-60
                                           Calculation Sequence for Surcharges and Factors ....................................... H-63
                                           Transition Matrix and Transition Times .......................................................... H-64
                                           Setup Times ................................................................................................... H-70
                                           Time Factors for Series .................................................................................. H-71
                                           Define Default Times ..................................................................................... H-72
                                           Create Special Time ...................................................................................... H-76
                                           Exercises ....................................................................................................... H-80
                                         Selection of Machines ....................................................................................... H-81
                                           Priorities ......................................................................................................... H-82
                                           Restrictions .................................................................................................... H-83
                                           Priority vs. Restriction .................................................................................... H-84
                                           Automatic Scheduling .................................................................................... H-85
                                           Machine Selection for Alternative Work Types .............................................. H-89
                                           Locks .............................................................................................................. H-90
4.02 / 01-2017




                                           Define Production Line ................................................................................... H-93
                                           Default Settings for Machine Selection .......................................................... H-95




                 A+W Business Pro Capacity Planning                                                                                                            H-5
                 Contents




                             Allocate the A+W Business Pro Master Data .................................................... H-97
                               Production Sequence ..................................................................................... H-98
                               Combined Product Type, Combined Product Class .................................... H-101
                               Define Allocation .......................................................................................... H-103
                               Exercises ..................................................................................................... H-106
                            Capacity Planning ............................................................................................... H-107
                             Scheduling Orders ........................................................................................... H-108
                               Date Calculation ........................................................................................... H-109
                               Scheduling ................................................................................................... H-113
                               Capacity Problems ....................................................................................... H-114
                               Default Settings for Automatic Scheduling ................................................... H-118
                               Schedule Order ............................................................................................ H-119
                               Solve Capacity Problem ............................................................................... H-126
                               Exercises ..................................................................................................... H-130
                             Production ....................................................................................................... H-131
                               Reports about Production Status ................................................................. H-132
                               Registration Points ....................................................................................... H-134
                               Status Messages ......................................................................................... H-136
                               Completion Report ....................................................................................... H-138
                               Remaining Quantities from Previous Day .................................................... H-139
                               Breakage Report .......................................................................................... H-140
                               Print Production Papers ............................................................................... H-141
                               Report manually Order completed ............................................................... H-143
                               Manual Breakage Report ............................................................................. H-146
                               Check Production Status ............................................................................. H-148
                               Catch up on Completion Reports ................................................................. H-150
                               Exercises ..................................................................................................... H-152
                             Production Costs ............................................................................................. H-153
                               Time Costs ................................................................................................... H-154
                               Cost Centres ................................................................................................ H-156
                               Cost Calculation in Orders ........................................................................... H-159
                               Cost calculation for Quotations .................................................................... H-159
                               Exercises ..................................................................................................... H-160
                             Control Station ................................................................................................. H-161
                               Concept of the Control Station ..................................................................... H-162
                               Control Station – Order ............................................................................... H-164
                               Control Station – Machine ............................................................................ H-165
                               Postpone Scheduling for single Order ......................................................... H-166
                               Change Machine .......................................................................................... H-171
                               Exercises ..................................................................................................... H-173
4.02 / 01-2017




                 H-6                                                                    A+W Business Pro Capacity Planning
Capacity Planning           H

                        Tutorial




              A+W Business Pro
                 Tutorial                                                                                          Overview




                                        Overview
                                        The tutorial for the Capacity planning module focuses on the basic principles
                                        of planning production capacities in A+W Business Pro. The tutorial is based
                                        on the knowledge of master data and documents.

                                            Functions depend on the enabled modules
                                            Please note that the various functions are only available if the correspond-
                                            ing modules and interfaces are installed and enabled.

                                            If you find functions in this description that are not available in your version,
                                            please contact A+W Software GmbH.

                                        Subjects
                                        This tutorial includes the following subjects:
                                        •   Master Data
                                        •   Capacity Planning

                                        Required knowledge
                                        The tutorial is meant for those who plan capacities in A+W Business Pro and
                                        thus monitor the utilization of the machines. Participants must be familiar with
                                        the concept of master data in A+W Business Pro and the Documents module.
                                        Knowledge of the Production and Stock Management modules is advanta-
                                        geous.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                     H-9
                 Overview                                                                               Tutorial




                            Documentation
                            The following documents are available for the Capacity planning module:

                            Format                   Scope

                            Handout                  Printout of the tutorial for the training

                            PDF                      Complete documentation
                                                     • Tutorial
                                                     • Software reference
                                                     • Index

                            Online help <F1>         Context-sensitive dialog help of A+W Business Pro
                                                     software reference and tutorial


                            Tutorial Structure
                            The tutorial consists of subjects with several training modules each. Each
                            training module consists of the following elements:

                            Overview                 Each training module starts with an overview of the
                                                     major topics:
                                                     • Objectives: What shall be conveyed?
                                                     • Benefit: What can this knowledge be used for?
                                                     • Maxims: Which correlations are to be remembered?

                            Concepts                 First, the concepts and terms of the corresponding
                                                     training module will be explained. This is followed by
                                                     examples and instructions.

                            Exercises                For some of the training modules, exercises with certain
                                                     tasks and suggested solutions are available.

                            Cross-references         At the end of each training module there is a section
                                                     with cross references pointing out additional information
                                                     in the software reference and in other sections.
                                                     This will help you to extend your newly acquired
                                                     knowledge.
4.02 / 01-2017




                 H-10                                                A+W Business Pro Capacity Planning
                 Tutorial                                                                                           Overview




                                        Display Conventions
                                        Certain parts of sentences are specially marked. The meanings are:

                                        Italic                       marks character strings describing the software
                                                                     elements, e.g. the Stock info dialog.

                                        Bold                         marks character strings to be entered via keyboard, e.g.:
                                                                     Enter the value 0.

                                        >                            The so-called breadcrumb trail shows how to open a
                                                                     dialog, e.g. Production > Capacity planning > Control
                                                                     station.

                                        []                           Square brackets mark buttons in a dialog, e.g. [OK] to
                                                                     save the data.

                                        <>                           Angle brackets refer to keys or shortcuts on the
                                                                     keyboard, e.g. <F1> is used to open the online help.


                                        Reading instructions
                                        The contents of a training module are based on the knowledge conveyed in the
                                        previous module. We therefore recommend not to skip any training modules.
                                        If you are already familiar with a subject you should at least read the summary at the
                                        start of a training module to bring the main details to mind.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                      H-11
                 Overview                                                                                         Tutorial




                                         Menu Overview
                                         The capacity planning module in A+W Business Pro consists of two areas: the
                                         setup of capacity planning and the planning and monitoring of capacities. The
                                         associated dialogs are in the Capacity planning and Production modules. Both
                                         modules are introduced briefly.


                                         Capacity Planning Module
                                         In the Capacity planning module, you set up the master data and other speci-
                                         fications for planning the capacities.




                 Fig. H-1   Capacity planning module


                                         Master Data
                                         The Master Data menu is divided into three submenus:
                                         •   General:
                                             In this group, you set up general data, e.g. machine types, work types, tran-
                                             sition times.
4.02 / 01-2017




                                              Software Reference, “General” on page H-185




                 H-12                                                            A+W Business Pro Capacity Planning
                 Tutorial                                                                                       Overview




                                        •   Organisation:
                                            In this group you set up the master data for operational organization, e.g.
                                            production areas, machines, calendar, and restrictions.
                                             Software Reference, “Organisation” on page H-194
                                        •   Default Times:
                                            In this group you set up the data for calculating the production times, e.g.
                                            default times and special times.
                                             Software Reference, “Default Times” on page H-216

                                        Allocation
                                        Here you allocate e.g. products or product groups (PGRs) to work types. For
                                        some work types, you define a factor for calculating the times if a special effort
                                        makes this necessary, e.g. for the production of shapes.
                                         Software Reference, “Allocation” on page H-229

                                        Lock
                                        Here you define which machines must not be used, e.g. if an order includes
                                        certain products or product groups.
                                         Software Reference, “Lock” on page H-246

                                        Overview
                                        Here you can create overviews of the utilization of machines and production
                                        areas.
                                         Software Reference, “Overviews” on page H-257
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-13
                 Overview                                                                                      Tutorial




                                        Production Module
                                        In the Production module, you schedule orders in capacity planning and mon-
                                        itor the reports from production.
                                        In this module, you also find the program modules for transferring orders to
                                        production. These are described in the Production part.




                 Fig. H-2   Capacity planning menu


                                        Scheduling
                                        On the Scheduling menu, you find the following dialogs:
                                        •   Number Manager:
                                            In the number manager, you collect orders for manual scheduling.
                                        •   Book NM:
                                            Use this dialog to schedule the orders.
                                        •   Book order:
                                            Use this dialog to schedule an individual order.
                                        •   Machine Failure:
4.02 / 01-2017




                                            Use this dialog to lock a machine for scheduling.
                                         Software Reference, “Scheduling” on page H-268




                 H-14                                                          A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Overview




                                        Completion report
                                        On the Completion report menu, you find the following dialogs:
                                        •   Date:
                                            On this dialog, you report orders on a machine as completed.
                                        •   Batch:
                                            On this dialog, you report orders completed per batch.
                                        •   Manually:
                                            On this dialog, you report orders completed in part or completely.
                                         Software Reference, “Production Reports” on page H-291

                                        Production lists
                                        Here you can list the quantities to be produced per machine.
                                         Software Reference, “Production Reports” on page H-291

                                        Production level orders
                                        Here you can check the current status of production per order and catch up on
                                        any omitted completion reports.
                                         Software Reference, “Production Level Orders” on page H-307

                                        Control station
                                        Here you check the utilization of machines and reschedule orders if necessary
                                        by changing allocated machines, shifts, production or delivery dates.
                                         Software Reference, “Control Station” on page H-325
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-15
                 Overview                                                                                                         Tutorial




                                                  Basic Principles of Capacity Planning
                                                  With capacity planning, you can pre-plan the utilization of your production ca-
                                                  pacity and calculate production and time costs. The planning data will help you
                                                  to detect capacity bottlenecks well in advance. In this case you can intervene
                                                  in the planning and make amendments where necessary.
                                                  To do this, you must enter the master data for capacity planning and coordi-
                                                  nate them so that they reflect the flows in your production. The following figure
                                                  shows the interaction of these master data using as an example the settings
                                                  from which the dates for the start of the production are calculated.


                                                            Master data for capacity planning                      A+W Business Pro
                                                                                                                   product master data


                                                                    Machine types




                               Production areas                        Machines                  Work types
                                (work centers)




                        Dwell days, transition matrix              Calendar                 Default times               Allocate
                                (prod. areas)                                                                     production sequence
                              transition times




                                                                  Calculation: date of production start



                 Fig. H-3        Interaction of the master data of capacity planning


                                                  In this overview, you see how e.g. machines are used for capacity planning:
                                                  •     For the individual work types, the default times defined per machine are
                                                        used to calculate the (free) capacity and the required time for an order item.
                                                  •     Per machine, the days and times during which it can be used (shift hours
                                                        on the calendar) are specified.
                                                  •     The date for producing an order item is calculated from the dwelling time of
                                                        the item in the production area (transition matrix, transition times), the shift
                                                        hours (calendar), and the default times.
4.02 / 01-2017




                                                  When master data for capacity planning have been entered, the orders can be
                                                  scheduled in capacity planning. All order items and their BOM components are


                 H-16                                                                              A+W Business Pro Capacity Planning
                 Tutorial                                                                                     Overview




                                        allocated to the appropriate work types. After that, the required machine times
                                        and the costs are calculated. At the same time, the delivery date is checked
                                        and the start of production is calculated. During and/or after scheduling, you
                                        can intervene in the planning process and manually reschedule work process-
                                        es of an order item to other, similar machines.
                                        You monitor the current planning on the Control station dialog. From this dia-
                                        log, you can intervene in the planning process and display various overviews
                                        and graphics on the utilization.
                                        If the module is connected to the production software A+W Production, the re-
                                        sults of capacity planning (rough scheduling) are transferred to
                                        A+W Production. From A+W Production, in return, the reports are transferred
                                        to A+W Business Pro when orders or items are reported complete in produc-
                                        tion. In A+W Business Pro this will raise the order or item status. Data regard-
                                        ing machine costs and times are updated after completion of the order.

                                            Time and cost determination
                                            The time and machine costs are calculated from the settings of capacity
                                            planning. This rough scheduling process also checks whether the orders
                                            will be ready for shipping on time. Capacity planning in A+W Business Pro
                                            does not determine on which machines the orders are actually produced in
                                            the production process.


                                        Using Capacity Planning
                                        You can plan the production capacities based on the order, machine, and time
                                        data in A+W Business Pro without connection to A+W Production.
                                        The following main features characterize capacity planning of A+W Business
                                        Pro:
                                        •   Flexible creation of master data for capacity planning
                                        •   Determination of capacity bottlenecks
                                        •   Checking of the delivery date
                                        •   Calculation of the production costs
                                        •   Control station with overviews and rescheduling functions
                                        •   With connection to the production software A+W Production:
                                            – Transfer of planning data to A+W Production
                                            – Report on actual data to A+W Business Pro
                                            – Comparison of target and actual values

                                            Explanation of terms
                                            In A+W Business Pro and in this documentation, the terms capacity plan-
                                            ning and time management are used synonymously.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-17
                 Master Data                                                                            Tutorial




                               Master Data
                               With the help of master data, capacity planning can be adjusted to various cor-
                               porate structures and production processes.
                               In this topic block, you learn how the master data for capacity planning interact
                               and how to enter and maintain these data.
                               This includes the following learning sections:
                               •   “Machines and Production Areas” on page H-20
                               •   “Shift and Working Hours” on page H-34
                               •   “Allocate the A+W Business Pro Master Data” on page H-97

                               Rights management
                               Access to nearly all master data dialogs for capacity planning can be restricted
                               through rights management. This way, capacity planning can be adjusted even
                               better to the flows at your company. However, this also means that you need
                               full access rights to understand and execute the exercises in this tutorial.

                               History
                               Any change of order status in the individual production areas is automatically
                               recorded in the order history. Users who can only access the documents can
                               therefore always see when - and which - status change in the order header is
                               due to capacity planning and the reports from production.

                                   Master data for capacity planning
                                   Master data for machines and production areas are defined in the Capacity
                                   Planning module. This master data cannot be entered in the dialogs in the
                                   Master data module.

                                   If you have changed the settings in the master data for capacity planning,
                                   you must restart A+W Business Pro to reload the data.
4.02 / 01-2017




                 H-18                                                  A+W Business Pro Capacity Planning
                 Tutorial                                                                                Master Data




                                        Sequence for entering master data
                                        When entering machine-related master data, it makes sense to keep to the fol-
                                        lowing sequence:
                                        1 Machine types, e.g. cutting tables, TG ovens, shipping, etc.:
                                          type and scope of technical restrictions for machines are - among others -
                                          defined by the allocation to machine types.
                                            “Machine Types and Machines” on page H-21
                                        2 Production areas (work centers)
                                          Production and shipping are divided into areas, e.g. cutting, edge process-
                                          ing, drilling, inspection, packaging, etc.
                                            “Production Areas (Work Centers)” on page H-27
                                        3 Work units:
                                          For every individual machine, you can define the number of work units
                                          which form the basis for calculating the capacity.
                                            “Work Units” on page H-39
                                        4 Machines, e.g. Bystronic cutting table, Lisec cutting table, TG oven A, TG
                                          oven B, etc.:
                                          After defining the production areas and machine types, enter the individual
                                          machines and allocate them to the production areas and machine types.
                                            “Enter a Machine” on page H-29
                                        5 Work types (processes):
                                          All activities for which the times are calculated must be defined as work
                                          type, e.g. cutting, grinding, drilling, packaging, etc.
                                            “Work Types” on page H-25
                                        6 Default times:
                                          The times for work types depend on the individual machines. The times for
                                          work type Drilling e.g. depend on the glass thickness and the machine used
                                          for drilling. Therefore, times must be taken and entered per machine and
                                          work type.
                                          The default times are used to allocate the machines to the work types.
                                            “Default Times” on page H-55
                                        7 Time surcharges:
                                          In addition to the default times, time surcharges can be defined to be added
                                          to the basic value, e.g. for the cutting of shapes.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-19
                 Master Data                                                                                  Tutorial




                               Machines and Production Areas
                               Objectives

                               • Understanding the connection of machine types and machines.
                               • Entering production areas.
                               • Defining and entering work types.


                               Benefits

                               • You use master data for capacity planning to describe your production processes.
                                 Planning data therefore refer to the existing machines.


                               Note

                               Machine type               These are the machine types you use for production,
                                                          e.g. cutting tables, drilling machines, grinding machines,
                                                          TG ovens, etc.
                                                          A machine type can combine several individual
                                                          workstations, e.g. the IG line.
                                                          For every machine type, you define the restrictions to be
                                                          checked.

                               Machine                    Machines are all those stations where time is required. In
                                                          addition to the actual machines for cutting, drilling, etc.,
                                                          inspection, shipping, packaging also count as machines.
                                                          In A+W Business Pro there are no logical machines.

                               Production area            Production areas bundle machines performing the same
                                                          work, or machines performing a sequence of task, e.g.
                                                          IG production.

                               Work type                  The work type is the work performed at a machine.
                                                          All tasks for which times are calculated must be defined
                                                          as work types, e.g. cutting, grinding, drilling, packaging,
                                                          etc.

                               Work process               In this documentation, the term refers to the work type
                                                          performed for an order item. An order item usually
                                                          requires several work processes.

                               Restrictions               Restrictions which must be checked for certain
                                                          machines.
                                                          • These checks are activated for the machine type in
                                                            general.
                                                          • When defining the machine, you specify the values
                                                            that are to be consulted for the check and must not be
                                                            over- or underrun.
4.02 / 01-2017




                 H-20                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                                         Master Data




                                             Machine Types and Machines
                                             In capacity planning, any technical equipment where work is performed, is
                                             considered to be a machine. This can be a single machine as well as entire
                                             lines or the shipping area. Since different machines can perform the same
                                             work steps, several machines can be allocated to the same machine type.


                            A




                                B




                 A Machine types and possible restriction checks            B List of the machines for the machine type cutting
                 Fig. H-4       Example: machine type cutting and allocated machines


                                             As an example here is the machine type Cutting, which includes several ma-
                                             chines (B).
                                             Capacity planning checks the utilization of the available machines. It also ex-
                                             amines whether restrictions must be checked for the machine type in question
                                             (A) and whether the current order item meets or violates the defined values.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                      H-21
                 Master Data                                                                               Tutorial




                               Restrictions
                               Define the restrictions to be checked for every machine type.

                                   Example

                                   For machine type Cutting the following values should be checked:

                                   Dimension              One of the cutting tables cannot accommodate a
                                                          particular size of the stock sheets.

                                   Individual thickness   The cutting head must be changed for certain glass
                                                          thicknesses.

                                   Weight                 Depending on the weight, a second worker is required,
                                                          who works on just one of the cutting tables.

                                   Shape                  Automatic cutting is not suitable for shapes.

                                   Rotatability           Ornamental glass must not be rotated.


                               The fields in which the values for the active checks are entered, are released
                               for the machines.
                               In this example, the dimension and thickness of the glass shall be checked for
                               the Cutting machine type. For this, the values must be defined that must not
                               be over- or underrun.




                               A



                               B

                               A Check activated: values for height and B Check activated: value for thickness is
                                 width                                    not checked
                               Fig. H-5        Check values for automatic cutting machine


                               In this example, you see the that the Cutting machine cannot handle cuts
                               smaller than 100 mm (A). Also, only thicknesses from 4 to 10 mm (B) can be
                               cut. The glass thickness for manual cutting could be between 2 and 99 mm
                               which means that order items of 12 mm thickness have to be cut manually.
4.02 / 01-2017




                 H-22                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                                       Master Data




                                               Activated restriction checks
                                               If a restriction is checked, the corresponding field must not be blank. If the
                                               value is not to be checked, enter values in the fields that cannot be over-
                                               or underrun, e.g. 0.1 and 9999.

                                                “Define a Production Area” on page H-28


                   A               B               C




                                                                                                                   D
                 A Sheets can be turned                               C Check not activated for the machine type
                 B Check activated: shapes are not possible           D Weight
                 Fig. H-6     Checks for cutting machine


                                           In this example, you see that the cutting of shapes is not possible with the Cut-
                                           ting machine. Therefore, the order item is checked and not transferred to this
                                           machine if it includes a shape. For the Hand cutting machine, the shape cut-
                                           ting would be possible, so the checkbox is ticked.
                                           For the Hand cutting machine, the weight is set to 30 kg. For the normal cut-
                                           ting, here the weight 999 kg could be entered because the sheets are trans-
                                           ported automatically.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                    H-23
                 Master Data                                                                                Tutorial




                               Time and costs per machine
                               For every machine, you enter details based on which the machine costs are
                               calculated and the time required to produce an order item.
                               The defined times are used to calculate the capacities for the individual ma-
                               chine and for the entire production area.


                                   Number of units per                Machine
                                         hour                     e.g. cutting table A




                                             Costs per hour                              Work types
                                             • Wages per hour                            • Autom. cutting
                                               e.g. two workers                            (basic time)
                                             • Machine per hour
                                             • Variable costs per hour
                                               e.g. insurance




                               Fig. H-7       Entries for calculating times and costs per machine


                               The costs that arise per unit are defined for every machine. The number of
                               units per hour results from the measured time for the work type. The machine
                               capacity is the result of:
                               •   Units per hour
                               •   Number of hours per shift
                               •   Number of shifts the machine is working.
                               The way in which the units per machine are determined and how the time and
                               machine costs per order are calculated are described in separate sections.
                                “Work Units” on page H-39
                                “Production Costs” on page H-153
                               The definition of the data of a new machine requires additional details, e.g.
                               technical restrictions and priorities. These will be described in the following
                               sections. After that you will find detailed instructions on how to enter the data.
                                “Enter a Machine” on page H-29
                               A separate section describes how to control the selection of machines in con-
                               nection with automatic utilization.
                                “Selection of Machines” on page H-81
4.02 / 01-2017




                 H-24                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Master Data




                                        Work Types
                                        Work types (processes, tasks) form the basis for the production sequence.
                                        The work types are allocated to the machines which can perform the work type
                                        in question. A work type can be performed by several machines. Some ma-
                                        chines can perform several work types.

                                            Example

                                            The work type Polishing can be performed by various machines.

                                            •   One-sided grinding machine
                                            •   Two-sided grinding machine
                                            •   Grinding machine for series
                                            •   CNC machine


                                        A production process can include several work types, e.g. for LG production,
                                        a work type LG pre-bond and a work type LG autoclave.




                                        A




                                                                         B C                          D
                                        A Work types for cutting                 C Identifier for manual selection
                                        B Sequence order number                  D Alternative work type
                                        Fig. H-8       Work types


                                        In this example, you see that cutting (A) consists of three work types: automat-
                                        ic cutting, hand cutting, and the cutting of LG glass. This distinction is neces-
                                        sary because different machines are used for these work types, with different
                                        costs.
                                        The sequence ordering number (B) defines the production sequence of the in-
                                        dividual work types within capacity planning. The first work types usually refer
                                        to cutting and the following work types must be defined appropriately to
                                        achieve the correct sequence. Since the production of an IG unit can e.g. in-
4.02 / 01-2017




                                        clude a TG sheet, the work type TG tempering must always be performed be-
                                        fore IG production, which means that it has priority over IG production.




                 A+W Business Pro Capacity Planning                                                                  H-25
                 Master Data                                                                                                       Tutorial




                                               Work types for which the machine can only be selected manually during plan-
                                               ning have to be marked (C), e.g. the machine for manual cutting.
                                               The machines are allocated to the work types by means of the default times.
                                               The default times are described in detail in the Default Times section.
                                                “Default Times” on page H-52

                                               Alternative work type
                                               Alternative work types (D) are defined to cope with special situations, e.g. the
                                               drilling of thick sheets which requires other times and machines. Based on the
                                               technical specifications and the order item, the machine knows when to select
                                               the alternative work type, and calculates the time and costs accordingly.


                              Order                                  Work type                                         Machine

                                                                                                   Restrictions?
                            Float 6 mm                                    Drilling                                 Drilling machine I
                                                                                                                     up to 10 mm

                                                                                     Alternative work type

                            Float 12 mm                                 Drilling                                   Drilling machine II
                                                                     thick sheets                                  11 mm and thicker


                 Fig. H-9        Alternative work type for thick sheets


                                               In this example, you see that the alternative work type is selected because the
                                               standard machine cannot drill the thick sheet. The drilling machine II is select-
                                               ed because this machine has been allocated to the alternative work type.

                                                   Define new work type
                                                   Plan your work types in such a way that based on the number you can dis-
                                                   cern the grouping of related work types, or of work types belonging to the
                                                   same production process.

                                                   You define new work types in the same way as all basic tables. The proce-
                                                   dure is described in connection with the Production area.
4.02 / 01-2017




                 H-26                                                                              A+W Business Pro Capacity Planning
                 Tutorial                                                                                   Master Data




                                        Production Areas (Work Centers)
                                        A company is usually divided into different production areas, e.g. cutting,
                                        grinding, drilling, etc. Every production area can include several machines op-
                                        erated by a fixed number of workers. Similar machines can belong to different
                                        production areas.




                                        Fig. H-10     Production areas


                                        The production areas send status reports from production when an item has
                                        been produced completely. For this, you define the registration point that is go-
                                        ing to issue the report. In this example, the reports are sent from barcoding.
                                        As you can see, a production area has been defined for shipping. This is nec-
                                        essary so that the times in the shipping area can be included in the scheduling,
                                        and orders can be reported ready for shipment.
                                        Status reports can only be sent from production areas, not from machines. If
                                        you need e.g. two status reports for TG production, you must define two pro-
                                        duction areas: TG-furnace and Heat-soak.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-27
                 Master Data                                                                            Tutorial




                               Define a Production Area
                               When you set about entering new production areas from scratch you should
                               start by defining the relevant machines and work types.


                                How to enter the data for a production area
                               1 Select in the module Capacity planning > Master data > Organisation >
                                 Production area.
                                   The Production area dialog opens.
                                   This dialog is described in the Software Reference.
                               2 Select in the menu Start > New to change to the recording mode.
                                   The number of the production area is inserted automatically and can be
                                   changed.




                               A




                               Fig. H-11     Line inserted for new production area


                               3 Enter the name of the production area and if necessary, overwrite the num-
                                 ber.
                                   If you know the values for the other fields already, enter them in the appro-
                                   priate fields.
                               4 Select in the menu Start > Save to save the data.
                                   The data are saved. You can now enter the machines to be allocated to the
                                   new production area.
4.02 / 01-2017




                 H-28                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Master Data




                                          Enter a Machine
                                          You can enter all data for a new machine individually. If, however, you already
                                          have a comparable machine in your inventory, you should use its data as a ba-
                                          sis. This will make your task a lot easier. The following instructions will show
                                          you how to proceed.
                                          This includes the following training sessions:
                                          •   “How to enter the data for a new machine” on page H-29
                                          •   “How to adjust the technical restrictions” on page H-32


                                           How to enter the data for a new machine
                                          1 Select in the module Capacity planning > Master data > Organisation > Ma-
                                            chines.




                 A




                 Fig. H-12   Select production area


                                          2 Select the production area for allocating the new machine, e.g. Processing.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-29
                 Master Data                                                                                             Tutorial




                                              3 Select in the menu Start > Search to load the data for the machines from
                                                this production area.


                                                                                            A




                 B




                                                                                                                     D




                 C




                 A Pre-population of the fields with the data for the   C List of the machines in the production area
                   selected machine                                     D Registration point from which a completion report is
                 B Number and name of the selected machine                sent
                 Fig. H-13     Machines in the production area


                                                 In the overview (C) all machines allocated to this production area are listed.
                                                 The fields of the values (A) are pre-populated with the data for the selected
                                                 machine.
                                              4 On the overview, mark the machine the values of which you want to adopt.
                                              5 Select in the menu Start > New to change to the recording mode.
                                                 The field for the machine number (B) is released.
                                              6 Overwrite the number and name of the machine.
                                              7 If necessary, select another production area.
                                              8 Adjust the values in the fields for the costs (A).
4.02 / 01-2017




                 H-30                                                                 A+W Business Pro Capacity Planning
                 Tutorial                                                                                        Master Data




                                          9 In the Registration point field (D), enter the ID of the registration that will is-
                                            sue the completion report.




                 A




                                                                                                                            B




                 A Activating checks                                  B Locking machine
                 Fig. H-14   Adjusting values for the machine


                                          10 Select in the menu Start > Save to save the new data.
                                              With that, you have entered a new machine. The machine will be listed in
                                              the overview. You can now activate the checks (A) and adjust the details for
                                              the technical restrictions.

                                              Locking a new machine
                                              If you have entered a new machine that shall not be used for capacity plan-
                                              ning yet, you have to lock it (B).
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                     H-31
                 Master Data                                                                                          Tutorial




                                            How to adjust the technical restrictions
                                           1 Change to the Restrictions tab.




                                                                                                                  A



                                                                                                                  B




                   A Assigned work types                                B Technical restrictions
                   Fig. H-15   Adjusting technical restrictions


                                           2 In the Technical restrictions group (B), check which values apply to the ma-
                                             chine.
                                              If a required check is locked, you may have allocated the wrong machine
                                              type on the Machine tab. If the machine type is allocated correctly, check
                                              on the Machine types dialog whether the check boxes for the checks are
                                              ticked correctly.

                                              New restriction check activated
                                              If you enable a restriction check for the machine type, you have to fill in the
                                              corresponding fields for all machines. Enter at least zero (0) so that the field
                                              is not blank.

                                           3 Select in the menu Start > Save to save the data.
                                              The data are saved. The details on the allocated work types (A) will be dis-
                                              played only if they have been defined in the allocation dialogs.
4.02 / 01-2017




                 H-32                                                               A+W Business Pro Capacity Planning
                 Tutorial                                                                                 Master Data




                                        Exercises
                                        •   Consider the layout of the production and how you can map this organiza-
                                            tion in the master data with production areas and machines.
                                        •   Create a production area IG-2 plus the appropriate machines.
                                            The exercises are built on one another. You should therefore enter several
                                            different machines to be able to compare the exercises in the next ses-
                                            sions.
                                        •   Define a work type for triple IG.

                                            Exercises in real operation
                                            If your capacity planning module is already being used in daily business,
                                            you will have to lock the new machines to prevent them from being used
                                            for planning purposes.


                                        Additional information
                                         Software Reference, “Machine Types” on page H-185
                                         Software Reference, “Work Types” on page H-187
                                         Software Reference, “Allocated Machines” on page H-190
                                         Software Reference, “Production Area” on page H-195
                                         Software Reference, “Machines” on page H-196
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-33
                 Master Data                                                                                       Tutorial




                               Shift and Working Hours
                               Objectives

                               • Defining shift hours and calendar.
                               • Get to know work units.
                               • Calculate capacities per production area and per machine.


                               Benefits

                               • The defined shifts and the details on work units are used to calculate the capacities
                                 of the individual production areas. Based on these capacities, orders are
                                 scheduled.


                               Note

                               Shift                        The duration of shifts can differ for the individual
                                                            production areas.
                                                            Shifts must start at the same time in all production areas
                                                            to avoid overlapping shift changes and clashes in the
                                                            transition from one production area to the next.

                               Work unit                    With work units, you define how much can be produced
                                                            per hour.
                                                            Work units can be defined as man hours or as machine
                                                            hours.

                               Capacity                     The capacity of a machine is the product of work units
                                                            and shift hours.
                                                            The capacity of a production area is the total of all
                                                            machine capacities in the production area.

                               Closed capacity              With closed capacities, another date is searched
                                                            automatically if the available shifts and machines are at
                                                            full capacity.

                               Open capacity                With open capacities, the shift hours are not checked.

                               Default settings             Company data:
                                                            • Capacity planning > Number of shifts tab
4.02 / 01-2017




                 H-34                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Master Data




                                        Working Hours
                                        he calculation of dates is based on the entries you have made in various dia-
                                        logs. These are e.g. details on:
                                        •   the time a machine can be used (shift hour).
                                        •   the time required to produce a piece (default time).
                                        •   the additional time required for more complex work processes (time sur-
                                            charge).
                                        •   setup time.
                                        The correlations between the different default times and the default settings for
                                        the work times are explained below.


                                        Workdays and Shifts
                                        For the scheduling in capacity planning, it is important whether or not your
                                        company works in shifts.
                                        •   If production is not working in shifts, capacity planning will use the
                                            A+W Business Pro standard calendar.
                                        •   If production is working in shifts, the shift hours can be defined per produc-
                                            tion area.
                                        If not all production areas are working in all shifts, the number of shifts de-
                                        pends on the production area with the most shifts. You define this number in
                                        module Master data > Company > Company data.




                                        Fig. H-16     Company data – Capacity planning tab


                                        The length of a shift is defined on the calendar per machine or production area.
                                        If e.g. several production areas work in three shifts of different lengths, you
                                        must organize the shifts so that shifts 2 and 3 begin at the same time in all pro-
                                        duction areas.
                                        The shifts in the various production areas must not overlap because otherwise
                                        the transition from one shift to the next is not clear in case of a change of pro-
                                        duction area.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-35
                 Master Data                                                                                          Tutorial




                   Example

                    Production area Start of 1st Number of Start of 2nd Number of Start of 3rd Number of                 End
                                       shift       hrs.        shift      hrs.       shift       hrs.

                        Cutting       06:00          6            12:00              4          16:00        4          20:00

                          LG          08:00          4            12:00              4          16:00        4          20:00

                        Drilling      10:00          2            12:00              4          16:00        2          18:00

                     Heat-soak test   08:00          12                              0                       0          20:00

                                         This shift organisation guarantees that there are no delays between shifts be-
                                         cause the shifts change at the same time in the production areas.
                                         You define the times for the shift changes in module Capacity planning > Mas-
                                         ter data > Machines > Calendar > Functions menu > Shifts.




                                         Fig. H-17       Settings for shift change


                                         In this example, you see that shift 2 begins at 12:00 and ends at 16:00. Sub-
                                         sequently, shift 1, with a shift of 6 hrs., begins at 6:00. The transition from shift
                                         2 to shift 3 is at 16:00, which means that shift 2 is only 4 hours long.
4.02 / 01-2017




                 H-36                                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                                                       Master Data




                                              Maximum Capacity per Day
                                              The daily capacity of a machine is calculated in work units. The capacity for
                                              the corresponding production area consists of the units per hour of all ma-
                                              chines belonging to the production area.


                    Cutting production
                           area
                          Capacity:
                   Number of units per hour
                      for all machines


                                                 Number of units per                 Machine
                                                       hour                      e.g. cutting table A




                                                                                     Work type
                                                                                   Autom. cutting
                                                                                    (basic time)




                                                 Number of units per                 Machine
                                                      hour                      e.g. cutting table B




                                                                                     Work type
                                                                                    Hand cutting
                                                                                    (basic time)




                 Fig. H-18     Calculation of times per machine and production area


                                              The maximum capacity of a machine results from the total hours per day en-
                                              tered in the calendar multiplied by the work units per hour that are defined for
                                              the machine on the Machine dialog.

                                                 Example

                                                 Day: Tuesday, Cutting production area, Cutting table machine
                                                 On the cutting table, it is possible to produce 4 work units per hour.

                                                 Shift        Hours        x 4 work units/hour = max. work units/shift

                                                 1st shift    6 hours      x 4 work units/hour          = 24 work units/shift
                                                 2nd shift    4 hours      x 4 work units/hour          = 16 work units/shift
4.02 / 01-2017




                                                 3rd shift    4 hours      x 4 work units/hour          = 16 work units/shift

                                                 Max. capacity per day on the cutting table.            = 56 work units/day



                 A+W Business Pro Capacity Planning                                                                                   H-37
                 Master Data                                                                                         Tutorial




                                            The capacity of a production area results from the total daily capacities of all
                                            machines in this production area.
                                            Thereby, you must consider whether all machines can be used at any time. If,
                                            for example, you have 6 grinding machines but only 3 workers who can oper-
                                            ate these machines, the total capacity can only be calculated for three ma-
                                            chines. The check for free capacities therefore does not only refer to the
                                            machines themselves, but also to the maximum number of units that can be
                                            produced in a production area.




                                                                                                       B
                                                          A




                 A Units in the production area                               B Units on the machine
                 Fig. H-19     Number of units


                                            In the following section you will learn how to determine the work units.
4.02 / 01-2017




                 H-38                                                               A+W Business Pro Capacity Planning
                 Tutorial                                                                                           Master Data




                                        Work Units
                                        Work units can be defined for every single machine as well as for the entire
                                        production area. Both values are based on the same calculation type for the
                                        work unit.
                                        Before entering the values, you must define which work unit is used. There are
                                        a lot of options, e.g.:
                                        •   Work unit = man hour
                                        •   Work unit = machine hour
                                        You must answer the following questions to define the work units per hour and
                                        the default times:
                                        •   Which work unit shall be used to determine the machine capacity?
                                            What are man hours, machine hours, etc.?
                                             “Work unit = man hour” on page H-39
                                             “Work unit = machine hour” on page H-42
                                        •   Which value has to be entered for Unit/h?
                                             Software Reference, “Machines” on page H-196
                                        •   How much time does the machine need for a unit (running m, sq m, piece)
                                            in relation to the work unit?
                                             “Determination of the man hours” on page H-40

                                        Work unit = man hour
                                        In scheduling, the work units are used to check whether there are free capac-
                                        ities on this day.

                                            Example

                                            In the Drilling production area (5 machines), 12 persons are working in a
                                            total of three shifts per day. This makes it four persons per shift. These four
                                            persons correspond to four work units in the Drilling production area.

                                            Even if only four persons are available in the production area for five
                                            machines, in theory each machine can run the entire shift, e.g. eight hours.
                                            This means that you enter a work unit equal to 1 for each machine. Which
                                            four of the five machines are used depends on the scheduling data.


                                        The following is checked:
                                        •   Is the machine running to capacity?
                                        •   If so, are other machines available? This means: has the maximum capac-
                                            ity of the production area of four work units already been reached?
                                            – If so, you can schedule on a free machine.
                                            – If not, the work process must be moved to the next day or the next shift,
                                                or you can decide that overtime is required.

                                            Workers present
4.02 / 01-2017




                                            Capacity planning assumes that all persons (workers) are present all the
                                            time.




                 A+W Business Pro Capacity Planning                                                                           H-39
                 Master Data                                                                                      Tutorial




                               Determination of the man hours
                               To determine the man hours, the time values must be multiplied by the number
                               of persons working on the machine. The default time is calculated in different
                               ways, depending on whether you define individual times or a graduation, e.g.
                               by thickness,.
                               The following examples are mere calculation examples.

                                  Example: 3 persons, individual time

                                  Calculation of man hours at the cutting table:
                                  • 3 persons work at the cutting table.
                                  • In one hour, 200 sq m can be cut.
                                  • The default time is defined as individual time.


                                  Formula:

                                                                    1h
                                  Default time 1 sqm =                               x number of persons [man hours]
                                                         number of sqm per hour



                                  Calculation example:

                                                            1h
                                  Default time 1 sqm =                   x 3 persons = 0,015 [man hours]
                                                          200 sqm




                                  Example: graduated time (vector)

                                  Calculation of man hours at the cutting table, graduated to thickness:
                                  • 3 people work at the cutting table.
                                  • Time taken per unit produced, graduated by glass thickness.
                                  • The default times are entered in the vector format.


                                  Formula:

                                   Default time 1 sqm = stopped time x number of persons [man hours]



                                  Calculation example:

                                  Default time 1 sqm float 4 mm = 0.009 hrs. x 3 persons = 0.027 man hours
                                  Default time 1 sqm float 6 mm = 0.010 hrs. x 3 persons = 0.03 man hours
4.02 / 01-2017




                 H-40                                                         A+W Business Pro Capacity Planning
                 Tutorial                                                                                          Master Data




                                           Example: 2 persons, individual time

                                           Calculation of man hours at the grinding machine:
                                           • 2 persons work at the grinding machine.
                                           • In one hour, 3 linear meters can be ground.
                                           • The default time is defined as individual time.


                                           Formula:

                                                                           1h
                                             Default time =                                 x number of persons [man hours]
                                                              number of linear m per hour



                                           Calculation example:

                                                                 1h
                                            Default time =                 x 2 persons = 0,66 [man hours]
                                                              3 linear m
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                           H-41
                 Master Data                                                                            Tutorial




                               Work unit = machine hour
                               If the times are independent of the number of workers on the machine, you can
                               use the work unit Machine hours.
                               In this case, the work unit for the machine always has to be 1.




                               Fig. H-20    Machine dialog – Units and costs


                               By default, 1 is entered for the number of units. This makes it easier to under-
                               stand the calculation of capacities.

                               Work units per production area
                               The number of work units per production area usually corresponds to the num-
                               ber of machines used there. If three machines are used, the number of work
                               units is 3.
                               However, the conditions in production can be restricted as follows:
                               •   You are using e.g. three machines in the production area.
                               •   However, the power supply permits to operate only two machines at the
                                   same time. This means that one of the machines must always be switched
                                   off.
                               In this case, you must enter the value 2 as the work unit per hour for the entire
                               production area.




                               Fig. H-21    Units per production area
4.02 / 01-2017




                 H-42                                                   A+W Business Pro Capacity Planning
                 Tutorial                                                                                      Master Data




                                          Default Settings for Shift and Capacities
                                          In the Master data module, you specify the basic settings for capacity planning
                                          in A+W Business Pro.




                 A
                 B
                 C




                 A Number of shifts                                  B Defines degree of utilization
                                                                     C Setting for large order items
                 Fig. H-22   Company data – Capacity planning


                                          The number of shifts (A) depends on the production area in which the most
                                          shifts are run. The shifts will be considered, for example, for calculating the
                                          transition matrix and the transition times.
                                          You must define whether you are going to use closed or open capacities.
                                          •   In case of closed capacities, another date is searched automatically if the
                                              available shifts and machines are working at full capacity.
                                          •   In case of open capacities, the shift hours are not checked.
                                          Furthermore, you must define the extent to which a shift may be utilized if the
                                          orders are automatically transferred to capacity planning. If your shifts are al-
                                          ways run at full capacity, or nearly full capacity, there will be no leeway for re-
                                          scheduling, for express orders or for residual quantities from the day before.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                    H-43
                 Master Data                                                                              Tutorial




                               The following settings are available for the degree of utilization in the Produc-
                               tion scheduling mode field (B).
                               •   Autom. normal capacity:
                                   The orders will be scheduled based on the available shift times. Overbook-
                                   ing is impossible. This is the default setting (closed capacities).
                               •   Automatic full days:
                                   This setting ignores the specifications for the number of shifts and hours in
                                   the calendar. Scheduling is based on a workday of 24 hours in this case
                                   (open capacities). This applies only to common workdays, not to holidays.
                               •   Change machine only:
                                   If capacities are fully utilized, the program will automatically search for an-
                                   other machine. If this is used to capacity as well, scheduling is interrupted
                                   and manual intervention is required.
                               •   Schedule without check:
                                   This setting represents an open shift. This means e.g. that despite a shift
                                   time of 8 h, 16 h can be scheduled as well. The program will issue no report
                                   if a day's capacity is fully utilized. This option should only be used in excep-
                                   tional cases.
                               Larger items can be split to several machines, shifts or days. For this, in the
                               Fill shift in case of item splitting field (C), you define the percentage of the ma-
                               chine's shift that can be filled by splitting to leave leeway for other orders.

                                   Changing settings
                                   If you have changed settings in company data, you should restart
                                   A+W Business Pro.

                               You will learn about the other settings for workdays and shifts in the associated
                               learning sections.
4.02 / 01-2017




                 H-44                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                                     Master Data




                                        Adjust Calendar
                                        By default, capacity planning is based on one shift per day. If, however, you
                                        want to work in more than one shift, you must enter the number of shifts in the
                                        company data first.
                                        After that, you can enter a separate calendar with the corresponding shifts and
                                        shift hours for every work type and machine, or per production area. If no indi-
                                        vidual calendar is defined for a production area or machine, the general calen-
                                        dar applies.

                                            Change of year
                                            To schedule capacities beyond the turn of the year, you have to enter the
                                            calendar for the new year including all shift hours.

                                        This includes the following training sessions:
                                        •   “How to define the number of shifts” on page H-45
                                        •   “How to create a new calendar” on page H-46
                                        •   “How to enter additional shift hours” on page H-49
                                        •   “How to create a special shift” on page H-50

                                            Changing the calendar
                                            When you have edited or entered a calendar, you must restart
                                            A+W Business Pro to make sure that the data are available for scheduling.


                                         How to define the number of shifts
                                        1 Select in the module Master data > Company > Company data.
                                        2 Change to the Capacity planning tab.
                                        3 In the A+W Business capacity planning group, enter the number of shifts.




                                            Fig. H-23    Company data – Capacity planning tab


                                        4 Select in the menu Start > Save to save the changes.
                                            The data are saved. In the capacity planning calendar, the fields for the shift
                                            hours are released.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-45
                 Master Data                                                                                      Tutorial




                                          How to create a new calendar
                                         1 Select in the module Capacity planning > Master data > Organisation > Ma-
                                           chines.




                    A                                                                                  C

                    B




                   A Fields depending on mode (C)                 C Work type or production area
                   B Select calendar year
                   Fig. H-24   Creating calendar


                                            This dialog is described in the Software Reference.
                                         2 Select the mode (C):
                                            •      Work type/machine:
                                                   The new calendar shall be set up for a machine and/or a work type.
                                            •      Production area/client:
                                                   The new calendar shall be set up for a production area and/or a client.
                                            The labeling of the fields (A) depends on the mode. In this example, the cal-
                                            endar is created for a machine.
                                         3 Select the work type and the machine.

                                            New calendar year
                                            Consider that the new calendar year you have created with these steps is
4.02 / 01-2017




                                            available for work types and machines only. To create a new calendar year
                                            for production areas, repeat the entire process for the production area in
                                            question.



                 H-46                                                              A+W Business Pro Capacity Planning
                 Tutorial                                                                                 Master Data




                                        4 Select the year (B).
                                           If you enter the number of the new year, the calendar is created for this
                                           year.
                                        5 Select in the menu Start > New to change to the recording mode.




                                           Fig. H-25    Setting up calendar for machine


                                        6 Change to the Calendar tab.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-47
                 Master Data                                                                                Tutorial




                                    A                       B     C                                         D




                                  A Days of the week                    C Shift hours applied to the year
                                  B Hours per shift and day of the week D Apply details
                                  Fig. H-26    Entering shift hours


                               7 Enter the shift hour (B) per workday and shift.
                                  Make sure that the checkboxes (A) of the days on which you have entered
                                  shift hours are ticked.
                                  When you have entered the hours, the buttons for application are released.
                               8 Click the [Apply to year] button (D).
                                  The data are applied to the Calendar overview (C). When you have entered
                                  a new year, the new calendar is created.
                               9 Select in the menu Start > Save to save the data.
                                  The data are saved. The shift will be considered for scheduling after
                                  A+W Business Pro has been restarted. You can now continue editing the
                                  shift hours.
4.02 / 01-2017




                 H-48                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Master Data




                                         How to enter additional shift hours
                                        1 Select in the module Capacity planning > Master data > Organisation > Ma-
                                          chines.
                                        2 Select the current calendar year.
                                        3 Select in the menu Start > Search to start the search.
                                           All calendars that correspond to the selection criteria are loaded.
                                        4 Mark the required calendar and change to the Calendar tab.
                                        5 On the Calendar overview, mark a week to load the shift hours.
                                        6 In the Hours per shift group, enter the hours for the new shift.
                                           Make sure that you enter the hours for all shifts. If you leave the fields for
                                           the already-existing shift hours blank, the hours will be deleted when they
                                           are applied to the week or the year.




                                           Fig. H-27    Adding shift hours


                                        7 Check whether all checkboxes for the weekdays for which you have en-
                                          tered the hours are ticked.
                                        8 Click the [Apply to year] button.
                                           Thus the shift hours are applied to the entire calendar year.
                                        9 Select in the menu Start > Save to save the changes.
                                           The data are saved. The shift hours will be considered for scheduling after
                                           A+W Business Pro has been restarted.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-49
                 Master Data                                                                               Tutorial




                                How to create a special shift
                               1 Select the required calendar and change to the Calendar tab.

                                                                     A                             B     C




                               A Hours of the special shift               B Calendar week of the special shift
                                                                          C Applying hours
                               Fig. H-28     Setting up a special shift


                               2 Select the calendar week (B) in which the special shift shall be run.
                               3 Enter the hours (A) of the new special shift.
                               4 Click the [Apply to week] button (B).
                                  The shift hours are only applied to the selected week.
                               5 Select in the menu Start > Save to save the data.
                                  The data are saved. The special shift will be considered for scheduling after
                                  A+W Business Pro has been restarted
4.02 / 01-2017




                 H-50                                                     A+W Business Pro Capacity Planning
                 Tutorial                                                                                   Master Data




                                        Exercises
                                        •   Sketch the shift plan for your production areas on paper.
                                        •   Define that there will be three shifts (company data!).
                                        •   Enter the hours in the calendar. Please take into account that the working
                                            times differ for the individual production areas and on the different days of
                                            the week.
                                            Example: Shipping - do 8 hours in shift 3 make sense on a Friday?
                                        •   Increase the number of shifts and check the effects on the calendar.


                                        Additional information
                                         Software Reference, “Default Settings in Company Data” on page H-179
                                         Software Reference, “Calendar” on page H-205
                                         Software Reference, “Shift Settings” on page H-183
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-51
                 Master Data                                                                                   Tutorial




                               Default Times
                               Objectives

                               • Getting to know different concepts of time calculation.
                               • Defining default times.


                               Benefits

                               • Based on the default times and the free capacities, the program determines when
                                 the individual production steps of an order can be executed.


                               Note

                               Default times               The times that are necessary to perform the individual
                                                           tasks (work types) have to be taken.
                                                           These times will be entered as the default times.

                               Basic time                  Time taken that a work type on a machine needs to
                                                           produce one unit. This time can be increased or
                                                           decreased by means of surcharges.

                               Time surcharge              Time surcharge is a difficulty surcharge, e.g. for multiple
                                                           layer IGs or shapes. The time surcharge always refers to
                                                           the basic time defined for a work type at a machine.
                                                           Surcharges are totaled. The basic time + 100% results in
                                                           a doubling of the time.

                               Factor                      Factors are multiplied by the basic time for the work type.
                                                           Factor 1 means that the time is not increased. Factor 0.5
                                                           means that the time is reduced by half.

                               Special times               Special times are always surcharges on the basic time
                                                           defined for a work type. Special times are used e.g. to
                                                           take care of the fact that two workers instead of just one
                                                           are necessary to operate a machine.
                                                           Special times can be entered as graduated times.

                               Transition times            The transition time defines the time a unit needs to move
                                                           from one work process or production area to the next.
                                                           The time is entered in shifts.

                               Dwell times                 These times define how long a unit dwells in a
                                                           production area.

                               Setup times                 Setup times are defined as work types and are allocated
                                                           to the machine and the processing.
4.02 / 01-2017




                 H-52                                                     A+W Business Pro Capacity Planning
                 Tutorial                                                                                   Master Data




                                        Basic Components of Time Planning
                                        In addition to the order quantity, the following specifications are considered in
                                        time planning:


                                            Work type/machine               Default time
                                                                           for work type
                                                e.g. seaming
                                                                            (basic time)



                                                Surcharge               Graduated surcharge
                                              e.g. for thickness



                                                Allocation                    Factor
                                            e.g. for processing of         e.g. per edge
                                                    shapes



                                             Production area                Dwell days              Production area
                                               e.g. TG furnace                                         e.g. Shipping



                                                Work type                  Transition time             Work type
                                                e.g. washing              Transition matrix          e.g. TG tempering


                                        Fig. H-29      Times


                                        In this overview, you can see the default times that can be defined:
                                        •   Default times
                                            defines the time a work type requires at a certain machine.
                                            These times are entered on the Default Times dialog.
                                        •   Time surcharges
                                            are usually graduated surcharges that increase, under certain circumstanc-
                                            es, the default times for rectangular sheets.
                                            These times are entered on the Special times dialog.
                                        •   Time surcharges and factors
                                            increase or reduce, under certain circumstances, the default times for pro-
                                            ducing non-rectangular sheets (shapes).
                                            These times are entered on the dialogs on the Allocation menu.
                                        •   Dwell days
                                            define the time a unit dwells in a certain production area.
                                            These times are entered on the Production area dialog.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                    H-53
                 Master Data                                                                            Tutorial




                               •   Transition times
                                   define how long it takes a unit to get from a certain work type to another or
                                   from a certain production area to another.
                                   These times are entered on the Transition matrix and Transition times dia-
                                   logs.
                               •   Setup times
                                   define the time that is necessary to set a machine up for the next process.
                                   Set-up times are usually entered as a times surcharge.
                               The following sections explain the concepts for using these time components.
                               After that, the dialogs are shown in action sequences, so that you can see how
                               to make the individual settings.

                                   Editing master data
                                   After editing the master data - and especially the default times - in the Ca-
                                   pacity planning module, you should restart capacity planning.
4.02 / 01-2017




                 H-54                                                  A+W Business Pro Capacity Planning
                 Tutorial                                                                                           Master Data




                                              Default Times
                                              Default times are specified for every single work type per machine. These
                                              times can be graduated with up to three limit types.



                 A




                 B




                 C




                                                                                 D          E          F
                 A Tab for graduated times                                D Work type
                 B Priority for machines of the same type                 E Machine for which the time has been specified
                 C Selection of surcharges (special times)                F Type of the default time
                 Fig. H-30    Default Times


                                              For all tasks, the times per machine and unit are taken. Whether you take the
                                              times per piece, sq m or edge length depends on the product to be produced,
                                              the work type, and the machine. Based on the defined work unit, the number
                                              of workers operating the machine is considered as well. These times are de-
                                              fined for every machine and for all work times performed by this machine.

                                              Type of Default time
                                              Default times can be included in the calculation in different ways.
                                              A+W Business Pro distinguishes four different types (F):
                                              •   Basic time:
                                                  This is the taken default time for a work type, e.g. for the work type Cutting.
                                                  Since the time requirement for a work process usually depends on the size,
                                                  these times can be graduated with up to three limit types.
                                              •   Time surcharge:
4.02 / 01-2017




                                                  A time surcharge is required, e.g. for cutting of shapes. This means that for
                                                  the cutting of shapes, no individual default time is measured. Instead, the




                 A+W Business Pro Capacity Planning                                                                         H-55
                 Master Data                                                                              Tutorial




                                   normal default time is increased by a surcharge.
                                   The time surcharges will be discussed in detail in a separate section.
                                    “Work Types and Time Surcharges” on page H-59
                               •   Alternative procedure:
                                   This default time is only considered if an alternative work type exists for the
                                   work type. In this case, you must enter the alternative machine number in
                                   the Alternative A+W Prod.no. field.
                               •   Alternative without BOM:
                                   As a LG producer, your LG item is usually entered with a BOM by default.
                                   If, however, e.g. a LG sheet is not produced but directly to be cut from a
                                   laminated stockplate for once, the BOM must not be taken into account for
                                   production. For the LG cutting work type, you must therefore set the option
                                   Alternative without BOM. In this case, you must enter the alternative ma-
                                   chine number in the Alternative A+W Prod. no. field.
                               •   Ignore process:
                                   A corner cut-out e.g. includes three processes: 1. Drilling (of corner hole),
                                   2. Cutting, and 3. Grinding.
                                   The CNC machine can execute all three procedures as one work process,
                                   therefore you have to allocate a default time only to the work type Drilling.
                                   To the other two work types on this machine you allocate the value Ignore
                                   process.

                               Priority
                               If several machines are available for a work type, you must define which ma-
                               chine is queried first during the search for free capacities.
                               If two machines have the same priority (B), then capacity planning checks the
                               costs defined per machine. In this case, the most economic machine will be
                               selected automatically.
                               If no costs are defined per machine, the priority for equivalent machines must
                               be clear, that is, different.
                               •   9: highest priority (standard machine). These machines are always select-
                                   ed first.
                               •   8 to 1: decreasing priority. These machines are selected depending on uti-
                                   lization.
                               •   0: lowest priorities. These machines are only selected if all other (equiva-
                                   lent) machines are used to capacity.
                               •   -1: for manual scheduling. These machines are selected by automatic
                                   scheduling only in case of bottlenecks.
                               •   -2: only for manual scheduling. These machines are never selected by au-
                                   tomatic scheduling. The machine can only be selected manually.
                               •   -3: is only selected with reporting from the production system when orders
                                   have been rescheduled there. In case of rescheduling in capacity planning,
                                   only machines with prio >-3 are displayed.
4.02 / 01-2017




                 H-56                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                                      Master Data




                                        Limit types and graduation
                                        Times can be graduated with up to three limit types.
                                        •   Vector:
                                            For vectors, times are entered based on one limit type, e.g. metre, surface.
                                        •   Matrix:
                                            For a matrix, times are entered based on two limit types, e.g. width and
                                            height.
                                            You can create a triangular matrix so that the limit types can be exchanged,
                                            e.g. height and width.
                                        •   Cube:
                                            The structure of a cube is similar to the matrix times but offers three limit
                                            types, e.g. width, height, and thickness.
                                        The limit types and graduations have been introduced in connection with pric-
                                        ing in the training on master data.
                                        A list of available limit types is available in section Master data.
                                         Master Data: Tutorial 2, “Available Limit Types” on page B-512

                                        Triangle
                                        You can enter times in a matrix or in a cube so that the defined limit values can
                                        be exchanged, e.g. height and width. You only have to enter one of the com-
                                        binations.

                                        Times in hours
                                        The times are not defined in minutes, but in hours. This means that you have
                                        to convert times measured in minutes into hours.

                                            Example

                                            Formula:
                                            Minutes taken / 60 = time value in hours

                                            Minutes               Entry of the time value (in hours)

                                            60                    1
                                            30                    0.5
                                            15                    0.25
                                            7.5                   0.125
                                            3.75                  0.0625
                                            1.875                 0.03125


                                        If for a work type you have measured a time of 2.5 minutes, enter a time value
                                        of 0.0417 as basic value.

                                            Copying default times
                                            If two equivalent machines require the same time, you can use the copy
                                            function to copy the times from one machine to the other and adjust them.
4.02 / 01-2017




                                            This is especially useful for graduated times.




                 A+W Business Pro Capacity Planning                                                                  H-57
                 Master Data                                                                               Tutorial




                               Special Times
                               The measured times cannot be kept if, for example, an especially large sheet
                               requires more time in production. In this case, you define a special time as
                               time surcharge, which is usually added to the basic item.
                               Special times are useful if the size, material or thickness of the sheet repre-
                               sents a particular challenge.




                               A




                               B




                                              C       D             C   D           E   F            G
                               A   Number of the surcharge table            E Amount of the surcharge
                               B   Graduated surcharge                      F Unit to which the surcharge refers.
                               C   Limit value (1, 2)                       G Surcharge type
                               D   Limit type (1, 2)
                               Fig. H-31     Special times dialog


                               In this example, you see that the time of the basic item is increased by 100%
                               if the sheet is especially small (smallest edge length 300 mm) or if it is espe-
                               cially large (width over 1400 mm, height over 2400 mm). The area between
                               these dimensions is calculated without time surcharge.
                               Special times are entered in the same manner as the Miscellaneous surcharg-
                               es in A+W Business Pro master data.
                                Master Data, “Miscellaneous Surcharges” on page B-301
4.02 / 01-2017




                 H-58                                                   A+W Business Pro Capacity Planning
                 Tutorial                                                                                         Master Data




                                        Work Types and Time Surcharges
                                        A special work type is usually defined for every task; the basic time (default
                                        time) is then entered for the work type. If tasks can be combined in a process,
                                        the basic task must be increased by a factor.

                                           Example

                                           The production of a triple IG unit takes 2.5 times as long as the production
                                           of an IG unit with two sheets.
                                           At the IG line you enter a factor that increases the value of the basic time
                                           (for the double IG) accordingly.
                                           For detailed calculation examples, see:
                                            “Case Study IG and Shape” on page H-60


                                        Additional work for shapes is also defined as default time with the type Time
                                        surcharge for the work type in question.
                                        For every time surcharge you want to define, you must enter a work type. This
                                        means that you must define e.g. a work type for the cutting of shapes and a
                                        work type for the processing of shapes.
                                        It is easier however to define a work type Shape surcharges and enter the
                                        amount of time surcharge required for this work type for those machines per-
                                        forming this work type.


                                                                        Time surcharge A              Cutting table


                                         Work type                                                    Grinding machine
                                                                        Time surcharge B
                                         Shape surcharges

                                                                        Time surcharge C              IG line


                                        Fig. H-32     Work type Shape surcharges for time surcharges on different machines


                                           Rescheduling orders in case of bottlenecks
                                           Time surcharges also make rescheduling much easier. If you have to post-
                                           pone e.g. the production of a (complex) IG unit without time surcharges,
                                           this can mean that you will have to postpone all previous work processes
                                           individually.

                                        Shapes belong to the master data product type Shapes. Due to the allocation
                                        of product type Shapes to the work type Shape surcharges, the shapes are de-
                                        tected at scheduling. The times per order item will then be increased for
                                        shapes by the surcharge defined for the corresponding machine. These allo-
                                        cations will be introduced in the next topic block.
                                         “Allocate the A+W Business Pro Master Data” on page H-97
4.02 / 01-2017




                                        The following case study for the production of IG units shows the sequence in
                                        which time surcharges are defined, and how the required time is calculated at
                                        scheduling.


                 A+W Business Pro Capacity Planning                                                                       H-59
                 Master Data                                                                                                          Tutorial




                                               Case Study IG and Shape
                                               The production of IG units with three and more sheets and as shapes requires
                                               the definition of many default times. A possible concept is presented in this ex-
                                               ample. The aim is to define the default times so that they can be used for the
                                               calculation of IG sheets and shapes, reducing the data entry and maintenance
                                               efforts.


                         Machine                       Default time                    Work type                       Allocation

                             IG line                                                   Producing IG                   Product class
                                                        Basic time                                                 (A+W Business Pro
                                                                                                                      master data)
                                                         0.018 hr.
                                                                                                                        Triple IG
                                                                                                                       x factor 2.5
                                                                                         Triple IG




                                                      Time surcharge                 Shape surcharges
                                                          + 50 %



                 Fig. H-33       Definition of default times for example IG production


                                               Settings
                                               The settings below have to be made in the various dialogs. This example will
                                               be followed by more detailed instructions for action. The example is based on
                                               the following settings:
                                               •   The daily capacity of 450 IG units means:
                                                   8 hrs. / 450 units = 0.018 hr. per unit.
                                               •   For the IG line, a default time has been defined as an individual time of the
                                                   type Basic time.




                                                   Fig. H-34       Default time dialog – Individual time for IG unit
4.02 / 01-2017




                 H-60                                                                        A+W Business Pro Capacity Planning
                 Tutorial                                                                                      Master Data




                                        •   For shape surcharges and triple IG, work types of the same name are de-
                                            fined.


                                        A




                                        B
                                        A Work types Shape surcharges             B Work type Triple IG
                                        Fig. H-35     Work types for shapes and triple IG


                                        •   The Shapes product type is allocated to the Shape surcharges work type.




                                        A




                                        B

                                        A Allocated work type            B Product type (A+W Business Pro master data)
                                        Fig. H-36     Allocation of the product type to the Shape surcharges work type
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                      H-61
                 Master Data                                                                               Tutorial




                               •   As default time for the Shape surcharges work type, a time surcharge of
                                   50% is calculated for the IG line machine.




                                   Fig. H-37    Default time dialog – Time surcharge for shapes


                               •   Triple IGs are combined into the product class Triple IG.
                               •   The product class Triple IG is allocated to the work type Produce IG.
                               •   For triple IG, the factor 2.5 shall be calculated.




                                   Fig. H-38    Assignments Product class dialog – Factor for triple IG


                               •   Furthermore, a surcharge for oversizes shall be calculated. This has been
                                   defined as special surcharge.




                                   Fig. H-39    Special time dialog – Special surcharge for large and small sheets
4.02 / 01-2017




                 H-62                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                               Master Data




                                        Factors and surcharges for calculation
                                        Factors are multiplied by the basic time of the work process. Factor 1 means
                                        that the time is not increased. Factor 0.5 means that the time is reduced by
                                        half.
                                        Other surcharges are added as percentage surcharges. The basic time +
                                        100% results in a doubling of the time.
                                        These surcharges are defined as special times in surcharge tables and are al-
                                        located to the default time.
                                        The scheduling result only shows the times for work types for which a basic
                                        time has been entered. All time surcharges added to the basic times are in-
                                        cluded in these results and are not shown.


                                        Calculation Sequence for Surcharges and Factors

                                        Item                               Calculation                    Time (hr.)

                                        IG                                 Time                               0.018

                                        IG + shape                         0.018                               0.018
                                                                           + time surcharge 50%              + 0.009
                                                                                                             = 0.027

                                        IG + oversize                      0.018                               0.018
                                                                           + special surcharge 100 %         + 0.018
                                                                                                             = 0.036

                                        IG + shape + oversize              0.018                               0.018
                                                                           + time surcharge 50%              + 0.009
                                                                                                             = 0.027
                                                                           + special surcharge 100 %         + 0.027
                                                                                                             = 0.054

                                        Triple IG                          0.018 x factor 2.5            0.018 x 2.5
                                                                                                             = 0.045

                                        Triple IG + shape                  0.018 x factor 2.5                0.0450
                                                                           + time surcharge 50%            + 0.0225
                                                                                                           = 0.0675

                                        Triple IG + oversize               0.018 x factor 2.5                  0.045
                                                                           + special surcharge 100 %         + 0.045
                                                                                                             = 0.090

                                        Triple IG + shape + oversize       0.018 x factor 2.5                0.0450
                                                                           + time surcharge 50%            + 0.0225
                                                                                                           = 0.0675
                                                                           + special surcharge 100 %       + 0.0675
                                                                                                           = 0.1350
4.02 / 01-2017




                                        These examples show the sequence in which factors, surcharges, and special
                                        surcharges are included in the calculation.


                 A+W Business Pro Capacity Planning                                                            H-63
                 Master Data                                                                                      Tutorial




                               Transition Matrix and Transition Times
                               In addition to the time for the work process, the units also need time to move
                               from one production area to the next.
                               These times are entered as dwell and transition times on the following dialogs:
                               •   Production area:
                                   How long does a unit remain in a production area? The duration is entered
                                   in days or fractions of days.
                                   For this entry, the subsequent production area is not considered.
                                    Software Reference, “Production Area” on page H-195
                               •   Transition times:
                                   How much time does a unit need to move from one work type to the next
                                   or from one production area to the next? The duration is entered in shifts.
                                    Software Reference, “Transition Times” on page H-192
                               •   Transition matrix:
                                   How much time does a unit need to move from one production area to the
                                   next? The duration is specified in days or fractions of days.
                                    Software Reference, “Transition Matrix” on page H-210
                               If for the time calculation of an order item, entries are found on all three dia-
                               logs, the program will use the larger value. Also, the number of shifts will be
                               considered in which the individual areas work.
                               Shifts and days can also be entered in values <1. The length of time eventually
                               depends on the shifts and the times defined for this workday in the calendar.

                                   Example

                                   If the value 0.1 (shifts) has been entered for the transition time, there is
                                   exactly one shift between the work processes.


                                Software Reference, “Examples for the calculation of the transition” on page H-211

                                   Considering order priority
                                   If in addition to the order priority Normal the priority Urgent shall be consid-
                                   ered, a special transition time must be defined for the corresponding com-
                                   bination of production areas. This applies to all times that can be shortened
                                   for rush orders if required. If these have not been defined, the order will be
                                   scheduled with Normal priority.
4.02 / 01-2017




                 H-64                                                        A+W Business Pro Capacity Planning
                 Tutorial                                                                                             Master Data




                                                 Interaction of Dwell and Transition times

                  Sequence of                       Cutting                       Heat-soak                    Shipping
                  production


                  Specifications for               No entries                Production area dialog            No entries
                  dwell, transition                                           Dwell days: 0.2 days
                  time                                                      Transition matrix dialog
                                                                             Transition time: 1 day



                  Planning                      Thursday shift 1                Thursday shift 1             Friday shift 1

                  (for 3 shifts)                                               Dwell time: 1 day


                                                  Transition to                   Transition to
                                                production area:                production area:
                                                 from Cutting to               from Heat-soak to
                                                    Heat-soak                      Shipping
                                                    in shift 1                     in shift 3




                 Fig. H-40         Example 1: Dwell days in the area + transition matrix


                                                 After cutting on Thursday in shift 1, the item remains in the Heat-soak produc-
                                                 tion area for one day before it moves into Shipping on Friday in shift 1. The
                                                 larger value (1 day) from the transition matrix is used instead of the dwell days
                                                 (0.2 days) in the production area.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                           H-65
                 Master Data                                                                                                   Tutorial




                                                In case of a later cutting, the transition to the next production area is post-
                                                poned accordingly:


                  Sequence of                      Cutting                       Heat-soak                     Shipping
                  production


                 Settings for                     No entries                Production area dialog             No entries
                 dwell, transition                                           Dwell days: 0.2 days
                 time                                                      Transition matrix dialog
                                                                            Transition time: 1 day



                 Planning                      Thursday shift 3                 Friday shift 1                Friday shift 3

                 (for 3 shifts)                                               Dwell time: 1 day


                                                 Transition to                   Transition to
                                               production area:                production area:
                                                from Cutting to               from Heat-soak to
                                                   Heat-soak                      Shipping
                                                   in shift 3                   Friday shift 3




                 Fig. H-41        Example 2: Dwell days in the area + transition matrix


                                                After cutting on Thursday in shift 3, the item would reach Heat-soak on Friday
                                                in shift 1, and Shipping on Friday in shift 3.
4.02 / 01-2017




                 H-66                                                                        A+W Business Pro Capacity Planning
                 Tutorial                                                                                              Master Data




                                                 This example looks different if the TG is to be installed into an IG unit, and a
                                                 transition time has been defined for the following work type:


                  Sequence of                       Cutting                       Heat-soak                       IG line
                  production


                  Settings for                     No entries                Production area dialog
                  dwell, transition                                           Dwell days: 0.2 days
                  time                                                       Transition time dialog
                                                                            Transition time: 3 shifts



                  Planning                      Thursday shift 1                Thursday shift 1

                  (for 3 shifts)                                            Transition time: 3 shifts


                                                  Transition to                   Transition to           Following work type IG:
                                                production area:                production area:               Friday shift 2
                                                from Cutting to                from Heat-soak to
                                                   Heat-soak                        IG line
                                                   in shift 1                   Thursday shift 3




                 Fig. H-42         Example 3: Dwell days in the area + transition time


                                                 After cutting on Thursday in shift 1, the TG could reach the following area on
                                                 Thursday in shift 3, but will be installed in the IG not before shift 2 on Friday
                                                 because the transition to the following work type takes 3 shifts.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                            H-67
                 Master Data                                                                                                 Tutorial




                                                In case of a later cutting, the transition to the next work type is postponed ac-
                                                cordingly:


                  Sequence of                      Cutting                       Heat-soak                        IG line
                  production


                 Settings for                     No entries                Production area dialog              No entries
                 dwell, transition                                           Dwell days: 0.2 days
                 time                                                       Transition time dialog
                                                                           Transition time: 3 shifts



                 Planning                      Thursday shift 3                 Friday shift 1

                 (for 3 shifts)                                            Transition time: 3 shifts


                                                 Transition to                   Transition to            Following work type IG:
                                               production area:                production area:                Monday shift 1
                                               from Cutting to                from Heat-soak to
                                                  Heat-soak                        IG line
                                                  in shift 3                    Friday shift 3




                 Fig. H-43        Example 4: Dwell days in the area + transition time


                                                If the TG is cut in shift 3 on Thursday, it will not be installed in the IG before
                                                shift 1 on Monday.
                                                You will find more calculation examples in:
                                                 “Date Calculation” on page H-109
4.02 / 01-2017




                 H-68                                                                        A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Master Data




                                        Formula for Transition Time
                                        If, for example 50 sheets have to be transferred from cutting to the washing
                                        area, days or shifts are insufficient for calculating the exact time. In these cas-
                                        es, it is possible to enter a formula that considers the number of sheets.




                                                                                                                           A




                                                        B


                                        A Formula for transition matrix           B Content of the formula 500 (excerpt)
                                        Fig. H-44     Transition matrix and formula


                                        In this example, you see that the formula 500 has been entered for the change
                                        from TG production to shipping. This formula defines that the time is set to 1
                                        (= 1 day). From a quantity of 11 upwards, calculation shall be based on 3 days.
                                        To select the formula on the Transition matrix dialog, place the cursor in the
                                        Transition time field and press the right mouse key.
                                        The formula itself is entered in A+W Business Pro Master data > Company >
                                        Formulas. The formula can be entered and edited on the Formula manage-
                                        ment > Forms tab.
                                        If you are going to work with formulas, please contact a member of the service
                                        team of A+W Software GmbH.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-69
                 Master Data                                                                                        Tutorial




                                            Setup Times
                                            Setup times are defined as work type and allocated to the machine and the
                                            processing. This requires the following steps:
                                            •   Enter the work type Setup time.
                                            •   Allocate the work type Setup time as type Basic time to the machine, e.g.
                                                the CNC machine.
                                            •   Enter an individual time with the unit Qty (once), because the machine is
                                                set up just once per work process.
                                            •   Allocate the work type to the product classes produced on the machine,
                                                e.g. product class Processings/Corner cut-outs on the CNC machine.
                                            •   Define the production line so as not to calculate the setup time for subse-
                                                quent processings twice.




                                   A                                          B           C           D
                 A Machine                           B Work type Setup time             C Next machine
                                                                                        D Total lock
                 Fig. H-45     Lock work type setup time for next machine


                                            In this example, you see that the setup time for the CNC machine is skipped if
                                            the next machine is also the CNC machine. The machine will be defined once
                                            for all subsequent processings.
                                            If, however, the CNC machine must be set up anew for the following process-
                                            ing, the setup times must be defined and calculated separately. They can be
                                            locked by defining a production line.
4.02 / 01-2017




                 H-70                                                               A+W Business Pro Capacity Planning
                 Tutorial                                                                                     Master Data




                                        Time Factors for Series
                                        It may take less time to produce series, e.g. because set-up times are reduced
                                        or not required. The machine is available earlier in that case and can be
                                        scheduled for the next order.
                                        For this time calculation, you create serial tables with the factors for series pro-
                                        duction.

                                                    A          B




                                        A Graduated quantities                    B Time factor per graduation
                                        Fig. H-46       Series factors


                                        In this example, you see a graduated reduction for calculating the time require-
                                        ment. The actual amount of the reduction depends on the default time for the
                                        corresponding work process.
                                        Serial tables are not based on a certain machine or work type. If you want to
                                        use different reductions for production with particular work types, you have to
                                        create several tables for series. Choose a term that makes clear what the table
                                        shall be used for, e.g. Drilling series.
                                        To use the series factors for calculation you have to define the table that is to
                                        be used on the Machine and Special technical restrictions dialogs.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-71
                 Master Data                                                                           Tutorial




                               Define Default Times
                               Before entering the default times, you should make a plan taking into account
                               the following questions:
                               •   Which work types can each of your machines perform. Which work type
                                   can the new machine perform.
                               •   Which unit shall be used to enter the time, e.g. time per metre, per edge,
                                   per surface.
                               •   Are you going to enter the time taken (basic time) or a time surcharge.
                               •   Are you going to enter the time as individual time or with graduation.
                               •   Which limit types and limit values shall be used for the time graduation.

                                   Tip
                                   If you have previously selected the default time for an equivalent machine
                                   or an equivalent work type, you can adopt the data as pre-population and
                                   edit them.
                                   In the following action sequences, time will be defined completely anew.

                               This includes the following training sessions:
                               •   “How to specify the basic data for the default time” on page H-72
                               •   “How to enter the times for a work type” on page H-74


                                How to specify the basic data for the default time
                               1 Select in the module Capacity planning > Master data > Default Times >
                                 Default Times.




                                   Fig. H-47    Create default time for work type


                                   This dialog is described in the Software Reference.
4.02 / 01-2017




                 H-72                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                                  Master Data




                                        2 Select in the menu Start > New to change to entry mode.




                                        A
                                        B
                                        C




                                        A Select the work type and machine        C Priority
                                        B Type of the default time
                                        Fig. H-48     Create default time: enter basic data


                                            The fields are released. They are pre-populated with the data for the first
                                            machine.
                                        3 First select the work type and then the machine (A).
                                            If a machine can perform more than one work type, you have to repeat the
                                            entire action sequence for every work type defining the appropriate times.
                                            Alternatively, you can define a new work type that includes all tasks that
                                            can be performed by the machine. This default time will be valid for the
                                            complete sequence of tasks.
                                        4 Select the type (B) of the default time.
                                            In this example, the selected type is Basic time. The procedure is the same
                                            for time surcharges and work processes.
                                        5 Define the priority (C).
                                            Based on the work type, the priority defines which machine shall be used
                                            to produce the order item in question.
                                        6 Define the format of the default time by selecting the appropriate tab.
                                            In this example, a graduated default time is entered. An individual time is
                                            entered in the same manner on the corresponding tab.
                                            The basic data has been entered now. You can proceed to enter the times.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-73
                 Master Data                                                                             Tutorial




                                How to enter the times for a work type
                               1 Change to the Matrix tab.
                                   Graduations and time are entered in the same manner on the Vector and
                                   Cube tabs.

                                                                C     D




                               A
                               B

                               A
                               B




                               A Limit value 1, limit value 2             C Row header
                               B Limit type 1, limit type 2               D Column header
                               Fig. H-49     Limit values for default times


                                   The limit types and the unit are pre-populated. You have to change them.
                               2 Select the limit types (B) 1 and 2, e.g. Thickness and sqm rectangle.
                                   Now enter the limit values for the graduation.
                               3 Open the context menu (right mouse key) of the column header (D).




                               4 From the context menu, select Insert > Before.
                                   The field for the limit value (A) is released.
4.02 / 01-2017




                 H-74                                                         A+W Business Pro Capacity Planning
                 Tutorial                                                                                   Master Data




                                        5 Enter the first limit value, e.g. 4.00 for the thickness, and use the <Tab> key
                                          to go to the next field.
                                           The new column is inserted.
                                        6 Repeat the steps 3 to 5 until you have entered the entire graduation for the
                                          limit type 1.
                                        7 Open the context menu (right mouse key) for the row header (C) and repeat
                                          the steps 4 and 5 for the limit type 2.
                                        8 Select in the menu Start > Save to save the data.
                                           The data are saved.
                                        9 Now enter the appropriate value in each cell of the time table.




                                        10 Check in the Time unit field whether the entry is selected correctly.
                                           In this example, the unit sqm is selected. This means that the times entered
                                           relate to the area, that is, e.g. 0.013 hr. per sqm.
                                        11 Select in the menu Start > Save to save the data.
                                           The data are saved. The new data are listed on the Time selection tab in
                                           the overview.




                                        Fig. H-50     New default times created
4.02 / 01-2017




                                        To create the graduation in the shape of a cube, please refer to the instructions
                                        on prices in the Master data part.


                 A+W Business Pro Capacity Planning                                                                H-75
                 Master Data                                                                           Tutorial




                               Create Special Time
                               You create special times as surcharges to be able to calculate particular fea-
                               tures, e.g. a surcharge for oversizes. You can consider two limit types per data
                               record. For surcharge tables, the limit types can change from record to record.
                               In the following examples, the table for size surcharges is copied and adjusted.
                               This includes the following training sessions:
                               •   “How to create a new surcharge table” on page H-76
                               •   “How to create additional levels for graduation of the surcharge” on
                                   page H-78


                                How to create a new surcharge table
                               1 Select in the module Capacity planning > Master data > Default Times >
                                 Special times.




                                   Fig. H-51    Creating a special surcharge


                                   If tables have been created before, you can select an entry. The sur-
                                   charge(s) will be applied to the new table.
4.02 / 01-2017




                 H-76                                                   A+W Business Pro Capacity Planning
                 Tutorial                                                                                   Master Data




                                        2 Select in the menu Start > New to change to the entry mode.




                                        A
                                        B




                                        A Freely-selectable number                B Name
                                        Fig. H-52     Creating a new table


                                            The fields are released. They are pre-populated with the entries of the se-
                                            lected table.
                                        3 Enter the number (A) and the designation (B) of the new table.
                                            For this, overwrite the entries in both fields.
                                        4 Select in the menu Start > Save to save the data.
                                            The data are saved.
                                        5 Enter the value for the new surcharge.
                                            You can overwrite the existing limit types and surcharges or add more en-
                                            tries.
                                        In this example, the new table is based on the size table. It is now to be adjust-
                                        ed for edge processing. In the following action sequence, therefore, the limit
                                        types and graduation will be changed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-77
                 Master Data                                                                               Tutorial




                                How to create additional levels for graduation of the surcharge
                               1 Display the surcharge you want to edit.




                                           A      B                A   B         C D             E
                               A Limit value 1, limit value 2              C Value of the surcharge
                               B Limit type 1, limit type 2                D Unit of the surcharge
                                                                           E Calculation basis of the surcharge
                               Fig. H-53       Graduated special surcharge


                               2 Change Limit type 1 (B) in the first row, e.g. to Thickness and Limit type 2,
                                 e.g. to Largest edge length.
                               3 Adjust the limit values (A) accordingly.




                                     A                                               B
                                  A Row header                               B Amount of the surcharge
                                  Fig. H-54       Edit surcharge


                                  In this example, no surcharge will be applied to glass thickness up to 5 mm
                                  and edge lengths of up to 1200 mm. With the same thickness, a surcharge
                                  of 50% (B) will be applied to edge lengths between 1201 mm and
                                  1800 mm.
4.02 / 01-2017




                                  The next levels shall refer to the same edge lengths, and a thickness of
                                  6 mm.




                 H-78                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                                   Master Data




                                        4 Overwrite the last row using the values required for the limit types, the limit
                                          values, and the surcharge.
                                           For the next level, a new row must be inserted.
                                        5 Double-click in the row header (A) of the last level.
                                           The context menu is displayed.




                                        6 Select the Insert entry.
                                           A new row is inserted. The limit types and the surcharge unit are pre-pop-
                                           ulated with the entries from the previous row.




                                           Fig. H-55    Adding new limit value


                                        7 Add the new limit value in the first field and adjust the entries in the other
                                          fields, if necessary.
                                        8 Use this process to define all required surcharge levels.
                                        9 Select in the menu Start > Save to save the data.
                                           The data are saved.

                                           Delete entries
                                           To delete an entry, select the appropriate command from the context menu.
                                           If you select the command in the menu Start > Delete, the entire table will
                                           be deleted.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-79
                 Master Data                                                                           Tutorial




                               Exercises
                               •   Enter the default times for your exercise machine.
                               •   Enter a surcharge for muntins with the factor 1.5.
                               •   Enter a special time for cutting wired glass with 2 limit values.
                               •   Enter a time surcharge for triple IG.
                               •   Enter a time surcharge for the setup time, which is calculated just once for
                                   series.


                               Additional information
                                Software Reference, “Serial Factors” on page H-191
                                Software Reference, “Transition Times” on page H-192
                                Software Reference, “Transition Matrix” on page H-210
                                Software Reference, “Default Times (dialog)” on page H-217
                                Software Reference, “Special Times” on page H-226
4.02 / 01-2017




                 H-80                                                  A+W Business Pro Capacity Planning
                 Tutorial                                                                                         Master Data




                                        Selection of Machines
                                        Objectives

                                        • Using restrictions and priorities of the machines so as to guarantee a smooth
                                          production flow.
                                        • Checking the settings in company data.


                                        Benefits

                                        • At automatic scheduling, machines are checked and selected based on whether
                                          they are technically up to performing the required tasks in time.


                                        Note

                                        Technical restrictions      Restrictions for the automatic selection of machines are
                                                                    entered on the Machines dialog and on the Special
                                                                    technical restrictions dialog.

                                        Automatic scheduling        When orders are automatically scheduled in capacity
                                                                    planning, the settings for priorities and restrictions are
                                                                    analyzed. After that, an appropriate free machine is
                                                                    searched.

                                        Utilization                 The possible utilization of a machine of the individual
                                                                    machines depends on the machine's capacity and the
                                                                    settings in company data. You should therefore leave
                                                                    some leeway for manual scheduling and for the
                                                                    processing of residue from the day before.

                                        Manual scheduling           An order can be scheduled manually if the utilization
                                                                    settings allow this.

                                        Default settings            Company data:
                                                                    • Capacity planning tab
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                        H-81
                 Master Data                                                                                                  Tutorial




                                              Priorities
                                              If the machines for a work type, e.g. drilling, are equivalent, the selection made
                                              by capacity planning depends on the priority defined for the machine and work
                                              type. If two machines for the same work type have the same priority, the pro-
                                              gram will choose the faster and more economic machine.
                                              Priorities can also be used to define that special machines, e.g. manual cut-
                                              ting, are omitted from automatic machine allocation.
                                              The priorities are specified on the Default Times dialog.

                                                  Priorities for equivalent machines
                                                  It is possible to assign the same priority to equivalent machines, e.g. if you
                                                  are using two Bystronic cutting tables. If these machines are allocated to
                                                  different order areas or clients, the selection is still clear. Equivalent ma-
                                                  chines whose selection is not restricted by other criteria, should have dif-
                                                  ferent priorities however.

                                              Alternative priorities
                                              Another way of controlling the selection are alternative priorities, which can be
                                              specified on the Special priorities dialog.


                             Order                                  Work type                                   Machine
                                                                                       Restrictions?

                             6 pcs                                    Drilling                              Drilling machine I
                                                                                                                   Prio. 9
                                                                                                               up to 10 pcs


                             40 pcs
                                                                                                            Drilling machine II
                                                                                                                   Prio. -2
                                                                                                              Special priorities
                                                                                                        starting with 11 pcs Prio 9




                 Fig. H-56      Special priority (example 5, dotted line = 40 pcs)


                                              In this example, you see that the drilling machine II has the priority -2. This
                                              means that it can only be selected manually. On the Special priorities dialog,
                                              however, it is specified that from a quantity of 11 upwards, it has the
                                              priority 9.This means that this machine will only be used for large quantities. It
                                              will not be selected automatically even if the drilling machine I is used to ca-
                                              pacity.
4.02 / 01-2017




                 H-82                                                                  A+W Business Pro Capacity Planning
                 Tutorial                                                                                      Master Data




                                        Restrictions
                                        A restriction limits the machine selection. This limitation can be due to the di-
                                        mensions, the glass thickness, the speed. A restriction specifies, for example,
                                        if a drilling machine can only be used up to a glass thickness of 12 mm. If the
                                        setup of a machine is very time-consuming, the use of the machine will depend
                                        on the quantity. Restrictions can be used to lock machines for certain work
                                        types.
                                        These simple restrictions are specified when creating the machine data. Com-
                                        plicated restrictions can be defined only by means of lock formulas.

                                           Example

                                           Grinding machine B shall only be used for shapes or very small and very
                                           large sheets because this machine is very slow.
                                           All rectangular sheets with a width of >200 and <2600 mm and a height of
                                           >300 and <1600 mm shall not be ground on this machine.
                                           This restriction can only be defined by means of a formula.

                                           In this case, enter the minimum and maximum values for which grinding is
                                           technically feasible on this machine, e.g. 40 to 3210 mm for the width and
                                           100 to 6000 mm for the height.
                                           The range in between (width > 200 and <2600 mm, height > 300 and
                                           <3600 mm) is locked by a formula.


                                        The result for this example could be summed up as follows:




                                                                                      A
                                                          B




                                                                                                   C


                                        A Technically feasible      B Selection of the          C Example for lock formula
                                          values                      locking formula             (excerpt)
                                        Fig. H-57     Technical restrictions and lock formula
4.02 / 01-2017




                                        In the master data for the machine, the values for width and height (A) are de-
                                        fined on the General tab according to the machine’s working dimensions, that
                                        is the entire area. The number for the lock formula (B) is entered in the Lock
                                        group.


                 A+W Business Pro Capacity Planning                                                                     H-83
                 Master Data                                                                              Tutorial




                               The lock formula itself is entered in A+W Business Pro Master data > Compa-
                               ny > Formulas. On the Formula management > Formula tab (C), the formula
                               can be defined and edited.
                               If you are going to work with formulas, please contact a member of the service
                               team of A+W Software GmbH.


                               Priority vs. Restriction
                               The different options of controlling the automatic selection of machines work
                               together. This already became clear in the example with the restriction formu-
                               la. However, machine selection can also be accurately controlled without for-
                               mulas:
                               •   A machine of priority 9 and the restriction quantity >10 will be selected only
                                   if the item contains at least 11 pieces. If the quantity is less than or equals
                                   10, the machine with the priority below will be selected.
                               •   If a machine with priority 9 cannot process any large sheets, it will be se-
                                   lected only for items with standard dimensions.
                               You can define these combinations on the Special priorities dialog.




                               Fig. H-58     Special priorities


                               In this example, you see that the CNC machine should be used for quantities
                               of more than 10 with priority 9 for drilling. By default, this machine only has
                               priority 4 for the work type Drilling.
                               If a restriction is violated when the order is scheduled, the machine will not be
                               used for this order. It cannot be selected manually either in this case because
                               it is not offered for selection.

                                   Available fields for check values (lock values)
                                   The input fields for check values have to be released for the machine types.
                                   When checks are enabled afterwards, you have to check all machines that
                                   belong to the changed machine type. At scheduling, check fields without
                                   entries will prevent the machine from being selected – even if it is suited for
                                   producing the item.

                                    Software Reference, “Machine Types” on page H-185
4.02 / 01-2017




                 H-84                                                    A+W Business Pro Capacity Planning
                 Tutorial                                                                                              Master Data




                                             Automatic Scheduling
                                             For automatic scheduling, the machines allocated to the corresponding work
                                             type will be selected. Several machines can be allocated to a work type, e.g.
                                             several drilling machines to drilling. The combination of work type and ma-
                                             chine results in the time required (reserved capacity) and the costs. The auto-
                                             matic selection of the drilling machine is, among other things, based on the
                                             free capacities, technical restrictions, and costs.
                                             The selection of a machine can therefore be controlled using the following set-
                                             tings:
                                             •   Priority of the machine (9 to -2)
                                             •   Work type
                                             •   Locking of the machine, e.g. for certain product types
                                             •   Restrictions that refer to the order item's requirements, e.g. dimensions,
                                                 quantity.
                                             In the following two figures, you can see how these settings interact. Priorities
                                             and restrictions will be explained afterwards in detail in separate sections.


                             Order                                  Work type                                   Machine
                                                                                          Restrictions?
                             6 pcs                                    Drilling                              Drilling machine I
                                                                                                                   Prio. 9
                                                                                                               up to 10 pcs
                                                                                           40




                             40 pcs
                                                                                             pc
                                                                                               s.




                                                                                                            Drilling machine II
                                                                                                                   Prio. 8
                                                                                                          Starting with 11 pieces



                 Fig. H-59     Priority and technical restrictions (example 1, dotted line = 40 pcs.)


                                             In the scheduled order, it is first checked which work type is to be performed.
                                             Based on the work type, the possible machines are determined and the pro-
                                             gram checks the existing restrictions. Machines that are not suited to produc-
                                             ing this item will not be offered for selection after this check. They will not be
                                             offered for manual selection either.
                                             In example 1, you see that the default machine with priority 9 (drilling
                                             machine I) is only activated for the first item. The restriction check has re-
                                             vealed that the 40 pcs of the second order item must not be produced on drill-
                                             ing machine I. Drilling machine II is selected. If there is a drilling machine III
                                             with the same priority, which can also produce large quantities, the program
                                             will decide based on costs, time required, and free capacities.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                               H-85
                 Master Data                                                                                                    Tutorial




                                              Exchanging the priorities of the two machines results in the following process:


                             Order                                  Work type                                     Machine
                                                                                            Restrictions?
                                                                                              Priority?
                             6 pcs                                     Drilling                               Drilling machine I
                                                                                                                     Prio. 8
                                                                                                                 up to 10 pcs


                             40 pcs




                                                                                                                   6 pcs.
                                                                                                              Drilling machine II
                                                                                                                     Prio. 9
                                                                                                            Starting with 11 pieces



                 Fig. H-60      Priority and technical restrictions (example 2, dotted line = 40 pcs.)


                                              Example 2 shows that the priority does not influence the selection of the ma-
                                              chine because the restriction check has revealed the machine that can be
                                              used for the quantities to be produced. Drill I is selected because of the quan-
                                              tity because less than 11 pieces are to be drilled in the first item.
                                              If the technical restrictions are changed now, the process is the following:


                             Order                                  Work type                                     Machine
                                                                                            Restrictions?
                                                                                              Priority?
                             6 pcs                                     Drilling                               Drilling machine I
                                                                                                                     Prio. 8
                                                                                                                 up to 10 pcs


                             40 pcs
                                                                                                                if no
                                                                                                              capacities
                                                                                                                 free


                                                                                                              Drilling machine II
                                                                                                                     Prio. 9
                                                                                                             Starting with 1 piece



                 Fig. H-61      Priority and technical restrictions (example 3, dotted line = 40 pcs.)


                                              The restriction check shows that both machines can drill the first item. Drill I is
                                              selected only if drill II has no free capacity. Drill I would never be chosen for
                                              producing the second item however.
4.02 / 01-2017




                 H-86                                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                                          Master Data




                                            To prevent individual sheets from being drilled by drill II, another restriction can
                                            be set in the dialog Special technical restrictions.




                                                                                                            A




                       B




                 A Restriction of the quantity on the machine             B Special restriction for the quantity
                 Fig. H-62    Restrictions and special technical restrictions


                                            The dialog Special technical restrictions serves to define the restrictions for a
                                            machine in connection with a work type. In our example, the quantity (A) for
                                            drill II remains unchanged (from 1 piece), but the special technical restrictions
                                            (B) define that it shall be used only from 11 pieces onward.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                       H-87
                 Master Data                                                                                                    Tutorial




                             Order                                  Work type                                     Machine
                                                                                           Restrictions?

                             6 pcs                                    Drilling                                Drilling machine I
                                                                                                                     Prio. 8
                                                                                                                 up to 10 pcs


                             40 pcs                                                                         6 pcs.




                                                                                                              Drilling machine II
                                                                                                                     Prio. 9
                                                                                                             starting with 1 piece
                                                                                                           Spec. techn. restriction
                                                                                                           Starting with 11 pieces




                 Fig. H-63      Special technical restrictions (example 4, dotted line = 40 pieces)


                                              This example shows that the special technical restrictions prevent the 6 pcs.
                                              from being drilled by drill II even if it has got priority 9 and can handle individual
                                              sheets. With these settings, drill II is also available for manual selection in con-
                                              nection with small quantities.
4.02 / 01-2017




                 H-88                                                                     A+W Business Pro Capacity Planning
                 Tutorial                                                                                              Master Data




                                               Machine Selection for Alternative Work Types
                                               The alternative work type can also be used for diverting large quantities. For
                                               this purpose, an alternative work type is defined which is going to be used for
                                               scheduling large quantities.
                                               Define an additional serial table with the factors for serial production. This ta-
                                               ble must be introduced to the machine at two points: In the Machine dialog and
                                               in the Special technical restrictions dialog.
                                               Example 3, Automatic selection shall take serial production into account now.


                             Order                                   Work type                                    Machine
                                                                                          Restrictions?

                             6 pcs                                     Drilling                               Drilling machine I
                                                                                                                     Prio. 9
                                                                Alternative work type:
                                                                    drilling series                              up to 10 pcs


                             40 pcs



                                                                    Drilling series                           Drilling machine II
                                                                                                                     Prio. 9
                                                                                                            Starting with 11 pieces




                 Fig. H-64      Alternative work type for series (dotted line = series)


                                               Drill I will be selected only if the quantity does not exceed 10. For work type
                                               Drilling, the alternative work type Serial drilling has been defined. Drill II is al-
                                               located to this work type. The diversion is therefore triggered by the work type
                                               although both machines have got priority 9. Drill II is allocated to the series ta-
                                               ble in which the times for series production are graduated.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                                H-89
                 Master Data                                                                                    Tutorial




                               Locks
                               Locks have to be defined e.g. to avoid certain work steps from being executed
                               twice, or to avoid controlling a machine the performance of which is too low for
                               a certain product.
                               •   Products or product groups or product classes can be locked for certain
                                   machines, e.g. TG can be locked for cutting because a toughened sheet
                                   will never be cut.
                               •   Machines can also be locked for following processing steps.
                               •   If a machine can e.g. perform several work types, it does not have to be
                                   locked completely but just for one of the work types.
                               •   Machinery locks are customer-related and can also be defined based on
                                   the work type.

                                   Examples

                                   • If the drill washes the glass automatically, the glass does not have to be
                                     washed again before being toughened. To prevent this second wash
                                     cycle you can define a lock.

                                   • A customer insists that his sheets be drilled only by a certain machine.
                                     All other drills will therefore be locked for this customer.


                               Depending on how the work types and machines have been specified you can
                               define the lock for the first example in different ways:
                               •   Dialog Skip next machine:
                                   At the Drill you define that the Washer shall be skipped.
                               •   Dialog Skip processes:
                                   At the Drill you define that the work type Washing shall not be executed.
4.02 / 01-2017




                 H-90                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                                         Master Data




                                           Dialogs for locking
                                           Work types that shall not be performed for certain product classes can be
                                           locked by allocating the machine.


                                                                                 B              C             D



                 A




                 A Product class A+W Business Pro B Work types locked for the            C Locked machine for work type
                   master data                      product class                        D Total lock
                 Fig. H-65   Total lock of the TG product class for automatic cutting


                                           By combining the product class and the work types, a machine can be locked
                                           completely or partly. A total lock (D) means that the machine is locked even if
                                           the product class including the work type is part of a bill of material, e.g. TG as
                                           part of an IG unit. Capacity planning will not search for an alternative machine
                                           in that case.
                                           All lock dialogs have the same structure but differ with regard to the lock type.
                                           The different locks and their characteristics are therefore briefly sketched be-
                                           low:
                                           •   Lock by PGR:
                                               This kind of lock is set for product groups which are not to be produced by
                                               a certain machine.
                                           •   Lock by product class:
                                               This lock is set for product classes for which a certain work type shall not
                                               be produced by the defined machine. You can thus define that the work
                                               type for this product class is performed by an alternative machine.
                                           •   Lock machines by product:
                                               This type of lock is set for products for which a defined work type shall not
                                               be performed by a certain machine. You can thus control that this work type
                                               for the product is performed by an alternative machine.
                                           •   Skip next machine:
                                               This lock is set if a work type executed by a certain machine already in-
                                               cludes the following work type. If e.g. the drill also washes the sheet, the
                                               Washer will be locked.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                     H-91
                 Master Data                                                                            Tutorial




                               •   Customer-related locks:
                                   This lock is set for customers if certain processing steps are to be executed
                                   by an alternative machine. The machine with top priority will be locked in
                                   this case.
                               •   Define production line:
                                   This lock is set if certain work types are not going to be charged in connec-
                                   tion with a defined machine, e.g. if the set-up time for a CNC machine shall
                                   not be charged twice for successive processing steps.
                               •   Skip processes:
                                   This lock is set if a process at a machine also includes the following work
                                   type. If e.g. the drill also washes the sheet, the Washer can be skipped.

                               Lock machine completely
                               You can lock a machine completely e.g. when you have entered a new ma-
                               chine but have not made all of the entries. In this case, go to the dialog Ma-
                               chine and tick the checkbox Locked.

                               Lock machine temporarily
                               A machine can be locked temporarily, e.g. for maintenance work. Scheduled
                               orders will be rescheduled.

                                                        A         B                          C




                               A Locked machine                         C Orders which have already been
                               B Duration of the lock                     scheduled have to be rescheduled
                                                                          manually.
                               Fig. H-66     Lock machine temporarily
4.02 / 01-2017




                 H-92                                                   A+W Business Pro Capacity Planning
                 Tutorial                                                                                          Master Data




                                            Define Production Line
                                            A work type can be locked if it also occurs on the next machine.

                                               Example

                                               The CNC machine performs the work types corner cut-out and edge cut-out.
                                               For both product groups, the work type Set-up time has been entered with a
                                               factor of 1.2.

                                               If an order includes corner cut-outs and edge cut-outs, the CNC machine will
                                               be set up just once. The time must be charged only once in this case.


                                             How to define a production line
                                            1 Select in the module Capacity planning > Lock > Define production line.
                                            2 Select in the menu Start > New to change to the recording mode.
                                               The fields are released.
                                            3 Select the machine, e.g. the CNC machine.




                 A
                                                                                                                              B




                 A Machine on which the lock is set up                    B Details about the lock
                 Fig. H-67    Machine for production line


                                               This dialog is described in the Software Reference.




                                                            A     B              C       D
4.02 / 01-2017




                                               A Insert new row                          C Select next machine
                                               B Open combo box for selection            D Lock work type for next machine
                                               Fig. H-68        Select the work type and machine



                 A+W Business Pro Capacity Planning                                                                       H-93
                 Master Data                                                                                       Tutorial




                                             4 In the Machines group, click the [New] button (A).
                                                The row is released.
                                             5 Click in the Work type field and from the combo box (B) select the work type
                                               that you want to lock.
                                                In this example, this is the setup time.
                                             6 Select the next machine (C).
                                                In this example, the next machine is the CNC machine, because the follow-
                                                ing processing is also performed on it.
                                             7 Tick the Total checkbox (D) to completely lock the work type.
                                             8 Select in the menu Start > Save to save the data.




                 Fig. H-69     Machine for production line


                                                The set-up time will be charged just once if more than one processing step
                                                is performed. It will be charged again however for a new order item (with
                                                different sizes).
4.02 / 01-2017




                 H-94                                                                A+W Business Pro Capacity Planning
                 Tutorial                                                                                      Master Data




                                           Default Settings for Machine Selection
                                           The settings for utilizing the shifts have already been introduced in the session
                                           on Shifts and working time.
                                            “Default Settings for Shift and Capacities” on page H-43
                                           This session introduces the settings for selecting the machine.




                 A




                 A Type of selection of a machine
                 Fig. H-70    Company data – Capacity planning


                                           If you are using several machines which can perform the same work types,
                                           scheduling can consider these machines in different ways:
                                           •   Automatic:
                                               The program automatically searches for the most cost- and time-effective
                                               machine and schedules the orders on this machine. This is the default set-
                                               ting.
                                           •   Semi-automatic:
                                               The program offers the alternative machines for selection. If the delivery
                                               date cannot be adhered to, you must intervene.
                                           •   Manual:
4.02 / 01-2017




                                               With this option, every possible change (machine, shift, etc.) requires man-
                                               ual intervention. Alternative machines can only be selected for manual
                                               scheduling or rescheduling.


                 A+W Business Pro Capacity Planning                                                                   H-95
                 Master Data                                                                            Tutorial




                               These settings only apply to automatic scheduling. If orders are always sched-
                               uled manually, the machines have to be selected manually as well.

                                  Changing settings
                                  If you have changed settings in the company data, you should restart
                                  A+W Business Pro.


                               Additional information
                                Software Reference, “Default Settings in Company Data” on page H-179
                                Software Reference, “Special Technical Restrictions” on page H-212
                                Software Reference, “Special Priorities” on page H-227
                                Software Reference, “Lock” on page H-246
                                Software Reference, “Machine Failure” on page H-287
4.02 / 01-2017




                 H-96                                                 A+W Business Pro Capacity Planning
                 Tutorial                                                                                           Master Data




                                        Allocate the A+W Business Pro Master
                                        Data
                                        Objectives

                                        •   Using allocations for particular products or classes of products.
                                        •   Specifying production sequence.
                                        •   Considering particularities for shapes and processings.
                                        •   Increasing or reducing the times required with factors.


                                        Benefits

                                        • The production sequence is determined based on the allocation of the necessary
                                          work types.
                                        • Due to the allocation of A+W Business Pro master data, business organisation
                                          specifics can be taken into account, e.g. identical machines as part of different
                                          production lines.


                                        Note

                                        Production sequence           Per work type, it must be specified in which sequence
                                                                      these are performed. For example, on a rectangular
                                                                      sheet, the edges 1 and 3 and then the edges 2 and 4 are
                                                                      processed.

                                        Explicit allocations          For an explicit (direct) allocation, the product is assigned
                                                                      to the appropriate work type in capacity planning from
                                                                      the master data, e.g. the product Polish edges to the
                                                                      work type Polish edges.

                                        Implicit allocations          For an implicit (indirect) allocation, e.g. the product type
                                                                      Single glass is assigned to the work type Cutting. Even if
                                                                      there is no product Cutting in the A+W Business Pro
                                                                      master data, it is clear that the single glass must be cut
                                                                      to the respective order dimension.

                                        Default settings              Product master data
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                         H-97
                 Master Data                                                                                  Tutorial




                               Production Sequence
                               Basic products are created in the A+W Business Pro master data, e.g. single
                               glass, LG, TG, surcharges, shapes, muntins, etc. These products have to be
                               allocated to the work types and machines to define the production sequence.
                               We distinguish explicit and implicit allocations:
                               •   With explicit (direct) allocation, the product group Rounded corners is e.g.
                                   allocated to the work type CNC processing.
                               •   With implicit (indirect) allocation, the product type Single glass is e.g. allo-
                                   cated to the work type Cutting. Even if there is no product called Cutting in
                                   A+W Business Pro master data, it is clear that the single glass has to be
                                   cut to the appropriate order size.
                               You can allocate several work types. You also define the sequence in which
                               these work types are going to be performed.

                                   Example: product type TG

                                   •   Wash glass
                                   •   Check
                                   •   Produce TG
                                   •   Package processed TG
                                   •   Load



                                           Work type                                          Product type


                                            Cutting                                            Single glass



                                            Washing                                                LG



                                           Produce IG                                          Processings



                                            Dispatch                                                IG




                               Fig. H-71      Examples for allocations of work types to product types


                               Not every allocation makes sense however: The work type Dispatch has to be
                               allocated to the product type Single glass for example because even a simple
                               float glass sheet can be shipped. Allocating Dispatch to Processing steps how-
                               ever does not make sense at all.
                               The different product types, product groups, etc. can be allocated to the same
4.02 / 01-2017




                               work types, e.g. the work type Dispatch applies to TG and LG as well as to fit-
                               tings.




                 H-98                                                     A+W Business Pro Capacity Planning
                 Tutorial                                                                                          Master Data




                                           The allocations are evaluated in the sequence in which the dialogs are ar-
                                           ranged:
                                           •   Product type
                                           •   Product group
                                           •   Product class
                                           •   Product
                                           •   Combined product type
                                           •   Special allocation (1 to 4)
                                           •   Combined product class
                                           •   Stock articles
                                           This means that the product types form the top level of the allocations. All oth-
                                           er allocations are exceptions thereof.

                                               Example

                                               Product type Single glass is allocated to work type Cutting. This means that
                                               all single glass sheets can be cut.

                                               Product group Wired ornamental can be allocated e.g. to work type Manual
                                               cutting.


                                           If no work type has been allocated (<n. e.>), the corresponding entry will be
                                           ignored,e.g. the product class Processing.

                                           Dialogs for allocations
                                           Work types that are not allocated cannot be performed on the products of the
                                           order. This means that you cannot produce a single IG unit if the work type
                                           Produce IG is not allocated.


                                                                           B        C           D



                 A




                 A Product type A+W Business Pro C Work types performed on the            D Factor (see IG example)
                   master data                     product type                            “Case Study IG and Shape” on
                 B Sequence of work types                                                   page H-60
4.02 / 01-2017




                 Fig. H-72   Allocation of the product type single glass




                 A+W Business Pro Capacity Planning                                                                           H-99
                 Master Data                                                                                           Tutorial




                                            Allocating the product types to the appropriate work types usually covers most
                                            cases. This allocation is quite a rough one however since e.g. the cutting of
                                            single glass is not as easy as this allocation lets us assume. Float glass is no
                                            problem but patterned glass can often be cut only manually.


                                                                                 B



                 A




                 A Product class A+W Business Pro master data          B Work type manual cutting
                 Fig. H-73     Assignment to the product class Patterned glass


                                            You have to allocate the product class Patterned glass to the work type Manual
                                            cutting as well. Work type Dispatch does not have to be allocated again be-
                                            cause dispatch has already been allocated by means of the product type.
                                            All allocation dialogs have the same structure but differ with regard to the allo-
                                            cation type. The different allocation types are therefore briefly described be-
                                            low:
                                            •   Product types:
                                                These allocations are defined for all work types that will be performed as a
                                                rule, e.g. Cutting, Dispatch.
                                            •   PGR:
                                                These allocations are made for product groups which require more work
                                                and therefore have to get a surcharge, e.g. the cutting of antique glass.
                                            •   Product class:
                                                This allocation is made for the product classes that shall be allocated to a
                                                different product type, e.g. for the cutting of wired ornamental glass which
                                                belongs to the product type Single glass.
                                            •   Products:
                                                This allocation is made for products for which the usual allocation of prod-
                                                uct type and/or product class shall not apply, e.g. triple IG and the work type
                                                Sawing.
                                            •   Combined product type:
                                                These allocations are made for individual products that can be part of a
                                                BOM (in the products of a product type), e.g. LG 6 mm as part of an IG unit
                                                (product type IG).
4.02 / 01-2017




                 H-100                                                               A+W Business Pro Capacity Planning
                 Tutorial                                                                                          Master Data




                                        •   Special allocations:
                                            – Special allocation 1:
                                                This allocation is made for the product type Processing which is fol-
                                                lowed by another processing step.
                                            – Special allocation 2:
                                                This allocation is made for the processing of shapes.
                                            – Special allocation 3:
                                                This allocation is made for edgework.
                                            – Special allocation 4:
                                                This allocation is made for the processing and following processing
                                                steps for shapes.
                                        •   Combined product group:
                                            This allocation is made for individual products that can be part of the BOM
                                            of a product (in a product group), e.g. the product Float 6 mm as part of a
                                            LG unit (product class Laminated glass).
                                        •   Stock article:
                                            This allocation is made for stock articles (articles taken from stock) which
                                            are just packed and shipped. As a result, this product class is e.g. sched-
                                            uled for dispatch, and the appropriate cost and time is calculated.

                                            Description of allocation dialogs
                                            For a detailed description of the dialogs please refer to the Software Refer-
                                            ence.


                                        Combined Product Type, Combined Product Class
                                        Products which are part of a bill of materials, or which influence a product
                                        group as a processing step, can be allocated differently. This means that the
                                        product can be allocated to different work types depending on the combined
                                        product type or combined product class in which it is used.

                                            Example

                                            Float glass is part of IG units, and part of LG. The cutting table for IG is
                                            located in the same hall as the IG line. The cutting table for LG is in the same
                                            hall as the LG production. This means that two different work types have to
                                            be defined, one each for the corresponding cutting type.

                                            You can therefore allocate the work type Laminated glass cutting to the float
                                            glass if it is part of the LG bill of material.


                                        When you have defined two work types for cutting, you can allocate the corre-
                                        sponding cutting tables to the work types (in Default Times). If there is a bot-
                                        tleneck at one cutting table however, the other will not be used because it has
                                        not been allocated to the other work type.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                       H-101
                 Master Data                                                                                                 Tutorial




                                  Allocation                           Work type                         Machine

                                  Product type:                                                        Cutting table I
                                                                         Cutting
                                  Single glass                                                             Hall A




                             Combined product class:
                                                                                                       Cutting table II
                                   if float 6 mm                        Cutting LG
                                                                                                           Hall B
                               in product class LG




                 Fig. H-74      Example: Cutting control for product class LG


                                                  Cutting table I is used to capacity with this. If a float glass sheet shall be cut
                                                  for a laminated sheet, cutting table I will be ignored, and cutting table II is cho-
                                                  sen.
                                                  Both dialogs for allocation are structured analogously. The Combination prod-
                                                  uct type dialog is used as an example here.


                                                  B                                    C



                 A




                 A Selected product                                             C Work types t allocated to the selected product
                 B Selected product is part of
                 Fig. H-75      Example for the allocation of work type to product


                                                  This example shows that product Float 4 mm (A) has been allocated to work
                                                  type LG cutting (C) if this is part of the product type LG (B).
4.02 / 01-2017




                 H-102                                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                                        Master Data




                                              Define Allocation
                                              In this example, a special allocation is made for the edge processings in
                                              shapes. It serves to explain nearly all steps that can occur in connection with
                                              allocations. The allocations in the other dialogs are made accordingly.


                                               How to specify a special allocation
                                              1 Select in the module Capacity planning > Allocation > Special allocation 4.
                                                 The dialog of the same name opens.
                                                 This dialog is described in the Software Reference.
                                              2 Select in the menu Start > New to change to the recording mode.




                 A
                 B
                 C




                 A Selection of the product            B Selection of the processing       C Selection of the shape
                 Fig. H-76    Fields for new special allocation released


                                              3 Select the A+W Business Pro master data:
                                                 •   Product, e.g. ornamental glass (A)
                                                 •   Processing, e.g. seaming (B)
                                                 •   Shape, e.g. shape with 2 rounded corners (C).
                                                 The data are displayed in the overview.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                   H-103
                 Master Data                                                                                          Tutorial




                                                          A                B



                                                                                                                     C




                 A Schematic sketch of the shape               B Insert fields               C Edges of the shape
                 Fig. H-77     Specifying special allocation


                                                 In the Identification group, a sketch of the shape (A) is displayed, from
                                                 which you can see the numbering of the edges and corners.
                                             4 Click in the Work types with edge allocation group on [New] (B) to enter the
                                               first work type.




                                             5 Place the cursor in the Work type field and select the first work type from
                                               the combo box, e.g. Hand cutting.
                                             6 Repeat step 4 and 5 to select the next work types, e.g. Seaming, Washing.
                                             7 Place the cursor in the Factor field and enter the factor by which this work
                                               type should be increased, e.g. 2.5.
                                                 This factor means that the time defined for seaming will be multiplied by 2.5
                                                 if a shape with two rounded corners is produced.
4.02 / 01-2017




                 H-104                                                                A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Master Data




                                        8 Tick the checkboxes in columns 1 to 6 to select the edges to be processed,
                                          to which the factor shall be applied.
                                           If the factor is not to be applied to all edges, you have to define a second
                                           allocation for the remaining edges.




                                           This example shows that edge 1 shall be processed first. No additional time
                                           will be charged for that. For edges 2 to 6, the required time will be increased
                                           by a factor.
                                        9 Check the sequence of the steps.
                                           If you select a line you can use the arrow buttons to move the work step up
                                           or down until the right sequence is achieved.
                                        10 Select in the menu Start > Save to save the data.
                                           The data will be saved. The sequence of work types has been fixed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-105
                 Master Data                                                                           Tutorial




                               Exercises
                               •   Specify the complete allocations for IG units with shape as shown in the ex-
                                   amples.
                                   This exercise is quite complex. Therefore, feel free to adopt the examples.
                                    “Case Study IG and Shape” on page H-60


                               Additional information
                                Software Reference, “Allocation” on page H-229
4.02 / 01-2017




                 H-106                                                 A+W Business Pro Capacity Planning
                 Tutorial                                                                         Capacity Planning




                                        Capacity Planning
                                        Orders have to be scheduled in capacity planning so that the time costs are
                                        calculated and production times can be planned. The dates will be calculated
                                        based on the settings you have made in master data.
                                        This session will show you how to determine dates, schedule orders, handle
                                        capacity problems, how to control automatic scheduling in general, and how
                                        to monitor the planning by means of the control unit.
                                        This includes the following learning sections:
                                        •   “Scheduling Orders” on page H-108
                                        •   “Production” on page H-131
                                        •   “Production Costs” on page H-153
                                        •   “Control Station” on page H-161
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                          H-107
                 Capacity Planning                                                                                 Tutorial




                                     Scheduling Orders
                                     Objectives

                                     • Get to know date calculation.
                                     • Recognize planning processes.
                                     • Get to know flow of scheduling.


                                     Benefits

                                     • Orders are usually scheduled by a work flow task. You will only have to intervene in
                                       case of bottlenecks. It is therefore essential to know the scheduling process in
                                       detail.


                                     Note

                                     Scheduling                  Scheduling always starts from the delivery at the
                                                                 customer's and calculates the production dates so that
                                                                 the produced goods do not have to be stored.

                                     Bottleneck                  Bottlenecks usually occur only at machines performing
                                                                 complex work types. Cutting for example is generally
                                                                 unproblematic.

                                     Residual quantities         Residue from the day before are items of which the
                                                                 production has not begun yet. Once the first sheet has
                                                                 been produced, the remaining quantities are no longer
                                                                 considered as residue.

                                     Closing time                Closing time defines the point in time up to which orders
                                                                 can be scheduled for a shift. This makes sure that the
                                                                 scheduled orders can actually be produced, and no
                                                                 residue remains for the next day.

                                     Default settings            Company data:
                                                                 • Capacity planning tab
4.02 / 01-2017




                 H-108                                                          A+W Business Pro Capacity Planning
                 Tutorial                                                                               Capacity Planning




                                        Date Calculation
                                        Scheduling starts from the delivery date, from which the individual processes
                                        are counted back. The explicit and implicit work processes defined in the bills
                                        of materials are scheduled for the most cost-effective, valid machine according
                                        to their chronological sequence and their position on the bills of materials. If
                                        this is used to capacity, another machine will be selected (automatically or
                                        manually).

                                        Backward scheduling
                                        Scheduling is based on the delivery date. The check for free capacities always
                                        starts with the last work type in the last shift before the delivery date, e.g. pack-
                                        ing in shift 2, then goes back to shift 1.
                                        If all machines are used to capacity for a work process on a certain day, the
                                        program tries to move the process to the day before, etc.

                                        Forward scheduling
                                        If all backward scheduling is to no avail, the program searches for a new de-
                                        livery date based on the next possible route day. Backward scheduling then
                                        starts again from that new date. This process can be repeated until scheduling
                                        is successful.

                                        Times for date calculation
                                        In addition to the production times of a machine, dwell and transition times are
                                        considered. These times were described in detail in the Default Times section.
                                        In summary, this concerns the following criteria:
                                        •   Change of the production area, e.g. from cutting to washing.
                                        •   Change of work type, e.g. from cutting a ticket window to fine polishing of
                                            the hole edge.
                                        •   Rest time in the production area, e.g. cooling off after the TG furnace.
                                        When the production area is changed, the definition in the Transition matrix di-
                                        alog will override the entry in the Production area dialog.
                                        If on both dialogs times are stored, the following must be observed:
                                        •   Produce LG and Saw LG are e.g. two work types performed in the same
                                            production area, Laminated glass. In this case, only the transition time de-
                                            fined in the Transition times dialog will be considered.
                                        •   TG production and Picking are two work types executed in different produc-
                                            tion areas. In this case, capacity planning will check the entries in the Tran-
                                            sition matrix dialog and the Transition times dialog. The higher value will be
                                            used.
                                        The following examples show how the definitions in the different dialogs influ-
                                        ence the calculation of the start of production. Our example is based on a com-
                                        pany working in three shifts as a standard. The production area Heat soak test
                                        only works one shift.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-109
                 Capacity Planning                                                                                                  Tutorial




                                               Example for dwell days
                                               This example shows only entries in the Production area dialog. If one dwell
                                               day each is set for every production area, this will influence the calculation of
                                               the start of production as follows.

                                               Work types             Cutting -> Heat-soak test -> Picking

                                               Calculation of         •    Delivery date is Friday.
                                               dates                  •    Heat-soak test on Wednesday in the 1st shift.
                                                                      •    Picking on Thursday in the 1st shift.
                                                                      •    Cutting (production start) on Tuesday in the 1st shift

                                               Tab. H-1           Settings for the dwell days example


                                                                          Time scheme 1




                                 Dwell days
                                                          1 day                           1 day                      1 day




                                                                                                                                      Delivery date Friday
                   Shifts of the production       1         2          3          1         0          0      1        2       3
                                      area


                             Production area           Cutting                        Heat-soak test                Picking




                          Day of the week             Tuesday                          Wednesday                   Thursday



                 Fig. H-78       Example with dwell days in the production area


                                               This example shows that the shifts will not be taken into account if one holding
                                               day has been defined per production area.
4.02 / 01-2017




                 H-110                                                                            A+W Business Pro Capacity Planning
                 Tutorial                                                                                             Capacity Planning




                                               Example for different transition times
                                               In this example, there are entries on the Transition matrix and Transition times
                                               dialogs. The start day of the production is calculated as follows.

                                               Work types             Cutting -> Heat-soak test -> Picking

                                               Calculation of         • The delivery date is Friday.
                                               dates                  • In the Transition matrix dialog, 0.1 days (= one shift) was
                                                                        entered for all production areas. Assuming that this route will
                                                                        be shipped in the second shift by default, picking can still be
                                                                        done in the first shift on Friday. Otherwise, picking takes place
                                                                        in the third shift on Thursday.
                                                                      • In the Transition time dialog, the value 3 is entered.
                                                                        Starting from picking which is done in the first shift on Friday,
                                                                        three shifts are counted backwards. Even if 0 has been
                                                                        entered for the heat soak test in shifts 2 and 3, these will be
                                                                        included in the reckoning. The heat soak test therefore starts
                                                                        only in the first shift on Thursday. The entry in the Transition
                                                                        matrix dialog is ignored because the entry in the Transition
                                                                        times dialog is higher.
                                                                      • Cutting (start production) is done in the third shift on
                                                                        Wednesday because the transition from production area
                                                                        Cutting to the heat soak test has been defined as 0.1 days
                                                                        (= one shift) in the Transition matrix dialog.

                                               Tab. H-2          Settings for the transition times example


                                                                        Time scheme 2


                         Transition matrix
                      between production
                                    areas                                  0.1                        0.1           0.1

                 Transition times between                                   0                             3           0
                                work types                                                                                            Delivery date Friday



                   Shifts of the production       1          2         3         1         0          0       1      2        3
                                      area


                             Production area              Cutting                    Heat-soak test               Picking




                             Day of the week          Wednesday                        Thursday                    Friday



                 Fig. H-79       Example with transition times
4.02 / 01-2017




                                               This example shows how the shifts are taken into account for calculation.




                 A+W Business Pro Capacity Planning                                                                                 H-111
                 Capacity Planning                                                                                         Tutorial




                                             Example for transition times for several work processes in one
                                             shift
                                             The start of production is determined as follows.

                                             Work types        Cutting -> Grinding -> Screen printing -> Picking

                                             Calculation of    • The delivery date is Friday.
                                             the dates         • 0.1 days (= one shift) has been entered in the Transition
                                                                 matrix dialog. If this route is shipped in the second shift,
                                                                 picking can be done in the first shift on Friday. Otherwise,
                                                                 picking takes place in the third shift on Thursday.
                                                               • The entry in the Transition time dialog is 2.
                                                                 Starting from picking which is done in the first shift on Friday,
                                                                 two shifts are counted backwards. Silk screening therefore
                                                                 starts in the second shift on Thursday.
                                                                 The entry in the Transition matrix dialog is ignored because
                                                                 the entry in the Transition times dialog is higher.
                                                               • The entry in the Transition matrix dialog for the transition from
                                                                 production area Grinding to production area Silk Screening is
                                                                 0.1 days (= one shift). Grinding starts in the first shift on
                                                                 Thursday.
                                                               • Cutting (start of production) is done in the same shift as
                                                                 grinding because the entry in the Transition matrix dialog is 0
                                                                 (= same shift).

                                             Tab. H-3     Settings for the transition times example


                                                                 Time scheme 3



                         Transition matrix between
                                  production areas                           0.1              0.1            0.1

                    Transition times between work                                0                2               0
                                            types                                                                              Delivery date Friday



                      Shifts of the production area                      1           2        3        1      2        3




                                  Production area                      Cutting
                                                                                 Grinding
                                                                                     Screen printing       Picking


                                  Day of the week                                Thursday                   Friday



                 Fig. H-80    Example with different work types in the same shift
4.02 / 01-2017




                                             This example shows a calculation where several work types can be performed
                                             on the same day.



                 H-112                                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                                 Capacity Planning




                                        Scheduling
                                        There are three ways of scheduling orders in capacity planning:
                                        •   Manually, per order
                                        •   Manually, per number manager
                                        •   Automatically, in batch operation.
                                            In this case, the orders are entered in capacity scheduling via work flow
                                            task. The program will automatically search for new orders in defined inter-
                                            vals.

                                        Manual scheduling
                                        For manual scheduling, the defaults can be set so that you can trace every sin-
                                        gle step by scheduling the order items individually to different machines. In
                                        general, you will want to set the default so that intervention is only required in
                                        case of bottlenecks.
                                        Manual intervention is necessary if you are not satisfied with the scheduling
                                        results. Orders will have to be rescheduled in that case.
                                        Rescheduling may also be necessary if a machine breaks down and needs to
                                        be repaired.
                                        For manual scheduling, you can e.g. define the earliest start of production.

                                            Example

                                            If an order entered in September with a delivery date of 25.11. is to be
                                            produced so that the finished units do not have to be stored, you can enter a
                                            date for the earliest start of production.


                                        Automatic scheduling
                                        A work flow task (batch program) can be used to schedule orders automatical-
                                        ly for production. The program will automatically search for free machines. De-
                                        pending on the setting you will have to intervene only in case of bottlenecks,
                                        e.g. if machine A is used to capacity while machines B and C are not.
                                        You can use the Control unit dialog to intervene in scheduling, and reschedule
                                        items to another machine or another date.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                    H-113
                 Capacity Planning                                                                          Tutorial




                                     Settings for the work flow task
                                     Work flow tasks serve to process orders automatically. If manual intervention
                                     between two successive work flow tasks is necessary, depends on how the
                                     processes in your company are organized. The necessary settings are made
                                     during the installation A+W Business Pro and should not be changed after-
                                     wards. This paragraph therefore only explains the basic principles.
                                     A work flow task consists of one or more customizing formulas. These formu-
                                     las define the individual actions to be performed. The A+W Business Interface
                                     Service executes the task at a fixed time or in intervals.
                                     Three steps are necessary for defining a work flow task:
                                     •   Define the formulas in Master data > Company > Formulas. For capacity
                                         planning purposes, these can be e.g. formulas for searching for orders:
                                         – to be scheduled
                                         – left over from the day before (residue)
                                     •   Allocate the formulas to a work flow task in Master data > Company >
                                         Customizing > Work flow tasks tab.
                                     •   Set the starting time or interval for the work flow task in Master data >
                                         Company > Customizing > Autom. process execution tab.
                                     If you want to define work flow tasks, please ask a member of the A+W Soft-
                                     ware GmbH team for support.

                                         Transfer to production
                                         Orders are not automatically transferred from capacity planning to produc-
                                         tion. The transfer to production is handled by a separate work flow task.


                                     Capacity Problems
                                     Cutting usually causes no problems because it is done right at the start of the
                                     production chain. Capacity bottlenecks can occur easily however if a process
                                     is more complex, e.g. in connection with shapes or IG production.
                                     If (automatic) scheduling encounters capacity bottlenecks, manual interven-
                                     tion should be possible. You can of course make the default settings so that
                                     any order can be scheduled by means of automatic postponement of delivery
                                     dates. Manual intervention permits however to move less complex orders in
                                     favour of others.
4.02 / 01-2017




                 H-114                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                                  Capacity Planning




                                           Item split
                                           Apart from postponing dates, large items can also be split if shift times and ma-
                                           chine utilization require this. Production of an item will be split into several
                                           shifts and/or days this way.
                                           Splitting items into sub-items offers the following options:
                                           •   You can enter the quantity for every sub-item required.
                                           •   You let the program create the necessary sub-items.
                                           In the following example, 100 IG units with two rounded corners shall be pro-
                                           duced. This is a total of 400 rounded corners for which a total time of
                                           13.66 hours must be scheduled. The machine works 8 hours a shift. This
                                           means that the item must be split.




                 Fig. H-81   Exceeding of the machine capacity – Splitting


                                           From 100 sheets in order item 3, two sub-items of 50 sheets each are created
                                           for cutting and processing. Splitting is not required for the cutting process. It is
                                           done however so that the cut sheets do not have to be stored before process-
4.02 / 01-2017




                                           ing.




                 A+W Business Pro Capacity Planning                                                                    H-115
                 Capacity Planning                                                                                      Tutorial




                                     The production of 100 IG units is distributed as follows.

                                     SI       Glass / unit           Machine                         Date

                                     SI 1     Glass 1                Cutting 50 sheets               Shift 2 on 08/02

                                              Glass 2                Cutting 50 sheets               Shift 2 on 08/02

                                              Glass 1 + Glass 2      Rounded corners on 100          Shift 1 on 08/03
                                                                     sheets

                                              IG production          50 pcs                          Shift 1 on 08/04

                                              Picking/shipping       50 pcs                          Shift 1 on 08/05

                                     SI 2     Glass 1                Cutting 50 sheets               Shift 1 on 08/03

                                              Glass 2                Cutting 50 sheets               Shift 1 on 08/03

                                              Glass 1 + Glass 2      Rounded corners on 100          Shift 1 on 08/04
                                                                     sheets

                                              IG production          50 pcs                          Shift 2 on 08/04

                                              Picking/shipping       50 pcs                          Shift 1 on 08/05

                                     SI = sub-item


                                     Reserving production times
                                     In the splitting process, the remaining time of a shift can be locked for other
                                     orders. This prevents the machine from being set up again in the course of a
                                     shift.
                                     You can also define the production date. This is especially useful if the produc-
                                     tion times for the different processes differ considerably.

                                          Example

                                          10 oversized IG sheets have to be produced.
                                          All sheets can be cut on the same day. The IG line can only produce one
                                          unit of this size per day. This means that the cut sheets have to be stored
                                          up to 9 days.

                                          Splitting creates 10 sub-items (= one IG sheet per day) for which you define
                                          the production dates.
                                          Every sub-item will be cut separately and is produced on the IG line the
                                          same day.
4.02 / 01-2017




                 H-116                                                            A+W Business Pro Capacity Planning
                 Tutorial                                                                                Capacity Planning




                                        Closing Time
                                        Obviously, items cannot be produced completely if they are scheduled at the
                                        end of a shift. Since unfinished items have to be produced the next day (as res-
                                        idue from the day before), you should define times for the last scheduling.
                                        The closing time defines the point in time up to which orders can be scheduled
                                        for a shift. This makes sure that the scheduled orders can actually be pro-
                                        duced, and no residue remains for the next day.

                                           Example

                                           You receive a new order on Friday 12 a.m. In manual scheduling you enter
                                           2 p.m. although the shift ends at 4 p.m. This means that the order will not
                                           be scheduled because it cannot be produced that day.
                                           If the order cannot be scheduled because of the closing time, the dialog
                                           Delivery date issues a message to that effect. You will have to change the
                                           delivery date.


                                        Closing times are generally defined in the dialog Shift settings. In case of bot-
                                        tlenecks, manual intervention can be used to check the times.
                                         “Shift Settings” on page H-183
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                      H-117
                 Capacity Planning                                                                                       Tutorial




                                              Default Settings for Automatic Scheduling
                                              The settings for the number of shifts and the degree of utilization in company
                                              data have been introduced in the section on Shifts and working times. This de-
                                              scription is completed by the machine settings in the section on Machine Se-
                                              lection.
                                               “Default Settings for Shift and Capacities” on page H-43
                                               “Default Settings for Machine Selection” on page H-95
                                              In addition to these settings, you have other setting possibilities for controlling
                                              automatic scheduling.


                                                                         A




                                                                                                                            D
                                                                                                                            C
                 B




                 A Search for delivery date                               C Force scheduling
                 B Shift filling                                          D Do not split orders
                 Fig. H-82    Company data – Capacity planning


                                              If you permit that orders are split at automatic scheduling you must also define
                                              how much of the machine capacity can be used (B). This is not necessary if
                                              you prevent automatic scheduling (D). Please consider however that an order
                                              item can be so big that its production exceeds the capacity of the machine. The
4.02 / 01-2017




                                              order cannot be scheduled and manual intervention is required.




                 H-118                                                                 A+W Business Pro Capacity Planning
                 Tutorial                                                                               Capacity Planning




                                        Choosing of the delivery date
                                        The program can automatically search for a new delivery date in case of bot-
                                        tlenecks. A route day (A) should be chosen as the next delivery date. The sug-
                                        gested date can be changed manually for rush orders, e.g. if a special route is
                                        used for delivery. This setting only makes sense however if you have defined
                                        routes and allocated them to the customers.
                                        You can also force the scheduling of an order to match the delivery date stated
                                        in the order (C). With this setting, orders will be scheduled without searching
                                        for an alternative delivery date, no matter if capacities are available or not. This
                                        can result in frequent residue from the previous day. Real scheduling will hard-
                                        ly be possible in this case.

                                            Change settings
                                            If you have changed settings in the company data, you should restart
                                            A+W Business Pro.


                                        Schedule Order
                                        Orders are usually capacity-scheduled by a work flow task. You can schedule
                                        all orders of a number manager or every single order manually.
                                        The steps below describe the manual scheduling of a single order. The follow-
                                        ing session will tell you how to solve possibly occurring scheduling problems.
                                         “Solve Capacity Problem” on page H-126

                                            Scheduling impossible
                                            The order cannot be scheduled if it is being processed by another user and
                                            therefore open in Documents module at the time.
                                            To schedule capacities beyond the turn of the year, you have to enter the
                                            calendar for the new year including all shift times.

                                            Reschedule an order
                                            To schedule an order once more, you have to delete the old scheduling
                                            first. This applies especially if the order has been manually reported com-
                                            plete by mistake, and therefore has to be rescheduled.

                                        This includes the following training sessions:
                                        •   “How to schedule an order” on page H-120
                                        •   “How to schedule an individual order item” on page H-124
                                        •   “How to delete an order from capacity planning” on page H-125
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-119
                 Capacity Planning                                                                      Tutorial




                                      How to schedule an order
                                     1 Select Production > Capacity planning > Schedule > Schedule order.




                                        Fig. H-83   Schedule order


                                        This dialog is described in the Software Reference.
                                     2 Enter the order number and press the <Tab> key.
                                        The order is loaded.
                                     3 Select on the menu Functions > Group settings > Date search to check the
                                       criteria for the scheduling.
4.02 / 01-2017




                 H-120                                                     A+W Business Pro Capacity Planning
                 Tutorial                                                                             Capacity Planning




                                            In this example, the following settings are selected so that the scheduling
                                            can be traced step by step:
                                            •   Automatic normal capacity for the determination of the production date.
                                            •   Manual for the selection of the machines.
                                        4 Click [OK] to apply the settings and close the dialog.




                                        A
                                        B
                                        C
                                        D




                                        A Priority -1 = machines for manual     C Specify start of production
                                          selection                             D Priority from the order
                                        B Delivery date from the order must not
                                          be changed
                                            Fig. H-84    Schedule order manually


                                        5 Specify whether the machines for manual selection (A) are to be consid-
                                          ered in the search for free capacities.
                                            For especially urgent orders, this setting makes sense, because the ma-
                                            chines with the priority -1 are not considered otherwise.
                                        6 Specify whether the delivery date (B) from the order should be adhered to
                                          or whether it may be changed in case of bottlenecks.
                                            If you have ticked the checkbox, the delivery date may not be changed.
                                            This can mean that other orders must be rescheduled to free up the re-
                                            quired capacities for the current order.
                                            If you do not tick the checkbox, the delivery date may be changed accord-
                                            ing to the free capacities. The changed date is written back to the order.
                                            The new delivery date is searched for according to the route if you have se-
                                            lected the setting this way in the company data.
4.02 / 01-2017




                                            If the order should not be produced until later, specify the date for the pro-
                                            duction start (C).



                 A+W Business Pro Capacity Planning                                                               H-121
                 Capacity Planning                                                                          Tutorial




                                     7 Check whether the priority from the order (D) should be adopted or
                                       changed.
                                        If you change the setting, the new priority will only be adopted and written
                                        back to the order if you have confirmed the change in Functions menu >
                                        Apply priority to order.
                                        The change of the priority only makes sense if the appropriate transition
                                        times for all priorities are set up.
                                     8 Select in the menu Start > Execute to start the scheduling.
                                        If there are bottlenecks during scheduling, the following dialogs are dis-
                                        played:
                                        •   Delivery date
                                        •   Machine selection in case of bottleneck
                                        The procedure for resolving bottlenecks will be described in the following
                                        sequences.
                                        During scheduling, it is displayed which item or sub-item is scheduled with
                                        which work type.
4.02 / 01-2017




                 H-122                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                               Capacity Planning




                                              For large quantities, the scheduling runs through several phases until an
                                              optimal result has been achieved.
                                              Thus the order is completely scheduled. Usually it is now transferred to pro-
                                              duction via a work flow task.
                                              You can have the result displayed.
                                          9 Select in the menu Functions > Scheduling result to do this.




                    Fig. H-85   Result of the scheduling
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-123
                 Capacity Planning                                                                            Tutorial




                                      How to schedule an individual order item
                                        If an order item has subsequently been changed, it can be scheduled sep-
                                        arately. The other items of the order remain scheduled unchanged.
                                     1 Select Production > Capacity planning > Book > Book order.
                                     2 Enter the order number and press the <Tab> key.
                                        The order is loaded.
                                     3 Check the shipping date and correct it if necessary.

                                                                                      A                   B




                                        A Schedule individual item            B Number of the item
                                        Fig. H-86    Scheduling order item manually


                                     4 Tick the Schedule individual item checkbox (A).
                                        The field for the number of the item is released.
                                     5 Enter the number of the item (B).
                                     6 Select in the menu Start > Execute to schedule the item.
                                        In case of bottlenecks please stick to the following instructions for the com-
                                        plete order.
                                         “Capacity Problems” on page H-114
4.02 / 01-2017




                 H-124                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                         Capacity Planning




                                         How to delete an order from capacity planning
                                        1 Select Production > Capacity planning > Book > Book order.
                                        2 Enter the order number and press the <Tab> key.
                                           The order is loaded.




                                        Fig. H-87     Delete scheduling


                                        3 Select from the menu Functions > Delete scheduling.
                                           The scheduling data will be deleted. You can schedule the order once more
                                           now.
                                           This function also serves to delete orders from capacity planning which
                                           have already been reported complete.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                           H-125
                 Capacity Planning                                                                                  Tutorial




                                            Solve Capacity Problem
                                            If orders are scheduled automatically, intervention will be necessary only in
                                            case of capacity problems - and only provided that the appropriate settings
                                            were made in the company data.
                                            The following examples describe problems which can occur in connection with
                                            automatic scheduling or in connection with scheduling several orders from a
                                            number manager.

                                                Split item
                                                If you want to split an order item on all accounts, you have to schedule the
                                                order manually and choose the option Manual in the dialog Search date.

                                            This includes the following training sessions:
                                            •   “How to resolve bottlenecks when scheduling” on page H-126
                                            •   “How to split an item” on page H-127


                                             How to resolve bottlenecks when scheduling
                                                The Machine selection in case of bottleneck dialog is displayed if the cur-
                                                rent item cannot be scheduled.
                                            1 Check which item (A) on which machine (B) cannot be scheduled.


                                                                         A




                    B




                                                                     C                   D       E
                    A Item to be scheduled                               C Time required for the current item
                    B Machines where the bottleneck occurs.              D Schedule item
4.02 / 01-2017




                      Machine with priority -1 is marked in color        E Shift time of the machine is exceeded
                    Fig. H-88     Manual selection of the machine



                 H-126                                                              A+W Business Pro Capacity Planning
                 Tutorial                                                                                      Capacity Planning




                                           2 Check whether the scheduling for the date displayed is possible in another
                                             shift or on another machine.
                                              Using the arrow buttons, you can select another shift or another date.
                                              If no suitable capacities are found, you will have to split the item, i.e. divide
                                              it into several sub-items. This process is described below.
                                               “How to split an item” on page H-127
                                           3 Click [Schedule] (D) to schedule the item with the changed defaults.
                                              The items are scheduled and the process is repeated for the previous ma-
                                              chine.
                                           4 Repeat the steps until no more bottlenecks are displayed.
                                              The scheduling of the order is confirmed with a message.


                                            How to split an item
                                              The Machine selection in case of bottleneck dialog is displayed if the cur-
                                              rent item cannot be scheduled.


                                                                              A




                    B




                                C                                         D                           E
                    A Item to be scheduled                                    D Time required for the current item
                    B Machine where the bottleneck occurs                     E Shift time of the machine is exceeded
                    C Split item
                    Fig. H-89   Required time does not fit in one shift
4.02 / 01-2017




                                           1 Click [Split item] (C).




                 A+W Business Pro Capacity Planning                                                                      H-127
                 Capacity Planning                                                                              Tutorial




                                        A

                                        B




                                        C



                                        D


                                        A Order item                               C Specify production date
                                        B Number of shifts or quantity             D Overview of the bottlenecks
                                        Fig. H-90     Split order item


                                        This dialog is described in the Software Reference.
                                        On this dialog, you specify how the item is to be split. For this, you have the
                                        following possibilities:
                                        •   You specify the quantity that can be produced without a problem on all
                                            machines.
                                        •   You specify in how many shifts the total quantity should be produced.
                                            The quantities for appropriate sub-items are then calculated automati-
                                            cally.
                                            This version will be demonstrated in the following steps.
                                        •   You have the item split automatically by not specifying the quantity.
                                            – With [Qty = Shifts] the quantity will be distributed evenly across the
                                                possible shifts.
                                            – With [Qty = units per shift] the quantity will be divided up evenly so
                                                that the first shift is filled and the remaining quantity is produced in
                                                the following shift.
                                                For both variants, the split is only calculated for the machine on
                                                which the scheduling has come to a standstill.
                                        If you are not satisfied with the suggested split, you can delete the defaults
                                        and have the split calculated with new values.
                                     2 Click on the [Overview] button (D) to check where additional bottlenecks
                                       may occur.
                                        Based on this list you can determine the maximum size of the sub-items to
4.02 / 01-2017




                                        prevent bottlenecks at all the machines. When you have closed the dialog
                                        you can enter the number of sub-items.




                 H-128                                                        A+W Business Pro Capacity Planning
                 Tutorial                                                                              Capacity Planning




                                        3 Specify the quantity (B), e.g. 3.
                                           This value should relate to shifts.
                                        4 Click [Quantity = Shifts].




                                           A
                                                                                                            D
                                           B




                                           C




                                           A Enter quantity                        C Specify production date
                                           B Apply quantity for shifts             D Enter production date, shift
                                           Fig. H-91     Quantity and size of the sub-items


                                           Now you can specify an individual production date (C) for each item.
                                        5 Tick the checkbox (C) and enter the date and shift (D) for all sub-items.
                                        6 Click [OK] to confirm the splitting and close the dialog with [End].
                                           The order item is split according to your instructions.
                                           The Machine selection in case of bottleneck dialog is displayed again.
                                           Then the scheduling for each of the sub-items begins again with shipping.
                                        7 Click [Schedule] to schedule the sub-items.
                                           Scheduling continues and is interrupted when the next bottleneck is en-
                                           countered. Please note that the sub-items will be scheduled now and that
                                           it may be necessary to split them again in case of further bottlenecks.
                                        8 Repeat the steps 4 to 7 until no more bottlenecks are displayed.
                                           When you have split the sub-items so that no more bottlenecks occur,
                                           scheduling is completed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-129
                 Capacity Planning                                                                           Tutorial




                                     Exercises
                                     Use the orders you have entered in this exercise to check the settings you
                                     have made in capacity planning master data. It will therefore be useful if you
                                     enter as many complex orders as possible.
                                     •   Enter several orders:
                                         – Cutting of large quantities of single glass.
                                         – Several items with identical bills of materials but with different sizes.
                                         – Items with complex work steps, e.g. a shape as part of a stepped IG
                                            unit.
                                     •   Schedule the orders manually, using different modes (settings in the Mode
                                         Search Dates dialog):
                                         – Automatically
                                         – Manually
                                         – Schedule w/o checking
                                         Check the differences based on the scheduling result.

                                         Schedule an order several times
                                         You can schedule any order several times if no items have been produced
                                         yet. Delete the old scheduling result in this example before scheduling the
                                         order again but under different conditions.


                                     Additional information
                                      Software Reference, “Default Settings in Company Data” on page H-179
                                      Software Reference, “Schedule Number Manager” on page H-269
                                      Software Reference, “Change Criteria (Search Date)” on page H-272
                                      Software Reference, “Delivery Date” on page H-274
                                      Software Reference, “Book Order” on page H-275
                                      Software Reference, “Machine Selection in Case of Bottleneck” on page H-281
                                      Software Reference, “Split Items” on page H-284
4.02 / 01-2017




                 H-130                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                                 Capacity Planning




                                        Production
                                        Objectives

                                        •   Set up reports from production.
                                        •   Set up registration points.
                                        •   Check status reports in the order.
                                        •   Manually report orders completed.
                                        •   Reschedule residual quantities from the previous day.


                                        Benefits

                                        • The shop floor sends reports on the current status of the order items and thus, the
                                          order. The team in the sales department can check whether the delivery date of the
                                          order can be kept.
                                        • Delays due to breakage or production bottlenecks become evident based on the
                                          reports.


                                        Note

                                        Reports                      Production reports in A+W Business Pro serve to
                                                                     provide information on the production progress. The
                                                                     reports update the status of items and orders.

                                        Status reports from          The status of every single item changes during
                                        production                   production. When all items of an order have reached the
                                                                     same status, the order status is changed too.

                                        Completion report            To report an order complete, the registration point from
                                                                     which A+W Business Pro expects the port, must be
                                                                     defined and allocated in company data.

                                        Manual status allocation     Every (omitted) status report can be manually made up
                                                                     for. If reports have been omitted at several machines,
                                                                     they will all be reported complete with the newest
                                                                     reported date.

                                        Default settings             Master data:
                                                                     • Registration points
                                                                     Company data:
                                                                     • Stock/EK/EDI tab
                                                                     • Production tab
                                                                     • Capacity planning tab
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                    H-131
                 Capacity Planning                                                                            Tutorial




                                     Reports about Production Status
                                     Production reports in A+W Business Pro serve to provide information on the
                                     production progress. The reports update the status of items and orders.
                                     If you are using the production software A+W Production, orders can be trans-
                                     ferred to production after capacity planning. There is at least one registration
                                     point per production area on the shop floor. These registration points can re-
                                     port items or partial quantities to A+W Business Pro to change their status.
                                     The order status can be changed in the following ways:
                                     •   If you do not use A+W Production shop floor data collection (barcoding),
                                         you can manually report order items and orders complete.
                                     •   If you are using A+W Production barcoding, completion reports are sent to
                                         capacity planning and will raise the status of the order items. When all
                                         items have the same status, the order status is raised in the order header.
                                         Status reports are shown in the Report list dialog. This gives you a con-
                                         stantly updated overview of an order's production progress or of the pres-
                                         ent day.
                                     A process that is reported complete by A+W Production or manually, is fixed
                                     and cannot be changed in capacity planning. When the entire order has been
                                     reported complete, it appears in capacity statistics.
                                     Reports are created by A+W Production and loaded by the A+W Business Pro
                                     interface service (AIS). This program runs centrally on the server and checks
                                     the defined directories periodically for new items.

                                         Reports from production
                                         Reports from A+W Production can be received and edited by
                                         A+W Business Pro in different ways. This subject is described in detail in
                                         the section Production. In the tutorial on capacity planning, it will be ex-
                                         plained only briefly.
                                         File-less reporting can only be processed with A+W Production Capacity
                                         Planner.
4.02 / 01-2017




                 H-132                                                        A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Capacity Planning




                                            Settings for reports
                                            In the company data, you must check the settings for the production reporting.




                 A


                 B
                 C

                 D




                 E




                 A Production manager                                    D URL for the PPS Webservice
                 B Settings for production reports                       E URL for the ERP Webservice
                 C File-less reports
                 Fig. H-92    Master data – Settings for production reports


                                                A+W Business Pro
                                                The program version A+W Business Pro works with the production manag-
                                                er (A) by default. Thus file-less reports are not possible.

                                            The URL of the ERP-Webservice is valid for transfer to production and for pro-
                                            duction reports in OrderXML format. These settings are described in detail in
                                            the Production tutorial.
                                             Production: Tutorial, “Reports from Production” on page E-55
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                    H-133
                 Capacity Planning                                                                                   Tutorial




                                     Registration Points
                                     Completion of work steps in a production area is reported through barcode
                                     registration points. One registration point per production area will usually do.
                                     You can however set up two registration points in a production area.

                                        Example: TG dispatch

                                        One registration point is set up where the finished sheets are loaded onto
                                        racks, and one in the fittings stock where the fittings are arranged.
                                        Only when all items (glass as well as fittings) have the same status, e.g.
                                        540, the order is ready for dispatch and the order status is set to Goods
                                        shipped.


                                     Production reports from barcoding are expected, e.g. from the following sta-
                                     tions:

                                        Barcoding status             Meaning

                                        455                          Break in production
                                        460                          Cutting finished
                                        465                          Grinding finished
                                        470                          Drilling finished
                                        475                          Check
                                        480                          Screen printing finished
                                        485                          TG finished
                                        490                          LG finished
                                        495                          Bending finished
                                        500                          Heat-soak furnace finished
                                        510                          IG finished
                                        515                          Clear Shield finished
                                        540                          Ready for shipping


                                     Details on the current state of an order's and the items' production are provid-
                                     ed in the Report list dialog. It shows the production areas every item has
                                     passed so far, and those it still needs to pass.
                                     When an item has passed a production area and has been scanned at the reg-
                                     istration point, its status is raised. When all work steps in a production area
                                     have been completed for all items of an order, the order status is raised auto-
                                     matically. Since the processing machines are not going to be changed at that
                                     point, the costs will be recalculated and saved in the order.
4.02 / 01-2017




                 H-134                                                             A+W Business Pro Capacity Planning
                 Tutorial                                                                                 Capacity Planning




                                           Registration point for reports
                                           To analyze the reports from A+W Production in A+W Business Pro you have
                                           to allocate a registration point for the completion report. This allocation will be
                                           required for production reports and barcode reports.




                                                                                                                     A




                 Fig. H-93   Master data – Registration point for reporting


                                           If AWBar or A+W Production reports are sent to the files of the types STSP,
                                           STSL, STSD, STSB, STSG, you have to select a registration point that is allo-
                                           cated to a status point. If no such registration point has been allocated, the re-
                                           port will cause an error.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                      H-135
                 Capacity Planning                                                                           Tutorial




                                     Status Messages
                                     In capacity planning, status reports have to be allocated to the production ar-
                                     eas in which they are supposed to raise the item or order status. You can only
                                     allocate one status per production area.
                                      Software Reference, “Production Area” on page H-195

                                     Item and order status
                                     The order status changes after an order has been scheduled in capacity plan-
                                     ning. This change is recorded in the order history.
                                     Status allocation is different for items and orders. When an item is complete,
                                     its status changes to ready for dispatch, the order itself however is not ready
                                     for dispatch yet.

                                                 A           B




                                     A Status of the order                   B Status of the item
                                     Fig. H-94    Overview of production reports


                                     The order status is raised only when all order items have reached the status
                                     ready for dispatch.
4.02 / 01-2017




                 H-136                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                                  Capacity Planning




                                        Automatic status allocation in connection with different work
                                        types
                                        Items of an order can be quite different so that they undergo different work
                                        types before reaching a common item status.

                                           Example

                                           Only one of five items has to pass the production area Toughening furnace.
                                           If this is the only item that needs to be reported complete in this production
                                           area for this order, the status in the order header would normally be raised
                                           automatically when this item is reported complete at the toughening
                                           furnace.

                                           This must not happen however, as long as the other order items have not
                                           reached the same production status. These may still be in the Cutting area,
                                           for example, and have to pass the production area Drilling before the order
                                           status can be raised to Toughening furnace.
                                           Capacity planning therefore checks which production area has to be
                                           passed by the four items before they reach the toughening furnace, in this
                                           case the production area Drilling. Only when the four items have been
                                           reported complete in the production area Drilling, the order status is raised
                                           to Toughening furnace.


                                        Manual status allocation
                                        It may happen that registration points do not register the completion reports for
                                        items so that the status is not raised for the time being. When the item is re-
                                        ported completed by one of the following production areas however, capacity
                                        planning (not A+W Production) automatically assumes that the previous pro-
                                        duction area has been passed. The status will be raised automatically.

                                           Example

                                           Let us assume that the items have been reported complete by production
                                           area Drilling. Cutting always precedes drilling. If the item has not been
                                           reported complete in the cutting area, capacity planning still assumes that it
                                           has been cut and automatically raises the status for production area
                                           Cutting.
                                           Registration point Drilling however has no data on the cutting table used.
                                           The data for the start of production are missing as well. In this case, the
                                           data and costs are only updated for production area Drilling, not for the
                                           Cutting area. This is why completion reports should be duly made at the
                                           registration points.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                        H-137
                 Capacity Planning                                                                                   Tutorial




                                           Completion Report
                                           Orders and items are reported complete by reports from the shop floor.
                                           A completion report always assumes that the previous process has been com-
                                           pleted. If the appropriate completion report has been omitted, it will be made
                                           automatically. The program adopts the date of the latest completion report for
                                           the last area for which this report is missing. Logically, this date does not match
                                           the date on which the item was actually produced in that area.
                                           If you are not using the (automatic) reports from shop floor data collection (bar-
                                           coding), you can issue manual completion reports for orders or items for the
                                           different production areas, e.g. by batch, by date, or by order.




                                           Fig. H-95    Reporting cutting complete manually


                                           On the Control station dialog, the data will be updated accordingly.




                    A Open order                                                  B Order reported completed
                 Fig. H-96   Control station


                                           When the order is reported complete manually, all work steps that have not yet
4.02 / 01-2017




                                           been reported will be moved to the day of the completion report. In this case,
                                           the production dates are shown in green.
                                           The Control station dialog is covered in detail in a separate section.

                 H-138                                                              A+W Business Pro Capacity Planning
                 Tutorial                                                                               Capacity Planning




                                        Remaining Quantities from Previous Day
                                        When an order has been scheduled for the previous day but was not pro-
                                        duced, this residue must be rescheduled for the present day. A batch program
                                        (work flow task) searches for orders that have not been started yet and re-
                                        schedules them. Since this process requires quite a lot of processor capacity,
                                        the batch is defined as a work flow task and is automatically run outside work-
                                        ing hours, e.g. after midnight. For details on the work flow task please see:
                                         “Automatic scheduling” on page H-113
                                        Using status settings, the program searches for orders that should have been
                                        produced the day before. It checks whether production has already begun.
                                        The resulting orders will be rescheduled without a capacity check.

                                           Example workday 07/22

                                           Order A: 100 pcs, production start 07/21,
                                           on 07/21 20 sheets are cut.
                                           These items will not be taken into account: Work has already begun and the
                                           worker will resume it today (07/22).

                                           Order B: 30 pcs, production start 07/21.
                                           No sheet has been cut.
                                           The batch runs at 4:00 a.m. and reschedules the order for 07/22 (today).


                                        The status settings for the search for orders are usually made just once.




                                        Fig. H-97     Status for residual quantity transfer


                                        As a minimum status, the order must have been (successfully) scheduled in
                                        capacity planning. You cannot reschedule orders that have not been sched-
                                        uled yet.
                                        The maximum status (lock status) depends on your production organisation. If
                                        you print delivery notes only after an order has been reported complete, this
                                        print status could be the upper limit for the search. If you are using barcode
                                        reports, the lock status could also be roughly scheduled.

                                           Catching up
                                           If you realize that the scheduling of residue from the day before results in
                                           always new and ever increasing residue, you can aim at a lower use of ca-
                                           pacity when planning the next shifts. This will create a buffer for the re-
4.02 / 01-2017




                                           scheduled orders. Alternative remedies could be overtime, special shifts, or
                                           spending an entire day just catching up on those old orders.




                 A+W Business Pro Capacity Planning                                                                   H-139
                 Capacity Planning                                                                            Tutorial




                                     Breakage Report
                                     Production reports also include breakage reports. Examples of breakage re-
                                     ports are:
                                     •   Sheets broken after passing a registration point.
                                     •   Sheets with flaws that have to be reproduced.
                                     A+W Business Pro can consider breakage reports for status allocation only if
                                     a registration point has been allocated in A+W Business Pro master data.
                                      Master Data, “Registration Points Production” on page B-854

                                         Completion report before breakage report
                                         When a unit reaches the next production area, it has usually been reported
                                         complete at the previous registration point. The breakage report can be en-
                                         tered right away in that case.
                                         Please note that before a manual breakage report is made, a completion
                                         report must be issued. If this is missing, the unit must be reported complete
                                         first before the breakage report can be entered.
4.02 / 01-2017




                 H-140                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                                   Capacity Planning




                                             Print Production Papers
                                             The program can analyze which quantity of an order has to be produced by a
                                             certain machine, and when the order is expected to reach the next machine.


                                              How to print a list of the orders on a particular machine
                                             1 Select Production > Capacity planning > Completion report > Manual.




                 A




                 B




                                                                                 C
                 A Time period                                           C Selection of an individual machine
                 B Selection of the data
                 Fig. H-98    Settings for production list


                                                 This dialog is described in the Software Reference.
                                             2 In the fields from date and to date (A) enter the period of time for which you
                                               want to generate the list.
                                                 If you enter the same date in both fields, the list will be drawn up just for
                                                 that day.
                                             3 Tick the checkbox for the print settings (B) to list all machines.
                                                 To draw up the list for just one machine, select this machine (C).
                                                 If you change the settings after drawing up the list, you have to tick the
                                                 checkbox Reprint.
                                             4 Select in the menu Start > Search to start the search.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                     H-141
                 Capacity Planning                                                                                     Tutorial




                    A




                                              B
                    A Sub-items of order item 1                            B Order number
                    Fig. H-99      Detailed production list


                                                  For every work type, this list shows the sub-items of each item.
                                                  If you send the data to a printer, choose horizontal format to make sure that
                                                  all data are visible.
4.02 / 01-2017




                 Fig. H-100     Production list example (page 1)


                                                  One page is created per machine and day.



                 H-142                                                                 A+W Business Pro Capacity Planning
                 Tutorial                                                                             Capacity Planning




                                        Report manually Order completed
                                        The options for manual completion reports are:
                                        •   Complete orders
                                        •   Individual order items
                                        •   Sub-quantity of an order item
                                        In the following example, a sub-quantity is reported complete.

                                            Scanning
                                            If you are using a scanner please first go to menu Options and check
                                            whether barcode registration is active. If so, the cursor is automatically po-
                                            sitioned in the barcode field.


                                         How to report an order completed on a machine
                                        1 Select Production > Capacity planning > Completion report > Manual.
                                            The Manual completion reports dialog opens.
                                        2 Select in the menu Functions > Settings.




                                            Fig. H-101   Selection of the machines


                                            This dialog is described in the Software Reference.
                                        3 Select the machines for which you want to record the completion reports
                                          and apply the selection with [OK].
                                            You can select several machines.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-143
                 Capacity Planning                                                                             Tutorial




                                                                         B                A



                                     C
                                     D


                                     E




                                                                    F                           G
                                     A   Completion report option             E Quantity to be reported complete
                                     B   Field for barcode                    F Enable quantity specification
                                     C   Order number                         G Selection of the machine
                                     D   Item number
                                     Fig. H-102    Manual completion report


                                         This dialog is described in the Software Reference.
                                     4 Check whether the Completion report option (A) is activated.
                                     5 Specify the order number (C) or record the barcode.
                                         The cursor goes to the next field.
                                     6 In the from item field (D), enter the item number and press the <Tab> key.
                                         The item is loaded and the quantity displayed.
                                     7 Tick the With quantity checkbox (F).
                                         If you have scanned the barcode, just one sheet will be reported complete.
                                         You have to tick the checkbox and enter the number of completed sheets.
                                         To report the entire item complete, tick the checkbox Item complete. You
                                         do not have to enter the quantity in that case.
                                     8 Go to the Quantity field (E) and enter the quantity to be reported completed.
                                     9 Go to the Select machine field (G) and choose the machine where the
                                       quantity was completed.
                                     10 If necessary, add the date and the shift.
4.02 / 01-2017




                 H-144                                                         A+W Business Pro Capacity Planning
                 Tutorial                                                                                Capacity Planning




                                           A
                                           B




                                           A Partial quantity                       B Report completed
                                           Fig. H-103   Details for the manual completion report of a partial quantity


                                        11 Click [Report items completed (F9)].




                                           Fig. H-104   Partial quantity reported completed


                                           The specified quantity is reported completed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                      H-145
                 Capacity Planning                                                                             Tutorial




                                     Manual Breakage Report
                                     Breakage reports can be made only for items which have already been report-
                                     ed complete. The options for manual breakage reports are:
                                     •   Breakage report - entry:
                                         The defined quantities are reported broken at the machine entry. They
                                         have to be reproduced by the previous machine.
                                     •   Breakage report - exit:
                                         The defined quantities are reported broken at the machine exit. They have
                                         to be reproduced by the same machine.


                                      How to report breakage of an item
                                     1 Select Production > Capacity planning > Completion report > Manual.
                                         The Manual completion reports dialog opens.
                                     2 If necessary, select in the menu Functions > Settings the machine for which
                                       you want to record breakage reports.

                                                                                          A



                                     B
                                     C


                                     D




                                                                     E                          F
                                     A Completion report option              D Quantity of flawed sheets
                                     B Order number                          E Enable quantity specification
                                     C Item number                           F Selection of the machine
                                     Fig. H-105   Manual completion report


                                         This dialog is described in the Software Reference.
                                     3 Enter the order number (B) or record the barcode.
                                         The cursor jumps to the next field.
                                     4 Enter the item number (C) and press the <Tab> key.
                                         The item is loaded and the quantity is displayed.
4.02 / 01-2017




                                     5 Select the report type (A).
                                         This setting defines whether the defective sheets have to be reproduced by
                                         the previous or the same machine.


                 H-146                                                         A+W Business Pro Capacity Planning
                 Tutorial                                                                            Capacity Planning




                                        6 In the Quantity field (D), enter the quantity that you want to report complet-
                                          ed.
                                           If you have recorded the barcode via scanner, precisely 1 sheet is reported
                                           complete.
                                        7 In the Select machine field (G), mark the machine on which the breakage
                                          should be reported.
                                        8 If necessary, add the date and the shift.
                                        9 Click [Report items completed (F9)].




                                           Fig. H-106   Breakage report for partial quantity


                                           The data are saved. The confirmation is displayed below the button.
                                           When the rejected sheets have been re-produced, the item status is in-
                                           creased.

                                           Breakage report cannot be confirmed
                                           If the breakage report cannot be confirmed, you have to report the item
                                           complete first. After the completion report has been made, you can enter
                                           the breakage report.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-147
                 Capacity Planning                                                                           Tutorial




                                     Check Production Status
                                     You can check the production status of the orders in detail and add any omitted
                                     completion reports. To this end, you can view the orders for a customer or all
                                     orders for a certain delivery date.


                                      How to check the production status of individual order items
                                     1 Select Production > Capacity planning > Production status.




                                        Fig. H-107   Check production status of an order


                                        This dialog is described in the Software Reference.
                                     2 Enter the number of the order or the customer.
                                        You can enter the delivery date to restrict the selection even more. Alterna-
                                        tively, you can use this to view all orders for the defined date.
                                     3 Select in the menu Start > Search to load the data.
                                        The order data are loaded and displayed on the Selection tab.
                                        If you use the customer number as a selection criterion, all orders of this
                                        customer are shown, even the ones already produced.
                                     4 Change to the Items tab to check the production status of the individual or-
                                       der items.
4.02 / 01-2017




                 H-148                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                            Capacity Planning




                                                                             A                      B            C
                                           A Quantity of the item                 B Partial quantity reported completed
                                                                                  C Report item completed
                                           Fig. H-108   Check production status of the items


                                        5 Check the date for which you want to report the item completed.
                                        6 Tick the Report completed checkbox (C) for the item that has already been
                                          completely produced.
                                           A security message is displayed. When you have confirmed the message,
                                           the quantity of the item is displayed in the Completely finished column.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-149
                 Capacity Planning                                                                        Tutorial




                                     Catch up on Completion Reports
                                     You can view the residue from the day before to check if completion reports
                                     have been omitted.


                                      How to check if there is residue from the day before
                                     1 Select Production > Capacity planning > Control station > Functions
                                       menu > Display residual quantities.



                                                                                                             A



                                                                                                             B




                                        A Select minimum status                B Report order completed
                                        Fig. H-109   Display residual quantities and report completed


                                        This dialog is described in the Software Reference.
                                     2 Select the minimum status (A).
                                        The orders have to be at least scheduled in capacity planning. Therefore,
                                        a lower status does not make sense.
                                     3 Tick the Completion report checkbox (B).
                                     4 Click [OK] to save the data.
                                        The status of the orders is increased. The orders reported completed are
                                        deleted from the overview.
4.02 / 01-2017




                 H-150                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                               Capacity Planning




                                              On the Control station (order) dialog, you can check if the data were
                                              amended correctly. All additional completion reports are set for the present
                                              date.




                 Fig. H-110   Caught-up-on completion reports


                                              This dialog is described in the Software Reference.

                                              Show completed orders
                                              When making the settings for the control station you can define that orders
                                              which have been reported complete are not to be displayed. If you choose
                                              this option, you will not be able to check the status change as shown in this
                                              example.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-151
                 Capacity Planning                                                                        Tutorial




                                     Exercises
                                     •   Report completion of one of your orders manually.
                                     •   Report an item completed in one of your orders.
                                     •   Record breakage for one IG sheet. Consider thereby that the item or the
                                         order must be reported completed beforehand.
                                     •   Report the residual quantities from the previous day completed. You can
                                         only do this exercise if there are residual quantities.


                                     Additional information
                                      Software Reference, “Production Area” on page H-195
                                      Software Reference, “Residue Transfer” on page H-290
                                      Software Reference, “Date” on page H-292
                                      Software Reference, “Manual Completion Report” on page H-298
                                      Software Reference, “Production Level Orders” on page H-307
                                      Software Reference, “Report List” on page H-318
                                      Software Reference, “Utilisation (Date)” on page H-351
                                      Software Reference, “Residue Qty.” on page H-361
4.02 / 01-2017




                 H-152                                                     A+W Business Pro Capacity Planning
                 Tutorial                                                                                Capacity Planning




                                        Production Costs
                                        Objectives

                                        • Checking machine and time costs in the order or quotation.


                                        Benefits

                                        • Even before an order is produced, you can check whether the time and machine
                                          costs are sufficiently taken into account for pricing.


                                        Note

                                        Production costs            These are:
                                                                    • Wage costs per unit
                                                                    • Machine costs per hour
                                                                    • Variable costs per hour, e.g. for insurances
                                                                    These costs are stored per machine and checked during
                                                                    scheduling.

                                        Production in a quotation   To determine the production costs for a quotation, a work
                                                                    flow task must be defined which transfers the quotations
                                                                    to capacity planning.

                                        Actual costs                The actual costs are not determined until production,
                                                                    because only then it is decided which machines have
                                                                    actually been used. The actual costs are written back to
                                                                    the order with the reports.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                   H-153
                 Capacity Planning                                                                                   Tutorial




                                            Time Costs
                                            The program calculates the time costs for orders and - if required - for quota-
                                            tions. This way you can check before production whether the order can still be
                                            produced at a profit considering the expected time costs.
                                            Production cost calculation is based on the following details:
                                            •   Machine costs per hour
                                            •   Variable costs per hour, e.g. insurance costs
                                            •   Costs per unit of default time, e.g. labour costs per unit
                                            These costs are defined per machine and are checked at scheduling.




                                                                                                              A


                                                                                                              B




                 A Cost records                                        B Total costs per unit produced
                 Fig. H-111   Compilation of the costs for a machine


                                            The cost of an order item and for the entire order will be recalculated after the
                                            completion report. They can differ from the originally calculated costs, e.g. be-
                                            cause the order or item was produced by another machine than the scheduled
                                            one.
4.02 / 01-2017




                 H-154                                                               A+W Business Pro Capacity Planning
                 Tutorial                                                                             Capacity Planning




                                        On the Order production status dialog, you can display the current production
                                        costs.




                                                                     A                                     B
                                        A Planned production costs for the     B Productions costs incurred so far
                                          whole order
                                        Fig. H-112    Check current production costs
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-155
                 Capacity Planning                                                                                        Tutorial




                                            Cost Centres
                                            You can define special cost centres for analyzing the production costs. This
                                            way, you can analyze the costs for a defined period.




                 A                                                                                        B




                 A Sorting by                                              B Evaluation of the product types, product classes or
                   Production area – Order area or                           products
                   Order area – Production area
                 Fig. H-113   Evaluate cost centres for production costs


                                            This analysis lists the cost centres for product types. You can sort this analysis
                                            by cost centre or by order area.
                                            Cost centres and analysis can be defined according to your company's re-
                                            quirements. In the following examples, the last line of the analysis, Cost centre
                                            Processed TG shall be explained.

                                               Cost centres in A+W Business Pro master data
                                               Capacity planning cost centres are not connected with the cost centres de-
                                               fined in module Master data.
4.02 / 01-2017




                 H-156                                                                  A+W Business Pro Capacity Planning
                 Tutorial                                                                                    Capacity Planning




                                        Principle of the evaluation columns
                                        In each of the columns, it is specified what the query shall evaluate.

                                                                                  A        B         C   D            E




                                        A Main product type: number of the       C        Type 1, Type 2:
                                          product type from the A+W Business              0 = Not specified
                                          Pro master data                                 1 = Product type
                                        B No 1, No 2:                                     2 = Product class
                                          Number of the product class or product D        Priority (sequence of the query)
                                          type in the Type field                 E        Products that are excluded from the
                                                                                          evaluation
                                        Fig. H-114       Define cost centres


                                        With the combination of the columns No and Type you set what shall be
                                        searched for in the BOM.

                                           Example: evaluation of processed TG

                                                 MPT                  No 1        No 2         Type 1    Type 2    Priority
                                                     2                 20             0          1           0       19

                                             Main product:        Product type:                   1:
                                                  TG              Processings                  Product
                                                                                                type


                                        This example shows that the main product of product type TG (2) shall be
                                        searched for Type1 (i.e. Product type) number 20 (Processing). This means
                                        that this cost centre shall include only TG with processings.
                                        Before you start entering cost centres, you should decide in which sequence
                                        the cost centres are going to be checked. This sequence is defined in the col-
                                        umn Priority.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                       H-157
                 Capacity Planning                                                                                 Tutorial




                                        Example TG

                                        First you check whether this is a TG with processing (cost centre no. 7 with
                                        prio 19).
                                        If this is not the case, the next check is applied, that is prio 20.

                                        The TG that is not processed automatically goes into the cost centre TG
                                        (cost centre no. 6 with prio 20).


                                     The column Exclusion can be used to exclude a product from this rule by en-
                                     tering the product number. The product number must be entered in brackets.

                                        Example

                                        All TG sheets are seamed. Therefore, you do not want seamed TG sheets
                                        to flow into the cost centre TG with processing.
                                        You can exclude this by entering the product number for seaming.


                                     A detailed description on the definition of columns is found in the Production
                                     part. There, the definition of the preview columns is described, which follows
                                     the same principle.
                                      Production, “The concept of preview columns” on page E-153
4.02 / 01-2017




                 H-158                                                             A+W Business Pro Capacity Planning
                 Tutorial                                                                              Capacity Planning




                                        Cost Calculation in Orders
                                        A+W Business Pro calculates the material prices based on the purchase price.
                                        Apart from that, time and machine costs can be displayed in the order.
                                        These costs are calculated per order in capacity planning at scheduling and
                                        shown in the order.
                                        Material and time costs are shown in the order header on the Totals tab.




                                        Fig. H-115    Cost calculation: order – Totals tab


                                        The costs are displayed in the order header via the Functions menu > Docu-
                                        ments group > Cost and surcharge calculation.




                                        Fig. H-116    Cost calculation in the order


                                        Cost calculation for Quotations
                                        Quotations can be transferred to capacity planning with a special work flow
                                        task for cost calculation. This function permits to display the costs in the order
                                        header and at item entry just like in the order. Quotations will not be scheduled
                                        in capacity planning, and are not transferred to production.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-159
                 Capacity Planning                                                                         Tutorial




                                     Exercises
                                     •   Check whether the machinery costs are shown in the orders you have
                                         transferred to capacity planning.
                                         If costs are missing: Check whether you have entered the costs for the ma-
                                         chines. Add them if necessary and schedule the orders again. Then check
                                         if the costs are displayed.


                                     Additional information
                                      Software Reference, “Accounts” on page H-264
                                      Software Reference, “Cost Centre Definitions” on page H-265
4.02 / 01-2017




                 H-160                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                                Capacity Planning




                                        Control Station
                                        Objectives

                                        • Navigation on the Control station dialog.
                                        • Check utilization of the machines.
                                        • Reschedule orders or order items.


                                        Benefits

                                        • On the Control station dialog, you get an overview of the utilization of the
                                          machines.
                                        • You can use this dialog to access all programs for checking and rescheduling the
                                          orders.


                                        Note

                                        Control station             From the Control station dialog you can load all dialogs
                                                                    for checking and rescheduling.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                   H-161
                 Capacity Planning                                                                                  Tutorial




                                             Concept of the Control Station
                                             The Control station dialog provides an overview of the hours scheduled per
                                             machine and allows to change dates if required.


                                                        A




                  B




                           C
                 A Scheduled time for cutting         B Machines on which times have     C Orders to be processed by the
                                                        been scheduled.                    machines.
                 Abb. H-117    Planned times on the control station


                                             This example shows the utilization of production area Cutting (A) for one week.
                                             The detailed data for the individual machines in production area Cutting (B)
                                             and the orders (C) to be produced by a certain machine can be displayed in
                                             the Control station dialog.
4.02 / 01-2017




                 H-162                                                              A+W Business Pro Capacity Planning
                 Tutorial                                                                                 Capacity Planning




                                        The Control station dialog gives access to all programs for checking and re-
                                        scheduling orders. These are the following dialogs:
                                        •   Using the Functions menu:
                                            – Select order > Control station (order)
                                            – Display residual quantities > Residual quantities
                                            – Graphic display of the utilization
                                            – Utilization > Utilization on date
                                        •   Using Control station > Prev.processes tab:
                                            – [In Detail] > Production lists
                                        •   Using Control station (order) > Functions menu:
                                            – Overview of reports
                                            – Schedule > Schedule order
                                            – Manual defaults (Production level orders)
                                        On the Control station dialog, you navigate as follows:

                                        Tab                 Action                             Tab / dialog

                                        Areas               Double-click on row           ->   Machines (all machines)
                                                            header
                                                            Double-click on production         Machines (only machines in
                                                            area                               the production area)

                                        Machines            Double-click on machine       ->   Orders
                                                            Double-click on detail data        Reschedule order
                                                            Double-click on row                Control station (machine)
                                                            header

                                        Orders              Double-click on number        ->   Control station (order)
                                                            Double-click on detail data        Reschedule item

                                        Reschedule order    Click on row header           ->   Reschedule item
                                                            Click on [Elements] or        ->   Prev. processes
                                                            [Prev.processes]

                                        Reschedule item     Context menu for process ->        Delete setup time
                                                            (right mouse key)
                                                                                               Add setup time

                                        Work types          Click on row header           ->   Details

                                        Details             Double-click on number        ->   Control station (order)

                                        Prev. processes     Click on [In Detail]          ->   Production lists
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                      H-163
                 Capacity Planning                                                                                     Tutorial




                                             Control Station – Order
                                             To check the scheduling of the individual order, the Control station (order) di-
                                             alog is available.
                                             You reach the dialog via Control station > Functions menu > Select order.


                                                                                            A




                                                                     B
                 A Delivery date                                       B Shipping date
                 Fig. H-118   Control station for individual order


                                             This example shows the backdating process based on the delivery date: On
                                             the day before the scheduled delivery date, the order must reach the produc-
                                             tion area Dispatch to be packed. All other work is done before, taking into ac-
                                             count the production and transition times.
                                             Navigation in the Control station – Order dialog:

                                             Tab                     Action                           Tab / dialog

                                             Machines                Double-click on machine     ->   Move II
                                                                     Double-click on date             Detail

                                                                     Click on cell header        ->
4.02 / 01-2017




                                             Detail                                                   Work types




                 H-164                                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                                Capacity Planning




                                            Control Station – Machine
                                            To check the utilization of an individual machine, the Control station (machine)
                                            dialog is available.
                                            You reach the dialog via Control station > Machines tab > Double-click in row
                                            header.




                                                                       A                       B
                 A Machine                                             B Hours required
                 Fig. H-119   Control station for individual machine


                                            This example shows the orders including quantities and times required for the
                                            selected machine. The period shown matches the display in the Control sta-
                                            tion dialog from which you have accessed this dialog.
                                            The next tab shows the detailed times. You can change the displayed period
                                            so that you see the utilization e.g. for just one day.
                                            The sub-items generated by a splitting are listed individually. To move a sched-
                                            uling, you can change with a double-click on the order number to the Control
                                            station (order) dialog.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-165
                 Capacity Planning                                                                                  Tutorial




                                            Postpone Scheduling for single Order
                                            You want to check whether the shipping of an order can be postponed, e.g.
                                            due to a delay in the delivery of ordered elements.
                                            In this example, the shipping of an order shall be postponed by several days.
                                            This means that both the delivery date and the scheduling must be changed.


                                             How to check the scheduling of an order
                                            1 Select in the module Production > Capacity planning > Control station >
                                              Functions menu > Select order.
                                                The Control station – Order dialog opens.
                                            2 Enter the order number.
                                            3 Select in the menu Start > Search to load the data.




                                                                                                             B




                                                                                                             A




                 A Current delivery date                              B Shipping: completion one day before delivery date
                 Fig. H-120   Plan data for the current order


                                                This dialog is described in the Software Reference.
                                            4 Enter the new date in the Delivery date field (B).
4.02 / 01-2017




                                            5 Click [Change].
                                                The display will be updated the next time you open the dialog.


                 H-166                                                             A+W Business Pro Capacity Planning
                 Tutorial                                                                          Capacity Planning




                                        6 Select in the menu Functions > Schedule.




                                           Fig. H-121   Schedule order for new delivery date


                                           This dialog is described in the Software Reference.
                                           The order is shown with the new delivery date. It has not been scheduled
                                           for this date yet however. You can check this by using the button [Result]
                                           to open the dialog Scheduling result.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                           H-167
                 Capacity Planning                                                                          Tutorial




                                        Fig. H-122   Old scheduling


                                        This example shows that shipping is still scheduled for the old date. Sched-
                                        uling continues when you close the dialog.
                                     7 Select in the menu Start > Execute to reschedule the order.
                                        Scheduling starts. Depending on the setting, you have to confirm the deliv-
                                        ery date for the individual items. After successful scheduling you can view
                                        the result again.
4.02 / 01-2017




                 H-168                                                      A+W Business Pro Capacity Planning
                 Tutorial                                                                          Capacity Planning




                                           Fig. H-123   New scheduling


                                           This example shows that shipping is scheduled for the new date. All work
                                           steps at the previous machines have been rescheduled accordingly.
                                        8 Change back to the Control station (order) dialog.
                                           To update the display, you must load the order again.
                                        9 Select in the menu Start > Filter to change to the search mode.
                                        10 Enter the order number again and start the search to load the order.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                           H-169
                 Capacity Planning                                                                            Tutorial




                                                                                                                  A




                                                                                                                  B



                 A New delivery date                            B Shipping: completion one day before delivery date
                 Fig. H-124   Changed plan data for the order
4.02 / 01-2017




                 H-170                                                       A+W Business Pro Capacity Planning
                 Tutorial                                                                               Capacity Planning




                                            Change Machine
                                            You can move scheduled order items to another machine, e.g. from IG line I
                                            to IG line II.


                                             How to reschedule an order item on another machine
                                            1 Select Production > Capacity planning > Control station > Functions
                                              menu > Select order.
                                                The Control station (order) dialog opens.
                                            2 Enter the order number and start the search.
                                                The order data are loaded.




                 Fig. H-125   Plan data for the current order


                                            3 Double-click on the machine to open the control station for the machine.
                                                The Control station (machine) dialog is displayed with the Move II tab.
                                            4 Tick the checkbox for the item that is to be moved to another machine.
                                            5 In the Move group, select another machine.
                                                In addition, you can enter a new date and/or another shift.
4.02 / 01-2017




                                            6 With [Load] you can check whether the move makes sense.




                 A+W Business Pro Capacity Planning                                                                 H-171
                 Capacity Planning                                                                                 Tutorial




                 Fig. H-126   Check moves


                                            7 Select in the menu Start > Execute to start the action.
                                               The scheduling is moved. The change will be displayed after a restart of the
                                               dialog.
4.02 / 01-2017




                 H-172                                                             A+W Business Pro Capacity Planning
                 Tutorial                                                                               Capacity Planning




                                        Exercises
                                        •   Practice navigation on the control station:
                                            Starting point for the following exercises is always the control station. Close
                                            the dialog to execute the next exercise.
                                            – Have the machines for a production area displayed.
                                            – Change to the Control station (machine) dialog.
                                            – Change to the Control station (order) dialog.
                                            – Have the data displayed on the Detail tab.

                                            Tip for practicing navigation
                                            Print out the overview of the navigation. You will also find this in the soft-
                                            ware reference.

                                             “Navigation through the tabs and dialogs” on page H-307

                                        •   Change from the control station to an order and check the scheduling.
                                        •   Move the delivery date of an order by one week. What else do you have to
                                            do? When are the new dates displayed?
                                        •   Schedule an order with 10 large IG sheets so that only one unit per day is
                                            produced (item split and specification of production date).


                                        Additional information
                                         Software Reference, “Control Station (Dialog)” on page H-326
                                         Software Reference, “Control Station (Machine)” on page H-344
                                         Software Reference, “Control Station (Order)” on page H-362
                                         Software Reference, “Production Level Orders” on page H-307
                                         Software Reference, “Change Production Times” on page H-319
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-173
                 Capacity Planning                              Tutorial
4.02 / 01-2017




                 H-174               A+W Business Pro Capacity Planning
Capacity Planning                  H

                    Software Reference




              A+W Business Pro
                 Software Reference                                                                         Overview




                                        Overview
                                        Capacity planning in A+W Business Pro is organized in two areas:
                                        •   Management of capacity planning
                                        •   Planning and monitoring of capacities
                                        You will find the associated dialogs in the Capacity planning and Production
                                        modules.
                                        In this software reference, the dialogs from both modules are described in the
                                        following sections:
                                        •   “Administration” on page H-178
                                        •   “Capacity Planning” on page H-267
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-177
                 Administration                                                              Software Reference




                                  Administration
                                  In order to work with capacity planning in A+W Business Pro, the master data
                                  must be set up. These data are the basis for all allocations, scheduling, and
                                  analyses.
                                  This section provides information on the following master data:
                                  •   “Default Settings in Company Data” on page H-179
                                  •   “General” on page H-185
                                  •   “Organisation” on page H-194
                                  •   “Default Times” on page H-216
                                  Apart from the description of master data, you will find information on the fol-
                                  lowing subjects:
                                  •   “Allocation” on page H-229
                                  •   “Lock” on page H-246
                                  •   “Overviews” on page H-257
                                  •   “Scheduling” on page H-268
                                  •   “Production Reports” on page H-291
                                  •   “Control Station” on page H-325
4.02 / 01-2017




                 H-178                                                    A+W Business Pro Capacity Planning
                 Software Reference                                                                       Administration




                                           Default Settings in Company Data
                                           Master data > Company > Company data > Capacity planning tab




                 Fig. H-127   Company data – Capacity planning


                                           In the Master data module, you specify the basic settings for A+W Business
                                           Pro Capacity Planning. These settings mainly refer to automatic scheduling.
                                           In case of manual scheduling, you can overwrite them.

                                              Changing settings
                                              If settings were changed in company data and in capacity planning master
                                              data, you have to reboot A+W Business Pro to reload the data.

                                           Capacity planning

                                           Version For the selection of the program for capacity planning, you must pay
                                           attention to how you receive reports from production. If you want to work with
                                           Capacity Planning of A+W Business Pro, you must select the A+W Business
                                           Capacity Planning entry.
                                           This setting does not permit the use of online reports.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-179
                 Administration                                                                Software Reference




                                  Error message from automatic capacity planning
                                  With the selection of the option, you specify to whom error reports are sent.
                                  •   To operator:
                                      With this setting, the error messages are sent to the employee who had en-
                                      tered the order in question. Such error messages usually refer to dates that
                                      cannot be adhered to because there are not enough capacities available.
                                      This is the default setting.
                                  •   To employee:
                                      With this setting, the field for the selection of an employee is released. Se-
                                      lect this option if only a single employee processes the orders that cannot
                                      be scheduled without problems.

                                      Schedule orders automatically
                                      Usually the orders are scheduled in capacity planning automatically at
                                      specified intervals by a workflow task. This function is described in the tu-
                                      torial.

                                  A+W Business capacity planning

                                  Number of shifts Number of shifts in which you work. You specify the shift
                                  hours in the Capacity planning module on the Calendar dialog.
                                   “Calendar” on page H-205

                                  Production scheduling mode Specification whether you want to work with
                                  open or closed capacities.
                                  • Autom. normal capacity:
                                     The orders will be scheduled based on the available shift times. Overbook-
                                     ing is impossible. This is the default setting (closed capacities).
                                  • Automatic full days:
                                     This setting ignores the specifications for the number of shifts and hours in
                                     the calendar. Scheduling is based on a workday of 24 hours in this case
                                     (open capacities). This applies only to common workdays, not to holidays.
                                  • Change machine only:
                                     If capacities are fully utilized, the program will automatically search for an-
                                     other machine. If this is used to capacity as well, scheduling is interrupted
                                     and manual intervention is required.
                                  • Schedule without check:
                                     This setting represents an open shift. This means e.g. that despite a shift
                                     time of 8 h, 16 h can be scheduled as well. The program will issue no report
                                     if a day's capacity is fully utilized. This option should only be used in excep-
                                     tional cases.

                                  Fill shift in case of item splitting Large items can be split to several ma-
                                  chines, shifts, or days. For this, you specify up to what percent the shift of a
                                  machine may be filled by splitting to keep capacity for other orders.
4.02 / 01-2017




                 H-180                                                     A+W Business Pro Capacity Planning
                 Software Reference                                                                        Administration




                                        Machine alignment If you work with several machines that can perform the
                                        same work types, the planning can consider these machines in different ways:
                                        • Automatic:
                                          The program automatically searches for the most cost- and time-effective
                                          machine and schedules the orders on this machine. This is the default set-
                                          ting.
                                        • Semi-automatic:
                                          The program offers the alternative machines for selection. If the delivery
                                          date cannot be adhered to, you must intervene.
                                        • Manual:
                                          With this option, every possible change (machine, shift, etc.) requires man-
                                          ual intervention. Alternative machines can only be selected for manual
                                          scheduling or rescheduling.

                                        Scheduling priority Priorities defined in the order can be taken into account
                                        for scheduling:
                                        • Standard:
                                            The capacities of the required machines are checked and the orders are
                                            scheduled based on the defined priority.
                                        • Low priority:
                                            All orders are scheduled with low priority by default.
                                        • Adopt changed priority for the order:
                                            If the priority is changed at scheduling, it will be automatically saved in the
                                            order.

                                        Product classes without status change
                                        You can suppress the increasing of the item status (order status) with comple-
                                        tion reports for product classes. Just select the appropriate entries on the list.

                                        Order areas without scheduling
                                        You can define that certain order areas shall be excluded from automatic
                                        scheduling. This means that orders for the selected order areas can be sched-
                                        uled manually only.

                                        Autom. delivery date search by route In case of bottlenecks, it is possible
                                        to search for a new delivery date automatically.
                                         The next possible date is selected as delivery date regardless of whether
                                        it is a route day or not. This is the default setting.
                                         The new delivery date is searched for according to the customer's route
                                        days.

                                        Do not split order Large orders must be split into smaller items if the work
                                        process cannot be performed completely in one day for an order.
                                         The orders can be split in automatic scheduling. This is the default setting.
                                         The orders can only be split manually. For the automatic scheduling of large
                                        orders, a message is displayed so that you can intervene.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-181
                 Administration                                                                Software Reference




                                  Reduced scheduling check if structure identical An order may contain
                                  items with the same BOM structure, which differ only for the dimensions.
                                   The entire BOM structure is checked for each item.
                                   With the same BOM structure, the scheduling assumes the previous item
                                  without checking the BOM. This is the default setting.

                                  Schedule for delivery date For automatic scheduling, orders are sched-
                                  uled for the delivery date by default. Another delivery date is searched for only,
                                  if no capacities are free.
                                   Orders are scheduled with delivery date search. This is the default setting.
                                   The orders are scheduled without a search for an alternative delivery date,
                                  regardless whether or not there are free capacities.

                                  Autom. completion report for invoiced orders Currently not used.

                                  Transfer to production (OrderXML) incl. planning data For the transfer
                                  to production, the data determined from capacity planning can be written into
                                  an OrderXML file.
                                   The data determined from capacity planning is not written into an OrderXML
                                  file.
                                   The machine allocation, production date and shift, time costs are written to
                                  the transfer file.

                                  Use change of shifts table If you work with more than one shift, you can
                                  specify when the scheduling changes from one shift to the next.
                                   The change of shifts table is not used.
                                   The change of shifts table is used. If no shift changes are specified, the Shift
                                  settings dialog opens.
                                   “Shift Settings” on page H-183
4.02 / 01-2017




                 H-182                                                     A+W Business Pro Capacity Planning
                 Software Reference                                                                    Administration




                                        Shift Settings
                                        Master data > Company > Company data > Capacity planning tab > Use
                                        change of shifts table checkbox




                                        Fig. H-128    Master data – Shift settings


                                        On this dialog, you specify the shift changes and the lock times in which no
                                        order can be scheduled.

                                           Requirements
                                           You must have administrator rights to open the dialog. In addition, the Use
                                           change of shift table checkbox must be ticked on Company data dialog.

                                            “Use change of shifts table” on page H-182

                                        General
                                        The settings in this group are taken over from the company data.
                                         “A+W Business capacity planning” on page H-180

                                        Number of shifts The number of shifts is loaded from company data.

                                        Alignment mode Search mode for the machines:
                                        • 0 = Automatic:
                                           The program automatically searches for the most cost- and time-effective
                                           machine and schedules the orders on this machine. This is the default set-
                                           ting.
                                        • 1 = Semi-automatic:
                                           The program offers the alternative machines for selection. If the delivery
                                           date cannot be adhered to, you must intervene.
                                        • 3 = Manual:
                                           With this option you must intervene manually for each possible change
4.02 / 01-2017




                                           (machine, shift, etc.). Alternative machines can be selected only in manual
                                           scheduling or rescheduling.




                 A+W Business Pro Capacity Planning                                                            H-183
                 Administration                                                                    Software Reference




                                  Options

                                  Correct time tables when saving If you have changed the values, the
                                  times for the scheduled orders can be revised.
                                   The new times do not change the currently-scheduled orders.
                                   The new times are taken over immediately. All scheduled orders are recal-
                                  culated.

                                  Shift changes

                                  Shift 1 > Shift 2, … Specification when the transition from one shift to the
                                  next shift takes place. This setting is important for the calculation of transition
                                  times. The number of fields displayed depends on the number of shifts that are
                                  specified in the company data.
                                   “A+W Business capacity planning” on page H-180

                                  Locked shift times

                                  1st, 2nd, … shift Specification from which time on the respective shift is
                                  locked for new orders.

                                     Example: 2nd shift 10:00

                                     Up to 17:00, orders can be scheduled in the second shift of the current day.
                                     Thus you keep the 2nd shift free so that all scheduled orders can actually
                                     be produced and there are no residual quantities.
                                     Orders that are scheduled after 17:00 will be planned for the 3rd shift or the
                                     following day.
4.02 / 01-2017




                 H-184                                                        A+W Business Pro Capacity Planning
                 Software Reference                                                                         Administration




                                          General
                                          Capacity planning > Master data > General
                                          On these dialogs, you store the data for work processes and machines that are
                                          available in production.
                                          This section provides information on the following master data:
                                          •   “Machine Types” on page H-185
                                          •   “Work Types” on page H-187
                                          •   “Allocated Machines” on page H-190
                                          •   “Serial Factors” on page H-191
                                          •   “Transition Times” on page H-192


                                          Machine Types
                                          Capacity planning > Master data > General > Machine Types




                 Fig. H-129   Machine types


                                          On this dialog, you define the machine types you are using on the shop floor,
                                          e.g. cutting tables, drills, edgers, toughening furnaces, etc. First, you have to
                                          define the machine types and the restrictions to be checked.
                                          By activating the checkboxes, the appropriate fields on the Machines dialog
                                          are released.
                                           “Machines” on page H-196

                                              Attention in case of subsequent activation
4.02 / 01-2017




                                              If you tick a checkbox later, you must check all machines that belong to the
                                              changed machine type. The newly-released fields are blank by default.
                                              This can cause errors during checking.


                 A+W Business Pro Capacity Planning                                                                 H-185
                 Administration                                                              Software Reference




                                  With a click of the row header, you open the Allocated machines dialog.
                                   “Allocated Machines” on page H-190

                                  No. User-defined number which serves as an ID for the individual machine
                                  types.

                                  Name Name of the machine type.

                                     Settings
                                     The function of each checkbox is described below. A complete description
                                     of the function and the individual settings is available on the Machines dia-
                                     log.

                                      “Machines” on page H-196

                                  Machine type The selection of the machine type is only available in A+W
                                  Business Pro. For this program version, the machine types are fixed. The ma-
                                  chine type refers to the concrete machines and the drivers to be used.
                                  The specification defines which machine drivers are available on the Ma-
                                  chines > Additional options dialog. A+W Business Pro can activate the ma-
                                  chines with these drivers.
                                  In contrast to machine types above, these types cannot be configured.

                                  Dim. check The dimension restrictions must be checked for this machine
                                  type.

                                  Spacer The spacer restrictions must be checked.

                                  Total thickness The total thickness of an IG or LG unit must be checked.

                                  Indiv. thickness The thickness of an individual single glass must be
                                  checked.

                                  Weight The weight of the sheet must be checked.

                                  No. of sheets The number of sheets of a product (double, triple IG or LG)
                                  must be checked.

                                  Area The area of the sheet must be checked.

                                  Gas The item must be checked for gas filling.

                                  Edge prot. The edge protection must be checked for insulated glass.

                                  Shape The item must be checked for shapes.

                                  Georgian bars The item must be checked for georgian bars.

                                  Quantity In the item, the quantity or quantity range must be checked.
4.02 / 01-2017




                                  The definition of the quantity is machine-dependent, e.g.:
                                  • Drilling machine = number of drill holes
                                  • Grinding machine = number of edges


                 H-186                                                   A+W Business Pro Capacity Planning
                 Software Reference                                                                          Administration




                                           Aspect The aspect of the sheet must be checked.

                                           Rotatable For each glass it must be checked whether it may be rotated.

                                           Drilling diameter The diameter of drill holes must be checked.

                                           Corner radius The radius of rounded corners must be checked.

                                           Diagonal Diagonal between the rollers, e.g. on the conveyor belt in front of
                                           the TG furnace must be checked.

                                           Mitre angle Min. and max. mitre angle for facets must be checked.


                                           Work Types
                                           Capacity planning > Master data > General > Work Types




                 Fig. H-130   Work types


                                           On this dialog, you store the work types. These are all activities f that require
                                           time, e.g., cutting, manual cutting, seaming edges, polishing edges, sawing
                                           LG, packaging.
                                           Within a process, several work types can be executed in succession, e.g. cut-
                                           ting and toughening as part of toughened glass production. You have to decide
                                           whether you are going to define these steps as individual work types, or if you
                                           are going to define the entire work process. Depending on how your produc-
                                           tion is organized, it may be useful to choose both types.
                                            Tutorial, “Work Types” on page H-25
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-187
                 Administration                                                                   Software Reference




                                     Scan work types
                                     If you are working with barcoding, you must create all work types that can
                                     be recorded with the scanner. Only then you can also evaluate the reports
                                     for the status.

                                  Functions menu
                                  With this menu, you can display an overview of the machines that are allocat-
                                  ed to the selected work type.
                                   “Allocated Machines” on page H-190

                                  No. User-defined number which serves as an ID for the individual work types.
                                  We recommend to enter these numbers in steps of ten to leave space for in-
                                  serting new work types. This permits to keep similar work types together. Work
                                  types should also be numbered in the sequence in which they appear in the
                                  production process.

                                  Name Name of the work type. Even a surcharge which prolongs the cutting
                                  of shapes for instance, can be defined as a work type.

                                  Hierarchy Sequence order number. This field specifies the priority (produc-
                                  tion sequence) of the individual work types within capacity planning.

                                     Example

                                     Edges have to be ground before holes are drilled.
                                     TG pre-bonding after drilling.
                                     From this it follows that the hierarchy number for the grinding of edges must
                                     be smaller, and that for the laminating pre-compound bigger than the
                                     number for drilling.


                                  Numbers should be allocated in steps of at least 10, better in steps of 50 or
                                  100 to leave enough space for defining new work types.

                                  Only main product Some work types make sense only for the main product
                                  but not for the BOM elements.
                                   This work type can be applied to the main product as well as for the BOM
                                  elements.
                                   This work types only applies to the main product; BOM elements cannot be
                                  shipped for example.

                                  AWProd no. Article number from A+W Production. Work types which are or-
                                  dered from a glass producer but are not specified explicitly in the purchase or-
                                  der, will need an article number from A+W Production, e.g. cutting.
                                  In A+W Business Pro, you have to define a product of the product type/class
                                  Processing for this article; the article numbers must be the same.
4.02 / 01-2017




                 H-188                                                       A+W Business Pro Capacity Planning
                 Software Reference                                                                              Administration




                                        % Limit By default, capacity planning will schedule an order so that it is pro-
                                        duced shortly before the shipping date. This can cause problems in case of
                                        large orders. This percentage defines the maximum share of the order in the
                                        daily production. Large orders will be split onto several days.

                                           Example

                                           You receive a large order on July 17
                                           The delivery date is September 22.

                                           Capacity planning would schedule this order to be produced shortly before
                                           the delivery date. Production would be blocked by this order however for
                                           four whole days for example. No other order could be scheduled during that
                                           time.

                                           Since you have time to produce the order distributed across the entire
                                           period up to the delivery date, you can define that this work type must not
                                           use up more than e.g. 10% of the daily capacity per order item.


                                        This entry will be taken into account if you activate the Pos.Control option. You
                                        will find this option on the following dialogs:
                                         “Schedule Number Manager” on page H-269
                                         “Book Order” on page H-275
                                         “Machine Failure” on page H-287

                                        Manual machine selection If you have several machines that can perform
                                        the same work type, you specify a machine with priority 9 in the default times
                                        so that it is selected by default. If this machine is used to capacity on a certain
                                        date, the program can access one of the other machines.
                                         The order is automatically allocated to another machine. If, however, the
                                        production day is changed, you must intervene manually.
                                         If the capacity of a machine is exceeded, you must select another machine
                                        manually. The possible alternatives are displayed on a dialog.

                                        Alternative work type You can allocate an alternative work type to any work
                                        type, e.g. for the drilling of special sizes.

                                           Example

                                           You have two work types Drilling and Drill special sizes.
                                           For the work type Drilling, the alternative work type Drilling special sizes is
                                           specified.
                                           The standard drilling machine is assigned to the work type Drilling.
                                           However, it can only drill limited drill diameters. If these dimensions are
                                           exceeded, then capacity planning checks whether an alternative work type
                                           is entered.
                                           If so, the program searches for the allocated machine.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                          H-189
                 Administration                                                             Software Reference




                                  Allocated Machines
                                  Capacity planning > Master data > General > Work Types > Functions menu
                                  > Allocated machines




                                  Fig. H-131   Allocated machines


                                  On this dialog, the machines are listed that are allocated to a machine type or
                                  a work type. The info section shows the dialog from which this list has been
                                  accessed.

                                  Machine Name of the allocated machine.

                                  Comment This column shows whether the work type is analyzed as basic
                                  time or as a time surcharge for the allocated machine.

                                  Prio Priority for selecting this machine for scheduling.
                                  • 9: highest priority (standard machine). These machines are always select-
                                     ed first.
                                  • 8 to 1: decreasing priority. These machines are selected depending on uti-
                                     lization.
                                  • 0: lowest priorities. These machines are only selected if all other (equiva-
                                     lent) machines are used to capacity.
                                  • -1: for manual scheduling. These machines are selected by automatic
                                     scheduling only in case of bottlenecks.
                                  • -2: only for manual scheduling. These machines are never selected by au-
                                     tomatic scheduling. The machine can only be selected manually.
                                  • -3: is only selected with reporting from the production system when orders
                                     have been rescheduled there. In case of rescheduling in capacity planning,
                                     only machines with prio >-3 are displayed.
4.02 / 01-2017




                 H-190                                                   A+W Business Pro Capacity Planning
                 Software Reference                                                                      Administration




                                        Serial Factors
                                        Capacity planning > Master data > General > Series Factors




                                        Fig. H-132    Serial factors


                                        On this dialog, you specify the quantities for which the scheduled times shall
                                        be reduced, e.g. because no set-up time is required for grinding or drilling.
                                        You assign the number of the series table to the machine on the Machines di-
                                        alog.
                                         “Serial tables” on page H-201

                                        Identification

                                        Number The number is assigned automatically when you create a new se-
                                        ries table.

                                        Name Name of the series table. Specify a meaningful name if you create sev-
                                        eral tables, e.g. for drilling and grinding.

                                        Serial tables

                                        From … qty. Minimum quantity for applying this factor.

                                        Factor Factor by which the basic time for the work process shall be multi-
                                        plied.

                                           Example

                                           From … qty.                       Factor           Time on the machine
                                                          1                       1                          0.10 hr.
                                                         10                     0.9         10 x 0.9 x 0.1 = 0.90 hr.
4.02 / 01-2017




                                                         50                     0.7         50 x 0.7 x 0,1 = 3.50 hr.




                 A+W Business Pro Capacity Planning                                                               H-191
                 Administration                                                                 Software Reference




                                  Table
                                  This list shows all serial tables you have defined.


                                  Transition Times
                                  Capacity planning > Master data > General > Transition Times




                                  Fig. H-133    Transition times


                                  On this dialog, you specify the time in shifts that is required to change from one
                                  work type to another. For example, after the TG furnace, the sheets must cool
                                  off before the next work type can start.
                                   Tutorial, “Transition Matrix and Transition Times” on page H-64

                                      Editing transition times
                                      The combo boxes in the table fields are released only if you specify a new
                                      transition time. The work types allocated to the transition times cannot be
                                      changed once they were saved. If you want to change an assignment, you
                                      must recreate it and then delete the invalid assignment.

                                  Order priority Order priority that is considered for the transition time. You
                                  can select one of these priorities:
                                  •   Normal:
                                      The transition time applies to all orders which have no special priority. This
                                      is the default setting.
                                  •   Urgent:
                                      The defined transition time applies to rush orders only. If transition times
4.02 / 01-2017




                                      can be shortened for rush orders, a different transition time must be defined
                                      for this combination of work types.




                 H-192                                                      A+W Business Pro Capacity Planning
                 Software Reference                                                                             Administration




                                        •   Extra:
                                            This priority means that the order shall be produced from residue (plates)
                                            left over from cutting other orders.
                                        •   Release order:
                                            The transition time applies only to orders that are produced on-call.

                                            Considering order priority
                                            If in addition to the order priority Normal the priority Urgent shall be consid-
                                            ered, then an individual transition time must be set up for the respective
                                            combination of work types. This applies to all transition times that can be
                                            shortened for urgent orders. If these have not been defined, the order will
                                            be scheduled with Normal priority.

                                        From work type Initial work type, e.g. polishing.

                                        To work type Next work type, e.g. drilling. If you select <n.e.>, the transition
                                        time applies to all subsequent work types.

                                        Time in shifts In this field you enter the number of shifts that are required for
                                        the change from one work type to the next:
                                        • 0 = the next process can take place in the same shift.
                                        • 1 = the next process takes place at the earliest in the next shift.
                                        • 2 = the next process takes place at the earliest in the shift after the next
                                           one.

                                            Example

                                            In your company, you regularly work in 3 shifts, in the heat-soak test, e.g.
                                            however only in one shift of 12 hours.
                                            If you want to achieve that the next work type always begins on the next
                                            day, then you must enter the value 3 in this field. Thus capacity planning
                                            calculates the date for the next work type automatically for the next day.


                                        Incl. days off For the calculation, the days off are considered.
                                         Days off are not considered.
                                         Days off are considered. This means that a TG that comes out of the fur-
                                        nace on Friday can be processed further normally on Monday because the
                                        weekend is longer than the transition time.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                        H-193
                 Organisation                                                             Software Reference




                                Organisation
                                Capacity planning > Master data > Organisation
                                On these dialogs you specify how capacity planning is organized, e.g. the pro-
                                duction areas, machines, shift times.
                                This section provides information on the following subjects:
                                •   “Production Area” on page H-195
                                •   “Machines” on page H-196
                                •   “Calendar” on page H-205
                                •   “Transition Matrix” on page H-210
                                •   “Special Technical Restrictions” on page H-212
                                •   “Org. Overview” on page H-215
4.02 / 01-2017




                 H-194                                                 A+W Business Pro Capacity Planning
                 Software Reference                                                                                Organisation




                                           Production Area
                                           Capacity planning > Master data > Organisation > Production area




                 Fig. H-134   Production areas


                                           On this dialog you define the production areas, e.g. cutting, grinding, drilling.
                                           At the same time you define which statuses shall be reported by the individual
                                           production areas when the item is reported completed.
                                            Tutorial, “Production Areas (Work Centers)” on page H-27

                                           No. Freely-definable number that serves as ID for the individual production
                                           areas. The numbering does not represent a hierarchy.

                                                 Production area <n.e.>
                                                 The production area No. 0 (zero) with the description <n.e.> must be de-
                                                 fined once as default production area. After this entry was saved, it is no
                                                 longer displayed on this dialog. Enter this production area to see if it exists.
                                                 An error report will indicate that it has already been entered.

                                           Production area Name of the production area.

                                           Max. unit/h Specification of how many units (pieces) can be processed in
                                           the production area per hour.
                                           If, for example, you have 6 grinding machines but only 3 workers who can work
                                           on these machines, you can only calculate the total capacity for three ma-
                                           chines.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                       H-195
                 Organisation                                                              Software Reference




                                Min. dwell days Number of days that an element of an item dwells in the
                                production area:
                                • 0 = no dwell time
                                • 0.1 = one shift
                                • 1 = one day, e.g. entry into the production area today, exit tomorrow.
                                Additional times are defined as transition times.
                                 “Transition Times” on page H-192
                                 “Transition Matrix” on page H-210

                                Client Client to whom the production area is assigned. The clients are stored
                                in the company data.
                                 Master Data, “Company Data – Client” on page B-900

                                Status report The status in capacity planning and in the order can be imple-
                                mented automatically by the report from barcoding of A+W Production. With
                                the setting you specify from which registration point the report is sent.
                                The status of the items and of the order can be checked on the Status reports
                                dialog.
                                 Sales, “Status Message” on page C-498



                                Machines
                                Capacity planning > Master data > Organisation > Machines
                                All machines used are created with technical restrictions and operating costs
                                required for planning and cost calculation.
                                This dialog contains the following tabs:
                                •   “Machines – General” on page H-197
                                •   “Machines – Restrictions” on page H-202
                                The fields for the definition of restrictions are released on the Machine types
                                dialog.
                                 “Machine Types” on page H-185

                                    Attention in case of subsequent activation of checks
                                    If you tick a checkbox for a machine type later, you must check all machines
                                    that belong to the changed machine type. The newly-released fields are
                                    blank by default. This can cause errors during checking.
4.02 / 01-2017




                 H-196                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                       Organisation




                                          Machines – General
                                          Capacity planning > Master data > Organisation > Machines > General tab




                 Fig. H-135   Machines – General


                                          On this tab, you specify the machines that you use and that are relevant for
                                          capacity planning. You should also create a machine Shipping so that the
                                          times for that can be planned.
                                           Tutorial, “Machine Types and Machines” on page H-21

                                          Machine

                                          No./description Number (ID) and description can be selected freely. We rec-
                                          ommend grouping similar machines in number ranges, e.g. 100-199 for cutting
                                          tables, 400-499 for drills, etc.

                                          Type Machine type to which the machine belongs. With the assignment, the
                                          fields for the restriction checks are released.
                                           “Machine Types” on page H-185

                                          Production area Production area in which the machine is installed.
4.02 / 01-2017




                                           “Production Area” on page H-195




                 A+W Business Pro Capacity Planning                                                             H-197
                 Organisation                                                              Software Reference




                                Options

                                Sheets rotatable Defines whether the sheets can be rotated on the ma-
                                chine.
                                 The sheets cannot be rotated.
                                 The sheets can be rotated.

                                Edge protection permitted Defines whether this machine can apply edge
                                protection.
                                 Edge protection cannot be put on.
                                 Edge protection can be put on.

                                Auto break Specification whether the cutting table has an automatic break-
                                ing device.
                                 The table has no automatic breaking device.
                                 The sheets can be broken automatically.

                                Shapes possible Specification whether shapes (non-rectangular sheets)
                                can be produced on the machine.
                                 Shapes are not possible.
                                 Shapes are possible.

                                Georg. bar permitted Defines whether this machine can produce Georgian
                                bars.
                                 Georgian bars are not possible.
                                 Georgian bars are possible.

                                LG Specification whether LG can also be cut on the cutting table.
                                 The table cannot cut any LG sheets.
                                 The table can cut LG sheets.

                                Gas filling possible Defines whether this machine can handle gas fillings.
                                 Gas fillings are not possible.
                                 Gas fillings are possible.

                                Autosupport Specification whether the cutting table has an automatic sup-
                                port.
                                 The table has no automatic support.
                                 The table has an automatic support. In this case, for each
                                stock plate that is cut on this table, a support code must be assigned.

                                Decoating Specification whether the edges of sheets can be decorated on
                                the machine.
                                 Edge decoatings are not possible.
                                 Edge decoatings are possible.
4.02 / 01-2017




                                Mitre-cut table
                                Selection of the number of mitre-cut tables. This setting is not displayed for
                                A+W Business Pro.


                 H-198                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                          Organisation




                                        Additional options
                                        These settings apply only for A+W Business Pro.

                                        Output directory Selection of the storage location for output file.

                                        Machine code Selection of the machine code. The machine codes are stored
                                        on a dialog by the same name. If the code you are searching for is missing,
                                        you can create it in this dialog.

                                        IG driver, IG section The fields are filled if the machine code for an IG line is
                                        selected.

                                        Keyword

                                        Z-cut Specification of the location of Z-cuts in cutting mode.
                                        • (<n.e.>):
                                           Not applicable.
                                        • up:
                                           Normally it is better to place the Z-cuts up, that is, to place them away from
                                           the working width so that individual cuts can first be broken across the
                                           whole width and then rotated. If overlying sheets have Z-cuts, then there is
                                           already space on the breaking table to break the sheets for the Z-cut.
                                        • bottom:
                                           The starting point is at the top
                                        • anywhere:
                                           The starting point can be selected at will.

                                        Cutting mode Specification of the sequence in which the cuts will be made:
                                        •   1 - XYZW:
                                            The first cut runs parallel to the lower edge of the plate. After that come the
                                            Y-cut and the Z-cut. The further sequence is optional.
                                        •   2 - XYZ*:
                                            Like 1. After the Z-cut comes any other cut.
                                        •   3 - XYZW:
                                            The first cut runs perpendicular to the lower edge of the plate. After that
                                            come the Y-cut and then the Z-cuts
                                        •   4 - XYZZ:
                                            Like 3. However only two Z-cuts are possible.
4.02 / 01-2017




                                            Fig. H-136   XYZ cuts on the stock plate




                 A+W Business Pro Capacity Planning                                                                 H-199
                 Organisation                                                                   Software Reference




                                Cost factor Z-cut Specification for the price increase of Z-cuts. Factor 1
                                means that the price for the cut is not increased. Factor 1.5 increases the price
                                by half.

                                Reference point Selection of the reference point for the cutting mode. The
                                reference point of the table refers to the point with the coordinates 0/0 on which
                                the cutting mode is built. It is important to cut shapes correctly.

                                    Reference point vs. home position of the cutting head
                                    The reference point must not match the home position of the cutting head.
                                    At Bystronic, for example, there are mirrored tables whose reference point
                                    is at the left front, while the cutting head's home position is in the right front.
                                    For some tables, this can be set as a parameter.

                                Break start Selection of the break start. The break start is oriented according
                                to the spatial relations in the operation and determines the storage of the re-
                                sidual plate as well as to a certain extent the cutting sequence (first sheet to
                                be broken top or bottom).

                                Values

                                Units per hour The value in this field depends on the work unit capacity
                                planning shall use to calculate the capacity of this machine: man hours or ma-
                                chine hours. By default, a 1 is entered.
                                 Tutorial, “Work Units” on page H-39

                                Labour costs per unit The entry in this field depends on the work unit capac-
                                ity planning shall use to calculate the capacity of this machine, e.g. man hours
                                or machine hours.
                                You will find detailed information under:
                                 Tutorial, “Work unit = man hour” on page H-39

                                Machinery costs Machine costs per hour, e.g. for maintenance, repair, con-
                                sumables.

                                Variable costs per hour Miscellaneous costs which belong neither to labour
                                costs nor to machinery costs, can be included in the production costs, e.g. in-
                                surance. The total insurance fee has to be converted in to costs per hour.

                                Costs per unit Total costs per unit for this machine. They are the basis for
                                cost calculation. These costs are calculated from labour costs, machinery
                                costs, variable costs, and the work unit per hour.

                                .
                                    Example

                                    Labor costs/hr
                                    + machine costs/hour divided by units/hour
                                    + variable costs/hour divided by units/hour
4.02 / 01-2017




                                    = costs/unit




                 H-200                                                      A+W Business Pro Capacity Planning
                 Software Reference                                                                              Organisation




                                        Registration point Number of the registration point (machine) in
                                        A+W Production this machine refers to. The numbers must be identical in
                                        A+W Business Pro and A+W Production. If you are using barcoding (scan-
                                        ners), you have to scan the registration point number.

                                        Output per hour Average targets (based on experience or based on infor-
                                        mation from the machine manufacturer) in quantity units.
                                        You can use this entry if you have e.g. defined all master data except the de-
                                        fault times and want to schedule those in advance to estimate the capacity of
                                        your production. This allows to bridge the time until all standard times have
                                        been entered.

                                        Serial tables Selection of the serial table in which the special times for series
                                        are defined.
                                         “Serial Factors” on page H-191

                                        Lock

                                        Locked The machine can be locked for scheduling.
                                         The machine is not locked.
                                          The machine is locked and cannot be included in scheduling. This set-
                                        ting is used for example if a new machine shall be tested first before it is actu-
                                        ally used.
                                        To lock a machine for maintenance purposes please go to the Machine down-
                                        time dialog:
                                         “Machine Failure” on page H-287

                                        Locking formula With a locking formula, you can store additional restric-
                                        tions that cannot be reached with standard means.

                                           Example

                                           On a machine, only shapes, very small, and very large sheets shall be
                                           produced because this machine is very slow.
                                           All rectangular sheets with a width >200 and <2600 mm as well as a height
                                           >300 and <1600 mm shall not be cut on this machine.
                                           This restriction can only be specified with a formula. If you want to use
                                           formulas, contact your service employee at A+W Software GmbH.


                                        Add. work type for coupled machines Currently not used.

                                        Table
                                        In the overview, the machines that are available for capacity planning are listed
                                        depending on the selection criteria.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                    H-201
                 Organisation                                                                           Software Reference




                                            Machines – Restrictions
                                            Capacity planning > Master data > Organisation > Machines > Restrictions tab




                 Fig. H-137   Machines – Technical restrictions


                                            On this tab, you store minimum and maximum values for the restriction
                                            checks. Enter 0 to 9999 if all values are permitted.
                                            The fields for the definition of restrictions are released on the Machine types
                                            dialog.
                                             “Machine Types” on page H-185
                                            If the technical restrictions are different for a machine with the same work
                                            types, define these restrictions on the Special technical restrictions dialog. Ca-
                                            pacity planning checks the entry in Special technical restrictions dialog first.
                                             “Special Technical Restrictions” on page H-212
                                            The fields in the Machine group are described for the General tab.
                                             “Machines – General” on page H-197

                                            Work types / time surcharges
4.02 / 01-2017




                                            In this group, all work types are listed for which default times on this machine
                                            are defined.
                                             “Default Times (dialog)” on page H-217



                 H-202                                                                 A+W Business Pro Capacity Planning
                 Software Reference                                                                              Organisation




                                        Technical restrictions
                                        The fields for the definition of restrictions are released on the Machine types
                                        dialog.
                                         “Machine Types” on page H-185
                                        Enter 0 or 9999 if all values are permitted.

                                        Width, height Min. and max. sheet dimensions for this machine.

                                        Spacer Min. and max. spacer for this machine

                                        Total thickness Min. and max. total thickness for IG and LG.

                                        Glass thickness Min. and max. thickness of single glass.

                                        Surface in sqm Min. and max. surface for this machine.

                                        Mitre angle Min. and max. mitre angle for facets.

                                        Quantity Min. and max. quantity for the order item. In the item, the quantity
                                        or quantity range must be checked. The definition of the quantity is machine-
                                        dependent, e.g.
                                        • Drilling machine = number of drill holes
                                        • Grinding machine = number of edges

                                        Drilling diameter Min. and max. dimensions for this machine.

                                        Radius round. corner Min. and max. dimensions for this machine.

                                        Diagonal Diagonal between the rollers, e.g. on the conveyor belt in front of
                                        the TG furnace.

                                        Max. number of sheets Maximum quantity of sheets for a TG or IG unit, e.g.
                                        3 on an IG line.

                                        Max. ratio Maximum ratio for this machine.

                                           Example

                                           You enter the value 5. This corresponds to a max. ratio of 1:5. If one side is
                                           500 mm long, for example, then the other side can be max. 2500 mm.


                                        Weight up to kg Maximum weight of a unit.

                                        Distance between cuts
                                        For cutting tables with an automatic breaking device, you must set the maxi-
                                        mum and minimum distances between the cuts. These distances must be ad-
                                        hered to so that the system can still break the sheet.
4.02 / 01-2017




                                        Min. Dist. X-X with Y Minimum distance between X-X cuts if Y-cuts are also
                                        made.


                 A+W Business Pro Capacity Planning                                                                     H-203
                 Organisation                                                            Software Reference




                                Min. Dist. X-X without Y Minimum distance between X-X cuts if no Y-cuts
                                are also made.

                                Max. Dist. X-X cuts Maximum distance between X-X cuts.

                                Min. Dist. Y-Y with Z Minimum distance between X-X cuts if Y-cuts are also
                                made.
                                For cutting tables with several Y-cutting heads, the minimum distance corre-
                                sponds to the distance of the cutting wheels of two immediately adjacent cut-
                                ting heads, e.g. Bystronic XYZVA = 300 mm.

                                Min. Dist. X-X without Z Minimum distance between X-X cuts if no Z-cuts
                                are also made.

                                Max. Dist. Y-Y cuts Maximum distance between Y-Y cuts.

                                Min. residual width Minimum width at the edge of the plate.

                                Min. Dist. X-Z cuts Minimum distance between X and Z-cuts.

                                Min. Dist. Z-Z cuts Minimum distance between Z-cuts.
4.02 / 01-2017




                 H-204                                                A+W Business Pro Capacity Planning
                 Software Reference                                                                                Organisation




                                        Calendar
                                        Capacity planning > Master data > Organisation > Calendar
                                        On this dialog, you specify the work days and shift times. The data can be
                                        saved only if at least one shift has been entered. The number of shifts is de-
                                        fined in company data
                                         “Default Settings in Company Data” on page H-179
                                        If no calendars are defined in capacity planning, the A+W Business Pro stan-
                                        dard calendar will be used.
                                        By default, capacity planning assumes one shift per day. If, however, you want
                                        to work in more than one shift, you have to enter the number of shifts first. After
                                        that you can define calendars for machines with different shifts and shift times.

                                            Example

                                            The calendar permits to enter a maximum of six shifts per day. If the hours
                                            are equally distributed, this is a maximum of four hours per shift. The
                                            distribution of the number of hours per shift varies however, e.g. 5, 3, 5, 3,
                                            5, 3 or 4, 2, 6, 6, 3, 3.
                                            These examples show that you do not have to stick to an even distribution
                                            of hours.

                                            In case of 4 shifts and uniform distribution per shift, a maximum of 6 hours
                                            can be entered.

                                            The total hours x shifts per day must not exceed 24 hours of course.

                                            Changing the calendar
                                            When you have edited a calendar or entered a new one, you have to reboot
                                            A+W Business Pro to make sure that the data are available for scheduling.

                                        This dialog contains the following tabs:
                                        •   “Calendar – Selection” on page H-206
                                        •   “Calendar – Calendar” on page H-208
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                          H-205
                 Organisation                                                               Software Reference




                                Functions Menu
                                Capacity planning > Master data > Organisation > Calendar
                                Using this menu, you can open other dialogs without closing the calendar.
                                The following entries are displayed:
                                •   Copy:
                                    Opens the Copy calendar dialog to transfer a calendar, e.g. into a new year.
                                     “Copy Calendar” on page H-209
                                •   Shift times:
                                    Opens the Shift settings dialog on which you can specify the shift transition
                                    and closing times.
                                     “Shift Settings” on page H-183
                                    You must have administrator rights to open the dialog. In addition, the Use
                                    change of shift table checkbox must be ticked on the Company data dialog.
                                     “Use change of shifts table” on page H-182


                                Calendar – Selection
                                Capacity planning > Master data > Organisation > Calendar > Selection tab




                                Fig. H-138    Calendar – Selection
4.02 / 01-2017




                                On this tab, you specify calendar for work types, machines, production area,
                                and clients.


                 H-206                                                   A+W Business Pro Capacity Planning
                 Software Reference                                                                         Organisation




                                        If no special calendar is defined for a production area or a machine, the com-
                                        mon calendar will be used.
                                         Tutorial, “Adjust Calendar” on page H-45

                                        Identification
                                        The labeling of the two selection fields depends on the mode selected.

                                        Work type, machine Work type and machine to which the calendar applies.

                                        Production area, client Production area and client to whom the calendar
                                        applies.

                                        Year Year to which the calendar is edited or created.

                                        Mode
                                        With the selection of the option, you specify for what you want to create the
                                        calendar. The fields are only released in selection mode.
                                        •   Work type, machine:
                                            With this setting, you specify a calendar for a work type and/or a machine.
                                        •   Production area/client:
                                            With this setting you specify a new calendar for a production area and/or a
                                            client.
                                            In order to create a general calendar, select this option and enter the pro-
                                            duction area <n.e.> and for the clients all.

                                        Calendar tables In the overview, all calendars are displayed that correspond
                                        to the selection criteria. If you have limited the selection only according to the
                                        Work type mode or Production area, all calendars are displayed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-207
                 Organisation                                                                Software Reference




                                Calendar – Calendar
                                Capacity planning > Master data > Organisation > Calendar > Calendar tab




                                Fig. H-139   Calendar – Calendar


                                On this tab, you specify the work time per shift. The number of shifts is speci-
                                fied in the company data.
                                 “Default Settings in Company Data” on page H-179

                                Working week

                                Monday – Sunday If you want to change the shift time of a weekday, you
                                must tick the appropriate checkbox and enter the new number of hours. The
                                change applies only to the date displayed. If necessary, you must transfer the
                                new shift time to the year or the calendar week.

                                Hours per shift Number of available hours per week day and shift.

                                   Set up additional shift
                                   If you want to set up an additional shift for a machine or a production area,
                                   you must re-enter all shift times.
                                   It is not sufficient to specify only the hours for the new shift, because during
4.02 / 01-2017




                                   transfer to the year (or the week), the blank fields are also taken over. This
                                   deletes the old shift times.



                 H-208                                                   A+W Business Pro Capacity Planning
                 Software Reference                                                                      Organisation




                                        Adopting shifts for calendar

                                        [Apply to year] Transfers the changes to all appropriate weekdays of the
                                        year.
                                        Only the shift times of the weekdays are transferred for which the checkbox is
                                        ticked.

                                        [Apply to week] Transfer the change to all days of the calendar week.

                                        Calendar week

                                        Go to Selection of the calendar week.

                                        [Current calendar week] Changes the display in the Working week group to
                                        edit the shift times for the current calendar week.


                                        Copy Calendar
                                        Capacity planning > Master data > Organisation > Calendar > Functions menu
                                        > Copy




                                        Fig. H-140    Copy calendar


                                        On this dialog, you copy the calendar for a machine or a production area, e.g.
                                        by transferring it to another machine.

                                        Calendar source selection
                                        The labeling of the two selection fields depends on the mode selected.

                                        Work type, machine Work type and machine for which the calendar is cre-
                                        ated.

                                        Production area, client Production area and client to whom the calendar ap-
                                        plies.
4.02 / 01-2017




                                        Year Year for which the calendar is created.




                 A+W Business Pro Capacity Planning                                                            H-209
                 Organisation                                                                  Software Reference




                                Calendar destination selection

                                Work type, machine Work type and machine to which the calendar shall be
                                transferred.

                                Production area, client Production area and client to whom the calendar
                                shall be transferred.


                                Transition Matrix
                                Capacity planning > Master data > Organisation > Transition matrix




                                Fig. H-141    Transition matrix


                                On this dialog, you enter how long it takes until the item moves from one pro-
                                duction area to the next one. The times can be designed differently depending
                                on the order priority.

                                    Example

                                    The transition from the Cutting production area to the Processing
                                    production area can normally be done in the same shift.
                                    The transfer from the TG production area to the IG production area takes
                                    several shifts or 1 day.

                                 Tutorial, “Transition Matrix and Transition Times” on page H-64

                                Order priority Selection with which order priority the transition time shall be
                                considered. You can select one of these priorities:
4.02 / 01-2017




                                •   Normal:
                                    The transition time applies to all orders which have no special priority. This
                                    is the default setting.


                 H-210                                                    A+W Business Pro Capacity Planning
                 Software Reference                                                                                 Organisation




                                             •   Urgent:
                                                 The defined transition time applies to rush orders only. If transition times
                                                 can be shortened for rush orders, a different transition time must be defined
                                                 for this combination of work types.
                                             •   Extra:
                                                 This priority means that the order shall be produced from residue (plates)
                                                 left over from cutting other orders.
                                             •   Release order:
                                                 The transition time applies only to orders that are produced on-call.

                                                 Consider order priority
                                                 If in addition to the order priority Normal the priority Urgent shall be consid-
                                                 ered, a special transition time must be defined for the corresponding com-
                                                 bination of production areas. This applies to all times that can be shortened
                                                 for rush orders if required. If these have not been defined, the order will be
                                                 scheduled with Normal priority.

                                             From production area Production area the item comes from.

                                             To production area Next production area to which the item changes.

                                             Transition time Time that a glass requires to change to the next production
                                             area. The values are entered in days:
                                             • 0 = same day or same shift
                                             • 0.01 to 0.99 = next shifts
                                             • 1 = next day

                                             Examples for the calculation of the transition

                 No.        1/no.       Same       Next s.      e.g.   S. after the e.g.   S. two       e.g.   S. three     e.g.
                 shifts     hours       shift                          next one            shifts after        shifts after
                                                                                           the next            the next
                                                                                           one                 one

                 4          1/4=0.25    0          0.1-0.24     0.2    0.26-0.49    0.4    0.51-0.74    0.6    0.76-1       1
                            Transition: S1-Mo      S2-Mo               S3-Mo               S4-Mo               S1-Tu
                            Transition: S2-Mo      S3-Mo               S4-Mo               S1-Tu               S2-Tu

                 3          1/3=0.33    0          0.1-0.3      0.2    0.4-0.6      0.5    0.7-1        1      -            -
                            Transition: S1-Mo      S2-Mo               S3-Mo               S1-Tu               -            -
                            Transition: S2-Mo      S3-Mo               S1-Tu               S2-Tu               -            -

                 2          1/2=0.5     0          0.1-0.49     0.3    0.51-0.1     1      -            -      -            -
                            Transition: S1-Mo      S2-Mo               S1-Tu               -            -      -            -
                            Transition: S2-Mo      S1-Tu               S2-Tu               -            -      -            -

                 Tab. H-4      Transition times in days
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                       H-211
                 Organisation                                                                             Software Reference




                                                Flexible transition time
                                                Instead of a fixed value, you can also enter a formula if the transition time
                                                depends on different parameters, e.g. thickness. With a right-click in the
                                                field, the Formula search dialog opens.
                                                If you want to work with formulas, call your service employee at A+W Soft-
                                                ware GmbH for assistance.


                                             Special Technical Restrictions
                                             Capacity planning > Master data > Organisation > Special technical restric-
                                             tions tab




                 Fig. H-142   Special technical restrictions


                                             On this dialog, you specify restrictions for machines that refer to particular
                                             work types.
                                             If a machine can execute different work types, e.g. Drilling and Corner cut-out,
                                             you can define different check values per work type. If capacity planning finds
                                             no definition for the work type, the general technical restrictions of the machine
                                             will be checked.
                                              “Machines – Restrictions” on page H-202
                                             The available parameters depend on the settings on the Machine types dialog.
                                              “Machine Types” on page H-185
4.02 / 01-2017




                 H-212                                                                A+W Business Pro Capacity Planning
                 Software Reference                                                                      Organisation




                                        Functions menu
                                        Using this menu, you can copy the values from the standard machine. Al-
                                        ready-entered values are overwritten without a query.
                                         “Machines – Restrictions” on page H-202

                                        Identification

                                        Work type Work type to which the restrictions apply.

                                        Machine Machine to which the restrictions apply when the appropriate work
                                        type is performed.

                                        Technical restrictions (minimum/maximum)
                                        Enter 0 or 9999 if all values are permitted.

                                        Width, height Min. and max. dimensions for this machine.

                                        Spacer Min. and max. spacer for this machine.

                                        Total thickness Min. and max. total thickness for IG and LG for this ma-
                                        chine.

                                        Glass thickness Min. and max. thickness of single glass.

                                        Quantity Min. and max. quantity for the order item. In the item, the quantity
                                        or quantity range must be checked. The definition of the quantity is machine-
                                        dependent, e.g.
                                        • Drilling machine = number of drill holes
                                        • Grinding machine = number of edges

                                        Drilling diameter Min. and max. size for this machine.

                                        Radius round. corner Min. and max. size for this machine.

                                        Surface in sqm Min. and max. surface for this machine.

                                        Diagonal Diagonal between the rollers, e.g. on the conveyor belt in front of
                                        the TG furnace.

                                        Mitre angle Min. and max. mitre angle for bevelling.

                                        Other technical restrictions
                                        Enter 9999 if all values are permitted.

                                        Serial table Number of the serial table that shall be used for serial produc-
                                        tion.
4.02 / 01-2017




                                         Software Reference, “Serial Factors” on page H-191

                                        Max. number of sheets Maximal number of sheets permitted for a laminat-
                                        ed glass or IG unit on this machine.


                 A+W Business Pro Capacity Planning                                                            H-213
                 Organisation                                                                 Software Reference




                                Weight up to kg Maximum weight.

                                Max. ratio Maximum ratio for this machine.

                                   Example

                                   The value 5 corresponds to a max. ratio of 1:5.
                                   If one edge of the sheet is 500 mm, for example, then the other edge can
                                   be max. 2500 mm long.


                                Technical restrictions (options)

                                Shapes possible Defines whether this machine can produce shapes.
                                 Shapes are not possible.
                                 Shapes are possible.

                                Georg. bar permitted Defines whether this machine can produce Georgian
                                bars.
                                 Georgian bars are not possible.
                                 Georgian bars are possible.

                                Gas filling possible Defines whether this machine can handle gas fillings.
                                 Gas fillings are not possible.
                                 Gas fillings are possible.

                                Sheets rotatable Defines whether the sheets can be rotated on the ma-
                                chine.
                                 The sheets cannot be rotated.
                                 Sheets can be rotated

                                Edge protection permitted Defines whether this machine can apply edge
                                protection.
                                 Edge protection cannot be put on.
                                 Edge protection can be put on.

                                Overview of special restrictions
                                On the overview, the work types and machines are listed for which special re-
                                strictions are stored.
4.02 / 01-2017




                 H-214                                                   A+W Business Pro Capacity Planning
                 Software Reference                                                                               Organisation




                                              Org. Overview
                                              Capacity planning > Master data > Organisation > Org. overview




                 Fig. H-143   Org. overview


                                              On this dialog, you check which machines and work types are allocated to the
                                              production areas.

                                              Selection

                                              Client Client to whom the production area is assigned.

                                              Production area Production area to which the machines are assigned.

                                              Breakdown level
                                              With the selection of the option, you filter the display in the overview.

                                              View
                                              The columns in the overview depend on the breakdown level.
                                              •   Production area:
                                                  Production area to which the machine is assigned.
                                              •   Machine:
                                                  Machines that are assigned to the production area in question.
                                              •   Work type:
                                                  Work types that are assigned to the machine in question.
4.02 / 01-2017




                                              •   Surcharges:
                                                  Type of default time that is consulted for the work type in question for cal-
                                                  culation.



                 A+W Business Pro Capacity Planning                                                                       H-215
                 Default Times                                                              Software Reference




                                 Default Times
                                 Capacity planning > Master data > Default Times
                                 In this program group, you will find the dialogs on which the defaults for the
                                 time calculation are stored.
                                 This section provides information on the following subjects:
                                 •   “Default Times (dialog)” on page H-217
                                 •   “Change Default Times” on page H-225
                                 •   “Copy Default Times” on page H-225
                                 •   “Special Times” on page H-226
                                 •   “Special Priorities” on page H-227
4.02 / 01-2017




                 H-216                                                   A+W Business Pro Capacity Planning
                 Software Reference                                                                     Default Times




                                        Default Times (dialog)
                                        Capacity planning > Master data > Default Times > Default Times
                                        On this dialog, you enter the time values determined for your machines per
                                        work type and machine. It depends on the machine whether the calculation of
                                        times is based on linear metres, square metres, pieces, etc.
                                        On this dialog, you will find the following tabs:
                                        •   “Default Times – Time Selection” on page H-218
                                        •   “Default Times – Matrix” on page H-221
                                        •   “Default Times – Vector” on page H-222
                                        •   “Default Times – Individual Time” on page H-223
                                        •   “Default Times – Cube” on page H-224

                                        Entry of time values in hours
                                        Times are not entered in minutes but in hours. This means that the measured
                                        minutes must be converted into hours:

                                            Minutes       Time entry in hr.

                                            60            1
                                            30            0.5
                                            15            0.25
                                            7.5           0.125
                                            3.75          0.0625
                                            1.875         0.03125


                                        Functions menu
                                        Capacity planning > Master data > Default Times > Default Times
                                        Using this menu, you can open other dialogs without closing the default times.
                                        The following entries are displayed:
                                        •   Change:
                                            Opens the dialog by the same name to increase or reduce the default times
                                            by a factor.
                                             “Change Default Times” on page H-225
                                        •   Copy:
                                            Opens the dialog by the same name to copy the default times from the
                                            standard machine.
                                             “Copy Default Times” on page H-225
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-217
                 Default Times                                                                          Software Reference




                                            Default Times – Time Selection
                                            Capacity planning > Master data > Default Times > Default Times > Choose
                                            time tab




                 Fig. H-144   Default Times – Table selection


                                            On this tab, you specify the type of calculation and the priority.
                                             Tutorial, “Default Times” on page H-55

                                            Identification

                                            Work type Work type to which the default time applies.

                                            Machine Machine on which the work time requires the default time.
4.02 / 01-2017




                 H-218                                                                 A+W Business Pro Capacity Planning
                 Software Reference                                                                         Default Times




                                        Type Type of the default time:
                                        • 0 - Basic time:
                                           Stopped time for a work process.
                                             “Entry of time values in hours” on page H-217
                                        •   1 - Time surcharge:
                                            A time surcharge is required for work types that require more effort, e.g. for
                                            cutting shapes.
                                        •   2 - Alternative procedure:
                                            This default time is only considered if an alternative work type exists for the
                                            work type. In this case, in the Alternative A+W Prod. no. field you must en-
                                            ter the alternative machine number.
                                        •   3 - Alternative without BOM:
                                            Laminated glass producers usually enter all LG articles with bills of materi-
                                            als. When a LG sheet is not going to be produced but directly cut from a LG
                                            stockplate, the bill of material must be ignored. For the work type LG cut-
                                            ting, the Alternative w/o BOM would be selected. In this case, enter the al-
                                            ternative machine number in field altern. A+W Prod. no.
                                        •   4 - Ignore process:
                                            A corner cut-out for example requires three processes: 1. Drilling (of corner
                                            hole), 2. Cutting, and 3. Grinding.
                                            The CNC machine can do everything on one, so that just the drilling will be
                                            taken into account. The other two work types will be ignored. You only have
                                            to assign the default time for the work type Drilling which covers the whole
                                            process. The other two work types are allocated the entry Ignore process
                                            for this machine.

                                        Priority If several machines are available for one work type, you must spec-
                                        ify which machine is queried first during the search for free capacities and
                                        which, for example, can only be selected manually.
                                        If two machines have the same priority, then capacity planning checks the
                                        costs that are defined per machine. In this case, the cheaper machine is se-
                                        lected automatically.
                                        If no costs per machine are stored, the program can find the cheapest ma-
                                        chine. In this case, the priority must be clear for the same machines.
                                        • 9: highest priority (standard machine). These machines are always select-
                                            ed first.
                                        • 8 to 1: decreasing priority. These machines are selected depending on uti-
                                            lization.
                                        • 0: lowest priorities. These machines are only selected if all other (equiva-
                                            lent) machines are used to capacity.
                                        • -1: for manual scheduling. These machines are selected by automatic
                                            scheduling only in case of bottlenecks.
                                        • -2: only for manual scheduling. These machines are never selected by au-
                                            tomatic scheduling. The machine can only be selected manually.
                                        • -3: is only selected with reporting from the production system when orders
                                            have been rescheduled there. In case of rescheduling in capacity planning,
                                            only machines with prio >-3 are displayed.
4.02 / 01-2017




                                        Alternative A+W Prod. no. In this field, you must enter the machine number
                                        from A+W Production if in the Type field the value Alternative process or Alter-
                                        native without BOM is selected.

                 A+W Business Pro Capacity Planning                                                                H-219
                 Default Times                                                             Software Reference




                                 Grouped by
                                 With the selection of the option, you specify how the display in the overview
                                 shall be grouped. The fields are only released in selection mode.
                                 •   Work type:
                                     For each work type, the assigned machines are displayed.
                                 •   Machine:
                                     The work types with defined times are displayed per machine.

                                 Other surcharges

                                 Table Reference to surcharge table, e.g. for oversizes. These surcharge ta-
                                 bles are created on the Special times dialog.
                                  “Special Times” on page H-226

                                 Overview
                                 All default times with the assigned work types are listed in the overview. With
                                 a double-click on allocations, the allocated products, product types, product
                                 classes, and/or product groups are displayed.
                                 You select the grouping in the selection mode.
4.02 / 01-2017




                 H-220                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                          Default Times




                                           Default Times – Matrix
                                           Capacity planning > Master data > Default Times > Default Times > Matrix tab




                 Fig. H-145   Default Times – Matrix


                                           On this tab, you specify the default times, which are graduated according to
                                           two limit types.
                                            Tutorial, “Default Times” on page H-55

                                           Limit type 1, limit type 2 Default times can be graduated by means of limit
                                           types. The limit type defines the measure for the graduation. You can select
                                           thickness and area, for example.
                                           The input field for the limit value is released if you insert a new column/row.
                                           The limit value refers to the limit type.
                                            Master Data, “Quantity Limits” on page B-872

                                           Specification

                                           Time unit The unit refers to the limit type. The limit value can refer to pieces,
                                           square meters, linear meters, etc.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-221
                 Default Times                                                                            Software Reference




                                           Triangle You can record times in a matrix or in a cube so that the specified
                                           limit values can be switched, e.g. height and width.
                                            The limit types must not be switched. In this case, you must enter a time
                                           per column/row in all fields. Select this setting for glass for which it is important
                                           in which direction it is cut.
                                            The limit types may be switched. Thus you only have to record the time in
                                           one of the combinations of limit types.

                                           Min. values
                                           The min. values are checked at scheduling. If values are under-run, a mes-
                                           sage is displayed and/or a surcharge is charged.

                                           Minimum time You can specify how much minimum time is calculated for an
                                           item.

                                           Overview
                                           In the overview, you specify in each field per row and column the time that is
                                           required for this combination of limit types for the work type.


                                           Default Times – Vector
                                           Capacity planning > Master data > Default Times > Default Times > Vector tab
4.02 / 01-2017




                 Fig. H-146   Default Times – Vector



                 H-222                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                           Default Times




                                            On this tab, you specify default times, which are graduated according to one
                                            limit type, e.g. by thickness.
                                            The fields are described on the Matrix tab.
                                             “Default Times – Matrix” on page H-221


                                            Default Times – Individual Time
                                            Capacity planning > Master data > Default Times > Default Times > Indiv. time
                                            tab




                 Fig. H-147   Default Times – Individual time


                                            On this tab, you store individual times. Generally you store individual times for
                                            the work processes. There is a row displayed for each combination of machine
                                            and work type. Entries in red indicate that no times are defined.

                                            Overview
                                            •   Machine:
                                                Machine that is selected on the Choose time tab.
                                            •   Work type:
                                                Work type for which a time is specified on the selected machine.
4.02 / 01-2017




                                            •   Time:
                                                Measured time.



                 A+W Business Pro Capacity Planning                                                                   H-223
                 Default Times                                                                        Software Reference




                                           •   Time unit:
                                               Unit to which the measured time refers, e.g. to piece, square meter, linear
                                               meter, etc.
                                           •   Minimum time:
                                               Minimum time that is calculated for an item if the required time is here.
                                           •   Type:
                                               Type of the time. The type specifies how the time shall be calculated, e.g.
                                               as basic time or surcharge.
                                                “Default Times – Time Selection” on page H-218


                                           Default Times – Cube
                                           Capacity planning > Master data > Default Times > Default Times > Cube tab




                 Fig. H-148   Default Times – Cube


                                           On this tab, you store default times that are graduated according to three limit
                                           types, e.g. by height, width, and thickness.
                                           The fields are described on the Matrix tab.
                                            “Default Times – Matrix” on page H-221
4.02 / 01-2017




                 H-224                                                             A+W Business Pro Capacity Planning
                 Software Reference                                                                       Default Times




                                        Change Default Times
                                        Capacity planning > Master data > Default Times > Default Times > Functions
                                        menu > Change




                                        Fig. H-149    Change default times


                                        On this dialog, you can change the default times for a machine or work type.
                                        If, for example, you enter the factor 1.5, all times of the selected combination
                                        of machine and work time are increased by half. The factor 0.5 would reduce
                                        the times by half.


                                        Copy Default Times
                                        Capacity planning > Master data > Default Times > Default Times > Functions
                                        menu > Copy




                                        Fig. H-150    Copy default times


                                        On this dialog, you can copy default times from a machine and work type to
                                        transfer them to another machine and work type. You can also reduce or in-
                                        crease the values by a factor.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-225
                 Default Times                                                                           Software Reference




                                              Special Times
                                              Capacity planning > Master data > Default Times > Special Times




                 Fig. H-151   Special times


                                              On this dialog, you define the time surcharges for especially time-consuming
                                              processings, e.g. for special sizes. You can assign the time surcharges on the
                                              Default Times dialog in the Other surcharges group. Special times which have
                                              been defined with the same criteria, can be collected in groups (tables).
                                               Tutorial, “Special Times” on page H-58
                                              Another possibility for defining time surcharges in the form of factors is using
                                              the allocation dialog boxes.
                                               “Default Times (dialog)” on page H-217
                                               “Allocation” on page H-229

                                              Time surcharge for

                                              Number Use-defined number (ID) of the table.

                                              Name Name of the table, e.g. oversizes.

                                              Surcharges (overview)
                                              In the overview, all defined surcharges are listed.
4.02 / 01-2017




                                              Surcharges
                                              In the overview, the graduation of the time surcharge is shown that is selected
                                              on the Table tab.


                 H-226                                                                   A+W Business Pro Capacity Planning
                 Software Reference                                                                                Default Times




                                             •     Up to limit 1, 2:
                                                   Value per limit type up to which the surcharge shall be calculated.
                                             •     Limit type 1, 2:
                                                   Limit type to which the limit value refers, e.g. the edge length for the calcu-
                                                   lation of oversizes.
                                                    Master Data, “Quantity Limits” on page B-872
                                             •     Surcharge:
                                                   Amount of the surcharge. The value refers to the surcharge unit.
                                             •     Surcharge unit:
                                                   Unit with which the surcharge shall be calculated.
                                             •     Surcharge type:
                                                   Basis on which the surcharge is assessed.


                                             Special Priorities
                                             Capacity planning > Master data > Default Times > Special priorities




                 Fig. H-152   Special priorities


                                             On this dialog, you enter the priorities per machine and work type based on
                                             additional criteria, e.g. by product class, thickness, customer. If there is a zero
                                             (0) in the fields, the special priority applies overall, e.g. to the selected custom-
                                             er or to the specified quantity.
                                             This can be useful in the following cases:
                                             •     If several machines of the same type are available for a work type.
                                             •     If customers require special processing steps, which can only be executed
                                                   on special machines.
4.02 / 01-2017




                                             Work type Work type for which an exception has been defined.

                                             Machine Machine on which the work type is performed.


                 A+W Business Pro Capacity Planning                                                                       H-227
                 Default Times                                                            Software Reference




                                 Customer Customer to whom the priority applies.

                                 Company Company to whom the priority applies.

                                 PGR Product group to which the priority applies.

                                 Edge length Edge length in mm, to which the priority applies.

                                 Thickness >= Glass thickness in mm, to which the priority applies. 0 = all
                                 thicknesses.

                                 Quantity > Quantity starting from which the priority applies, e.g. number of
                                 holes, of corner cut-outs.

                                 Drilling diameter >= Diameter of a hole in mm from which on the priority is
                                 applied.

                                 Priority The digits have the following meaning:
                                 • 9: highest priority (standard machine). These machines are always select-
                                    ed first.
                                 • 8 to 1: decreasing priority. These machines are selected depending on uti-
                                    lization.
                                 • 0: lowest priorities. These machines are only selected if all other (equiva-
                                    lent) machines are used to capacity.
                                 • -1: for manual scheduling. These machines are selected by automatic
                                    scheduling only in case of bottlenecks.
                                 • -2: only for manual scheduling. These machines are never selected by au-
                                    tomatic scheduling. The machine can only be selected manually.
                                 • -3: is only selected with reporting from the production system when orders
                                    have been rescheduled there. In case of rescheduling in capacity planning,
                                    only machines with prio >-3 are displayed.
4.02 / 01-2017




                 H-228                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                        Allocation




                                        Allocation
                                        Capacity planning > Master data > Allocation
                                        On these dialogs, you allocate the basic products of A+W Business Pro (single
                                        glass, TG, LG, processings, shapes, muntions, etc.) to the work types.
                                        This section provides information on the following subjects:
                                        •   “Product Types” on page H-230
                                        •   “PGR” on page H-232
                                        •   “Product Class” on page H-233
                                        •   “Products” on page H-234
                                        •   “Combined Product Type” on page H-235
                                        •   “Special Allocation 1” on page H-236
                                        •   “Special Allocation 2” on page H-237
                                        •   “Special Allocation 3” on page H-239
                                        •   “Special Allocation 4” on page H-241
                                        •   “Combined Product Class” on page H-243
                                        •   “Stock Articles” on page H-244
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                           H-229
                 Allocation                                                                          Software Reference




                                          Product Types
                                          Capacity planning > Master data > Product Types




                 Fig. H-153   Product Types


                                          On this dialog, you allocate the work types to the A+W Business Pro product
                                          types in the sequence in which they will be performed in production or in ship-
                                          ping. For each work type, you can specify a time factor that shall be calculated
                                          for planning.
                                           Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                          Product type Product type to which work types are allocated.

                                          Work types
                                          In the overview, the allocated work types are displayed.

                                          # Number of the sequence.

                                          Work type Product number and name of the work type. If you enter <n.e.>
                                          the product type is ignored. This makes sense for the product type Surcharg-
                                          es, for example.
4.02 / 01-2017




                 H-230                                                            A+W Business Pro Capacity Planning
                 Software Reference                                                                         Allocation




                                        Factor The time calculated at scheduling is multiplied by this factor.
                                        • 0 or 1: the time is not increased or reduced.
                                        • 1: A factor of 1.5 corresponds to a time increase of 50%.

                                        Buttons

                                        [New], [Delete] With these buttons you enable a new row or delete a marked
                                        entry.

                                        Arrow buttons Use this buttons to change the sequence of work types. For
                                        the product type TG, for example, the allocation could look as follows:
                                        • Wash glass
                                        • Check
                                        • Produce TG
                                        • Package processed TG
                                        • Loading

                                        List of allocations
                                        In the list, the product types are displayed to which work types are assigned.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-231
                 Allocation                                                                           Software Reference




                                           PGR
                                           Capacity planning > Master data > PGR




                 Fig. H-154   Product groups


                                           On this dialog, you allocate the product types to the A+W Business Pro prod-
                                           uct groups in the sequence in which they will be performed in production or in
                                           shipping. For each work type, you can specify a time factor that shall be cal-
                                           culated for planning.
                                            Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                           Identification

                                           Product group Product group to which the work types are allocated.

                                           Work types
                                           The fields and buttons in this group are described for the Product types dialog.
                                            “Product Types” on page H-230

                                           List of allocations
4.02 / 01-2017




                                           In the list, the product groups are displayed to which work types are assigned.




                 H-232                                                             A+W Business Pro Capacity Planning
                 Software Reference                                                                                  Allocation




                                              Product Class
                                              Capacity planning > Master data > Product Class




                 Fig. H-155   Product Class


                                              On this dialog, you allocate the work types to the A+W Business Pro product
                                              classes in the sequence in which they will be performed in production or in
                                              shipping. For each work type, you can specify a time factor that shall be cal-
                                              culated for planning.
                                               Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                              Identification

                                              Product class Product class to which work types are allocated.

                                              Work types
                                              The fields and buttons in this group are described for the Product types dialog.
                                               “Product Types” on page H-230

                                              List of allocations
4.02 / 01-2017




                                              In the list, the product classes are displayed to which work types are assigned.




                 A+W Business Pro Capacity Planning                                                                     H-233
                 Allocation                                                                         Software Reference




                                         Products
                                         Capacity planning > Allocation > Products




                 Fig. H-156   Products


                                         On this dialog, you allocate the work types to the A+W Business Pro products
                                         in the sequence in which they will be performed in production or in shipping.
                                         For each work type, you can specify a time factor that shall be calculated for
                                         planning.
                                          Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                         Identification

                                         Product Product to which work types are allocated.

                                         Work types
                                         The fields and buttons are described for the Product types dialog.
                                          “Product Types” on page H-230

                                         List of allocations
4.02 / 01-2017




                                         In the list, the products are displayed to which work types are assigned.




                 H-234                                                           A+W Business Pro Capacity Planning
                 Software Reference                                                                              Allocation




                                          Combined Product Type
                                          Capacity planning > Master data > Combined product type




                 Fig. H-157   Combined product types


                                          On this dialog, you allocate the work types to the A+W Business Pro products
                                          that are a component of a BOM or affect a product group as a processing. You
                                          allocate the work types in the sequence in which they are performed in pro-
                                          duction or in shipping. For each work type, you can specify a time factor that
                                          shall be calculated for planning.
                                           Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                          Identification

                                          Product Product which – as a BOM element e.g. of TG, LG, etc. – has been
                                          assigned a work type other than the work type defined by default for the main
                                          product.

                                          As part of, affects If the float sheet is part of a BOM, the production se-
                                          quence or the work type can change. Enter the appropriate product type, e.g.
                                          TG.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-235
                 Allocation                                                                            Software Reference




                                            Work types
                                            The fields and buttons in this group are described for the Product types dialog.
                                             “Product Types” on page H-230

                                            List of allocations
                                            In the list, the combination product types are displayed to which work types are
                                            assigned.


                                            Special Allocation 1
                                            Capacity planning > Allocation > Special Allocation 1




                 Fig. H-158   Special Allocation 1 – Processings


                                            On this dialog, you allocate the work types to a A+W Business Pro processing
                                            product and the subsequent processing. You allocate the work types in the se-
                                            quence in which they are performed in production or in shipping. For each
                                            work type, you can specify a time factor that shall be calculated for planning.
                                             Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97
4.02 / 01-2017




                                            Identification

                                            Processing Processing to which work types are allocated.


                 H-236                                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                             Allocation




                                           Next processing Next processing to which work types are allocated.

                                           Work types
                                           The fields and buttons in this group are described for the Product types dialog.
                                            “Product Types” on page H-230

                                           List of allocations
                                           In the list, the processings and next processings are displayed to which work
                                           types are assigned.


                                           Special Allocation 2
                                           Capacity planning > Allocation > Special Allocation 2




                 Fig. H-159   Special Allocation 2 – Processings to shapes


                                           On this dialog, you allocate the work types to a processing on shapes and the
                                           subsequent processing. You allocate the worktypes in the sequence in which
                                           they are performed in production or in shipping. For each work type per edge,
                                           you can specify a time factor that shall be calculated for planning.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-237
                 Allocation                                                                 Software Reference




                                 Example

                                 On a sheet with round edges, the edge processing on straight edges can be
                                 performed on the standard grinding machine, the edge processing for the
                                 round edges must be done on another machine.


                               Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                              Identification

                              Processing Processing to which work types are allocated.

                              Shape Shape to which work types are allocated.

                              Up to qty. Quantity if the assignment of the work types depends on the num-
                              ber of sheets, e.g. large quantities on CNC machines. Enter 9999 if the quan-
                              tity shall not be checked.




                              Fig. H-160   Identification of corners and edges of the selected shape


                              Work types
                              In the overview, the allocated work types are displayed. The number of edges
                              depends on the shape selected.
                              The buttons are described for the Product types dialog.
                               “Product Types” on page H-230

                              # Number of the sequence.

                              Work type Number and name of the work type. If you enter <n.e.> the pro-
                              cessing is ignored.

                              Factor The time calculated during scheduling is multiplied by this factor.
                              • 0 or 1: the time is not increased or reduced.
                              • 1: A factor of 1.5 corresponds to a time increase of 50%.

                              1 - n (edge) Specification to which edge the factor applies. The number of
                              fields available depends on the number of edges and corners of the shape. In
                              the shape sketch, the edges are marked with red numbers.
                               The factor is not calculated for this edge.
                               The factor is calculated.

                              List of allocations
4.02 / 01-2017




                              In the list, the processings on shapes are displayed to which work types are
                              assigned.



                 H-238                                                 A+W Business Pro Capacity Planning
                 Software Reference                                                                                      Allocation




                                            Special Allocation 3
                                            Capacity planning > Allocation > Special Allocation 3




                 Fig. H-161   Special Allocation 3 – Edge processing (rectangular sheets)


                                            On this dialog, you allocate the sequence of edge processing for rectangular
                                            sheets.

                                               Example

                                               If for a rectangular sheet all edges shall be polished, by default the edges 1
                                               and 3 are polished simultaneously and after that 2 and 4 (or vice-versa).

                                               If on a machine 2 edges across from one another can be polished, seamed,
                                               etc. simultaneously, then you must assign the work type per edges 1 + 3
                                               and 2 + 4.


                                             Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                            Identification

                                            Processing Processing to which work types are allocated.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                         H-239
                 Allocation                                                                   Software Reference




                              Edges 1 - 4 Specification to which edges the allocation applies.
                               This edge is not processed.
                               This edge is processed.




                              Fig. H-162   Identification of corners and edges for the calculation of the factor


                              Work types
                              In the overview, the allocated work types are displayed. A factor can be spec-
                              ified per edge.
                              The buttons are described for the Product types dialog.
                               “Product Types” on page H-230

                              # Number of the sequence.

                              Work type Number and name of the work type. If you enter <n.e.> the pro-
                              cessing is ignored.

                              Factor The time calculated during scheduling is multiplied by this factor.
                              • 0 or 1: the time is not increased or reduced.
                              • >1: A factor of 1.5 corresponds to a time increase of 50%.

                              1 - 4 (edges) Specification to which edges the factor applies. In the shape
                              sketch, the edges are marked with red numbers.
                               The factor is not calculated for this edge.
                               The factor is calculated.

                              List of allocations
                              In the list, the processings are displayed to which work types are assigned.
4.02 / 01-2017




                 H-240                                                   A+W Business Pro Capacity Planning
                 Software Reference                                                                                     Allocation




                                            Special Allocation 4
                                            Capacity planning > Allocation > Special Allocation 4




                 Fig. H-163   Special Allocation 4


                                            On this dialog, you allocate different work types to a product, depending on the
                                            next processing and a shape. For each work type, you can specify a time fac-
                                            tor that shall be calculated for planning.
                                             Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                            Identification

                                            Product Product to which work types are allocated.

                                            Next processing Next processing to which work types are allocated.

                                            Shape Shape to which the allocation applies.
4.02 / 01-2017




                                            Fig. H-164   Identification of corners and edges for the calculation of the factor




                 A+W Business Pro Capacity Planning                                                                         H-241
                 Allocation                                                             Software Reference




                              Work types
                              In the overview, the allocated work types are displayed. The number of fields
                              for the edges depends on the selection of the shape.
                              The buttons are described for the Product types dialog.
                               “Product Types” on page H-230

                              # Number of the sequence.

                              Work type Number and name of the work type. If you enter <n.e.> the pro-
                              cessing is ignored.

                              Factor The time calculated during scheduling is multiplied by this factor.
                              • 0 or 1: the time is not increased or reduced.
                              • >1: A factor of 1.5 corresponds to a time increase of 50%.

                              1 - n (edges) Specification to which edges the factor applies. The number of
                              fields available depends on the number of edges of the shape. In the shape
                              sketch, the edges are marked with red numbers.
                               The factor is not calculated for this edge.
                               The factor is calculated.

                              List of allocations
                              In the list, the processings are displayed to which work types are allocated.
4.02 / 01-2017




                 H-242                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                              Allocation




                                          Combined Product Class
                                          Capacity planning > Master data > Combined product class




                 Fig. H-165   Combined product classes


                                          On this dialog, you allocate the work types and a time factor to the products
                                          that are a component of a BOM or affect a product class as a processing. For
                                          each work type, you can specify a time factor that shall be calculated for plan-
                                          ning.
                                           Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                          Identification

                                          Product Product to which, as BOM of e.g. TG, LG, etc., is assigned to anoth-
                                          er work type than the one that normally applies to the main product.

                                          As part of, affects If the float sheet is part of a BOM, the production se-
                                          quence or the work type can change. Enter the appropriate product type, e.g.
                                          LG

                                          Work types
4.02 / 01-2017




                                          The fields and buttons in this group are described for the Product types dialog.
                                           “Product Types” on page H-230



                 A+W Business Pro Capacity Planning                                                                 H-243
                 Allocation                                                                                Software Reference




                                               List of allocations
                                               List of the products to which work types are allocated.


                                               Stock Articles
                                               Capacity planning > Allocation > Stock articles




                 Fig. H-166   Stock articles


                                               On this dialog, you allocate the work type Shipping to stock articles. This allo-
                                               cation is used because stock articles (supply type Stock withdrawal) will not be
                                               processed, e.g. handles which are just packed and shipped. As a result, this
                                               product class is, e.g., scheduled for dispatch, and the appropriate cost and
                                               time is calculated. For each stock article, you can specify a time factor that
                                               shall be calculated for planning.
                                                Tutorial, “Allocate the A+W Business Pro Master Data” on page H-97

                                               Identification

                                               Product class Stock articles to which work type is allocated.
4.02 / 01-2017




                 H-244                                                                 A+W Business Pro Capacity Planning
                 Software Reference                                                                          Allocation




                                        Work types
                                        The fields and buttons in this group are described for the Product types dialog.
                                         “Product Types” on page H-230

                                        List of allocations
                                        In the list, the product classes are displayed to which work type is assigned.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-245
                 Lock                                                              Software Reference




                         Lock
                         You must define locks to prevent, for example, that particular work is per-
                         formed twice or that a machine is planned that cannot provide a service for a
                         particular product.
                         The procedure for locking products, product classes or product groups on par-
                         ticular machines is similar in all dialogs.
                         This section provides information on the following subjects:
                         •   “Lock by PGR” on page H-247
                         •   “Lock by Product Classes” on page H-248
                         •   “Lock Machines by Products” on page H-250
                         •   “Skip next Machine” on page H-251
                         •   “Customer-related Locks” on page H-252
                         •   “Define Production Line” on page H-254
                         •   “Skip Processes” on page H-255
4.02 / 01-2017




                 H-246                                          A+W Business Pro Capacity Planning
                 Software Reference                                                                                 Lock




                                            Lock by PGR
                                            Capacity planning > Lock > Lock by PGR




                 Fig. H-167   Lock by PGR


                                            On this dialog, you lock particular product groups for one or more machines.
                                             Tutorial, “Locks” on page H-90

                                            Identification

                                            Product group Product group for which the machine is locked.

                                            Machines
                                            In the overview, the allocated machines are displayed.

                                            # Number of the sequence.

                                            Machine Number and name of the machine.

                                            Buttons
4.02 / 01-2017




                                            [New], [Delete] With these buttons you enable a new row or delete a marked
                                            entry.



                 A+W Business Pro Capacity Planning                                                               H-247
                 Lock                                                                                       Software Reference




                                           Arrow buttons With these buttons you can change the sequence of the
                                           work types.

                                           Lock overview
                                           In the list, the PGRs are displayed for which the locks were defined.


                                           Lock by Product Classes
                                           Capacity planning > Lock > Lock by product types




                 Fig. H-168   Lock by product classes


                                           On this dialog, you lock a product class depending on the work type for one or
                                           more machines.
                                            Tutorial, “Locks” on page H-90


                                              Example

                                              Two IG lines are available for IG production. Steel spacers can be fitted into
                                              the IG unit only on IG line no. 2 however.
                                              This is why product class IG must be locked for IG line no. 1 for the work
4.02 / 01-2017




                                              type Fit steel spacer.




                 H-248                                                                 A+W Business Pro Capacity Planning
                 Software Reference                                                                                Lock




                                        Identification

                                        Product class Product class for which the machine is locked.

                                        Machines
                                        The buttons are described for the Lock by PGR dialog.
                                         “Lock by PGR” on page H-247

                                        # Number of the sequence.

                                        Work type Number and name of the work type.

                                        Machine Number and name of the machine.

                                        Total In the combination of product class and work type, the machine can be
                                        locked completely or partially.
                                         This machine is locked only for this product class (main product) and this
                                        work type.
                                         If the product class including the work type is component of a BOM, then
                                        the machine is locked completely, i.e. also for all other work types that affect
                                        the main product and its BOM components.

                                        Lock overview
                                        In the overview, the product classes are displayed for which the locks were de-
                                        fined.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-249
                 Lock                                                                               Software Reference




                                           Lock Machines by Products
                                           Capacity planning > Lock > Lock by products




                 Fig. H-169   Lock machines by products


                                           On this dialog, you lock a product depending on the work type for one or more
                                           machines.
                                            Tutorial, “Locks” on page H-90

                                           Identification

                                           Product Product for which the machine is locked.

                                           Machines
                                           The fields and buttons are described for the Lock machines by products dia-
                                           log.
                                            “Lock by Product Classes” on page H-248

                                           Lock overview
                                           In the overview, the products are displayed for which the locks were defined.
4.02 / 01-2017




                 H-250                                                           A+W Business Pro Capacity Planning
                 Software Reference                                                                                             Lock




                                           Skip next Machine
                                           Capacity planning > Lock > Skip next machines




                 Fig. H-170   Skip next machines


                                           On this dialog, you lock a machine depending on the next machine.

                                              Example

                                              If the drilling line automatically includes washing, then you can lock the next
                                              machine Washing or skip it to prevent doubled washing.


                                            Tutorial, “Locks” on page H-90

                                           Identification

                                           Machine Machine for which the next machine is locked.

                                           Machine
                                           The fields and buttons are described for the Lock machines by products dia-
                                           log.
4.02 / 01-2017




                                            “Lock by Product Classes” on page H-248




                 A+W Business Pro Capacity Planning                                                                         H-251
                 Lock                                                                                         Software Reference




                                           Lock overview
                                           In the overview, the machines are displayed for which the locks were defined.


                                           Customer-related Locks
                                           Capacity planning > Lock > Customer-related locks




                 Fig. H-171   Customer-related locks


                                           On this dialog, you lock machines depending on the customer number, product
                                           or processing.

                                               Example

                                               If a customer insists that a particular drilling machine not be used for his
                                               orders, this drilling machine must be locked for him.


                                            Tutorial, “Locks” on page H-90

                                           Functions menu
                                           Using this menu, you can extend the lock of a customer to the entire customer
                                           group or lift the lock.
                                           The following entries are displayed:
                                           •   Set lock:
                                               The lock is expanded to all customers of the customer group to which the
                                               customer displayed belongs. All affected customers will be listed in the
                                               overview.
                                           •   Lift lock:
                                               The lock is deleted for all customers of the customer group. The customers
                                               are all removed from the overview.
4.02 / 01-2017




                 H-252                                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                                Lock




                                        Identification

                                        Customer Customer for whom the lock has been set.

                                        Product/processing Product or processing for which the machine is locked.

                                        Locked machine Machine that is locked.

                                        Table
                                        In the overview, all customers are displayed for whom locks are defined.
                                        • Customer no., Customer:
                                            Number and name of the customer.
                                        • Customer group:
                                            Customer group to which the customer belongs.
                                        • Place:
                                            Customer's headquarters.
                                        • Product no., Product:
                                            Number and name of the product for which the lock is defined.
                                        • Locked machine:
                                            Machine that is locked for the combination of customer and product.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                           H-253
                 Lock                                                                                Software Reference




                                            Define Production Line
                                            Capacity planning > Lock > Define production line




                 Fig. H-172   Define production line


                                            On this dialog, you lock a machine depending on the previous machine.
                                             Tutorial, “Define Production Line” on page H-93
                                            The buttons are described for the Lock by PGR dialog.
                                             “Lock by PGR” on page H-247

                                            Identification

                                            Machine Machine for which the next machine is locked. This next machine
                                            is specified in the Machines group.

                                            Machines
                                            In the overview, the work types and allocated machines are displayed.

                                            # Number of the sequence.
4.02 / 01-2017




                                            Work type Number and name of the work type.

                                            Machine Number and name of the machine.


                 H-254                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                                             Lock




                                           Total The machine can be locked partially or completely.
                                            The machine can be selected manually.
                                            This machine is completely locked for this work type.

                                           Lock overview
                                           In the overview, the machines are displayed for which the locks were defined.


                                           Skip Processes
                                           Capacity planning > Lock > Skip processes




                 Fig. H-173   Skip processes


                                           On this dialog, you lock next processings depending on the machine.

                                               Example

                                               If the drilling line includes washing, then you can lock the next process Wash
                                               glass to prevent doubled washing.


                                            Tutorial, “Locks” on page H-90
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                        H-255
                 Lock                                                               Software Reference




                         Identification

                         Machine Machine on which the work type is locked.

                         Work types
                         In the overview, the allocated work types are displayed.
                         The buttons are described for the Lock by PGR dialog.
                          “Lock by PGR” on page H-247

                         # Number of the sequence.

                         Work type Number and name of the work type for which the machine is
                         locked.

                         Lock overview
                         In the overview, the machines are displayed for which the locks were defined.
4.02 / 01-2017




                 H-256                                          A+W Business Pro Capacity Planning
                 Software Reference                                                                        Overviews




                                        Overviews
                                        With various tables and graphics, you get an overview of the utilization on a
                                        particular date or in a period of time.
                                        This section provides information on the following subjects:
                                        •   “Statistics” on page H-258
                                        •   “Area Graphic” on page H-259
                                        •   “Statistics by Order Area” on page H-260
                                        •   “Statistics by Order Area (short)” on page H-263
                                        •   “Accounts” on page H-264
                                        •   “Cost Centre Definitions” on page H-265
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-257
                 Overviews                                                             Software Reference




                             Statistics
                             Capacity planning > Overview > Statistics




                             Fig. H-174   Statistics


                             In this overview, you can display all orders that have been reported completed
                             by a machine within a period of time.
                             The screen display applies only to the selected machine. The printout, howev-
                             er, shows all machines and the time costs.

                             Selection

                             From, to Evaluation period. If you enter the same date in both fields, a daily
                             evaluation is created.

                             Machine Machine whose utilization is displayed.

                             Utilisation times
                             In the overview, he values for all quantities reported completed, by machine.
                             are listed.

                             … Work type

                             Pcs. Quantity reported completed.

                             Area Square meters reported completed.
4.02 / 01-2017




                             Circumference Edge length in total.



                 H-258                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                             Overviews




                                           Time Time required in total.

                                           Machine Machine that reported the values.

                                           Total time Total of the times for the selected machine.


                                           Area Graphic
                                           Capacity planning > Overview > Graphic Areas > Legend




                 Fig. H-175   Area graphic – Weekly overview


                                           In this overview, you display a graphic overview of the utilization either by ma-
                                           chine types or by production areas.
                                           You can limit the display with the Plant menu to a particular plant or a custom-
                                           er.
                                           The graphic can be opened from various dialogs. The display of the data is
                                           then filtered according to the initial dialog, e.g. per daily shift.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-259
                 Overviews                                                              Software Reference




                             Period

                             Date Date for which the graphic shall be created.

                             Week You can only evaluate the day entered or the whole week.
                              Only the selected day is evaluated.
                              The evaluation considers the whole week (Monday through Sunday).

                             Machine type, production area With the selection of the option, you specify
                             to what the evaluation shall refer.

                             [Legend] Shows/hides the legend with the significance of the colors in the
                             graphic. The setting applies to all graphics.

                             Graphic

                             Red lines The red line indicates the end of a shift.

                             Left column The left column changes depending on the day or week view.
                             • Day view: shifts
                             • Week view: day's date.


                             Statistics by Order Area
                             Capacity planning > Overview > Statistics by Order Area
                             Order area statistics is product-based and includes all work types reported
                             completed.
                             This dialog contains the following tabs:
                             •   “Statistics by Order Area – Selection” on page H-261
                             •   “Statistics by Order Area – Table” on page H-262
4.02 / 01-2017




                 H-260                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                            Overviews




                                        Statistics by Order Area – Selection
                                        Capacity planning > Overview > Statistics by Order Area > Selection tab




                                        Fig. H-176    Statistics by order area – Selection


                                        On this tab, you select the criteria according to which the overview of comple-
                                        tion reports shall be created. If you want to display all details for a period, you
                                        must not limit the search with restrictions.

                                        Evaluation period

                                        From, to Evaluation period. If you enter the same date in both fields, a daily
                                        evaluation is created.

                                        Restrictions
                                        In this group you can limit the selection.

                                           Entry <n.e.>
                                           If one of the fields shall not be taken into account, you have to delete the
                                           complete entry. <n. e.> means for example that the product type <n. e.>
                                           shall be excluded.
                                           To view information on all products, product classes, order areas, and pro-
                                           duction areas, leave all four fields empty.

                                        Product type The selected product type shall not be displayed.
4.02 / 01-2017




                                        Product class The selected product class shall not be displayed.

                                        Order area The selected order area shall not be displayed.



                 A+W Business Pro Capacity Planning                                                                H-261
                 Overviews                                                                               Software Reference




                                            Production area The selected production area shall not be displayed.

                                            Output / sorting
                                            The left field displays the output options. The right field shows the sorting cri-
                                            terion. This setting determines the display of the results on Table tab.
                                            You move a selected entry into the right field or back into the left field with the
                                            arrow buttons.

                                            List by
                                            With the selection of the option, you specify which data shall be displayed:
                                            •   Product type:
                                                The evaluation shall refer to the product type.
                                            •   Product class:
                                                The evaluation shall refer to the product class.
                                            •   Product:
                                                The evaluation shall refer to the products.


                                            Statistics by Order Area – Table
                                            Capacity planning > Overview > Statistics by Order Area > Table tab




                 Fig. H-177   Statistics by order area – Table


                                            On this tab, the results of the evaluation is displayed. Based on the selection
                                            criteria you can determine, for example in which order area the glass is con-
                                            sumed.
4.02 / 01-2017




                 H-262                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                         Overviews




                                        Overview
                                        The second column is filled in only if the sorting is made by production area
                                        and order area, no matter in which sequence this is done.
                                        •   Production area, Order area:
                                            Display depending on the sorting criterion.
                                        •   Product, Product class, Product type:
                                            Display depending on the selection of the sorting criterion.
                                        •   Process:
                                            This field displays the work types.
                                        •   Quantity:
                                            Quantities produced.
                                        •   Sqm:
                                            Area produced.
                                        •   Lm:
                                            Linear meters produced (edges)
                                        •   Time costs:
                                            Time costs determined.
                                        •   Material costs:
                                            Material costs determined.


                                        Statistics by Order Area (short)
                                        Capacity planning > Overview > Statistics by Order Area (short)
                                        On this dialog, you can display an abbreviated list of the evaluation by order
                                        areas, which is automatically sorted according to the two criteria Order area
                                        and Production areas.
                                        The fields are described for the Order area statistics dialog.
                                         “Statistics by Order Area” on page H-260
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-263
                 Overviews                                                             Software Reference




                             Accounts
                             Capacity planning > Overview > Accounts




                             Fig. H-178    Accounts – Selection


                             On this dialog, you can display to which cost centres or order areas particular
                             products, product classes or product types were booked. The data is read out
                             of the orders. Archived orders are not taken into consideration.

                             Cost centres menu
                             Using this menu, you can open the Cost centre definition dialog to create or
                             edit the cost centres.
                              “Cost Centre Definitions” on page H-265

                             Evaluation period delivery date

                             From, to Evaluation period. If you enter the same date in both fields, a daily
                             evaluation is created.

                             Sorted by
                             With the selection of the option, you specify how the display shall be sorted:
                             • Cost centres:
                                These are the cost centres that you have created for capacity planning.
                                  “Cost Centre Definitions” on page H-265
4.02 / 01-2017




                             •   Order areas:
                                 Order areas from the A+W Business Pro master data.




                 H-264                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                         Overviews




                                            Define cost centres
                                            You define new cost centres the same way as the preview columns in the
                                            Production module.

                                        List by
                                        With the selection of the option, you specify whether the evaluation is dis-
                                        played by product type, product class or according to the individual products.

                                        Overview
                                        The following data is displayed in the overview:
                                        •   Cost centre:
                                            Name of the cost centre. The names are specified on the Cost centre def-
                                            inition dialog.
                                             “Cost Centre Definitions” on page H-265
                                        •   Order area:
                                            Order area to which the cost centre is assigned.
                                        •   Product type, product class, product:
                                            The display of the appropriate data depends on the option that was select-
                                            ed on the Selection tab.
                                        •   Qty:
                                            Quantity of sheets produced.
                                        •   Area:
                                            Total area of the sheets produced.
                                        •   Material costs:
                                            Material costs of the sheets produced.


                                        Cost Centre Definitions
                                        Capacity planning > Overview > Accounts > Cost centres menu




                                        Fig. H-179    Cost centre definition
4.02 / 01-2017




                                        On this dialog, you specify the cost centres for the evaluation of production
                                        data and costs.




                 A+W Business Pro Capacity Planning                                                             H-265
                 Overviews                                                                  Software Reference




                             Before you create cost centres, you should consider in which sequence the
                             cost centres should be queried.

                                Example TG

                                First you query whether this is a TG with processing (cost centre no. 7 with
                                prio 19).
                                If this is not the case, the follow-up query starts.

                                The TG that is not processed flows automatically into the cost centre TG
                                (cost centre no. 6 with prio 20).

                                Define cost centres
                                You define new cost centres the same way as the preview columns in the
                                Production module.

                             No. Number of the cost centre.

                             Name Name of the cost centre.

                             MPT Main product type. In this field you enter the product type for which the
                             evaluation shall be done.

                             No 1, No 2 These entries refer to the fields Type 1 and Type 2. Here you en-
                             ter the number for the product type or product class of Type 1 or Type 2 or 0
                             for no specification.

                             Type 1, type 2 Product type or product class that is BOM element of the
                             main product type.
                             • 0 = no specification
                             • 1 = product type
                             • 2 = product class
                             Example: You search for the Product class (Type 1 = 1) Processings (No 1 =
                             20), which is a component of TG (MPT = 2).

                             Priority Number of the sequence in which the query of the cost centres shall
                             be done.

                             Exclusion You can exclude a product from the rule. The product number
                             must be in brackets.

                                Example

                                All TG sheets are seamed. Therefore, seamed TG sheets shall not flow into
                                the cost centre 'Processed TG'.
                                You exclude this by entering the appropriate product number (in brackets).



                             Lisec Interface
4.02 / 01-2017




                             This dialog is only released if you are working with an appropriate interface.



                 H-266                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                Capacity Planning




                                        Capacity Planning
                                        Production > Capacity planning
                                        The Production module offers various dialogs for capacity planning purposes.
                                        Apart from transferring data to production, you can use this module to monitor
                                        the production progress by means of reports.
                                        This section provides information on the following subjects:
                                        •   “Scheduling” on page H-268
                                        •   “Production Reports” on page H-291
                                        •   “Control Station” on page H-325
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-267
                 Scheduling                                                              Software Reference




                              Scheduling
                              Time and material costs can only be calculated for orders that are scheduled
                              in capacity planning. Orders can be scheduled automatically at defined inter-
                              vals or manually.
                              This section provides information on the following subjects:
                              •   “Number Manager” on page H-268
                              •   “Schedule Number Manager” on page H-269
                              •   “Change Criteria (Search Date)” on page H-272
                              •   “Delivery Date” on page H-274
                              •   “Book Order” on page H-275
                              •   “Scheduling Result” on page H-280
                              •   “Machine Selection in Case of Bottleneck” on page H-281
                              •   “Order Numbers” on page H-283
                              •   “Split Items” on page H-284
                              •   “Item Times” on page H-286
                              •   “Machine Failure” on page H-287
                              •   “Residue Transfer” on page H-290
                              •   “Shift Settings” on page H-183



                              Number Manager
                              Production > Capacity planning > Booking > Number manager
                              You have the possibility to schedule several orders manually at once in capac-
                              ity planning. For this, the orders are collected in a number manager.
                              On the Schedule orders dialog, you can select the number manager and
                              schedule the orders. The program shows all number managers created for
                              documents.
                               “Schedule Number Manager” on page H-269
                              On the Number manager dialog, you can open the Production overview dialog
                              for the order you have selected in the overview. That dialog is described in de-
                              tail in the Sales section.
                               Sales, “Status Message” on page C-498
                              The Number manager dialog and the associated menus are the same for all
                              modules. It is described in detail in the Sales section.
                               Sales, “Number Manager” on page C-543
4.02 / 01-2017




                 H-268                                                A+W Business Pro Capacity Planning
                 Software Reference                                                                            Scheduling




                                        Schedule Number Manager
                                        Production > Capacity planning > Booking > Book NM
                                        Using a number manager, you schedule all orders manually that match the
                                        minimum status.
                                        This section provides information on the following subjects:
                                        •   “Functions Menu” on page H-269
                                        •   “Options Menu” on page H-269
                                        •   “Schedule Orders (Dialog)” on page H-270


                                        Functions Menu
                                        Production > Capacity planning > Booking > Book NM > Functions menu
                                        Using this menu, you can display the history of the selected order. The history
                                        is described in detail in the Sales section.
                                         Sales, “History” on page C-478


                                        Options Menu
                                        Production > Capacity planning > Booking > Book NM > Options menu
                                        Using this menu, you can determine the default setting of the dialog and open
                                        other dialogs without leaving the current dialog. You can activate or deactivate
                                        options. The setting will not be reset when you close the dialog. The following
                                        entries are displayed:
                                        •   Mode date search:
                                            Opens the Change criteria dialog on which you can specify the criteria for
                                            the schedule search.
                                             “Change Criteria (Search Date)” on page H-272
                                        •   Item check:
                                            When the order is scheduled, the program checks its share in the daily ca-
                                            pacity. The percentage is defined on the Work types dialog.
                                             “% Limit” on page H-189
                                        •   Old dwell day mode:
                                            This setting is only required if you want to retain the old mode for dwell days
                                            (= Transition matrix).
                                        •   Check for ST:
                                            If the set-up time has been defined for several work types performed for an
                                            order item, this time shall be charged just once per item.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-269
                 Scheduling                                                                       Software Reference




                                          Schedule Orders (Dialog)
                                          Production > Capacity planning > Booking > Book order




                 Fig. H-180   Schedule by number manager


                                          On this dialog, you transfer the orders from a number manager to capacity
                                          planning. You start the transfer with the menu Start > Execute.
                                           Tutorial, “Scheduling Orders” on page H-108

                                          Identification

                                          Client Selection of the client whose orders shall be scheduled.

                                          Area Selection of the order area whose orders shall be scheduled.
                                           Master Data, “Order Areas” on page B-983

                                          Employee Employee logged in.

                                          Number Manager If you have selected a number manager, all orders are
                                          transferred that are in this number manager and have achieved the minimum
                                          status.
4.02 / 01-2017




                 H-270                                                            A+W Business Pro Capacity Planning
                 Software Reference                                                                            Scheduling




                                        Order priority
                                        The field is only released if you have selected the Take over changed priority
                                        in order setting on Company data > Capacity planning tab > Scheduling priority
                                        field.
                                        Orders are usually scheduled withe Normal priority. Only e.g. for rush orders
                                        which have to have shorter through times, you will have to select the appropri-
                                        ate priority.
                                        • Normal:
                                           The order is scheduled according to the default settings.
                                        • Urgent:
                                           The order must be scheduled with top priority.
                                        • Release order:
                                           The order is only produced if the customer calls the items.
                                        • Extra:
                                           This priority means that the order shall be produced from residue (plates)
                                           left over from cutting other orders.

                                            Consider order priority
                                            If in addition to the order priority Normal the priority Urgent shall be consid-
                                            ered, a special transition time must be defined for the corresponding com-
                                            bination of production areas. This applies to all times that can be shortened
                                            for rush orders if required.

                                             “Transition Times” on page H-192
                                             “Transition Matrix” on page H-210

                                        Behavior in case of delivery date problems
                                        With the selection of the option, you specify how the program shall react to
                                        problems during scheduling:
                                        • No automatism:
                                           The order shall not be automatically scheduled for the next possible pro-
                                           duction date. If this option is chosen, Delivery date dialog opens on which
                                           you can specify the settings for scheduling.
                                             “Delivery Date” on page H-274
                                        •   Next delivery date:
                                            The order shall be scheduled on the next possible delivery date. The new
                                            delivery date is written back to the order.
                                        •   Schedule for delivery date:
                                            The order shall be scheduled for the original delivery date, even if this ex-
                                            ceeds the machine capacities. You can select this option if you are sure
                                            that you can postpone other, already scheduled orders.
                                        •   Infinite capacities:
                                            The order will be scheduled regardless of the actual capacities.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-271
                 Scheduling                                                                Software Reference




                              Change Criteria (Search Date)
                              Production > Capacity planning > Booking > Book NA > Options menu >
                              Search date
                              Production > Capacity planning > Booking > Book order > Functions menu >
                              Mode date search




                              Fig. H-181   Settings for schedule search


                              On this dialog, you specify the criteria for manual scheduling or in case of ca-
                              pacity problems. The settings are valid only for the current scheduling.

                              Determine the production date
                              With these settings you override the default settings from the company data.
                              The overridden settings apply only to the current session:
                              • Autom. normal capacity:
                                 The orders will be scheduled based on the available shift times. Overbook-
                                 ing is impossible. This is the default setting (closed capacities).
                              • Automatic full days:
                                 This setting ignores the specifications for the number of shifts and hours in
                                 the calendar. Scheduling is based on a workday of 24 hours in this case
                                 (open capacities). This applies only to common workdays, not to holidays.
                              • Change machine only:
                                 If capacities are fully utilized, the program will automatically search for an-
                                 other machine. If this is used to capacity as well, scheduling is interrupted
                                 and manual intervention is required.
                              • Schedule without check:
                                 This setting represents an open shift. This means e.g. that despite a shift
                                 time of 8 h, 16 h can be scheduled as well. The program will issue no report
                                 if a day's capacity is fully utilized. This option should only be used in excep-
4.02 / 01-2017




                                 tional cases.




                 H-272                                                    A+W Business Pro Capacity Planning
                 Software Reference                                                                               Scheduling




                                        Mode for aligning the machines
                                        If you work with several machines that can perform the same work types,
                                        scheduling can consider these machines in different ways:
                                        • Automatic:
                                            The program automatically searches for the most cost- and time-effective
                                            machine and schedules the orders on this machine. This is the default set-
                                            ting.
                                        • Semi-automatic:
                                            The program offers the alternative machines for selection. If the delivery
                                            date cannot be adhered to, you must intervene.
                                        • Manual:
                                            With this option you must intervene manually for each possible change
                                            (machine, shift, etc.). Alternative machines can only be selected for the
                                            manual scheduling or rescheduling.

                                        Options

                                        Closing time For manual scheduling, you can specify the point in time up to
                                        which orders can be scheduled. This setting will be kept until the next change
                                        is made.

                                           Example

                                           You get a new order on Friday at 12 a.m. For manual scheduling, you enter
                                           14 h although the shift goes to 16 h. This ensures that the order will not be
                                           scheduled if it cannot be produced on this day. You thus prevent residual
                                           quantities of not-yet-begun orders from arising, which must then be
                                           rescheduled on the following day.
                                           If the order cannot be scheduled due to the closing time, an appropriate
                                           message will be displayed on the Delivery date dialog. You then have to
                                           change the delivery date.


                                        Closing times are generally defined on the Shift settings dialog.
                                         “Shift Settings” on page H-183

                                        Reduced control Scheduling usually searches for each item for free capac-
                                        ities to schedule the order items.
                                        However, an order may contain items with the same BOM structure, where
                                        only the sizes are different.
                                         The entire BOM structure is checked for each item.
                                         If the BOM structure is the same, scheduling is based on the previous item
                                        without checking the BOM again. This is the default setting.
                                        The program notes the start date of production of the first item, e.g. on the
                                        grinding machine. The next item starts from that date, starts the capacity of this
                                        machine and if it this already running to capacity, goes to the previous shift or
                                        the previous day. The next item starts from that new date with its capacity
                                        check, etc.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                    H-273
                 Scheduling                                                               Software Reference




                              Do not split orders If an order cannot be produced on one day, the order
                              has to be split.
                               The order can be split so that production is distributed across several days.
                               The order shall not be split. The search for a suitable date must continue
                              until all capacities needed for this order are free.


                              Delivery Date
                              Production > Capacity planning > Booking > Book order, Book NM > Schedule




                              Fig. H-182   Delivery date for scheduling


                              On this dialog, you specify manually when or how the order shall be sched-
                              uled.
                              The dialog is displayed if the delivery date from the order cannot be kept be-
                              cause the capacity check did not come up with a suitable free date. These
                              manual settings will be recorded in the order history.
4.02 / 01-2017




                 H-274                                                    A+W Business Pro Capacity Planning
                 Software Reference                                                                            Scheduling




                                        The following options are available for selection:
                                        •   Define automatically:
                                            With this option, the next possible delivery date is determined and saved in
                                            the order. The customer's route days will be taken into account.
                                            This option is based on forward scheduling.
                                        •   Choose delivery date:
                                            With this option, you select another delivery date. he program then checks
                                            again whether sufficient capacities are available on that date. This process
                                            continues until the order can be scheduled.
                                            When scheduling is successful, the new date is saved in the order.
                                        •   Schedule for delivery date:
                                            With this option, the default times are ignored and the program tries to
                                            schedule the order for the delivery date. The search for free capacities
                                            goes one day back at a time until the current date. If by then no capacities
                                            are found, the order is scheduled on this day regardless of whether or not
                                            capacities are free.
                                        •   Infinite capacities:
                                            With this option, the order is scheduled for the delivery date regardless of
                                            whether or not capacities are free.
                                        •   Individual setting:
                                            With this option, it is first possible to determine the delivery date manually.
                                            After that, the program stops for each work type included in the order. You
                                            have to specify the appropriate machines, the production day, and the shift
                                            manually.

                                        [End] With this button, you abort the scheduling of the current order. After
                                        you have answered a security query with [Yes], the program proceeds with the
                                        next order in the number manager. The unscheduled order has to be sched-
                                        uled separately afterwards.


                                        Book Order
                                        Production > Capacity planning > Booking > Book order
                                        On this dialog, you schedule an individual order or an individual item of an or-
                                        der manually in capacity planning.
                                        This section provides information on the following subjects:
                                        •   “Functions menu” on page H-276
                                        •   “Options menu” on page H-277
                                        •   “Settings group” on page H-276
                                        •   “Book Order (Dialog)” on page H-277
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-275
                 Scheduling                                                                Software Reference




                              Functions menu
                              Production > Capacity planning > Booking > Book order
                              Using this menu, you can open other dialogs without closing the Schedule or-
                              der dialog.

                              Current order group
                              •   Scheduling result:
                                  Opens the Scheduling result dialog on which you can check the results of
                                  the scheduling.
                                   “Scheduling Result” on page H-280
                              •   Apply priority:
                                  Applies the changed priority and writes it back to the order. Only if you write
                                  back the change to the order is it considered during the scheduling.
                              •   Delete scheduling:
                                  Deletes the scheduled order from capacity planning, e.g. to scheduled it
                                  again using changed criteria or in case of cancellations.
                                  The order is deleted from capacity planning, the reserved capacities are re-
                                  leased again.
                              •   Transfer to production:
                                  Transfers the order directly to production.
                              •   Display messages:
                                  After scheduling, displays a message with various information about the
                                  scheduling.
                                  The entry is only released if you are logged in with administrator rights.

                              Settings group
                              •   Search date:
                                  Opens the dialog by the same name on which you can specify the criteria
                                  for the schedule search.
                                   “Change Criteria (Search Date)” on page H-272
                              •   Shift times:
                                  Opens Shift time settings dialog where you can define the shift transition
                                  and the closing time.
                                   “Shift Settings” on page H-183
                                  You must have administrator rights to open the dialog. In addition, the Use
                                  change of shift table checkbox must be ticked on the Company data dialog.
                                   “Use change of shifts table” on page H-182
                              •   Select shift:
                                  Enables the Shift field to enter the requested shift.
                              •   Residue transfer:
                                  Opens Residue transfer dialog where you can define the status up to which
                                  orders shall be checked for residue.
                                   “Residue Transfer” on page H-290
4.02 / 01-2017




                 H-276                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                            Scheduling




                                        Options menu
                                        Production > Capacity planning > Booking > Book order
                                        Using this menu, you can determine the default setting of the dialog. You can
                                        activate or deactivate options. The settings will not be reset when you close
                                        the dialog. The following entries are displayed:
                                        •   Old dwell day mode:
                                            This setting is only required if you want to retain the old mode for dwell days
                                            (= Transition matrix).
                                        •   Check for ST:
                                            If the set-up time has been defined for several work types performed for an
                                            order item, this time shall be charged just once per item.
                                        •   Item check:
                                            When the order is scheduled, the program checks its share in the daily ca-
                                            pacity. The percentage is defined on the Work types dialog.
                                             “% Limit” on page H-189
                                        •   Consider closing time for scheduling:
                                            The program shall check until when orders can be scheduled for a shift.
                                             “Shift Settings” on page H-183


                                        Book Order (Dialog)
                                        Production > Capacity planning > Booking > Book order




                                        Fig. H-183    Book order manually
4.02 / 01-2017




                                        On this dialog, you schedule an individual order or an individual order item
                                        manually in capacity planning.
                                         Tutorial, “Scheduling Orders” on page H-108


                 A+W Business Pro Capacity Planning                                                                H-277
                 Scheduling                                                                 Software Reference




                              Order information

                              Order Entry of the order number.

                              Customer Display of the customer name.

                              Shipping date Shipping date from the order. You can overwrite the date. The
                              change is written back to the order. If you have ticked the checkbox Keep de-
                              livery date, you cannot choose another date.

                                 Pushing up production
                                 In order to push up the scheduling of production, you have to change the
                                 shipping date first before ticking the checkbox Keep delivery date.

                              Shift Specification of the shift number in which the order shall be produced.
                              The field is released in menu Functions > Settings group > Select shift.

                              Status Current order status.

                              Priority By default, the orders are scheduled with the priority Normal. You
                              can select another priority and use the Functions menu > Settings group > Ap-
                              ply priority to write it back to the order. Only after that is the new priority con-
                              sidered for scheduling. The following entries are available for selection:
                              • Normal:
                                  The order is scheduled according to the default settings.
                              • Urgent:
                                  The order must be scheduled with top priority.
                              • Release order:
                                  The order is only produced if the customer calls the items.
                              • Extra:
                                  This priority means that the order shall be produced from residue (plates)
                                  left over from cutting other orders.

                                 Consider order priority
                                 If in addition to the order priority Normal the priority Urgent shall be consid-
                                 ered, a special transition time must be defined for the corresponding com-
                                 bination of production areas. If these have not been defined, the order will
                                 be scheduled with Normal priority.

                                  “Transition Times” on page H-192
                                  “Transition Matrix” on page H-210
4.02 / 01-2017




                 H-278                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                           Scheduling




                                        Options

                                        Schedule individual item You can schedule individual items from an order.
                                         All items of the order are scheduled.
                                         The field for entry of the item number is released. Only the defined item will
                                        be scheduled.

                                        Item number Entry of the item that shall be scheduled. The field is only re-
                                        leased if the Schedule individual item checkbox is ticked.

                                        Also use priority -1 Machine selection takes the machine priorities into ac-
                                        count. By default, the program checks the availability of the machine with the
                                        highest priority. Priority -1 is usually assigned to the machines for manual se-
                                        lection, e.g. manual cutting.
                                         Machines with priority -1 can only be scheduled manually.
                                         Machines with priority -1 are included in the scheduling process.

                                        Keep delivery date If the utilization of the machines makes the delivery date
                                        impossible, it can be postponed.
                                         Order scheduling permits postponing the delivery date.
                                         The order shall be scheduled so that the delivery date stated in the order
                                        is kept. With this setting, you will not be able to choose another date in field
                                        Shipping date.

                                        Earliest production start If you have a delivery date that is far in the future,
                                        you can specify the earliest date for production start.

                                        Current scheduling
                                        In this group is displayed which item is currently being scheduled.

                                        Item/processings
                                        In the overview, the product names and processings of the individual items are
                                        displayed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-279
                 Scheduling                                                                              Software Reference




                                            Scheduling Result
                                            Production > Capacity planning > Booking > Book orders > Functions menu >
                                            Scheduling result




                 Fig. H-184   Result of the scheduling


                                            On this dialog, you check how the order was scheduled.

                                            Processes
                                            In the overview, the items are displayed per work type.
                                            •   Item:
                                                Item number from the order.
                                            •   Machine:
                                                Name of the machine.
                                            •   Work type:
                                                Work type that is performed on the machine.
                                            •   Time:
                                                Time scheduled per item and work type. The totals line shows the total time
                                                scheduled for this order.
                                            •   Pcs.:
                                                Number of process steps, e.g. 10 sheets to be cut but 4 x 10 units for
                                                rounded corners.
                                            •   Date:
                                                Production date.
                                            •   Shift:
                                                Shift in which the item is scheduled.
                                            •   Costs:
                                                Costs per work type and item. In the total line, the total costs for the order
4.02 / 01-2017




                                                are displayed.




                 H-280                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                               Scheduling




                                           Sort result
                                           With the selection of the option, you specify how the display shall be sorted:
                                           • By item:
                                              The work types are listed per item.
                                           • By production date:
                                              The items are listed according to the date of the work type in question.

                                           Totals
                                           In this group, the totals for the times and costs are displayed, which were cal-
                                           culated for the scheduled order.


                                           Machine Selection in Case of Bottleneck
                                           Production > Capacity planning > Booking > Book order > Scheduling > (bot-
                                           tleneck)




                 Fig. H-185   Bottleneck during scheduling – Select machine


                                           On this dialog, you select another machine manually. The dialog is displayed
                                           automatically at scheduling if the default machine with the priority 9 is fully uti-
                                           lized.
                                            Tutorial, “Capacity Problems” on page H-114

                                           Capacity bottleneck

                                           Order, customer, shipping date Display of the order number, the customer
4.02 / 01-2017




                                           name, and the shipping date stated in the order.




                 A+W Business Pro Capacity Planning                                                                    H-281
                 Scheduling                                                              Software Reference




                              Item/element/sub-item Display of item number, level of the BOM and for
                              split items, the number of the sub-item where the capacity bottleneck occurs.

                              Quantity Quantity of the item or sub-item.

                              Product, dimensions Product name and dimensions of the order item.

                              Work type Work type for which the bottleneck occurs.

                              Production

                              Date Scheduled production date. With the arrow buttons, you can move the
                              date forward or backward.

                              Shift Scheduled shift. With the arrow buttons, you can move the shift forward
                              or backward on the same day. If you are working with just one shift, the date
                              is shifted.

                              Valid machines
                              In the overview, all machines are displayed which can also perform this work
                              type.
                              •   Machine:
                                  Alternate machines.
                              •   Time required:
                                  Time required for the process, for the item and quantity displayed.
                              •   Time reserved:
                                  Time that is already reserved for other orders on that machine.
                              •   Set-up time:
                                  Time that is required to set up the machine if the items displayed shall be
                                  produced.
                              •   Maximum time:
                                  Shift time of the machine on the selected date.

                              Buttons

                              [Overview] Opens the Order numbers dialog to check which orders are al-
                              ready scheduled on the machine for the current settings.
                               “Order Numbers” on page H-283

                              [Alignment] Currently not used.

                              [Split item] Opens the Split item dialog to split the item into sub-items.
                               “Split Items” on page H-284

                              [Criteria] Opens the Change criteria dialog.
                               “Change Criteria (Search Date)” on page H-272
4.02 / 01-2017




                              [Schedule] Schedules the item based on the set conditions. Depending on
                              the setting, you have to schedule each work type per item individually. If all
                              items are scheduled, a message with the changes is displayed.


                 H-282                                                A+W Business Pro Capacity Planning
                 Software Reference                                                                            Scheduling




                                        [Schedule previous day] Schedules the item based on the set conditions
                                        on the previous day. For this, you first have to select the last shift of the previ-
                                        ous day in the Shift field.


                                        Order Numbers
                                        Production > Capacity planning > Booking > Book order > Schedule machine
                                        in case of bottleneck > [Overview]




                                        Fig. H-186    Bottleneck during scheduling – Overview of the scheduled orders


                                        On this dialog, you check which orders are already scheduled on the machine
                                        at the set conditions.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-283
                 Scheduling                                                               Software Reference




                              Split Items
                              Production > Capacity planning > Booking > Book order > Scheduling > Ma-
                              chine selection in case of bottleneck > [Split items]




                              Fig. H-187   Bottleneck during scheduling – Split item


                              On this dialog, you split an order item into several sub-items.
                               Tutorial, “Capacity Problems” on page H-114

                              Item information

                              Order, item Order number and number and product name for the order item.

                              Product, quantity Product number and quantity of the order item.

                              Split
                              In this group, you specify how the item shall be split. The splitting of the item
                              into sub-items is displayed in the overview.
                              If you have ticked the Preset production date checkbox in the Options group,
                              in addition to the quantity, the date and shift are also displayed. You can enter
                              the requested values directly in these fields.

                              Quantity Specification of the quantity. Using the buttons below, you specify
                              whether the quantity shall be interpreted as shift or as quantity.

                              [Reset splitting] Resets the splitting of the item. Then you can try other pos-
4.02 / 01-2017




                              sibilities for splitting the item.




                 H-284                                                 A+W Business Pro Capacity Planning
                 Software Reference                                                                           Scheduling




                                        [Quantity = Shifts] The value in the Quantity field shall refer to shifts, e.g.
                                        2 shifts. The quantity of the item is split evenly across the number of shifts. In
                                        the overview, you can overwrite the values.

                                        [Quantity = units per shift] The value in the Quantity field shall refer to the
                                        units per shift, e.g. 50 units per shift.
                                        If you have not made any specifications about the quantity, as many sub-items
                                        are generated as the settings from the company data permit, e.g. 50% of the
                                        shift. In the overview, you can overwrite the values.
                                         “Fill shift in case of item splitting” on page H-180

                                        Options

                                        Maximum work types for preset date The field is only released if the Pre-
                                        set production date checkbox is ticked. The field must not be empty.
                                        You can specify production dates for the item split. In this case, you can also
                                        specify starting with which work type these dates shall not apply. This setting
                                        makes sense, e.g., because the sub-items are not packaged and shipped sep-
                                        arately.

                                        Reduced control Normally the scheduling checks for each item on which
                                        day there are still capacities available to schedule the item there.
                                        An order can however include items with the same BOM structure where only
                                        the sizes are different.
                                         The entire BOM structure is checked for each item.
                                         With the same BOM structure, the scheduling assumes the previous item
                                        without checking the BOM. This is the default setting.
                                        The program notes the start date of production of the first item, e.g. for the
                                        grinding machine. The next item starts precisely on this date in order to check
                                        the capacity for this machine and goes, if the machine is fully utilized on this
                                        day, to the previous shift or the previous day. The next item, in turn, relies on
                                        this new date for the checking of the capacity, etc.

                                        With locks When splitting, the remaining shift time for other orders can be
                                        locked, e.g. so that the machine does not have to be set up again.
                                         Remaining time of the shift or the day in question is not locked for other
                                        orders.
                                         Only sub-items created by splitting the order will be produced. The remain-
                                        ing time will not be scheduled otherwise.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-285
                 Scheduling                                                                 Software Reference




                              Preset production date You can specify a date per sub-item.
                               The date cannot be preset.
                               In the overview, the columns Date and Shift are displayed, and in the Op-
                              tions group the field Max. work type for preset date.

                              [OK] Applies the data. Scheduling is continued with the new sub-items.

                              [End] Interrupts the splitting. The Machine selection in case of bottleneck di-
                              alog is displayed again in the foreground.

                              [Overview] Opens the Item times dialog.
                               “Item Times” on page H-286



                              Item Times
                              Production > Capacity planning > Booking > Book order > Scheduling > Ma-
                              chine selection in case of bottleneck > [Split items] > [Overview]




                              Fig. H-188   Bottleneck during scheduling – Overview of the item split


                              On this dialog, you check the times that are required for the current item. The
                              times are displayed in red for which no capacities are available.
4.02 / 01-2017




                 H-286                                                 A+W Business Pro Capacity Planning
                 Software Reference                                                                          Scheduling




                                        Machine Failure
                                        Production > Capacity planning > Booking > Machine Failure
                                        Machines can be locked temporarily or completely. Scheduled orders have to
                                        be rescheduled in this case. The query regarding rescheduling appears when
                                        you lock a machine for which orders have already been scheduled. You should
                                        therefore set the search mode first.
                                         “Change Criteria (Search Date)” on page H-272
                                        This section provides information on the following subjects:
                                        •   “Functions Menu” on page H-287
                                        •   “Options Menu” on page H-288
                                        •   “Machine Failure (Dialog)” on page H-289


                                        Functions Menu
                                        Production > Capacity planning > Booking > Machine Failure
                                        Using this menu, you can open other dialogs without closing the Machine Fail-
                                        ure dialog.

                                        Date search group
                                        •   Change criteria:
                                            Opens the dialog by the same name on which you can specify the criteria
                                            for the date search.
                                             “Change Criteria (Search Date)” on page H-272

                                        Residual quantities group
                                        •   Transfer:
                                            Opens the Residual quantity transfer dialog on which you can specify up to
                                            which status orders shall be checked for residual quantities.
                                             “Residue Transfer” on page H-290

                                        Scheduling group
                                        •   Schedule selection:
                                            Opens the Schedule order dialog to reschedule the selected orders on oth-
                                            er machines.
                                             “Book Order” on page H-275

                                        Capacity planning group
                                        •   Shifts:
                                            Opens the Shift settings dialog on which you can specify the shift transition
                                            and closing times.
                                             “Shift Settings” on page H-183
                                            You must have administrator rights to open the dialog. In addition, the Use
4.02 / 01-2017




                                            change of shift table checkbox must be ticked on Company data dialog.
                                             “Use change of shifts table” on page H-182




                 A+W Business Pro Capacity Planning                                                               H-287
                 Scheduling                                                                Software Reference




                              Options Menu
                              Production > Capacity planning > Booking > Machine Failure
                              Using this menu, you can determine the default setting of the dialog. You can
                              activate or deactivate options. The settings will not be reset when you close
                              the dialog.

                              Dwell days group
                              •   Use old mode:
                                  This setting is only required if you want to retain the old mode for dwell days
                                  (= Transition matrix).

                              Set-up time group
                              •   Check:
                                  If the set-up time has been defined for several work types performed for an
                                  order item, this time shall be charged just once per item.

                              Scheduling group
                              •   Check item:
                                  When the order is scheduled, the program checks its share in the daily ca-
                                  pacity. The percentage is defined on the Work types dialog.
                                   “% Limit” on page H-189
                              •   Obey closing time:
                                  The program shall check until when orders can be scheduled for a shift.
                                   “Shift Settings” on page H-183
4.02 / 01-2017




                 H-288                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                        Scheduling




                                        Machine Failure (Dialog)
                                        Production > Capacity planning > Booking > Machine Failure




                                        Fig. H-189    Machine Failure


                                        On this dialog, you store downtimes for your machines, so that capacity plan-
                                        ning can consider this during the planning. Such downtimes arise, e.g. due to
                                        maintenance work or repairs.
                                         Tutorial, “Locks” on page H-90

                                        Selection

                                        Machine Selection of the machine to which the downtimes shall be as-
                                        signed. Downtimes are entered in days, not in shifts.

                                        Downtime from, to Period during which the machine is probably unavail-
                                        able. If you save the entered times, the affected orders are displayed in the
                                        overview. These orders can automatically scheduled for other machines. A
                                        query appears in which you can confirm or reject the rescheduling.

                                        Data
                                        In the overview, all machines are listed for which downtimes are defined.

                                        Affected orders
                                        In the overview, all orders are listed that are scheduled on the selected ma-
4.02 / 01-2017




                                        chine. The Hours column shows the time reserved for the order on the locked
                                        machine.



                 A+W Business Pro Capacity Planning                                                             H-289
                 Scheduling                                                              Software Reference




                              Residue Transfer
                              Production > Capacity planning > Booking > Book order > Functions menu >
                              Settings group > Residue transfer




                              Fig. H-190   Transfer of residual quantities


                              On this dialog, you specify the status up to which the workflow task searches
                              for non-produced residual quantities from the previous day. This includes only
                              orders and items which should have been produced the day before, but have
                              not been started yet.
                               Tutorial, “Remaining Quantities from Previous Day” on page H-139
4.02 / 01-2017




                 H-290                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                 Production Reports




                                        Production Reports
                                        The current production status can be included in capacity planning so that in
                                        addition to the order status, other lists can be drawn up, e.g. production lists
                                        and diagrams on the production status.
                                        If you are not working with reports from barcoding, on the dialogs for manual
                                        completion reporting at the various production stations, you can report batch-
                                        es, orders, or order items complete.
                                        On the dialogs, you can display all orders or only orders that have not been
                                        reported completed yet. You can enter completion reports or breakage reports.
                                        The rights to report completed can be limited by the administrator on special
                                        dialogs.
                                        This section provides information on the following subjects:
                                        •   “Date” on page H-292
                                        •   “Graphic” on page H-295
                                        •   “Batch” on page H-296
                                        •   “Settings for Batch Completion Report” on page H-297
                                        •   “Manual Completion Report” on page H-298
                                        •   “Settings for Manual Completion Reports” on page H-301
                                        •   “Production Lists” on page H-302
                                        •   “Settings for Production Lists” on page H-306
                                        •   “Production Level Orders” on page H-307
                                        •   “Report List” on page H-318
                                        •   “Change Production Times” on page H-319
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-291
                 Production Reports                                                                      Software Reference




                                           Date
                                           Production > Capacity planning > Completion reports > Date




                 Fig. H-191   Completion report by date


                                           On this dialog, you report the production of an order, order item or sub-item
                                           completed at a certain machine. Once the first element of an item has been
                                           reported completed, the corresponding process cannot be changed.
                                            Tutorial, “Report manually Order completed” on page H-143

                                           Functions menu
                                           Using this menu, you open a graphical display of the orders produced in the
                                           production area in question.
                                            “Graphic” on page H-295

                                           Selection

                                           Production date Date of production.

                                           Show items reported complete You can display per order which items
                                           were reported completed.
                                            Only the items are displayed that are not yet reported completed.
4.02 / 01-2017




                                            All items are displayed.




                 H-292                                                             A+W Business Pro Capacity Planning
                 Software Reference                                                                   Production Reports




                                        Production area You can limit the display to the machines of a particular
                                        production area.
                                         All production areas are displayed.
                                         Only the machines of the selected production area are displayed. The field
                                        for selection of the production area is released.

                                        Machines
                                        In the overview, all machines are displayed that correspond to the selection
                                        criteria.

                                        Details
                                        In this list, the totals reported for the quantities and times are displayed.
                                        •   Completed:
                                            Quantity produced on the current day.
                                        •   Pcs.
                                            Total pieces that are to be produced on this machine on this day.
                                        •   Time:
                                            Time (in hours) that is required to produce the total quantity on this ma-
                                            chine.
                                        •   Remaining time:
                                            Remaining time for the not yet produced quantities.

                                        By unit
                                        In the overview, all items are displayed that are produced on the machine on
                                        the selected date. You can report an item partially or entirely completed.
                                        •   Item:
                                            Item number from the order.
                                        •   BOM ID:
                                            BOM ident number, i.e. the BOM level.
                                        •   Sub item(s):
                                            Sub-items created at scheduling by the splitting of the item.
                                        •   Process:
                                            Work type.
                                        •   Product/Processing:
                                            Product name.
                                        •   Pcs.:
                                            Item quantity.
                                        •   Size:
                                            Dimensions of the item.
                                        •   Already completed:
                                            Quantity produced on the current day.
                                        •   Completion report:
                                            Entry of the quantity to be reported completed.
                                        •   Fixed:
4.02 / 01-2017




                                            As soon as the first piece of an item is reported the checkbox is ticked. The
                                            process cannot be changed any more.
                                            If you tick this checkbox (manually) while no completion report has been



                 A+W Business Pro Capacity Planning                                                                H-293
                 Production Reports                                                              Software Reference




                                          made yet, you will force the production of the item on the set date, on the
                                          defined machine.

                                      P.O. elements
                                      In the overview, all order items with purchased elements are displayed.
                                      •   Order, Item:
                                          Order and item number from the order.
                                      •   Element:
                                          If the purchased element is a processing, the component is displayed that
                                          will be processed.
                                      •   Article/processing:
                                          Product name of the purchased element.
                                      •   Pcs.
                                          P.O. quantity.
                                      •   Size:
                                          Dimensions of the item.
                                      •   Ordered for:
                                          Requested delivery date.
                                      •   Delivered quantity:
                                          Quantity already delivered.
                                      •   Required on, shift:
                                          These two columns show where and when the purchased elements will be
                                          needed.
4.02 / 01-2017




                 H-294                                                        A+W Business Pro Capacity Planning
                 Software Reference                                                                  Production Reports




                                        Graphic
                                        Production > Capacity planning > Completion reports > Date > Functions
                                        menu > Graphic




                                        Fig. H-192    Graphical display of the quantities produced


                                        This display presents the quantities of a production area, a machine or an or-
                                        der item in graphical form.
                                        •   Blue graphic:
                                            Quantities that have not yet been reported completed.
                                        •   Green graphic:
                                            Quantities that have been reported completed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-295
                 Production Reports                                                               Software Reference




                                      Batch
                                      Select Production > Capacity planning > Completion report > Batch




                                      Fig. H-193    Report batch completed


                                      On this dialog, you report a production batch completed manually if you are
                                      not working with the status reports from barcoding.

                                      Functions menu
                                      Using this menu, you open the Settings for batch completion report dialog to
                                      select the production area for the completion report.
                                       “Settings for Batch Completion Report” on page H-297

                                      Selection
                                      With the option, you specify the selection of the orders for the completion re-
                                      port:
                                      •   By batch number from, to:
                                          An entire batch is reported completed. With the selection of this option, the
                                          fields from and to are released, where you can enter a batch number of a
                                          range of batch numbers.
                                          The batch numbers are assigned in A+W Production.
                                      •   By number manager:
                                          The orders of a whole number manager are reported completed. With the
                                          selection of this option, the field for selecting the number manager is re-
4.02 / 01-2017




                                          leased.




                 H-296                                                         A+W Business Pro Capacity Planning
                 Software Reference                                                                    Production Reports




                                        Enter date By default, the current date is taken over for the completion re-
                                        port.
                                         The current date is taken over for the completion report.
                                         The field for the specification of the date is released. The batch is reported
                                        completed with the changed date.

                                        Production areas / machines
                                        In this field, the production areas or machines are displayed for which the
                                        batch is reported completed. The required areas or machines are selected in
                                        the Selection menu on the Settings for batch completion report dialog.
                                         “Settings for Batch Completion Report” on page H-297

                                        Table
                                        In the overview, all orders are listed that match the criteria in the Selection
                                        group.


                                        Settings for Batch Completion Report
                                        Select Production > Capacity planning > Completion report > Batch > Func-
                                        tions menu > Production areas/machines




                                        Fig. H-194    Select areas or machines for completion report


                                        On this dialog, you specify for which production area or which machines the
                                        batch is reported completed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-297
                 Production Reports                                                               Software Reference




                                      Completion report
                                      With the selection of the option, you specify to what the completion report ap-
                                      plies:
                                      •   Whole order:
                                          With this option, all items and thus the entire order is reported completed.
                                          For the completion report, the current date or the specified date is taken
                                          over.
                                      •   Selected production areas:
                                          With this option, the production areas are listed in the Selection field. You
                                          can select one or more entries. The selected production areas are dis-
                                          played on the Batch dialog. The batch numbers can be reported completed
                                          for the selected production areas.
                                      •   Selected machines:
                                          With this option, the machines are listed in the Selection field. You can
                                          mark one or more entries. The selected machines are displayed on the
                                          Batch dialog. The batch numbers can be reported complete for the select-
                                          ed machines.


                                      Manual Completion Report
                                      Select Production > Capacity planning > Completion report > Manually
                                      With this dialog, you can report individual orders or order items complete.
                                      This section provides information on the following subjects:
                                      •   “Functions Menu” on page H-298
                                      •   “Options Menu” on page H-299
                                      •   “Manually (Completion Report)” on page H-299


                                      Functions Menu
                                      Select Production > Capacity planning > Completion report > Manually
                                      Using this menu, you can open the dialog for the settings to limit completion
                                      reports to particular production areas.
                                       “Settings for Manual Completion Reports” on page H-301
4.02 / 01-2017




                 H-298                                                        A+W Business Pro Capacity Planning
                 Software Reference                                                                   Production Reports




                                        Options Menu
                                        Select Production > Capacity planning > Completion report > Manually
                                        Using this menu, you can determine the default setting of the dialog. You can
                                        activate or deactivate options. The settings will not be reset when you close
                                        the dialog. The following entries are displayed:
                                        •   Scanning:
                                            Enables the field for entering the barcode (next to the order number).
                                        •   Adjust prod. date:
                                            By default, the date of the completion report is entered as production date.
                                            You can specify another date, e.g. that of the previous day.


                                        Manually (Completion Report)
                                        Select Production > Capacity planning > Completion report > Manually




                                        Fig. H-195    Manual completion report


                                        On this dialog, you report orders partially or entirely completed. In addition to
                                        the completion reports, you can also record breakage reports. The dialog can
                                        be used by employees in production. The completion reports can be set here
                                        so that the employee can report completed only own production area and cer-
                                        tain machines.
                                         Tutorial, “Report manually Order completed” on page H-143

                                        Completion report

                                        Order You can enter the order number or record by scanner. The field for the
                                        barcode is released in the Options menu.

                                        From item, to item You can report an individual item or several items of an
                                        order.
                                        If you enter several items, only the whole items can be reported.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-299
                 Production Reports                                                               Software Reference




                                      Total qty. Display of the total quantity of processings for the items you have
                                      entered.

                                          Example                                           Cutting       Shipping

                                          Item 1: 12 x IG                                   24 pcs.        12 pcs.

                                          Item 2: 6 x single glass                            6 pcs.         6 pcs.

                                          Item 1 - 2:                                       30 pcs.        18 pcs.


                                      Quantity Quantity to be reported The field is released only if you have en-
                                      tered a single item number, e.g. 2.

                                      Item complete Scanning will report one unit completed for every scanned
                                      order item.
                                       Every item will be scanned until the required quantity is reached.
                                       The scanned item is reported completed as a whole.

                                      With quantity You can also report a partial quantity of the scanned item
                                      completed.
                                       One piece is reported completed for the scanned item.
                                       The quantity entered in Quantity field will be reported completed for the
                                      scanned item.

                                      [Report items completed (F9)] Only the selected items are reported com-
                                      pleted.

                                      [Report order completed (F12)] The entire order is reported completed.

                                      Preset date

                                      Enter date By default, the current date is taken over for the completion re-
                                      port. You can change the date.
                                       The present date will be used for the completion report.
                                       The fields for the date and the shift are released.

                                      Shift The field is released only if the Enter date checkbox is ticked. You can
                                      then enter the shift to which the report applies.

                                      Report type
                                      With the selection of the option, you specify the type of report:
                                      •   Completion report:
                                          The specified quantity is reported completed.
                                      •   Breakage report - entry:
                                          The specified quantities are reported as broken at the machine entry. They
                                          must be reproduced by the previous machine.
4.02 / 01-2017




                                      •   Breakage report - exit:
                                          The specified quantities are reported as broken at the machine exit. They
                                          must be reproduced by the same machine.



                 H-300                                                        A+W Business Pro Capacity Planning
                 Software Reference                                                                Production Reports




                                           Breakage report
                                           A breakage report can be entered only if the item has been reported com-
                                           pleted before.
                                           This means that a sheet which is damaged at the station where is has been
                                           processed can be reported broken only after the completion report has
                                           been issued.
                                           A sheet that arrives damaged at the station, has already been reported
                                           completed by the previous station and can therefore be reported broken
                                           right away

                                        Select machine In this field, the machines are displayed that are available
                                        in the selected production area. You have to mark one of the suggested ma-
                                        chines so that you can enter the report. The program will offer only the ma-
                                        chines that are eligible for the current user.
                                         “Settings for Manual Completion Reports” on page H-301



                                        Settings for Manual Completion Reports
                                        Production > Capacity planning > Completion report > Manually > Functions
                                        menu > Settings




                                        Fig. H-196    Machine selection for manual report


                                        On this dialog, you specify for which production area and which machines the
                                        production employee can record reports.

                                        Select machines

                                        Production area Selection of the production area in which the respective
                                        employee shall record reports. The program then lists all machines belonging
4.02 / 01-2017




                                        to the selected production area.
                                        You can choose only one production area at a time but you can choose as
                                        many of the listed machines as you like. You have to select at least one entry.


                 A+W Business Pro Capacity Planning                                                             H-301
                 Production Reports                                                                    Software Reference




                                            Scanner

                                            Separator Specification of the separator with which the barcodes are sepa-
                                            rated if several codes are scanned in succession. This specification must
                                            match the scanner setting. Please refer to the scanner's operating instructions
                                            for details.


                                            Production Lists
                                            Production > Capacity planning > Production lists




                 Fig. H-197   Production lists


                                            On this dialog, you can evaluate which quantity of which order must be pro-
                                            duced on a particular machine and when the order is required on which sub-
                                            sequent machine.

                                            Settings menu
                                            Using this menu, you can specify the sorting of the data for printing.
                                             “Settings for Production Lists” on page H-306

                                            Selection

                                            From date, to date Entry of the date or the time range for which you require
                                            the production papers.
4.02 / 01-2017




                                            Machine Selection of the machine for which the production papers shall be
                                            printed. For selection, only the machines are offered for which processes are
                                            scheduled on the selected date or in the selected period.


                 H-302                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                 Production Reports




                                        Print settings
                                        The checkboxes in this group are only released in selection mode.

                                        Reprint You can print the production papers several times on a day. You can
                                        also specify whether only the new data shall be printed, or all data.
                                         By default, only the new data will be printed, i.e. the data which have not
                                        been printed before.
                                         All data for that day – up to the present point in time – will be printed.

                                        Print for all machines You can specify whether the production papers shall
                                        be printed for a single machine or for all machines.
                                         The data will only be printed for the machine defined in field Machine.
                                         The data of all machines will be printed.

                                        Incl. information on origin You can also print the production area from
                                        which the item came.
                                        The checkbox is blocked if the output on the production papers is summarized
                                        by orders or items.
                                         The previous production area is not displayed.
                                         The previous production area is displayed.

                                        Orders summarized You can summarize the data by orders.
                                         The orders are printed individually.
                                         The data will be summarized per order. The checkbox for the items is au-
                                        tomatically ticked and cannot be deactivated. With this setting, no origin infor-
                                        mation can be printed.

                                        Items summarized You can summarize the data by order.
                                         For each order item, one line per machine is printed.
                                         The items of an order are summarized and printed in one line. With this set-
                                        ting, no origin information can be printed.

                                        Show set up times as well Set-up times can be displayed only if the have
                                        been defined as basic times and allocated appropriately.
                                         Setup times are not printed.
                                         The setup time is printed.

                                        Table
                                        In the overview, all data is displayed that match the selection criteria. Depend-
                                        ing on the settings in the Print settings group, the following columns are dis-
                                        played:
                                        •   Date:
                                            Production date.
                                        •   Shift:
                                            Shift in which the order or item was produced.
4.02 / 01-2017




                                        •   Order:
                                            Order number




                 A+W Business Pro Capacity Planning                                                              H-303
                 Production Reports                                                          Software Reference




                                      •   Priority:
                                          Priority from the order or from the scheduling.
                                      •   Status:
                                          Order status.
                                      •   Item:
                                          Number of the order item.
                                      •   Item status:
                                          Item status.
                                      •   Product:
                                          Product name.
                                      •   Glass size:
                                          Size of the item.
                                      •   Shape:
                                          Shape number.
                                      •   Element:
                                          Product name of the BOM component.
                                      •   Processing:
                                          Product name of the processing.
                                      •   Work type:
                                          Name of the work type
                                      •   Pcs:
                                          Number of pieces of the item.
                                      •   Quantity:
                                          Number of sheets.
                                      •   Sqm/pc:
                                          Area per piece.
                                      •   Lm/pc:
                                          Linear meters of the edges per piece.
                                      •   Next processing:
                                          Next processing (process).
                                      •   Following machine:
                                          Machine.
                                      •   Date:
                                          Production date on the current machine.
                                      •   Customer:
                                          Customer name from the order.
                                      •   BOM part:
                                          Number of the BOM component.
                                      •   Previous Machine, Previous work type, Production date:
                                          Data for the previous process.
4.02 / 01-2017




                 H-304                                                      A+W Business Pro Capacity Planning
                 Software Reference                                                                        Production Reports




                                             Production Lists – Print
                                             Production > Capacity planning > Production lists > Print menu > Printer




                 Fig. H-198   Production lists – Print


                                             In the printed lists, the order items are displayed with size, quantities, and next
                                             processings. The output is set with the checkboxes on the Production lists di-
                                             alog.
                                              “Print settings” on page H-303
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                     H-305
                 Production Reports                                                                         Software Reference




                                           Settings for Production Lists
                                           Production > Capacity planning > Production lists > Settings menu > Produc-
                                           tion lists




                                           Fig. H-199      Settings for production lists


                                           On this dialog, you select the criteria for sorting the production list.

                                           Production list

                                           PRLIST Variables (0,1,2) The PRLIST variable setting depends on the re-
                                           port definition. By default, the following settings are available for printing the
                                           report:
                                           • 0:
                                              If the product texts of main product and BOM product are identical, the text
                                              is only printed for item 1.
                                           • 1:
                                              If the product texts of main product and BOM product are identical, the text
                                              is only printed for item 2.
                                           • 2:
                                              Both texts, both the text for the main product and the text for the BOM prod-
                                              uct are printed on the list.


                    Example

                          Text main product = Float 4 mm                     Text main product = IG
                          Text BOM product = Float 4 mm                      Text BOM product = Float 4 mm

                     No. Text item 1             Text item 2                 Text item 1              Text item 2

                      0   Float 4 mm             -                           IG                       Float 4 mm

                      1   -                      Float 4 mm                  IG                       Float 4 mm
4.02 / 01-2017




                      2   Float 4 mm             Float 4 mm                  IG                       Float 4 mm




                 H-306                                                                     A+W Business Pro Capacity Planning
                 Software Reference                                                                    Production Reports




                                        Sorting by
                                        With the selection of the option, you specify how the data shall be sorted in the
                                        production papers.

                                        Status

                                        From, to Status or status area of orders to be printed.


                                        Production Level Orders
                                        Production > Capacity planning > Production level orders
                                        On this dialog, you can check and report completed individual machines, or-
                                        ders, and order items down to the BOM level.
                                        There are the following tabs on the Order dialog:
                                        •   “Production Level Order – Selection” on page H-310
                                        •   “Production Level Orders – Overview” on page H-311
                                        •   “Production Level Orders – Items” on page H-312
                                        •   “Production Level Orders – Detail” on page H-314
                                        •   “Production Level Orders – P.O. Elements” on page H-315
                                         Tutorial, “Check Production Status” on page H-148

                                        Navigation through the tabs and dialogs
                                        The following overview shows you how to display the data.

                                        Tab                 Action                            Tab / dialog

                                        Selection           Click on row header        ->     Items

                                        Items               Click on row header        ->     Detail
                                                                                              P.O.elements

                                        Detail              Click on row header        ->     Production level orders
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                     H-307
                 Production Reports                                                              Software Reference




                                      Functions Menu
                                      Production > Capacity planning > Production level orders > Functions menu
                                      Using this menu, you can open other dialogs without closing the Completion
                                      report order dialog.

                                      Document group
                                      •   Display:
                                          Opens the view of the document.
                                      •   History:
                                          Opens the History dialog on which you can check the course of the status
                                          changes.
                                           Sales, “History” on page C-478
                                      •   Status change:
                                          Opens the dialog by the same name on which you can changes the status
                                          of the order.
                                           Sales, “Status Change” on page C-479

                                      Reports group
                                      •   Overview:
                                          Opens the Reports dialog to check the status of the individual items.
                                           “Report List” on page H-318

                                      Capacity planning group
                                      •   Completion report by date:
                                          Opens the Date dialog to report the order completed.
                                           “Date” on page H-292
                                      •   Move:
                                          Opens the Change production times dialog to move the order.
                                           “Change Production Times” on page H-319
4.02 / 01-2017




                 H-308                                                       A+W Business Pro Capacity Planning
                 Software Reference                                                                 Production Reports




                                        Scheduling group
                                        •   Scheduling:
                                            Opens the Schedule order dialog to schedule the order.
                                             “Book Order” on page H-275
                                        •   Delete:
                                            Deletes the selected order from capacity planning. After that, the order can
                                            be rescheduled. The right to delete can be limited in the rights manage-
                                            ment.

                                        Status group
                                        •   Show graphics:
                                            Opens the graphical display of the completed and open work per item. The
                                            entry is only released on the Items tab.
                                             “Graphic” on page H-295

                                        Miscellaneous group
                                        •   Update purchase prices:
                                            Updates the purchase prices of the selected order.
                                             “Report List” on page H-318
                                        •   LG numbers:
                                            This entry is only released customer-specifically.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-309
                 Production Reports                                                                    Software Reference




                                            Production Level Order – Selection
                                            Production > Capacity planning > Production level orders > Selection tab




                 Fig. H-200   Production level orders – Selection


                                            On this tab, you select an order for one customer or several orders for the de-
                                            livery date. The orders found are listed in the Table group.

                                            Order, customer, date
                                            In this group, you set the selection criteria.

                                            Number With the entry of the order number the order data are displayed.

                                            Number With the entry of the customer number, all orders for the customer
                                            are displayed.

                                            Customer The customer name is displayed automatically.

                                            Delivery date With the entry of the delivery date, all orders with this date are
                                            displayed.
4.02 / 01-2017




                 H-310                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                    Production Reports




                                           Completion report

                                           Enter date If you want to report an order completed, you can specify the
                                           date.
                                            The current date is entered as completion report date.
                                            You can change the date. The order is reported completed with the
                                           changed date.

                                           Production date Display of the production date for the order that is selected
                                           on the overview.

                                           Result
                                           In the overview, all orders are displayed that correspond to the selection crite-
                                           ria.


                                           Production Level Orders – Overview
                                           Select Production > Capacity planning > Production level orders > Overview
                                           tab




                 Fig. H-201   Production level orders – Overview


                                           On this tab, you can view details on the calculation of the selected order.

                                           Production
4.02 / 01-2017




                                           Start, End Display of the respective dates for the order that is marked on the
                                           Selection tab.




                 A+W Business Pro Capacity Planning                                                                  H-311
                 Production Reports                                                                    Software Reference




                                            Quantity

                                            Pcs Total quantity of the order.

                                            Completed Quantity completed.

                                            Calculation

                                            Material cost Material cost from the order.

                                            Planned time costs Calculated time costs.

                                            Total costs planned Total of material cost and planned time costs.

                                            Order value Total order value.

                                            Actual time costs Actual time costs. This value is calculated based on the
                                            report from A+W Production.

                                            Actual total costs Total of material cost and actual time costs.


                                            Production Level Orders – Items
                                            Select Production > Capacity planning > Production level orders > Items tab




                 Fig. H-202   Production level orders – Items
4.02 / 01-2017




                                            On this tab, all items of a selected order are listed. You can report manually
                                            individual items completed.




                 H-312                                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                  Production Reports




                                        The fields are described on the Selection tab.
                                         “Production Level Order – Selection” on page H-310

                                        Table
                                        In the overview, all items per order are displayed.
                                        •   Item:
                                            Items of the selected order.
                                        •   Article:
                                            Name of the article that is included in this item.
                                        •   Date:
                                            Production date of the first process on the main product of the item.
                                        •   Pcs.:
                                            Item quantity.
                                        •   Size:
                                            Size of the item.
                                        •   Completed w/o processing:
                                            Display of the quantity for which the cutting has already been done, but not
                                            yet the processing, e.g. drilling.
                                            However, this statement is very imprecise because the glass is usually sub-
                                            jected to a multitude of processings. A precise statement of the state of pro-
                                            duction can therefore only be made with the reports from the registration
                                            points in production.
                                             “Report List” on page H-318
                                        •   Completely finished:
                                            Number of completely finished units of an item.
                                        •   Ordered:
                                            Display whether there are ordered articles.
                                        •   Completion report:
                                            Display whether the item was reported completed.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-313
                 Production Reports                                                                  Software Reference




                                            Production Level Orders – Detail
                                            Select Production > Capacity planning > Production level orders > Detail tab




                 Fig. H-203   Production level orders – Detail


                                            On this tab, the BOM components are displayed per item. The tab is released
                                            only if you have selected an order item with BOM on the Items tab.
                                            With a click of the header row, you open the Production status > Date dialog.
                                             “Date” on page H-292

                                            Table
                                            In the overview, all BOM components of the current item are displayed.
                                            •   Date:
                                                Production date.
                                            •   Shift:
                                                Shift in which the item shall be produced.
                                            •   BOM ID:
                                                BOM ident number, that is the BOM level.
                                            •   Product:
                                                Product name.
                                            •   Work type:
                                                Work type.
                                            •   Pcs.:
                                                Item quantity.
4.02 / 01-2017




                 H-314                                                             A+W Business Pro Capacity Planning
                 Software Reference                                                                     Production Reports




                                            •   Completed:
                                                Quantity that was reported completed.
                                            •   Machine:
                                                Machine on which the item is or was produced.


                                            Production Level Orders – P.O. Elements
                                            Select Production > Capacity planning > Production level orders > P.O. ele-
                                            ments tab




                 Fig. H-204   Production level orders – P.O. elements


                                            On this tab, the P.O. elements are displayed that are included in the items of
                                            the current order.
                                            With a click of the header row, you open the Schedule P.O. elements dialog
                                             “Scheduling of Purchased Elements” on page H-317

                                            Table
                                            In the overview, all items are listed that contain P.O. elements.
                                            •   Item:
                                                Item number from the order.
                                            •   Article
                                                Product name of the P.O. element.
                                            •   Pcs.:
                                                Quantity to be purchased.
4.02 / 01-2017




                                            •   Size:
                                                Dimensions of the item.



                 A+W Business Pro Capacity Planning                                                                H-315
                 Production Reports                                                            Software Reference




                                      •   Ordered for (date):
                                          Requested delivery date.
                                      •   Quantity delivered:
                                          Quantity already delivered.
                                      •   Required on, Date, Shift:
                                          These three columns display when the purchased elements are required
                                          where.


                                      Production Status – Graphic
                                      Select Production > Capacity planning > Production level orders > Items tab >
                                      Functions menu > Status group > Show graphics




                                      Fig. H-205   Production status of order items


                                      This display shows you the quantities of an order in graphical form.
4.02 / 01-2017




                 H-316                                                         A+W Business Pro Capacity Planning
                 Software Reference                                                              Production Reports




                                        Scheduling of Purchased Elements
                                        Select Production > Capacity planning > Production level orders > P.O. ele-
                                        ments tab > Click in row header




                                        Fig. H-206    Scheduling of purchased elements


                                        On this dialog, you schedule the purchased elements after the receipt of
                                        goods.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                           H-317
                 Production Reports                                                               Software Reference




                                      Report List
                                      Select Production > Capacity planning > Production level orders > Functions
                                      menu > Reports group > Overview




                                      Fig. H-207   Completion report order – Production reports


                                      On this dialog, you check which positions were reported completed on which
                                      machines.

                                      Order information

                                      Order Number of the order.

                                      Address Name and address of the customer.

                                      Status Status of the order.

                                      Production Start and end date of production.
4.02 / 01-2017




                 H-318                                                         A+W Business Pro Capacity Planning
                 Software Reference                                                                  Production Reports




                                        Order information
                                        For each order item, a column with the current reports is displayed. The report-
                                        ed figures are displayed in different colors:
                                        •   Black: 0 indicates that no pieces of the item have been produced.
                                        •   Green: the reported quantity corresponds to the item quantity.
                                        •   Blue: the reported quantity is only a partial quantity of the item.
                                        •   Red: the reported quantity must be ordered again, e.g. due to breakage.

                                        Item overview
                                        In this field, the BOM structure is displayed if you double-click in the Order in-
                                        formation group on the column heading of an item.


                                        Change Production Times
                                        Select Production > Capacity planning > Production level orders > Functions
                                        menu > Capacity planning group > Move
                                        You can change the dates and machines that were planned for an order.
                                        Thereby the capacities are not considered, however, so that you can move the
                                        process of an order item to a machine that is already fully utilized.
                                        This dialog contains the following tabs:
                                        •   “Change Production Times – Selection” on page H-320
                                        •   “Change Production Times – Overview” on page H-321
                                        •   “Change Production Times – Overview 2” on page H-323


                                        Plant Menu
                                        Select Production > Capacity planning > Production level orders > Functions
                                        menu > Capacity planning group > Move > Change production times > Plant
                                        menu
                                        Using this menu, you specify whether the capacity of an individual plant or all
                                        plants shall be considered.
                                        •   All:
                                            All defined production areas are displayed.
                                        •   Plant 1:
                                            Only the production areas with entry 0 and 1 are displayed.
                                        •   Plant 2:
                                            Only the production areas with entry 0 and 2 are displayed.
                                        •   Plant 3:
                                            Only the production areas with entry 0 and 3 are displayed.
                                        The plant refers to the key that is entered in the company data for a site.
                                        The sites are then assigned on the Production areas dialog.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-319
                 Production Reports                                                            Software Reference




                                      Change Production Times – Selection
                                      Select Production > Capacity planning > Production level orders > Functions
                                      menu > Capacity planning group > Move > Selection tab




                                      Fig. H-208   Change production times – Selection


                                      On this tab, the machines for a selected date are displayed.

                                      Selection

                                      Production date Selection of the date on which the order shall be produced.

                                      Machines by product area
                                      The following data is displayed in the overview:
                                      •   Production areas/Machines:
                                          All machines of the production area for which orders have been scheduled
                                          for the production date.
                                      •   Pcs.:
                                          Quantity to be produced by the corresponding machine.
                                      •   Hours:
                                          Utilization of the machine in hours.
                                      •   Set-up time:
                                          Set-up times can be scheduled in addition to the hours. Set-up times will
                                          be displayed only if they are allocated to the machine in question.
4.02 / 01-2017




                 H-320                                                        A+W Business Pro Capacity Planning
                 Software Reference                                                                 Production Reports




                                        Change Production Times – Overview
                                        Production > Capacity planning > Production level orders > Functions menu >
                                        Capacity planning > Move > Overview tab




                                        Fig. H-209    Change production times – Overview


                                        On this tab, all orders and/or items are displayed that shall be produced on the
                                        current machine on the production date. You can change the date, the shift,
                                        and the machine for an item or for an entire order.

                                        Order overview by machine

                                        Machine Current machine. In selection mode, any machine can be chosen.

                                        Suppress message Errors that occur during rescheduling for another date
                                        or another machine are displayed in a message.
                                         The message is displayed.
                                         Messages are not displayed.

                                        List
                                        In the overview, all orders are listed that shall be produced on the machine on
                                        the current day.
                                        •   Delivery date, Number, Customer:
                                            Delivery date, order number, and customer name from the order.
                                        •   Shift:
4.02 / 01-2017




                                            Shift in which the order in question shall be produced.
                                        •   Pcs.:
                                            Quantity to be produced.


                 A+W Business Pro Capacity Planning                                                              H-321
                 Production Reports                                                                Software Reference




                                      •   Move:
                                          Changes can be adopted only if this checkbox is ticked.
                                          If the changes clash with other processes for this order, an error message
                                          will indicate that this process cannot be moved.
                                      •   Hours:
                                          Hours scheduled for this order.

                                      Allocation of elements
                                      In the overview, all items of the selected order are listed that shall be produced
                                      on the machine on the current day.
                                      •   Shift:
                                          Shift in which the item shall be produced.
                                      •   Item:
                                          Item number from the order.
                                      •   BOM ID:
                                          BOM ident number, i.e. the BOM level.
                                      •   Sub item:
                                          Sub-items resulting from the splitting of items at scheduling.
                                      •   Process:
                                          Work type for the BOM item.
                                      •   Product/Processing:
                                          Product name.
                                      •   Pcs.:
                                          Item quantity.
                                      •   Size:
                                          Dimensions of the item.
                                      •   Move:
                                          Changes can be adopted only if this checkbox is ticked.
                                          If the changes clash with other processes for this order, an error message
                                          will indicate that this process cannot be moved.
                                      •   Hours:
                                          Hours planned for the order.

                                      Changed
                                      The changes in these fields apply to the order or the item, based on the selec-
                                      tion in the Move column.

                                      New date Production date to which the order shall be moved.

                                      Shift Shift to which the order shall be moved.

                                      New machine Selection of an alternative machine.
4.02 / 01-2017




                 H-322                                                         A+W Business Pro Capacity Planning
                 Software Reference                                                                Production Reports




                                        Change Production Times – Overview 2
                                        Production > Capacity planning > Production level orders > Functions menu >
                                        Time management group > Move > Overview 2 tab




                                        Fig. H-210    Change production times – Overview 2


                                        On this tab, detailed information per shift and machine is displayed.

                                        Work type overview by machine
                                        In the overview, all work types are listed that are scheduled on the machine on
                                        the current day.
                                        •   Number:
                                            ID of the work type.
                                        •   Process:
                                            Work type on the machine.
                                        •   Shift:
                                            Shift in which the work in question shall be performed.
                                        •   Quantity:
                                            Quantity to be produced.
                                        •   Move:
                                            Changes can be adopted only if this checkbox is ticked.
                                            If the changes clash with other processes for this order, an error message
                                            will indicate that this process cannot be moved.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-323
                 Production Reports                                                              Software Reference




                                      •   Hours:
                                          Utilization of the machine in hours.
                                      •   Setup time:
                                          Set-up times can be scheduled in addition to the hours. Set-up times will
                                          be displayed only if they are allocated to the machine in question.

                                      Order overview by work type/shift
                                      In the overview, all orders with the same work type per shift are listed:
                                      •   Order, Customer:
                                          Order number and customer name from the order.
                                      •   Item:
                                          Item number from the order.
                                      •   BOM ID:
                                          BOM ident number, i.e. the BOM level.
                                      •   Sub item:
                                          Sub-items created by splitting the item at scheduling.
                                      •   Product/Processing:
                                          Product name.
                                      •   Quantity:
                                          Quantity to be produced.
                                      •   Size:
                                          Dimensions of the item.
                                      •   Move:
                                          Changes can be adopted only if this checkbox is ticked.
                                          If the changes clash with other processes for this order, an error message
                                          will indicate that this process cannot be moved.
                                      •   Hours:
                                          Hours planned for the item.

                                      Changed
                                      The fields in the Changed group are described for the Overview tab.
                                       “Change Production Times – Overview” on page H-321
4.02 / 01-2017




                 H-324                                                        A+W Business Pro Capacity Planning
                 Software Reference                                                                    Control Station




                                        Control Station
                                        Production > Capacity planning > Control station
                                        On this dialog, you can check and correct the entire scheduling.
                                        This section provides information on the following subjects:
                                        •   “Control Station (Dialog)” on page H-326
                                        •   “Settings for Control Station” on page H-359
                                        •   “Control Station (Machine)” on page H-344
                                        •   “Utilisation (Date)” on page H-351
                                        •   “Utilisation – Print” on page H-358
                                        •   “Display Status” on page H-359
                                        •   “Settings for Control Station” on page H-359
                                        •   “Residue Qty.” on page H-361
                                        •   “Control Station (Order)” on page H-362
                                        •   “Moving impossible” on page H-375
                                        •   “Change Production Times” on page H-319
                                         Tutorial, “Control Station” on page H-161



                                        Functions Menu
                                        Production > Capacity planning > Control station
                                        Using this menu, you can open other dialogs without closing the control sta-
                                        tion.

                                        Additional displays group
                                        •   Select order:
                                            Opens the Control station (order) dialog on which you can edit the sched-
                                            uling of the order.
                                             “Control Station (Order)” on page H-362
                                        •   Display residual quantities:
                                            Opens the Residual quantities dialog to report these completed.
                                             “Residue Qty.” on page H-361
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-325
                 Control Station                                                                Software Reference




                                   Display group
                                   •   Graphic:
                                       Opens a graphical display to compare the produced and remaining quanti-
                                       ties.
                                        “Graphic” on page H-295
                                   •   Utilization:
                                       Opens the Utilization on date dialog. The entry is only released on the Ma-
                                       chines and Orders tab.
                                        “Utilisation (Date)” on page H-351

                                   Settings group
                                   •   Settings:
                                       Opens the Settings for control station dialog where you can define the data
                                       to be displayed by the control station.
                                        “Settings for Control Station” on page H-359
                                   •   No messages:
                                       After scheduling, a message with various information about the scheduling
                                       is suppressed.
                                       The entry is only released if you are logged in with administrator rights.


                                   Control Station (Dialog)
                                   Production > Capacity planning > Control station
                                   On this dialog, you check the utilization of the machines. On various tabs, you
                                   can reschedule manually entire orders or individual items.
                                   The Control station dialog contains the following tabs:
                                   •   “Control Station – Areas” on page H-328
                                   •   “Control Station – Machines” on page H-329
                                   •   “Control Station – Orders” on page H-330
                                   •   “Control Station – Reschedule Order” on page H-332
                                   •   “Control Station – Reschedule Item” on page H-334
                                   •   “Control Station – Work Types” on page H-336
                                   •   “Control Station – Details” on page H-338
                                   •   “Control Station – Shifts” on page H-340
                                   •   “Control Station – Prev. Processes” on page H-341
                                   •   “Control Station – Purchased Elements” on page H-343
                                    Tutorial, “Concept of the Control Station” on page H-162
4.02 / 01-2017




                 H-326                                                        A+W Business Pro Capacity Planning
                 Software Reference                                                                          Control Station




                                        Navigation through the tabs and dialogs
                                        The following overview shows you how to display the data.

                                        Tab                Action                             Tab / dialog

                                        Areas              Double-click on row           ->   Machines (all machines)
                                                           header
                                                           Double-click on production         Machines (only machines in
                                                           area                               the production area)

                                        Machines           Double-click on machine       ->   Orders
                                                           Double-click on detail data        Reschedule order
                                                           Double-click on row
                                                           header                             Control station (machine)

                                        Orders             Double-click on number        ->   Control station (order)
                                                           Double-click on detail data        Reschedule item

                                        Reschedule order   Click on row header           ->   Reschedule item
                                                           Click on [Elements] or        ->   Prev. processes
                                                           [Prev.processes]

                                        Reschedule item    Context menu for process ->        Delete setup time
                                                           (right mouse key)
                                                                                              Add setup time

                                        Work types         Click on row header           ->   Details

                                        Details            Double-click on number        ->   Control station (order)

                                        Prev. processes    Click on [In Detail]          ->   Production lists


                                        Period displayed
                                        When opening the dialog, the current and next week are displayed. With the
                                        navigation buttons, you can page forward and back across days or weeks.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                     H-327
                 Control Station                                                                        Software Reference




                                            Control Station – Areas
                                            Production > Capacity planning > Control station > Areas tab




                 Fig. H-211   Control station – Areas


                                            On this tab, you check the utilization of the production areas.

                                            Navigation through the tabs

                                            Action                                    Tab

                                            Double-click on row header          ->    Machines

                                            Double-click on production area     ->    Machines (only machines in the area)

                                            Buttons for navigation              ->    Page forward and back day by day


                                            Overview
                                            The following data is displayed in the overview:
                                            •   Production area:
                                                Production areas that are used in the period displayed.
                                            •   Day of the week, Date:
4.02 / 01-2017




                                                The planned day per day of the week (all shifts) is displayed.




                 H-328                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                          Control Station




                                           Control Station – Machines
                                           Production > Capacity planning > Control station > Machines tab




                 Fig. H-212   Control station – Machines


                                           On this tab, you check the utilization of per machine.

                                           Navigation through the tabs and dialogs

                                           Action                              Tab / dialog

                                           Double-click on machine        ->   Orders

                                           Double-click on details        ->   Reschedule order

                                           Double-click on row header     ->   Control station (machine) dialog


                                           Overview
                                           The following data is displayed in the overview:
                                           •   Machine:
                                               Machines of the production area. If you have changed to the Machines tab
                                               from the Areas tab with a double-click, only the machines are displayed that
4.02 / 01-2017




                                               belong to the appropriate production area.




                 A+W Business Pro Capacity Planning                                                                  H-329
                 Control Station                                                                         Software Reference




                                            •   Day of the week, Date:
                                                The utilization with the following totals of all shifts per machine can be dis-
                                                played per day of the week:
                                                – Scheduled and free time (all shifts)
                                                – Open and produced quantity of all sheets in pcs.
                                                – Total surface in sqm
                                                – Edge length of all sheets
                                                – Utilization in percent
                                            All details except for the time can be selected or deselected in the control sta-
                                            tion settings.
                                             “Settings for Control Station” on page H-359


                                            Control Station – Orders
                                            Production > Capacity planning > Control station > Orders tab




                 Fig. H-213   Control station – Orders


                                            On this tab, you check the utilization of the machines per order.
4.02 / 01-2017




                 H-330                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                        Navigation through the tabs and dialogs

                                        Action                          Tab / dialog

                                        Double-click on number     ->   Control station (order) dialog

                                        Double-click on quantity   ->   Reschedule item


                                        Overview
                                        The following data is displayed in the overview:
                                        •   Order, Status, Customer:
                                            Order number, status, and name of the customer from the order.
                                        •   Day of the week, Date:
                                            The utilization with the following details per day of the week is displayed:
                                            – Scheduled and free time (all shifts)
                                            – Open and produced quantity of all sheets in pcs.
                                            – Total surface in sqm
                                            – Edge length of all sheets
                                            – Percentage of the utilization, e.g. 29 % means that this order has a
                                               share 29% in the available 100 % utilization.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-331
                 Control Station                                                                        Software Reference




                                           Control Station – Reschedule Order
                                           Production > Capacity planning > Control station > Machines tab > Double-
                                           click on machine > Reschedule order tab




                 Fig. H-214   Control station – Reschedule order


                                           On this tab, you move an order on the machine in question, e.g. to another
                                           date, another shift or another machine.

                                           Navigation through the tabs

                                           Action                          Tab

                                           Click on row header       ->    Reschedule item

                                           Click on [Elements]        ->   Prev. processes - Elements

                                           Click on [Prev. processes] ->   Prev. processes


                                           [Elements] Changes to the display of the items on the Prev. processes tab.

                                           [Prev. processes] Changes to the display of previous processes on the Prev.
                                           processes tab.
4.02 / 01-2017




                 H-332                                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                        Overview
                                        The following data is displayed in the overview:
                                        •   Delivery date:
                                            Delivery date from the order.
                                        •   Order, Status, Customer:
                                            Order number, status, and name of the customer stated in the order.
                                        •   Shift:
                                            Currently-scheduled shift.
                                        •   Pcs.:
                                            Quantity of the sheets or processings.
                                        •   Finished:
                                            Number of sheets produced.
                                        •   Move:
                                            Changes can be adopted only if this checkbox is ticked.
                                            If the changes clash with other processes for this order, an error message
                                            will indicate that this process cannot be moved.
                                        •   Hours:
                                            Time reserved for this order.

                                        Move

                                        New date Production date to which the order shall be moved.

                                        Shift Shift to which the order shall be moved.

                                        Machine Machine to which the order shall be moved. The field is released if
                                        you have ticked the Move checkbox on the Start > Execute menu.

                                        [Load] Checks the utilization of the new machine. The value is displayed in
                                        hours. It includes the times for the order you have selected by clicking on the
                                        row header.

                                        Without check You can force the moving of an order or an order item.
                                         Before moving, there is a check whether there are sufficient free capacities
                                        on the new date, on the new machine, and/or for the new shift. If the capacities
                                        are not sufficient, a message indicates that the moving is impossible. You will
                                        have to move the order elsewhere in that case.
                                         The move is accepted without a check even if this exceeds the capacity.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-333
                 Control Station                                                                      Software Reference




                                           Control Station – Reschedule Item
                                           Production > Capacity planning > Control station > Machines tab > Double-
                                           click on detail data > Reschedule item tab




                 Fig. H-215   Control station – Reschedule item


                                           On this tab, you can move an order item to another date, another shift or an-
                                           other machine. The Process column displays the work type.

                                               Edit set-up times
                                               Use the context menu for a process (right mouse-button) to add or delete
                                               set-up times.

                                           [Product] For long lists, you can highlight all entries in the display that con-
                                           tain a particular product.
                                           Tick the line that includes the required product. When you click on this button,
                                           all lines that include the same product will be selected.

                                           [All], [None] You can use these buttons to tick or untick all checkboxes the
                                           Move column.
4.02 / 01-2017




                 H-334                                                             A+W Business Pro Capacity Planning
                 Software Reference                                                                    Control Station




                                        Overview
                                        The following data is displayed in the overview:
                                        •   Shift:
                                            Shift in which the item shall be produced.
                                        •   Item:
                                            Item number from the order.
                                        •   BOM ID:
                                            BOM ident number, that is the BOM level.
                                        •   SI:
                                            Sub-items resulting from the splitting of items at scheduling.
                                        •   Process:
                                            Work type.
                                        •   Product/Processing:
                                            Product name.
                                        •   Pcs.:
                                            Item quantity.
                                        •   Finished:
                                            Quantity of sheets produced.
                                        •   Size:
                                            Dimensions of the item.
                                        •   Move:
                                            Changes can be adopted only if this checkbox is ticked.
                                            If the changes clash with other processes for this order, an error message
                                            will indicate that this process cannot be moved.
                                        •   Hours:
                                            Time reserved for this item.

                                        Move
                                        The fields in this group are described for the Reschedule order tab.
                                         “Control Station – Reschedule Order” on page H-332
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-335
                 Control Station                                                                     Software Reference




                                            Control Station – Work Types
                                            Production > Capacity planning > Control station > Work types tab




                 Fig. H-216   Control station – Work types


                                            On this tab, you check which work types are to be performed on a machine on
                                            a production date.
                                            The tab is only filled if you have displayed elements or previous processes.

                                            Navigation through the tabs

                                            Action                        Tab

                                            Click on row header      ->   Details


                                            [Elements] Changes to the display of the items on the Prev. processes tab.

                                            [Prev. processes] Changes to the display of previous processes on the Prev.
                                            processes tab.
4.02 / 01-2017




                 H-336                                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                    Control Station




                                        Overview
                                        The following data is displayed in the overview:
                                        • Number:
                                          Number of the work type.
                                        • Process:
                                          Name of the work type.
                                        • Articles:
                                          Name of the product.
                                        • Shift:
                                          Shift in which this work type shall be performed.
                                        • Pcs.:
                                          Item quantity.
                                        • Move:
                                          Changes can be adopted only if this checkbox is ticked.
                                          If the changes clash with other processes for this order, an error message
                                          will indicate that this process cannot be moved.
                                        • Hours:
                                          Time reserved for this item.

                                        Move
                                        The fields in this group are described for the Reschedule order tab.
                                         “Control Station – Reschedule Order” on page H-332
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-337
                 Control Station                                                                             Software Reference




                                            Control Station – Details
                                            Production > Capacity planning > Control station > Prev. processes tab > Click
                                            in row header > Details tab




                 Fig. H-217   Control station – Details


                                            On this tab, detailed information per shift and work type is displayed.

                                            Navigation

                                            Action                          Dialog

                                            Double-click on order      ->   Control station (order) dialog
                                            number
4.02 / 01-2017




                 H-338                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                    Control Station




                                        Overview
                                        The following data is displayed in the overview:
                                        •   Order, Customer:
                                            Order number and customer name from the order.
                                        •   Item:
                                            Item number from the order.
                                        •   BOM ID:
                                            BOM ident number, i.e. the BOM level.
                                        •   SI:
                                            Sub-items resulting from the splitting of items at scheduling.
                                        •   Product/Processing:
                                            Product name.
                                        •   Pcs.:
                                            Item quantity.
                                        •   Size:
                                            Dimensions of the item.
                                        •   Move:
                                            Changes can be adopted only if this checkbox is ticked.
                                            If the changes clash with other processes for this order, an error message
                                            will indicate that this process cannot be moved.
                                        •   Hours:
                                            Time reserved for this item.

                                        Move
                                        The fields in this group are described for the Reschedule order tab.
                                         “Control Station – Reschedule Order” on page H-332
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-339
                 Control Station                                                                      Software Reference




                                             Control Station – Shifts
                                             Production > Capacity planning > Control station > Shifts tab




                 Fig. H-218   Control station – Shifts


                                             On this tab, you the machine utilization per shift.

                                             Overview
                                             The following data is displayed in the overview:
                                             •   Machine:
                                                 Machine.
                                             •   Shift:
                                                 One line is displayed per shift.
                                             •   Day of the week, date:
                                                 Scheduled time and shift time in hours, per shift.
4.02 / 01-2017




                 H-340                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                        Control Station




                                            Control Station – Prev. Processes
                                            Production > Capacity planning > Control station > Reschedule order tab >
                                            [Elements], [Prev. processes] > Prev. processes tab




                 Fig. H-219   Control station – Prev.processes


                                            On this tab, you check from which production area the items come, for which
                                            the current data are displayed. You can display the data in the Elements and
                                            Prev. processes modes.

                                            Navigation

                                            Action                        Dialog

                                            Click on row header      ->   Order column is displayed


                                            [In detail] Opens the Production list dialog to check for which orders the pre-
                                            vious machines are utilized.
                                             “Production Lists” on page H-302

                                            [Elements] Changes to display of the items.
4.02 / 01-2017




                                            [Prev. processes] Changes to display of the previous processes




                 A+W Business Pro Capacity Planning                                                                 H-341
                 Control Station                                                              Software Reference




                                   Selection
                                   This group displays the number and area of the elements in total and per shift.

                                   Options
                                   In Prev. processes mode, you can display additional information.
                                   •   With name:
                                       In the Elements column, the product name is displayed.
                                   •   With work type:
                                       In the Prev. work type column, the work type is shown that was performed
                                       previously.
                                   •   By areas:
                                       If there are several machines available for the previous processes, the dis-
                                       play in the Comes from column can be toggled between production area
                                       and machine.
                                   •   With order items:
                                       The order items are also displayed.
                                    The additional information is not displayed.
                                    The additional information is shown in the overview in an additional column.
                                   The selection must be confirmed on the Start > Execute menu to update the
                                   display.

                                   Overview (Elements / Previous processes)
                                   By default, the following columns are displayed in the overview:
                                   •   Work type:
                                       Name of the work type in the production area.
                                   •   Order:
                                       The order number is displayed if you click on the row header.
                                   •   Customer:
                                       The customer name is displayed if you click on the row header in Elements
                                       mode.
                                   •   Quantity:
                                       Number of sheets in the shift.
                                   •   Element:
                                       Product name (Elements mode).
                                   •   Article no.:
                                       Product number (Elements mode).
                                   •   Sqm:
                                       Total area in the shift (Prev. processes mode).
                                   •   Comes from:
                                       Previous production area (Prev. processes mode).
4.02 / 01-2017




                 H-342                                                     A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                           Control Station – Purchased Elements
                                           Production > Capacity planning > Control station > Purchased elements tab




                 Fig. H-220   Control station – Purchased elements


                                           On this tab, you check which orders (purchased articles) are included in the
                                           items.

                                           Overview
                                           The following data is displayed in the overview:
                                           •   Order, item:
                                               Order and item number from the order.
                                           •   Element:
                                               Number of the BOM level.
                                           •   (Blank column):
                                               Series, currently not used.
                                           •   Article/processing:
                                               Product name of the purchased element.
                                           •   Quantity:
                                               Quantity that must be purchased.
4.02 / 01-2017




                                           •   Size:
                                               Dimensions of the item.




                 A+W Business Pro Capacity Planning                                                              H-343
                 Control Station                                                               Software Reference




                                   •   Ordered to:
                                       Delivery date requested by the supplier.
                                   •   Deliv.:
                                       Quantity delivered.
                                   •   Shift:
                                       Shift in which the item is required.


                                   Control Station (Machine)
                                   Production > Capacity planning > Control station > Machines tab > Double-
                                   click on row header
                                   On this dialog, you check the machine utilization per shift.
                                   The Control station (machine) dialog contains the following tabs:
                                   •   “Control Station (Machine) – Shift” on page H-346
                                   •   “Control Station (Machine) – Load” on page H-348
                                   •   “Control Station (Machine) – Move II” on page H-350
                                    Tutorial, “Control Station – Machine” on page H-165


                                   Functions Menu
                                   Production > Capacity planning > Control station > Machines tab > Double-
                                   click on row header > Control station (machine) > Functions menu
                                   Using this menu, you can open other dialogs without closing the control sta-
                                   tion.

                                   Fill shift group
                                   •   Backwards:
                                       Recalculates the shifts. The quantities are moved to one of the previous
                                       shifts if possible.
                                   •   Forwards:
                                       Recalculate the shifts. The quantities are moved to one of the next shifts if
                                       possible.
4.02 / 01-2017




                 H-344                                                      A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                        Compress group
                                        You can have the machine utilization recalculated. This way you can fill gaps
                                        which occurred due to the settings regarding the proportional utilisation when
                                        an item was split or if e.g. an order was cancelled so that there is more free
                                        capacity.
                                        •   Backwards:
                                            Recalculates the utilization, starting backwards from the displayed date.
                                        •   Forwards:
                                            Recalculates the utilization, starting forward from the displayed date.
                                         “Fill shift in case of item splitting” on page H-180
                                         “Split Items” on page H-284

                                        Graphic group
                                        •   Graphic:
                                            Opens a graphical daily overview of the production area.
                                             “Graphic” on page H-295


                                        Options Menu
                                        Production > Capacity planning > Control station > Machines tab > Double-
                                        click on row header > Control station (machine) > Functions menu
                                        Using this menu, you can determine the default setting of the dialog. You can
                                        activate or deactivate options. The settings will not be reset when you close
                                        the dialog.
                                        The description of the following entries reflects the activated state:
                                        •   Move setup time:
                                            Enables the possibility to move the set-up times.
                                        •   Suppress messages:
                                            Errors that occur during rescheduling for another date or another machine
                                            are displayed in a message. You can suppress these messages.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-345
                 Control Station                                                                         Software Reference




                                            Control Station (Machine) – Shift
                                            Production > Capacity planning > Control station > Machines tab > Double-
                                            click on row header > Control station (machine) > Move I




                 Fig. H-221   Control station (machine) – Shift


                                            On this tab, you check which orders and quantities have to be produced per
                                            shift by this machine.

                                            Navigation through the tabs

                                            Action                                    Dialog

                                            Double-click on order number        ->    Control station (order)


                                            Overview
                                            The quantities for the selected machine are displayed in the overview.
                                            •   Date:
                                                Production date.
                                            •   Shift:
                                                Shift in which the orders are produced.
4.02 / 01-2017




                                            •   Order:
                                                Order number



                 H-346                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                     Control Station




                                        •   Pcs.:
                                            Pieces of the order on the current machine.
                                        •   Finished:
                                            Quantity of glass produced.
                                        •   Move:
                                            Changes can be adopted only if this checkbox is ticked.
                                            If the changes clash with other processes for this order, an error message
                                            will indicate that this process cannot be moved.
                                        •   Hours:
                                            Time scheduled for the quantity.

                                        Move

                                        New date Production date to which the order shall be moved.

                                        Shift Shift to which the order shall be moved.

                                        Machine Machine to which the order shall be moved.

                                        [Load] Checks the utilization of the new machine. The utilisation is shown in
                                        hours. It includes the times for the order you have selected by clicking on the
                                        row header.

                                        [Roll back] Sets the move back to the original values.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-347
                 Control Station                                                                     Software Reference




                                           Control Station (Machine) – Load
                                           Production > Capacity planning > Control station > Machines tab > Double-
                                           click on row header > Control station (machine) > Load




                 Fig. H-222   Control station (machine) – Load


                                           On this tab, all items are displayed that shall be produced in the selected pe-
                                           riod.
                                            Tutorial, “Control Station – Machine” on page H-165

                                           Selection

                                           From date, to date Entry of the period to be checked.

                                           Machine Selection of the machine for which you want to check the utilization.
4.02 / 01-2017




                 H-348                                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                        Overview
                                        In the overview, all order items are listed that must be produced in the selected
                                        period.
                                        •   Date:
                                            Production date.
                                        •   Shift:
                                            Shift in which the item shall be produced.
                                        •   Order, item:
                                            Order and item number stated in the order.
                                        •   Product:
                                            Product name.
                                        •   Glass size:
                                            Size of the item.
                                        •   Element:
                                            Product name of the BOM component.
                                        •   Work type:
                                            Work type in the production area.
                                        •   Pcs:
                                            Number of pieces of the item.
                                        •   Time:
                                            Scheduled time
                                        •   Customer:
                                            Customer name from the order.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                               H-349
                 Control Station                                                                          Software Reference




                                            Control Station (Machine) – Move II
                                            Production > Capacity planning > Control station > Machines tab > Double-
                                            click on row header > Control station (machine) > Move II




                 Fig. H-223   Control station (machine) – Move II


                                            On this tab, all shifts are displayed in the selected period. Colored fields indi-
                                            cate a scheduling problem.

                                            Overview
                                            In the overview, all shifts for the selected period are listed.
                                            •   Date:
                                                Production date.
                                            •   Shift:
                                                Shift in which the pieces are produced.
                                            •   Hours:
                                                Time required. If there are scheduling problems, the field is red.

                                            Move
                                            The fields in this group are described for the Move I tab.
4.02 / 01-2017




                                             “Control Station (Machine) – Shift” on page H-346




                 H-350                                                                A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                        Utilisation (Date)
                                        Production > Capacity planning > Control station > Machines tab > Functions
                                        menu > Display group > Utilisation
                                        On this dialog, you display an overview of the quantities to be produced for a
                                        specified time period. The overview can optionally be output by production ar-
                                        eas, machines or machine types.
                                        The data is displayed if you have started the filtering in the Start > Execute
                                        menu.
                                        This section provides information on the following subjects:
                                        •   “Plant Menu” on page H-352
                                        •   “Display Menu” on page H-352
                                        •   “Utilisation on (Date) (Display Period)” on page H-353
                                        •   “Utilisation on (Date) – Selection” on page H-355
                                        •   “Utilisation on (Date) – Details” on page H-356
                                        •   “Utilisation – Graphic” on page H-357
                                        •   “Utilisation – Print” on page H-358
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-351
                 Control Station                                                              Software Reference




                                   Plant Menu
                                   Production > Capacity planning > Control station > Machines tab > Functions
                                   menu > Display group > Utilisation
                                   Using this menu, you specify whether the capacity of an individual plant or all
                                   plants shall be considered.
                                   •   All:
                                       All defined production areas are displayed.
                                   •   Plant 1:
                                       Only the production areas with entry 0 and 1 are displayed.
                                   •   Plant 2:
                                       Only the production areas with entry 0 and 2 are displayed.
                                   •   Plant 3:
                                       Only the production areas with entry 0 and 3 are displayed.
                                   The plant refers to the code entered in the client's company data.
                                   Clients can be allocated in the Production areas dialog.


                                   Display Menu
                                   Production > Capacity planning > Control station > Machines tab > Functions
                                   menu > Display group > Utilisation
                                   Using this menu, you can specify the order status up to which the orders shall
                                   be displayed.
                                    “Display Status” on page H-359
4.02 / 01-2017




                 H-352                                                    A+W Business Pro Capacity Planning
                 Software Reference                                                                         Control Station




                                        Utilisation on (Date) (Display Period)
                                        Production > Capacity planning > Control station > Machines tab > Functions
                                        menu > Display group > Utilisation




                                        Fig. H-224    Utilisation on (date) – Select period


                                        On this dialog, you specify the criteria for the display of the utilization. You can
                                        display the result as a graphic or as a list.
                                         “Utilisation – Graphic” on page H-357
                                         “Utilisation – Print” on page H-358

                                        Evaluation period

                                        From, to Period for which you would like to have an overview.

                                        Options

                                        Show turnover This checkbox is released only if you have selected the Ma-
                                        chine option in the Overview of group.
                                         The turnover will not be displayed.
                                         The turnover will be displayed for the selected machine.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                  H-353
                 Control Station                                                               Software Reference




                                   Overview of
                                   With the selection of the option, you filter the display.
                                   •   Production area:
                                       You can limit the overview to a particular production area (<n.e.> = all).
                                   •   Machine types:
                                       You can limit the overview to a particular machine type.
                                   •   Machine:
                                       You can limit the overview to a particular machine. With this option, you can
                                       release the Show turnover checkbox.
                                   •   All machines by production area:
                                       With this option, all machines are sorted by production areas.

                                   Overview
                                   The following data is displayed in the overview:
                                   •   Date, Production areas/machines:
                                       The utilization is displayed per date and production area or machine.
                                   •   Pcs.
                                       Total quantity.
                                   •   Area:
                                       Total area.
                                   •   Circumference:
                                       Total edge length.
                                   •   Time:
                                       Scheduled time.
                                   •   Costs:
                                       Time costs.
                                   •   Turnover:
                                       Turnover per machine. This column is displayed only if you have selected
                                       the Machine option and ticked the Show turnover checkbox.
4.02 / 01-2017




                 H-354                                                      A+W Business Pro Capacity Planning
                 Software Reference                                                                          Control Station




                                        Utilisation on (Date) – Selection
                                        Production > Capacity planning > Control station > Machines tab > Functions
                                        menu > Display group > Utilisation > Display evaluation period > Click in row
                                        header




                                        Fig. H-225    Utilization on date – Select production area/machine


                                        On this dialog, you check the utilization in a particular period.

                                        Evaluation date

                                        From, to Period for which you would like to have an overview.

                                        Only shift Specification of the shift whose utilization shall be displayed. The
                                        field is only released in selection mode.

                                        Shift info The checkbox is only released in selection mode.
                                         The selection is not limited to particular shifts. After filtering, all shifts are
                                        displayed in the overview.
                                         The selection is limited to the shift that is specified in the Only shift field.

                                        Overview
                                        With the selection of the option, you specify the filtering of the display:
                                        •   All machines:
                                            The utilization of all machines in the set period is displayed.
4.02 / 01-2017




                                        •   Only for production area:
                                            The utilization for a particular production area is displayed.
                                            The field for selection of the production area is released.



                 A+W Business Pro Capacity Planning                                                                   H-355
                 Control Station                                                                  Software Reference




                                   Arrange detailed view With the selection of the option, you specify the
                                   grouping on the Details tab. The fields are released only if data is displayed.
                                   • Order, customer:
                                      The utilization is displayed per order and customer.
                                   • Product:
                                      The utilization is displayed per product.

                                   Utilization
                                   The hit list is displayed in the overview.


                                   Utilisation on (Date) – Details
                                   Production > Capacity planning > Control station > Machines tab > Functions
                                   menu > Display group > Utilisation > Display evaluation period > Click in row
                                   header > Details tab




                                   Fig. H-226    Utilization on date – Details on production area/machine


                                   On this dialog, you check the details of the utilization.

                                   Navigation through the tabs

                                   Action                                       Dialog

                                   Click on row header                    ->    Production level orders


                                   Details
4.02 / 01-2017




                                   The display of the columns and data is oriented according to the selection cri-
                                   teria. The lists are grouped by the option that is chosen on the Selection tab.



                 H-356                                                         A+W Business Pro Capacity Planning
                 Software Reference                                                                        Control Station




                                        Production area Display of the production area in which the machines are
                                        or where the work will be performed.

                                        Number manager Selection of the number manager in which the orders dis-
                                        played shall be placed.

                                        [Fill NM] Places all displayed orders in the specified number manager.


                                        Utilisation – Graphic
                                        Production > Capacity planning > Control station > Machines tab > Functions
                                        menu > Display group > Utilisation > Display evaluation period > Functions
                                        menu > Display group > Graphic




                                        Fig. H-227    Utilisation on date – Graphic


                                        The graphical display shows the utilization based on the criteria selected on
                                        the Utilisation (date) dialog.
                                        You can print the result from the Utilisation (date) dialog. The period to be print-
                                        ed can be limited to 8 or 12 days.
                                         “Utilisation – Print” on page H-358
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                 H-357
                 Control Station                                                               Software Reference




                                   Utilisation – Print
                                   Production > Capacity planning > Control station > Machines tab > Functions
                                   menu > Display group > Utilisation > Display evaluation period > Print menu




                                   Fig. H-228   Print


                                   You can print the result shown in the Utilisation at a date dialog. The period to
                                   be printed can be limited to 8 or 12 days. With 12 days, make sure to print the
                                   list in landscape format.
                                   The display shows a daily overview of the units to be produced per machine
                                   and production area. The nominal value is shown as well.
4.02 / 01-2017




                 H-358                                                     A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                        Display Status
                                        Production > Capacity planning > Control station > Machines tab > Functions
                                        menu > Display group > Utilisation > Display menu > Status display




                                        Fig. H-229    Specify display status


                                        On this dialog, you limit the display of the orders to a maximum status. Dis-
                                        played are only the orders whose status is smaller than the status entered.


                                        Settings for Control Station
                                        Production > Capacity planning > Completion report > Functions menu > Set-
                                        tings




                                        Fig. H-230    Settings for the control station


                                        On this dialog, you specify which data shall be displayed in the Control station
                                        dialog.
                                        You must confirm the changed settings with [OK]. The Control station dialog
                                        must be re-opened o that the data can be reloaded.

                                        Only these production areas
4.02 / 01-2017




                                        You can restrict the display to a certain production area or several production
                                        areas. If no entry has been selected, all production areas will be displayed.



                 A+W Business Pro Capacity Planning                                                              H-359
                 Control Station                                                               Software Reference




                                   Selection criteria
                                   You can set that only the items not produced are displayed:
                                   •   All entries:
                                       With this setting, the produced and open items are displayed.
                                   •   Only show entries which were not reported completed:
                                       With this setting, only items are displayed that still have to be produced.

                                   Order area You can limit the display to a particular order area.

                                   From status, to status You can limit the display by order status. If you select
                                   the same status in both fields, only orders with this one status will be dis-
                                   played.

                                   Display in addition to times
                                   By default, only the hours available on the day per machine are displayed. You
                                   can expand these details to include the following details:
                                   • Pcs.:
                                     Quantities for all shifts and orders.
                                   • Sqm:
                                     Total area for all shifts and orders.
                                   • Linear m:
                                     Total edge length for all shifts and orders.
                                   • In %:
                                     Percentage utilization for all shifts.
                                    The information is not displayed.
                                    The information is displayed on the Machines and Orders tabs.
4.02 / 01-2017




                 H-360                                                      A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                        Residue Qty.
                                        Production > Capacity planning > Control station > Functions menu > Show
                                        residue quantities




                                        Fig. H-231    Display residual quantities and report completed


                                        On this dialog, you check which orders have not yet been reported completed,
                                        and to report them as such if required.

                                        Display from status You can limit the display of the open orders to a mini-
                                        mum status, e.g. to exclude orders from the display the production of which
                                        has already begun.

                                        Overview
                                        In the overview, all orders are displayed which have not been produced up to
                                        the current date. When you tick the checkbox, the corresponding order will be
                                        reported completed for the current date when you have confirmed with [OK].
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                              H-361
                 Control Station                                                                   Software Reference




                                   Control Station (Order)
                                   Production > Capacity planning > Control station > Functions menu > Select
                                   order.
                                   On this dialog, you check the individual machines that an order runs through
                                   from production to shipping to move the scheduling on the "critical" machines.
                                   The Control station (Order) dialog contains the following tabs:
                                   •   “Control Station (Order) – Machines” on page H-364
                                   •   “Control Station (Order) – Detail” on page H-366
                                   •   “Control Station (Order) – Work Types” on page H-368
                                   •   “Control Station (Order) – Purchased Elements” on page H-370
                                   •   “Control Station (Order) – Move I” on page H-371
                                   •   “Control Station (Order) – Move II” on page H-372
                                   •   “Control Station (Order) – Load” on page H-374
                                    Tutorial, “Control Station – Order” on page H-164

                                   Navigation through the tabs and dialogs
                                   The following overview shows you how to display the data.

                                   Tab                  Action                           Tab / dialog

                                   Machines             Double-click on machine     ->   Move II
                                                        Double-click on date             Detail

                                   Detail               Click on cell header        ->   Work types


                                   Functions Menu
                                   Production > Capacity planning > Control station > Functions menu > Select
                                   order.
                                   Using this menu, you can open other dialogs without closing the control sta-
                                   tion.

                                   Document group
                                   •   Show document:
                                       Opens the document view.
                                   •   History:
                                       Opens the History dialog where you can check the process of status chang-
                                       es.
                                        Sales, “History” on page C-478
                                   •   Status change:
                                       Opens the dialog by the same name on which you can change the order
                                       status.
                                        Sales, “Status Change” on page C-479
4.02 / 01-2017




                 H-362                                                         A+W Business Pro Capacity Planning
                 Software Reference                                                                       Control Station




                                        Graphic group
                                        •   Production area:
                                            Opens the graphical display Production areas/weekly overview to compare
                                            the completed and open quantities.
                                        •   Order:
                                            Opens the graphical display Order info/weekly overview to compare the
                                            completed and open quantities.
                                            These graphics correspond to the Graphic areas display.
                                             “Area Graphic” on page H-259

                                        Production group
                                        •   Reports list:
                                            Opens the Reports overview dialog to check the current status of produc-
                                            tion per order item.
                                             “Report List” on page H-318
                                        •   Scheduling:
                                            Opens the Schedule order dialog to change the scheduling of the current
                                            order.
                                             “Book Order” on page H-275
                                        •   Manual settings:
                                            Opens the Order completion status dialog on which you can check the pro-
                                            duction status of the order.
                                             “Production Level Orders” on page H-307


                                        Options Menu
                                        Production > Capacity planning > Control station > Functions menu > Select
                                        order.
                                        Using this menu, you can determine the default setting of the dialog. You can
                                        activate or deactivate options. The settings will not be reset when you close
                                        the dialog.
                                        The description of the following entries reflects the activated state:
                                        •   Check dwell time:
                                            Before moving, it is checked whether the transition times permit a move.
                                            You should select this setting if you know that the transition requires longer
                                            transfer times, e.g. for TG production.
                                            You should only suppress this check if the transition from one production
                                            area to the next one does not require long transition times.
                                        •   Ignore dwell days:
                                            Ignores the dwell day when rescheduling.
                                        •   Postpone setup time:
                                            If this option is activated, the buttons on the Move II tab are locked.
                                        •   Setup time check:
                                            If the set-up time has been defined for several work types performed for an
4.02 / 01-2017




                                            order item, this time shall be charged just once per item.




                 A+W Business Pro Capacity Planning                                                                H-363
                 Control Station                                                                         Software Reference




                                             •   Suppress messages:
                                                 Errors that occur during rescheduling for another date or another machine
                                                 are displayed in a message. You can suppress these messages.


                                             Control Station (Order) – Machines
                                             Production > Capacity planning > Control station > Functions menu > Ma-
                                             chines tab




                    Fig. H-232     Control station (order) – Machines


                                             On this tab, you check the utilization of the machines which are producing this
                                             order. If you have opened the dialog from the control station, the data for the
                                             current order is displayed. However, you can use the search mode to display
                                             another order or limit the display to a particular position.
                                             If the order was reported completed manually, all previously not reported val-
                                             ues are shifted to the day of the completion report. In this case, the production
                                             dates are shown in green.

                                             Order

                                             Number, customer Number and customer name stated in the order.
4.02 / 01-2017




                 H-364                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                        Control Station




                                        Only item Number of the item to be changed. The field is released in selec-
                                        tion mode. You can specify the item number if you want to display one order
                                        item only. If you enter a zero (0), all items are displayed.

                                        Delivery date Delivery date stated in the order. You can change the date and
                                        confirm this by [Change].
                                         Tutorial, “Postpone Scheduling for single Order” on page H-166

                                        [Change] Confirms the new date.

                                        Order area Order area from which the order comes.

                                        Production of, to Display of the period in which the order is produced.

                                        Overview
                                        In the overview, all machines are displayed on which the order is produced.

                                        Day of the week, date Per weekday, the utilization is displayed with the
                                        scheduled and free time (all shifts) per machine.
                                        • Scheduled and free time (all shifts).
                                        • Open and produced quantity of all sheets in pcs.
                                        • Total surface in sqm.
                                        • Edge length of all sheets.
                                        • Utilization in percent.
                                        All details except for the time can be selected or deselected in the control sta-
                                        tion settings.
                                         “Settings for Control Station” on page H-359
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-365
                 Control Station                                                                       Software Reference




                                              Control Station (Order) – Detail
                                              Production > Capacity planning > Control station > Functions menu > Select
                                              order > Detail tab




                    Fig. H-233     Control station (order) – Detail


                                              On this tab, you can move quantities manually or report them completed. The
                                              machine to which these details refer is shown above the fields.
                                              If you have moved a whole item, it is removed from the display.

                                              Overview
                                              The quantities for the current order on the selected machine are displayed in
                                              the overview. The following columns are displayed:
                                              •   Shift:
                                                  Current shift.
                                              •   Pcs.:
                                                  Pieces of the order on the current machine.
                                              •   Finished:
                                                  Quantity of glass produced.
4.02 / 01-2017




                 H-366                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                    Control Station




                                        •   Move:
                                            Changes can be adopted only if this checkbox is ticked.
                                            If the changes clash with other processes for this order, an error message
                                            will indicate that this process cannot be moved.
                                        •   Hours:
                                            Time scheduled for the quantity displayed.

                                        [Load / Day] Updates the display in the field below.

                                        Move

                                        New date Production date to which the order shall be moved.

                                        Shift Shift to which the order shall be moved.

                                        Machine Machine to which the order shall be moved. The field is released if
                                        you have ticked the Move checkbox and confirmed with [OK].

                                        [Load] Checks the utilization of the alternative machine. The value is dis-
                                        played in hours. It includes the times of the order.

                                        [Roll back] Sets the move back to the original values.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                            H-367
                 Control Station                                                                       Software Reference




                                             Control Station (Order) – Work Types
                                             Production > Capacity planning > Control station > Functions menu > Select
                                             order > Work types tab




                    Fig. H-234     Control station (order) – Work types


                                             On this tab, you check which work types are to be performed on a machine on
                                             a production date.
                                             If you have moved a whole item to another date, it is removed from the display.

                                             [All], [None] Ticks or unticks all checkboxes in the Move column.

                                                 Edit setup times
                                                 Using the context menu (right mouse key) on an item, you can add or de-
                                                 lete set-up times. For this, the set-up time must be created as work type
                                                 with a basic time.
4.02 / 01-2017




                 H-368                                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                     Control Station




                                        Overview
                                        The following data is displayed in the overview:
                                        •   Shift:
                                            Shift in which the item shall be produced.
                                        •   Item:
                                            Item number from the order.
                                        •   BOM ID:
                                            BOM ident number, i.e. the BOM level.
                                        •   SI:
                                            Sub-items resulting from the splitting of items at scheduling.
                                        •   Process:
                                            Work type.
                                        •   Product/Processing:
                                            Product name.
                                        •   Pcs.:
                                            Item quantity.
                                        •   Pcs:
                                            Quantity of sheets produced.
                                        •   Size:
                                            Dimensions of the item.
                                        •   Move:
                                            Changes can be adopted only if this checkbox is ticked.
                                            If the changes clash with other processes for this order, an error message
                                            will indicate that this process cannot be moved.
                                            These messages can be switched off using the Options menu.
                                        •   Hours:
                                            Time reserved for this item.

                                            Move scheduling
                                            The fields in the Move group are explained for the Detail tab.

                                             “Control Station (Order) – Detail” on page H-366
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                             H-369
                 Control Station                                                                      Software Reference




                                             Control Station (Order) – Purchased Elements
                                             Production > Capacity planning > Control station > Functions menu > Select
                                             order > Purchased elements tab




                    Fig. H-235     Control station (order) – Purchased elements


                                             On this tab, you check which purchased articles are required for production.

                                             Overview
                                             The following data is displayed in the overview:
                                             •   Item:
                                                 Item number from the order.
                                             •   Article/processing:
                                                 Product name of the purchased element.
                                             •   Quantity:
                                                 Quantity that to be purchased.
                                             •   Size:
                                                 Dimensions of the item.
                                             •   Ordered to:
                                                 Delivery date requested by the supplier
4.02 / 01-2017




                 H-370                                                              A+W Business Pro Capacity Planning
                 Software Reference                                                                      Control Station




                                          •   Deliv.:
                                              Quantity delivered.
                                          •   Required on, date, shift:
                                              These three columns display when the purchased elements are required
                                              where.


                                          Control Station (Order) – Move I
                                          Production > Capacity planning > Control station > Functions menu > Select
                                          order > Move I tab




                   Fig. H-236   Control station (order) – Move I


                                          On this tab, you plan and edit the load of the machines with series. This func-
                                          tion is not currently used.

                                          Order
                                          This group displays the order number and name of the customer.

                                          Postpone for whole days

                                          No. of days Number of days by which the production of the series shall be
4.02 / 01-2017




                                          postponed.




                 A+W Business Pro Capacity Planning                                                               H-371
                 Control Station                                                                        Software Reference




                                              Only from date Initial date from which the full days specified above shall be
                                              counted.


                                              Control Station (Order) – Move II
                                              Production > Capacity planning > Control station > Functions menu > Select
                                              order > Move II tab




                    Fig. H-237     Control station (order) – Move II


                                              On this tab, you move the items or orders to other dates, shifts or machines.
                                              If you have moved a whole item, it is deleted from the display.

                                              Overview
                                              The quantities for the current order for the selected machine are displayed in
                                              the overview. The following columns are displayed:
                                              •   Date:
                                                  Scheduled production date.
                                              •   Shift:
                                                  Current shift.
                                              •   Pcs.:
4.02 / 01-2017




                                                  Pieces of the order on the current machine.
                                              •   Finished:
                                                  Quantity of glass produced.


                 H-372                                                               A+W Business Pro Capacity Planning
                 Software Reference                                                                       Control Station




                                        •   Move:
                                            Changes can be adopted only if this checkbox is ticked.
                                            If the changes clash with other processes for this order, an error message
                                            will indicate that this process cannot be moved.
                                        •   Hours:
                                            Time scheduled for the quantity displayed.

                                            Areas locked
                                            The Fill shift and Compress areas can be locked in the Options > Move set-
                                            up time menu.

                                        Fill shift
                                        You can recheck the shift times to fill gaps in a shift using suitable quantities
                                        from the previous or the next shift.

                                        [Backwards] Recalculates the shifts. The quantities are moved to an earlier
                                        shift if possible.

                                        [Forward] Recalculates the shifts. The quantities are moved to the next shift
                                        if possible.

                                        Compress
                                        You can recalculate the utilization of the machine. This way you can fill gaps
                                        which occurred due to the settings regarding the proportional utilisation when
                                        an item was split or if e.g. an order was cancelled so that there is more free
                                        capacity.
                                         “Fill shift in case of item splitting” on page H-180
                                         “Split Items” on page H-284

                                        [Backwards] Recalculates the utilization, starting backwards from the dis-
                                        played date.

                                        [Forward] Recalculates the utilization, starting forward from the displayed
                                        date.

                                        Move
                                        The fields in the Move group are explained for the Detail tab.
                                         “Control Station (Order) – Detail” on page H-366
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                                H-373
                 Control Station                                                                         Software Reference




                                             Control Station (Order) – Load
                                             Production > Capacity planning > Control station > Functions menu > Select
                                             order > Load tab




                    Fig. H-238     Control station (order) – Load


                                             On this tab, you check which order items are to be produced by the machine
                                             in addition to the current order items. The order items for which the display has
                                             been started are highlighted in green.

                                             Selection

                                             From date, to date Period that you want to check.

                                             Machine Machine for which you want to check the scheduled orders.

                                             Overview
                                             In the overview, all order items are listed that must be produced in the selected
                                             period.
                                             •   Date:
                                                 Production date.
4.02 / 01-2017




                                             •   Shift:
                                                 Shift in which the item is produced.



                 H-374                                                                  A+W Business Pro Capacity Planning
                 Software Reference                                                                  Control Station




                                        •   Order, item:
                                            Order and item number.
                                        •   Product:
                                            Product name.
                                        •   Glass size:
                                            Size of the item.
                                        •   Element:
                                            Product name of the BOM component.
                                        •   Work type:
                                            Work type in the production area.
                                        •   Pcs:
                                            Number of pieces of the item.
                                        •   Time:
                                            Scheduled time.
                                        •   Customer:
                                            Customer name from the order.


                                        Moving impossible
                                        Production > Capacity planning > Control station > Move




                                        Fig. H-239    Move not possible


                                        On this dialog, you check why the intended move of an order is impossible.
                                        You can suppress the display of this message.
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                          H-375
                 Control Station                   Software Reference
4.02 / 01-2017




                 H-376             A+W Business Pro Capacity Planning
Capacity Planning            H

                    Section Index




              A+W Business Pro
                 Section Index                                                                                Index




                 Index
                 A                                                C
                 Activity see work type                           Calculation example
                 Allocate                                         – machine hour H-46
                 – next processing H-240                          – man hour H-43
                 – PGR - work type H-236                          Calendar
                 – product H-238                                  – add shift times H-53
                 – product class - work type H-237                – adjust H-49
                 – product type - work type H-234                 – closing time for shift H-187
                 Allocation                                       – create for capacity planning H-50
                 – BOM component H-105                            – for unit, production area H-50
                 – combination product class H-247                – machine H-209
                 – combination product type H-239                 – set up special shift H-54
                 – combined product type, product class   H-105   – shift times H-212
                 – implicit, explicit H-102                       – specify shift times H-49
                 – machine H-102                                  Capa see capacity planning
                 – overview of the dialogs H-103                  Capacity
                 – special work type H-106                        – bottleneck H-285
                 – specifying H-107                               – item split H-288
                 – specifying special allocation H-107            – per machine H-201
                 Alternative process H-60, H-223                  – per workday H-41
                 Alternative without BOM H-223                    – specify utilization H-47
                 Alternative work type H-30                       – work unit H-43
                 – selection of the machine H-93                  Capacity planning
                 – work types H-191                               – basic ideas H-20
                 Assigned machines                                – calculation example H-113
                 – production areas H-194                         – cost centres H-160, H-268
                 – work types H-191                               – default settings in company data H-183
                                                                  – interplay of the master data H-20
                 B                                                – menu overview H-16
                 Backward scheduling H-113                        – org. overview H-219
                 Basic time H-61, H-223                           – possibilities for using H-21
                 – creating graduation H-76                       – production list H-306
                 – enter time value H-78                          – resolve bottleneck H-130
                 – work process H-59                              – scheduling according to route H-122
                 Batch                                            – scheduling order H-123
                 – report completed H-300                         – series factor H-195
                 – setting for manual completion report H-301     – shift filling H-122
                 BOM                                              – statistics H-262
                 – allocation H-105                               – time calculation H-39
                 – production status H-318                        Capacity planning module H-16
                 Bottleneck                                       Capacity problems H-118
                 – resolving H-130                                – item split H-119
                 – selection of the delivery date H-123           Change of the production area H-68
                 Breakage                                         Check
                 – manual report H-150                            – specify in machine types H-189
                                                                  Check value see restriction
4.02 / 01-2017




                 – reporting H-140
                                                                  Checking
                                                                  – fields for restrictions H-88
                                                                  – restrictions H-26


                 A+W Business Pro Capacity Planning                                                          H-383
                 Index                                                                        Section Index




                 Closing time for scheduling H-121          Conversion
                 Combination product class                  – default time in hours H-61
                 – time factor H-247                        Cost calculation
                 Combination product type                   – in order H-163
                 – allocating (capa) H-239                  – in quotation H-163
                 Company data                               Cost centres
                 – settings for capacity planning H-99      – analysis in capacity planning H-268
                 Completion report                          – definition (capa) H-269
                 – catching up on H-154                     – period for evaluation (capa) H-268
                 – graphic H-299                            Costs
                 – manual H-147                             – machine H-201
                 – navigation through the tabs H-311        – per machine H-204
                 – overview H-296                           – per order H-315
                 – per item H-297                           Create setup time H-74
                 – piece by piece H-297                     Cube
                 – production batch H-300                   – default time H-228
                 – production date H-296                    – limit types (capa) H-228
                 – purchased elements H-298
                 – report order completed manually H-302    D
                 – reports H-136                            Date
                 – reports overview H-322                   – calculation example H-113
                 – residual quantities H-365                – change production date H-325, H-327
                 – setting for batch H-301                  – mode for date search H-276
                 Completion status                          Date calculation
                 – order H-311                              – example dwell days H-114
                 Control station                            Date search mode H-276
                 – check prev. processes H-345              Deduction for series H-75
                 – machine (dialog) H-348                   Default time H-61
                 – machine (tab) H-333                      – alternative process H-60
                 – navigation through the tabs H-331        – basic time H-59
                 – order (dialog) H-366                     – change per work time, machine H-229
                 – orders (tab) H-334                       – conversion to hours H-61
                 – production areas H-332                   – copy H-229
                 – purchased elements H-347                 – cube H-228
                 – reschedule item H-338                    – entering time value H-78
                 – reschedule order H-336                   – format H-61
                 – settings H-363                           – graduated H-225, H-226, H-228
                 – utilization per shift H-344              – individual time per unit H-227
                 – work types H-340                         – matrix H-225
                 – working with the control station H-166   – priority H-60
                 Control station machine                    – setup time H-74
                 – load H-352                               – specifying H-76
                 – utilization H-354                        – specifying format H-76
                 – utilization of the shifts H-350          – time surcharge H-63
                 – working with the control station H-169   – triangle H-61, H-225
                 Control station order                      – type H-59
                 – machines H-368                           – type basic time H-222
                 – move H-370, H-376                        – vector H-226
                 – navigation through the tabs H-366        Default times
4.02 / 01-2017




                 – purchased elements H-374                 – other surcharges H-222
                 – utilization H-378                        Defaults
                 – work types H-372                         – times H-57
                 – working with the control station H-168


                 H-384                                                A+W Business Pro Capacity Planning
                 Section Index                                                                                    Index




                 Definition of cost centres (capa) H-269               G
                 Delivery date                                         Gas
                 – for bottleneck H-123                                – technical restriction (capa) H-206
                 – move for scheduling H-278                           Graduation H-61
                 – schedule in capacity planning H-278                 – cube for default time H-228
                 – select manually H-278                               – matrix for default time H-225
                 Detail                                                – triangular shape for time H-61
                 – control station H-342                               – vector for default time H-226
                 – control station order H-370                         Graphic
                 Display conventions H-15                              – completion reports H-299
                 Dwell days                                            – utilization H-361
                 – calculation example H-114                           – weekly overview H-263
                 – calculation example with transition
                   times H-115
                                                                       H
                 – dwell matrix H-214
                                                                       Hours
                 – production area H-200
                                                                       – per shift   H-39

                 E                                                     I
                 Edge processing
                                                                       Ignore process H-223
                 – time factor H-243
                                                                       Individual time as default time H-227
                 Example
                                                                       Item
                 – calculation for transition and dwell times   H-69
                                                                       – change production date H-327
                 – calculation of capacities H-113
                                                                       – check dimensions H-190
                 – plan time for IG H-64
                                                                       – forbid split H-185
                                                                       – production status H-316
                 F                                                     – report completed manually H-302
                 Factor                                                – schedule manually H-281
                 – calculation example for time planning H-67          – scheduling in capacity planning H-128
                 – default time H-67                                   – shift filling for split H-184
                 – series H-75                                         – splitting H-131
                 Factor for                                            Item split H-288
                 – combination product class H-247                     Item splitting
                 – combination product type H-239                      – manual scheduling H-130
                 – edge processing H-243
                 – next processing H-240
                                                                       L
                 – next processing+shape H-245
                                                                       Labor costs
                 – PGR H-236
                                                                       – machines H-201
                 – product H-238
                                                                       – per unit H-204
                 – product class H-237
                                                                       Lock
                 – shape H-241
                                                                       – by PGR H-251
                 – special time H-75
                                                                       – by product H-254
                 – work type H-234
                                                                       – by product class H-252
                 Failure
                                                                       – customer-related (capa) H-256
                 – machine H-291
                                                                       – production line H-258
                 Formula
                                                                       Lock value see restrictions
                 – for workflow task for scheduling H-118
                                                                       Locking
                 Forward scheduling H-113
                                                                       – lock formula H-87
                 Function enabled H-13
                                                                       – machine H-94
4.02 / 01-2017




                                                                       – overview of the dialogs H-95
                                                                       – shifts H-187




                 A+W Business Pro Capacity Planning                                                              H-385
                 Index                                                                                Section Index




                 M                                                  Master data (capa)
                 Machine H-25                                       – calendar H-209
                 – assigned work types H-206                        – Components of capacity planning H-20
                 – calendar H-210                                   – general H-189
                 – changing after scheduling H-175                  – machines H-200
                 – complete, locking temporarily H-96               – production area H-199
                 – costs per order H-163                            – recommended sequence H-23
                 – create H-33                                      – special technical restrictions H-216
                 – default time H-59                                – special times H-230
                 – failure H-291                                    Matrix
                 – lock H-201                                       – default times H-225
                 – lock customer-related H-256                      Menus
                 – lock for PGR H-251                               – capacity planning in the Production
                 – lock for product H-254                             module H-18
                 – lock for product class H-252                     – master data for the capacity planning H-16
                 – lock on production line H-258                    Move
                 – locking H-94                                     – control station order H-376
                 – priority H-60                                    – not possible H-379
                 – selection during scheduling H-89
                 – selection for alternative work type H-93         N
                 – selection for manual completion report H-305     Navigation
                 – selection in case of capacity bottleneck H-285   – control station dialog H-331
                 – selection of work type H-191                     – control station order dialog H-366
                 – skip next machine H-255                          – order completion status dialog H-311
                 – skip process H-259                               Next machine
                 – skipping H-94                                    – skip H-255
                 – specifying default time H-76                     Next processing H-240, H-245
                 – specifying restrictions H-36                     Number manager
                 – time costs H-158                                 – schedule in capacity planning H-272
                 – times and costs H-28
                 Machine hour H-46
                                                                    O
                 Machine type H-25, H-189
                                                                    Order
                 – assigned machines H-194
                                                                    – change production date H-325
                 – restrictions H-26
                                                                    – completion status H-311
                 Machines H-200
                                                                    – delete scheduling H-129
                 – calendar H-209
                                                                    – report completed manually H-302
                 – check production dimensions H-190
                                                                    – reporting complete manually H-147
                 – check spacer H-190
                                                                    – rescheduling H-170
                 – control station order H-368
                                                                    – resolve capacity bottleneck H-130
                 – in the production area H-219
                                                                    – schedule manually H-279
                 – per machine type H-194
                                                                    – scheduling in capacity planning H-123
                 – per production area H-194
                                                                    – time costs H-163
                 – per work type H-194
                                                                    Order item
                 – priorities H-86
                                                                    – scheduling individual H-128
                 – technical restriction H-206
                                                                    – split H-119
                 – type H-189
                                                                    – splitting H-131
                 – utilization control station order H-378
                                                                    Other surcharge
                 Man hour H-43
                                                                    – editing graduation H-82
                 Manual
                                                                    Overview
4.02 / 01-2017




                 – report order completed H-302
                                                                    – area graphic H-263
                 – setting for completion report H-305
                                                                    – completion reports H-296
                 Manual scheduling
                                                                    – current production status H-314
                 – order H-281


                 H-386                                                        A+W Business Pro Capacity Planning
                 Section Index                                                                   Index




                 – display residual quantities H-365     – items H-316
                 – production list H-307                 – order H-315
                 – purchased elements (control station   – purchased elements H-319
                   order) H-374                          – reports overview H-322
                 – scheduled orders H-287                Production time
                 – utilization on date H-355             – change H-324
                                                         – specify H-288
                 P                                       – specify start date H-281
                 Personnel costs                         Purchased elements
                 – per order H-163                       – completion reports H-298
                 PGR                                     – control station H-347
                 – allocate (capa) H-236                 – control station order H-374
                 Priority                                – order (production status) H-319
                 – alternative priority H-86
                 – default times H-222                   Q
                 – distinction from restriction H-88     Quotation
                 – for equivalent machine H-86           – time costs   H-163
                 – special priority H-231
                 Process                                 R
                 – alternative H-222                     Reports H-136
                 – skip H-259                            – breakage H-144
                 Process see work type                   – completion report H-142
                 Product                                 – items H-322
                 – allocating (capa) H-238               – production area H-200
                 Product class                           – registration points H-138
                 – allocating H-237                      – status assignment H-140
                 Production area H-199                   Reschedule
                 – calendar H-210                        – control station order H-372, H-376
                 – create H-32                           – item (control station) H-338
                 – dwell days H-200, H-214               – not possible H-379
                 – dwell time H-68                       – order (control station) H-336
                 – org. overview H-219                   Rescheduling
                 – transition time H-68                  – item H-342
                 – transition type H-196                 – work type H-340
                 – units H-199                           Residual quantities
                 Production areas H-31                   – checking H-154
                 Production line H-258                   – previous day H-365
                 – defining H-97                         – report completed H-365
                 Production list                         – setting for transfer H-294
                 – capacity planning H-306               – status setting H-143
                 – print format H-309                    Restrictions
                 – printing H-145                        – activate checks H-189
                 – settings H-310                        – comparison with priorities H-88
                 – sorting H-310                         – per machine H-36
                 production list H-310                   – technical restrictions H-26
                 Production module                       – with lock formula H-87
                 – Capacity planning H-18                Route
                 Production sequence H-102               – date search H-122
                 Production status
4.02 / 01-2017




                 – BOM H-318
                 – calculation H-315
                 – checking H-152



                 A+W Business Pro Capacity Planning                                             H-387
                 Index                                                                            Section Index




                 S                                               Shape
                 Schedule                                        – allocating H-241
                 – by number manager H-273                       – technical restrictions H-206
                 – by order H-279                                – time factor H-241
                 – check result H-284                            Shift
                 – date search H-276                             – add times H-53
                 – item split H-288                              – closing time H-187
                 – search for delivery date H-186                – filling H-122
                 – select machine automatically H-185            – set up special shift H-54
                 Schedule calculation                            – shift change H-40
                 – backward scheduling H-113                     – shift transition H-39
                 – example transition times H-116                – specify number H-49
                 – example transition times + dwell days H-115   – specify quantity H-184
                 – forward scheduling H-113                      – times for shift H-187
                 Schedule manually                               – times in the calendar H-212
                 – check times H-290                             – times per workday H-39
                 – result H-284                                  Shift change H-40
                 – select machine H-285                          SI see subitem
                 – split item H-288                              Skip
                 Scheduling                                      – next machine H-255
                 – automatic H-117                               – process H-259
                 – capacity bottleneck H-285                     Sorting H-310
                 – capacity problems H-118                       Special allocation H-240
                 – changing machine H-175                        – edge processing H-243
                 – Closing time H-121                            – next processing + shape H-245
                 – in capacity planning H-117                    – shape H-241
                 – individual item in capacity planning H-128    – specifying H-107
                 – manual H-117                                  Special priority H-86, H-231
                 – moving order H-170                            Special times
                 – order H-123                                   – creating H-80
                 – resolving bottleneck H-130                    – surcharge (capa) H-230
                 – schedule calculation H-113                    Special times (surcharge) H-62, H-75
                 – settings for automatic scheduling H-99        Splitting
                 – split item H-131                              – item H-288
                 – workflow task H-117                           – item split H-119
                 Sequence                                        – locking of production times H-120
                 – recommendation for master data for capacity   – manual item splitting H-130
                   planning H-23                                 Statistics
                 Sequence of the work processes H-102            – by order area H-264
                 Sequencing number H-191                         – capacity planning H-262
                 Series                                          – order area short H-267
                 – factor for time H-75                          Statistics by order area
                 Series factor H-195                             – long H-264
                 Set up special shift H-54                       – short H-267
                 Settings                                        Status
                 – automatic scheduling H-99                     – assignment in capacity planning H-140
                 – batch H-301                                   – assignment through report H-141
                 – control station H-363                         – Manual allocation H-141
                 – default settings in company data H-99         Status report H-200
4.02 / 01-2017




                 – manual completion report H-305                Stock articles
                 – production list H-310                         – allocate work type H-248
                 – reports H-137



                 H-388                                                     A+W Business Pro Capacity Planning
                 Section Index                                                                        Index




                 Surcharge                                 U
                 – creating special times H-80             Utilisation
                 – for production time H-62                – machines (control station) H-333
                 – special time H-62, H-230                – per production area (control station) H-332
                                                           Utilization
                 T                                         – completion reports H-296
                 Technical restriction                     – default settings H-47
                 – machines H-206                          – graphic H-361
                 – work type H-216                         – on date H-357
                 – work types H-206                        – orders (control station) H-334
                 Time                                      – overview for date H-355
                 – graduation, limit types H-61            – prev. processes (control station) H-345
                 – reduction H-67                          – print overview H-362
                 – reservation for item split H-120        – set status H-363
                 – value for basic time H-78               – shifts H-344
                 Time calculation H-39
                 Time costs H-158                          V
                 – per order H-163, H-315                  Vector
                 – per quotation H-163                     – default times   H-226
                 Time factor
                 – combination product class H-247
                                                           W
                 – edge processing H-243
                                                           Work centers see production areas
                 – next processing H-240
                                                           Work process
                 – next processing+shape H-245
                                                           – skipping H-94
                 – series H-75
                                                           Work type
                 – shape H-241
                                                           – allocate stock articles H-248
                 Time management see capacity planning
                                                           – alternative work type H-30
                 Time planning
                                                           – assigned machines H-191, H-194
                 – basic components H-57
                                                           – control station H-340
                 – calculation example H-67
                                                           – control station order H-372
                 – example IG H-64
                                                           – factor for product type H-234
                 – factor, surcharge H-67
                                                           – machines H-206
                 Time surcharge H-223
                                                           – processes, activities H-29
                 – calculation example H-67
                                                           – skipping H-94
                 – creating special time H-80
                                                           – special for allocation H-106
                 – default time H-59
                                                           – specifying default time H-76, H-78
                 – work type H-63
                                                           – time surcharge H-63
                 Transition time
                                                           Work unit
                 – calculation example H-115
                                                           – machine hour H-46
                 – calculation example with shifts H-116
                                                           – man hour H-43
                 – work type H-196
                                                           Workdays H-39
                 Triangle H-61
                                                           – capacity per production area H-41
                 – default time H-225
                 Type
                 – default time H-59
4.02 / 01-2017




                 A+W Business Pro Capacity Planning                                                 H-389
                 Index                         Section Index
4.02 / 01-2017




                 H-390   A+W Business Pro Capacity Planning

