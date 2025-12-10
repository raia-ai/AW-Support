---
description: "EN AWProduction Machinery Allocation 2.10"
---



# EN AWProduction Machinery Allocation 2.10

Machine Allocation         D




                            english




                A+W Production
                                                                                                                Introduction




                                        Introduction
                                        This part of the documentation contains editorial notes.


                                        Revision Overview
                                        Machine Allocation         Description
                                        Version / Date

                                        2.10 / 11-2018             New chapter regarding Machine type.
                                                                   Screenshots updated.

                                        2.02 / 01-2017             Product and company names adjusted.

                                        2.01 / 01-2013             Layout adjusted to CI 2013.

                                        2.00 / 09-2012             Creation of tutorial, revision of software reference

                                        1.00 / 01-2003             Original version



                                        Editorial
                                        The editorial contains the following themes:
                                        •   Notes on this document
                                        •   Copyrights
                                        •   Trademarks
                                        •   Contact

                                        Notes on this document
                                        This document is intended only for end users of A+W Production.
                                        The documentation and software described are licenses that must be used or
                                        copied only in accordance with the conditions of our license agreement. The
                                        contents of the documentation are only informative and is subject to changes
                                        without prior notice.
                                        The text and illustrations were compiled with the utmost care. Still, errors can-
                                        not be totally excluded. A+W Software GmbH cannot be held liable for errors
                                        or inaccuracies, unless they can be attributed to wilful or grossly negligent ac-
                                        tion.
                                        The descriptions in this document are based on the full program level of A+W
                                        Production.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                        D-3
                 Introduction




                                Copyrights
                                © 2018, A+W Software GmbH, all rights, including the right of reprint, produc-
                                tion of copies and translation, are reserved.
                                The documentation must be copied, completely or in part, saved, or transfer-
                                red only in accordance with our license agreement. Transmission of the docu-
                                mentation is not allowed, neither electronically, nor mechanically, nor by
                                recording or in any other way, without A+W Software GmbH prior approval in
                                writing.

                                Trademarks
                                All hardware and software names mentioned in this documentation might also
                                be registered trademarks or other property rights of third parties. The property
                                rights of third parties must be observed.

                                Contact
                                A+W Software GmbH

                                Am Pfahlgraben

                                D-35415 Pohlheim

                                   +49 6404 2051 0

                                   +49 6404 2051 877

                                aw.zentrale@a-w.com

                                http://www.a-w.com
2.10 / 11-2018




                 D-4                                                     A+W Production Machine Allocation
                                                                                                                                                        Contents




                                        Contents
                                        Introduction ............................................................................................................. D-3
                                          Revision Overview ............................................................................................... D-3
                                          Editorial ............................................................................................................... D-3

                                        Tutorial                                                                                                             D-7
                                        Overview ................................................................................................................. D-9
                                         Documentation .................................................................................................. D-10
                                            Tutorial Structure ........................................................................................... D-10
                                            Display Conventions ...................................................................................... D-11
                                        Basics ................................................................................................................... D-12
                                        Machine Allocation ................................................................................................ D-14
                                         Machines ........................................................................................................... D-15
                                            Machines and Machine Allocation ................................................................. D-16
                                            Machine Definition and Management ............................................................ D-22
                                            Definition and Editing of Machine Restrictions ............................................... D-26
                                            Machines Exercises ....................................................................................... D-32
                                         Logical Machines ............................................................................................... D-33
                                            Machines and Machine Allocation ................................................................. D-34
                                            Definition and Management of Logical Machines .......................................... D-36
                                            Logical Machines - Exercises ........................................................................ D-40
                                         Work Processes ................................................................................................ D-41
                                            Work Processes and Machine Allocation ....................................................... D-42
                                            Work Process Definition and Management .................................................... D-49
                                            Work Processes - Exercises .......................................................................... D-51
                                         Allocation of Work Processes ............................................................................ D-52
                                            Flexible Adaptation of Work Processes ......................................................... D-53
                                            Allocation of Work Processes and Logical Machines .................................... D-58
                                            Work Process Allocation - Exercises ............................................................. D-62
                                         Conditions, Formulas, Restrictions .................................................................... D-63
                                            Conditions and Formulas in Connection with Machine Allocation ................. D-64
                                            Select a Condition .......................................................................................... D-65
                                            Select a Formula for the Processing Time of a Logical Machine ................... D-66
                                            Selection of Conditions - Exercises ............................................................... D-68
                                         Processing Types and Processing Articles ....................................................... D-69
                                            Processing Types and Machine Allocation .................................................... D-70
                                            Processing Articles and Machinery Allocation ............................................... D-71
                                            Definition and Management of Processing Types ......................................... D-73
                                            Definition and Management of Processing Articles ....................................... D-76
                                            Machine Allocation - Exercises ...................................................................... D-80
                                        Machine Allocation - Buttons ................................................................................ D-81

                                        Software Reference                                                                                                D-83
                                        Machine Allocation ................................................................................................ D-85
                                         MA Editor ........................................................................................................... D-86
                                           MA Editor - Machines ..................................................................................... D-87
                                           MA Editor – Logical Machines ....................................................................... D-88
                                           MA Editor – Work Processes ......................................................................... D-90
                                           MA Editor – Work Process Allocation ............................................................ D-91
                                           MA Editor – Machine Types ........................................................................... D-93
2.10 / 11-2018




                                         New Machine ..................................................................................................... D-94
                                         Machine ............................................................................................................. D-95
                                         Dimension Restrictions .................................................................................... D-100
                                         Spacer Restrictions ......................................................................................... D-101


                 A+W Production Machine Allocation                                                                                                             D-5
                 Contents




                              Select a Condition ........................................................................................... D-102
                              New Logical Machine ...................................................................................... D-103
                              Logical Machine .............................................................................................. D-104
                              Formula Selection ........................................................................................... D-106
                              New Work Process .......................................................................................... D-107
                              Work Process .................................................................................................. D-108
                              New Machine Type .......................................................................................... D-110
                              Machine Type .................................................................................................. D-111
                            Machine Allocation - Formulas ........................................................................... D-113
                              Select Conditions ............................................................................................ D-114
                              Condition Editor (Graphic Version) .................................................................. D-115
                              New Condition ................................................................................................. D-117
                              Info (about the new condition) ......................................................................... D-117
                              Select quantity ................................................................................................. D-118
                              Condition Editor (Text Version) ....................................................................... D-119
                              Formula Editor ................................................................................................. D-120
                            Processings in Machine Allocation ..................................................................... D-122
                              Processing Types ............................................................................................ D-123
                              Processing Articles .......................................................................................... D-125
                              Adjust Columns ............................................................................................... D-128
                              Column Definition ............................................................................................ D-129

                            Section Index                                                                                             D-131
2.10 / 11-2018




                 D-6                                                                      A+W Production Machine Allocation
Machine Allocation          D

                        Tutorial




                A+W Production
                 Tutorial                                                                                       Overview




                                        Overview
                                        The tutorial on the Machine Allocation (MA) module deals with the allocation
                                        of machines in A+W Production. Machine allocation assigns the scheduled
                                        processing steps to the individual machines, taking into account machine re-
                                        strictions and instructions for production control. Check programs provided by
                                        the machine manufacturers can be used in A+W Production to see whether
                                        the processes are plausible.

                                           The functions depend on the released modules
                                           Please note that the individual functions are available only if the correspon-
                                           ding modules and interfaces have been installed and released.
                                           If you detect functions in this description which are not available in your ver-
                                           sion, please contact A+W Software GmbH.

                                        Prerequisite knowledge
                                        This tutorial is meant for persons in charge of production scheduling in A+W
                                        Production who are responsible for organizing the optimum production pro-
                                        cess. Participants must be familiar with the master data concept in A+W Pro-
                                        duction.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                    D-9
                 Overview                                                                                Tutorial




                            Documentation
                            The following documents are available on module Machine Allocation:

                            PDF                       Complete documentation
                                                      • Tutorial
                                                      • Software reference
                                                      • Index

                            Online help <F1>          Context-sensitive dialog help


                            Tutorial Structure
                            This tutorial consists of subjects with several training modules each. Each ses-
                            sion consists of the following elements:

                            Overview                  Each training session starts with an overview of the
                                                      major topics:
                                                      • Objectives: What shall be conveyed?
                                                      • Benefit: What can this knowledge be used for?
                                                      • Maxims: Which correlations are to be remembered?

                            Concepts                  Concepts and terms of the corresponding training
                                                      session will be explained first. This is followed by
                                                      examples and operating instructions.

                            Exercises                 There are exercises featuring special tasks for some of
                                                      the training sessions.
2.10 / 11-2018




                 D-10                                                 A+W Production Machine Allocation
                 Tutorial                                                                                        Overview




                                        Display Conventions
                                        Certain parts of the sentences are specially marked. Their meanings are:

                                        Italics                   mark character strings describing software elements,
                                                                  e.g. the dialog New machine.

                                        Bold                      marks character strings to be entered via keyboard, e.g.
                                                                  Enter 0.

                                        >                         shows the way to open a dialog, e.g. Master data > MA
                                                                  > MA editor > Machines > New.

                                        []                        Square brackets mark the buttons in the dialog, e.g.
                                                                  [OK] to save the data.

                                        <>                        Pointed brackets refer to keys or shortcuts on the
                                                                  keyboard, e. g. <F1> is used to open the online help.


                                        Reading instructions
                                        The contents of a training session are based on the knowledge conveyed in
                                        the previous session. We therefore recommend not to skip any session.
                                        If you are already familiar with a subject you should at least read the summary
                                        at the beginning of the session in order to bring the main details to mind.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                   D-11
                 Basics                                                                                                               Tutorial




                                               Basics
                                               The machine allocation depicts the references between work processes and
                                               machine. Based on the machines and the work processes, the capacity plan-
                                               ning can schedule the orders optimally.
                                               To set up the master data, the following questions must be answered:
                                               •      What task must be performed by the processing on a lite of an order: What
                                                      must be done.
                                               •      What method will be used: How will this be done.
                                               •      What tool will be used: Where will the processing be performed.
                                               •      Which ranking and restrictions have to be adhered to: Why or when will the
                                                      machine be used.



                             Restrictions, formulas,
                            e. g. minimum thickness
                                      2 mm


                                Properties,e. g.                                                               Processing article,
                             registration point 180,                                                            e. g. float cutting
                                 cost center 25



                                 Machine type,                          Formulas,                              Processing type,
                                  e. g. cutting                      e. g. is a shape                            e. g. cutting



                                                                    Logical machine,
                                    Machine,                                                                     Work process,
                                                                      e. g. logical
                              e. g. cutting table 8                                                              e. g. IG cutting
                                                                     cutting table 8




                                                                                          Allocation of work




                                                                                        A+W Production issues
                                                                                                the


                 Fig. D-1       Elements of machine allocation.


                                               This figure shows the software elements belonging to machine allocation and
2.10 / 11-2018




                                               how they are connected.




                 D-12                                                                         A+W Production Machine Allocation
                 Tutorial                                                                                         Basics




                                        Machines are defined by a Machine type, Properties, and Restrictions. In the
                                        above example, cutting table 8 is allocated to machine type Cutting.
                                        One of the properties of cutting table 8 is that it is allocated to registration
                                        point 180 and cost center 25. The logical machine for cutting table 8 is called
                                        logical cutting table 8. It has been assigned the formula Is a shape.

                                        Description of the work processes
                                        Using the work processes, the material streams in production are divided up
                                        and can be handled separately. Work processes therefore have to be regar-
                                        ded first.
                                        For the set-up of the work processes, the following questions are considered:
                                        •   Which processings can be combined and which may not be combined?
                                        •   Are there processings that are performed but that do not appear in the
                                            BOM?
                                        •   Are there different material streams, e.g. series lites, bathroom mirrors, RV
                                            lites that make very individual ways through production and therefore
                                            should be distinguished early on?
                                        •   Are there work processes that are not performed here, e.g. sand blasting
                                            at the other end of the city?

                                        Description of the machines
                                        In that the machines are described precisely, it is guaranteed that lites to be
                                        produced find valid machines. Here, there is a distinction between physical re-
                                        strictions and logical machines with additional restrictions, cost rates and tran-
                                        sition times.
                                        Added to the list of machines are places that are not machines in the usual
                                        sense but that are relevant for production, e.g. warehouse, incoming goods,
                                        shipping warehouse, loading ramp, additional production locations.

                                        Description of the logical machine
                                        Logical machines are used to express different transition times, cost rates or
                                        processing durations in the capacity planning. As a guideline, you can set up
                                        a logical machine if a machine can be used in different operating modes.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                  D-13
                 Machine Allocation                                                                           Tutorial




                                      Machine Allocation
                                      This chapter tells you which sections of A+W Production are part of machine
                                      allocation (MA) and how to allocate the machines.
                                      The MA editor is used to manage machines, logical machines, and processes
                                      as well as their allocations and properties.
                                      Machine allocation includes the following chapters:
                                      •   “Machines” on page D-15
                                      •   “Logical Machines” on page D-33
                                      •   “Work Processes” on page D-41
                                      •   “Allocation of Work Processes” on page D-52
                                      •   “Conditions, Formulas, Restrictions” on page D-63
                                      •   “Processing Types and Processing Articles” on page D-69


                                      The following sessions will familiarize you with the machines, logical machi-
                                      nes, processes, and allocation of processes. This knowledge will be deepened
                                      later on when we will be dealing with processing types and the selection of for-
                                      mulas.
2.10 / 11-2018




                 D-14                                                          A+W Production Machine Allocation
                 Tutorial                                                                               Machine Allocation




                                        Machines
                                        Objectives

                                        • The meaning of machines in A+W Production and especially in the context of
                                          machine allocation.
                                        • How to manage, define, edit, or delete machines.
                                        • The use of meaningful names and numbers.


                                        Benefit

                                        • Machines represent the physical machinery. Machines are therefore the basis for
                                          production control.


                                        Note

                                        Machines                   Machines represent the physical machinery.
                                                                   Names and numbers are systematically assigned in
                                                                   A+W Production.

                                        Machine types              Machine types are already defined in A+W Production
                                                                   and are allocated to the machines. Machine types define
                                                                   the type of machine, e.g. cutting, spacer bender or
                                                                   Others.

                                        Relations                  AND-/OR relations are the operators by which
                                                                   restrictions, conditions, and formulas are linked in A+W
                                                                   Production.

                                        Cuts                       Z- and W cuts are more complex cuts which can be
                                                                   allocated an additional cost factor, Costs per Z cut.

                                           Prerequisite
                                           To define a machine in A+W Production, the suitable machine type must
                                           be defined first. The machine type is selected in dialog New machine.
                                           If the corresponding machine type is not available in dialog New machine
                                           please contact A+W Software GmbH.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                     D-15
                 Machine Allocation                                                                             Tutorial




                                      Machines and Machine Allocation
                                      This session shows you how to reflect your machinery in A+W Production and
                                      the properties of the machines.




                                      Fig. D-2     MA editor - Machines


                                      Tab Machines lists all physical machines. Tab Machines therefore reflects your
                                      actual machinery.
                                      Each machine can be identified uniquely with an ID. For each machine, there
                                      is a registration point for the recording of the production data collection (PDC).
                                      You assign each machine a machine type that specifies what kind it is, for ex-
                                      ample Cutting, CNC Center or muntin construction. The machines types are
                                      permanently defined and cannot be changed. A+W Production automatically
                                      creates a logical machine for every machine.
                                      That is, for each machine that actually exists in your plant, you must create a
                                      machine in A+W Production and define its properties.
2.10 / 11-2018




                 D-16                                                           A+W Production Machine Allocation
                 Tutorial                                                                            Machine Allocation




                                                      Machinery                           Represented in
                                                                                         A+W Production

                                                    Cutting table 1,
                                                     Machine type                         Cutting
                                                                                          Cutting table 1
                                                        Cutting


                                                    Cutting table 2,
                                                     Machine type                          Cutting table 2
                                                        Cutting


                                                    CNC machine 1,
                                                     Machine type                         CNC machine 1
                                                     CNC center


                                                    CNC machine 2,
                                                     Machine type                         CNC machine 2
                                                     CNC center


                                                   Drilling machine 1,
                                                     Machine type                        Drilling machine 1
                                                          Drilling


                                                   Drilling machine 2



                                        Fig. D-3       Machines in A+W Production


                                        In this example, no machine is created in A+W Production for drilling machine
                                        2. Thus, the machine is not known to the software and it also cannot be cont-
                                        rolled.

                                        Machine properties
                                        For each machine created in A+W Production, the following properties of the
                                        machine must be specified.
                                        •   Manual operation:
                                            Identifier for machines that do not have automatic loading equipment. This
                                            identification prevents, among other things, that using the manual proces-
                                            sing time there is a split or that items are automatically scheduled on ma-
                                            nual cutting tables.
                                        •   Individual processing:
                                            Identifier for machines whose processings may not be combined, e.g.
                                            – drillings = 0: for two drillings on the same machine, two dates are not
2.10 / 11-2018




                                               determined.
                                            – Screen printing or coatings = 1: for two coatings, two different dates are
                                               not determined, even if they are done on the same machine.


                 A+W Production Machine Allocation                                                                D-17
                 Machine Allocation                                                                               Tutorial




                                      •   Minimum size:
                                          Minimum dimensions for a lite that can be produced on the machine, e.g.
                                          without falling through the rollers.
                                          If you can place small lites on a larger lite, e.g. to print them, do not specify
                                          the size restriction on the machine, but on the logical machine, e.g. as
                                          screen printing with carrier lite.
                                      •   Maximum size:
                                          Maximum dimensions for a lite that can be produced on the machine be-
                                          cause it exceeds the width of the guide rails, the furnace width or the ceiling
                                          height. If you can produce larger lites by unscrewing the side walls on the
                                          processing center and setting up spray protection, for example, do not spe-
                                          cify the size restriction on the machine, but on the logical machine, e.g. as
                                          processing center for extra-large sizes.
                                      •   Thicknesses:
                                          Thickness range in which the machine can work. Other thicknesses cannot
                                          be processed on the machine, e.g. because 3 mm is not supported reliably
                                          and the guides are too narrow for 15 mm.
                                          If a 15 mm lite can be produced by reconstructing the machine, do not
                                          place the size restriction on the machine, bur on the logical machine, e.g.
                                          grinding machine for thick glass.
                                      •   Shapes:
                                          Specification whether the machine can produce only rectangles, only
                                          shapes or both. Consider, for example, that free shapes or arcs cannot be
                                          produced, e.g. for LG cutting.
                                      •   Weight:
                                          Maximum weight of a lite for which the machine is approved. In order to ex-
                                          press that the machine can process the weight but there must be a second
                                          employee ready for handling, enter the restriction for the logical machines,
                                          e.g. one-sider with two people.

                                          Delete machine
                                          Deleting a machine can affect your production! Before you delete a machi-
                                          ne, always make sure that it is no longer used on the shop floor.

                                      Assigning names, IDs, and numbers
                                      For machines of the same type, assign IDs in the same range of hundreds,
                                      e.g. for all cutting tables IDs from 100 to 199. Cutting tables are therefore ea-
                                      sily recognizable on the list. If you have no special number areas for machines,
                                      use the numbering pattern of operational data collection as a guideline.
                                      Always use the same names for machines of the same type, numbering them
                                      all the way through; the eighth cutting table at your plant will therefore be called
                                      Cutting table 8.

                                      Machine restrictions
                                      Depending on their construction, machines can have different restrictions, e.g.
                                      being able to process lites only up to a certain size. The restrictions of the in-
                                      dividual machines can be edited in dialog Machine.
2.10 / 11-2018




                 D-18                                                             A+W Production Machine Allocation
                 Tutorial                                                                                Machine Allocation




                                        Restrictions available in dialog Machine:
                                        •   Minimum thickness
                                        •   Maximum thickness
                                        •   Shapes
                                        •   Coated glass
                                        •   Patterned glass
                                        •   Stepped IG
                                        •   Dimensions
                                        •   AIR
                                        If there are machines which come with further restrictions, additional condi-
                                        tions have to be used to define these restrictions. These conditions can also
                                        contain formulas.
                                         “Conditions and Formulas in Connection with Machine Allocation” on page D-64
                                        Below are some examples of restrictions available in dialog Machine.

                                            Example: Restriction thickness

                                            The restriction Thickness can be set as follows:
                                            • If the machine can process only lites from a thickness of 8 mm upwards,
                                              enter the restriction minimum thickness 8 mm.
                                            • If the machine can process only lites up to a thickness of 15 mm, enter the
                                              restriction maximum thickness 15 mm.


                                            Example: Restriction Shapes

                                            The restriction Shapes can be set as follows:
                                            • No restriction: the machine can process shapes and rectangles, which is
                                              the case for modern cutting tables.
                                            • The machine can only process shapes, e.g. to prevent rectangular lites
                                              from being transferred to a CNC center for grinding.
                                            • The machine cannot process shapes but only rectangles which is the case
                                              for grinding/drilling lines.


                                            Example: Restriction Coated glass

                                            The restriction Coated glass can be set as follows:
                                            • No restriction: the machine can process coated and uncoated lites.
                                            • The machine can only process coated glass.
                                            • The machine can only process uncoated glass.


                                            Example: Restriction Patterned glass

                                            You can set the restriction Patterned glass as follows:
                                            • No restriction: the machine can process patterned glass and glass without
                                              patterns.
2.10 / 11-2018




                                            • The machine can only process patterned glass.
                                            • The machine can only process glass without a pattern.




                 A+W Production Machine Allocation                                                                      D-19
                 Machine Allocation                                                                             Tutorial




                                          Example: Restriction Stepped IG

                                          You can set the restriction Stepped IG as follows:
                                          • No restriction: the machine can process stepped IG and common IG.
                                          • The machine can only process stepped IG.
                                          • The machine can only process common IG.


                                      Size restrictions and lite format
                                      You can define the minimum and maximum size of lites to be processed by a
                                      machine. You should use the machine's direction of movement as a guideline.
                                      The entries for the Width and Height only serve as landmarks; you can also
                                      process lites the width and height of which have been exchanged. The lite
                                      must be aligned by hand on the machine in this case.

                                      Spacer restrictions
                                      This defines whether the machine can process common IG with one spacer or
                                      multiple IG with two spacers. A minimum and a maximum value can be ente-
                                      red for every spacer.

                                      AND-/OR relations
                                      When defining the machine restrictions you have to enter them as logical re-
                                      lations (AND/OR). These are basic relations in the Boolean algebra which
                                      serve to show logical relations.
                                      •   AND relation: If two (or more) statements apply, a statement is true.
                                          Example: A machine can process only lites which are wider than 150 mm
                                          and higher than 200 mm. It follows that:
                                          Width >= 150 mm AND height >= 200 mm.
                                      •   OR relation: If one or the other statement applies, the statement is true.
                                          Example: A machine can process only lites which are wider than 150 mm
                                          or shorter than 3500 mm. It follows that:
                                          Width >= 150 mm OR length <= 3500 mm.
2.10 / 11-2018




                 D-20                                                              A+W Production Machine Allocation
                 Tutorial                                                                           Machine Allocation




                                        Element ID
                                        The element ID is only used for the machine types Line, Cutting, and Bender.
                                        The element ID can be used to distinguish lines, tables, or benders if there are
                                        several machines of the same type.
                                        The tables 1, 2, and 3 for example could get the element IDs TB1, TB2, and
                                        TB3.
                                        The element ID defines the format in which the NC code is issued.

                                        Additional conditions
                                        Additional conditions seriously influence the behavior and the properties of
                                        machines.
                                        If an additional condition is defined, you have to understand its consequences.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                D-21
                 Machine Allocation                                                                         Tutorial




                                      Machine Definition and Management
                                      This session will show you how to define new machines and edit or delete
                                      existing ones.
                                      After entering a machine you have to edit the machine data.
                                      There are the following instructions on this subject.
                                      •   “How to define a machine” on page D-22
                                      •   “How to enter the machine's properties” on page D-23
                                      •   “How to delete a machine” on page D-25

                                          Prerequisite
                                          A new machine can only be entered if a suitable machine type has been
                                          defined, e. g. Cutting, CNC center, Spacer bender, Others.
                                          The machine type catalog is predefined in A+W Production. It appears in a
                                          combo box when you enter a new machine.


                                       How to define a machine
                                      1 Go to Master data > MA > MA editor > Machines > [New].




                                      2 Enter an ID from the number area intended for this machine type, e.g. 180.
                                      3 Enter a name which clearly describes the machine, e.g. Cutting table 8.
                                      4 Choose the appropriate machine type, e.g Cutting.
                                      5 Enter an element ID, e.g. TB8.
                                          You have to enter an element ID for the machine types Line, Table, or Ben-
                                          der. This allows to recognize the machines should there be several of the
                                          same type.
2.10 / 11-2018




                 D-22                                                          A+W Production Machine Allocation
                 Tutorial                                                                          Machine Allocation




                                           Fig. D-4     Example for a new machine


                                        6 Click on [OK] to save the data.
                                           With that, you have entered a new machine. It will appear on the list of Ma-
                                           chines in the MA Editor dialog.
                                           You have to define properties and allocations to describe the machine in
                                           detail.


                                         How to enter the machine's properties
                                        1 Go to Master data > MA > MA editor > Machines.
2.10 / 11-2018




                                           Fig. D-5     MA editor - Machines




                 A+W Production Machine Allocation                                                               D-23
                 Machine Allocation                                                                          Tutorial




                                      2 Select the machine you want to edit.
                                      3 Click on the [Edit].




                                         A

                                                                                            B




                                         A General properties                   B Combo box
                                         Fig. D-6     Machine


                                      4 Add the General properties (A).
                                         When you click on a field you can select data from the combo box (B).
                                         The restrictions in the bottom part of the dialog can be completed later .
                                      5 Confirm by [OK].
                                         With that, you have defined the machine master data.
                                         Machine restrictions will be introduced in a special session.
                                          “Definition and Editing of Machine Restrictions” on page D-26
2.10 / 11-2018




                 D-24                                                           A+W Production Machine Allocation
                 Tutorial                                                                         Machine Allocation




                                         How to delete a machine

                                           Delete machines
                                           Deleting machines in A+W Production can affect your production. Before
                                           you delete a machine, always make sure that it is no longer used.

                                        1 Go to Master data > MA > MA editor > Machines.
                                        2 Tag the machine you want to delete.
                                        3 Click on [Delete].
                                           A security query appears.
                                        4 Confirm this security query by [Yes] to delete the machine once and for all.
                                           The machine data will be deleted.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                              D-25
                 Machine Allocation                                                                             Tutorial




                                      Definition and Editing of Machine Restrictions
                                      In this unit, you will learn how to specify the restrictions for a machine.
                                      There are the following instructions on this subject:
                                      •   “How to edit restrictions regarding the thickness” on page D-26
                                      •   “How to edit the restrictions for shapes, coated glass, patterned glass, and
                                          stepped IG” on page D-28
                                      •   “How to edit the restrictions for sizes and spacers” on page D-30
                                      •   “How to remove the size and spacer restrictions” on page D-31

                                          Restrictions and additional condition at the same time
                                          Active restrictions in connection with the selection of a formula can cause
                                          a conflict.
                                          Restrictions can neutralize each other.

                                          In case of questions please contact the A+W Software GmbH support
                                          team.


                                       How to edit restrictions regarding the thickness
                                      1 Go to Master data > MA > MA editor > Machines.




                                          Fig. D-7     MA editor - Machines
2.10 / 11-2018




                                      2 Select the machine you want to edit.
                                      3 Click on [Edit]:


                 D-26                                                           A+W Production Machine Allocation
                 Tutorial                                                                                 Machine Allocation




                                           A                                                       B




                                           A Activate the restriction                   B Open input field.
                                           Fig. D-8      Restriction - edit thickness


                                        4 Double-click on […] (B).




                                        5 Click on the [Arrow] to enter the value for the minimum thickness.




                                        6 Enter the minimum thickness in millimeters.
2.10 / 11-2018




                                        7 Click on [OK] to save the value.
                                           With that, you have changed the minimum thickness for the machine.



                 A+W Production Machine Allocation                                                                    D-27
                 Machine Allocation                                                                             Tutorial




                                      8 Repeat the steps 4 to 7 to edit the restrictions for the maximum thickness.


                                       How to edit the restrictions for shapes, coated glass, patterned glass,
                                        and stepped IG
                                      1 Go to Master data > MA > MA editor > Machines.
                                      2 Select the machine you want to edit.
                                      3 Click on [Edit]:




                                         A                                                  B




                                         A Activate the restriction shapes        B Open additional checkbox.
                                         Fig. D-9     Restriction - edit shapes


                                      4 Double-click on […] after Shapes ().
                                         An [Arrow] appears.
2.10 / 11-2018




                 D-28                                                             A+W Production Machine Allocation
                 Tutorial                                                                              Machine Allocation




                                        5 Click on the [Arrow] (B) to activate shapes.



                                           A                                            B

                                                        C
                                                                                                   D


                                                                       E
                                                                                                               F


                                           A and B          No restriction. The machine can process rectangles and shapes.
                                           C and D          The machine can only process rectangles.
                                           E and F          The machine can only process shapes.
                                           Fig. D-10     Shape restrictions, combinations of checkboxes


                                        6 Choose the required combination of checkboxes to define the restriction:
                                           •   No restriction (A, B)
                                           •   No shapes (C, D)
                                           •   No rectangles (E, F)
                                        7 Click on the [OK] button to save the shape restrictions.
                                           That way, you have edited the Shapes restriction for this machine.
                                        8 Edit the restrictions for coated glass, patterned glass, and stepped IG in the
                                          same way.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                  D-29
                 Machine Allocation                                                                           Tutorial




                                       How to edit the restrictions for sizes and spacers

                                          Restrictions will be deleted irrevocably
                                          Dimension restrictions are deleted permanently and without security query
                                          if you click the [cross].

                                      1 Go to Master data > MA > MA editor > Machines.
                                      2 Select the machine you want to edit.
                                      3 Click on [Edit]:

                                      s




                                                                                       A




                                          A Edit
                                          Fig. D-11   Restrictions – Edit sizes


                                      4 Click on the [Pen icon] in field Dimensions to open the Size restrictions dia-
                                        log.
2.10 / 11-2018




                 D-30                                                             A+W Production Machine Allocation
                 Tutorial                                                                          Machine Allocation




                                        5 Check the checkboxes of the input fields you want to edit.
                                        6 Fill in the input fields.
                                        7 Click on [OK] to save the amended size restrictions.
                                           That way, you have changed the Dimensions restriction for the machine.
                                           The restriction is shown in field Dimensions as AND/OR relations.




                                        8 Edit the spacer restrictions in the same way.


                                         How to remove the size and spacer restrictions

                                           Deletion of size restrictions
                                           Dimension restrictions are deleted permanently and without security query
                                           if you click the [cross].

                                        1 Go to Master data > MA > MA editor > Machines.
                                        2 Select the machine you want to edit.
                                        3 Click on [Edit].
                                           Dialog Machine appears.
                                        4 Click in the Dimensions area on [X] to remove a restriction.
                                           With that, you have deleted the Size restrictions for this machine.
                                        5 Click on [OK] to save the changes.
                                        6 Delete the spacer restrictions in the same way.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                               D-31
                 Machine Allocation                                                                        Tutorial




                                      Machines Exercises
                                      The following exercises shall help to strengthen your newly acquired know-
                                      ledge.
                                      •   Take a piece and paper and sketch your factory's machinery.
                                      •   Note which machines belong to which machine type.
                                      •   Systematically assign IDs to the machines (number ranges).
                                      •   Note the properties which apply to the machines and whether there are re-
                                          strictions:
                                          – Are there restrictions like e.g. minimum thickness, maximum thickness,
                                              or size restrictions.
                                          – Can the machine process IG or triple IG? Where must these entries be
                                              made?
                                      •   Enter the machines as exercise machines in A+W Production and amend
                                          them to match your machinery.
                                      •   Keep those test machines as a basis for further exercises.


                                      Additional information
                                       Software Reference, “New Machine” auf Seite D-94
                                       Software Reference, “Machine” auf Seite D-95
                                       Software Reference, “Dimension Restrictions” auf Seite D-100
                                       Software Reference, “Spacer Restrictions” auf Seite D-101
2.10 / 11-2018




                 D-32                                                          A+W Production Machine Allocation
                 Tutorial                                                                              Machine Allocation




                                        Logical Machines
                                        Objectives

                                        • The meaning of logical machines in A+W Production and especially in the context
                                          of machine allocation.
                                        • Why do logical machines exist?
                                        • How to assign names and numbers.
                                        • How to manage, define, edit, or delete logical machines.
                                        • When can logical machines be deleted, and when not?


                                        Benefit

                                        • Logical machines represent one machine function. If a machine can be used for
                                          drilling and edgework, two logical machines will be created for this machine in
                                          A+W Production. In the next step, a process can be allocated to the machine
                                          function.
                                        • Among other things, A+W Production barcoding (production data collection)
                                          analyses data of the logical machines, e.g. for statistics.


                                        Note

                                        Logical machines            Logical machines represent a function of a real machine.
                                                                    Logical machines are used for production control and
                                                                    cost calculation.
                                                                    Logical machines are used for production data
                                                                    collection.
                                                                    When you enter a machine, a logical machine will be
                                                                    created automatically.
                                                                    Any number of logical machines can be defined for one
                                                                    (physical) machine.

                                        Allocation                  Logical machines are allocated to processes.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                    D-33
                 Machine Allocation                                                                                Tutorial




                                      Machines and Machine Allocation
                                      Logical machines represent one function of a real machine. The properties of
                                      the machine are applied to the logical machine. The properties of the logical
                                      machine are valid in addition to the properties of the (real) machine.




                                      Fig. D-12     Logical machines


                                      Logical machines are used for:
                                      •   Describing individual machine functions.
                                      •   Allocating processes.
                                      •   Prioritizing processes.
                                      •   Capacity planning and rescheduling.
                                      •   Logical machines distinguish individual machine functions. Thus, e.g. diffe-
                                          rent rates or transition times can be defined for a machine.
                                      •   Statistical evaluations.

                                          Example

                                          You have a CNC machine that can drill, grind, and polish. Define the machine
                                          as CNC machine 1. A+W Production automatically creates a logical machine.
                                          Since the CNC machine has three functions, three logical machines will be
                                          defined.
2.10 / 11-2018




                                          Define this machine and enter the master data for Drilling. Now define to
                                          more logical machines for CNC machine 1; for one of them, enter the master
                                          data for Grinding and for the other, the master data for Polishing.



                 D-34                                                             A+W Production Machine Allocation
                 Tutorial                                                                           Machine Allocation




                                                                                       Logical CNC machine 1
                                                                                       • automatically created
                                                                                       • manually configured
                                                                                       • drilling

                                            Real CNC machine
                                            Functions:                                 Logical CNC machine 2

                                            • drilling                                 • manually created
                                            • grinding                                 • manually configured
                                            • polishing                                • grinding


                                                                                       Logical CNC machine 3
                                                                                       • manually created
                                                                                       • manually configured
                                                                                       • polishing


                                        Fig. D-13    Example: Three logical machines result from one CNC center


                                        The processing times that a logical machine requires for its allocated work pro-
                                        cess are defined as formula in the capacity planning. For this, the separate do-
                                        cumentation for the Capacity planning part is available.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                D-35
                 Machine Allocation                                                                         Tutorial




                                      Definition and Management of Logical Machines
                                      This part of the tutorial will show you how to define new logical machines and
                                      edit or delete existing ones.
                                      There are the following instructions on this subject.
                                      •   “How to define a logical machine” on page D-36
                                      •   “How to edit a logical machine” on page D-38
                                      •   “How to delete a logical machine” on page D-39

                                          Prerequisite
                                          You can define logical machines only after you have entered the correspon-
                                          ding (real) machine.


                                       How to define a logical machine
                                      1 Go to Master data > MA > MA editor > Logical machines.




                                          Fig. D-14   Logical machine selected


                                          A+W Production automatically creates a logical machine for every machi-
                                          ne. All additional logical machines can only be defined based on the exis-
                                          ting one.
2.10 / 11-2018




                                      2 Select the logical machine that shall be used as a basis for the new logical
                                        machine.
                                      3 Click on [New].


                 D-36                                                            A+W Production Machine Allocation
                 Tutorial                                                                        Machine Allocation




                                        4 Enter the ID and the name.
                                        5 Click on [OK] to save the data.




                                           Fig. D-15   New logical machine


                                           With that, you have entered a new logical machine. The new logical ma-
                                           chine is listed on tab Logical machines in the MA editor.
                                           You can now edit the properties of the new logical machine.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                           D-37
                 Machine Allocation                                                                         Tutorial




                                       How to edit a logical machine
                                      1 Go to Master data > MA > MA editor > Logical machines.
                                         Tab Logical machines appears in the MA editor.
                                      2 Select the logical machine you want to edit.
                                      3 Click on [Edit].




                                         Fig. D-16    Logical machine - properties


                                      4 Enter the data for the logical machine, e.g. for a cutting table.
                                      5 Click on [OK] to save the data.
                                         With this, you have defined the master data for the logical machine.
2.10 / 11-2018




                 D-38                                                          A+W Production Machine Allocation
                 Tutorial                                                                          Machine Allocation




                                         How to delete a logical machine

                                           Delete logical machines
                                           A+W Production automatically creates a logical machine for every machine
                                           defined. This automatically created logical machine cannot be deleted.
                                           When a machine is deleted, all related logical machines will be automati-
                                           cally deleted too.

                                           If you delete a logical machine, you delete the function of a machine. This
                                           can cause significant problems in the production process. Make sure that
                                           the logical machine and the machine are not used in production before you
                                           delete them.

                                        1 Go to Master data > MA > MA editor > Logical machines.
                                        2 Select the logical machine you want to delete.
                                        3 Click on [Delete].
                                           A security query appears.
                                        4 Confirm this security query by [Yes] to delete the logical machine once and
                                          for all.
                                           The data will be deleted.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                              D-39
                 Machine Allocation                                                                             Tutorial




                                      Logical Machines - Exercises
                                      The following exercises shall help to strengthen your newly acquired know-
                                      ledge.
                                      •   Define the exercise machines representing the machinery in your factory
                                          or use the exercise machines from the previous session.
                                          – Note the processes that can be executed by the individual machines,
                                             e. g. drilling, grinding, arrissing.
                                          – Create the appropriate logical machines.
                                      •   A toughening furnace can toughen and semi-toughen the lites. Would you
                                          create different logical machines for the two functions? List the benefits and
                                          disadvantages.


                                      Additional information
                                       “Machines Exercises” on page D-32
                                       Software Reference, “New Logical Machine” auf Seite D-103
                                       Software Reference, “Logical Machine” auf Seite D-104
2.10 / 11-2018




                 D-40                                                           A+W Production Machine Allocation
                 Tutorial                                                                                  Machine Allocation




                                        Work Processes
                                        Objectives

                                        •   The meaning of work processes in the context of machinery allocation.
                                        •   How to manage, define, edit, or delete work processes.
                                        •   Why work processes have priorities, and how they can be changed.
                                        •   The relation between work processes, processing types and articles?


                                        Benefit

                                        • A work process fulfils the request to perform a processing step defined in the bill of
                                          materials. This requested process may be polishing or grinding. Based on this
                                          request, the work process defines the special type of polishing or grinding.
                                        • The level of the logical machine establishes the connection between the work
                                          process and the physical machine which is to perform the work process.


                                        Note

                                        Work processes               Work processes bring together the properties of
                                                                     processing type, like e.g. Cutting with the properties of
                                                                     the work piece.
                                                                     Work processes are based on processing types or
                                                                     articles.

                                        Conditions/formulas          Conditions/formulas can also be used to define work
                                                                     processes.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                        D-41
                 Machine Allocation                                                                            Tutorial




                                      Work Processes and Machine Allocation
                                      A work process is defined by a processing type, a processing article, an article
                                      group, and/or an additional condition.
                                       “Processing Types and Processing Articles” on page D-69




                                      Fig. D-17     Work processes


                                      If a processing type has been defined for a work process, e.g. Cutting, this de-
                                      scribes the technical type of processing for this work process. We recommend
                                      using the standard A+W Software GmbH processing type catalog for defining
                                      work processes.
                                      Only create your own processing types if there are no appropriate pre-defined
                                      processing types. You create separate work processes if you can make state-
                                      ments about your production, e.g.:
                                      •   You combine screen printing in dark colors on a particular day of the week
                                          because you then dispose of the solvent (possible campaign planning).
                                      •   The thick lites are ground on machine 1. The thin lites on machine 2, but
                                          they serve one another as substitute machine (selection of the tool)
                                      •   Series lites may only be drilled on the automatic drilling line. If it breaks
                                          down, you must shift the delivery date.
                                      The work process pseudo-processing stands for processings in the BOM that
2.10 / 11-2018




                                      have an informative character, e.g. do not stamp, use gloves, heed tolerance.
                                      So that no scheduling is done for these processings, they are scheduled on a




                 D-42                                                           A+W Production Machine Allocation
                 Tutorial                                                                          Machine Allocation




                                        machine Dummy for informative processings, which has no PDC registration
                                        point and thus also no shift plan.

                                        Processing items on work process
                                        If a processing type has been defined for a work process, e.g. Shape cutting
                                        for laminated glass, you can set off the processing of laminated glass shapes
                                        from the processing of other shapes even before the actual machinery alloca-
                                        tion.




                                        A
                                        B
                                        C




                                        A Article type                         C Article
                                        B Article group
                                        Fig. D-18    Work process – article


                                        You can specify the work process even further by additionally choosing a re-
                                        striction in field Article. The Article type (A) is predefined by A+W Software
                                        GmbH. It includes basic articles, e. g. toughened glass, laminated glass, and
                                        Muntins.


                                        If you select e.g. the processing type Cutting and also the article Toughened
                                        glass, you define a work process for the cutting of toughened glass.
                                        The Article group (B) can be used to choose a production article group you
2.10 / 11-2018




                                        have defined before. For the processing type Cutting for example, you can
                                        choose the article group Glass doors. This way, you have defined a work pro-
                                        cess for the cutting of glass doors.


                 A+W Production Machine Allocation                                                              D-43
                 Machine Allocation                                                                                           Tutorial




                                              Select an Article (C) to allocate a work process to a special article. Enter e. g.
                                              for a work process the processing type Cutting and the article Float 6 mm to
                                              define a work process for the cutting of 6 mm float glass.

                                                 Processing types
                                                 There is a special session on processing types:

                                                  “Processing Types and Processing Articles” on page D-69




                         Work process for cutting:             Work process for                    Work process for
                                                            toughened glass cutting:              Float 6 mm cutting:



                                                               Work process Cutting               Work process Cutting
                              Work process Cutting
                                                                      LAMI                            Float 6 mm



                             Processing type Cutting          Processing type Cutting            Processing type Cutting




                                                                      Catalog:                           Article:
                                                                       LAMI                            Float 6 mm



                 Fig. D-19      Examples of differently defined work processes


                                              Exact definition of work processes
                                              Use the options in dialog Work process in field Article for a detailed definition
                                              of work processes.

                                                 Example 1:

                                                 Laminated glass can only be cut on cutting tables that have two heads or use
                                                 other technologies like e.g. Waterjet.

                                                 The work process Cutting has already been defined for float glass cutting.
                                                 Define a new work process for laminated glass cutting. Select processing
                                                 type Cutting glass type LAMI.


                                                 This defines a work process that takes into account the peculiarities of
                                                 laminated glass cutting and which can only be allocated logical machines
                                                 which can perform this type of processing.
2.10 / 11-2018




                 D-44                                                                    A+W Production Machine Allocation
                 Tutorial                                                                                 Machine Allocation




                                           Example 2, option Article group:

                                           Certain articles are produced only infrequently.


                                           To handle this case, define an article group that includes these rare articles,
                                           then start a campaign. Since campaign planning is based on a work process,
                                           choose the article group containing rare articles for this campaign.

                                           You can thus plan when and how those rarely occurring articles shall be
                                           produced.
                                           Campaigns are described in detail in section Capacity planning.


                                        Non-allocated work processes
                                        A work process is shown in red until it is assigned a logical machine. Always
                                        allocate a logical machine to the work processes. If the corresponding logical
                                        machine has not been defined yet you should allocate Dummy as a logical ma-
                                        chine.
                                         “Allocation of Work Processes” on page D-52

                                        Priority of work processes
                                        Work processes can be moved upwards or downwards on the list. For alloca-
                                        ting work processes, the list is processed from top to bottom. A work process
                                        will be allocated if all conditions allocated to work process are met. The priority
                                        allocated to specialized work processes must therefore always be higher than
                                        the priority allocated to unspecialized work processes.

                                        Several work processes for the same lite
                                        You have got an order for a glass door. This requires the work processes Rec-
                                        tangular grinding, Drilling, and Cut-outs.
                                        Instead of using the more cost-effective rectangular grinding machine for grin-
                                        ding, all three work processes can be performed by the CNC center.
                                        This makes the single work process Rectangular grinding expensive but it sa-
                                        ves time because all three processes can be executed on one machine, right
                                        after another.


                                        You have defined the work process Rectangular grinding on CNC center for
                                        this purpose, to which you have allocated the logical machine CNC center rec-
                                        tangular grinding, with high priority.
                                        To avoid bottlenecks, the work process Rectangular grinding on CNC center
                                        is also allocated to the logical machine Rectangular grinding machine, with low
                                        priority.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                       D-45
                 Machine Allocation                                                                                         Tutorial




                                             If you would produce the glass door on less expensive machines, the produc-
                                             tion flow would look like this:
                                             •   Grinding on the rectangular grinding machine.
                                             •   Then drilling on the automatic drilling machine.
                                             •   Then production of the cut-outs on the CNC center.
                                                 Added to this are 2x handling, 2x washing and the set-up time for the CNC
                                                 center.
                                             All things considered, producing the entire glass door on the CNC center may
                                             therefore be more reasonable.

                                             Additional conditions in work processes
                                             Work processes are not exclusively linked to processing steps. They can also
                                             include additional conditions. A condition can be for example: This work pro-
                                             cess is executed on the CNC center. When you define the work process you
                                             can therefore define the machinery to be used with priority.



                                             An additional condition can also check the bill of materials. Defining such a
                                             condition can therefore be used to control the lite's progress on the shop floor.
                                             The condition could be for instance: If the lite's bill of material includes the pro-
                                             cessing steps Grinding, Drilling, and Cut-out, the lite shall be completely pro-
                                             duced on the CNC center.



                     Bill of                                      Work process                            Logical machine


                     BOM glass door:                              Work process                            Logical machine
                     • grinding
                     • drilling                        Work process Glass door with condition:            Logical machine
                     • cut-out                         If the BOM includes
                                                       Grinding + drilling + cut-out
                     Bill of                           = production on CNC center


                     Bill of                                      Work process                                 CNC center



                 Fig. D-20     Example: An additional condition in the work process queries the bill of material


                                             The example shows another way of controlling the lite's progress on the shop
                                             floor, a work process allocation based on a processing article.


                                             Define the processing article Glass door for example. The processing article
                                             Glass door is executed by the work process Glass door, and the work process
                                             Glass door includes the condition that it is produced on the CNC center.
2.10 / 11-2018




                 D-46                                                                     A+W Production Machine Allocation
                 Tutorial                                                                                        Machine Allocation




                     Processing article Glass door               Work process                               Logical machine


                     Processing article                          Work process                                    CNC center


                     Processing article         Work process Glass door                                     Logical machine
                                                is based on the processing article Glass door
                                                Condition: production on CNC center                         Logical machine
                     Processing article


                                                                 Work process



                 Fig. D-21     Example: Work process allocation based on a processing article


                                                Example: Bottleneck because of an additional condition

                                                The condition defined for the work process Glass door says that glass doors
                                                are produced on the CNC center. The condition can either refer to the bill of
                                                material, or to a processing article.
                                                If there is another order in addition to the order for glass doors, this time e.g.
                                                including shapes, there is going to be a bottleneck at the CNC center.
                                                Solution: Change the priority of the logical machine CNC center so that the
                                                CNC center is no longer the first choice for glass doors. This means that
                                                glass doors are not produced on the CNC center but in individual steps on
                                                the rectangular grinding machine, the automatic drill, and the cutting table for
                                                cut-outs.
                                                While this increases the handling effort for the glass doors it permits to
                                                produce the shapes on the CNC center at the same time.
                                                When the bottleneck has been resolved, the original priorities for the logical
                                                machines must be restored.


                                             Work processes can also be defined for a processing article which makes sen-
                                             se for instance if you want to explicitly add a processing step to the bill of ma-
                                             terial.

                                                Example: Work process based on processing articles

                                                A TG has been coated after which it must be handled with gloves.


                                                In this case, define the processing article Wear gloves! and choose it as the
                                                basis for this work process. In work process allocation, allocate this work
                                                process to the logical machine Dummy.

                                                This way, you have introduced a work process that does not run on any
                                                machine but exists on the shop floor as handle coated TG with gloves.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                               D-47
                 Machine Allocation                                                                     Tutorial




                                      Work process based on processing article only as an exception
                                      Work processes based on processing articles are an exception because
                                      you have to complete and maintain the work process allocation in order to
                                      add new processing articles. The definition of work processes based on
                                      processing articles makes sense only in exceptional cases, like the above
                                      example.
2.10 / 11-2018




                 D-48                                                     A+W Production Machine Allocation
                 Tutorial                                                                             Machine Allocation




                                        Work Process Definition and Management
                                        This session shows you how to define and edit new work processes, and who
                                        to delete them from the list.
                                        There are the following instructions on this subject.
                                        •   “How to define a work process” on page D-49.
                                        •   “This is how to edit the restrictions for a work process” on page D-50.
                                        •   “How to delete a work process” on page D-51

                                            IDs for work processes
                                            Always allocate to a work process the ID of the processing and/or item,
                                            multiplied by 10.
                                            Example: The work process is based on the processing step Arrissing (ID
                                            1000) from the standard processing catalog. In this case, allocate the new
                                            work process the ID 100000.With this system, it is easy to keep proces-
                                            sings, items and work processes apart, but the fact that they belong to-
                                            gether is still apparent.


                                         How to define a work process
                                        1 Go to Master data > MA > MA editor > Work processes > [New].
                                            Dialog New work process appears.
                                        2 Enter the data.




                                            Fig. D-22    New work process


                                        3 Click on [OK] to save the data.
                                            Dialog New work process appears to edit the restrictions.

                                            Work processes in red
                                            In the MA editor, a work process is shown in red until it is assigned a logical
                                            machine. Always allocate a logical machine to the work processes. If the
                                            corresponding logical machine has not been defined yet you should alloca-
                                            te Dummy as a logical machine.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                   D-49
                 Machine Allocation                                                                        Tutorial




                                       This is how to edit the restrictions for a work process
                                      1 Go to Master data > MA > MA editor > Work processes.
                                         Tab Work processes appears.
                                      2 Select the work process you want to edit.
                                      3 Click on [Edit]:




                                         Fig. D-23    Work process - edit restrictions


                                      4 Select the necessary options and corresponding types or articles to define
                                        the work process.
                                         You have edited the work process.
                                      5 Click on [OK] to save the data.
2.10 / 11-2018




                 D-50                                                            A+W Production Machine Allocation
                 Tutorial                                                                             Machine Allocation




                                         How to delete a work process
                                        1 Go to Master data > MA > MA editor > Work processes.
                                            Tab Work processes appears.
                                        2 Select the work process to be deleted.
                                            A work process is shown in red in the MA editor until it is assigned a logical
                                            machine.
                                        3 Click on [Delete].
                                            A security query appears.
                                        4 Click on [Yes] to delete the work process for good.
                                            The data will be deleted.


                                        Work Processes - Exercises
                                        The following exercises shall help to strengthen your newly acquired know-
                                        ledge.
                                        •   Define the exercise machines and the logical machines representing the
                                            machinery in your factory or use the exercise machines and logical exer-
                                            cise machines from the previous sessions.
                                             “Machines Exercises” on page D-32
                                             “Logical Machines - Exercises” on page D-40
                                            – Define an exercise work process Polishing based on the standard pro-
                                                cessing catalog.
                                            – Define the exercise work process handle coated toughened lites with
                                                gloves. The work process shall be based on a processing article.
                                            – Define the exercise work process Laminated glass cutting based on the
                                                standard processing catalog; use an article to define it in closer detail.
                                        •   Take a piece of paper and sketch your factory's machinery, then list the re-
                                            sulting logical machines.
                                            Look at the orders on hand: Which work processes have to be defined in
                                            this situation?


                                        Additional information
                                         Software Reference, “New Work Process” auf Seite D-107
                                         Software Reference, “Work Process” auf Seite D-108
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                  D-51
                 Machine Allocation                                                                                 Tutorial




                                      Allocation of Work Processes
                                      Objectives

                                      •   Introducing and understanding work process allocation
                                      •   Allocating work processes
                                      •   Resolving allocations
                                      •   Changing the priority of logical machines
                                      •   The use of defining priorities for logical machines


                                      Benefit

                                      • Work process allocation serves to allocate logical machines to work processes.
                                        Clever allocation will help to optimize the production costs.


                                      Note

                                      Allocation of work          Work process allocation links logical machines and work
                                      processes                   processes.

                                      Priorities                  Work process allocation serves to define the priorities of
                                                                  logical machines. You therefore define that the specified
                                                                  work process shall be performed on the optimal
                                                                  machine, as cost-effective as possible.

                                      Allocation of work          Work process allocation allows the user to intervene in
                                      processes                   the production process.
2.10 / 11-2018




                 D-52                                                             A+W Production Machine Allocation
                 Tutorial                                                                             Machine Allocation




                                        Flexible Adaptation of Work Processes
                                        Logical machines are allocated to work processes. The sequence, and thus
                                        the priority of the logical machines, can be individually defined for every work
                                        process. You therefore define the priorities of machines in the production pro-
                                        cess.
                                        Work processes tend to be allocated to machines that can perform several
                                        functions like the CNC center for instance, rather than being allocated to more
                                        specialized machines which can perform just one function.
                                        As a result, more work processes are allocated to the expensive CNC center
                                        which will cause a bottleneck sooner or later.


                                        This can be prevented by defining priorities in the allocation of work proces-
                                        ses, and by defining flexibly adaptable work processes.
                                        Define work processes which exactly reflect the individual applications, and al-
                                        locate these work processes to suitable logical machines. This makes sure
                                        that the work processes will be performed by the most cost-effective machine.

                                        Condition in a work process
                                        Work processes can include additional conditions. When you define the work
                                        process you can therefore define the machinery to be used with priority.


                                        An additional condition can also check the bill of materials. The condition could
                                        be for instance: If the lite's bill of material includes the processing steps Grin-
                                        ding, Drilling, and Cut-out, the lite shall be completely produced on the CNC
                                        center.
                                        Defining such a condition can therefore be used to control the lite's progress
                                        on the shop floor.

                                           Always allocate work processes
                                           A work process is shown in red until it is assigned a logical machine. Al-
                                           ways allocate a logical machine to the work processes. If the correspon-
                                           ding logical machine has not been defined yet you should allocate Dummy
                                           as a logical machine.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                   D-53
                 Machine Allocation                                                                                         Tutorial




                     Bill of                                      Work process                            Logical machine


                     BOM glass door:                              Work process                            Logical machine
                     • grinding
                     • drilling                        Work process Glass door with condition:            Logical machine
                     • cut-out                         If the BOM includes
                                                       Grinding + drilling + cut-out
                     Bill of                           = production on CNC center


                     Bill of                                      Work process                                 CNC center



                 Fig. D-24     Example: An additional condition in the work process queries the bill of material


                                             The example shows another way of controlling the lite's progress on the shop
                                             floor, a work process allocation based on a processing article.


                                             Define the processing article Glass door for example. The processing article
                                             Glass door is executed by the work process Glass door. The condition for the
                                             work process Glass door is that it is produced by the CNC center.



                    Processing article Glass door                Work process                             Logical machine


                    Processing article                           Work process                                  CNC center


                    Processing article           Work process Glass door                                  Logical machine
                                                 is based on the processing article Glass door
                                                 Condition: production on CNC center                      Logical machine
                    Processing article


                                                                 Work process



                 Fig. D-25     Example: Work process allocation based on a processing article
2.10 / 11-2018




                 D-54                                                                     A+W Production Machine Allocation
                 Tutorial                                                                                        Machine Allocation




                             A




                                                                                                                         B
                                                                                                                         C




                 A Newly defined work processes                             B Logical machine: rectangular grinder
                                                                            C Logical machine: CNC shape grinding
                 Fig. D-26       Example: Flexibly adapted work process allocation


                                                  Example: Flexibly adapted work process allocation

                                                  You have got a rectangular grinding machine and a CNC center on your shop
                                                  floor. Both can execute the processing step Grinding.
                                                  • The list of work processes includes the work process Rectangular grinding
                                                    which is used for all rectangular lites. In work process allocation, the work
                                                    process Rectangular grinding is allocated to the Rectangular grinder. It
                                                    has got top priority.
                                                  • The list of work processes includes the work process Shape grinding
                                                    which is used for all shapes. In work process allocation, the work process
                                                    Shape grinding is allocated to the CNC center.
                                                  • The CNC center is also allocated to the work process Rectangular
                                                    grinding, albeit with a lower priority.
                                                  With these settings, rectangular lites will be ground by the more cost-effective
                                                  rectangular grinder. In case of a bottleneck, rectangular lites will also be
                                                  ground by the CNC center.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                               D-55
                 Machine Allocation                                                                                       Tutorial




                             A

                             B




                 A Work process: Rectangular grinding                   B Work process: Shape grinding
                 Fig. D-27    Example: Flexibly adapted work process allocation


                                           If a lite is to undergo several work processes, it may be reasonable to accept
                                           slightly higher costs for a single work process. The number of lites to be pro-
                                           duced is usually the crucial factor.

                                               Example: Several work processes for the same lite

                                               To produce a glass door the work processes Rectangular grinding, Drilling, and
                                               Cut-outs are required.
                                               Instead of using the more cost-effective rectangular grinding machine for grinding,
                                               all three work processes can be performed by the CNC center. This makes the
                                               single work process Rectangular grinding expensive but it saves time because all
                                               three processes can be executed on one machine, right after another.
                                               You have defined the work process Rectangular grinding on CNC center for this
                                               purpose, to which you have allocated the logical machine CNC center rectangular
                                               grinding, with high priority.
                                               To avoid bottlenecks, the work process Rectangular grinding on CNC center is
                                               also allocated to the logical machine Rectangular grinding machine, with low
                                               priority. It has got top priority.
                                               The production process on cheaper machines look like:
                                               • Grinding on the rectangular grinding machine.
                                               • Drilling on the automatic drilling machine.
                                               • Production of the cut-outs on the CNC center.
2.10 / 11-2018




                                                 Added to this are 2x handling, 2x washing and the set-up time for the CNC
                                                 center.




                 D-56                                                                   A+W Production Machine Allocation
                 Tutorial                                                                               Machine Allocation




                                      A




                                                                                                                          B




                 C




                                                                                                    D




                 A Work process: Rectangular grinding on CNC center. C Work process: Rectangular grinding on CNC center.
                 B Logical machine: CNC center rectangular grinding. D Logical machine: rectangular grinder.
                 Fig. D-28    Example: Several work processes for the same lite


                                           This example shows that the work process Rectangular grinding on CNC cen-
                                           ter has been allocated the logical machine CNC center rectangular grinding
                                           with top priority. The logical machine Rectangular grinder was also allocated
                                           with a lower priority to help prevent bottlenecks. As with the example of several
2.10 / 11-2018




                                           work processes for the same machine, producing the entire glass door on the
                                           CNC center is therefore more reasonable.




                 A+W Production Machine Allocation                                                                    D-57
                 Machine Allocation                                                                            Tutorial




                                      Allocation of Work Processes and Logical Machi-
                                      nes
                                      This session is about allocating logical machines to work processes, separa-
                                      ting work processes and logical machines, and changing the priorities of logi-
                                      cal machines.
                                      There are the following instructions on this subject.
                                      •   “How to allocate a logical machine to a work process” on page D-58.
                                      •   “How to separate logical machines from work processes” on page D-60.
                                      •   “How to change a logical machine's priority” on page D-61.


                                       How to allocate a logical machine to a work process
                                      1 Go to Master data > MA > MA editor > Work process allocation.
                                          Tab Work process allocation appears.
                                      2 Select the work process and the logical machine you want to allocate to
                                        each other.




                                          Fig. D-29   Work process and logical machine selected


                                      3 Click on the arrow pointing to the right to allocate the logical machine to the
                                        work process.
2.10 / 11-2018




                                          The logical machine has been allocated to the work process and appears
                                          on the list below the work process, highlighted in gray.



                 D-58                                                           A+W Production Machine Allocation
                 Tutorial                                                                            Machine Allocation




                                           Fig. D-30    Work process and logical machine allocated


                                        4 Click on [Accept] to save the data.
                                           The allocation will be saved.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                               D-59
                 Machine Allocation                                                                            Tutorial




                                       How to separate logical machines from work processes
                                      1 Go to Master data > MA > MA editor > Work process allocation.
                                         Tab Work process allocation appears.
                                      2 Click on the [+] for the work process.
                                         The view opens and the logical machines allocated to the work process are
                                         listed.
                                      3 Select the logical machine you want to remove.




                                         Fig. D-31    Separating work process and logical machine


                                      4 Click on the arrow pointing right to separate the logical machine from the
                                        work process.
                                      5 Click on [Accept] to save the changes.

                                         Logical machine still in use
                                         If an assignment should be removed that is still in use, it is deactivated au-
                                         tomatically. Deactivated assignments are depicted in italics and with an ap-
                                         propriate icon.

                                         Please note, if a deactivated logical machine represents an alternative for
                                         a work process in an existing order but this assignment has been deactiva-
2.10 / 11-2018




                                         ted in the meantime, this alternative is offered during the scheduling now




                 D-60                                                          A+W Production Machine Allocation
                 Tutorial                                                                            Machine Allocation




                                           as before (this cannot be avoided due to the internal data structure). Only
                                           with a repetition of the MZO for this order is the deactivation taken into con-
                                           sideration.


                                         How to change a logical machine's priority
                                        1 Go to Master data > MA > MA editor > Work process allocation.
                                           Tab Work process allocation appears.
                                        2 Click on the [+] for a work process to view the allocated logical machines.

                                           Show all logical machines
                                           You can view all allocated logical machines by checking the checkbox
                                           [Open all].

                                        3 Select the logical machine the priority of which you want to change.
                                        4 Click on the arrow up or arrow down to raise or lower the priority.




                                           Fig. D-32    Changing the priority of logical machines


                                           The logical machine will be moved further up or down the list depending on
                                           its new priority.
                                        5 Click on [Accept] to adopt the changes.
                                           The new priority will be saved.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                  D-61
                 Machine Allocation                                                                          Tutorial




                                      Work Process Allocation - Exercises
                                      The following exercises shall help to deepen your newly acquired knowledge.
                                      •   For test purposes, define exercise machines, logical exercise machines,
                                          and exercise work processes reflecting your machinery, or use the exercise
                                          machines, logical exercise machines, and exercise work processes from
                                          previous sessions:
                                           “Machines Exercises” on page D-32
                                           “Logical Machines - Exercises” on page D-40
                                           “Work Processes - Exercises” on page D-51
                                          – Allocate the logical "test" machines and work processes.
                                          – Try various scenarios and define priorities to execute work processes
                                              on the most cost-effective machine to run several work processes on a
                                              CNC center.
                                      •   Consider the actual situation of your machinery and the machines, logical
                                          machines, and work processes defined.
                                          Make a note of which work process allocation is practical for the orders on
                                          hand and which priorities have to be defined to achieve the optimum re-
                                          sults.


                                      Additional information
                                       Software Reference, “New Work Process” auf Seite D-107
                                       Software Reference, “Work Process” auf Seite D-108
2.10 / 11-2018




                 D-62                                                          A+W Production Machine Allocation
                 Tutorial                                                                               Machine Allocation




                                        Conditions, Formulas, Restrictions
                                        Objectives

                                        • The use of formulas and conditions
                                        • Selecting formulas and conditions
                                        • The difference of formulas and conditions and their meaning


                                        Benefit

                                        • Formulas and restrictions are used to define machines, logical machines, and work
                                          processes in closer detail.


                                        Note

                                        Formulas                   Formulas are used in connection with machines, logical
                                                                   machines, and work processes.
                                                                   Formulas are predefined or can be defined by means of
                                                                   the graphic formula editor or the text formula editor.
                                                                   Formulas are used to define restrictions for machines,
                                                                   logical machines, and work processes.
                                                                   Formulas are restrictions or conditions which can be
                                                                   expressed in the database language SQL.

                                        Formula editor             The formula editor is a tool that enables the user to
                                                                   define restrictions of his own.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                     D-63
                 Machine Allocation                                                                              Tutorial




                                      Conditions and Formulas in Connection with Machi-
                                      ne Allocation
                                      This session shows you how to select formulas/conditions.
                                      Machine allocation can be completed by formulas and conditions for machi-
                                      nes, logical machines, and work processes. The terms 'restrictions' and 'con-
                                      ditions' are often used in connection with formulas. In A+W Production,
                                      formulas, restrictions, and conditions are related as follows:
                                      •   Machines, logical machines, and work processes have certain properties
                                          which are often restrictive. Cutting tables for instance can handle lites only
                                          up to a certain size.
                                          The Machine dialog offers predefined fields for some of the most common
                                          restrictions.
                                          The values entered there will be saved as a formula in the master data of
                                          the machine, logical machine, or work process.
                                      •   Apart from that, the field Additional condition allows to define one's own for-
                                          mulas. You are therefore free to define facts and circumstances which
                                          match your production precisely.

                                          Definition of formulas
                                          In case of questions on how to define or amend formulas please contact
                                          the A+W Software GmbH support team.

                                          There is a separate tutorial on formula definition and management.
2.10 / 11-2018




                 D-64                                                            A+W Production Machine Allocation
                 Tutorial                                                                             Machine Allocation




                                        Select a Condition
                                        You can select a condition in the properties of the machines, logical machines
                                        or work processes. You edit the formulas for a condition in the formula editor.
                                         “Select a Formula for the Processing Time of a Logical Machine” on page D-66


                                         How to select a condition
                                        1 Go to Master data > MA > MA editor > Logical machines.
                                           In this example, the condition for a logical machine is set up. The descrip-
                                           tion applies analogously for machines and work processes.
                                        2 Select the logical machine and click [Edit].
                                        3 Click the [magnifying glass] in the Additional condition area in order to se-
                                          lect a condition.




                                           Fig. D-33    Select a condition


                                        4 Select the condition you want to adopt.
                                           If a formula is created for the condition, the content is displayed in the Text
                                           field.
                                        5 Click on [OK] to adopt the condition.
                                           The designation is displayed in the Additional condition area.




                                        6 Click on [OK] to save the data.
                                           In order to edit the formula, you must change to the formula editor.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                  D-65
                 Machine Allocation                                                                             Tutorial




                                      Select a Formula for the Processing Time of a Logi-
                                      cal Machine
                                      You can select a formula for processing duration directly in the properties of
                                      the logical machines. You edit the formulas for a condition in the formula editor.
                                      Alternatively, the processing duration of a logical machine can also be created
                                      or edited in the A+W Production capacity planning.


                                       How to select a formula for the processing time
                                      1 Go to Master data > MA > MA editor > Logical machines.
                                      2 Select the logical machine and click [Edit].




                                         A                                              B




                                         A Processing time                      B Formula selection
                                         Fig. D-34     Logical machine


                                      3 Click on […] (B).
2.10 / 11-2018




                 D-66                                                           A+W Production Machine Allocation
                 Tutorial                                                                           Machine Allocation




                                           Fig. D-35    Formula selection


                                        4 Go to dialog Formula selection and select a formula.
                                        5 Click on [OK] to adopt the formula in the properties of the logical machine.
                                           The formula is displayed in the Processing duration line.
                                        6 Click on [OK] to save the data.
                                           You can edit the formula by clicking [Edit]. There is a detailed description
                                           of the formulas in the documentation for the Formulas part.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                D-67
                 Machine Allocation                                                                         Tutorial




                                      Selection of Conditions - Exercises
                                      The following exercises shall help to strengthen your newly acquired know-
                                      ledge.
                                      •   Make a note of the machine allocation dialogs in which you can select con-
                                          ditions.
                                      •   Take a piece of paper and sketch your factory's machinery with all the ma-
                                          chines, logical machines, and work processes. Or use your existing notes:
                                           “Machines Exercises” on page D-32
                                           “Logical Machines - Exercises” on page D-40
                                           “Work Processes - Exercises” on page D-51
                                           “Work Process Allocation - Exercises” on page D-62
                                          – Which conditions are practical for your machinery and the orders on
                                            hand?
                                          – Which effects would the conditions have on the other areas of machine
                                            allocation?


                                      Additional information
                                       Software Reference, “Select a Condition” auf Seite D-102
                                       Software Reference, “Select Conditions” auf Seite D-114
2.10 / 11-2018




                 D-68                                                          A+W Production Machine Allocation
                 Tutorial                                                                                 Machine Allocation




                                        Processing Types and Processing Artic-
                                        les
                                        Objectives

                                        • Definition of processing types in A+W Production and especially in connection with
                                          machine allocation
                                        • Defining, editing and deleting processing types
                                        • The reason why processing types cannot be deleted
                                        • The meaning of processing articles in A+W Production and especially with regard
                                          to machine allocation
                                        • Defining, editing and deleting processing articles


                                        Benefit

                                        • Work processes can be defined based on processing types or processing articles.
                                        • If a processing type has been defined for a work process, it describes the technical
                                          type of processing, e.g. Cutting.
                                        • If a processing article has been defined, it describes the technical type of
                                          processing, but more detailed than the processing type. A processing article is
                                          used to define a work process e.g. as Bevelling.


                                        Note

                                        Processing types            Processing types describe the technical type of
                                                                    processing.
                                                                    Processing types are processing steps defined by the
                                                                    user. In addition to that, there is the predefined catalog
                                                                    from A+W Software GmbH.

                                        Processing article          Processing articles define - in closer detail than the
                                                                    processing type - the technical type of processing.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                        D-69
                 Machine Allocation                                                                            Tutorial




                                      Processing Types and Machine Allocation
                                      The processing type describes the technical type of processing. It defines for
                                      example if this is Cutting, Assembly, Arrissing, Grinding, or Packing.
                                      Work processes are based on processing types. The work process unites the
                                      properties of the work piece and those of the processing type.



                                         Processing type
                                         Arrissing


                                         Processing type
                                         Cutting
                                                                                                     Work
                                                                   New work process
                                                                                                     process
                                         Processing type
                                         Grinding


                                         Processing type
                                         Polishing



                                      Fig. D-36    Processing type as the basis for a work process


                                      Processing types are predefined by A+W Software GmbH but can also be de-
                                      fined by the user.




                                      Fig. D-37    Processing types
2.10 / 11-2018




                 D-70                                                           A+W Production Machine Allocation
                 Tutorial                                                                                  Machine Allocation




                                        Processing Articles and Machinery Allocation
                                        Processing articles refer to processing types. Processing articles can be used
                                        to describe processing types in closer detail. For the processing type Grinding
                                        for instance, you can define the processing articles Bevelling, Mitres, Groo-
                                        ving, Frosting, and Rounded corners to describe the technical process.
                                        Since processing articles refer to the corresponding processing type, amend-
                                        ments can be made centrally. When you change the setting Count processing
                                        steps for the processing type Grinding for instance, this setting also changes
                                        for all related processing articles like Bevelling, Mitre, Grooving, Frosting, and
                                        Rounded corners.



                                            Processing article
                                            Mitre



                                            Processing article
                                            Bevelling
                                                                           New work                 Work process
                                                                           process                  Bevelling

                                            Processing article
                                            Grooving



                                            Processing article
                                            Frosting



                                        Fig. D-38     Processing articles as the basis of a work process


                                        The example shows how work processes can be defined based on processing
                                        articles. The work process unites the properties of the work piece and those of
                                        the processing article.
                                        You can define processing articles of your own.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                     D-71
                 Machine Allocation                                                               Tutorial




                                      Fig. D-39   Processing article:
2.10 / 11-2018




                 D-72                                                   A+W Production Machine Allocation
                 Tutorial                                                                           Machine Allocation




                                        Definition and Management of Processing Types
                                        This session will tell you how to define, edit, or delete processing types.
                                        There are the following instructions on this subject.
                                         “How to define a processing type” on page D-73
                                         “How to edit a processing type” on page D-74
                                         “How to delete a processing type” on page D-75

                                            Standard catalog of processing types
                                            A+W Production offers a standard catalog of processing types. They have
                                            got four-digit numbers and must not be amended or deleted by the user.
                                            You can define additional processing types. We recommend to use the ap-
                                            propriate processing type from the standard catalog as a basis.


                                         How to define a processing type
                                        1 Go to Master data > Processings > Processing types.

                                                                       B




                                        A




                                                                                                                      C




                                        A Processing type to be used as a basis B Define processing
                                          for the new processing type           C Processing fields
                                        Fig. D-40    Define a processing type
2.10 / 11-2018




                                        2 Select the processing type that shall be used as a basis for the new pro-
                                          cessing type (A).


                 A+W Production Machine Allocation                                                                    D-73
                 Machine Allocation                                                                                Tutorial




                                            3 Click on [New] (B).
                                               The input fields (C) are released.
                                            4 Enter the data.
                                                Software Reference, “Processing Types” auf Seite D-123
                                            5 Click on [Save] to save the new processing type.
                                               You have defined a new processing type. You can now edit it further if re-
                                               quired.
                                               Click on the [Reject] button to abort the process without saving the data.


                                             How to edit a processing type
                                            1 Go to Master data > Processings > Processing types.


                                   B




                 A




                                                                        J




                                                                                                                       C




                 A Processing type to be edited                        C Released fields
                 B Release fields for editing
                 Fig. D-41    Editing a processing type.


                                            2 Select the processing type you want to edit (A).
                                            3 Click on [Change] (B).
                                               The input fields for the processing type - except the ID - are released and
                                               can be edited (C).
2.10 / 11-2018




                                                Software Reference, “Processing Types” auf Seite D-123
                                            4 Enter the data.



                 D-74                                                               A+W Production Machine Allocation
                 Tutorial                                                                             Machine Allocation




                                        5 Click on [Save] to save the changes.


                                           Click on [Reject] to abort the process without saving the data


                                         How to delete a processing type

                                           Prerequisite
                                           Processing types cannot be deleted if they are allocated to a processing ar-
                                           ticle. An error message appears in this case.
                                           Resolve the allocation before you delete a processing type.

                                            “How to undo the allocation of a processing type and a processing article” on
                                             page D-79
                                        1 Go to Master data > Processings > Processing types.
                                           Dialog Processing types appears.
                                        2 Select the processing type to be deleted.
                                        3 Click on [Delete].
                                           A security check appears.
                                        4 Click on [Yes] to delete the processing type.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                   D-75
                 Machine Allocation                                                                                     Tutorial




                                            Definition and Management of Processing Articles
                                            This session will show you how to define, edit, and delete processing articles
                                            and how to undo the allocation of a processing type and a processing article.
                                            There are the following instructions on this subject.
                                             “How to define a processing article” on page D-76
                                             “How to edit a processing article” on page D-78
                                             “How to undo the allocation of a processing type and a processing article” on
                                              page D-79
                                             “How to delete a processing article” on page D-79


                                             How to define a processing article
                                            1 Go to Master data > Processing > Processing articles.


                                                   B




                 A




                                                                                                                              C




                 A Processing article that serves as a basis            B Defining a processing article.
                                                                        C Released fields
2.10 / 11-2018




                 Fig. D-42    Defining a processing article.




                 D-76                                                                  A+W Production Machine Allocation
                 Tutorial                                                                            Machine Allocation




                                        2 Select the processing article to be used as a basis for the new processing
                                          article (A).
                                        3 Click on [New] (B).
                                           The input fields (C) are released and can be edited.
                                        4 Enter the data.
                                            Software Reference, “Processing Articles” auf Seite D-125
                                        5 Click on [Save] to save the processing article.
                                           You have defined a new processing article. You can now edit it further if re-
                                           quired.
                                           Click on [Reject] to abort the process without saving the data.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                D-77
                 Machine Allocation                                                                                   Tutorial




                                              How to edit a processing article
                                             1 Go to Master data > Processing > Processing articles.


                                     B




                 A




                                                                                                                           C




                 A Processing article to be edited.                     C Released fields
                 B Release fields for editing.
                 Fig. D-43     Defining a processing article.


                                             2 Select the processing article (A) you want to edit.
                                             3 Click on [Change] (B).
                                                 The input fields (C) are released and can be edited.
                                                  Software Reference, “Processing Articles” auf Seite D-125
                                             4 Enter the data.
                                             5 Click on [Save] to save the changes.
2.10 / 11-2018




                                                 [Reject] can be used to abort the process without saving the data.




                 D-78                                                                  A+W Production Machine Allocation
                 Tutorial                                                                          Machine Allocation




                                         How to undo the allocation of a processing type and a processing
                                          article
                                        1 Go to Master data > Processing > Processing articles.
                                           Dialog Processing articles appears.
                                        2 Select the processing article that shall be allocated to another processing
                                          type.
                                           You can sort the list of processing articles by Processing type to make se-
                                           arching for the appropriate processing article easier.
                                        3 Click [Change].
                                           The input fields of the processing article are released and can be edited.
                                        4 Select another processing type from combo box Processing type.
                                        5 Click on [Save] to save the processing article.
                                           [Reject] can be used to abort the process without saving the data.


                                         How to delete a processing article
                                        1 Go to Master data > Processing > Processing articles.
                                           Dialog Processing articles appears.
                                        2 Select the processing article to be deleted.
                                        3 Click on [Delete].
                                           A security check appears.
                                        4 Click on [Yes] to delete the processing article.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                              D-79
                 Machine Allocation                                                                             Tutorial




                                      Machine Allocation - Exercises
                                      The following exercises shall help to deepen your newly acquired knowledge.
                                      Enter the following master data:
                                      •   Define an exercise machine, Drilling. Enter the following restrictions for the
                                          drill:
                                          – The drill can process only lites from a thickness of 10 mm upwards, up
                                              to a thickness of 20 mm.
                                          – The machine cannot process shapes.
                                          – The machine can process lites with and without patterns.
                                      •   Define an exercise machine Line. Enter the following restrictions for the
                                          line:
                                          – The machine can process stepped and common IG.
                                          – The minimum lite size is 200 x 300 mm.
                                          – The maximum lite size is 2500 x 4000 mm.
                                          – The machine can process triple IG without size restrictions.
                                          – Enter an additional condition. Which effects can an additional condition
                                              have on the machine?
                                      •   Define an exercise machine CNC center.
                                      •   The CNC center shall include two logical machines for the processing
                                          steps Drilling and Polishing.
                                      •   Define an exercise cutting table where the lites are put upright onto the ma-
                                          chine.
                                      •   Define an exercise work process, Drilling.
                                      •   Allocate the drill and the CNC center to the work process. The drill shall
                                          have top priority.
                                      •   Define an exercise work process Drilling on CNC center and allocate it to
                                          the CNC center with top priority. Allocate the drill to this work process with
                                          a lower priority, in case of bottlenecks.
                                      •   Define an exercise work process based on the processing article.
                                      •   Define your own exercise processing type Drilling.
                                      •   Amend the work processes from this exercise so that they are based on
                                          your own exercise processing type Drilling.


                                      Additional information
                                       “Machines” on page D-15
                                       “Logical Machines” on page D-33
                                       “Work Processes” on page D-41
                                       “Allocation of Work Processes” on page D-52
                                       “Conditions, Formulas, Restrictions” on page D-63
                                       “Processing Types and Processing Articles” on page D-69
2.10 / 11-2018




                 D-80                                                           A+W Production Machine Allocation
                 Tutorial                                                                   Machine Allocation - Buttons




                                        Machine Allocation - Buttons
                                        Button       Meaning

                                                     Definition of master data.


                                                     Edit an entry on the list.


                                                     Edit an entry on the list.


                                                     Delete an entry from the list.


                                                     Adopt changes.


                                                     Save data.

                                                     Close the dialog without adopting the changes.


                                                     Move elements upwards or downwards on the list.

                                                     Allocate elements, undo the element allocation.

                                                     Define restrictions for a machine, delete the defined restrictions.

                                                     Select additional restrictions.

                                                     Delete restrictions


                                                     Adopt changes.


                                                     Do not adopt changes.


                                                     An AND relation is added to the graphics editor.


                                                     An OR relation is added to the graphics editor.


                                                     Delete the selected relation from the graphics editor.


                                                     Open a dialog to adjust columns in the window.


                                                     Reset changes.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                     D-81
                 Machine Allocation - Buttons                             Tutorial
2.10 / 11-2018




                 D-82                           A+W Production Machine Allocation
Machine Allocation              D

                 Software Reference




                A+W Production
                 Software Reference                                                                Machine Allocation




                                        Machine Allocation
                                        Machine allocation (MA) allocates the existing machinery to work processes,
                                        taking into account machine restrictions and instructions to increase produc-
                                        tivity. Machine manufacturers' check programs can also be integrated for as-
                                        certaining the feasibility of allocations.
                                        This section provides information on the following subjects:
                                        •   “MA Editor” on page D-86
                                        •   “New Machine” on page D-94
                                        •   “Machine” on page D-95
                                        •   “Dimension Restrictions” on page D-100
                                        •   “Spacer Restrictions” on page D-101
                                        •   “Select a Condition” on page D-102
                                        •   “New Logical Machine” on page D-103
                                        •   “Logical Machine” on page D-104
                                        •   “Formula Selection” on page D-106
                                        •   “New Work Process” on page D-107
                                        •   “Work Process” on page D-108
                                        •   “New Machine Type” on page D-110
                                        •   “Machine Type” on page D-111
2.10 / 11-2018




                 A+W Production Machine Allocation                                                              D-85
                 Machine Allocation                                                             Software Reference




                                      MA Editor
                                      Master data > MA > MA editor.
                                      The MA editor is used to manage machines, logical machines, and work pro-
                                      cesses. You also allocate machines to work processes.
                                      The MA Editor offers the following tabs:
                                      •   “MA Editor - Machines” on page D-87
                                      •   “MA Editor – Logical Machines” on page D-88
                                      •   “MA Editor – Work Processes” on page D-90
                                      •   “MA Editor – Work Process Allocation” on page D-91
                                      •   “MA Editor – Machine Types” on page D-93
2.10 / 11-2018




                 D-86                                                            A+W Production Machine Allocation
                 Software Reference                                                                   Machine Allocation




                                        MA Editor - Machines
                                        Master data > MA > MA editor > Machines.




                                        Fig. D-44    MA editor - Machines


                                        This tab serves to define new machines and edit or delete existing ones.
                                         Tutorial, “Machine Definition and Management” on page D-22
                                         “Machine” on page D-95

                                        ID Freely selectable ID.

                                        Name Machine name

                                        Type Machine type allocated to the machine. Machine types in general (e.g.:
                                        machine types can be Cutting, Edgework, or Bender.

                                           Machine types
                                           The machine type catalog is predefined in A+W Production. It appears in a
                                           combo box when you enter a new machine.
                                           To change the machine type catalog please contact the support team of
                                           A+W Software GmbH.

                                        Registration point Registration point allocated to the machine. The registra-
2.10 / 11-2018




                                        tion point is required for capacity planning as well as for shop floor data collec-
                                        tion.



                 A+W Production Machine Allocation                                                                   D-87
                 Machine Allocation                                                              Software Reference




                                      Element ID Freely selectable element identification. Only used for the ma-
                                      chine types Line, Table, and Bender.

                                         Delete machines
                                         A+W Production automatically creates a logical machine for every machine
                                         defined. Further logical machines can be defined.
                                         When a machine is deleted, all related logical machines will be automati-
                                         cally deleted too.
                                         Attention: Deleting a machine may cause a production stop.


                                      MA Editor – Logical Machines
                                      Master data > MA > MA editor > Logical machines.




                                      Fig. D-45    MA editor – Logical machines


                                      This tab serves to define logical machines and edit or delete existing logical
                                      machines.
                                      A+W Production automatically creates a logical machine for every machine
                                      defined. In addition to that, any number of logical machines can be defined for
                                      a (real) machine.
                                      Logical machines represent just one machine function. For a CNC center that
                                      can drill, grind, and polish glass, three logical machines are defined: One for
2.10 / 11-2018




                                      the processing step Drilling, one for the processing step Grinding, and one for
                                      the processing step Polishing.



                 D-88                                                             A+W Production Machine Allocation
                 Software Reference                                                                 Machine Allocation




                                        The automatically defined logical machine cannot be deleted manually. If ad-
                                        ditional logical machines have been defined, these can be deleted however.
                                        When the machine is deleted from the Machine list, all related logical ma-
                                        chines will be deleted too.
                                         Tutorial, “Definition and Management of Logical Machines” on page D-36
                                         “Logical Machine” on page D-104

                                        [New] Opens the New logical machine dialog with which another logical ma-
                                        chine of the same type (as the selected logical machine) can be defined. The
                                        [New] button is active only if a logical machine is selected on the list.
                                         “New Logical Machine” on page D-103

                                        ID Machine ID.

                                        Machine Name of the machine the master data of which were selected for
                                        this logical machine.

                                        ID Freely selectable ID for the logical machine.

                                        Name Freely selectable name for the logical machine.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                 D-89
                 Machine Allocation                                                                Software Reference




                                      MA Editor – Work Processes
                                      Master data > MA > MA editor > Work processes.




                                      Fig. D-46    MA editor – Work processes


                                      This tab serves to define new work processes and edit or delete existing ones.
                                      A work process is shown in red until it is assigned a logical machine. Always
                                      allocate a logical machine to the work processes. If the corresponding logical
                                      machine has not been defined yet you should allocate Dummy as a logical ma-
                                      chine.
                                       Tutorial, “Work Process Definition and Management” on page D-49
                                       “Work Process” on page D-108

                                      ID Freely selectable ID for the work process.

                                      Name Name of the work process.

                                      Additional condition Condition assigned to the work process.

                                      [Priority] Move elements upwards or downwards on the list. The higher a
                                      work process's position on the list, the higher its priority in machine allocation.
                                      Based on the priority, A+W Production determines the work process to be giv-
2.10 / 11-2018




                                      en priority for economic reasons.




                 D-90                                                           A+W Production Machine Allocation
                 Software Reference                                                                   Machine Allocation




                                           Delete work processes
                                           Work processes can be deleted from the list only if they are not allocated
                                           to a logical machine.
                                           To delete a work process, first remove the machine allocation.


                                        MA Editor – Work Process Allocation
                                        Master data > MA > MA editor > Work process allocation.




                                        Fig. D-47    MA editor – Work process allocation


                                        The tab serves to allocate logical machines to the work processes.
                                         Tutorial, “Allocation of Work Processes” on page D-52
                                         “Work Process” on page D-108

                                        Work processes List of defined work processes.

                                        Machines List of defined logical machines.

                                        [Priority] Move logical machines upwards or downwards on the list. The
                                        higher a machine's position on the list, the higher its priority in machine alloca-
                                        tion. Logical machines with high priority will be preferred by A+W Production
                                        for economic reasons.
2.10 / 11-2018




                                        [Allocation] Allocate machines to work processes by selecting a machine
                                        and a work process and click on the arrow pointing left. You can undo an allo-



                 A+W Production Machine Allocation                                                                   D-91
                 Machine Allocation                                                             Software Reference




                                      cation by selecting a machine on the Work processes list and click on the ar-
                                      row pointing right.
                                       Tutorial, “Machine Allocation - Buttons” on page D-81
                                      Use the [+] button for a work process to view all allocated logical machines.
                                      Checkbox [Open all] can be used to display all allocated logical machines on
                                      the Work processes list.
                                      The logical machines allocated to a work process are highlighted in grey when
                                      you select the work process.

                                         Work processes in red
                                         A work process is shown in red until it is assigned a logical machine. Al-
                                         ways allocate a logical machine to the work processes. If the correspond-
                                         ing logical machine has not been defined yet you should allocate Dummy
                                         as a logical machine.
2.10 / 11-2018




                 D-92                                                           A+W Production Machine Allocation
                 Software Reference                                                                  Machine Allocation




                                        MA Editor – Machine Types
                                        Master data > MA > MA editor > MA types




                                        Fig. D-48     MA editor - MA types


                                        This tab is used to manage the machine types. Machine types are used,
                                        among other things, in order to separate procurement types from one another
                                        and form batches.
                                        The system-internal machine types have IDs up to 1000 and are displayed in
                                        italics. They cannot be edited.
                                         “Machine Type” on page D-111
                                        Overview
                                        The following columns are displayed:
                                        •   ID:
                                            ID of the machine type.
                                        •   Exclusive:
                                            Indication whether the machine type is allocated exclusively. Default set-
                                            ting for system-internal machine types: No.
                                        •   Mandatory:
                                            Indication of whether the allocation is prescribed. Default setting for sys-
                                            tem-internal machine types: Yes.
2.10 / 11-2018




                                        •   Implicit:
                                            Indication whether the machine type is allocated implicitly. Default setting
                                            for system-internal machine types: Yes exception to the entry Other.


                 A+W Production Machine Allocation                                                                 D-93
                 Machine Allocation                                                                   Software Reference




                                      •   Type name:
                                          Indication of the type name.
                                      •   Table reference:
                                          Specification of the relevant database table.
                                      User-defined machine types have lost their meaning. They have been re-
                                      placed by A+W processing types


                                      New Machine
                                      Master data > MA > MA editor > Machines > New.




                                      Fig. D-49     New machine


                                      Use this dialog to enter the master data for the new machine, thus defining a
                                      new machine.
                                       “Machine” on page D-95

                                      ID Freely selectable ID.

                                      Name Machine name

                                      Machine type Machine type, e.g. Cutting, Edgework or Bender.

                                      Element ID Freely selectable ID for the machine. The element ID is only used
                                      for the machine types Line, Cutting, and Bender.

                                          Example

                                          The element ID can be used to distinguish lines, tables, or benders if there
                                          are several machines of the same type.
                                          The tables 1, 2, and 3 for example could get the element IDs TB1, TB2, and
                                          TB3.
2.10 / 11-2018




                 D-94                                                             A+W Production Machine Allocation
                 Software Reference                                                                Machine Allocation




                                        Machine
                                        Master data > MA > MA editor > Machines > Edit.




                                        Fig. D-50    Machine


                                        Use this dialog to edit the machine master data.
                                         Tutorial, “Machine Definition and Management” on page D-22

                                        Machine Name of the selected machine.

                                        General properties of the machine Machine master data. When you select
                                        a field in Machine properties, the field below shows a short description.
                                        • ID:
                                            ID the machine has been assigned when it was defined.
                                        • Name:
                                            Name you have given the machine.
                                        • Registration point:
                                            This combo box serves to allocate a registration point to the machine. This
                                            number is used by A+W in order to make allocation easier in case of devi-
2.10 / 11-2018




                                            ating machine numbers. It is also used for setting up the PDC.
                                        • Overload limit per shift:
                                            This entry (in percent) refers to the capacity of the corresponding shift.


                 A+W Production Machine Allocation                                                               D-95
                 Machine Allocation                                                             Software Reference




                                      •   Overload limit for a period:
                                          This entry (in percent) refers to the capacity for a defined period, e.g. a
                                          week.
                                      •   Days:
                                          Defines the period (in days) to which the overload limit applies.
                                      •   Bottleneck:
                                          Define whether the machine is a potential bottleneck on the shop floor.
                                      •   Display type:
                                          Defines the unit to be used for the machine, e.g. quantity, scheduled quan-
                                          tity, sqm, weight, etc.
                                      •   Check load distribution:
                                          Defines whether the allocated logical machines shall be checked by A+W
                                          Capacity Planner capacity planning.
                                      •   Machinery group:
                                          Defines the machine group this machine has been allocated to in A+W Ca-
                                          pacity Planner.
                                      •   Location:
                                          Location of the machine.
                                      •   Cost center:
                                          Cost center the machine belongs to.
                                      •   Automatic scheduling:
                                          Specification of whether the machine may be scheduled automatically by
                                          A+W Capacity Planner.
                                      •   Processing chains:
                                          Specification of whether processing changes by A+W Capacity Planner are
                                          possible on the machine. With processing chains on a machine, subse-
                                          quent processings can be combined, insofar as the machine alternatives
                                          are the same. This setting may not be used for screen printing.
                                      •   Alternative machine:
                                          Defines whether A+W Capacity Planner can use this machine as an alter-
                                          native machine.

                                      Additional properties of the machine This section is only displayed for
                                      machines that belong to the machine types cutting, spacer bender, IG line, and
                                      cast resin.
                                      • Name:
                                         Machine name.
                                      • Machine code format:
                                         Format in which the machine code is transferred.
                                      • Call section:
                                         Selection of the allocated driver call. This way, you can configure machines
                                         of the same type differently and assign each one a call section. The setting
                                         0 corresponds to the section 1.
                                      • Line D:
                                         ID production line.
2.10 / 11-2018




                 D-96                                                          A+W Production Machine Allocation
                 Software Reference                                                                      Machine Allocation




                                        For cutting, you can define the following properties:




                                        X-, Y-, Z-, and W Cuts

                                        y axis,
                                        Cartesian


                                                                                   Y
                                                                                                     X



                                                                                                     Z
                                                3210 mm




                                                                 W




                                        Zero point 0                         6000 mm
                                                                                                                 x axis,
                                                                                                              Cartesian

                                        Fig. D-51         X-, Y-, Z-, and W cuts in A+W Production


                                        Cutting tables distinguish X-, Y-, Z-, and W cuts as shown above. The
                                        directions X and Y seem to be changed by 90° in A+W Production as
                                        compared with the common coordinate system.
                                        •   The definition of X and Y cuts in A+W Production is: The cut is made at an
2.10 / 11-2018




                                            X- or Y value referring to the Cartesian coordinate system.
                                            This means that the cut is at right angles with the Cartesian coordinate sys-
                                            tem in A+W Production.


                 A+W Production Machine Allocation                                                                    D-97
                 Machine Allocation                                                                 Software Reference




                                          An example for cutting a lite:
                                          The lite shall be cut to a size of 5000 x 2500 mm. You enter in A+W Pro-
                                          duction X = 5000 mm and Y = 2500 mm. The cutting table will apply a ver-
                                          tical cut at the X coordinate 5000 mm and a horizontal cut at the Y
                                          coordinate 2500 mm.
                                      •   W- and Z cuts: These match the X and Y cuts in terms of the direction but
                                          are smaller and therefore more complex. To apply a Z cut, the sheet must
                                          be turned on the cutting table in order to break it. This takes time and is ex-
                                          pensive. From a defined amount of work on, cuts are called W- and Z cuts.
                                      A+W Production tries to avoid W and Z cuts. The importance of avoiding W-
                                      and Z cuts can be defined when editing cutting tables by means of the variable
                                      Cost per X cut.

                                      Show field description You can display the field descriptions for the marked
                                      property:
                                      ☐ The field description is not displayed.
                                      ☑ Opens the dialog Field description (database field). The dialog title shows
                                      the name of the database field.

                                      Restrictions Machine restrictions indicate the physical limits of a machine,
                                      which cannot be overcome.
                                      These checkboxes serve to define the restrictions for the machine:
                                      •   Minimum thickness
                                      •   Maximum thickness
                                      •   Shapes
                                      •   Coated glass
                                      •   Patterned glass
                                      •   Stepped IG
                                       Tutorial, “Definition and Editing of Machine Restrictions” on page D-26

                                          Machine restrictions and logical machines
                                          If the restrictions of a machine can be overcome through reconfiguration or
                                          set-up, you should create a logical machine for the respective application
                                          cases.

                                      Sizes Size restrictions define whether a machine can process only elements
                                      of a minimum or maximum size, e.g. lites wider than 100 mm.
                                      The button [Pen] is used to open the dialog Size restrictions to define restric-
                                      tions in terms of sizes.
                                       “Dimension Restrictions” on page D-100
                                      If size restrictions have been defined, these are shown in field Sizes.

                                      Spacer Spacer restrictions define the spacers that can be processed by the
                                      machine, e.g. spacers wider than 16 mm and narrower than 24 mm.
                                      Button [Pen] can be used to open the dialog Spacer restrictions to define re-
2.10 / 11-2018




                                      strictions for the spacers.
                                       Software Reference, “Spacer Restrictions” on page D-101
                                      If spacer restrictions have been defined, these are shown in field Spacer.


                 D-98                                                            A+W Production Machine Allocation
                 Software Reference                                                                 Machine Allocation




                                        Additional condition Allows to select additional conditions which have been
                                        defined before by means of the formula editor.
                                        Use the [Zoom] button to open the dialog Select condition to choose additional
                                        conditions or formulas.
                                         “Select a Condition” on page D-102
                                        If an additional condition has been selected, this is shown in field Additional
                                        condition.

                                           Additional conditions
                                           Additional conditions seriously influence the behavior and the properties of
                                           machines.
                                           If an additional condition is defined, you have to understand its conse-
                                           quences.
                                           An additional condition could invert all properties of a certain machine for
                                           instance.

                                        For information about the topic of formulas and restrictions in A+W Production,
                                        see the part about the Formula editor.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                D-99
                 Machine Allocation                                                                Software Reference




                                      Dimension Restrictions
                                      Master data > MA > MA editor > Machines > Edit > Select property > [Edit].




                                      Fig. D-52    Size restrictions


                                      This dialog is used to define restrictions with regard to sizes. You can therefore
                                      define whether only lites from a certain size onward or up to a certain size can
                                      be processed.
                                       Tutorial, “Machine Definition and Management” on page D-22

                                      Machine name
                                      The name is adopted from the machine's properties.

                                      Min. width, min. height Specification of the smallest width and/or height
                                      that can be processed on the machine.

                                      Max. width, max. height Specification of the largest width and/or height that
                                      can be processed on the machine.
2.10 / 11-2018




                 D-100                                                          A+W Production Machine Allocation
                 Software Reference                                                                 Machine Allocation




                                        Spacer Restrictions
                                        Master data > MA > MA editor > Machines > Edit > Spacer > [Edit].




                                        Fig. D-53    Spacer restrictions


                                        This dialog serves to define restrictions for the airspace (AIR).
                                         Tutorial, “Machine Definition and Management” on page D-22

                                        Machine name
                                        The name is adopted from the machine's properties.

                                        Min. AIR 1, Min. AIR 2 Specification of the smallest width and/or height that
                                        can be processed on the machine.

                                        Max. AIR 1, Max. AIR 2 Specification of the largest width and/or height that
                                        can be processed on the machine.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                             D-101
                 Machine Allocation                                                                   Software Reference




                                      Select a Condition
                                      Master data > MA > MA editor > Machine > Logical machines > Work process-
                                      es > Edit > [Zoom].




                                      Fig. D-54    Select a condition


                                      On this dialog, you select conditions for a machine, logical machine or a work
                                      process and you assign them to the respective machine, logical machine or
                                      work process.
                                      These additional conditions are defined and edited by means of the formula
                                      editor. Thus, you can specify exact restrictions for machines, logical machines,
                                      and work processes, e.g. with a complex formula.
                                       Tutorial, “Conditions, Formulas, Restrictions” on page D-63

                                          Additional conditions
                                          Additional conditions seriously influence the behavior and the properties of
                                          machines.
                                          If an additional condition is defined, you have to understand its conse-
                                          quences.
                                          An additional condition could invert all properties of a certain machine for
                                          instance.

                                      For information about the topic of formulas and restrictions in A+W Production,
                                      see the part in the manual about the Formula editor.

                                      List
                                      •   ID:
                                          ID allocated to the condition.
                                      •   Condition:
                                          Name assigned to the condition.
2.10 / 11-2018




                                      Description Description entered for the condition.



                 D-102                                                           A+W Production Machine Allocation
                 Software Reference                                                                    Machine Allocation




                                        Language Selection of the language in which the description is displayed.

                                        Text Display of the formula. If the selected formula was defined in the formula
                                        editor (text variant) based on an existing formula, the name of the original for-
                                        mula is specified here.

                                        Only own You can limit the display of the formulas.
                                        ☐Lists all conditions.
                                        ☑Lists only user-defined conditions.

                                        ID Specification of the ID or part of the ID to which you want to restrict the list.

                                        Text Specification of the ID or part of the ID of the name to which you want
                                        to restrict the list.


                                        New Logical Machine
                                        Master data > MA > MA editor > Logical machines > New.




                                        Fig. D-55     New logical machine


                                        Use this dialog to enter the master data for the new machine, to define a new
                                        logical machine.
                                         “Logical Machine” on page D-104

                                        Machine Shows the ID and name of the machine belonging to the logical ma-
                                        chine.

                                        ID Freely selectable ID of the logical machine.

                                        Name Freely selectable name of the logical machine.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                                  D-103
                 Machine Allocation                                                             Software Reference




                                      Logical Machine
                                      Master data > MA > MA editor > Logical machines > Edit.




                                      Fig. D-56    Logical machine


                                      This dialog is used to enter the master data for the logical machine.
                                       Tutorial, “Logical Machines” on page D-33

                                      General properties of the logical machine Master data of the logical ma-
                                      chine. When you select a field, the field below shows a short description.
                                      • ID:
                                         ID you have assigned to the logical machine.
                                      • Name:
                                         Name you have given the logical machine.
                                      • Type:
                                         Machine type.
                                      • Speed behavior:
                                         Speed reference, defined by the machine manufacturer.
                                      • Performance:
                                         Defined by the machine manufacturer.
                                      • Check program:
                                         The logical machine can be allocated to an external check program which
                                         determines whether the machine can perform this task.
2.10 / 11-2018




                                      • Driver:
                                         Machine driver for the production machine.




                 D-104                                                         A+W Production Machine Allocation
                 Software Reference                                                                 Machine Allocation




                                        •   Allowance group:
                                            ID of the group for calculating the grinding allowance.
                                        •   DynOpt:
                                            Defines if the program DynOpt is being used.
                                        •   Processing time:
                                            Formula used to calculate the time this process takes. Double-click on the
                                            field or a selected formula to open the dialog Formula selection.
                                             “Formula Selection” on page D-106
                                        •   Set-up time:
                                            Formula used to calculate the set-up time.
                                        •   Element ID:
                                            Element ID of the logical machine. It is automatically adopted from the ma-
                                            chine in question and cannot be changed.
                                        •   Allow as alternative:
                                            Defines if the logical machine can be used as an alternative machine in
                                            case of a bottleneck at a different machine which was actually scheduled
                                            for the work process. This setting is important for rescheduling.
                                        When you select a field in General properties of the logical machine, the field
                                        below shows a short description.

                                        Show field description You can display the field descriptions for the marked
                                        property:
                                        ☐ The field description is not displayed.
                                        ☑Opens the dialog Field description (database field).

                                        Additional condition Shows the additional condition.
                                        Use the [Zoom] button to open the dialog Select condition to choose additional
                                        conditions or formulas.
                                         “Select a Condition” on page D-102

                                            Additional conditions
                                            Additional conditions seriously influence the behavior and the properties of
                                            machines.
                                            If an additional condition is defined, you have to understand its conse-
                                            quences.
                                            An additional condition could invert all properties of a certain machine for
                                            instance.

                                            For information about the topic of formulas and restrictions in A+W Produc-
                                            tion, see the part in the manual about the Formula editor.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                               D-105
                 Machine Allocation                                                                Software Reference




                                      Formula Selection
                                      Master data > MA > MA editor > Logical machines > Edit > Select Processing
                                      time > [...].




                                      Fig. D-57    Formula selection


                                      Use this dialog to choose the formula that defines the processing time for a
                                      logical machine.. The formulas for the processing time are defined and edited
                                      in the Formula editor.
                                       Tutorial, “Select a Formula for the Processing Time of a Logical Machine” on
                                        page D-66
                                       “Formula Editor” on page D-120
                                      The processing time of a logical machine can also be entered or edited in A+W
                                      Capacity Planner capacity planning.
                                      For information about the topic of formulas and restrictions in A+W Production,
                                      see the part in the manual about the Formula editor.

                                      Available formulas List of formulas defined for the processing time.

                                      Description Select the description of the formula.

                                      [New] Opens the dialog Formula editor where a new formula can be entered.
                                       “Formula Editor” on page D-120
2.10 / 11-2018




                                      [Edit] Opens the dialog Formula editor for editing the selected formula.

                                      [OK] Imports the selected formula into the Logical machine dialog.



                 D-106                                                           A+W Production Machine Allocation
                 Software Reference                                                               Machine Allocation




                                        [Cancel] Closes the dialog without adopting the changes.


                                        New Work Process
                                        Master data > MA > MA editor > Work processes > New.




                                        Fig. D-58    New work process


                                        This dialog serves to enter new work processes and allocate IDs and names.
                                         “Work Process” on page D-108

                                        ID Freely selectable ID.

                                        Name Freely selectable name.
                                        Press [OK] to save the ID and Name and open dialog Work process.
                                         Software Reference, “Work Process” on page D-108

                                           Non-allocated work processes
                                           A work process is shown in red until it is assigned a logical machine. Al-
                                           ways allocate a logical machine to the work processes. If the correspond-
                                           ing logical machine has not been defined yet you should allocate Dummy
                                           as a logical machine.

                                         Tutorial, “Allocation of Work Processes” on page D-52
2.10 / 11-2018




                 A+W Production Machine Allocation                                                            D-107
                 Machine Allocation                                                              Software Reference




                                      Work Process
                                      Master data > MA > MA editor > Work processes > Edit.




                                      Fig. D-59    Work process


                                      This dialog serves to enter the master data for a work process.
                                       Tutorial, “Work Process Definition and Management” on page D-49
                                       Tutorial, “Definition and Management of Processing Types” on page D-73

                                      Properties
                                      •   ID:
                                          ID you have assigned to the work process.
                                      •   Name:
                                          Name you have given the work process..
2.10 / 11-2018




                 D-108                                                         A+W Production Machine Allocation
                 Software Reference                                                                 Machine Allocation




                                        Restrictions
                                        The option is used to define the processing type on which the work process is
                                        based. The appropriate combo boxes are accessible.
                                        • None:
                                           No restriction.
                                        • A+W types:
                                           Selection from the A+W default processing catalogue.
                                        • Types:
                                           Selection from the processing types defined by the user.
                                           You will find the processing types under Master Data > Processings > Pro-
                                           cessing Items.
                                        • Item:
                                           Selection from the processing items defined by the user.
                                           You will find the processing types under Master Data > Processings > Pro-
                                           cessing Items.

                                           Work processes, processing types, and articles
                                           Due to the complexity of this subject we recommend allocating work pro-
                                           cesses only the processing types Catalog and Types.

                                        Article
                                        The option is used to define the article or article group on which the work pro-
                                        cess is based. The appropriate combo boxes are accessible.
                                        • None:
                                           No restriction.
                                        • Article type:
                                           Selection of article type.
                                        • Article group:
                                           Selection of production article group..
                                        • Article:
                                           Selection of a certain article.

                                        Additional condition Shows an additional condition.
                                        Use the [Zoom] button to open the dialog Select condition to choose additional
                                        conditions.
                                         “Select a Condition” on page D-102

                                           Additional conditions
                                           Additional conditions seriously influence the behavior and the properties of
                                           machines.
                                           If an additional condition is defined, you have to understand its conse-
                                           quences.
                                           An additional condition could invert all properties of a certain machine for
                                           instance.

                                        For information about the topic of formulas and restrictions in A+W Production,
2.10 / 11-2018




                                        see the part in the manual about the Formula editor.




                 A+W Production Machine Allocation                                                              D-109
                 Machine Allocation                                                                   Software Reference




                                      New Machine Type
                                      Master data > MA > MA editor > Machine type > New.




                                      Fig. D-60     New machine type


                                      On this dialog, you enter the master data for the new machine type and there-
                                      fore create a new machine type.
                                       “Machine Type” on page D-111

                                      ID Freely selectable ID. Must be >1000.

                                      Name Freely selectable name.

                                      Table reference Specification of the database table for the new machine
                                      type. The data for the allocated machines are saved in this table.

                                         Example

                                         In the table XOPT_TISCH, all cutting tables are listed that are assigned to the
                                         machine type cutting.

                                         In the table MZO_ISOLINIE, all details about the machine format are saved,
                                         e.g. format of the machine code for activation of the line or of the bender.


                                      Driver type Database field
                                      MZO_MASCHINTYP.DRIVER_CALL_METHOD. The property is only re-
                                      quired for inventory maintenance. For compatibility reasons, the setting can be
                                      set to the following values:
                                      ☐ Yes= Method (driver call)
                                      ☑ No
                                       Irrelevant
2.10 / 11-2018




                 D-110                                                             A+W Production Machine Allocation
                 Software Reference                                                                Machine Allocation




                                        Machine Type
                                        Master data > MA > MA editor > Machine types > Select machine type > [Edit].




                                        Fig. D-61    Editing machine type


                                        On this dialog, you edit the properties for a user-defined machine type.

                                        Machine
                                        Name of selected machine type

                                        General properties of the machine type Master data of the machine type:
                                        • ID: ID the machine type has been assigned when it was defined.
                                        • Text:
                                          Name you have given the machine type.
                                        • Table reference:
                                          Display of the database table in which the data for the allocated machines
                                          is saved.
                                        • Driver type:
                                          The property is only required for inventory maintenance for reasons of
2.10 / 11-2018




                                          compatibility.
                                        • Exclusive, Mandatory, Implicit:
                                          Indication how the machine type is allocated.


                 A+W Production Machine Allocation                                                             D-111
                 Machine Allocation                                                             Software Reference




                                      Show field description You can display the field descriptions for the marked
                                      property:
                                      ☐ The field description is not displayed.
                                      ☑Opens the dialog Field description (database field).

                                      Restrictions

                                      Additional condition Shows an additional condition.
                                      Use the [Zoom] button to open the dialog Select condition to choose additional
                                      conditions or formulas.
                                       “Select a Condition” on page D-102

                                         Additional conditions
                                         Additional conditions seriously influence the behavior and the properties of
                                         machines.
                                         If an additional condition is defined, you have to understand its conse-
                                         quences.
                                         An additional condition could invert all properties of a certain machine for
                                         instance.

                                      For information about the topic of formulas and restrictions in A+W Production,
                                      see the part in the manual about the Formula editor.
2.10 / 11-2018




                 D-112                                                        A+W Production Machine Allocation
                 Software Reference                                                    Machine Allocation - Formulas




                                        Machine Allocation - Formu-
                                        las
                                        Formulas are used to define restrictions for machines, logical machines, and
                                        work processes for specific cases.
                                        Existing formulas can be selected from the following dialogs:
                                         “Machine” on page D-95
                                         “Logical Machine” on page D-104
                                         “Work Process” on page D-108
                                        Formulas and conditions are described in detail in the Formula editor part.
                                        This section provides information on the following subjects:
                                        •   “Select a Condition” on page D-102
                                        •   “Select Conditions” on page D-114
                                        •   “New Condition” on page D-117
                                        •   “Info (about the new condition)” on page D-117
                                        •   “Select quantity” on page D-118
                                        •   “Formula Editor” on page D-120
                                        •   “Formula Editor” on page D-120
2.10 / 11-2018




                 A+W Production Machine Allocation                                                             D-113
                 Machine Allocation - Formulas                                                    Software Reference




                                         Select Conditions
                                         Master data > MA > Formula.




                                         Fig. D-62    Select conditions


                                         On this dialog, you manage the conditions that can be assigned in the MA. You
                                         can create, edit or delete formulas for the conditions.
                                         A+W Production offers two editors for defining and editing formulas:
                                          “Condition Editor (Graphic Version)” on page D-115
                                          “Condition Editor (Text Version)” on page D-119

                                         Existing conditions List of all conditions defined (predefined and user-de-
                                         fined).

                                         Description Description entered for the condition.

                                         [New condition (graphic)...] Opens the condition editor (graphic version).
                                          “Condition Editor (Graphic Version)” on page D-115

                                         [New condition (text)...] Opens the condition editor (text version).
                                          “Condition Editor (Text Version)” on page D-119

                                         [Edit] Opens the condition selected in the condition editor (graphic version)

                                         [Delete] Deletes the selected condition.
2.10 / 11-2018




                                         No condition You can assign a condition or remove an assigned condition.
                                         ☐ The condition is assigned.



                 D-114                                                             A+W Production Machine Allocation
                 Software Reference                                                       Machine Allocation - Formulas




                                        ☑The dialog shows as a result that Nothing was selected. Confirm this setting
                                        by [OK].


                                        Condition Editor (Graphic Version)
                                        Master data > MA > Formula > New condition (graphics).




                                        Fig. D-63    Condition editor (graphic version)


                                        Use this dialog to define formulas for conditions with graphic support. The for-
                                        mulas are defined as logical relations in the editor.
                                         Tutorial, “Conditions, Formulas, Restrictions” on page D-63
2.10 / 11-2018




                 A+W Production Machine Allocation                                                               D-115
                 Machine Allocation - Formulas                                                               Software Reference




                                           Menus

                                           Entry                        Function

                 Menu Conditions           Name                          “New Condition” on page D-117

                                           Info                          “Info (about the new condition)” on page D-117

                                           Quantity                      “Select quantity” on page D-118

                                           Invert                       Can be used to invert the formula of the condition.

                                           OK                           Creates the new condition and displays it in the
                                                                        selection.

                                           Cancel                       Cancels the transaction.

                 Menu element              Add (column)                 An AND relation is added.
                 conditions

                                           Add (line)                   An OR relation is added.

                                           Delete                       Deletes the selected relation.

                 Tab. D-1    Menus in conditions editor

                                           Buttons
                                           In addition to the menus, the functions can be selected by means of the follow-
                                           ing buttons:

                                           Icon                         Function

                                                                        The defined condition will be saved, and the editor is
                                                                        closed.

                                                                        The defined condition will be rejected, and the editor is
                                                                        closed

                                                                        Opens the dialog for defining the condition. With a
                                                                        second click, another control opens in order to display
                                                                        an AND link.

                                                                        Opens the dialog for defining the condition. With a
                                                                        second click, another control opens in order to display
                                                                        an OR link.

                                                                        Deletes the selected condition.


                                           Options switch All           Considers the conditions for all elements of a BOM.

                                           Options switch One           Only the characteristics of the lite in question will be
                                                                        considered.

                                           Options switch Zero          The quantity allocated to the condition will not be taken
                                                                        into account.
2.10 / 11-2018




                                           Tab. D-2       Buttons in condition editor




                 D-116                                                                  A+W Production Machine Allocation
                 Software Reference                                                        Machine Allocation - Formulas




                                        New Condition
                                        Master data > MA > Formula > New condition (graphics) > Menu conditions >
                                        Name.




                                        Fig. D-64    Condition editor (graphic version) > Condition name


                                        On this dialog, you specify the name of the condition in order to create it.


                                        Info (about the new condition)
                                        Master data > MA > Formula > New condition (graphics) > Menu conditions >
                                        Info




                                        Fig. D-65    Condition editor (graphic version) > Info


                                        On this dialog, you specify additional information about a new condition.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                               D-117
                 Machine Allocation - Formulas                                                          Software Reference




                                         Select quantity
                                         Master data > MA > Formula > New condition (graphics) > Menu conditions >
                                         Quantity
                                         Master data > MA > Formula > Condition editor (text).




                                         Fig. D-66    Condition editor (graphic version) > Select quantities


                                         In this dialog you can select the quantity for a condition.
2.10 / 11-2018




                 D-118                                                              A+W Production Machine Allocation
                 Software Reference                                                       Machine Allocation - Formulas




                                           Condition Editor (Text Version)
                                           Master data > MA > Formula > New condition (text) > Edit > [Quantity].




                 Fig. D-67   Condition editor (text version)


                                           Use this dialog to create or edit a conditions with formulas. The formulas are
                                           defined as logical relations in the editor.

                                           Condition

                                           ID Condition ID

                                           Name Condition name.

                                           Valid syntaxes
                                           List of valid, logical operators

                                           Condition Enter the formula.

                                           Description Description of the condition, e.g. the use.

                                           General
2.10 / 11-2018




                                           Status Shows the current state of the condition.




                 A+W Production Machine Allocation                                                                 D-119
                 Machine Allocation - Formulas                                                        Software Reference




                                          Language Selection of the language in which the description is displayed.

                                          Available formulas List of the defined formulas. These can be taken over
                                          with a double-click. In the Condition field, they are inserted in the cursor loca-
                                          tion.

                                          Description Description of the selected formula.

                                          [Delete] Deletes a selected formula without query.

                                          [New formula] Open a formula editor to define formulas. These appear in the
                                          list of Available formulas and can be used to define conditions.

                                          [Edit] Opens the formula selected in the editor so that it can be edited.


                                          Formula Editor
                                          Master data > MA > MA editor > Logical machines > Processing time > For-
                                          mula selection > New, edit.




                 Fig. D-68   Formula editor


                                          Use this dialog to enter and process formulas which e.g. define the processing
2.10 / 11-2018




                                          time for logical machines.




                 D-120                                                              A+W Production Machine Allocation
                 Software Reference                                                    Machine Allocation - Formulas




                                        Formula

                                        ID Formula ID.

                                        Name Formula name,

                                        Formula Formula definition.

                                        Description Formula description.

                                        Available formulas

                                        Formula List of the defined formulas. These can be adopted with a double-
                                        click. In the Condition field, they are inserted at the cursor location.

                                        Name Name of the selected formula.

                                        Description Description of the selected formula.

                                        [Add formula] Inserts the selected formula in the formula that is being edited.

                                        [Apply] Saves the new or amended formula. This will then be shown on the
                                        list in dialog Formula selection.

                                        [Close] Closes the Formula editor dialog.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                              D-121
                 Processings in Machine Allocation                                                 Software Reference




                                         Processings in Machine Allo-
                                         cation
                                         The MA works with a standardized processing catalog so that the data can be
                                         exchanged with the other programs of A+W Software GmbH. In the MA, this
                                         processing catalog includes the processing types and processing items.
                                         This section provides information on the following subjects:
                                         •   “Processing Types” on page D-123
                                         •   “Processing Articles” on page D-125
2.10 / 11-2018




                 D-122                                                             A+W Production Machine Allocation
                 Software Reference                                                  Processings in Machine Allocation




                                        Processing Types
                                        Master data > Processings > Processing types.




                                        Fig. D-69    Processing types


                                        This dialog lists all defined processing types. You can create and edit or delete
                                        processing types.
                                        The processing type describes the technical type of processing, e.g. Cutting,
                                        Assembly, Arrissing, Grinding, or Packing.

                                        List
                                        •   No.:
                                            Unique number of processing type.
                                        •   Name:
                                            Name of processing type.
                                        •   Sequence:
                                            Sequence of processing type.

                                            Processing types
                                            A+W Production offers a standard catalog of processing types. They have
                                            got four-digit numbers and must not be amended by the user.
                                            You can define additional processing types.

                                        Processing type no.: Number of the processing type; can be chosen at ran-
                                        dom.

                                        Sequence Enter the sequence assigned to the processing type. The lower
                                        the sequence number, the earlier on the processing step comes in the produc-
2.10 / 11-2018




                                        tion process. Correct sequences are vital for the reliable calculation of produc-
                                        tion dates in capacity planning.




                 A+W Production Machine Allocation                                                                D-123
                 Processings in Machine Allocation                                                   Software Reference




                                         Name Specification of a name with which you briefly describe the processing
                                         type.

                                         Counting of processings Defines how the processings shall be counted.
                                         • Accumulate:
                                           If the same processing step is executed several times for a lite, every pass
                                           through will be counted.
                                         • Count once:
                                           If the same processing step is executed several times for a lite, the pro-
                                           cessing step is counted just once to make sure that it has been executed.
                                         • Do not count:
                                           The processing is not counted.

                                         Processing type Choose the processing type. The processing type controls
                                         the correct turning of lites to be printed or coated. The following processing
                                         types are available:
                                         • 505 Glass cutting for the cutting of lites
                                         • 588 Screen printing for silk screen printing
                                         • 00 not allocated for all other processing steps

                                         Barcoding tracking Processings that belong to the current processing type
                                         are considered in the PDC initialization.
                                         The setting is imported from the column assignment of the PDC and cannot
                                         be changed on the processing type.
                                         You will find a description of the master data for the PDC in the Plant Data Col-
                                         lection part.

                                         [Change]    Enables the input fields for the selected processing.

                                         [Reject] End the process without adopting the changes.

                                            Delete processing types
                                            Processing types cannot be deleted if they are allocated to a production ar-
                                            ticle. A security query appears in this case.
                                            Undo the allocation before starting the deletion.

                                             Tutorial, “How to delete a processing type” on page D-75
2.10 / 11-2018




                 D-124                                                             A+W Production Machine Allocation
                 Software Reference                                                  Processings in Machine Allocation




                                        Processing Articles
                                        Master data > Processing > Processing articles.




                                        Fig. D-70    Processing article


                                        This dialog lists all defined processing articles. You can define processing ar-
                                        ticles and edit or delete existing ones.
                                        The processing article describes the technical type of processing in closer de-
                                        tail like Bevelling, Mitre, Grooving, or Frosting, A processing article always re-
                                        fers to a processing type.

                                        List List of defined processing articles.
                                        • Article no.:
                                           Unique number allocated to the processing article.
                                        • Name:
                                           Name assigned to the processing article..
                                        • Processing type:
                                           Processing type the processing article refers to..

                                        Article no. Number of the processing article; can be chosen at random.

                                        Name Free description of the processing article.
2.10 / 11-2018




                                        Processing type Processing type the processing article refers to.




                 A+W Production Machine Allocation                                                                D-125
                 Processings in Machine Allocation                                                  Software Reference




                                         Category The category defines the BOM position in which the contents of the
                                         plan text is saved. Valid entries for the category are 1- 8.

                                         Plan text/Prior. The Plan text is a code added to the bill of materials. The
                                         plan text can define for instance that a lite needs to be polished.
                                         The priority defines which code or plan text shall be used if several processing
                                         steps of the same category are to be executed. The lower the value, the higher
                                         the priority.

                                         Transition time Transition time for processing article. Function Transition
                                         time is currently inactive.

                                         Duration Duration of the processing. In the combo box, you select the refer-
                                         ence variable Piece, Length, Area or Volume.

                                         Sequence Sequence of the processing on the bill of materials. This can be
                                         used to define the processing sequence in closer detail.

                                         Grinding group Grinding group if the processing article is edgework. Edge-
                                         work – even if no material is removed – will be taken into account for geometry
                                         calculation and feasibility checks only if a grinding group has been selected.

                                          Text Description for processing article.

                                         Extra 1 Data for the link with the CAD system. Define the entries together with
                                         the A+W Software GmbH project team.

                                         Extra 2 This field is currently inactive.

                                         Can be applied to ... This entry supports the BOM check at order scheduling
                                         by rejecting processing steps that have been positioned wrongly.
                                         • 00 not allocated:
                                            The processing step will be rejected in any case.
                                         • 01 Non-glass article:
                                            The processing step must not be applied to glass, e.g. packing of fittings.
                                         • 02 Basic glass:
                                            The processing step must be applied to basic glass only, e.g. float cutting.
                                         • 04 IG:
                                            The processing step must be applied to IG only, e.g. gas filling.
2.10 / 11-2018




                 D-126                                                               A+W Production Machine Allocation
                 Software Reference                                                 Processings in Machine Allocation




                                        •   54 Untoughened glass:
                                            The processing step must be applied only to untoughened glass.
                                        •   62 All products:
                                            The processing step can be applied to all glass types.

                                        Contains processing dimensions You can specify whether the processing
                                        dimensions are considered for the geometry calculation.
                                        ☐Default setting. This checkbox should not be checked because otherwise,
                                        geometry calculation will take into account even processing steps which are
                                        no edgework.
                                        ☑The processing step will be considered for geometry calculation.

                                        Correct cutting dimensions You can specify where the cutting dimensions
                                        are calculated.
                                        ☐ Default setting. This checkbox should not be checked.
                                        ☑The cutting size will be calculated irrespective of article master data.

                                        Explicit planning You can specify whether the processing is enabled sepa-
                                        rately.
                                        ☐ No function
                                        ☑ The processing article can be released separately if the processing step is
                                        applied. You can use it for example to release a basic glass separately for the
                                        processing step screen printing.

                                        Internal processing You can specify whether the processing item serves
                                        only for internal calculations.
                                        ☐ No function
                                        ☑ The processing step describes the creation of the BOM element as a 'defin-
                                        ing' processing step.

                                        External processing You can specify whether the processing item serves for
                                        third-party processings.
                                        ☐ The processing item is used in A+W Production.
                                        ☑ This processing step will be performed by an external supplier.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                              D-127
                 Processings in Machine Allocation                                                 Software Reference




                                         Adjust Columns
                                         Master data > Processings > Processing types > [Adjust columns].




                                         Fig. D-71    Adjust Columns


                                         On this dialog you can specify which columns are displayed. This way, you can
                                         influence the design of the dialog.

                                         Available columns Display of the database fields that are available.

                                         Current columns Display of the database fields that are currently displayed.

                                         [Edit] Opens the Column definition dialog in order to edit the selected entry.
2.10 / 11-2018




                 D-128                                                           A+W Production Machine Allocation
                 Software Reference                                                 Processings in Machine Allocation




                                        Column Definition
                                        Master data > Processings > Processing types > [Adjust columns] > [Edit].




                                        Fig. D-72    Column definition


                                        On this dialog, you can edit the columns.

                                           Editing column definition
                                           The column definition reaches deep into the functionality of A+W Produc-
                                           tion. Consult A+W Software GmbH service if you want to edit the settings.
2.10 / 11-2018




                 A+W Production Machine Allocation                                                            D-129
                 Processings in Machine Allocation                  Software Reference
2.10 / 11-2018




                 D-130                               A+W Production Machine Allocation
Machine Allocation            D

                     Section Index




                A+W Production
                 Section Index                                                Index Machine Allocation




                 Index Machine Allocation
                 A                                     – Machine types D-93
                 Additional condition D-21             – Machines D-87
                 – Select D-102                        – Work process allocation D-91
                 AND/OR relations D-20                 – Work processes D-90
                                                       Machine D-15, D-16, D-87
                                                       – Additional condition D-21
                 B
                                                       – AND/OR relations D-20
                 Buttons in MA    D-81
                                                       – Coated glass D-28
                                                       – Coated lites D-19
                 C                                     – Define D-22, D-94
                 Coated lites D-19                     – Delete D-25
                 Condition editor                      – Edit D-23, D-26, D-95
                 – Graphic version D-115               – Edit properties D-23
                 – Text version D-119                  – Element ID D-21
                 Conditions and formulas D-63, D-113   – Enter D-22, D-94
                 – in MA D-64                          – Lite format D-20
                 – Processing time D-66, D-106         – Manage D-22
                                                       – Maximum thickness D-26
                 D                                     – maximum thickness D-19
                 define   D-110                        – Minimum thickness D-26
                                                       – minimum thickness D-19
                                                       – Names and numbers D-18
                 E
                                                       – Patterned glass D-19, D-28
                 Element ID   D-21
                                                       – Restrictions D-18
                                                       – Shapes D-19, D-28
                 F                                     – Size restrictions D-20, D-30, D-31, D-100
                 Formula editor                        – Spacer restrictions D-20, D-30, D-31, D-101
                 – Graphic version D-115               – Stepped IG D-20, D-28
                 – Text version D-119                  – X-, Y-, Z-,W cuts D-97
                 Formulas and conditions D-63, D-113   Machine allocation D-14
                 – in MA D-64                          – Buttons D-81
                 – Processing time D-66, D-106         – Elements D-12
                                                       – logical machine D-33
                 L                                     – Work process D-41
                 Lite format D-20                      – Work process allocation D-52
                 Logical machine D-33, D-34, D-88      Machine restrictions D-18
                 – Define D-36, D-103                  – Edit D-26
                 – Delete D-39                         Machine type D-110
                 – Edit D-38, D-104                    – Edit D-111
                 – Enter D-36, D-103                   Machine types D-93
                 – Formula selection D-106, D-120      Machinery allocation
                 – Manage D-36                         – Machine D-15, D-16
                 – Processing time D-106, D-120        Maximum thickness D-19
                                                       Minimum thickness D-19
                 M
                                                       N
2.10 / 11-2018




                 MA D-14
                 – Elements D-12                       New logical machine D-103
                 MA editor                             New machine D-22, D-94
                 – Logical machines      D-88          New machine type D-110


                 A+W Production Machine Allocation                                             D-133
                 Index Machine Allocation                                         Section Index




                 New work process   D-107

                 P
                 Patterned glass D-19
                 Processing articles D-69
                 – Define D-76
                 – Delete D-79
                 – Edit D-78
                 – Enter D-76
                 – in MA D-71
                 – Manage D-76
                 – Undo allocation to processing type D-79
                 Processing types D-69, D-122, D-123
                 – Define D-73
                 – Delete D-75
                 – Edit D-74
                 – Enter D-73
                 – in MA D-70
                 – Manage D-73

                 S
                 Select condition D-65, D-102
                 Select formula D-65, D-102
                 Shapes D-19
                 Size restrictions D-20, D-100
                 Spacer restrictions D-20, D-101
                 Stepped IG D-20

                 W
                 Work process D-41, D-42, D-90
                 – Additional condition D-46
                 – Based on processing article D-47
                 – Define D-49, D-107
                 – Delete D-51
                 – Edit D-50, D-108
                 – Enter D-49, D-107
                 – Exact definition D-44
                 – Manage D-49
                 – not allocated D-45
                 – Priority D-45
                 – Several work processes D-45
                 Work process allocation D-52, D-91
                 – Additional condition D-53
                 – Allocate logical machine and work
                   process D-58
                 – Change priority D-61
                 – flexibly adapted D-53
                 – Separate logical machine and work
                   process D-60
2.10 / 11-2018




                 D-134                                       A+W Production Machine Allocation

