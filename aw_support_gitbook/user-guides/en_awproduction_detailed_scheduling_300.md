---
title: "EN AWProduction Detailed Scheduling 3.00"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["EN_AWProduction_Detailed_Scheduling_3.00"]
version: "1.0"
last_updated: "2025-12-10"
description: "Detailed Scheduling        D                                 English                     A+W Production                                                                                                              Introduction                                             Introduction                                         In this part of the documentation you can find editorial notices.                                           Revision Overview                                         Part"
source_file: "EN_AWProduction_Detailed_Scheduling_3.00.pdf"
---


# EN AWProduction Detailed Scheduling 3.00

Detailed Scheduling        D




                            English




                A+W Production
                                                                                                             Introduction




                                        Introduction
                                        In this part of the documentation you can find editorial notices.


                                        Revision Overview
                                        Part                       Description
                                        Version / Date

                                        3.00 / 01-2023             Complete revision.

                                        2.02 / 01-2017             Product and company names adjusted, fields added

                                        2.01 / 08-2013             Complete revision of the ALCIM documentation and
                                                                   adjustment to A+W Production.

                                        2.00 / 11-2012             Complete revision.

                                        1.00 / 09-2007             Original version.



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
                                        without prior notice. The text and illustrations were compiled with the utmost
                                        care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be
                                        held liable for errors or inaccuracies, unless they can be attributed to wilful or
                                        grossly negligent action.
                                        The descriptions in this document are based on the full installation of A+W
                                        Production.

                                        Copyrights
                                        © 2023, A+W Software GmbH, any right, also the right of reprint, the produc-
                                        tion of copies and of the translation, is reserved. The documentation must be
                                        copied, completely or in part, saved, or transferred only in accordance with our
3.00 / 01-2023




                                        license agreement. Transmission of the documentation is not allowed, neither
                                        electronically, nor mechanically, nor by recording or in any other way, without
                                        A+W Software GmbH prior approval in writing.


                 A+W Production Detailed Scheduling                                                                   D-3
                 Introduction




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
3.00 / 01-2023




                 D-4                                                   A+W Production Detailed Scheduling
                                                                                                                                                        Contents




                                        Contents
                                        Introduction ............................................................................................................. D-3
                                          Revision Overview ............................................................................................... D-3
                                          Editorial ............................................................................................................... D-3
                                        Contents ................................................................................................................. D-5

                                        Tutorial                                                                                                             D-9
                                        Notes on the Documentation ................................................................................ D-11
                                          Important Notes ................................................................................................. D-11
                                          Documentation .................................................................................................. D-13
                                            Tutorial Structure ........................................................................................... D-13
                                            Display Conventions ...................................................................................... D-14
                                        Detailed Scheduling - Overview ............................................................................ D-15
                                          The Process of Detailed Scheduling ................................................................. D-16
                                          Terms of Detailed Scheduling ........................................................................... D-18
                                            Lot Type ......................................................................................................... D-18
                                            Lots ................................................................................................................ D-19
                                              Application lot ............................................................................................. D-19
                                              Production lot .............................................................................................. D-19
                                            Racks ............................................................................................................. D-19
                                              Application rack .......................................................................................... D-20
                                              Production rack ........................................................................................... D-20
                                            Batches .......................................................................................................... D-20
                                              Archiving batches ....................................................................................... D-21
                                              Archiving method ........................................................................................ D-22
                                            Element Tree ................................................................................................. D-25
                                            Organization ................................................................................................... D-25
                                        Grouping and Sorting ............................................................................................ D-26
                                          Overview ........................................................................................................... D-27
                                            Introduction .................................................................................................... D-28
                                            Grouping ........................................................................................................ D-29
                                            Sorting ............................................................................................................ D-30
                                            Additional sorting ........................................................................................... D-33
                                            Special Elements ........................................................................................... D-34
                                              Filler Orders ................................................................................................ D-34
                                              Residue lites ............................................................................................... D-36
                                              Rejects ........................................................................................................ D-37
                                              Rush orders ................................................................................................ D-37
                                            Demos and Exercises .................................................................................... D-38
                                        Racks and Stacking Modes .................................................................................. D-40
                                          Overview ........................................................................................................... D-41
                                            Racks ............................................................................................................. D-42
                                            Logical Racks ................................................................................................. D-43
                                            Stacking Rules ............................................................................................... D-43
                                            Predefined Stacking Modes for A Racks ....................................................... D-45
                                              Glass mode ................................................................................................ D-45
                                              Unit mode ................................................................................................... D-46
                                              Production mode ........................................................................................ D-48
                                              VABGLA mode ........................................................................................... D-49
                                            Robot Racks .................................................................................................. D-51
                                            Modes for Harp Racks ................................................................................... D-51
3.00 / 01-2023




                                            Modes for Fixed Racks .................................................................................. D-51
                                          Standard Settings in the A+W Production Configuration .................................. D-51
                                          Rack Settings in Master Data ............................................................................ D-53
                                            Demos and Exercises .................................................................................... D-56


                 A+W Production Detailed Scheduling                                                                                                            D-5
                 Contents




                            Optimization Modes .............................................................................................. D-59
                              Overview ........................................................................................................... D-60
                                Different Optimization Modes ......................................................................... D-61
                                  Optimization mode 6.2 - fixed sequence .................................................... D-61
                                  Optimization mode 6.1 - keep customers together ..................................... D-63
                                  Optimization mode 5.2 - standard .............................................................. D-65
                                  Optimization mode 5.1 - IG on harp racks or many A racks ....................... D-67
                                  Optimization mode Free Optimization - lites on harp racks ........................ D-69
                                  Double optimization .................................................................................... D-70
                                Demos and exercises .................................................................................... D-71
                            Organizations ........................................................................................................ D-73
                              Organization Types ........................................................................................... D-74
                                General .......................................................................................................... D-75
                                Tree Structure ................................................................................................ D-75
                                Master Organization ....................................................................................... D-76
                                Reject Organization ....................................................................................... D-81
                                Sequence of checks ....................................................................................... D-81
                                Organization Type and Batch Type ............................................................... D-84
                                  Application and production organizations ................................................... D-84
                                Global settings ............................................................................................... D-85
                                Demos and Exercises .................................................................................... D-86
                              Production Sequence ........................................................................................ D-87
                                General .......................................................................................................... D-88
                                Grouping Key for Organization Groups .......................................................... D-88
                                  No grouping ................................................................................................ D-88
                                  Including grouping ...................................................................................... D-89
                              A+W Standard Organizations ............................................................................ D-91
                                Rack Organization ......................................................................................... D-92
                                  A racks spacers .......................................................................................... D-92
                                  IG A racks ................................................................................................. D-101
                                  A racks dispatch ....................................................................................... D-106
                                  Harp racks, no filling up ............................................................................ D-112
                                  Filled harp racks ....................................................................................... D-117
                                Demos and Exercises .................................................................................. D-122

                            Software Reference                                                                                              D-125
                            Overview ............................................................................................................. D-127
                            Organizations ...................................................................................................... D-128
                              Tab Master Organization ................................................................................. D-128
                              Tab Production Sequence ............................................................................... D-130
                              Tab Test Sequence ......................................................................................... D-132
                              Master Organization ........................................................................................ D-134
                              Organization .................................................................................................... D-138
                              Organization Groups ....................................................................................... D-140
                              Rack Settings .................................................................................................. D-142
                              Default Settings ............................................................................................... D-146
                            Grouping and Sorting .......................................................................................... D-147
                              Grouping/Sorting Dialog .................................................................................. D-147
                                Tab Editor - Grouping .................................................................................. D-147
                                Tab Editor - Sorting ...................................................................................... D-150
                                Tab Additional Sorting .................................................................................. D-151
                              Defining an Additional Sorting ......................................................................... D-152
                            Racks .................................................................................................................. D-153
3.00 / 01-2023




                              Racks .............................................................................................................. D-153
                            Lots ..................................................................................................................... D-158




                 D-6                                                                         A+W Production Detailed Scheduling
                                                                                                                                                 Contents




                                         Lot Types and Processings ............................................................................. D-158
                                            Tab Lot Types .............................................................................................. D-158
                                            Tab Processings .......................................................................................... D-161
                                            Tab Implicit Processing ................................................................................ D-163
                                        Detailed Scheduling of Batches .......................................................................... D-165
                                         Detailed Scheduling for Batch … .................................................................... D-165
                                            Tab Glass Types .......................................................................................... D-166
                                            Tab Rack Allocation ..................................................................................... D-169
                                            Tab Results .................................................................................................. D-174
                                            Tab Specials ................................................................................................ D-176
                                              Tab Nested Shapes .................................................................................. D-176
                                              Tab Filler Orders ....................................................................................... D-178
                                              Tab Residue Plates .................................................................................. D-180
                                              Tab Rejects .............................................................................................. D-181
                                              Tab Rush Order Lites ............................................................................... D-183
                                              Tab Thickness .......................................................................................... D-184
                                            Tab Free Optimization ................................................................................. D-186
                                            Tab Partial Quantities .................................................................................. D-187
                                            Tab Organization ......................................................................................... D-189
                                            Tab Organization Options ............................................................................ D-191
                                            Tab Options ................................................................................................. D-193
                                            Tab Stockplate Selection ............................................................................. D-195
                                         Change Minimum Number of A Racks ............................................................ D-196
                                         Sequence of Tables ........................................................................................ D-197

                                        Section Index                                                                                            D-199
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                                                      D-7
                 Contents
3.00 / 01-2023




                 D-8        A+W Production Detailed Scheduling
Detailed Scheduling         D

                        Tutorial




                A+W Production
                 Tutorial                                                                   Notes on the Documentation




                                        Notes on the Documentation
                                        The tutorial on module Detailed Scheduling deals with the basics of the whole
                                        production process. Starting from cutting, via the different production lines, up
                                        to the transport racks. It is based on the knowledge of rough scheduling.

                                            The functions depend on the released modules
                                            Please note that the individual functions are available only if the corre-
                                            sponding modules and interfaces have been installed and released.

                                            If you detect functions in this description which are not available in your ver-
                                            sion, please contact A+W Software GmbH.

                                        Sets of Topics
                                        The training on module Detailed Scheduling consists of the following sets of
                                        topics:
                                        •   Grouping and Sorting
                                        •   Racks and Stacking Modes
                                        •   Optimization Modes
                                        •   Organizations


                                        Important Notes
                                        This documentation is meant as an aid for the daily business and as a training
                                        document for software training accompanied by a certified A+W trainer. It is
                                        not meant for self-studies and cannot guarantee an operation which is com-
                                        pletely free of errors because the complexity does not depend on the software
                                        but rather on the real processes. Detailed scheduling defines the entire orga-
                                        nization and production process within your production. According to your re-
                                        quirements, it can be quite complex which is why it will be exclusively set up
                                        by an experienced member of the A+W team, and installed together with you.
                                        Should you want to change the settings please always contact A+W first to
                                        avoid undesired effects!
                                        The user has to be versed in the application of physical processes in glass pro-
                                        duction and organization.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                   D-11
                 Notes on the Documentation                                                                   Tutorial




                                        Product names
                                        In the course of strategic product realignment, the product range and product
                                        names of A+W have been simplified. ALCIM for instance has become A+W
                                        Production.
                                        Since the old as well as the new product versions have been adapted and ex-
                                        tended in the product development cycle, we shall be using only the old prod-
                                        uct names in this document to simplify matters - the new product versions are
                                        also covered by the old names.
3.00 / 01-2023




                 D-12                                                          A+W Production Detailed Scheduling
                 Tutorial                                                                    Notes on the Documentation




                                        Documentation
                                        Training on A+W Production is supported by the following documents:

                                        Hand-out                   Printed training documentation for the participants

                                        PDF                        Complete documentation
                                                                   • Tutorial
                                                                   • Software Reference
                                                                   • Index

                                        Online help <F1>           Context-sensitive dialog help in the A+W Production
                                                                   software reference.


                                        Tutorial Structure
                                        This tutorial consists of sets of topics with several sessions each. Each ses-
                                        sion consists of the following elements:

                                        Overview                  Each training session starts with an overview of the
                                                                  major topics:
                                                                   • Objectives: What shall be conveyed?
                                                                   • Benefit: What can this knowledge be used for?
                                                                   • Maxims: Which correlations are to be remembered?

                                        Concepts                   Concepts and terms of the corresponding training
                                                                   session will be explained first. This is followed by
                                                                   examples and operating instructions.

                                        Exercises                  For some of the sessions, exercises with certain tasks
                                                                   and suggested solutions are available.

                                        Cross references          At the end of each learning unit there is a section with
                                                                  cross reference pointing out the corresponding
                                                                  descriptions in the software reference.
                                                                   This shall help you to extend your new-found
                                                                   knowledge.


                                        Reading instructions
                                        The contents of a learning unit are based on the knowledge conveyed in the
                                        previous unit. We therefore recommend not to skip any learning units. The
                                        contents of a learning unit are based on the knowledge conveyed in the previ-
                                        ous unit. We therefore recommend not to skip any learning units.
                                        If you are already familiar with a subject you should at least read the summary
                                        at the start of the session in order to bring the main details to mind.
                                        The practical part of each training unit automatically includes the software ref-
                                        erence and the exercises on the cross references. This will provide a central
                                        thread through the entire documentation. The practical part of each training
3.00 / 01-2023




                                        unit automatically includes the software reference and the exercises on the
                                        cross references. This will provide a central thread through the entire docu-
                                        mentation.


                 A+W Production Detailed Scheduling                                                                       D-13
                 Notes on the Documentation                                                                       Tutorial




                                        Display Conventions
                                        Individual elements of the sentences are displayed in a special form. Their
                                        meanings are:

                                        Italics                  mark character strings describing the software
                                                                 elements, e.g. the dialog Grouping.

                                        Bold                     marks phrases to be entered via keyboard, e.g. the
                                                                 number 0.

                                        >                        shows the way to open a dialog, e.g. File > Import >
                                                                 Transfer file. Master data > Detailed scheduling >
                                                                 Organization

                                        []                       Square brackets mark the buttons in the dialog, e. g.
                                                                 [OK] to save the data.

                                        <>                       Pointed brackets refer to keys or shortcuts on the
                                                                 keyboard, e. g. <F1> is used to open the online help.
3.00 / 01-2023




                 D-14                                                           A+W Production Detailed Scheduling
                 Tutorial                                                                Detailed Scheduling - Overview




                                        Detailed Scheduling - Over-
                                        view
                                        The glass required for production is usually cut from stockplates on the cutting
                                        tables. Most companies have several, automatic cutting tables and at least
                                        one cutting table for manual cutting or shapes.
                                        After cutting, the lites are put onto racks depending on the next processing
                                        step (e.g. A racks); the rack is then moved to the next processing station.
                                        In a working area (e.g. cutting) or within a process chain (e.g. cutting > IG line),
                                        dwelling and processing times can very considerably. Among other things, this
                                        depends on the space available in this area for the racks onto which the lites
                                        are put, on the complexity of the stacking logic, and on the distance to be cov-
                                        ered in between steps. These are essential questions in terms of Detailed
                                        scheduling. If there is only little space for the racks behind the cutting table,
                                        this fact must be compensated by the appropriate optimization and the se-
                                        quence of lites so that as few racks as possible are needed and only little ad-
                                        ditional sorting is required.
                                        For assembly on the IG line, the lites of a unit have to be stacked as closely
                                        together as possible. They do not have to be put onto the same rack however.
                                        This means that depending on the optimization, sorting may have to take place
                                        before the line.




                                           Optimization result
                                           The optimization with the lowest waste is not always the chief target of
                                           A+W Production. This is the case for instance if such an optimization re-
                                           sults in an unreasonable amount of sorting work before assembly.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-15
                 Detailed Scheduling - Overview                                                                         Tutorial




                                         An important criterion for detailed scheduling results and the dwelling and pro-
                                         cessing time is the size and composition of batches. Various aspects have to
                                         be taken into account:
                                         •   If a job contains only a few lites, or only very large lites, there will be too
                                             much waste. The stockplates cannot be cut to the best effect; the residue
                                             plate will be too big.
                                         •   If the job is too big however, i. e. if it consists of a large number of lites, the
                                             production time for this job is extended and the racks will be occupied for
                                             quite a long time. Racks can be used again only after the production of this
                                             batch is completed.


                                         The Process of Detailed Scheduling
                                         Detailed scheduling begins just where rough scheduling ends. Rough sched-
                                         uling results in jobs. Jobs contain elements to be produced. The task of de-
                                         tailed scheduling is to determine a production sequence for the elements of
                                         these jobs.
                                         The production sequence can be determined by criteria like:
                                         •   Customer's requirements,
                                         •   results of packing optimization (PMO), or
                                         •   production restrictions
                                         Detailed scheduling consists of various steps. All necessary processes (load-
                                         ing data from the database, etc.) are run in the background, invisible to the us-
                                         er. The steps are based on each other:
                                         •   In the first step, data are loaded from the database.
                                         •   After this, detailed scheduling creates a bill of material based on the ele-
                                             ments and the processing required.
                                         •   After the bill of material was created, detailed scheduling allocates the ele-
                                             ments to the available organizations and rack types.
                                         •   Now, grouping and sorting takes place within the organization groups and
                                             on the racks.
                                         •   As a next step, detailed scheduling deals with putting the lites onto racks.
                                         •   Next, production jobs are created.
                                         •   In the last step, detailed scheduling handles special elements (residue
                                             plates, filler orders, breakage, etc.)
                                         The primary products have to be put into a suitable sequence onto the racks
                                         to produce the sequence required for the individual production steps. The rack
                                         load after each production step results from the production sequence.
3.00 / 01-2023




                 D-16                                                                A+W Production Detailed Scheduling
                 Tutorial                                                                Detailed Scheduling - Overview




                                        The following illustration shows the symbolic effects of the different settings in
                                        A+W Production.

                                                                   Sequence




                                        Yield                                                 Flexibility



                                        You can define just one spot on the triangle. You can move this spot by chang-
                                        ing the production settings by means of A+W Production.
                                        You can work in just one corner of the triangle, ignoring the other two. You can
                                        also move along one side, right in the middle of two corners, ignoring the third
                                        corner. At present, production cannot take all three corners into account at the
                                        same time.
                                        •   You can apply a strict sequence (in one corner) - this will impede flexibility
                                            and also the results.
                                        •   You can apply a combination of sequence and yield (on one side) - which
                                            means that you are no longer flexible.
                                        •   …
                                        We are going to use this pattern time and again in this documentation.


                                        Additional information
                                         Tutorial, “Terms of Detailed Scheduling” on page D-18
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-17
                 Detailed Scheduling - Overview                                                                         Tutorial




                                         Terms of Detailed Scheduling
                                         The following terms are used in connection with A+W Production:
                                         •   Lot Type
                                         •   Lots
                                             – Application lot
                                             – Production lot
                                         •   Racks
                                             – Application rack
                                             – Production rack
                                         •   Element Tree
                                         •   Organization


                                         Lot Type
                                         The lot type is defined by the properties Processing type and Procurement
                                         type.




                                         Fig. D-1     Schematic display of the lot types cutting and stock withdrawal
3.00 / 01-2023




                 D-18                                                              A+W Production Detailed Scheduling
                 Tutorial                                                               Detailed Scheduling - Overview




                                        Lots
                                        A lot is a number of lites which are used or produced on the same machines
                                        and under the same conditions within a defined space of time. A lot contains
                                        a number of lites of the same Lot type. In A+W Production, there are two lot
                                        types:
                                        •   Application lot
                                        •   Production lot

                                        Application lot
                                        The lites of an application lot are necessary for producing the lites in the batch-
                                        es. All lites of this lot have the same lot type.

                                        Production lot
                                        The lites of a production lot are produced in the corresponding job. All lites
                                        have the same lot type. lites of a production lot are produced on the same ma-
                                        chines. lites destined for another machine are assigned to another lot of the
                                        same type. Also, production lots can be separated by other criteria. It is possi-
                                        ble for instance to split the production of IG units by spacer. This way, several
                                        production lots would be created each of which contains only lites with a cer-
                                        tain spacer.


                                        Additional information
                                         Abb. D-2 on page D-20


                                        Racks
                                        Elements of a job can be treated differently after they were cut. The elements
                                        are put onto racks for the next processing step. The always belong to an ap-
                                        plication lot, i.e. they are necessary for production. Therefore, they have to be
                                        put on the application racks in such a way that the sequence can be main-
                                        tained for the next processing step.
                                        A+W Production distinguishes
                                        •   Application rack
                                        •   Production rack
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-19
                 Detailed Scheduling - Overview                                                                     Tutorial




                                         Application rack
                                         Elements of a batch can be treated in different ways after they have been cut.
                                         The elements are put onto an application rack for the next processing step.
                                         The always belong to an application lot, i.e. they are necessary for production.
                                         Therefore, they have to be put on the application racks in such a way that the
                                         sequence can be maintained for the next processing step.



                                                               Processing


                                                                               Application Lot
                                                               Application
                                                                  Rack


                                                               Production      Production Lot
                                                                  Racl
                                          Time




                                                               Processing



                                                                               Application Lot
                                                               Application
                                                                  Rack



                                         Fig. D-2         Production and application rack - overview


                                         Production rack
                                         Right after production, lites are put onto production racks. The sequence of the
                                         lites on the rack is the sequence in which they have been produced. These li-
                                         tes belong to the same production lot. Production racks do not have to be used
                                         for A+W Production at any cost; the lites can as well be put onto application
                                         racks for the next processing step.

                                                 Production and application racks
                                                 A+W Production allows to use a different grouping/sorting for every pro-
                                                 cessing step. A production rack cannot be simply assigned a different num-
                                                 ber in order to use it as an application rack for the next processing step.
                                                 When lites are put onto an application rack (instead of a production rack)
                                                 after processing, they have to be stacked in such a way that the production
                                                 sequence for the next processing step can be maintained.


                                         Additional information
                                          Software Reference, “Racks” on page D-153


                                         Batches
3.00 / 01-2023




                                         Batches contain a set of order items that are released together for production
                                         and produced together.



                 D-20                                                                   A+W Production Detailed Scheduling
                 Tutorial                                                             Detailed Scheduling - Overview




                                        Archiving batches
                                        Batches that you no longer need in the production system can be archived. In
                                        the Batches display, with the context menu (Manage batch > Archive batch),
                                        you can set the selected batch and the selected batches to "archivable". Ar-
                                        chived batches then have the batch status 2000.
                                        There are 2 types of archiv:
                                        •   Manual archiving
                                        •   Automatic archiving

                                        Manual archiving
                                        The settings for the manual archiving are in the parameter administrator un-
                                        der:
                                        Parameters > A+W Production > General > ALCIM Server > Automatic Batch
                                        Archiving
                                        The entry for the manual archiving is 0.
                                        After the batch has been archived, it has the status archivable. Whether a
                                        batch is actually archived or should be deleted instead can be defined in the
                                        system configuration. For the archiving of a batch, an archive database and a
                                        process (ALCIM server) are required. This process can be started manually or
                                        is configured as automatic in the background.


                                         How to archive a batch
                                        1 Open the Batches view.
                                        2 Mark the batch that you want to archive or delete.
                                        3 Open the context menu and select Manage batch > Archive batch.
                                        4 You will then see a security query asking whether you really want to archive
                                          the batch.




                                        5 Click [OK] to archive the batch.
                                        6 Then the batch has the status archivable.

                                        Automatic archiving
3.00 / 01-2023




                                        In addition to manual archiving, there are now 3 new archiving modes that re-
                                        fer to batch statuses 700 (produced), 800 (packed) and 900 (sent). These
                                        batch statuses are automatically set by AlcimBooking as soon as all header


                 A+W Production Detailed Scheduling                                                             D-21
                 Detailed Scheduling - Overview                                                                   Tutorial




                                         parts in the batch have received the processing steps for produced, packed or
                                         delivered.
                                         The settings for the automatic archiving are in the parameter administrator un-
                                         der:
                                         Parameters > A+W Production > General > ALCIM Server > Automatic Batch
                                         Archiving
                                         Here you can distinguish among:
                                         •   Batches are archived automatically if the status produced is reached.
                                         •   Batches are archived automatically if the status packed is reached.
                                         •   Batches are archived automatically if the status delivered is reached

                                             Booking discipline
                                             The automatic archiving is based on PDC bookings and therefore depends
                                             on the booking discipline. As soon as a header part in a batch does not re-
                                             ach the appropriate status, the batch status cannot be set and thus the au-
                                             tomatic archiving is initiated. Therefore, attention has to be paid that
                                             especially the header parts are booked completely.

                                             Essentially it applies that: a complete archiving of a batch can only be done
                                             when dependent batches (which contain common order items) are also in
                                             this status.

                                         Archiving method
                                         In this area, you select which archiving method should be used. The old archi-
                                         ving method (which is set by default and used) is available and the new exten-
                                         ded, which is less restrictive and allows more batches to be archived and
                                         released.
                                         The settings for the archiving method are in the parameter administrator un-
                                         der:
                                         Parameters > A+W Production > General > ALCIM Server > Archiving Method
                                         Here you can distinguish among:
                                         0: Standard archiving method.. This method works only based on the status of
                                         a batch.
                                         1: expanded checking of the batches. Here additional flags of the orders are
                                         considered in a batch in order to check whether an order can be archived. This
                                         method is less restrictive than the original method and allows the archiving and
                                         releasing of more batches. The parameter that underlies this method tells the
                                         AlcimServer starting with which status a batch should be regarded as archiva-
                                         ble. The value of the Automatic batch archiving can be
                                         •   1=Status 700 (produced),
                                         •   2=Status 800 (packed),
                                         •   3=Status 900 (delivered) oder
                                         •   0=Status 2000 (set manually as archivable).
3.00 / 01-2023




                                          Tutorial, “Automatic archiving” on page D-21




                 D-22                                                             A+W Production Detailed Scheduling
                 Tutorial                                                              Detailed Scheduling - Overview




                                        How standard archiving method (0) works
                                        As mentioned above, this method works only based on the status of a batch.
                                        This is clear in the following example:
                                        •   Batch: 1000
                                        •   Status: 900 (sent)
                                        •   Configuration parameter Automatic batch archiving: 3 (batches are archi-
                                            ved automatically when the status sent is reached)




                                        Fig. D-3      Standard archiving method (0)


                                        How this works: if the AlcimServer processes the batch 1000 (column A) with
                                        a status equal to or greater than 3 (status 900, send), it checks in the 1st step
                                        all orders of the batch 1000 (column D). In the 2nd step, it checks in which ot-
                                        her batches these are contained (column F) and in the 3rd step, whether the
                                        batches all have a status equal than or greater to status 3.
                                        In the example above, the order 2000001 cannot be archived. In addition to
                                        batch 1001, it contains batch 1002 and this batch only has the status 700 (pro-
                                        duced). Since this is less than "archivable status," batch 1000 cannot be archi-
                                        ved.

                                        How extended archiving method (1) works
                                        This new method was created in order to be able to archive more batches.
                                        The new method enables the archiving of orders that can be regarded as com-
                                        pleted, even if they are included in another batch with a status less than "ar-
                                        chivable status" but with a status equal to or greater than 700 (= produced).
                                        Example:
                                        •   Batch: 1000
                                        •   Status: 900
                                        •   Configuration parameter Automatic batch archiving: 3 (batches are archi-
                                            ved automatically when the status sent is reached)
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                D-23
                 Detailed Scheduling - Overview                                                                   Tutorial




                                         Fig. D-4     Extended archiving method (1)


                                         If the status of the batch is 700 or equal to and less than "archivable status,"
                                         then other data records from pool_teile and pool_auftrag also have to be ana-
                                         lyzed.
                                         Part of an order 2000001 [column D], which is included in the batch 1001 [co-
                                         lumn F] does not have to be analyzed since the status [column G] of this batch
                                         is equal than or greater to archivable status.
                                         But another part of an order 2000001 [column D], which is included in the
                                         batch 1002 [column F] must be analyzed since the status [column G] of this
                                         batch 700 is equal to or less than "archivable status".
                                         The condition that this part of the order 2000001 [column D] counts as archi-
                                         vable is that all pool_teile data records for the specified batch and given order
                                         have set at least one of bdefertig | bde_verpack | bde_versendet flags [co-
                                         lumns K,L,M] set to a value not equal to zero or that the auftkz value of the
                                         pool_auftrag has to be greater than zero (canceled).
                                         As you can see in comparison to the standard method, the new method con-
                                         siders the order 2000001 [column D] as archivable and thus the batch 1000
                                         can be archived.
3.00 / 01-2023




                 D-24                                                             A+W Production Detailed Scheduling
                 Tutorial                                                                     Detailed Scheduling - Overview




                                        Element Tree
                                        The element tree describes the structure and the production steps of a prod-
                                        uct. The finished product (IG) is the head of the element tree; the sub-ele-
                                        ments required for production (toughened glass and A+W Therm) are
                                        arranged below and the sub-elements thereof (float glass) again on the level
                                        below. This continues down to the basic elements (usually float). The produc-
                                        tive processing steps (insulating, cutting, toughening) are arranged on the
                                        same level as the elements. The following processing steps are arranged in
                                        ascending order.




                                        Fig. D-5         Element tree (example)


                                        Organization
                                        A+W Production offers so-called organizations for planning batches correctly
                                        and efficiently. An organization is a set of technical rules for handling the pro-
                                        duction processes. Depending on the company's structure, any number of or-
                                        ganizations (toughened glass organization, IG organization, processing
                                        organization, etc.) can be defined. The individual organizations organize the
                                        racks for the production steps (IG line, furnace, etc.).

                                         Master Organization

                                                       Organization 1


                                                      Organization 2

                                                               Organization Group 1

                                                               Organization Group 2

                                                                      Rack Type 1

                                                                      Rack Type 2
3.00 / 01-2023




                                                               Organization Group 3


                                        Fig. D-6         Schematic view of the organization



                 A+W Production Detailed Scheduling                                                                   D-25
                 Grouping and Sorting                                                                         Tutorial




                                        Grouping and Sorting
                                        This subject area introduces the different grouping and sorting options and
                                        shows you how to use them for A+W Production.
                                        This subject area includes the following training sessions:
                                        •   Introduction
                                        •   Grouping
                                        •   Sorting
                                        •   Additional sorting
                                        •   Demos and Exercises
3.00 / 01-2023




                 D-26                                                           A+W Production Detailed Scheduling
                 Tutorial                                                                               Grouping and Sorting




                                        Overview
                                        Objectives

                                        •   Knowing and understanding grouping
                                        •   Knowing and understanding sorting
                                        •   Knowing and understanding additional sorting
                                        •   Understanding the effects of grouping and sorting


                                        Benefit

                                        Grouping and sorting serves to organize the stacking of the individual lites in the
                                        required sequence. Without grouping and sorting, the lites would have to be resorted
                                        prior to every production step.


                                        Definitions

                                        Grouping                     is done by different, unique values for a property, e. g. by
                                                                     customer number, glass thickness.

                                        Sorting                      is based on properties which assume a progressive
                                                                     value within the defined group (e.g. size).

                                        Rack                         Rack (A rack, harp rack, fixed rack)

                                        Rack                         Colloquial term for 'rack'.


                                        Note

                                        Creation                     Grouping or sorting is created by random combinations
                                                                     of properties and formulas.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                        D-27
                 Grouping and Sorting                                                                            Tutorial




                                        Introduction
                                        The groups and sorting allows to allocate the required production sequence to
                                        the individual racks. Groups can also be used to distribute lites of the same lot
                                        type to different production lots.
                                        A+W Production allows defining grouping criteria and deciding whether group-
                                        ing shall be done in a certain sequence (sorted groups) or whether the con-
                                        tents of the groups shall be sorted (sorting within the group). Every rack type
                                        of an organization can have its own grouping and sorting.
                                        Optimization calculates the optimum yield taking into account the grouping
                                        and sorting. Once it has been set up, the defined sequence can be used for
                                        matching lites of an IG and laminated glass unit.
                                        Every lite and processing step has a number of properties which are either de-
                                        fined by the corresponding fields in the database, or are calculated.

                                                           Grouped by glass type




                                         Sorted by size

                                        Fig. D-7     Grouping and Sorting


                                        The illustration above shows lites grouped by thickness. Within each group
                                        (perhaps one rack per thickness), lites are sorted by height.
                                        Grouping and sorting depend on how your production is organized and being
                                        run. They are defined by a random combination of properties and formulas.
                                        The settings are made in menu Master data, in the sub-menus Organization,
                                        Grouping, and Racks.


                                        Additional information
                                         Tutorial, “Grouping” on page D-29
                                         Tutorial, “Sorting” on page D-30
3.00 / 01-2023




                 D-28                                                              A+W Production Detailed Scheduling
                 Tutorial                                                                         Grouping and Sorting




                                        Grouping
                                        Grouping is done by different, unique values for a property, e.g. by Customer
                                        number, glass thickness/colour, type of shape. Groups can be formed by var-
                                        ious criteria; the groups do not have to be sorted internally. Every group con-
                                        tains only elements that match the properties of the grouping key. Groups must
                                        be kept together throughout the production process.
                                        The corresponding settings are made in dialog Grouping/Sorting:
                                        Master Data > Detailed Scheduling > Grouping




                                        Fig. D-8      Grouping


                                         How to define a new group
                                        1 Go to menu Master Data > Detailed Scheduling > Grouping.
                                           Dialog Grouping/Sorting appears. Tab Sorting opens automatically.
                                        2 In the left section, choose the entry Grouping.
                                        3 Tick the checkbox Property or Formula to define whether the sorting is a
                                          property or a formula.
                                        4 Choose the appropriate property or formula.
                                        5 Press the [Add] button.
                                        6 The entry is added at the end of the list on the left side.
                                        The new group can now be used for settings regarding organizations.


                                        Additional information
                                         Tutorial, “Introduction” on page D-28
                                         Software Reference, “Grouping/Sorting Dialog” on page D-147
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                              D-29
                 Grouping and Sorting                                                                                              Tutorial




                                        Sorting
                                        You can sort by properties which take progressive values. Typical for instance
                                        is sorting by size. Sorting is done within the defined groups. If required, sorting
                                        can be refined by the values in the last part of the sorting key.

                                                                     Sequence of groups

                                           Customer #       sorted                    unsorted                   unsorted




                                                                        Customer #




                                                                                                  Customer #
                                                        Group 1                      Group 2                    Group 3

                                                                                                               Glass: Float 4 mm

                                        Fig. D-9             Grouping and Sorting


                                        As you can see from the figure above, you can also define a sequence of
                                        groups.

                                            Super groups
                                            Optimization uses the term Super group. A super group can consist of lites
                                            which have the same grouping key or combined grouping/sorting key.

                                        lites within a group can be sorted, but do not have to be.
                                        The corresponding settings are made in dialog Grouping/Sorting:
                                        Master Data > Detailed Scheduling > Grouping > tab Sorting




                                        Fig. D-10            Sorting
3.00 / 01-2023




                 D-30                                                                            A+W Production Detailed Scheduling
                 Tutorial                                                                         Grouping and Sorting




                                         How to define a new sorting
                                        1 Go to menu Master Data > Detailed Scheduling > Grouping.
                                           Dialog Grouping/Sorting appears. Switch to tab Grouping.
                                        2 In the left section, select the entry Sorting.
                                        3 Tick the checkbox Property or Formula to define whether the group is a
                                          property or a formula.
                                        4 Choose the appropriate property or formula.
                                        5 Press the [Add] button.
                                        6 The entry is added at the end of the list on the left side.


                                         How to add a property to an existing sorting
                                        1 Go to Master Data > Detailed Scheduling > Grouping > Editor-Sorting.
                                        2 Tick the radio button Properties.
                                        3 Select the property for this sorting in the window on the right.
                                        4 In the left window, select the sorting to which the property shall be added.
                                        5 Press the [Add] button. The new property will appear among the existing
                                          ones.


                                         Defining a new mode for group formation
                                           As an example, we will define groups acc. to the number of lites, per cus-
                                           tomer. This means that we will define a group per customer; these groups
                                           shall be sorted by the number of lites the include. The group with the largest
                                           number of lites will be produced first.
                                        1 Go to menu Master Data > Detailed Scheduling > Grouping
                                        2 Tick the radio button Formula then press button [Formulas …]. Dialog Se-
                                          lect formulas --1-- appears
                                        3 Press button [New formula …]. The dialog Formula - Editor appears.
                                        4 In the top left corner of the formula editor, enter the name of the group (in
                                          this case: number of lites per customer).
                                        5 In section Existing formulas, search for the Quantity and double-click on it.
                                          The formula #Quantity# will be adopted in section Formula.
                                        6 Press the [Quantity] button. The dialog Select quantity --1-- appears.
                                        7 In the top left corner of the dialog, existing quantities (in the sense of set
                                          theory) can be selected. Define a new quantity then click on [New
                                          quantity …]. This opens dialog Quantity - Editor.
                                        8 Starting from a given quantity we will perform quantity operations to get the
                                          final quantity. Detailed scheduling transfers to the formula interpreters val-
                                          ues for a customer's item, the quantity calculation, and all orders of the job
3.00 / 01-2023




                                          on hand. Just add the customer number.
                                          Select Quantity > Name. The dialog Quantity name appears. Enter a char-




                 A+W Production Detailed Scheduling                                                                D-31
                 Grouping and Sorting                                                                           Tutorial




                                           acteristic name for the quantity in field New Name. Select [OK]. The dialog
                                           closes.
                                        9 Select Quantity > Transferred quantity. As a result, not only the item used
                                          to start the quantity editor will be considered for quantity calculation, but
                                          also all items of the job.
                                        10 As the required quantity shall not contain all elements but only the released
                                           ones, tick the checkbox Master. For an explanation of the available options,
                                           please refer to
                                        11 To add the customer number as a property, select Quantity > Formula. The
                                           dialog Select formulas --2-- appears. Section Existing formulas shows all
                                           existing formulas. If the customer number does not exist yet, click on [New
                                           formula …]. The dialog Formula editor appears. In the formula editor, enter
                                           a name for the formula, select CUSTOMERNUMBER in section Existing
                                           Properties, and double-click on the property. This property will appear in
                                           field Formula. Press [OK] to create the formula.
                                        12 Close the dialog Select formulas --2-- using [OK].
                                        13 Dialog Quantity editor shows (bottom right) that this formula will be used to
                                           define the new quantity. We do not use a condition to define the required
                                           quantity. Conditions are defined in menu Quantity. The difference between
                                           formula and condition in connection with quantities is that while a condition
                                           always includes an absolute value, this refers to a certain item in connec-
                                           tion with a formula, so that the value may differ.
                                        14 Close all open dialogs by [OK] until you are back in dialog Grouping/Sort-
                                           ing. Select the new formula (number of lites per customer) then press
                                           [Add].
                                        15 Dialog Organizations groups and Rack settings now shows the defined
                                           group (number of lites per customer) in section Group formation; this can
                                           be used as required.


                                        Additional information
                                         Tutorial, “Sorting” on page D-30
                                         Software Reference, “Grouping/Sorting Dialog” on page D-147
3.00 / 01-2023




                 D-32                                                           A+W Production Detailed Scheduling
                 Tutorial                                                                           Grouping and Sorting




                                        Additional sorting
                                        Additional sorting can be applied only to the sorting itself. The aim of additional
                                        sorting is to complete the existing sorting depending on the value of the last
                                        element. You might, for instance, require a sorting by route, customer, and
                                        xxxxx; while xxxxx should be different for every customer. Therefore, you first
                                        sort by route and customer, then define all sorting options required for xxxxx.
                                        After this, the additional sorting can be allocated to the sorting by route and
                                        customer, based on the customer number. If there is no additional sorting for
                                        a given customer number, there will be no additional sorting.


                                         How to define an additional sorting
                                           Example: An existing sorting by route and customer is completed by an ad-
                                           ditional sorting by order number and item number for customer number 11.
                                        1 Go to Master data > Detailed scheduling > Grouping > Editor-Sorting.
                                        2 Tick the radio button Properties.
                                        3 Select the sorting in the left window (+order number+item number) the ad-
                                          ditional sorting shall apply to.
                                        4 Select the property for this additional sorting (customer number) in the win-
                                          dow on the right.
                                        5 Use button [Define additional sorting]. The dialog Define Additional Sorting
                                          appears.
                                            Software Reference, “Defining an Additional Sorting” on page D-152
                                        6 In field Value, enter the value for the sorting element (in this case, 11).
                                            Software Reference, “Value” on page D-151
                                        7 Tick the radio button Number.
                                        8 Press [OK]. The dialog closes.
                                        9 Open tab Additional sorting. The defined additional sorting appears (in this
                                          case: Key: Customer number, value: 11, additional sorting: +Order num-
                                          ber+Item number).


                                        Additional information:
                                         Tutorial, “Grouping” on page D-29
                                         Software Reference, “Defining an Additional Sorting” on page D-152
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-33
                 Grouping and Sorting                                                                             Tutorial




                                        Special Elements
                                        There is no grouping or sorting for special items as there is only one item per
                                        rack.
                                        Special items are:
                                        •   Filler Orders
                                        •   Residue lites
                                        •   Rejects
                                        •   Rush orders

                                        Filler Orders
                                        Filler orders are lites that do not firmly belong to a batch but can be used by
                                        the optimization for improving the yield. Filler orders are found in the database
                                        table POOL_TEILE, and are defined by the job number 10003. A+W Produc-
                                        tion offers a special view for filler orders, the so-called Filler order view. The
                                        filler order view does not appear by default but has to be activated by the user.

                                            Show filler orders
                                            To be able to use existing filler orders and show them on tab Special in di-
                                            alog Detailed scheduling for job …, you need to activate the section Use
                                            fillers in dialog Master Organization and define the appropriate racks!

                                            Should you want to change the settings please always contact A+W first to
                                            avoid undesired effects!


                                         How to activate the filler order view
                                        1 Go to menu Master Data > Configuration. Dialog Parameter administrator
                                          appears.
                                        2 Select the terminal in section ALCIM, General.
                                        3 Scroll to section Program menu on the right side.
                                        4 Select the line below (menu).
                                        5 Click on the button […] at the end of the line.
                                        6 Dialog Character String Editor opens.
                                        7 Go to the end of the list and enter the word Filler.
                                        8 Quit the dialog via button [OK]
                                        9 To make an amendment, you have to restart A+W Production.
3.00 / 01-2023




                 D-34                                                            A+W Production Detailed Scheduling
                 Tutorial                                                                         Grouping and Sorting




                                        Fig. D-11     Filler order view


                                        Additional information
                                         Software Reference, “Use Filler” on page D-136
                                         Software Reference, “Tab Filler Orders” on page D-178
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-35
                 Grouping and Sorting                                                                             Tutorial




                                        Residue lites
                                        You can click on an item in dialog Detailed Scheduling, tab Results and view
                                        the cutting pattern by using the button [PlanEdit]. In case of too much waste
                                        for example, you can resolve the lites of the last plate via the [Resolve] button.
                                        As a result, the lites will be returned to table FEIN_TEILE with job number
                                        10005, and can be cut later.
                                        These residue lites are also found on tab Special, tab Residue plates. They
                                        can be selected for a suitable job later on.
                                        Alternatively, lites can remain on the resolved residue plates in the original
                                        batch, and can be cut manually. In this case, they will not be entered in table
                                        FEIN_TEILE with job number 10005.

                                           Show residue plates
                                           To be able to use existing filler orders, and show them on tab Special in di-
                                           alog Detailed scheduling for job …, you need to activate section Use resi-
                                           due plates in dialog Master organization, and define the appropriate racks!

                                           Should you want to change the settings please always contact A+W first to
                                           avoid undesired effects!




                                        Fig. D-12    Master organization, Activation of residue plates


                                        Additional information
                                         Software Reference, “Use Residue Plates” on page D-136
                                         Software Reference, “Tab Residue Plates” on page D-180
3.00 / 01-2023




                 D-36                                                             A+W Production Detailed Scheduling
                 Tutorial                                                                           Grouping and Sorting




                                        Rejects
                                        Breakage is transferred to table FEIN_TEILE with job number 10000. It can be
                                        added to the required job at detailed scheduling. For rush orders, breakage will
                                        be cut manually, however.

                                           Show rejects
                                           To be able to use existing filler orders, and show them on tab Special in di-
                                           alog Detailed Scheduling for Batch … you need to activate section Use Re-
                                           jects in dialog Master Organization and define the appropriate racks!




                                        Fig. D-13     Master organization, Activation of breakage


                                        Additional information
                                         Software Reference, “Use Rejects” on page D-137
                                         Software Reference, “Tab Rejects” on page D-181

                                        Rush orders
                                        This function allows to enter lites quickly, and pass them on to production. You
                                        do not have to enter the lites via order entry, then transfer them to production.
                                        High-priority lites are entered in dialog Rush orders. This dialog is accessible
                                        via
                                        Extras > Rush orders
                                        High-priority lites are transferred to table FEIN_TEILE with job number 10002.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                D-37
                 Grouping and Sorting                                                                         Tutorial




                                        Demos and Exercises
                                        In this section you can use your newly acquired knowledge regarding grouping
                                        and sorting in practical exercises.

                                        Trainer demo: Explain grouping and sorting
                                        Grouping and sorting options are presented and described.
                                        The following dialog is explained from this point of view:
                                        •   Dialog Grouping/Sorting

                                        Exercise 1: Add a new group
                                        Add the existing group with the property Customer number as a new group.

                                        Exercise 1: Solution
                                        The result of this exercises looks like that:




                                        Fig. D-14    Groups


                                        The new group can now be used for settings regarding organizations.

                                        Exercise 2: Add another group to an existing one
                                        To the just defined group Customer number, add the group Order number.

                                        Exercise 2: Solution
                                        The result of this exercises looks like that:




                                        Fig. D-15    Further grouping


                                        Exercise 3: Add a new sorting
                                        Add the existing sorting with the property Item number as a new sorting.
3.00 / 01-2023




                 D-38                                                             A+W Production Detailed Scheduling
                 Tutorial                                                                       Grouping and Sorting




                                        Exercise 3: Solution
                                        The result of this exercises looks like that:




                                        Fig. D-16     Sorting


                                        The new sorting can now be used for settings regarding organizations.

                                        Exercise 4: Add another sorting to an existing one
                                        To the just defined sorting Item number, add the sorting Large_Size.

                                        Exercise 4: Solution
                                        The result of this exercises looks like that:




                                        Fig. D-17     Further sorting


                                        Additional information
                                         Tutorial, “Grouping” on page D-29
                                         Tutorial, “Sorting” on page D-30
                                         Software Reference, “Grouping/Sorting Dialog” on page D-147
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-39
                 Racks and Stacking Modes                                                                  Tutorial




                                       Racks and Stacking Modes
                                       This subject area introduces the different racks and stacking modes and
                                       shows you how to use them for A+W Production.
                                       This subject area includes the following training sessions:
                                       •    Introduction
                                       •    Racks
                                       •    Logical Racks
                                       •    Stacking Rules
                                       •    Predefined Stacking Modes for A Racks
3.00 / 01-2023




                 D-40                                                          A+W Production Detailed Scheduling
                 Tutorial                                                                       Racks and Stacking Modes




                                        Overview
                                        Objectives

                                        • Knowing and understanding racks
                                        • Knowing and understanding stacking modes
                                        • Understanding the effects of the stacking modes


                                        Benefit

                                        Once you have understood the functions of the stacking modes you can organize your
                                        production accordingly. A well-organized production will save time, space, and money.


                                        Definitions

                                        Physical rack                Rack (A rack, L rack, fixed rack)

                                        Logical rack                 A logical rack is an area on a physical rack with a certain
                                                                     number, onto which glass stacks can be put that belong
                                                                     together. A logical rack consists of one or more stacks of
                                                                     glass and defines how these stacks belong together (e.g.
                                                                     to turn them into IG or laminated glass units). This
                                                                     depends on the selected stacking mode.


                                        Note

                                        What can be put on a rack? Generally, only parts of a batch can be put onto a stack
                                                                   or on a harp rack.

                                        Different glass types on a   The program generally separates different glass types
                                        stack                        and allocates them to different stacks. You do not have to
                                                                     define a special logic for this.

                                        Stacking mode: Glass         In this case, one glass type is put onto a rack. Every
                                                                     stack gets its own rack number. Contrary to the VABGLA
                                                                     mode, lites will be put onto a stack only if their counter-
                                                                     panes can be stacked together as well.

                                        Stacking mode: Unit          Here, each unit is put onto a logical rack.

                                        Stacking mode: Production In this case, different glass types can be combined on a
                                                                  logical rack.

                                        Stacking mode: VABGLA        For every glass type, there is a logical rack with just one
                                                                     stack.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                       D-41
                 Racks and Stacking Modes                                                                      Tutorial




                                       Racks
                                       This chapter deals with the logical racks and the appropriate stacking modes.
                                       The subjects are:
                                       •    Logical Racks
                                       •    Stacking Rules
                                       •    Modes for Harp Racks
                                       •    Modes for Fixed Racks
                                       A+W Production offers various criteria for setting lites onto racks. You can put
                                       complete groups onto a rack, split groups, etc.
                                       This way, racks and stacking modes can be used for achieving a good yield
                                       while keeping a fixed production sequence. Production can be freely defined
                                       as well as the red point inside the red circle.

                                            Racks
                                            Please note that we will always be talking about racks here because we do
                                            not know whether a customer uses physical or logical racks. The size and
                                            width of the racks used by the customers are not known to us either.

                                                                 Sequence




                                       Yield                                               Flexibility
3.00 / 01-2023




                 D-42                                                           A+W Production Detailed Scheduling
                 Tutorial                                                                       Racks and Stacking Modes




                                        Logical Racks
                                        A logical rack consists of one or more stacks of glass and defines how these
                                        stacks belong together (e.g. to turn them into IG or laminated glass units). This
                                        depends on the selected stacking mode.
                                        A logical rack is an area on a physical rack with a certain number, onto which
                                        glass stacks can be put that belong together. lites are put onto logical racks
                                        usually in the production sequence defined for the corresponding rack.
                                        Physical racks are created from the logical racks. For A racks and fixed racks,
                                        this is done considering the rack width, the number of rack sides (1 or 2 for L
                                        or A racks respectively), and the maximum weight allowed for the rack.


                                        Stacking Rules
                                        •   Different glass types will always be separated.
                                        •   The defined stacking width must not be exceeded. Hence the question
                                            whether the system is allowed to separate groups, or keep them together.
                                        •   Large lites are usually put onto the rack first. Therefore, these have to be
                                            produced first, or resorting is required before the lites are put onto the rack.
                                            You have to define clear conditions or you can use the formula editor to de-
                                            fine certain restrictions.
                                        •   Stacking modes can be used to define how the system shall put units and
                                            groups on the physical and logical racks (a physical rack can offer enough
                                            space for several racks with different numbers = logical racks).




                                                                                                                 Maximum load




                                                                                      Logical rack 1001    Logical rack 1002
                                               Rack, side view
                                                                                               Rack, top view
                                        Maximum load             Maximum load
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                            D-43
                 Racks and Stacking Modes                                                                                        Tutorial




                                       One group per stack
                                       If you choose this setting,
                                       •    every group will be put onto one stack.
                                       •    if a group has to be split up (because the maximum weight is exceeded), it
                                            is split into two stacks - if the same or a new rack number (logical rack) will
                                            be used for the second stack, depends on the stacking mode.


                                                                                       Maximum load
                                            Group 1




                                                                    Group 2
                                              Logical rack 1001      Logical rack 1002
                                                      Rack, top view




                                       Complete groups can be stacked together
                                       If you choose this setting,
                                       •    different, complete groups will be put onto the same stack (considering the
                                            maximum weight allowed).


                                                                                       Maximum load
                                            Group 1




                                                                    Group 2




                                              Logical rack 1001      Logical rack 1002
                                                      Rack, top view




                                       Groups are split
                                       Choose this setting,
                                       •    if groups can be split (when the maximum total weight is reached) and the
                                            group can be stacked together with another group.
                                       •    to avoid the resorting of groups. The sequence of groups will be kept auto-
                                            matically (XOPTS 6.2).
                                                                    Grp.1
                                            Group 1




                                                                        Group 2




                                               Logical rack 1001                  Logical rack 1002
                                                       Rack, top view
3.00 / 01-2023




                 D-44                                                                                 A+W Production Detailed Scheduling
                 Tutorial                                                                  Racks and Stacking Modes




                                        Predefined Stacking Modes for A Racks
                                        A racks can be filled by four different methods:
                                        •   Glass mode
                                        •   Unit mode
                                        •   Production mode
                                        •   VABGLA mode

                                            Separation of glass types
                                            The program always separates the glass types. This applies to the stacking
                                            of glass types and to optimization.

                                        Glass mode
                                        In the Glass mode, every glass type is put on a separate rack. Every stack
                                        (group 3 and 4) gets its own rack number (1000, 2000, 3000).
                                                                Grp.4
                                            Grp.3




                                              Rack 1000            Rack 2000

                                                    Racks, top view




                                        •   You will need more racks and rack numbers than for other stacking modes.

                                        Stacking of complete groups
                                        When a stack has reached the maximum load, the last group is put onto a new
                                        rack - with a new rack number. The corresponding group on the other rack is
                                        also put onto a new rack - with a new rack number. Both racks (1000 and 2000)
                                        are considered to be full. More stacks (groups) can be put onto the two new
                                        racks - until the maximum load is reached.




                                            Rack 1000           Rack 2000      Rack 3000   Rack 4000


                                                    Racks, top view
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-45
                 Racks and Stacking Modes                                                                        Tutorial




                                       Stacking of split groups
                                       When a stack has reached the maximum load, the last group will be split. The
                                       remaining lites (which exceed the maximum load) go to a new rack - with a
                                       new rack number. The lites of the corresponding group on the other rack are
                                       also put onto a new rack - with a new rack number. Both racks (1000 and 2000)
                                       are considered to be full. More stacks (groups) can be put onto the two new
                                       racks - until the maximum load is reached.




                                                   Rack 1000            Rack 2000   Rack 3000     Rack 4000



                                                         Physical racks, top view




                                       Unit mode
                                       In the Unit mode, every unit (e.g. glass for IG or laminated units) is put onto a
                                       logical rack.
                                                                          Grp.4
                                           Grp.3




                                                           Logical rack 1001
                                                    Top view


                                                                 Unit




                                       •           Each glass type is set onto a different stack.
                                       •           Each unit gets its own rack number.
                                       •           When a stack has reached the maximum, the whole rack number is con-
                                                   sidered to be full.
                                       •           You will need less physical racks than for stacking mode Glass.
                                       •           As units are always kept together, production is simple.
3.00 / 01-2023




                 D-46                                                                 A+W Production Detailed Scheduling
                 Tutorial                                                                          Racks and Stacking Modes




                                        Stacking of complete groups
                                        When a stack has reached the maximum load, the last group is put onto a new
                                        rack, with a new rack number. The corresponding group on the other stack is
                                        always put onto this new (logical) rack (group 4 is over the limit which is why
                                        group 4 and 3 go to a new rack: 1002).
                                        Rack 1001 is considered to be full, rack 1002 can be loaded with further
                                        groups until the maximum load is reached.

                                                                                                         Maximum load




                                                                                                          Grp.4
                                                                               Grp.3
                                                Logical rack 1001                       Logical rack 1002
                                                Top view                                    Top view


                                                              Unit                                Unit




                                        Stacking of split groups
                                        When a stack has reached the maximum load, the last group will be split. The
                                        lites of this group which are over the maximum load plus the corresponding li-
                                        tes of the other group go to a new rack - with a new rack number. (Group 4 is
                                        over the limit; the last lite of group 4 and the last lite of group 3 go to a new
                                        rack: 1002).
                                        Rack 1001 is considered to be full, rack 1002 can be loaded with further
                                        groups until the maximum load is reached.

                                                                                                                  Maximum load
                                                                               Grp.3




                                                                                                          Grp.4




                                                     Logical rack 1001                     Logical rack 1002
                                          Top view                                     Top view



                                                               Unit                                  Unit
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                              D-47
                 Racks and Stacking Modes                                                                                                           Tutorial




                                                  Production mode
                                                  In the Production mode, different glass types can be put onto a logical rack,
                                                  combined in several stacks. Different combinations of products can be
                                                  stacked.


                                                              Float 4                                                        Maximum load

                                                      Grp.3                             Float 6

                                                                                         Float 6
                                                              Float 4
                                                                                                                           Thermal

                                                                                         Float 6




                                                                                                                   Grp.4
                                                               Float 4


                                                                                                                           Thermal
                                                                           Logical rack 1001
                                                                                 Top view




                                                  •           Each glass type is set onto a different stack.
                                                  •           Different glass types are put onto a logical (or physical) rack together.
                                                  •           When a stack has reached the maximum, the whole rack number is con-
                                                              sidered to be "full".
                                                  •           Groups belonging together must be defined and kept together.
                                                  •           You will need less physical racks.
                                                  •           You will need additional auxiliary and control mechanisms like e.g. produc-
                                                              tion papers or monitoring systems in order to keep track of things.

                                                  Stacking of complete groups
                                                  When a stack has reached the maximum load, the last group and the corre-
                                                  sponding group of the other stack will be put on a new rack - with a new rack
                                                  number (group 3 is over the limit which is why group 3 and 4 go to a new rack:
                                                  1002). You can put new glass types and new groups on this rack. Rack 1001
                                                  is considered to be full, rack 1002 can be loaded with further groups until the
                                                  maximum load is reached.


                                                                                                                                     Maximum load

                                                      Float 6

                                                      Float 6
                     Float 4


                                                      Float 6                                                                                      Thermal
                        Float 4                                                                                       Float 4
                                                                                                                                          Grp. 4
                                                                                                          Grp. 3




                                                                                        Thermal
                                  Logical rack 1001                                                                         Logical rack 1002
3.00 / 01-2023




                                          Top view                                                                                   Top view




                 D-48                                                                              A+W Production Detailed Scheduling
                 Tutorial                                                                                     Racks and Stacking Modes




                                                    Stacking of split groups
                                                    When a stack has reached the maximum load, the last group will be split. The
                                                    lites of this group which are over the maximum load plus the corresponding li-
                                                    tes of the other group on the other rack go together to a new rack - with a new
                                                    rack number. (Group 3 is over the limit which is why the last lite of group 3 and
                                                    the last lite of group 4 go to a new rack: 1002). You can put new glass types
                                                    and new groups on this rack. Rack 1001 is considered to be full, rack 1002 can
                                                    be loaded with further groups until the maximum load is reached.


                                                                                                                         Maximum load

                                                        Float 6
                  Grp.3




                                                        Float 6
                          Float 4


                                                        Float 6
                          Float 4




                                                                                                                               Grp.4
                                                                                                      Grp.3
                                                                                          Thermal             Float 4               Thermal
                                    Logical rack 1001                                                             Logical rack 1002
                                            Top view                                                                       Top view




                                                    VABGLA mode
                                                    In the VABGLA mode there is a logical rack per glass type, with one stack
                                                    each. Different combinations of products can be stacked.




                                                            Rack 1000                     Rack 2000


                                                                        Racks, top view




                                                    •      Each glass type is set onto a different rack.
                                                    •      Each glass type (stack) gets its own rack number.
                                                    •      Stacking and production is very complex.
                                                    •      Groups belonging together must be defined and kept together.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                                     D-49
                 Racks and Stacking Modes                                                                      Tutorial




                                       Stacking of complete groups
                                       When a stack has reached the maximum load, the last group is put onto a new
                                       rack - with a new rack number. The corresponding group (unit) on another rack
                                       will not be moved.




                                            Rack 1000             Rack 2000               Rack 3000

                                                             Racks, top view




                                       Stacking of split groups
                                       When a stack has reached the maximum load, the last group will be split. The
                                       lites of this group which are over the maximum load will go to a new rack - with
                                       a new rack number. The corresponding group (unit) on another rack will not be
                                       moved or split.




                                            Rack 1000             Rack 2000               Rack 3000


                                                                        Racks, top view
3.00 / 01-2023




                 D-50                                                               A+W Production Detailed Scheduling
                 Tutorial                                                                        Racks and Stacking Modes




                                        Robot Racks
                                        A racks can be marked as "robot racks". Robot racks are robot-controlled A
                                        racks. Robot racks have the following properties:
                                        •   Unlimited rack depth (> 20 m) and
                                        •   maximum number of groups on rack = 1.
                                        Only lites with the same properties (as per grouping rules) will be put on this
                                        type of rack.


                                        Modes for Harp Racks
                                        There are two different procedures with regards to harp racks:
                                        •   Together:
                                            lite and counterpane(s) are always put together on a harp rack (in different
                                            slots).
                                        •   Glass:
                                            lites will always be stacked separately (different harp racks).
                                        These modes are valid for application racks only because the counterpane for
                                        the element to be produced will not be considered for the actual production
                                        step. If there is a counterpane, this will be taken into account only for the ap-
                                        plication racks of the following production step.


                                        Modes for Fixed Racks
                                        There are no modes for fixed racks. Fixed racks only serve as temporary stock
                                        after cutting. lites will be put onto a fixed rack until it is full. The lites then need
                                        to be sorted for production.


                                        Standard Settings in the A+W Produc-
                                        tion Configuration
                                        The more racks are available on the shop floor, the higher the flexibility and
                                        the better the optimization results with regard to glass yield (despite the fixed
                                        sequence). Many racks need lots of space on the shop floor however.
                                        The A+W Production configuration offers various options for adjusting, e.g. the
                                        minimum number of racks.
                                        Master data > Configuration > A+W Production > Detailed scheduling
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                       D-51
                 Racks and Stacking Modes                                                                   Tutorial




                                       Fig. D-18     Minimum number of racks


                                            System settings
                                            These settings are made together with the service engineer when config-
                                            uring the system and must be changed afterwards only in agreement with
                                            the A+W Service team. These switches have major effects on the results
                                            and the functioning of the PPS and on the actual production results and
                                            processes.
3.00 / 01-2023




                 D-52                                                          A+W Production Detailed Scheduling
                 Tutorial                                                                  Racks and Stacking Modes




                                        Rack Settings in Master Data
                                        Certain rack types can be defined and managed in master data:
                                        Master Data > Detailed Scheduling > Racks




                                        Fig. D-19     Rack settings


                                        •   Stacking depth: Enter the maximum stacking depth in this field. This entry
                                            defines the maximum depth of the glass stack on the rack.
                                        •   Width: This entry refers to the total width of the rack.
                                        •   Max. slots/rack: Defines the number of groups that can be put onto the rack
                                            next to each other, or the number of logical racks on a physical rack.
                                        •   Maximum weight: Enter the maximum weight of all lites on the rack, e.g.
                                            750 kg = 75 m² Float 4.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                              D-53
                 Racks and Stacking Modes                                                                       Tutorial




                                        How to define a new type of A rack
                                       1 Go to menu Master Data > Detailed Scheduling > Racks.
                                       2 Use [Add] in section A racks. The dialog Detailed Scheduling appears.
                                       3 Enter a name in field New A rack then leave the dialog via [OK].
                                       4 In field Rack Depth enter the depth (in mm) for stacking lites.
                                       5 In field Width enter the width (in mm) for stacking lites.
                                       6 Enter in field Max.Slots / Rack whether a rack contains one, two, or four
                                         slots.
                                       7 If the rack is an L rack, tick the checkbox L rack.
                                       8 If you are using a robot to load the racks, tick the checkbox Robot.
                                       9 The two fields in section Quantity are active only if checkbox Robot is
                                         ticked. In the top field, enter the number of robot racks on the shop floor.
                                         The combo box below is used to define how the robot racks shall be load-
                                         ed.
                                       10 In field Maximum Weight (kg), enter the maximum load of the A rack.
                                       11 Press [OK].
                                       The new rack type can now be used for settings regarding organizations.


                                        How to define a new harp rack type
                                       1 Go to menu Master Data > Detailed Scheduling > Racks.
                                       2 Use [Add] in section harp racks. The dialog Detailed Scheduling appears.
                                       3 Enter a name in field New Harp Rack then leave the dialog via [OK].
                                       4 Enter the number of slots in field Number of Slots.
                                       5 In field Slot Width enter the width (in mm) of the individual slots.
                                       6 Tick or untick the checkbox Two Slots/Number. The lites of a unit (IG/lami-
                                         nated glass) can be put together on a harp rack; the fact that they belong
                                         together is identified by the identical slot number.
                                       7 Tick or untick the checkbox Start = 0. In case of 0, the number of the first
                                         harp racks starts from 0 instead of 1.
                                       8 Set the appropriate radio button in field Number of Digits for Slot Number:
                                       9 In field Max. Number of Harp racks enter the number of harp racks avail-
                                         able in your company.
                                       10 Tick or untick the checkbox Check Quantity.
                                       11 In field Maximum Weight (kg), enter the maximum load of the harp rack.
                                       12 Press [OK].
                                       The first harp rack can now be used for settings in the organization.
3.00 / 01-2023




                 D-54                                                           A+W Production Detailed Scheduling
                 Tutorial                                                                   Racks and Stacking Modes




                                         How to define a new type of fixed rack
                                        1 Go to menu Master Data > Detailed Scheduling > Racks.
                                        2 Use [Add] in section fixed racks. The dialog Detailed Scheduling appears.
                                        3 Enter a name in field New fixed rack then leave the dialog via [OK].
                                        4 In field Rack Depth enter the depth (in mm) for stacking lites.
                                        5 In field Width enter the width (in mm) for stacking lites.

                                           Slot width
                                           This field is currently not being analyzed by detailed scheduling. Still, an
                                           entry should be made to enable detailed scheduling to use it if possible.

                                        6 Enter the number of fixed racks on the shop floor in field Max. Number of
                                          Fixed Racks.
                                        7 Tick or untick the checkbox Check Quantity.
                                        8 In field Maximum Weight (kg), enter the maximum load of the fixed rack.
                                        9 Press [OK].
                                        The rack can now be used for settings in the organization.


                                        Additional information
                                         Tutorial, “Different Optimization Modes” on page D-61
                                         Software Reference, “Racks” on page D-153
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                D-55
                 Racks and Stacking Modes                                                                      Tutorial




                                       Demos and Exercises
                                       This session shows you how to define racks in A+W Production.

                                       Trainer demo: Explain the racks
                                       Possible racks are presented and described.
                                       The following dialog is explained from this point of view:
                                       •    Dialog Racks

                                       Exercise 1: Define an A rack
                                       Define an A rack.
                                       Rack type: A rack
                                       Stacking depth: 200 mm
                                       Width: 2000 mm
                                       Max. number of racks: 4
                                       Max. number of A racks: 99.

                                       Exercise 1: Solution
                                       The result of this exercises looks like that:




                                       Fig. D-20     A rack


                                            Rack loading by robot
                                            If you are using a robot to load the racks, tick checkbox Robot.
3.00 / 01-2023




                 D-56                                                            A+W Production Detailed Scheduling
                 Tutorial                                                               Racks and Stacking Modes




                                        Exercise 2: Define a harp rack
                                        Define a rack for harp racks.
                                        Rack type: Harp rack
                                        Number of slots: 99
                                        Max. number of harp racks: 50

                                        Exercise 2: Solution
                                        The result of this exercises looks like that:




                                        Fig. D-21     Rack


                                        Exercise 3: Define a fixed rack
                                        Define a fixed rack.
                                        Rack type: Fixed rack
                                        Stacking depth: 1000 mm
                                        Width: 2000 mm
                                        Max. number of fixed racks: 99
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                        D-57
                 Racks and Stacking Modes                                                                   Tutorial




                                       Exercise 3: Solution
                                       The result of this exercises looks like that:




                                       Fig. D-22    Fixed rack


                                       Additional information:
                                        Tutorial, “Racks” on page D-19
                                        Software Reference, “Racks” on page D-153
3.00 / 01-2023




                 D-58                                                            A+W Production Detailed Scheduling
                 Tutorial                                                                         Optimization Modes




                                        Optimization Modes
                                        This subject area introduces the optimizations and tells you how to use them
                                        in A+W Production.
                                        This subject area includes the following training sessions:
                                        •   Overview
                                        •   Different Optimization Modes
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                            D-59
                 Optimization Modes                                                                                 Tutorial




                                      Overview
                                      Objectives

                                      • Knowing and understanding the different optimization modes.
                                      • Circumstances in which the individual modes are used
                                      • Knowing and understanding the appropriate settings in A+W Production


                                      Benefit

                                      Only knowing and understanding the different optimization modes will enable you to
                                      adapt A+W Production detailed scheduling to your production so that it will operate
                                      effectively and in a time-saving manner.


                                      Definitions

                                      Unit                        A unit consists of two or more lites of glass which belong
                                                                  together because they are going to be assembled later,
                                                                  e.g. into IG or laminated glass.

                                      Group                       The group includes a quantity. It groups units according
                                                                  to certain criteria like customer number and order
                                                                  number.

                                      Super group                 Super groups unite different groups. This way, three
                                                                  groups which belong together can be treated by a set of
                                                                  similar rules for example. Example: Sorting onto racks
                                                                  because all three groups (e.g. orders) belong to the
                                                                  same customer or the same project.


                                      Note

                                      Choosing the optimization   When you select an optimization, you have to
                                                                  compromise between the optimum result (minimum
                                                                  waste) and the optimum production sequence with
                                                                  regards to assembly.
3.00 / 01-2023




                 D-60                                                            A+W Production Detailed Scheduling
                 Tutorial                                                                             Optimization Modes




                                        Different Optimization Modes
                                        When choosing the optimization you will always have to find a compromise be-
                                        tween the best optimization result (low waste) and the best production se-
                                        quence with regard to assembly.
                                        A+W Production uses the optimization modes:
                                        •   6.2
                                        •   6.1
                                        •   5.2
                                        •   5.1
                                        •   Free optimization

                                        Optimization mode 6.2 - fixed sequence
                                        This optimization mode works with a strict sequence. Nothing can be changed;
                                        the lites are produced in a totally strict sequence. This is the sequence in which
                                        they are released for optimization.
                                        •   The sequence of groups is fixed.
                                        •   The sequence of lites within a group is fixed.

                                            Alternating optimization items for items with unequal lites
                                            Items with two or more lites of a glass type that have different geometries
                                            can be set down like normal pairs, that is, on a common stack and alterna-
                                            ting (LIte1, Lite3, Lite1, Lite3, etc.). The desired behavior is only used for A
                                            racks for which the 6.2 mode (=fixed sequence) is set.

                                            A combination of shapes is only possible for these lites with the A+W Sha-
                                            pe Optimizer, no longer via the detailed scheduling-internal combination of
                                            shapes!

                                        Under which circumstances can this mode be used?
                                        •   You are using A racks for optimization
                                        •   You have got a strict production and delivery plan
                                        •   You produce either by customer or glass type
                                        •   Your yield is (usually) poor - the result is not the main criterion however but
                                            the production in strict sequence (e.g. aligning the entire production to the
                                            truck's unloading sequence for a special customer project).
                                        •   You have to make sure that the big lites are cut and stacked first, or you will
                                            need an additional rack for resorting
                                        •   You will usually need a fixed number of racks (number of groups = almost
                                            the number of physical racks)
                                        •   You can directly optimize in production or packing sequence
                                        The following illustration symbolizes the effects of this mode:
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-61
                 Optimization Modes                                                                      Tutorial




                                                               Sequence




                                      Yield                                               Flexibility



                                      Settings in A+W Production
                                      Optimizing in this mode requires the following settings:
                                      Master data > Detailed scheduling > Organization > tab Production sequence
                                      > Select rack > Settings




                                      Fig. D-23    Optimization mode 6.2


                                      Additional information
                                       Tutorial, “Racks” on page D-19
                                       Software Reference, “Default Settings” on page D-146
3.00 / 01-2023




                 D-62                                                         A+W Production Detailed Scheduling
                 Tutorial                                                                             Optimization Modes




                                        Optimization mode 6.1 - keep customers together
                                        The sequence of groups is fixed in this optimization mode, e.g. by size. The
                                        different groups can be rearranged to improve the result. A typical criterion for
                                        this would be
                                        •   Route | Customer
                                        This ways, the items of a customer will be produced together; you cannot de-
                                        fine however the lites of which customer are going to be produced first.
                                        •   The sequence of groups can be changed.
                                        •   The sequence of lites within a group is fixed.

                                        Under which circumstances will this mode be used?
                                        •   You are using A racks for optimization
                                        •   You have got a strict production and delivery plan
                                        •   You produce either by customer or glass type
                                        •   Your yield is relatively poor (better than in mode 6.2 however) - the yield is
                                            not the main criterion however
                                        •   You have to make sure that the big lites are cut and stacked first, or you will
                                            need an additional rack for resorting
                                        •   You will usually need a fixed number of racks (number of groups = almost
                                            the number of physical racks)
                                        •   You can directly optimize in production or packing sequence
                                        The following illustration symbolizes the effects of this mode:

                                                                   Sequence




                                        Yield                                                 Flexibility
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-63
                 Optimization Modes                                                                      Tutorial




                                      Settings in A+W Production
                                      Optimizing in this mode requires the following settings:
                                      Master Data > Detailed Scheduling > Organization > tab Production Sequence
                                      > Select Rack > Settings




                                      Fig. D-24    Optimization mode 6.1


                                      Additional information
                                       Tutorial, “Racks” on page D-19
                                       Software Reference, “Rack Settings” on page D-142
3.00 / 01-2023




                 D-64                                                         A+W Production Detailed Scheduling
                 Tutorial                                                                           Optimization Modes




                                        Optimization mode 5.2 - standard
                                        This optimization mode is the standard mode for detailed scheduling. The
                                        grouping and sorting key only includes the group number. This means that ev-
                                        ery item of the group has its own item number by which it can be clearly iden-
                                        tified. This is why the elements within the groups have no fixed sequence but
                                        can be optimized freely.
                                        •   The sequence of groups is fixed.
                                        •   The sequence of lites within a group can be changed. Only units (e.g. for
                                            IG) will be kept together.

                                        Under which circumstances will this mode be used?
                                        •   If mode 5.1 is not being used
                                        •   If the two properties ORDER NUMBER and ITEM NUMBER are not used
                                            together in combined grouping/sorting codes.
                                        The following illustration symbolizes the effects of this mode:

                                                                  Sequence




                                        Yield                                               Flexibility
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-65
                 Optimization Modes                                                                      Tutorial




                                      Settings in A+W Production
                                      Optimizing in this mode requires the following settings:
                                      Master data > Detailed scheduling > Organization > tab Production sequence
                                      > Select rack > Settings




                                      Fig. D-25    Optimization mode 5.2


                                      Additional information
                                       Tutorial, “Racks” on page D-19
                                       Software Reference, “Rack Settings” on page D-142
3.00 / 01-2023




                 D-66                                                         A+W Production Detailed Scheduling
                 Tutorial                                                                             Optimization Modes




                                        Optimization mode 5.1 - IG on harp racks or many A racks
                                        The grouping and sorting key only includes the group number. This means that
                                        every item of the group has its own item number by which it can be clearly
                                        identified. This is why the elements within the groups have no fixed sequence
                                        but can be optimized freely. This is identical with optimization mode 5.2 so far.
                                        •   The sequence of groups can be changed
                                        •   The sequence of lites within a group can be changed.
                                        •   Only units (e.g. for IG) will be kept together.

                                        Under which circumstances will this mode be used?
                                        •   You are using harp racks for optimization and you need additional A racks
                                        •   Your yield will be good
                                        •   You will have do to do a lot of sorting before delivery - this requires a large
                                            number of physical racks.
                                        The following illustration symbolizes the effects of this mode:

                                                                   Sequence




                                        Yield                                                 Flexibility
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-67
                 Optimization Modes                                                                      Tutorial




                                      Settings in A+W Production
                                      Optimizing in this mode requires the following settings:
                                      Master data > Detailed scheduling > Organization > tab Production sequence
                                      > Select rack > Settings




                                      Fig. D-26    Optimization mode 5.1


                                      Additional information
                                       Tutorial, “Racks” on page D-19
                                       Software Reference, “Rack Settings” on page D-142
3.00 / 01-2023




                 D-68                                                         A+W Production Detailed Scheduling
                 Tutorial                                                                             Optimization Modes




                                        Optimization mode Free Optimization - lites on harp racks
                                        Free optimization is the standard optimization for lites on harp racks. As for
                                        manual cutting, different glass types/thicknesses can be put onto a rack (dif-
                                        ferent stacks of glass) when the free optimization is used.
                                        •   Everything is free

                                        Under which circumstances will this mode be used?
                                        •   You are using harp racks for optimization (and you need additional A racks
                                            for special glass types, e.g. for large lites).
                                        •   Your yield will be excellent - waste is the most important parameter
                                        •   You will have do to do a lot of sorting - this requires a large number of phys-
                                            ical racks.
                                        The following illustration symbolizes the effects of this mode:

                                                                   Sequence




                                        Yield                                                 Flexibility
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-69
                 Optimization Modes                                                                            Tutorial




                                      Settings in A+W Production
                                      Optimizing in this mode requires the following settings:
                                      Master Data > Detailed Scheduling > Organization > tab Production Sequence
                                      > Select Rack > Settings




                                      Fig. D-27    Optimization mode Free Optimization


                                      As you can see there is a correlation between Grouping and Sorting, Result
                                      and the Number of racks. The more restrictive your Grouping and Sorting, the
                                      more restrictions you will have with regard to optimization and results.
                                      Grouping and Sorting are not the only important factors for rack allocation and
                                      production organization. The handling of lites of different sizes, glass types,
                                      shapes, etc. is as important as putting the lites onto racks.

                                      Double optimization
                                      Free optimization allows to run a double optimization which means that differ-
                                      ent glass types can be optimized with an identical cutting plan.
                                      The advantage of this kind of optimization is that although free optimization is
                                      used, the lites of a unit can be stored systematically. The lites of a double op-
                                      timization can be stored on a rack together with other double or free optimiza-
                                      tions.

                                         Double optimization
                                         Double optimization can be used only for racks with Unit mode.
3.00 / 01-2023




                 D-70                                                          A+W Production Detailed Scheduling
                 Tutorial                                                                            Optimization Modes




                                        Demos and exercises
                                        This section shows you how the optimization works.

                                        Complex exercise: Compare different detailed scheduling results
                                        together with the trainer:
                                        The optimization process is presented and explained.
                                        The following dialog is explained from this point of view:
                                        •   Dialog Detailed scheduling for batch ….

                                        Step 1: Enter test orders
                                        Together with the trainer, enter two test orders which include different product
                                        structures. The number of items should be 20-100 units each. You should at
                                        least enter an IG unit with toughened glass plus single float glass lites and sin-
                                        gle toughened lites (spread over several items and orders). There should be
                                        shapes, large lites, and smaller lites.
                                        Schedule the orders. Use these two test orders plus possibly existing test/
                                        training orders in the system to create a batch (or several batches, depending
                                        on the number of test orders).
                                        Enter the batch(es) in detailed scheduling. On tab 2 (rack load), check the re-
                                        sult of the rack allocation in detailed scheduling. Click on the Optimization but-
                                        ton and check the results on the cutting plan in A+W Plan Editor. What do you
                                        notice? Which data do you recognize and how can you read the rack allocation
                                        on the cutting plan? Discuss the results with the trainer.

                                        Step 2: Change the organization
                                        Close Plan Editor, select on tab 5 (Organization) another master organization
                                        and run the rack allocation again. To do this, press the Repeat button. Return
                                        to tab 2 (rack allocation). Compare the results with the first rack allocation.
                                        What are the differences? Discuss the results with the trainer.

                                        Step 3: Optimize the batch again
                                        Optimize the batch again and open the cutting plan (Plan Editor). What are the
                                        differences? Discuss the results with the trainer.
                                        Go to tab 5 and change the master organization again by choosing your own
                                        organization (the one you have previously defined together with the trainer).
                                        Compare the results.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-71
                 Optimization Modes                                                                         Tutorial




                                      Change the settings for Grouping and Sorting and the Stacking mode. Check
                                      the new results of rack allocation and the optimization/the cutting plan. What
                                      are the differences? Discuss the results with the trainer.

                                      Step 4: Extend the organization
                                      Extend your own organization, e.g. by an additional glass type, or separate
                                      large shapes from small shapes.
                                      Repeat step 3 as many times as necessary, with different settings, and com-
                                      pare the results each time.
3.00 / 01-2023




                 D-72                                                         A+W Production Detailed Scheduling
                 Tutorial                                                                             Organizations




                                        Organizations
                                        This subject area introduces the different organization types and shows you
                                        how to use them for A+W Production.
                                        This subject area includes the following training sessions:
                                        •   Organization Types
                                        •   Production Sequence
                                        •   A+W Standard Organizations
                                        •   Rack Organization
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                           D-73
                 Organizations                                                                                    Tutorial




                                 Organization Types
                                 Objectives

                                 • Knowing and understanding organization types
                                 • Understanding the effects of the organizations
                                 • Being able to set up organizations


                                 Benefit

                                 For correct batch planning, you have to understand the different types of
                                 organizations. Only then will you be able to assess the effects on the actual
                                 production processes, and plan them in advance.


                                 Definitions

                                 Organization                 An organization is a set of technical rules for handling the
                                                              production processes.

                                 Organization group           An organization group is a structural element of an
                                                              organization for detailed definition of rules and
                                                              conditions, e.g. for different glass types (toughened,
                                                              laminated, IG) or for distinguishing the treatment of
                                                              rectangles and shapes for a glass type (IG).

                                 Pseudo series                Usually, single lites must be stored/put onto fixed racks
                                                              only temporarily, e.g. to wait for remakes. By means of
                                                              pseudo series, identical items (single lites) can be
                                                              combined in a series which can be put together on fixed
                                                              rack as an exception from the rule.


                                 Note

                                 Different organizations      Depending on the company's structure, different
                                                              organizations can be defined.

                                 Organization groups/rack     An organization consists of one or more organization
                                 types                        groups which again consist of one or more rack types.

                                 Production sequence          The production sequence within an organization is
                                                              defined by the sequence of organization groups.
3.00 / 01-2023




                 D-74                                                         A+W Production Detailed Scheduling
                 Tutorial                                                                                Organizations




                                        General
                                        A+W Production offers so-called Organizations for the correct and efficient
                                        scheduling of batches. An organization is a set of technical rules for handling
                                        the production processes (with regard to production processes, process
                                        chains and rack management). Depending on the company's structure, any
                                        number of organizations (toughened glass organization, IG organization, pro-
                                        cessing organization, etc.) can be defined. The individual organizations orga-
                                        nize the racks for the production steps (IG line, furnace, etc.).


                                        Tree Structure
                                        To create the required production sequence, A+W Production assigns a so-
                                        called master organization to every batch. A master organization is a set of or-
                                        ganizations, consisting of one or more organizations. Several master organi-
                                        zations can be defined for a company. In this case, detailed scheduling will
                                        assign to the batch the master organization that comes closest to the product
                                        mix.
                                        A master organization must contain just one standard organization (applica-
                                        tion). Of all other organization types, a master organization must contain just
                                        one. An organization consists of one or more organization groups which again
                                        consists of one or more rack types. Also, you can define the required produc-
                                        tion sequence for the organization groups and rack types.

                                        Master organization
                                                       Organization 1
                                                       Organization 2
                                                                        Organization group 1
                                                                        Organization group 2

                                                                                Rack type 1
                                                                                          Condition 1
                                                                                 Rack type 2
                                                                                          Condition 2
                                                                        Organization group 3
3.00 / 01-2023




                                        Fig. D-28     A practical example




                 A+W Production Detailed Scheduling                                                               D-75
                 Organizations                                                                                Tutorial




                                 Master Organization
                                 Each master organization contains a standard application organization. More-
                                 over, application and production organizations can be created for every lot
                                 type.
                                 When an element shall be allocated to an organization, detailed scheduling
                                 first checks whether there is a production organization for the batch type in
                                 question (in this case, 300). If no production organization is found, detailed
                                 scheduling will search for a standard production organization. In our example,
                                 there is none. This means that no production organization will be allocated.
                                 Next, detailed scheduling searches for the application organization allocated
                                 to this batch type. If none if found, the element will get the standard application
                                 organization. The required application organization (300) is available and will
                                 be allocated to the element.

                                                                                                A
                                                                       Standard                 B

                                                                                  700           C
                                                                 300                            D

                                                                           700                  D

                                 E                300

                                 A Master organization                      D Application organization (blue) for
                                 B Standard application organization          batch type 700
                                   (blue)                                   E Element, batch type 300
                                 C Productions organization (yellow) for
                                   batch type 700
                                 Fig. D-29    Master organization, example 1


                                 A production and an application organization are found for the element of lot
                                 type 700. It will be allocated to two different organizations, with different rack
                                 types (application and production rack).
                                 You can of course define a standard production organization to be allocated to
                                 all elements for which no standard production organization is found that
                                 matches the batch type. In contrast to the application organization, you do not
                                 need to define in the production organization a buffer rack for elements that do
                                 not fulfil the conditions of another rack of this organization. If no suitable rack
                                 is found for an element in the production organization, the production organi-
                                 zation allocation will be simply ignored. This means that to allocate production
                                 organizations to certain batch types, a buffer rack should be defined in the or-
                                 ganization to prevent that the allocation of individual elements is ignored.
3.00 / 01-2023




                 D-76                                                        A+W Production Detailed Scheduling
                 Tutorial                                                                                      Organizations




                                                                                                        A
                                                                              Standard                  B

                                                                                         700            C
                                                                        300                             D

                                                                                  700                   D

                                        E                700

                                        A Master organization                       D Application organization (blue) for
                                        B Standard application organization           batch type 700
                                          (blue)                                    E Element, batch type 700
                                        C Productions organization (yellow) for
                                          batch type 700
                                        Fig. D-30     Master organization, example 2


                                        The corresponding settings are made in the Organization dialog:
                                        Master Data > Detailed Scheduling > Organization




                                        Fig. D-31     Master organization
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                     D-77
                 Organizations                                                                            Tutorial




                                  How to set up a master organization
                                 1 Go to Master Data > Detailed Scheduling > Organization.
                                 2 Press the [New] button. The dialog Master Organization appears.
                                 3 Enter the name for this master organization in field Name of Master Orga-
                                   nization.
                                 4 Tick or untick the checkbox XOPT - stack together.
                                 5 Tick or untick the checkbox Quick Organization.
                                 6 In combo box Production Groups, select the required group.
                                 7 Select the required series in combo box Pseudo Series.
                                 8 For pseudo series, enter a minimum quantity in field Minimum Quantity.
                                 9 If your system has been extended or adjusted by means of a special script
                                   you can select this script in field Used script.
                                 10 The Filler button can be used for selecting defined filler conditions.
                                 11 Edit the field Quasi elements. To view all existing quasi elements, use but-
                                    ton […].
                                 12 Tick or untick the checkbox Use Filler. If the checkbox is ticked, the fields
                                    Start of Filler and End of Filler must be edited!
                                 13 Tick or untick the checkbox Use residue plates. If the checkbox is ticked,
                                    the fields Start of residue plate and End of residue plate must be edited!
                                 14 Tick or untick the checkbox Double Optimizations together.
                                 15 Tick or untick the checkbox Use Rejects. If the checkbox is ticked, the fields
                                    Start of Rejects and End of Rejects must be edited!
                                 16 Press OK. The new master organization automatically appears in the Or-
                                    ganization Dialog.


                                  How to add an existing, new organization to a master organization
                                 1 Go to Master Data > Detailed Scheduling > Organization. Tab Master Or-
                                   ganization shows all existing master organizations.
                                 2 Select the master organization to which you want to add a new organiza-
                                   tion.
                                 3 The bottom right window shows all existing organizations. Select the orga-
                                   nization to add to the master organization.
                                 4 Press the [New] button. The new organization is shown below the master
                                   organization.
3.00 / 01-2023




                 D-78                                                     A+W Production Detailed Scheduling
                 Tutorial                                                                                  Organizations




                                         How to set up a new organization
                                        1 Go to Master Data > Detailed Scheduling > Organization.
                                        2 Open the tab Production Sequence.




                                                                                                     .
                                           Fig. D-32     Tab Production sequence


                                        3 Press the [New] button. The new organization is shown below the last or-
                                          ganization. This will be called unknown / … at first.
                                        4 Select this organization and use the button [Settings]. The dialog Organi-
                                          zation appears.




                                           Fig. D-33     Organization settings


                                        5 In field Name of Organization Type, change the name from unknown to a
                                          characteristic name.
                                        6 In combo box Type, select the required organization type.
                                        7 Tick the appropriate checkbox in section Stacking Mode.
3.00 / 01-2023




                                        8 If applicable, edit the fields in section Do not split … if rack load is over.
                                        9 Press [OK] to close the dialog.


                 A+W Production Detailed Scheduling                                                                 D-79
                 Organizations                                                                         Tutorial




                                  How to add a new organization group to an organization
                                 1 Go to Master Data > Detailed Scheduling > Organization.
                                 2 Open the tab Production Sequence.
                                 3 Select the organization to which a new organization group shall be added,
                                   then press the button [New]. The new organization group appears below
                                   the selected organization; it is called noname.
                                 4 Select the organization group called noname then press button [Settings].
                                   The dialog Organization Groups appears.
                                 5 In field Name, enter a characteristic name for this Organization Group.
                                 6 Select the required group from combo box Group Formation.
                                 7 Tick or untick the checkbox Sorting of Groups.
                                 8 Select the required sorting from combo box Sorting of Groups.
                                 9 Press [OK] to close the dialog.


                                 Additional information
                                  Tutorial, “Organizations” on page D-73
                                  Software Reference, “Organization” on page D-138
                                  Software Reference, “Organization Groups” on page D-140


                                  How to define the grouping and sorting for a rack
                                 1 Go to Master Data > Detailed Scheduling > Organization.
                                 2 Open the tab Production Sequence.
                                 3 Select the organization group for which a rack shall be defined, then press
                                   button [New]. The system automatically creates a rack called unknown.
                                 4 Select the rack called unknown then press button [Settings]. The dialog
                                   Rack Settings appears.
3.00 / 01-2023




                                    Fig. D-34    Rack settings




                 D-80                                                   A+W Production Detailed Scheduling
                 Tutorial                                                                                  Organizations




                                        5 In field Name, replace unknown by a characteristic name for this rack.
                                        6 In combo box Group Formation, define the rules for creating groups (e.g.
                                          by customer number and order number).
                                        7 Tick or untick the checkbox Sorting of Groups.
                                        8 In combo box Group Stacking Mode, define the stacking mode for the
                                          groups, per stack.
                                        9 Go to combo box Optimization Behavior and define whether the sequence
                                          of groups shall be sorted or unsorted (super groups) or if nothing shall be
                                          sorted (sequence of groups unsorted and lites within the groups unsorted).
                                        10 Tick or untick the checkbox Reception Rack (this is where all the lites go
                                           which are not allocated by means of rules to special racks). Each organi-
                                           zation must include at least one buffer rack.
                                        11 If this rack is an application rack, make the following settings in tab Appli-
                                           cation:
                                           •   Edit the fields From To.
                                           •   Tick the appropriate checkbox in section Stacking Mode.
                                           •   Tick or untick the checkbox Cycle Optimization.
                                           •   Edit the field Max. Number of Groups.
                                           •   Edit the field Cycle Size.
                                           •   Tick the appropriate checkbox in section Rack Type.
                                        12 If this rack is a production rack, make the following settings in tab Produc-
                                           tion:
                                           •   Edit the fields From To.
                                           •   Tick or untick the checkbox Create production racks.
                                           •   Edit the field Max. number of groups.
                                           •   Tick the appropriate checkbox in section Rack type.
                                        13 Press [OK] to close the dialog.


                                        Reject Organization
                                        This reject organization is used to put rejects onto racks according to freely de-
                                        finable criteria. Based on the programmed, internal conditions, the reject orga-
                                        nization automatically checks the properties of the broken lite (i.e. float). Like
                                        all other organizations, reject organizations are defined in the Organization di-
                                        alog.


                                        Sequence of checks
                                        Within an organization, racks are created for which conditions are defined.
                                        These conditions define the allocation of a lite to a certain rack. The sequence
                                        of rack types normally starts with the most restrictive conditions, using the
                                        checking sequence of the rack types as a filter for the lites.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-81
                 Organizations                                                                                          Tutorial




                                 Element
                                             Rack type 1 (shapes)



                                             Rack type 2 (large rectangles)




                                                                              Organization
                                             Rack type 3 (small rectangles)



                                             Rack type 4 (series)


                                             Rack type 5 (special)

                                 Fig. D-35    Rack conditions


                                 Special cases will be checked first. It is therefore possible to allocate the con-
                                 dition Shape to the rack that comes first in the checking sequence. All shapes
                                 would be allocated to this rack type. With the condition Large lites, the second
                                 rack type would get all lites up to a defined size, etc. The further down in the
                                 check sequence a rack type is, the weaker the conditions.
                                 If no rack type is found for an element in an application organization, it will be
                                 allocated to the buffer rack. A buffer rack either has no conditions at all, and
                                 thus stands at the end of the checking sequence, or the code Buffer rack is set
                                 (we recommend defining a buffer rack for every organization group by default,
                                 no matter if a production or organization application organization is used. You
                                 should also set the code for the buffer rack by default).
                                 Each organization group must have maximally one buffer rack; for application
                                 organizations, it is mandatory.


                                  How to change the sequence of checks
                                 1 Go to Master Data > Detailed Scheduling > Organization.
                                 2 Open tab Test Sequence.
                                 3 In section Organizations, select the organization for which you want to
                                   change the sequence of checks.
                                 4 In section Racks, choose the rack the sequence of which shall be changed.
                                 5 Shift the sequence of checks for the tagged rack by means of the buttons
                                   [Start], [Up], [Down] or [End] until the rack has reached the required posi-
                                   tion.
3.00 / 01-2023




                 D-82                                                                        A+W Production Detailed Scheduling
                 Tutorial                                                  Organizations




                                        Fig. D-36     Sequence of checks
3.00 / 01-2023




                 A+W Production Detailed Scheduling                               D-83
                 Organizations                                                                              Tutorial




                                 Organization Type and Batch Type
                                 Each element and processing has its own element type or processing type
                                 (basic glass, toughened glass, etc.), and its supply type (ordered, cutting,
                                 etc.). Depending on these two properties, the element or processing is allocat-
                                 ed to a certain batch type. This way, elements with different processing types
                                 can be allocated to the same batch type, to be treated together, e.g. at rack
                                 allocation.
                                 Apart from that, each organization has a certain organization type which de-
                                 fines the elements to be allocated to the organization. Ideally, definition and fil-
                                 ters are based on differences and similarities:
                                 •   Shapes?, Rectangles?
                                 •   Height?, Weight?
                                 •   …
                                 Production batches are created at cutting for different element types and dif-
                                 ferent glass types.

                                 Application and production organizations
                                 Apart from the organization type, organizations are distinguished by their be-
                                 ing used in production organizations and application organizations. Applica-
                                 tion organizations must be created while production organizations can be
                                 created additionally. Each element gets an application organization anyway,
                                 plus an additional production organization if required.
                                 An application rack will always be defined for a utilisation organization. A pro-
                                 duction rack can be defined additionally.
                                 For production organizations, only production racks can be defined. In the ap-
                                 plication organization, the conditions for distributing the lites to application and
                                 production racks are the same. Allocating a product for the same processing
                                 step to both an application and a production organization allows to distribute
                                 the lites to application and production racks according to different conditions.
                                 The lites on the application racks for instance can be sorted by size, and can
                                 be distributed after production (e.g. for toughened glass, after the furnace) to
                                 production racks depending on whether they will be used for IG, or will be
                                 shipped.
                                 If a production organization is allocated to an element for a certain processing,
                                 the groups and sorting on the application organization/racks will be ignored.
                                 After processing, the element will be put onto racks depending on the groups
                                 and sorting of the production rack (production organization).


                                 Additional information
                                  Software Reference, “Production” on page D-138
3.00 / 01-2023




                 D-84                                                      A+W Production Detailed Scheduling
                 Tutorial                                                                              Organizations




                                        Global settings
                                        The global settings are connected with the values selected in the dialogs and
                                        fields mentioned below:
                                        •   Dialog organization groups,
                                            – Fields: Formation of groups, sorting within groups
                                        •   Dialog Rack settings
                                            – Fields: Formation of groups, sorting within groups
                                        When you select in the above dialogs the value None for the corresponding
                                        fields, the global settings will be used.

                                            Default settings
                                            These entries should be made to avoid error messages at the start of A+W
                                            Production.


                                        Additional information
                                         Software Reference, “Default Settings” on page D-146
                                         Software Reference, “Organization Groups” on page D-140
                                         Software Reference, “Rack Settings” on page D-142
                                         Tutorial, “A+W Standard Organizations” on page D-91
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                            D-85
                 Organizations                                                                         Tutorial




                                 Demos and Exercises
                                 Open the master data of detailed scheduling. Check out with the trainer al-
                                 ready predefined in Orgas. Analyze the structure (tree structure, different
                                 racks, allocation of conditions). What do you notice?
                                 Discuss the structure with your trainer.
3.00 / 01-2023




                 D-86                                                       A+W Production Detailed Scheduling
                 Tutorial                                                                                     Organizations




                                        Production Sequence
                                        Objectives

                                        • Knowing and understanding the production sequence.
                                        • Understanding the effects of the production sequence


                                        Benefit

                                        Due to your knowledge of the possible settings in organization groups with regard to
                                        grouping and sorting, you can define the actual production sequence of batches and
                                        individual lites, and change it flexibly at any time.


                                        Definitions

                                        Grouping key                The grouping key for an organization group allows
                                                                    defining the production sequence without fixing a
                                                                    grouping/sorting for the racks.


                                        Note

                                        No grouping                 If no grouping is defined for the organization group, the
                                                                    production sequence depends on the sequence of racks
                                                                    within the organization group.

                                        Including grouping          If for instance, the organization group is grouped by
                                                                    customer, the production sequence is no longer defined
                                                                    by the sequence of rack types within the organization
                                                                    group. The main criterion is the element property
                                                                    Customer.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                     D-87
                 Organizations                                                                          Tutorial




                                 General
                                 The production sequence within an organization is defined by the sequence of
                                 organization groups. This again is defined by the sequence of rack types. The
                                 sequence within the rack types is defined by group and sorting keys.
                                 To avoid having to define the same sorting for each rack type within an orga-
                                 nization group, you can define the sorting per organization group. This is
                                 passed on to the rack types included in the organization group, and can be
                                 completed if necessary.
                                 The same applies to the group that can be defined for the organization group.
                                 This is also passed on to the rack types, and can be completed if required.
                                 However, the grouping of an organization group has a major impact on the pro-
                                 duction sequence. If the organization group is grouped by Route for instance,
                                 the production sequence is no longer defined simply by the sequence of rack
                                 types within the organization group. The main criterion is the element property
                                 Route. This means that all elements of Route A will be produced first, followed
                                 by the elements of Route B, etc. For a given route, however, the sequence of
                                 rack types within the organization group is decisive. An exception however is
                                 if on a rack type within the organization group, the sequence of groups is ran-
                                 dom. If the optimization could put them in a random sequence, the grouping
                                 defined for this organization group could no longer determine the sequence of
                                 groups. In this case, the sequence is defined by the sequence of rack types;
                                 the grouping of the organization group will be passed on to the rack types in-
                                 volved.
                                 Below please find information on
                                 •   “Grouping Key for Organization Groups” on page D-88
                                     – “No grouping” on page D-88
                                     – “Including grouping” on page D-89


                                 Grouping Key for Organization Groups
                                 The grouping key defined for an organization group has a major influence on
                                 the production sequence. It allows to define the production sequence without
                                 fixing a grouping/sorting for the racks.

                                 No grouping
                                 If no grouping is defined for the organization group, the production sequence
                                 depends on the sequence of racks within the organization group (e.g. small li-
                                 tes, Georgian bars, etc.).
3.00 / 01-2023




                 D-88                                                    A+W Production Detailed Scheduling
                 Tutorial                                                                                   Organizations




                                                           Production Sequence
                                                      without grouping in organization group


                                                                                                      Organization group
                                           Rack Type A




                                           Rack Type B




                                        Fig. D-37     Production sequence without grouping in the organization group


                                        Including grouping
                                        If for instance, the organization group is grouped by customer, the production
                                        sequence is no longer defined by the sequence of rack types within the orga-
                                        nization group. The main criterion is the element property Customer. In this ex-
                                        ample, this would mean that first, all lites for customer A will be produced, then
                                        for customer B, etc. For the customer itself, the production sequence depends
                                        on the sequence of racks within the organization group.
                                        Within the groups, the element sequence is free, i. e. there are no restrictions
                                        regarding the optimization (optimization mode 5.2).


                                                           Production Sequence
                                                       with grouping in organization group




                                           Rack Type A




                                           Rack Type B




                                                                        A                      B
                                        A Customer A                                   B Customer B
                                        Fig. D-38     Production sequence with grouping in the organization group
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                    D-89
                 Organizations                                                                        Tutorial




                                 Defining the production sequence by means of the grouping key
                                 To define the production sequence by means of the grouping key for the
                                 organization group, you must not set "sort by order and item number" for
                                 the racks. If this is done, optimization mode 6.1 will be used for optimiza-
                                 tion, and the grouping key for the organization group will be ignored.
3.00 / 01-2023




                 D-90                                                 A+W Production Detailed Scheduling
                 Tutorial                                                                                       Organizations




                                        A+W Standard Organizations
                                        Objectives

                                        • Knowing and understanding different standard organizations
                                        • Being able to understand the corresponding settings in A+W Production


                                        Benefit

                                        The advantage of standard organizations is that they have been defined before and
                                        can be used right away. This saves time and minimizes the risk of set-up errors.


                                        Definitions

                                        Standard organization      Organizations predefined by A+W.


                                        Note

                                        In case of changes         we recommend to copy the required standard
                                                                   organization and change the copied version. This way,
                                                                   the original version is still available and the risk of errors
                                                                   is kept low.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                        D-91
                 Organizations                                                                                   Tutorial




                                 Rack Organization
                                 A+W Production offers a number of standard organizations for glass produc-
                                 tion. Every organization uses special sorting and grouping criteria for the lites,
                                 and will optimize production according to the individual requirements.
                                 The table below gives an overview of the available organizations and their fea-
                                 tures. The sequence ranges from production-oriented, up to dispatch-oriented
                                 organization.

                                 Name                 Description

                                 A Racks Spacer       This organization will be useful for benders with very strict
                                                      spacer restrictions, which have no buffer to pre-produce and
                                                      sort the spacers. This organization does not consider dispatch
                                                      requirements.

                                 A Racks              This organization provides a moderately dispatch-organized
                                                      production sequence by customer and order, but is restricted
                                                      as to the number of racks that can be used before the line. The
                                                      degree of dispatch organization can be controlled by the
                                                      global settings for classification and sorting.With this
                                                      organization, repacking will be called for after IG production.

                                 A Racks Dispatch     This organization offers a dispatch-oriented production
                                                      sequence; several A racks will be used alternately before the
                                                      line. The organization needs racks before and behind the line,
                                                      and produces the lites in packing sequence. Racks for the
                                                      individual customers have to be provided after the line.

                                 Harp racks           Structure and rack allocation of this organization are similar to
                                                      the A rack organization but mainly uses harp racks; this will
                                                      generally improve the yield. Big and small units as well as
                                                      series will be put onto A racks.
                                                      Unlike the A rack organization, the lites are produced in
                                                      dispatch sequence. Even if the harp rack organization handles
                                                      one rack after the other in front of the line, the required glass
                                                      types can be put onto harp rack, in dispatch sequence.

                                 Filled harp racks    This organization makes sure that there are no half-filled harp
                                                      racks; it sorts all harp racks in production sequence. The harp
                                                      racks will be handled first, followed by the A racks containing
                                                      the specialities.

                                 Tab. D-1      Available organizations

                                 A racks spacers
                                 This organization is useful for IG producers using benders with very strict
                                 spacer restrictions, which have no buffer to pre-produce and sort the spacers.
                                 The organization A racks spacers sorts the production sequence by spacer,
                                 taking the units from A racks in front of the line in consecutive order.
                                 •   This organization does not consider dispatch requirements.
3.00 / 01-2023




                                 •   Only A racks will be used (200 mm in depth and 2000 mm in width).
                                 •   The stacking mode is Unit (lites of a unit being put onto the same rack, on
                                     different stacks).


                 D-92                                                        A+W Production Detailed Scheduling
                 Tutorial                                                                              Organizations




                                        Production sequence
                                        The production sequence is created from the following, optimized rack groups
                                        (in production sequence):
                                        •   Common IG lites
                                        •   IG shapes
                                        •   IG lites with Georgian bars
                                        •   IG shapes with Georgian bars
                                        •   Stepped IG
                                        •   Triple IG
                                        Each of these groups consists of five spacer rack groups, to be produced one
                                        after the other. The spacer groups are separated by adjustable threshold val-
                                        ues:
                                        Spacer group 1
                                            > spacer threshold 1
                                        Spacer group 2
                                            > spacer threshold 2
                                        Spacer group 3
                                            > spacer threshold 3
                                        Spacer group 4
                                            > spacer threshold 4
                                        Spacer group 5
                                        The threshold values are preset (see below) and can be adjusted:
                                        •   Spacer threshold 1 = 10 mm
                                        •   Spacer threshold 2 = 12 mm
                                        •   Spacer threshold 3 = 16 mm
                                        •   Spacer threshold 4 = 18 mm
                                        Each spacer rack group includes the following racks, in production sequence
                                        (small to big because the lites need to be repacked after the line):
                                        •   Series (series flag set or quantity ≥ 10)
                                        •   Small units, condition small unit, default setting:
                                            – short edge < 300 or
                                            – long edge < 500)
                                        •   Common units
                                        •   Large units, condition large unit, default setting:
                                            – long edge > 2100 or
                                            – short edge > 1600)
                                        The production sequence on each rack is grouped by customer and order. The
                                        sequence of items within the order is free (freedom of optimization). With the
3.00 / 01-2023




                                        exception of serial racks, a rack may accommodate several customers and or-
                                        ders. Series will be stacked separately, per item.




                 A+W Production Detailed Scheduling                                                             D-93
                 Organizations                                                                              Tutorial




                                 There are buffer racks for the lites which do not match any of the above rack
                                 groups; these racks will not be optimized however. There are:
                                 •   Toughened glass lites
                                 •   Laminated glass lites
                                 •   Non-allocated lites

                                 Optimization
                                 This organization can be optimized by XOPTS mode 5/1 or higher. This de-
                                 pends on the amount of sorting the IG producer is willing to invest, and on the
                                 optimization result.
                                 The stricter the restrictions for an A rack, the higher the waste that is likely to
                                 occur.
                                 The drawbacks of this organization are that on the one hand, it might use very
                                 many racks while on the other hand, much sorting will be required after pro-
                                 duction.

                                 Number ranges
                                 The organization will allocate the lites to the racks. The following racks and
                                 number areas have been defined for this purpose:

                                 Organization group              Rack                                Number range
                                                                                                      from     to

                                 Buffer                          Buffer                             10000    10999

                                 Toughened - processed           processed - series                 8951     8999

                                 Toughened - processed           processed - large lites            8921     8950

                                 Toughened - processed           processed - small lites            8901     8920

                                 Toughened - processed           processed                          8501     8899

                                 Toughened - arrissed            Arrissed - large lites             8421     8450

                                 Toughened - arrissed            Arrissed - small lites             8401     8420

                                 Toughened - arrissed            Arrissed                           8001     8399

                                 Toughened - arrissed            Arrissed - series                  8451     8499

                                 Single annealed                 large lites                        7921     7950

                                 Single annealed                 small lites                        7901     7920

                                 Single annealed                 Single                             7501     7899

                                 Single annealed                 Series                             7951     7999

                                 Tab. D-2     Number ranges for production organization A racks spacers
3.00 / 01-2023




                 D-94                                                          A+W Production Detailed Scheduling
                 Tutorial                                                                                  Organizations




                                        Organization group              Rack                               Number range
                                                                                                            from     to

                                        Single annealed - bevelled      bevelled - series                 7451    7499

                                        Single annealed - bevelled      bevelled - large lites            7421    7450

                                        Single annealed - bevelled      bevelled - small lites            7401    7420

                                        Single annealed - bevelled      single - bevelled                 7001    7399

                                        Triple IG                       Triple IG - large units           6921    6950

                                        Triple IG                       Triple IG                         6001    6899

                                        Triple IG                       Triple IG - small units           6901    6920

                                        Triple IG                       Triple IG - series                6951    6999

                                        IG - shaped bars - szrgr1       IG -1 - ShapeBars - small         1311    1320

                                        IG - shaped bars - szrgr1       IG -1 - ShapeBars - series        1351    1399

                                        IG - shaped bars - szrgr1       IG -1 - ShapeBars                 1901    1950

                                        IG - shaped bars - szrgr1       IG -1 - ShapeBars - large         1321    1350

                                        IG - shaped bars - szrgr2       IG -2 - ShapeBars - large         2321    2350

                                        IG - shaped bars - szrgr2       IG -2 - ShapeBars - small         2311    2320

                                        IG - shaped bars - szrgr2       IG -2 - ShapeBars - series        2351    2399

                                        IG - shaped bars - szrgr2       IG -2 - ShapeBars                 2901    2950

                                        IG - shaped bars - szrgr3       IG -3 - ShapeBars - large         3321    3350

                                        IG - shaped bars - szrgr3       IG -3 - ShapeBars                 3901    3950

                                        IG - shaped bars - szrgr3       IG -3 - ShapeBars - small         3311    3320

                                        IG - shaped bars - szrgr3       IG -3 - ShapeBars - series        3351    3399

                                        IG - shaped bars - szrgr4       IG -4 - ShapeBars - series        4351    4399

                                        IG - shaped bars - szrgr4       IG -4 - ShapeBars                 4901    4950

                                        IG - shaped bars - szrgr4       IG -4 - ShapeBars - small         4311    4320

                                        IG - shaped bars - szrgr4       IG -4 - ShapeBars - large         4321    4350

                                        IG - shaped bars - szrgr5       IG -5 - ShapeBars - series        5351    5399

                                        IG - shaped bars - szrgr5       IG -5 - ShapeBars - small         5311    5320

                                        IG - shaped bars - szrgr5       IG -5 - ShapeBars                 5901    5950

                                        IG - shaped bars - szrgr5       IG -5 - ShapeBars - large         5321    5350

                                        IG - shapes - szrgr1            IG-1 - shapes - unsealed          1241    1250

                                        IG - shapes - szrgr1            IG-1 - Shapes                     1701    1799
3.00 / 01-2023




                                        IG - shapes - szrgr1            IG -1 - Shapes - small units      1211    1220

                                        Tab. D-2      Number ranges for production organization A racks spacers


                 A+W Production Detailed Scheduling                                                               D-95
                 Organizations                                                                             Tutorial




                                 Organization group              Rack                               Number range
                                                                                                     from     to

                                 IG - shapes - szrgr1            IG -1 - Shapes - large units      1221     1240

                                 IG - shapes - szrgr1            IG-1 - shapes - series            1251     1299

                                 IG - shapes - szrgr2            IG -2 - Shapes - small units      2211     2220

                                 IG - shapes - szrgr2            IG-2 - shapes - series            2251     2299

                                 IG - shapes - szrgr2            IG-2 - Shapes                     2701     2799

                                 IG - shapes - szrgr2            IG -2 - Shapes - large units      2221     2240

                                 IG - shapes - szrgr2            IG-2 - shapes - unsealed          2241     2250

                                 IG - shapes - szrgr3            IG -3 - Shapes - large units      3221     3240

                                 IG - shapes - szrgr3            IG-3 - shapes - unsealed          3241     3250

                                 IG - shapes - szrgr3            IG -3 - Shapes - small units      3211     3220

                                 IG - shapes - szrgr3            IG-3 - shapes - series            3251     3299

                                 IG - shapes - szrgr3            IG-3 - Shapes                     3701     3710

                                 IG - shapes - szrgr4            IG-4 - Shapes                     4701     4799

                                 IG - shapes - szrgr4            IG -4 - Shapes - large units      4221     4240

                                 IG - shapes - szrgr4            IG-4 - shapes - unsealed          4241     4250

                                 IG - shapes - szrgr4            IG-4 - shapes - series            4251     4299

                                 IG - shapes - szrgr4            IG -4 - Shapes - small units      4211     4220

                                 IG - shapes - szrgr5            IG-5 - shapes - series            5251     5299

                                 IG - shapes - szrgr5            IG-5 - shapes - unsealed          5241     5250

                                 IG - shapes - szrgr5            IG -5 - Shapes - large units      5221     5240

                                 IG - shapes - szrgr5            IG -5 - Shapes - small units      5211     5220

                                 IG - shapes - szrgr5            IG-5 - Shapes                     5701     5799

                                 IG - Georgian bars - szrgr1     IG-1 - Georgian bars - series     1451     1499

                                 IG - Georgian bars - szrgr1     IG-1 - Georgian bars - small      1411     1420

                                 IG - Georgian bars - szrgr1     IG-1 - Georgian bars              1801     1899

                                 IG - Georgian bars - szrgr1     IG-1 - Georgian bars - large      1421     1450

                                 IG - Georgian bars - szrgr2     IG-2 - Georgian bars - small      2411     2420

                                 IG - Georgian bars - szrgr2     IG-2 - Georgian bars - large      2421     2450

                                 IG - Georgian bars - szrgr2     IG-2 - Georgian bars              2801     2899

                                 IG - Georgian bars - szrgr2     IG-2 - Georgian bars - series     2451     2499
3.00 / 01-2023




                                 IG - Georgian bars - szrgr3     IG-3 - Georgian bars - large      3421     3450

                                 Tab. D-2      Number ranges for production organization A racks spacers


                 D-96                                                      A+W Production Detailed Scheduling
                 Tutorial                                                                                  Organizations




                                        Organization group              Rack                               Number range
                                                                                                            from     to

                                        IG - Georgian bars - szrgr3     IG-3 - Georgian bars - small      3411    3420

                                        IG - Georgian bars - szrgr3     IG-3 - Georgian bars - series     3451    3499

                                        IG - Georgian bars - szrgr3     IG-2 - Georgian bars              3801    3899

                                        IG - Georgian bars - szrgr4     IG-4 - Georgian bars - small      4411    4420

                                        IG - Georgian bars - szrgr4     IG-4 - Georgian bars - series     4451    4499

                                        IG - Georgian bars - szrgr4     IG-4 - Georgian bars              4801    4899

                                        IG - Georgian bars - szrgr4     IG-4 - Georgian bars - large      4421    4450

                                        IG - Georgian bars - szrgr5     IG-5 - Georgian bars              5801    5899

                                        IG - Georgian bars - szrgr5     IG-5 - Georgian bars - large      5421    5450

                                        IG - Georgian bars - szrgr5     IG-5 - Georgian bars - series     5451    5499

                                        IG - Georgian bars - szrgr5     IG-5 - Georgian bars - small      5411    5420

                                        IG - stepped - szrgr1           IG-1 - stepped                    1951    1999

                                        IG - stepped - szrgr1           IG -1 - stepped - large units     1521    1550

                                        IG - stepped - szrgr1           IG -1 - stepped - small units     1511    1520

                                        IG - stepped - szrgr1           IG-1 - stepped - series           1551    1599

                                        IG - stepped - szrgr2           IG-2 - stepped                    2951    2999

                                        IG - stepped - szrgr2           IG -2 - stepped - large units     2521    2550

                                        IG - stepped - szrgr2           IG-2 - stepped - series           2551    2599

                                        IG - stepped - szrgr2           IG -2 - stepped - small units     2511    2520

                                        IG - stepped - szrgr3           IG -3 - stepped - small units     3511    3520

                                        IG - stepped - szrgr3           IG-3 - stepped                    3951    3999

                                        IG - stepped - szrgr3           IG -3 - stepped - large units     3521    3550

                                        IG - stepped - szrgr3           IG-3 - stepped - series           3551    3599

                                        IG - stepped - szrgr4           IG-4 - stepped                    4951    4999

                                        IG - stepped - szrgr4           IG-4 - stepped - series           4551    4599

                                        IG - stepped - szrgr4           IG -4 - stepped - large units     4521    4550

                                        IG - stepped - szrgr4           IG -4 - stepped - small units     4511    4520

                                        IG - stepped - szrgr5           IG-5 - stepped                    5951    5999

                                        IG - stepped - szrgr5           IG -5 - stepped - large units     5521    5550

                                        IG - stepped - szrgr5           IG -5 - stepped - small units     5511    5520
3.00 / 01-2023




                                        IG - stepped - szrgr5           IG-5 - stepped - series           5551    5599

                                        Tab. D-2      Number ranges for production organization A racks spacers


                 A+W Production Detailed Scheduling                                                               D-97
                 Organizations                                                                            Tutorial




                                 Organization group             Rack                               Number range
                                                                                                    from     to

                                 IG-szrgr1                      IG-1 - small units                1111     1120

                                 IG-szrgr1                      IG-1                              1601     1699

                                 IG-szrgr1                      IG-1 - large units                1121     1150

                                 IG-szrgr1                      IG-1 - series                     1151     1199

                                 IG-szrgr2                      IG-2 - large units                2121     2150

                                 IG-szrgr2                      IG-2 - small units                2111     2120

                                 IG-szrgr2                      IG-2                              2601     2699

                                 IG-szrgr2                      IG-2 - series                     2151     2199

                                 IG-szrgr3                      IG-3                              3601     3699

                                 IG-szrgr3                      IG-3 - small units                3111     3120

                                 IG-szrgr3                      IG-3 - series                     3151     3199

                                 IG-szrgr3                      IG-3 - large units                3121     3150

                                 IG-szrgr4                      IG-4 - small units                4111     4120

                                 IG-szrgr4                      IG-4                              4601     4699

                                 IG-szrgr4                      IG-4 - large units                4121     4150

                                 IG-szrgr4                      IG-4 - series                     4151     4199

                                 IG-szrgr5                      IG-5 - large units                5121     5150

                                 IG-szrgr5                      IG-5 - small units                5111     5120

                                 IG-szrgr5                      IG-5 - series                     5151     5199

                                 IG-szrgr5                      IG-5                              5601     5699

                                 Laminated glass                Laminated - large lites           9921     9950

                                 Laminated glass                Laminated - series                9951     9990

                                 Laminated glass                Laminated glass                   9001     9899

                                 Laminated glass                Laminated - small lites           9901     9920

                                 Tab. D-2     Number ranges for production organization A racks spacers

                                 The organization A racks spacers uses units for optimization. It is easy to han-
                                 dle but causes more sorting work after the line, plus you will need more space
                                 for racks:
3.00 / 01-2023




                 D-98                                                     A+W Production Detailed Scheduling
                 Tutorial                                                                             Organizations




                                        Settings in A+W Production
                                        The following dialogs show the appropriate settings in A+W Production for
                                        ISO-SZRGR1.
                                        Settings for the organization group:




                                        Fig. D-39     Settings for the organization group
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                           D-99
                 Organizations                                                                     Tutorial




                                 Rack settings




                                 Fig. D-40   Rack settings


                                 Additional information
                                  Software Reference, “Organization Groups” on page D-140
                                  Software Reference, “Rack Settings” on page D-142
3.00 / 01-2023




                 D-100                                                  A+W Production Detailed Scheduling
                 Tutorial                                                                                   Organizations




                                        IG A racks
                                        The A rack organization supplies a moderately dispatch-oriented production
                                        sequence by customer and order. The only restriction is that just a few racks
                                        can be used in front of the line. The degree of dispatch organization can be
                                        controlled by the global settings for classification and sorting.
                                        With this organization, repacking will be called for after IG production.
                                        •   Only A racks will be used (200 mm in depth and 2000 mm in width).
                                        •   The stacking mode is “unit”.

                                        Production sequence
                                        The production sequence consists of the following rack groups (in production
                                        sequence):
                                        •   Common IG lites
                                        •   IG shapes
                                        •   IG shapes with Georgian bars
                                        •   IG lites with Georgian bars
                                        •   Stepped IG
                                        •   Triple IG
                                        These rack groups are split into (in production sequence):
                                        •   Series (series flag set or quantity ≥ 10)
                                        •   Small units, condition small unit, default setting:
                                            – short edge < 300 or
                                            – long edge < 500)
                                        •   Common units
                                        •   Large units, condition large unit, default setting:
                                            – long edge > 2100 or
                                            – short edge > 1600)
                                        Because repacking is required after the line, the sequence runs from small to
                                        large.
                                        lites that do not fit one of the above rack groups; will be stacked on buffer racks
                                        which will not be optimized, however. There are:
                                        •   Toughened glass lites
                                        •   Laminated glass lites
                                        •   Non-allocated lites

                                        Grouping and sorting
                                        Grouping and sorting of the lites on each rack depends on the general settings
                                        for grouping and sorting.
                                        With the exception of serial racks, most of the A racks will accommodate sev-
                                        eral customers and orders. Series will be stacked separately, per item.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-101
                 Organizations                                                                                Tutorial




                                 Default
                                 The global sorting parameters are set as follows:
                                 •   Grouping = customer+order
                                 •   Sorting = none
                                 This means that customer orders will be kept together on the above racks (e.g.
                                 common IG - small units). This requires that combinations of different glass
                                 types are united in front of the line (i.e. taken from different racks). The se-
                                 quence of items within the order is free (freedom of optimization).

                                 Changing the setting
                                 If there is only little space in front of the line, the global settings can be
                                 changed:
                                 •   Grouping = article+customer+order
                                 •   Sorting = none
                                 The additional product code makes sure that on the racks, one glass combi-
                                 nation will be processed after the other. As a result, only the individual glass
                                 combinations will be produced in dispatch order. The product mix thus deter-
                                 mines the degree of dispatch-orientation.

                                 Optimization
                                 This organization can be optimized by XOPTS mode 5/1 or higher. This de-
                                 pends on the amount of sorting the IG producer is willing to invest, and on the
                                 optimization result.
                                 The stricter the restrictions for an A rack, the higher the waste that is likely to
                                 occur.

                                 Number ranges
                                 The organization will allocate the lites to the racks. The following racks and
                                 number areas have been defined for this purpose:

                                 Organization group          Rack                                  Number range
                                                                                                    from     to

                                 Buffer                      Buffer                              10000     10999

                                 Toughened - processed       processed                           8501      8899

                                 Toughened - processed       processed - small lites             8901      8920

                                 Toughened - processed       processed - large lites             8921      8950

                                 Toughened - processed       processed - series                  8951      8999

                                 Toughened - arrissed        Arrissed                            8001      8399

                                 Toughened - arrissed        arrissed - large lites              8421      8450
3.00 / 01-2023




                                 Toughened - arrissed        arrissed - series                   8451      8499

                                 Tab. D-3      Number ranges for production organization A racks



                 D-102                                                       A+W Production Detailed Scheduling
                 Tutorial                                                                                     Organizations




                                        Organization group          Rack                                  Number range
                                                                                                           from     to

                                        Toughened - arrissed        arrissed - small lites             8401       8420

                                        Single annealed             Series                             7951       7999

                                        Single annealed             Single                             7501       7899

                                        Single annealed             large lites                        7921       7950

                                        Single annealed             small lites                        7901       7920

                                        Single annealed - bevelled bevelled - small lites              7401       7420

                                        Single annealed - bevelled bevelled - large lites              7421       7450

                                        Single annealed - bevelled bevelled - series                   7451       7499

                                        Single annealed - bevelled single - bevelled                   7001       7399

                                        IG                          IG                                 1001       1899

                                        IG                          IG - small units                   1901       1920

                                        IG                          IG - series                        1951       1999

                                        IG                          IG - large units                   1921       1950

                                        Triple IG                   Triple IG                          6001       6899

                                        Triple IG                   Triple IG - small units            6901       6920

                                        Triple IG                   Triple IG - series                 6951       6999

                                        Triple IG                   Triple IG - large units            6921       6950

                                        IG - shapes                 IG - shapes - series               2951       2999

                                        IG - shapes                 IG - shapes - small units          2901       2920

                                        IG - shapes                 IG shapes                          2001       2899

                                        IG - shapes                 IG - shapes - large units          2921       2940

                                        IG - shapes                 IG - shapes - unsealed             2941       2950

                                        IG - shapes - Georgian      IG - shapes - Georgian bars -      3951       3999
                                        bars                        series

                                        IG - shapes - Georgian      IG - shapes - Georgian bars -      3901       3920
                                        bars                        small

                                        IG - shapes - Georgian      IG - shapes - Georgian bars        3001       3899
                                        bars

                                        IG - shapes - Georgian      IG - shapes - Georgian bars -      3921       3950
                                        bars                        large

                                        IG - Georgian bars          IG - Georgian bars - small units   4901       4920
3.00 / 01-2023




                                        IG - Georgian bars          IG - Georgian bars                 4001       4899

                                        Tab. D-3      Number ranges for production organization A racks




                 A+W Production Detailed Scheduling                                                                 D-103
                 Organizations                                                                              Tutorial




                                 Organization group          Rack                                   Number range
                                                                                                     from     to

                                 IG - Georgian bars          IG - Georgian bars - large units   4921      4950

                                 IG - Georgian bars          IG - Georgian bars - series        4951      4999

                                 IG - stepped                IG - stepped - small units         5901      5920

                                 IG - stepped                IG - stepped                       5001      5899

                                 IG - stepped                IG - stepped - large units         5921      5950

                                 IG - stepped                IG - stepped - series              5951      5999

                                 Laminated glass             Laminated - series                 9951      9990

                                 Laminated glass             Laminated - large lites            9921      9950

                                 Laminated glass             Laminated glass                    9001      9899

                                 Laminated glass             Laminated - small lites            9901      9920

                                 Tab. D-3       Number ranges for production organization A racks

                                 The A rack organization optimizes in a more dispatch-oriented way. Less sort-
                                 ing is required at the end of the line which is why less space for racks is need-
                                 ed:




                                 Settings in A+W Production
                                 The following dialogs show the appropriate settings in A+W Production for IG
                                 - small units
                                 Settings for the organization group:
3.00 / 01-2023




                 D-104                                                      A+W Production Detailed Scheduling
                 Tutorial                                                                           Organizations




                                        Fig. D-41     Settings for the organization group


                                        Rack settings




                                        Fig. D-42     Rack settings
3.00 / 01-2023




                                        Additional information
                                         Software Reference, “Organization Groups” on page D-140
                                         Software Reference, “Rack Settings” on page D-142



                 A+W Production Detailed Scheduling                                                       D-105
                 Organizations                                                                            Tutorial




                                 A racks dispatch
                                 The A rack dispatch organization produces a dispatch-oriented production se-
                                 quence; several A racks will be used alternately before the line.
                                 The arrangement of the rack groups is based on size categories which are
                                 sorted by customer. The target is to achieve a production sequence which runs
                                 from large to small (taking into account certain deviations in size); inside each
                                 category, the customer orders are kept together, to be sorted onto transport
                                 racks at the end of the line.
                                 The organization needs racks before and behind the line, and produces the li-
                                 tes in packing sequence. Racks for the individual customers have to be pro-
                                 vided after the line.
                                 •       Only A racks will be used (200 mm in depth and 2000 mm in width).
                                 •       The stacking mode is Glass.

                                 Size Categories
                                 To classify lites by size, this organization uses two threshold values (S1 and
                                 S2 in the chart).


                                     A




                                                                          B

                                 A short edge                              B long edge
                                 Fig. D-43        Size Categories


                                 Since the organization will always search for and check the short edge, only
                                 the section below the diagonal (see graph) is important. The size categories
                                 are:
                                 •       Size category 1: short edge > Si_threshold_2
                                 •       Size category 2:
                                         – short edge ≥ Si_threshold_1 and
                                         – long edge ≤ Si_threshold_2
                                 •       Size category 3:
                                         – short edge ≥ Si_threshold_1 and
                                         – long edge ≤ Si_threshold_1
                                 •       Size category 4:
3.00 / 01-2023




                                         – short edge < Si_threshold_1 and
                                         – long edge > Si_threshold_2



                 D-106                                                        A+W Production Detailed Scheduling
                 Tutorial                                                                                      Organizations




                                        •   Size category 5:
                                            – short edge < Si_threshold_1 and
                                            – long edge ≥ Si_threshold_1
                                        •   Size category 6:
                                            – short edge < Si_threshold_1 and
                                            – long edge < Si_threshold_1

                                        Production sequence
                                        The rack groups are defined according to this size scheme; the production se-
                                        quence is created after the pattern 1 ' 2 ' 3 ' 4 ' 5 ' 6, i.e. from large to small.
                                        Sorting within these categories:
                                        •   IG size 1
                                            – Series
                                            – Common IG
                                            – IG specialities (step, shape, triple, Georgian bars)
                                        •   IG size 2
                                            – Series
                                            – Common IG
                                            – Stepped IG
                                            – Triple IG
                                            – IG shapes
                                            – IG lites with Georgian bars
                                        •   IG size 3
                                            – Like size 2
                                        •   IG size 4
                                            – Like size 2
                                        •   IG size 5
                                            – Like size 2
                                        •   IG size 6
                                            – Series
                                            – Common IG
                                            – IG specialities (step, shape, triple, Georgian bars)
                                        For the largest and smallest lites, all specialities will be united.

                                        Grouping and Sorting
                                        The rack group (size) is classified by:
                                        Customer + product + GeorgianCode + shape + steps
                                        lites for a certain customer usually have to be taken alternately from the racks
                                        of a size category. The product number makes sure that identical glass struc-
                                        tures are kept in production sequence (usually, same rack).
                                        Otherwise, steps range before shapes, and shapes before Georgian bars. Se-
3.00 / 01-2023




                                        ries are stacked separately, per item, but will be added to the production se-
                                        quence. All other A racks hold several customer orders.




                 A+W Production Detailed Scheduling                                                                  D-107
                 Organizations                                                                                Tutorial




                                 Number ranges
                                 The organization will allocate the lites to the racks. The following racks and
                                 number areas have been defined for this purpose:

                                 Organization group          Rack                               Number range
                                                                                                 from     to

                                 Buffer                      Buffer                            10000        10999

                                 Toughened - processed       processed - large lites           8921         8950

                                 Toughened - processed       processed - small lites           8901         8920

                                 Toughened - processed       processed                         8501         8899

                                 Toughened - processed       processed - series                8951         8999

                                 Toughened - arrissed        arrissed - large lites            8421         8450

                                 Toughened - arrissed        Arrissed                          8001         8399

                                 Toughened - arrissed        arrissed - small lites            8401         8420

                                 Toughened - arrissed        arrissed - series                 8451         8499

                                 Single annealed             small lites                       7901         7920

                                 Single annealed             large lites                       7921         7950

                                 Single annealed             Single                            7501         7899

                                 Single annealed             Series                            7951         7999

                                 Single annealed - bevelled bevelled - small lites             7401         7420

                                 Single annealed - bevelled single - bevelled                  7001         7399

                                 Single annealed - bevelled bevelled - large lites             7421         7450

                                 Single annealed - bevelled bevelled - series                  7451         7499

                                 IG Size 1                   Common IG size 1                  1001         1499

                                 IG Size 1                   Special IG size 1                 1801         1899

                                 IG Size 1                   IG - series - size 1              1951         1999

                                 IG Size 2                   IG - series - size 2              2951         2999

                                 IG Size 2                   Common IG size 2                  2001         2499

                                 IG Size 2                   IG Georgian bars size 2           2601         2699

                                 IG Size 2                   IG shapes size 2                  2501         2599

                                 IG Size 2                   Triple IG SizeCat 2               2701         2799

                                 IG Size 2                   IG stepped size 2                 2801         2899

                                 Tab. D-4      Number ranges for production organization A racks dispatch
3.00 / 01-2023




                 D-108                                                       A+W Production Detailed Scheduling
                 Tutorial                                                                                    Organizations




                                        Organization group         Rack                                Number range
                                                                                                        from     to

                                        IG Size 3                  Common IG size 3                   3001         3499

                                        IG Size 3                  IG stepped size 3                  3801         3899

                                        IG Size 3                  Triple IG SizeCat 3                3701         3799

                                        IG Size 3                  IG shapes size 3                   3501         3599

                                        IG Size 3                  IG - series - size 3               3951         3999

                                        IG Size 3                  IG Georgian bars size 3            3601         3699

                                        IG Size 4                  IG Georgian bars size 4            4601         4699

                                        IG Size 4                  Common IG size 4                   4001         4499

                                        IG Size 4                  IG stepped size 4                  4801         4899

                                        IG Size 4                  Triple IG SizeCat 4                4701         4799

                                        IG Size 4                  IG shapes size 4                   4501         4599

                                        IG Size 4                  IG - series - size 4               4951         4999

                                        IG Size 5                  Common IG size 5                   5001         5499

                                        IG Size 5                  IG - series - size 5               5951         5999

                                        IG Size 5                  Triple IG SizeCat 5                5701         5799

                                        IG Size 5                  IG shapes size 5                   5501         5599

                                        IG Size 5                  IG Georgian bars size 5            5601         5699

                                        IG Size 5                  IG stepped size 5                  5801         5899

                                        IG Size 6                  IG - series - size 6               6951         6999

                                        IG Size 6                  Common IG size 6                   6001         6499

                                        IG Size 6                  Special IG size 6                  6801         6899

                                        Laminated glass            Laminated glass                    9001         9899

                                        Laminated glass            Laminated - small lites            9901         9920

                                        Laminated glass            Laminated - large lites            9921         9950

                                        Laminated glass            Laminated - series                 9951         9990

                                        Tab. D-4      Number ranges for production organization A racks dispatch
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-109
                 Organizations                                                                           Tutorial




                                 The organization A racks dispatch optimizes directly with regard to packing
                                 and shipping. This will require more racks at the end of the line (per customer/
                                 order) but the stacking logic for the lites is simpler.




                                 Settings in A+W Production
                                 The following dialogs show the appropriate settings in A+W Production for IG
                                 series size category 1.
                                 Settings for the organization group:




                                 Fig. D-44    Settings for the organization group
3.00 / 01-2023




                 D-110                                                     A+W Production Detailed Scheduling
                 Tutorial                                                                           Organizations




                                        Rack settings




                                        Fig. D-45     Rack settings


                                        Additional information
                                         Software Reference, “Organization Groups” on page D-140
                                         Software Reference, “Rack Settings” on page D-142
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                       D-111
                 Organizations                                                                             Tutorial




                                 Harp racks, no filling up
                                 Structure and rack allocation of the harp rack organization is similar to the A
                                 rack organization only that harp racks will be used chiefly.
                                 This produces a much better yield. Big and small units as well as series will be
                                 put onto A racks.
                                 Compared with an A rack organization, an important difference is the dispatch-
                                 oriented production sequence. Even if the harp rack organization handles one
                                 rack after the other in front of the line, the required glass types can be put onto
                                 harp rack, in dispatch sequence.

                                 Production sequence
                                 Rack groups used (in production sequence):
                                 •   Common IG lites
                                 •   IG shapes
                                 •   IG shapes with Georgian bars
                                 •   IG lites with Georgian bars
                                 •   Stepped IG
                                 •   Triple IG
                                 To make direct packing possible in part, the rack groups range from large to
                                 small (in production sequence):
                                 •   Series: A rack, (series flag set or quantity ≥10)
                                 •   Large units: A rack, condition large unit, default setting:
                                     – long edge > 2100 or
                                     – short edge > 1600)
                                 •   Common units: harp racks
                                 •   Small units: A rack, condition small unit, default setting:
                                     – short edge < 300 or
                                     – long edge < 500)

                                 Grouping and Sorting
                                 Harp racks have 60 individually numbered slots. The lites on the harp racks
                                 are sorted by Customer+order+item while the A racks are sorted by Custom-
                                 er+order.
                                 lites belonging to the same product structure, will be set onto the harp rack
                                 next to another. Manually cut lites and ancillaries have to be added.
                                 In any of the rack groups (in production sequence) there may be harp racks
                                 which only contain a small number of lites at the end. For the rack group
                                 Shaped bars for example there is a rack with just two units if the production
                                 batch does not include more shaped bars. This effect is avoided in the Filled
                                 harp racks organization.
3.00 / 01-2023




                 D-112                                                     A+W Production Detailed Scheduling
                 Tutorial                                                                                      Organizations




                                        Optimization
                                        Jobs which include only lites for harp racks will be optimized as free optimiza-
                                        tions. If an optimization includes A rack lites, sequenced optimization will be
                                        used. The lites on the harp racks will be optimized without restrictions; the ef-
                                        fect is the same as for free optimization.

                                           Harp racks not filled!
                                           It is important for this organization that harp racks are not filled, i.e. the harp
                                           racks will not be used to the best effect. Some of the slots may remain emp-
                                           ty as the items will not be split. If an order item does not fit into the remain-
                                           ing slots of the harp rack, a new harp rack number will be allocated!

                                           The sorting on the harp rack is determined by the classification (or sorting),
                                           depending on the rack organization.

                                        Number ranges
                                        The organization will allocate the lites to the racks. The following racks and
                                        number areas have been defined for this purpose:

                                        Organization group          Rack                                 Number range
                                                                                                          from     to

                                        Buffer                      Buffer                              10000     10999

                                        Toughened - processed       processed - large lites             8921      8950

                                        Toughened - processed       processed - small lites             8901      8920

                                        Toughened - processed       processed                           8500      8899

                                        Toughened - processed       processed - series                  8951      8999

                                        Toughened - arrissed        arrissed - series                   8451      8499

                                        Toughened - arrissed        arrissed - large lites              8421      8450

                                        Toughened - arrissed        arrissed - small lites              8401      8420

                                        Toughened - arrissed        Arrissed                            8000      8399

                                        Single annealed             Series                              7951      7999

                                        Single annealed             small lites                         7901      7920

                                        Single annealed             Single                              7500      7899

                                        Single annealed             large lites                         7921      7950

                                        Single annealed - bevelled bevelled - large lites               7421      7450

                                        Single annealed - bevelled bevelled - small lites               7401      7420

                                        Single annealed - bevelled single - bevelled                    7000      7399

                                        Single annealed - bevelled bevelled - series                    7451      7499
3.00 / 01-2023




                                        Tab. D-5      Number ranges for production organization harp racks, no filling up




                 A+W Production Detailed Scheduling                                                                   D-113
                 Organizations                                                                                 Tutorial




                                 Organization group           Rack                                 Number range
                                                                                                    from     to

                                 IG                           IG                                  100       1899

                                 IG                           IG - small units                    1901      1920

                                 IG                           IG - large units                    1921      1950

                                 IG                           IG - series                         1951      1999

                                 Triple IG                    Triple IG                           6000      6899

                                 Triple IG                    Triple IG - large units             6921      6950

                                 Triple IG                    Triple IG - series                  6951      6999

                                 Triple IG                    Triple IG - small units             6901      6920

                                 IG - shapes                  IG - shapes - small units           2901      2920

                                 IG - shapes                  IG - shapes                         2000      2899

                                 IG - shapes                  IG - shapes - large units          2921       2940

                                 IG - shapes                  IG - shapes - series                2951      2999

                                 IG - shapes                  IG - shapes - unsealed              2941      2950

                                 IG - shapes - Georgian       IG - shapes - Georgians - large     3921      3950
                                 bars

                                 IG - shapes - Georgian       IG - shapes - Georgian bars         3000      3899
                                 bars

                                 IG - shapes - Georgian       IG - shapes - Georgians - small     3901      3920
                                 bars

                                 IG - shapes - Georgian       IG - shapes - Georgian bars -       3951      3999
                                 bars                         series

                                 IG - Georgian bars           IG - Georgian bars - series         4951      4999

                                 IG - Georgian bars           IG - Georgian bars - large units    4921      4950

                                 IG - Georgian bars           IG - Georgian bars - small units    4901      4920

                                 IG - Georgian bars           IG - Georgian bars                  4000      4899

                                 IG - stepped                 IG - stepped - small units          5901      5920

                                 IG - stepped                 IG - stepped - large units          5921      5950

                                 IG - stepped                 IG - stepped - series               5951      5999

                                 IG - stepped                 IG - stepped                        5000      5899

                                 Laminated glass              Laminated - series                  9951      9990

                                 Laminated glass              Laminated - large lites             9921      9950
3.00 / 01-2023




                                 Laminated glass              Laminated - small lites             9901      9920

                                 Tab. D-5       Number ranges for production organization harp racks, no filling up




                 D-114                                                           A+W Production Detailed Scheduling
                 Tutorial                                                                                      Organizations




                                        Organization group          Rack                                 Number range
                                                                                                          from     to

                                        Laminated glass             Laminated glass                     9000      9899

                                        Tab. D-5      Number ranges for production organization harp racks, no filling up

                                        The Harp rack organization optimizes dispatch-oriented; its structure and rack
                                        allocation is similar to the A rack organization; the difference is that harp racks
                                        will be used as the main racks.




                                        Settings in A+W Production
                                        The following dialogs show the appropriate settings in A+W Production for IG
                                        shapes.
                                        Settings for the organization group:




                                        Fig. D-46     Settings for the organization group
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                   D-115
                 Organizations                                                                     Tutorial




                                 Rack settings




                                 Fig. D-47   Rack settings


                                 Additional information
                                  Software Reference, “Organization Groups” on page D-140
                                  Software Reference, “Rack Settings” on page D-142
3.00 / 01-2023




                 D-116                                                  A+W Production Detailed Scheduling
                 Tutorial                                                                                Organizations




                                        Filled harp racks
                                        The Filled harp racks organization makes sure that there are no half-filled harp
                                        racks; it sorts all harp racks in production sequence. The harp racks will be
                                        handled first, followed by the A racks containing the specialties.

                                        Production sequence
                                        Rack groups used (in production sequence):

                                        • Common IG (sorted by product type)          Harp racks

                                        • IG large, small, series                     A Racks

                                        • IG shapes - large, small, series            A Racks

                                        • IG shapes/Georgian bars - large, small,     A Racks
                                          series

                                        • IG Georgian bars - large, small, series     A Racks

                                        • Stepped IG - large, small, series           A Racks

                                        • Triple IG, large, small, series             A Racks

                                        Tab. D-6      Production sequence

                                        Apart from slots kept free for adding purchased glass and manually cut glass,
                                        the harp racks are filled without gaps and will contain all common-size lites,
                                        including Georgian bars, shapes, etc.
                                        Large and small units as well as series are removed to be produced at the end.

                                        Grouping and sorting
                                        Series will be stacked separately, per item. All other A racks are grouped by
                                        Customer+order, with several orders per rack; the item sequence is free.
                                        This organization is internally sorted by product features. The sequence of li-
                                        tes on the harp racks and thus, the production sequence, can be overridden
                                        by defining a general classification and sorting.
                                        •   Grouping = none
                                        •   Sorting = none
                                        This general setting sorts the lites on the harp racks by the following product
                                        characteristics:
                                        Shapes, shaped Georgians, Georgians, steps, triple IG, and common IG
                                        These will be stacked and produced together.
                                        The following setting will keep customer orders together, notwithstanding the
                                        product characteristics:
                                        •   Grouping = customer+order
                                        •   Sorting = none
3.00 / 01-2023




                                        Shapes, Georgian bars, and triple IG will change depending on the order mix-
                                        ture; the orders are classified by product characteristics.



                 A+W Production Detailed Scheduling                                                              D-117
                 Organizations                                                                                Tutorial




                                 Harp racks have 60 individually numbered slots.
                                 The stacking mode is Unit - lites belonging to the same product structure will
                                 be put next to another on the harp racks. Manually cut lites and ancillaries
                                 have to be added.

                                 Optimization
                                 This organization is usually based on the sequence - see organization Harp
                                 racks, no filling up - but in this case, the harp racks will be filled completely
                                 even if an order item is split.

                                 Number ranges
                                 The organization will allocate the lites to the racks. The following racks and
                                 number areas have been defined for this purpose:

                                 Organization group          Rack                                  Number range
                                                                                                   from     to

                                 Buffer                      Buffer                                10000      10999

                                 Toughened - processed       processed - series                    8951       8999

                                 Toughened - processed       processed - large lites               8921       8950

                                 Toughened - processed       processed - small lites               8901       8920

                                 Toughened - processed       processed                             8500       8899

                                 Toughened - arrissed        arrissed - large lites                8421       8450

                                 Toughened - arrissed        arrissed - small lites                8401       8420

                                 Toughened - arrissed        Arrissed                              8000       8399

                                 Toughened - arrissed        arrissed - series                     8451       8499

                                 Single annealed             Single                                7500       7899


                                 Single annealed             Series                                7951       7999


                                 Single annealed             large lites                           7921       7950


                                 Single annealed             small lites                           7901       7920


                                 Single annealed - bevelled bevelled - series                      7451       7499

                                 Single annealed - bevelled bevelled - large lites                 7421       7450

                                 Single annealed - bevelled bevelled - small lites                 7401       7420

                                 Single annealed - bevelled single - bevelled                      7000       7399
3.00 / 01-2023




                                 Harp rack - filled          Harp rack - all                       11000      50999

                                 Tab. D-7       Number ranges for production organization Filled harp racks




                 D-118                                                         A+W Production Detailed Scheduling
                 Tutorial                                                                                    Organizations




                                        Organization group          Rack                                   Number range
                                                                                                           from     to

                                        IG                          IG - small units                       1901      1920

                                        IG                          IG - series                            1951      1999

                                        IG                          IG - large units                       1921      1950

                                        Triple IG                   Triple IG - small units                6901      6920

                                        Triple IG                   Triple IG - large units                6921      6950

                                        Triple IG                   Triple IG - series                     6951      6999

                                        IG - shapes                 IG - shapes - large units              2921      2940

                                        IG - shapes                 IG - shapes - small units              2901      2920

                                        IG - shapes                 IG - shapes - series                   2951      2999

                                        IG - shapes                 IG - shapes - unsealed                 2941      2950

                                        IG - shapes - Georgian      IG - shapes - Georgians - large        3921      3950
                                        bars

                                        IG - shapes - Georgian      IG - shapes - Georgian bars - series   3951      3999
                                        bars

                                        IG - shapes - Georgian      IG - shapes - Georgians - small        3901      3920
                                        bars

                                        IG - Georgian bars          IG - Georgian bars - small units       4901      4920

                                        IG - Georgian bars          IG - Georgian bars - series            4951      4999

                                        IG - Georgian bars          IG - Georgian bars - large units       4921      4950

                                        IG - stepped                IG - stepped - series                  5951      5999

                                        IG - stepped                IG - stepped - small units             5901      5920

                                        IG - stepped                IG - stepped - large units             5921      5950

                                        Laminated glass             Laminated - large lites                9921      9950

                                        Laminated glass             Laminated - series                     9951      9990

                                        Laminated glass             Laminated glass                        9000      9899

                                        Laminated glass             Laminated - small lites                9901      9920

                                        Tab. D-7       Number ranges for production organization Filled harp racks
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                   D-119
                 Organizations                                                                          Tutorial




                                 The organization Filled harp racks optimizes the lites production-oriented, ac-
                                 cording to the product properties, onto harp racks and A racks. You will need
                                 more racks but production is rather dispatch-oriented as the lites are grouped
                                 by customer and order number.




                                 Settings in A+W Production
                                 The following dialogs show the appropriate settings in A+W Production for Tri-
                                 ple IG, large units.
                                 Settings for the organization group:




                                 Fig. D-48    Settings for the organization group
3.00 / 01-2023




                 D-120                                                     A+W Production Detailed Scheduling
                 Tutorial                                                                           Organizations




                                        Rack settings




                                        Fig. D-49     Rack settings


                                        Additional information
                                         Software Reference, “Organization Groups” on page D-140
                                         Software Reference, “Rack Settings” on page D-142
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                       D-121
                 Organizations                                                                           Tutorial




                                 Demos and Exercises
                                 This session shows you how to define an organization in A+W Production.

                                 Trainer demo: Explaining master data
                                 The master data of A+W Production are presented and explained.
                                 The following dialog is explained from this point of view:
                                 •   Dialog Organization including the tabs
                                     – Master organization
                                     – Production sequence
                                     – Sequence of checks

                                 Exercise 1: Define a master organization
                                 Set up a master organization according to the following specifications.
                                 •   Name of the organization: New training organization.
                                 •   Production groups: by customer number+order number
                                 •   Name of the organization type: New training
                                 •   Type of the organization type: Standard
                                 •   Stacking mode: Unit
                                 •   Name of the organization group: Buffer rack
                                 •   Rack settings: A rack, super group formation: +customer number+order
                                     number, no sorting within the groups, complete groups are stacked togeth-
                                     er, optimization behavior 5.1, stacking mode unit.

                                 Exercise 1: Solution
                                 The individual steps for this task are performed in the following dialogs:
                                 •   Organization dialog
                                 •   Master organization dialog
                                 •   Dialog Rack settings


                                  Define a master organization
                                 1 Open the Organization dialog in Master Data > Detailed Scheduling.
                                 2 Press the [New] button. The dialog Master organization appears.
                                 3 In field Name of Master Organization, enter New training organization.
                                 4 Open the combo box Production Groups and select +Customer number-
                                   Order number.
                                 5 Press [OK]. The dialog closes and you will find yourself back in the Orga-
                                   nization dialog.
                                 6 The new organization appears on the list.
3.00 / 01-2023




                 D-122                                                   A+W Production Detailed Scheduling
                 Tutorial                                                                             Organizations




                                         Define the production sequence
                                        1 Open the tab Production Sequence.
                                        2 Press the [New] button. The entry unknown/standard is added.
                                        3 Press the [Settings] button. The Organization dialog appears.
                                        4 Go to the field Name of Organization Type and enter New training.
                                        5 In section Stacking Mode, tick Unit.
                                        6 Press [OK]. The dialog closes and you will find yourself back on tab Pro-
                                          duction Sequence.


                                         Define the organization group
                                        1 Select the just created organization type New training and press button
                                          [New]. The entry noname is added.
                                        2 Press the [Settings] button. The dialog Organization Groups appears.
                                        3 Go to field Name and enter Buffer rack.
                                        4 In section Group Formation, choose Customer Number.
                                        5 Tick the checkbox Sorting of Groups.
                                        6 Press [OK]. The dialog closes and you will find yourself back on tab Pro-
                                          duction Sequence.


                                         Define a rack
                                        1 Select the just defined organization group Reception Rack and press
                                          [New]. The entry unknown is added.
                                        2 Press the [Settings] button. The dialog Rack Settings appears.
                                        3 Go to field Name and enter A rack.
                                        4 In section Group Formation, select +Customer number+Order number.
                                        5 Go to combo box Sorting of Groups and select None.
                                        6 In section Stacking Mode Groups, select Complete Groups Together and in
                                          section Optimization behaviour, 5.1.
                                        7 Tick the checkbox Reception Rack.


                                        Additional information
                                         Software Reference, “Organization” on page D-138
                                         Software Reference, “Organization Groups” on page D-140
                                         Software Reference, “Rack Settings” on page D-142
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                          D-123
                 Organizations                              Tutorial
3.00 / 01-2023




                 D-124           A+W Production Detailed Scheduling
Detailed Scheduling             D

                 Software Reference




                A+W Production
                 Software Reference                                                                            Overview




                                        Overview
                                        Open menu Master data > Detailed Scheduling
                                        Menu Detailed Scheduling offers the following items:
                                        •   Presettings:
                                            You will need this menu if no settings have been made with regard to orga-
                                            nization, grouping and sorting in the organization, or regarding the sorting
                                            on the rack.
                                             “Default Settings” on page D-146
                                        •   Organization:
                                            This menu is used for setting up the organizations. You can define the pro-
                                            duction sequence and the sequence of checks
                                             Software Reference, “Tab Master Organization” on page D-128
                                             Software Reference, “Tab Production Sequence” on page D-130
                                             Software Reference, “Tab Test Sequence” on page D-132
                                        •   Grouping:
                                            This menu item serves to define the grouping and sorting.
                                             Software Reference, “Grouping/Sorting Dialog” on page D-147
                                        •   Racks:
                                            This menu is used for rack definition.
                                             Software Reference, “Racks” on page D-153
                                        •   Processing:
                                            This menu can be used to define new processing steps or change existing
                                            ones.
                                        •   Batch Types
                                            This menu allows defining batch types and allocating processing steps
                                             Software Reference, “Lot Types and Processings” on page D-158

                                            Dialogs are accessible from different points
                                            Please note that there are various ways of opening functions and dialogs.
                                            These instructions will describe the corresponding dialogs just once.

                                        Instructions on how to open individual dialogs are provided again in the follow-
                                        ing dialog descriptions. If there are several ways of opening a dialog, these are
                                        specified as well.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                              D-127
                 Organizations                                                               Software Reference




                                 Organizations
                                 Master Data > Detailed Scheduling > Organization
                                 This dialog is used for entering or changing master organizations, organiza-
                                 tions, or organization groups. Settings regarding the production sequence and
                                 the sequence of checks can be made as well. For detailed information, please
                                 see the explanations on the individual tabs.
                                 The dialog is split into the following tabs:
                                 •   “Tab Master Organization” on page D-128
                                 •   “Tab Production Sequence” on page D-130
                                 •   “Tab Test Sequence” on page D-132
                                 •   “Default Settings” on page D-146


                                 Tab Master Organization
                                 Master Data > Detailed Scheduling > Organization




                                 Fig. D-50    Organization dialog, tab Master organization


                                 Tab Master Organization is used for defining new master organizations or
                                 change existing ones. These master organizations will be allocated to batches
                                 in detailed scheduling. The left window shows all existing master organizations
                                 in a tree structure. Click on the plus sign to open a master organization and
                                 view the organization allocated to this master organization. The right window
                                 shows all existing organizations.
3.00 / 01-2023




                 D-128                                                     A+W Production Detailed Scheduling
                 Software Reference                                                                        Organizations




                                        The symbols in the right window mean:

                                              Standard organization / Application
                                              Standard organization / Production
                                              Non-Standard organization / Produc-
                                              tion
                                              Non-Standard organization /
                                              Application
                                        Fig. D-51     Explanation of organization symbols


                                        Description of buttons

                                        New Use this button to open the dialog Master organization which allows de-
                                        fining a new master organization. To define a new master organization you
                                        have to select the first entry in the tree structure in the left window, Master Or-
                                        ganization.

                                        Deletion Use this button to delete the master organization selected in the left
                                        window. The selected organization will be deleted.

                                           Deletion without security check
                                           If you have deleted something by mistake, leave the Organization Dialog
                                           via button [Abort]. Next time you open it, the data will still be there.

                                        Settings Use this button to open the Master Organization dialog or the mas-
                                        ter organization selected in the left window.


                                        Additional information
                                         Tutorial, “Master Organization” on page D-76
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                D-129
                 Organizations                                                              Software Reference




                                 Tab Production Sequence
                                 Master Data > Detailed Scheduling > Organization > tab Production Sequence




                                 Fig. D-52    Tab Production sequence


                                 Tab Production Sequence shows the sequence of the organization groups
                                 within the organization.

                                 Description of buttons

                                 Condition This button is active only for organization groups and racks be-
                                 cause conditions can be defined only for those. If you use this button after se-
                                 lecting an organization group, dialog Select Conditions opens. Define a
                                 condition for the organization group. If you use this button after selecting a
                                 rack, dialog Select conditions opens as well. Define a condition for the rack.
                                 The condition for a rack is marked by a ?.

                                 New Use to button to define a new organization, a new organization group, or
                                 a new rack. This depends on which entry has been selected. If you select Or-
                                 ganization and use button [New], a new organization (e.g. Machine allocation
                                 IG large) will be added below the last organization type. This new organization
                                 is called unknown at first. Select this new organization and use the button [Set-
                                 tings]. Dialog Organization appears in which you can make the required set-
                                 tings for this organization.
                                 When you select an organization and press button [New], a new organization
                                 group will be added at the end of the selected organization. The new organi-
                                 zation group is called noname at first. Select this new organization group and
                                 use the button [Settings]. Dialog Organization Group appears in which you can
3.00 / 01-2023




                                 make the required settings for this organization group.
                                 When you select an organization group and press button [New], a new rack
                                 will be added at the end of the selected organization group. This new rack is



                 D-130                                                    A+W Production Detailed Scheduling
                 Software Reference                                                                        Organizations




                                        called unknown at first. Select this rack and use the button [Settings]. Dialog
                                        Workstation Settings appears in which you can make the required settings for
                                        this rack.

                                        Cut Use this button to cut out the selected record and move it to the clipboard.
                                        It can then be added to another organization by using the button [Insert].
                                        Should you have cut the wrong record by mistake, the program will want to
                                        know whether the changes shall be ignored when you leave the dialog. If you
                                        confirm this question by [Yes], the cut-out record will be there next time you
                                        open the organization.

                                        Copy Use this button to transfer the selected record to the clipboard. It can
                                        then be added to another organization by using the button [Insert].

                                        Add Use this button to insert the copied or cut-out record from the clipboard.

                                        Delete Use this button to delete the selected record. If the record you want to
                                        delete is still used by an A+W Production process, a security check appears.
                                        Should you have deleted the wrong record by mistake, the system will want to
                                        know whether the changes shall be ignored when you leave the dialog. If you
                                        confirm this by [Yes], the deleted record will be available next time you open it.

                                        Settings Use this button to open the dialog for the selected entry.
                                        • Software Reference, “Organization” on page D-138
                                        • Software Reference, “Organization Groups” on page D-140
                                        • Software Reference, “Rack Settings” on page D-142
                                        • Software Reference, “Select Conditions” on page F-42

                                        Export Orga Use this button to export the selected organization.


                                        Additional information
                                         Tutorial, “Production Sequence” on page D-87
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                               D-131
                 Organizations                                                                Software Reference




                                 Tab Test Sequence
                                 Master Data > Detailed Scheduling > Organization > tab Test Sequence




                                 Fig. D-53    Organization dialog, tab Test Sequence


                                 This dialog shows the sequence of tests for an organization. This means that
                                 this tab is used to define the sequence in which the program checks whether
                                 a lite is allocated to the appropriate rack (the names of the racks are followed
                                 by the defined conditions. This way, they implicitly define the sequence in
                                 which the conditions are checked. On a rack, all allocated conditions - maxi-
                                 mally 7 per rack - are linked by an AND-operation).
                                 The right window shows the racks belonging to the organization selected in the
                                 left window. * in front of the name marks the buffer rack of this organization
                                 (which should always be found at the end of the list). Double-click on the rack
                                 you want to mark as a buffer rack. Please remember that there can be only
                                 one buffer rack per organization. This means that if there is already a buffer
                                 rack for an organization and you double-click on another rack to mark it as
                                 such, the first buffer rack becomes a normal rack again (without * ).
                                 The racks show the sequence (in descending order) in which the lites are al-
                                 located to certain racks. Depending on the set sequence of checks, a lite will
                                 be transferred from rack to rack until it meets a rack the condition of which it
                                 fulfils. It will be allocated to this rack. The columns from and to mark the range
                                 of numbers for the racks. Click on the required column to edit the range of
                                 numbers by means of this dialog.

                                 Description of buttons
3.00 / 01-2023




                                 Start Use this button to move the selected lite to first place.

                                 Up Use this button to move the selected lite one line up.



                 D-132                                                     A+W Production Detailed Scheduling
                 Software Reference                                                                     Organizations




                                        Down Use this button to move the selected lite one line down.

                                        End Use this button to move the selected lite to last place.


                                        Additional information
                                         Tutorial, “Sequence of checks” on page D-81
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                           D-133
                 Organizations                                                              Software Reference




                                 Master Organization
                                 Master Data > Detailed Scheduling > Organization > tab Master Organization
                                 > [New]
                                 Master Data > Detailed Scheduling > Organization > tab Master Organization
                                 > Select Master Organization > [Settings]




                                 Fig. D-54    Define master organization


                                 Dialog Master Organization allows defining a new master organization, or
                                 changing the settings for an existing master organization. Master organiza-
                                 tions are defined in two steps. First, define the master organization and the ap-
                                 propriate settings, then define the organizations that shall form the master
                                 organization. Further details are available in the corresponding fields.
                                 Technical info: database table: FEIN_MASTERORGA

                                 Description of fields

                                 Name of the Master Organization Enter the name of the master organiza-
                                 tion. The name of the master organization will appear in all views in connection
                                 with the organization.
                                 Technical info: Compulsory field, alpha-numeric, 32-digit, database field:
                                 NAME

                                 Stack XOPT Together Detailed scheduling allows to remove certain lites
                                 from the optimizations, and optimize them via XOPT.
                                  Despite different glass types and thicknesses, XOPT optimizations are
                                 stacked on an A rack together.
                                  Free optimizations are put separately onto A racks.
                                 Technical info: database field: TOGETHER
3.00 / 01-2023




                                 Combo box This checkbox defines the master organization type:
                                 • Standard: The usual master orga is used.



                 D-134                                                     A+W Production Detailed Scheduling
                 Software Reference                                                                        Organizations




                                        •  Quick organization: A quick organization will be run without showing the
                                           detailed scheduling views. If batches contain cut lites which undergo a
                                           quick master organization, these will be treated like manual cutting.
                                        • Phys. Rack Load: The system automatically creates a sensible load of
                                           physical racks and considers the rules and conditions (weight, size, etc.).
                                           Therefore, the Stack Optimizer will be started.
                                        Technical info: database field: QUICKORGA

                                        Creation of Pairs not Allowed This checkbox is used for triple IG. The units
                                        mainly consists of an uncoated and two coated lites; the first and third lite be-
                                        ing coated. The coating faces the airspace so that one of the two lites would
                                        have to be turned before entering the line. To turn the lite after cutting, before
                                        loading it onto the rack, detailed scheduling shall therefore put the lites onto
                                        different stacks.
                                        To put the two stacks into an identical sequence, optimization in fixed se-
                                        quence is required for this number range.
                                         Pairs must not be created.
                                         Pairs can be created.
                                        Technical info: database field: PAIRFORBIDDEN

                                        Maximum number of storage locations in optimization In this field you
                                        can specify how many stacks may be used simultaneously by the optimization.

                                        Production Groups The combo box shows all entries made on tab Group-
                                        ings in dialog Grouping/Sorting. If you select one of the groupings in this field,
                                        detailed scheduling will create production groups according to this value (as a
                                        pre-setting which can be changed later by means of the organization settings
                                        and in detailed scheduling (optimization)). The selected values refer to the ba-
                                        sic elements of the batch.
                                        Technical info: database field: ID_GROUP

                                        Pseudo High Quantities Items with identical structures can be combined in
                                        Pseudo series in detailed scheduling. The values in this combo box are taken
                                        from tab Grouping in dialog Grouping/Sorting. From this combo box, select the
                                        values to be applied to the pseudo series.
                                        Usually, single lites (individual items consisting of one lite each) must only be
                                        temporarily stored/put onto fixed racks, e.g. to wait for remakes. By means of
                                        pseudo series, identical items (single lites) can be combined in a series which
                                        can be put together on fixed rack as an exception from the rule.
                                        Pseudo series have another meaning.
                                        A series (quantity >100, but this can be defined by the customer) can pass
                                        through different production processes - different paths, different treatment. By
                                        means of pseudo series, single items can be marked as "series" and can be
                                        treated as such (the series flag will also be assigned internally).
                                        Technical info: database field: ID_PSEUDOGROUP

                                        Min. Quantity This field refers to field Pseudo series and defines the mini-
                                        mum quantity for the creation of pseudo series. If the values lies below, no
3.00 / 01-2023




                                        pseudo series will be formed.
                                        Technical info: database field: PSEUDOSCHWELLE



                 A+W Production Detailed Scheduling                                                               D-135
                 Organizations                                                                Software Reference




                                 Release At the release of the batch scheduled by this master organization,
                                 the displayed script (*.bas/*.bat file) will be used. Use button [Release] to open
                                 the dialog Select script. This dialog contains all scripts defined in the program.
                                 The scripts will be saved in the ALCIM directory in a separate file (file name:
                                 Scripts).
                                 Technical info: database field: SKRIPT

                                 Filler This field serves for optimizing lites that are thicker than ordered by the
                                 customer. These lites can be used as so-called Fillers. Prerequisite is that the
                                 lites will become part of an IG unit. Apart from that, the IG unit must fulfill the
                                 condition shown in this field. Use button [Filler] to open the formula editor. Se-
                                 lect the required formula. When you close the dialog, the name of the formula
                                 appears in the field behind the button.
                                 Technical info: database field: ID_FILLERCONDITION

                                 Pseudo Parts This field allows defining pseudo parts. Pseudo parts adopt
                                 the batch creation and rack information from their sub-elements and do not
                                 only depend on the batch type of the elements and processing steps. By de-
                                 fining a condition for the master organization you can specify the elements of
                                 the batch type for which this is permitted. Use the button [Pseudo parts] to
                                 open the formula editor. Select the required formula. When you close the dia-
                                 log, the name of the formula appears in the field behind the button.
                                 Technical info: database field: ID_QUASICONDITION

                                 Bottom Section This section deals with the use of special elements (fillers,
                                 residue plates, breakage, and rush orders). First select the special element on
                                 the list, then assign the rack number on the right.

                                 Use Filler This field refers to existing filler orders. Detailed scheduling can
                                 use filler orders only if this checkbox is active in the selected master organiza-
                                 tion.
                                  In the cutting area, the fillers are put onto any racks the number range of
                                 which is defined by Start Filler and End Filler. Each item is allocated to just one
                                 rack number.
                                  No fillers will be used.
                                 Technical info: database field: USEFUELLER

                                 Start of Filler This field refers to the range of rack numbers for the filler or-
                                 ders used. Enter the smallest rack number on which filler orders can be put.
                                 Technical info: database field: FUELLERSTART

                                 End of Filler This field refers to the range of rack numbers for the filler orders
                                 used. Enter the highest rack number on which filler orders can be put.
                                 Technical info: database field: FUELLERENDE

                                 Use Residue Plates This field refers to lites which belonged to resolved res-
                                 idue plates of previous detailed scheduling jobs.
                                  The selected master organization uses residue plates. In the cutting area,
3.00 / 01-2023




                                 the residue plates will be put onto any rack the number range of which is de-
                                 fined by Start Residue Plate and End Residue Plate. Every item is allocated
                                 just one rack number.


                 D-136                                                     A+W Production Detailed Scheduling
                 Software Reference                                                                      Organizations




                                         No residue plates will be used.
                                        Technical info: database field: USERESTBLATT

                                        Start of Residue Plate This field refers to the range of rack numbers for the
                                        residue plates used. Enter the smallest rack number on which residue plates
                                        can be put.
                                        Technical info: database field: RESTBLATTSTART

                                        End of Residue Plate This field refers to the range of rack numbers for the
                                        residue plates used. Enter the highest rack number on which residue plates
                                        can be put.
                                        Technical info: database field: RESTBLATTENDE

                                        Use Rejects This field refers to existing breakage.
                                         The selected master organization uses existing breakage. In the cutting ar-
                                        ea, the broken lites will be put onto any racks the number range of which is
                                        defined by Start of Rejects and End of Rejects. Every item is allocated just one
                                        rack number.
                                         No breakage will be used.
                                        Technical info: database field: USEBRUCH

                                        Start of Rejects This field refers to the range of rack numbers for the break-
                                        age used. Enter the smallest rack number on which breakage can be put.
                                        Technical info: database field: BRUCHSTART

                                        End of Rejects This field refers to the range of rack numbers for the break-
                                        age used. Enter the highest rack number on which breakage can be put.
                                        Technical info: database field: BRUCHENDE

                                        Use Rush Orders This field refers to existing rush orders.
                                         The selected master organization uses existing rush orders.
                                         No rush orders will be used.
                                        Technical info: database field: USEBRUCH


                                        Additional information
                                         Tutorial, “Master Organization” on page D-76
                                         Tutorial, “Special Elements” on page D-34
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-137
                 Organizations                                                            Software Reference




                                 Organization
                                 Master Data > Detailed Scheduling > Organization > tab Production Sequence
                                 > Select Organization > [Settings]




                                 Fig. D-55    Organization settings


                                 This dialog is used to define new organizations, or change existing ones. Fur-
                                 ther details are available in the corresponding fields.
                                 Technical info: database table: FEIN_ORGA

                                 Description of fields

                                 Name of Organization Type Enter the name of the organization.
                                 Technical info: database field: NAME

                                 Type Select the organization type from this combo box. Organization types
                                 are Standard, Rack, and all batch types in the system except cutting. You can
                                 select only batch types from this field which have been defined before! These
                                 are defined in dialog Batch types.
                                 Technical info: database field: LOSTYP

                                 Production The checkbox defines whether this is a production or application
                                 organization.
                                  This organization is a production organization
                                  This organization is an application organization.
                                 Technical info: database field: PRODUKTION

                                 Stacking Mode Use the radio buttons to set the default rack mode for A racks
                                 for this organization. These settings can be overridden at any time.
                                 The default value for the rack mode is Unit. Valid options:
                                 • Glass
                                 • Unit
                                 • Production
                                 • VABGLA
                                 Technical info: database field: BELEGUNGSMODE
3.00 / 01-2023




                 D-138                                                  A+W Production Detailed Scheduling
                 Software Reference                                                                          Organizations




                                        No splitting of … if rack contains more than … percent Valid options:
                                        Groups: If a group of lites is put on a rack but does not fit because of the rack
                                        depth, the group will not be split if the rack load is over X percent.
                                        Technical info: database field: USETIEFE_GRUPPE
                                        Units: If a group is split and part of it is put onto a rack, a unit could be split,
                                        theoretically. The unit will not be split if the rack load is over X per cent.
                                        Splitting a unit always necessitates to split a group; the value for groups should
                                        therefore always be bigger than that the entry for units.
                                        Technical info: database field: USETIEFE_EINHEIT


                                        Additional information
                                         Tutorial, “Organizations” on page D-73
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-139
                 Organizations                                                              Software Reference




                                 Organization Groups
                                 Master Data > Detailed Scheduling > Organization > tab Production Sequence
                                 > Organization Group > [Settings]




                                 Fig. D-56    Organization group settings


                                 Use this dialog to enter settings for existing or new organization groups. This
                                 means that you enter or change the name of the organization group, and allo-
                                 cate so-called groupings and/or sortings to the organization group. Further de-
                                 tails are available in the corresponding fields.
                                 Technical info: database table: FEIN_ORGAGRUPPE

                                 Description of fields

                                 Name Enter the name of the organization group.
                                 Technical info: database field: NAME

                                 DynOpt Settings This checkbox must be ticked if the organization group is
                                 meant for A+W DynOpt. This means that lites which are meant for A+W Dy-
                                 nOpt can be assigned only to an organization group with this code.
                                 Technical info: database field: DYNOPT

                                 Group Formation This field defines whether groups shall be created for the
                                 organization group in question. The combo box contains all defined groups
                                 from which you can select the required one. The groups are defined in master
                                 data.
                                 Select the required group from the combo box.
                                 Technical info: database field: GROUPINDEX

                                 Sorting of Groups The checkbox is related to field Group Formation and de-
                                 fines whether the selected group shall be sorted.
                                  The groups will be sorted.
                                  The groups will not be sorted.
                                 Technical info: database field: HASGSORT
3.00 / 01-2023




                 D-140                                                      A+W Production Detailed Scheduling
                 Software Reference                                                                     Organizations




                                        Sorting within Groups The combo box defines whether the groups selected
                                        in field Group Formation shall be sorted. The sorting options are:
                                        • None = The groups will not be sorted.
                                        • General = The default settings will be adopted.
                                        • Self-defined sorting
                                        Technical info: database field: SUBSORTINDEX

                                           Organization group settings
                                           Once the grouping and sorting of an organization group has been defined,
                                           you do not have to define grouping/sorting for the rack because this will be
                                           adopted from the organization group. Settings made for the rack will over-
                                           ride the grouping/sorting defined for the organization.


                                        Additional information
                                         Tutorial, “Organizations” on page D-73
                                         Tutorial, “Production Sequence” on page D-87
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-141
                 Organizations                                                             Software Reference




                                 Rack Settings
                                 Master Data > Detailed Scheduling > Organization > tab Production Sequence
                                 > Settings > tab [Application]




                                 Fig. D-57    Workstation settings


                                 This dialog allows allocating names and number ranges to racks. Please make
                                 sure that the names and number ranges match to the rack type (A rack, harp
                                 rack, etc.). Additionally, grouping, sorting, and rack modes can be allocated.
                                 Technical info: database table: FEIN_BOCKTYP

                                 Description of fields

                                 Name Enter the name of the rack type.
                                 Technical info: Compulsory field, alpha-numeric, 32-digit, database field:
                                 NAME

                                 Group Formation This field defines whether groups shall be created for the
                                 rack type in question. The combo box contains all defined groups from which
                                 you can select the required one. The groups are defined in master data. Select
                                 the required group from the combo box.
                                 Technical info: database field: GROUPINDEX

                                 Sorting within Groups The combo box defines whether the groups selected
                                 in field Group Formation shall be sorted. The sorting options are:
                                 • None = The groups will not be sorted.
                                 • General = The default settings will be adopted.
                                 • Self-defined sorting
                                 Technical info: database field: SUBSORTINDEX
3.00 / 01-2023




                 D-142                                                   A+W Production Detailed Scheduling
                 Software Reference                                                                        Organizations




                                        Check Inversion In the case of processings that are removed from the BOM
                                        within detailed scheduling via the lot type setting "Do not use", "Properties on-
                                        ly" or "Use sub-part", the responsible logical machine can be used to specify
                                        whether the sequence on A racks must be inverted by this processing step.
                                        In the number ranges for detailed scheduling, you can then specify whether
                                        the logical machine indicator should be used. If this is the case and there is an
                                        uneven number of processings between the step to be produced and the step
                                        used that have the above indicator, the sequence within the stacks is inverted
                                        on A racks. For this purpose, lites with different inversion behavior are placed
                                        on separate stacks.
                                        For cutting, this means that the break sequence is also adapted accordingly.
                                        Technical info: database field: INVERT_SEQUENCE

                                        Group Stacking Mode This field will be analyzed only if optimization mode
                                        6.1 or 5.1 is used. In this case, the combo box defines the stacking of groups.
                                        Select the required rack mode from the combo box. Valid options:
                                        • just 1 group per stack
                                        • complete groups together
                                        • fixed sequence
                                        • just 1 split group per stack
                                        • alternating
                                        Technical info: database field: BELEGMODE

                                        Optimization Behavior This combo box is related to field Group Formation.
                                        Please select the required optimization mode from the combo box. Options:
                                        • Free groups (6.1)
                                        • Groups sorted (6.2)
                                        • Everything free (5.1)

                                           Use Optimization Mode
                                           Optimization modes 6.1 and 6.2 will be used only if the grouping and sort-
                                           ing codes include the order number and the item number. If this is not the
                                           case, optimization mode 5.2 will be used.

                                        Reception Rack This checkbox defines the buffer rack. The selected recep-
                                        tion rack will collect all elements of a batch that cannot be allocated to another
                                        rack because they do not fulfil any condition required by the other racks.
                                         This rack is the buffer rack for the organization.
                                         This rack is not the buffer rack for the organization.
                                        Technical info: database field: AUFFAENGER

                                        From/To: For each rack type, enter at least one range of numbers that can
                                        be used for this rack type. Application rack types can even have two number
                                        ranges if production racks are assigned as well. Number ranges must not
                                        overlap in an organization or master organization (the program will prevent this
                                        and will issue error reports to that effect). Master organizations can even in-
                                        clude additional number ranges for specialities (rejects, fillers, residue).
3.00 / 01-2023




                                        Technical info: database field: MINIMUM
                                        Technical info: database field: MAXIMUM



                 A+W Production Detailed Scheduling                                                               D-143
                 Organizations                                                              Software Reference




                                 Maximum No. of Groups This field refers to the maximum number of groups
                                 that can be put on this rack. If any number of groups can be put onto the rack,
                                 enter 0.
                                 Technical info: database field: MAXNUMBER

                                 Separate Next Step If this checkbox is active, the batch formation of the next
                                 step will be taken into account for A racks, checking what can be stacked to-
                                 gether.

                                 Stacking Mode The listed values refer to the field Rack Type. If the radio but-
                                 ton A rack is ticked in field Rack Type, the following options appear:
                                 • Global: The mode defined for this organization will be used.
                                 • Glass: Each glass type gets its own number and is put onto a separate
                                      rack.
                                 • Unit: Lites that belong to the same unit (laminated glass, IG) will be put onto
                                      the same rack, with a common rack number. Different glass types will be
                                      automatically separated by the system and will be put onto separate, ad-
                                      joining stacks.
                                 • Production: Several glass types are put together on a rack in separate
                                      stacks per glass type. These stacks can be used for producing different
                                      products/combinations.
                                 • VAGBLA: For every glass type, there is a logical rack with just one stack.
                                      Unlike in case of the Glass mode, the groups will be split when the maxi-
                                      mum rack load has been reached. For details please refer to the description
                                      of modes in the tutorial.
                                 If the radio button Harp Rack is ticked in field Rack Types, the options are:
                                 • Together: Lite and counter lite(s) will always be put together onto a harp
                                      rack.
                                 • Glass: The lites will always be stacked separately.
                                 • Compact: Only lites with a common flag are put on a harp rack. Depeding
                                      on the configuration, this flag can be the fields XOPT_TISCH.CUTGO or
                                      POOL_TEILE.SONDERKZ3.
                                 If the radio button Fixed racks has been ticked in field Rack Types, section
                                 Stacking Mode is disabled.
                                 Technical info: database field: BELEGMODE
3.00 / 01-2023




                 D-144                                                    A+W Production Detailed Scheduling
                 Software Reference                                                                       Organizations




                                        Rack Type The radio buttons define the rack type. Valid options:
                                        • A Racks
                                        • Harp racks
                                        • Fixed Racks
                                        The combo box below always refers to the active rack type. If there are several
                                        types of A racks for instance, these will be listed in the combo box.
                                        Technical info: database field: TYPE

                                        Description of buttons

                                        Racks Use this button to open the dialog Racks.


                                        Additional information
                                         Tutorial, “Racks” on page D-42
                                         Tutorial, “Grouping Key for Organization Groups” on page D-88
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-145
                 Organizations                                                                Software Reference




                                 Default Settings
                                 Master Data > Detailed Scheduling > Presettings




                                 Fig. D-58    Presettings


                                 These settings will be used if no entries are made for the organization, for
                                 grouping and sorting for the organization, and sorting on the rack. We recom-
                                 mend to define settings at this point lest an error message should appear
                                 when detailed scheduling is started.

                                 Description of fields

                                 Processing Sequence This combo box allows to select a sorting. Sorting is
                                 defined in master data and controls the criteria used for the processing of lites.

                                 Organization This combo box allows to select a master organization. Master
                                 organizations are defined in master data and determine the master organiza-
                                 tion used for detailed scheduling.

                                 Group Formation This combo box allows to select a grouping. Groupings
                                 are defined in master data and determine the criteria for group formation.

                                 Sorting to Rack This combo box allows to select a sorting. Sortings are de-
                                 fined in master data and control the sorting criteria for lites.


                                 Additional information
                                  Tutorial, “Global settings” on page D-85
3.00 / 01-2023




                 D-146                                                        A+W Production Detailed Scheduling
                 Software Reference                                                               Grouping and Sorting




                                        Grouping and Sorting
                                        The settings made in section Grouping/Sorting shall be used for grouping and
                                        sorting the lites on the racks. The lites will be collected in Groups, and sorted
                                        within the groups. The sequence of groups can be defined as well.


                                        Grouping/Sorting Dialog
                                        The dialog consists of three tabs:
                                        •   Tab Editor - Grouping
                                        •   Tab Editor - Sorting
                                        •   Tab Additional Sorting


                                        Additional information
                                         Tutorial, “Grouping and Sorting” on page D-26


                                        Tab Editor - Grouping
                                        Master Data > Detailed Scheduling > Grouping > tab Editor - Grouping




                                        Fig. D-59     Grouping/Sorting dialog, tab Grouping


                                        This dialog is used to define new groups, or change existing ones. The entries
                                        on tab Editor - grouping will be used in the following areas:
                                        •   Software Reference, “Rack Settings” on page D-142
                                        •   Software Reference, “Organization Groups” on page D-140
                                        •   Software Reference, “Master Organization” on page D-134
                                        •   Software Reference, “Default Settings” on page D-146
                                        Technical info: database table: SORTING
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                               D-147
                 Grouping and Sorting                                                                Software Reference




                                        Description of fields

                                        Left Window This window shows all defined groups or sortings. The individ-
                                        ual groups/sortings are arranged in a tree structure; their characteristics can
                                        be displayed by opening the tree structure. Example: Group +Article num-
                                        ber+Stacking width includes the properties Article number and Stacking width.
                                        The plus or minus sign in front of the properties shows the direction in which
                                        this property is sorted. Example: +Article number means that the article num-
                                        bers are sorted in ascending order. -Article number means that the article
                                        numbers are sorted in descending order.

                                        Fields in section Sorting direction

                                        Ascending This field is active only if a property of the group/sorting is select-
                                        ed. Tick the radio button Ascending to sort the selected property in ascending
                                        order. This is marked by the plus sign in front of the property.

                                        Descending This field is active only if a property of the group/sorting is se-
                                        lected. Tick the radio button Descending to sort the selected property in de-
                                        scending order. This is marked by the minus sign in front of the property.

                                        Description of buttons in section Sorting Direction

                                        Delete Use this button to delete the selected group/sorting property, or to de-
                                        lete the entire group/sorting. This depends on which entry has been selected.
                                        When a property of the group/sorting is selected, only this property will be de-
                                        leted. When a group/sorting is selected however, the entire group/sorting will
                                        be deleted.

                                        Add This button refers to the right window. The property or formula selected
                                        in the right window can be added by using the [Add] button, either as a whole
                                        group/sorting, or as a property in the group/sorting. This depends on the se-
                                        lected entry. When a group/sorting is selected, the property or formula will be
                                        added to the selected group/sorting. If you select the top entry on the left list
                                        (on tab Editor - Grouping, this is the entry Grouping and on tab Editor - Sorting,
                                        this is the entry Sorting), a new group/sorting will be created.

                                        Description of radio buttons

                                        Property If the radio button Property is ticked, the right window shows all ex-
                                        isting properties.

                                        Formula If the radio button Formula is ticked, the right window shows all ex-
                                        isting formulas.
3.00 / 01-2023




                 D-148                                                           A+W Production Detailed Scheduling
                 Software Reference                                                            Grouping and Sorting




                                        Description of the button

                                        Formulas … Use this button to open the dialog Select formulas --1--. You can
                                        change an existing formula or define a new one. For more information please
                                        refer to the documentation on Formula editor.


                                        Additional information
                                         Tutorial, “Grouping and Sorting” on page D-26
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                          D-149
                 Grouping and Sorting                                                              Software Reference




                                        Tab Editor - Sorting
                                        Master Data > Detailed Scheduling > Grouping > tab Editor - Sorting




                                        Fig. D-60    Grouping/Sorting dialog, tab Sorting


                                        This dialog is used to define new sortings, or change existing ones.
                                        Apart from the button below, the contents of tab Editor - Sorting is the same as
                                        the contents of tab Editor - Grouping and will therefore not be described in de-
                                        tail at this point. For details please refer to the tab Editor - Grouping.
                                        Technical info: database table: SORTING

                                        Description of the button

                                        Additional Sorting Use this button to open the dialog Additional Sorting for
                                        the selected sorting.


                                        Additional information
                                         Tutorial, “Grouping and Sorting” on page D-26
3.00 / 01-2023




                 D-150                                                            A+W Production Detailed Scheduling
                 Software Reference                                                                     Grouping and Sorting




                                        Tab Additional Sorting
                                        Master Data > Detailed Scheduling > Grouping > tab Additional Sorting




                                        Fig. D-61     Grouping/Sorting dialog, tab Additional sorting


                                        This dialog shows all additional sortings. Additional sortings are defined in di-
                                        alog Define Additional Sorting.
                                        Technical info: database table:

                                        Description of fields

                                        Key Column Key shows the key for which the additional sorting is used.

                                        Value This field shows the value for the additional sorting.

                                        Additional Sorting The field shows the complete sorting this key has an ef-
                                        fect on.


                                        Additional information
                                         Tutorial, “Additional sorting” on page D-33
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-151
                 Grouping and Sorting                                                              Software Reference




                                        Defining an Additional Sorting
                                        Master Data > Detailed Scheduling > Grouping > tab Editor - Sorting > [Addi-
                                        tional Sorting]




                                        Fig. D-62     Define additional sorting


                                        Sortings can be completed by additional sortings. You only need to define an
                                        additional sorting to which the combination of sorting key/value is allocated. If
                                        a sorting ends with the defined sorting key, the group all elements of which
                                        match the defined sorting key, will be sorted into more groups.
                                        Example: The items on a rack are sorted by ROUTE+CUSTOMERNUMBER+.
                                        If there is an additional sorting SMALLSIZE+ for CUSTOMERNUMBER=4711,
                                        the extended sorting will be only applied to customer number 4711. For all oth-
                                        er customers, the sequence does not matter. You can of course allocate differ-
                                        ent additional sortings to different customers.
                                        Technical info: database table: MORESORTING

                                        Description of fields

                                        Value Enter the name of the additional sorting. The radio buttons Number,
                                        thickness, text, length, and airspace define the value. Additional sortings are
                                        shown on tab Additional Sorting.

                                        Description of the button

                                        No Value Check Press this button to use the additional sorting, notwithstand-
                                        ing the last sorting key.


                                        Additional information
                                         Tutorial, “Additional sorting” on page D-33
3.00 / 01-2023




                 D-152                                                             A+W Production Detailed Scheduling
                 Software Reference                                                                               Racks




                                        Racks
                                        The dialog consists of three sections:
                                        •   A Racks
                                        •   Harp racks
                                        •   Fixed Racks


                                        Racks
                                        Master Data > Detailed Scheduling > Racks
                                        Master Data > Detailed Scheduling > Organization > tab Production Sequence
                                        > Select Rack for the Organization Group > button [Settings]




                                        Fig. D-63     Racks


                                        Use this dialog to define the racks existing in your production, or to change the
                                        defined racks. The defined racks are used in the following detailed scheduling
                                        areas:
                                        •   Software Reference, “Rack Settings” on page D-142
                                        •   Software Reference, “Tab Organization” on page D-189
                                        Technical info: database table: ABSTELLPLATZ
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                               D-153
                 Racks                                                               Software Reference




                         Description of the fields in section A racks

                         Combo Box The combo box below the buttons [Add], [Delete] and [Rename]
                         shows the names of the racks defined for the A racks in the system.

                         Stacking Depth Enter the rack depth in mm. 1200 mm means that the stack
                         can be up to 1200 mm deep. Please note that rack depths over 20 m will au-
                         tomatically be treated like unlimited rack depths.
                         Technical info: database field: TIEFE

                         Width This field defines the total width of the rack in mm. 2000 mm for exam-
                         ple means that lites can be stacked on the rack up to a width of 2000 mm.
                         Technical info: database field: BREITE

                         Max. Stacks/Rack Enter the number of available slots per rack. Valid op-
                         tions:
                         • 1 = one stack per rack
                         • 2 = there are two stacks per rack
                         • 4 = there are four stacks per rack
                         Technical info: database field: MAXCOUNT

                         L Rack Tick this checkbox if the rack is an L rack (instead of an A rack).

                         Robot Tick this checkbox if the A rack is a robot rack. Robot racks are racks
                         controlled by a robot. Valid options:
                         • 0 = no robot rack
                         • 1 = single = robot rack, single
                         • 2 = reflected = robot rack, reflected
                         • 3 = double = robot rack, exists twice, both racks can be controlled sepa-
                            rately
                         Technical info: database field: ROBOT

                         Quantity This field is active only if the A rack is a robot rack. You can define
                         the number of robot racks existing in your production. Also, you can enter
                         whether these racks exist once or twice, or whether the robot racks actually
                         exist twice, but the system decides which one will be used. The rack with the
                         given number from the first or second quantity.

                         Max. No. of A Racks The maximum number of A racks is important for cre-
                         ating optimization groups. When a glass type reaches the maximum quantity
                         allowed, the current optimization group will be closed for all optimizations, and
                         a new one will be started. This can be cut once the racks are empty.

                         Check Quantity (Cutting) The checkbox refers to the entry in field Max. No.
                         of A Racks and checks this if necessary.

                         Sortjet If a Sortjet is being used, please tick this checkbox.
3.00 / 01-2023




                         Technical info: database field: SORTJET




                 D-154                                            A+W Production Detailed Scheduling
                 Software Reference                                                                              Racks




                                        Maximum Weight (kgs) Maximum weight of all lites on the A rack. When this
                                        weight is reached, a new rack will be started. 0 means that there is no weight
                                        limit.
                                        Technical info: database field: GEWICHT

                                        ID for Stack Opti If you are working with the Stack Optimizer, enter the ID of
                                        the physical rack. The possible values will be retrieved from the configuration
                                        files of the Stack Optimizer.
                                        Technical info: database field: STACK_ID

                                        Description of fields in section Harp Racks

                                        Combo Box The combo box below the buttons [Add], [Delete] and [Rename]
                                        shows the names of the harp racks defined.

                                        Number of Slots This field defines the number of slots on the rack. If there is
                                        one slot per number, the number of slot numbers matches the number of slots
                                        on the rack.
                                        Technical info: database field: FACHANZAHL

                                        Width This field defines the width of the slots.
                                        Technical info: database field: BREITE

                                        Two Slots/Number This checkbox defines whether two lites each shall get a
                                        common slot number. In this case, there are twice as many slots than there are
                                        slot numbers. This means that two lites can be put into the same slot.
                                        Technical info: database field: FACH_PRO_NR

                                        Start = 0 The checkbox defines whether the slot numbers will be counted
                                        from 0, or from 1
                                         The slot numbers will be counted from 0.
                                         The slot numbers will be counted from 1 (default).
                                        Technical info: database field: STARTFACH

                                        Slot Number Digits This radio button defines the number of digits of the rack
                                        number to be reserved for slot numbers.
                                        • 2 means that the last two digits are reserved.
                                        • 3 means that the last three digits are reserved.
                                        • 4 means that the last four digits are reserved.
                                        With 50 slot numbers, this will be 2 digits, starting from 100 slot numbers, 3
                                        digits, etc.
                                        Technical info: database field: DIGITSFACH

                                        Max. Number of Harp Racks The maximum number of harp racks is essen-
                                        tial for the creation of optimization groups. When a glass type reaches the
                                        maximum quantity, the current optimization group will be closed for all optimi-
                                        zations, and a new one will be started. This can be cut once the racks are emp-
3.00 / 01-2023




                                        ty.




                 A+W Production Detailed Scheduling                                                             D-155
                 Racks                                                                 Software Reference




                         Check Quantity (Cutting) The checkbox refers to the value in field Max.
                         Number of Harp Racks and checks this if necessary.
                          The value in field Max. Number of Harp Racks will be checked. An error
                         message appears if this is exceeded. In this case, detailed scheduling can nei-
                         ther be optimized, nor saved.
                          There will be no quantity check.

                         Sortjet If a Sortjet is being used, please tick this checkbox.
                         Technical info: database field: SORTJET

                         Maximum Load (kg) Maximum weight of all lites on the harp rack. When this
                         weight is reached, a new rack will be started. 0 means that there is no weight
                         limit. If you enter 0, the number of lites to be put onto the harp rack will be lim-
                         ited only by the number of slots.
                         Technical info: database field: GEWICHT

                         Empty Weight (kg) Empty weight of rack in kilogram.
                         Technical info: database field: LEERGEWICHT

                         Distance First/Last Slot from Axis Distance between outer edge and axis
                         (left/right).
                         Technical info: database field: ABSTAND_FACH_ACHSE

                         Max. Deviation Center of Gravity fr. Middle (%) Permitted deviation
                         fromcenter of gravity from middle in percent (+/-).
                         Technical info: database field: ABWEICHUNG_SP

                         Description of the fields in section Fixed Racks

                         Combo Box The combo box below the buttons [Add], [Delete] and [Rename]
                         shows the names of the fixed racks defined.

                         Stacking Depth Enter the rack depth in mm. Example: 1200 mm means that
                         the stack can be up to 1200 mm deep. Please note that rack depths over 20
                         m will automatically be treated like unlimited rack depths.
                         Technical info: database field: TIEFE

                         Width This field defines the total width of the rack in mm. 2000 mm for exam-
                         ple means that lites can be stacked on the rack up to a width of 2000 mm.
                         Technical info: database field: BREITE

                         Max. No. of Fixed Racks The maximum number of fixed racks is essential
                         for the creation of optimization groups. When a glass type reaches the maxi-
                         mum quantity, the current optimization group will be closed for all optimiza-
                         tions, and a new one will be started. This can be cut once the racks are empty.
3.00 / 01-2023




                 D-156                                             A+W Production Detailed Scheduling
                 Software Reference                                                                            Racks




                                        Check Quantity (Cutting) The checkbox refers to the value in field Max.
                                        Number of Fixed Racks and checks this if necessary.
                                         Checks the value in field Fixed Racks. An error message appears if this is
                                        exceeded. In this case, the detailed scheduling job can neither be optimized,
                                        nor saved.
                                         There will be no quantity check.

                                        Maximum Weight (kgs) Maximum weight of all lites on the fixed rack. When
                                        this weight is reached, a new rack will be started. 0 means that there is no
                                        weight limit.
                                        Technical info: database field: GEWICHT


                                        Additional information
                                         Tutorial, “Racks” on page D-42
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                           D-157
                 Lots                                                               Software Reference




                         Lots
                         Dialog Lot types and processings serves to make the settings for the lot cre-
                         ation for a lot type. Processing or related processing will then be allocated to
                         the lot type.


                         Lot Types and Processings
                         The dialog consists of three tabs:
                         •   Tab Lot Types
                         •   Tab Processings
                         •   Tab Implicit Processing


                         Tab Lot Types
                         Master Data > Detailed Scheduling > Lot Types




                         Fig. D-64    Lot types and processings, tab Lot types


                         Use this dialog to define new lot types, or change existing ones.
                         Technical info: database table: FEIN_LOSTYP
3.00 / 01-2023




                 D-158                                            A+W Production Detailed Scheduling
                 Software Reference                                                                                   Lots




                                        Description of fields

                                        Lot Type/Name The view shows all defined lot types including lot type num-
                                        bers and names. Detailed scheduling saves the lot type number in the data-
                                        base. The lot type name is used in the detailed scheduling views.

                                        Name/Type/Procurement The view shows all combinations of Processing
                                        Type and Procurement allocated to this lot type. Double-click on an entry to
                                        switch to the appropriate page in the dialog, and view the processing. An as-
                                        terisk (*) behind an entry in column Type marks a related processing.

                                        Lot Type(-number) The lot type number must be equal or bigger than 100,
                                        and also the multiple of 10. The reason for this is that for application lots, the
                                        lot number is raised by one, and saved in the database. Detailed scheduling
                                        will also save the lot type number in the database.
                                        Technical info: database field: LOSTYP

                                        Name This field shows the lot type name used in the detailed scheduling
                                        views.
                                        Technical info: database field: NAME

                                        Grouping The combo box contains all defined groups. This group can be
                                        used to distribute lites of the same lot type to different production lots. Without
                                        such a group, lots will be created only for real machines. When a group is de-
                                        fined, the production lots for IG e.g. can be assembled according to airspace.
                                        The group key only has to include the element airspace. An important excep-
                                        tion is cutting. For cutting purposes, lots are always assembled by glass type,
                                        glass thickness, and real tables. The groups are defined in master data.
                                        Technical info: database field: GRUPPIERUNG

                                           Grouping
                                           Groups can be used to form production lots. Application lots will be created
                                           by lots type only.

                                        Technology Type The combo box shows all defined machine types. The ma-
                                        chine type comes from machinery allocation. The machine type can be 0 if
                                        none has been allocated.
                                        Technical info: database field: TECHNOTYP
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                D-159
                 Lots                                                                Software Reference




                         Production Sequence The combo box shows all defined groupings. For re-
                         lated processing steps, the production sequence of the original processing will
                         be used as a rule. You can use the Production Sequence to define an individ-
                         ual sequence. Should the set production sequence allow freedom with regards
                         to the sequence, the direct or reversed sequence of the original processing will
                         be used, depending on the checkbox Reverse Sorting.
                         Technical info: database field: PROD_RF

                         Reverse Sorting This checkbox is active only if the combo box Production
                         Sequence shows the entry (unequal None). See explanation:
                         Technical info: database field: INVERT_RF

                         Behavior in Detailed Scheduling Except for Use sub-element, this setting
                         is currently used only for processing, not for the elements themselves. Valid
                         options:
                         • Standard: Lots and racks will be created and allocated to this processing.
                         • Use child part: There is no direct lot creation or rack allocation for this pro-
                             cessing or element. Instead, the same batch number, rack numbers and
                             sequences will be used as for the child element. Please note that this pro-
                             cess is not valid for all elements. The element must not be cutting; there
                             must be just one sub-element, and it must not belong to a rack optimization.
                             Also, sub-element and element must belong to the same batch.
                         • Properties only: In this case, there will be no lot creation or rack allocation
                             for the processing. The processing and all its properties are available for
                             rack allocation in connection with the organization. In this case, racks can
                             be allocated after the first processing, after cutting.

                             Processing will be removed from the element tree
                             The processing will be removed from the element tree right after rack allo-
                             cation. Grouping and sorting on the racks can no longer refer to this. This
                             can be avoided by using a trick. The required processing property can be
                             allocated to the lite by assigning an otherwise not required property.

                         •  Not used: This processing will not be added to the element tree, and is thus
                            not available for rack allocation. Naturally, there is no lot creation or rack
                            allocation in this case.
                         Please note that lots for related processing which are arranged below the orig-
                         inal processing do not only use their own group key but also depend on the lot
                         creation for the elements.
                         Technical info: database field: FEINPLANUNG_KZ


                         Additional information
                          Tutorial, “Lots” on page D-19
3.00 / 01-2023




                 D-160                                            A+W Production Detailed Scheduling
                 Software Reference                                                                              Lots




                                        Tab Processings
                                        Master Data > Detailed Scheduling > Processings




                                        Fig. D-65     Lot types and processing, tab Processing


                                        Use this dialog to define new processings, or change existing ones. The pro-
                                        cessing is specified by its name, its element or processing type, its supply
                                        type, and the allocated lot type. When detailed scheduling is started and the
                                        system finds no master data entry for a combination of processing type/pro-
                                        curement, this dialog will automatically be loaded so that you can enter the
                                        missing processing. Detailed scheduling can be recommenced immediately.
                                        Technical info: database table: FEIN_BEARBTYP

                                        Description of fields

                                        Name This field shows the processing name. This name will be used only in
                                        the other tabs of this dialog, and does not reappear in detailed scheduling.
                                        Technical info: database field: NAME

                                        Type Combo box Type shows all existing processing types. The processing
                                        types are loaded from master data.
                                        Technical info: database field: BEARBTYP

                                        Procurement Select the appropriate procurement type for the processing
                                        from the combo box. Valid options:
                                        • 0 = Production
                                        • 1 = Cutting
                                        • 2 = Stock withdrawal
3.00 / 01-2023




                                        • 9 = Ordered
                                        Technical info: database field: BESCHAFFUNGSART




                 A+W Production Detailed Scheduling                                                           D-161
                 Lots                                                              Software Reference




                         Lot Type The combo box refers to the lot types defined on tab Lot Type. Se-
                         lect the required lot type from the combo box. Please note that only processing
                         steps of the procurement type Cutting must be allocated to lot type number
                         100.
                         Technical info: database field: LOSTYP

                         Article Number for Missing Processing Import will use this product num-
                         ber for processing whenever this is needed, and exists nowhere else in the
                         system.
                         Technical info: database field: ARTIKEL
3.00 / 01-2023




                 D-162                                           A+W Production Detailed Scheduling
                 Software Reference                                                                               Lots




                                        Tab Implicit Processing
                                        Master Data > Detailed Scheduling > Processing > tab Implicit Processing




                                        Fig. D-66     Lot types and processing, tab Implicit processing


                                        Tab Implicit Processing can be used to automatically define further processing
                                        steps, to be added to the element tree. These implicit processings are speci-
                                        fied by the attributes Name (only for display in this dialog), Type (processing
                                        type as per table BEARB_TYP), the allocated Lot type, and the code Creation.

                                        Description of fields

                                        Name This field shows the name of the implicit processing.
                                        Technical info: database field: NAME

                                        Type The (processing) type must be defined so that the processing is not un-
                                        necessarily created should it be transferred from order entry to A+W Produc-
                                        tion so that the processing step would exist twice.
                                        Technical info: database field: BEARBTYP

                                        Lot Type Select the existing lot types from this combo box. The lot types are
                                        loaded from tab Lot Types.
                                        Technical info: database field: LOSTYP
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-163
                 Lots                                                              Software Reference




                         Definition This field defines under which circumstances the processing is
                         created. Valid options:
                         • Always
                         • Header parts
                         • Non-header parts
                         The processing step can be created always, only for main elements, or for el-
                         ements other than main elements. The implicit processing Despatch for exam-
                         ple could be created for all elements; this would make sense only for main
                         elements of course so that you will need to select Header parts.
                         Technical info: database field: ERZEUGUNG

                         The selected processing creates the following, implicit processing This
                         table lists the existing implicit processing steps for the selected processing.


                         Additional information
                          Tutorial, “Lots” on page D-19
3.00 / 01-2023




                 D-164                                           A+W Production Detailed Scheduling
                 Software Reference                                                    Detailed Scheduling of Batches




                                        Detailed Scheduling of Batch-
                                        es
                                        For batches shown in the batch view as roughly scheduled, detailed schedul-
                                        ing can be started by means of the context menu. Detailed scheduling runs in
                                        the background which means that you can go on working meanwhile. When
                                        detailed scheduling is terminated, a dialog appears Detailed Scheduling for
                                        Batch …


                                        Detailed Scheduling for Batch …
                                        The dialog is split into the following tabs:
                                        •   “Tab Glass Types” on page D-166
                                        •   “Tab Rack Allocation” on page D-169
                                        •   “Tab Results” on page D-174
                                        •   “Tab Specials” on page D-176
                                            – “Tab Nested Shapes” on page D-176
                                            – “Tab Filler Orders” on page D-178
                                            – “Tab Residue Plates” on page D-180
                                            – “Tab Rejects” on page D-181
                                            – “Tab Rush Order Lites” on page D-183
                                            – “Tab Thickness” on page D-184
                                        •   “Tab Free Optimization” on page D-186
                                        •   “Tab Organization” on page D-189
                                        •   “Tab Organization Options” on page D-191
                                        •   “Tab Options” on page D-193
                                        •   “Tab Stockplate Selection” on page D-195
                                        The individual tabs give a complete overview of all parameters used for de-
                                        tailed scheduling (cutting type, racks, stock sizes, etc.). The displayed param-
                                        eters can be changed in the corresponding tabs. Detailed scheduling has to
                                        be run once more. This should be done carefully, however!
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                             D-165
                 Detailed Scheduling of Batches                                                            Software Reference




                                         Tab Glass Types
                                         View > Batch View > Select Batch > Context menu detailed scheduling > tab
                                         Glass Types




                                         Fig. D-67       Detailed scheduling for one batch, tab Glass types


                                         The tab Glass Types refers to the glass types in this batch. It provides infor-
                                         mation on the thickness, the optimization, the surface to be produced, and the
                                         quantity to be produced. Select an item from the top section to view informa-
                                         tion on the counterpane in the bottom section. This applies only to lites which
                                         have counterpanes in the same batch.
                                         The symbols give a quick overview of the cutting type.
                                         The symbols in the two sections have the following meanings:

                                         Top section:
                                                  Automatic Cutting
                                                  Manual cutting
                                                  Manual cutting and cutting plan
                                         Counterpane section:
                                                  Automatic Cutting
                                                  Manual cutting

                                         Fig. D-68       Explanation of the detailed scheduling symbols for the individual batches
3.00 / 01-2023




                 D-166                                                                 A+W Production Detailed Scheduling
                 Software Reference                                                        Detailed Scheduling of Batches




                                        Description of the fields in the top section
                                        The fields in the top section provide information on:
                                        •   Glass type: Shows the article number of the glass type. Glass types are de-
                                            fined in master data.
                                        •   Thickness: This field shows the thickness of the glass type. The thickness
                                            is defined in master data.
                                        •   Optimization: This field shows the optimization type. The optimizations are
                                            fixed in the system and cannot be changed.
                                        •   Surface (B): This field shows the optimization surface in sqm.
                                        •   Qty (B): This field shows the quantity. * after the quantity means that you
                                            can use filler orders for this optimization.

                                        Description of buttons

                                        Up This button allows to define the optimization priority, i. e. the sequence in
                                        which the optimization shall be run. Use this button to move the selected re-
                                        cord one position up on the list.

                                        Down This button allows to define the optimization priority, i. e. the sequence
                                        in which the optimization shall be run. Use this button to move the selected re-
                                        cord one position down on the list.

                                        Manual Cutting Use this button to change the cutting type for the selected
                                        record from automatic to manual, or vice versa. This means that if the record
                                        is set to automatic cutting, it will be set to manual cutting; if it was set to manual
                                        cutting, it will be changed to automatic cutting.

                                        XOPT This button will appear if the selected lite is to be cut automatically. It
                                        will not appear if the selected lite shall be cut manually. Use this buttons to
                                        force or delete an XOPT optimization for elements that are not stacked on harp
                                        racks.

                                        Cutting Plan This button will appear if the selected lite is to be cut manually.
                                        It will not appear if the selected lite shall be cut automatically. This means that
                                        an optimization will be started for this lite although it will be cut manually. A cut-
                                        ting plan will be created for this optimization.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                   D-167
                 Detailed Scheduling of Batches                                                     Software Reference




                                         Description of the fields in section Counterpane Information
                                         This section contains information on the counterpane of the lite selected in the
                                         upper section:
                                         •   Glass type: Shows the article number of the glass type. Glass types are de-
                                             fined in master data.
                                         •   Thickness: This field shows the thickness of the glass type. The thickness
                                             is defined in master data.
                                         •   Optimization: This field shows the optimization type. The optimizations are
                                             fixed in the system and cannot be changed.
                                         •   Surface (B): This field shows the optimization surface in sqm. The system
                                             will automatically calculate the surface.
                                         •   Qty (B): This field shows the quantity to be optimized. The quantity will be
                                             imported from the order processing system.

                                         Description of buttons

                                         Double Optimization Use this button to create a double optimization for the
                                         item selected in the counterpane section.

                                         Remove This button is valid only for items for which a double optimization
                                         was created. In this case, the button allows to remove the double optimization.

                                         Repeat This button is active only if you have changed the detailed scheduling
                                         results. Whenever you have made changes, you have to repeat detailed
                                         scheduling to apply these changes.

                                         Optimization If the detailed scheduling for this batch is acceptable, use this
                                         button to start the optimization. When the optimization is completed, tab Re-
                                         sults will open automatically.

                                         PlanEdit After optimization you can use this button to view the cutting plan.
                                         Program Plan Editor is started.
3.00 / 01-2023




                 D-168                                                            A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Tab Rack Allocation
                                        View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                        Rack Allocation




                                        Fig. D-69     Detailed scheduling for one batch, tab Rack allocation


                                        This tab provides a detailed list of the racks required for this batch. This is the
                                        result of the rack settings you have made in tab Production Sequence in the
                                        Organization Dialog.
                                        The left section shows the individual racks in a tree structure. Click on the plus
                                        sign in front of a rack to open it so that you can see which rack numbers are
                                        used.
                                        The meaning of the symbols:

                                        Icon          Explanation

                                                      Rack load

                                                      A Racks

                                                      Harp racks

                                        Tab. D-8      Explanation of the systems in tab Rack allocation
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-169
                 Detailed Scheduling of Batches                                                        Software Reference




                                         Description of fields

                                         List on the left The list on the left side provides information on:
                                         • Glass Type: This field shows all glass type/thickness combinations for this
                                            batch. Example: 1306/6.0 means that the glass type has the product num-
                                            ber 1306, and a thickness of 6.0 mm. Glass types are defined in master da-
                                            ta.
                                         • Min. Stack No.: This field shows the minimum number of stacks. You can
                                            edit this number by double-clicking on it. The dialog Change Minimum
                                            Number of A Racks opens.
                                             Should you have made any changes, you will need to repeat detailed
                                             scheduling!
                                         •   Stack No.: This field shows the actually required number of stacks.
                                         •   Harp Rack No.: This field shows the actually required number of harp
                                             racks.
                                         The display in the right section of the dialog is based on what has been select-
                                         ed in the left section. When you select the top entry (rack load), the right sec-
                                         tion shows all glass type/thickness combinations of this batch.
                                         When you select the condition for the lites on an A rack on the left, the display
                                         looks as follows:




                                         Fig. D-70    Detailed scheduling for one batch, tab Rack allocation, A rack


                                         You will see the rack number, the stack number containing the lites, and the
                                         depth and width of the stack in mm.
3.00 / 01-2023




                 D-170                                                             A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Description of fields

                                        Rack No. Shows the rack number. The rack number area is loaded from mas-
                                        ter data.

                                        Stack No. This field is active only for A racks. This field shows the stack num-
                                        ber containing the lites.

                                        Depth Shows the depth of the stack (in mm).

                                        Width Shows the width of the stack (in mm).
                                        When you open in the left section the name of an A rack in the tree structure
                                        by clicking on the plus sign, you will see the rack number below. When you se-
                                        lect the rack number, the display looks as follows:




                                        Fig. D-71     Detailed scheduling for one batch, tab Rack allocation, A rack


                                        You can see how many lites of a glass type/thickness combination are stacked
                                        on a rack, and how deep and wide the stack is.

                                        Description of fields

                                        Glass Type This field shows all glass type/thickness combinations on this
                                        rack. Example: 1306/6.0 means that the glass type on this rack has the prod-
                                        uct number 1306, and a thickness of 6.0 mm. Glass types are defined in mas-
                                        ter data.

                                        Lites How many lites of this glass type/thickness combination does this rack
3.00 / 01-2023




                                        hold.




                 A+W Production Detailed Scheduling                                                                    D-171
                 Detailed Scheduling of Batches                                                        Software Reference




                                         Depth How deep (in mm) have the lites of this glass type/thickness combina-
                                         tion been stacked on this rack.

                                         Width How wide (in mm) have the lites of this glass type/thickness combina-
                                         tion been stacked on this rack.
                                         When you select the name for the lites of a harp rack on the left, the display
                                         looks as follows:




                                         Fig. D-72    Detailed scheduling for one batch, tab Rack allocation, Harp rack


                                         You will see the rack number, the stack number containing the lites, and the
                                         depth and width of the stack in mm.

                                         Description of fields

                                         Rack No. Shows the rack number. The rack number area is loaded from mas-
                                         ter data.

                                         Occupied Slots This field shows the number of occupied slots on this rack.
3.00 / 01-2023




                 D-172                                                             A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Number of Glass Types This field shows the number of different glass types
                                        on the harp rack.
                                        When you open in the left section the name of a harp rack in the tree structure
                                        by clicking on the plus sign, you will see the rack number below. When you se-
                                        lect the rack number, the display looks as follows:




                                        Fig. D-73     Detailed scheduling for one batch, tab Rack allocation, Harp rack


                                        You can see how many lites of a glass type/thickness combination are stacked
                                        on a rack.

                                        Description of fields

                                        List on the left The list on the left side shows the racks used for this batch,
                                        and the valid conditions.

                                        List on the right The list on the right provides information on:
                                        • Glass Type: This field shows all glass type/thickness combinations on this
                                           rack. Example: 1306/6.0 means that the glass type on this rack has the
                                           product number 1306, and a thickness of 6.0 mm. Glass types are defined
                                           in master data.
                                        • Thickness: This field shows the lite thickness. The thickness is defined in
                                           master data.
                                        • Lites: You can see how many lites of a glass type/thickness combination
                                           have been loaded onto the rack.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-173
                 Detailed Scheduling of Batches                                                        Software Reference




                                         Tab Results
                                         View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                         Results




                                         Fig. D-74    Detailed scheduling for one batch, tab Results


                                         This tab shows the processes involved in producing this batch (spacers, IG
                                         line, etc.) and which quantities will be produced on the individual machines
                                         (bender, IG line, etc.). The bottom section shows the glass types, thicknesses,
                                         surfaces, and quantities. The fields stockplates, waste, and residue plate will
                                         be filled after optimization. These fields will be empty until an optimization has
                                         been run.

                                         Description of fields

                                         List on the right The list on the right provides the following information:
                                         • Machines: Shows the machine that shall perform the process selected in
                                            the left section.
                                         • Value: This column is available - and filled - only if the production lot type
                                            has been allocated to a grouping (e.g. spacer). In this case, this column
                                            shows the valid entry for each property/formula.
                                         • Quantity: Shows the quantity to be produced in the corresponding lot.
3.00 / 01-2023




                 D-174                                                             A+W Production Detailed Scheduling
                 Software Reference                                                     Detailed Scheduling of Batches




                                        Bottom list The list at the bottom provides the following information:
                                        • Glass type. This field shows all glass type/thickness combinations on this
                                          rack. Example: 1306/6.0 means that the glass type on this rack has the
                                          product number 1306, and a thickness of 6.0 mm. Glass types are defined
                                          in master data.
                                        • Thickness: This field shows the lite thickness. The thickness is defined in
                                          master data.
                                        • Surface (B): Shows the optimized surface in sqm.
                                        • Quantity (B): This field shows the number of lites to be optimized for this
                                          glass type. The following positive figures in the brackets (e.g. 10) show the
                                          number of fillers to be cut. (10) means that 10 fillers will have to be cut.
                                          Negative (e.g. -4) figures show the number of lites that were removed from
                                          this batch, and will have to be cut with a different thickness. (-4) means that
                                          four lites were removed from the batch, and have to be cut with a different
                                          thickness. Both values can be combined, of course: (10/-4).
                                        • Stockplates: This field shows the number of stockplates required for opti-
                                          mization. Stock sizes are defined in master data.
                                        • Waste: This field shows the waste for this optimization in %.
                                        • Residue plate: This field shows the length of the residue plate.

                                        Description of buttons

                                        PlanEdit This button will be active after an optimization has been run. Use
                                        this button to open the program PlanEditor.
                                        For more information on PlanEdit please refer to the documentation on the
                                        program PlanEditor.

                                        Save This button will be active after an optimization has been run. Use this
                                        button to adopt the detailed scheduling results. If you do not want to adopt the
                                        results, close the dialog by clicking on X in the top right corner. Answer the en-
                                        suing security check as required.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                               D-175
                 Detailed Scheduling of Batches                                                      Software Reference




                                         Tab Specials
                                         This tab provides information on existing special elements such as filler or-
                                         ders, residue plates, and breakage.
                                         This tab consists of five sub-tabs:
                                         •   Tab Nested Shapes
                                         •   Tab Filler Orders
                                         •   Tab Residue Plates
                                         •   Tab Rejects
                                         •   Tab Rush Order Lites
                                         •   Tab Thickness

                                         Tab Nested Shapes
                                         View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                         Special > tab Nested Shapes




                                         Fig. D-75    Detailed scheduling for one batch, tab Specials, Tab Nested Shapes


                                         Tab Nested Shapes refers to the joining of shapes. Shapes can be joined in
                                         an optimization item even if they belong to different lites. Prerequisite is that
                                         the shapes belong to the same pseudo series. Double-click on the Shape icon
                                         to edit this option (join yes/no) on this tab.

                                             Define the standard behavior
                                             Whether or not shapes shall be nested by default can be set in A+W Pro-
                                             duction master data as follows: Master Data > Parameters > Module De-
3.00 / 01-2023




                                             tailed Scheduling > Special > Nested Shapes.




                 D-176                                                            A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                           This function is based on the A+W standard shape catalog. Certain shapes
                                           can be nested (e.g. two triangles are joined in a rectangle). This works only
                                           for a few shapes - not for all.

                                           In addition to this simple type of nesting shapes, A+W offers an extended
                                           module - A+W Shape Optimizer. This module allows the nesting of two
                                           shapes of the same shape within a surrounding rectangle which helps to
                                           improve the optimization results considerably.

                                        The symbols in front of the shape number are:

                                        Icon          Explanation

                                                      Shapes will not be joined, but can be.

                                                      Shapes will be joined.

                                        Tab. D-9      Explanation of the systems in tab Join

                                        Fields

                                        Shape This field shows the shape number. The shape number is imported
                                        from the ERP system.

                                        WxH This field shows the sizes of the surrounding rectangle.

                                        Qty. Shows how many of these shapes are included in the detailed schedul-
                                        ing for this batch.

                                        Order This field shows the number of the order which includes shapes. The
                                        shape number is imported from the ERP system.

                                        Item Shows the item number of the order which includes shapes.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                              D-177
                 Detailed Scheduling of Batches                                                         Software Reference




                                         Tab Filler Orders
                                         View > Batch View > Select Batch > Context menu Detailed Scheduling > tab
                                         Special > tab Filler Orders




                                         Fig. D-76    Detailed scheduling for one batch, tab Specials, Tab Filler orders


                                         This tab shows the filler orders available for this glass type.

                                            Show filler orders
                                            Tick the appropriate checkbox in the Organization dialog to use and display
                                            filler orders. If this checkbox is inactive, the table header shows the mes-
                                            sage Filler orders will not be used!

                                         The symbols in front of the date are:

                                         Icon         Explanation

                                                      The optimization defines whether the lite will be produced.

                                                      The lite will be produced with this batch in any case.

                                                      The lite will not be cut with this batch.

                                                      The order has already been scheduled in detail. It has not been
                                                      completed yet, or detailed scheduling could not be completed
                                                      successfully.

                                         Tab. D-10    Explanation of the systems in tab Filler orders
3.00 / 01-2023




                                         Select a record on the list and use the context menu to change the attributes.




                 D-178                                                                A+W Production Detailed Scheduling
                 Software Reference                                                        Detailed Scheduling of Batches




                                        Description of fields

                                        Del. Date This field shows the production date calculated by the system.

                                        Qty. Shows the quantity. The quantity in brackets is the order quantity. The
                                        quantity in front of the brackets is the quantity that can be produced in this
                                        batch.

                                        Order Shows the number of the order which includes filler orders.

                                        Item This field shows the item number of the order which includes filler or-
                                        ders. The shape number is imported from the ERP system.

                                        Change individually/change all Double-click on the table header to switch
                                        between Change individually and Change all. Depending on the mode (indi-
                                        vidual or all), the complete item will (or will not) be used as a filler. Accordingly,
                                        the symbol in front is changed either individually, or for all lites of an item.

                                        Priority This field shows the priority number. Valid entries are:
                                        • 3: lites will be scheduled together with the optimization to improve the over-
                                           all yield. More stockplates can be used.
                                        • 4: lites will be scheduled with the optimization to improve the overall yield.
                                           No additional stockplates will be used.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                   D-179
                 Detailed Scheduling of Batches                                                         Software Reference




                                         Tab Residue Plates
                                         View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                         Special > tab Residue Plates




                                         Fig. D-77    Detailed scheduling for one batch, tab Specials, Tab Residue plates


                                         This tab shows the residue plates available for this glass type.

                                            Show residue plates
                                            Tick the appropriate checkbox in the Organization dialog to use and display
                                            residue plates. If this checkbox is inactive, the table header contains the
                                            message Residue plates will not be used!

                                         The symbols in front of the date are:

                                         Icon         Explanation

                                                      The elements can always be used.

                                                      The elements cannot be used at present.

                                         Tab. D-11    Explanation of the systems in tab Filler orders

                                         Select a record on the list and use the context menu to change the attributes.
3.00 / 01-2023




                 D-180                                                              A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Description of fields

                                        Del. Date This field shows the production date.

                                        Qty. Shows the quantity.

                                        Order This field shows the number of the order which includes filler orders.
                                        The order number is imported from the ERP system.

                                        Item Shows the item number of the order which includes filler orders.

                                        Tab Rejects
                                        View > Batch View > Select ´Batch > Context menu Detailed scheduling > tab
                                        Special > tab Rejects




                                        Fig. D-78     Detailed scheduling for one batch, tab Specials, Tab Rejects


                                        This tab shows the rejects available for this glass type.

                                           Show reject
                                           Tick the appropriate checkbox in the Organization Dialog to use and dis-
                                           play reject. If this checkbox is inactive, the table header contains the mes-
                                           sage Rejects will not be used!
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-181
                 Detailed Scheduling of Batches                                                    Software Reference




                                         The symbols in front of the date are:

                                         Icon         Explanation

                                                      The elements can always be used.

                                                      The elements cannot be used at present.

                                         Tab. D-12    Explanation of the systems in tab Rejects

                                         Select a record on the list and use the context menu to change the attributes.

                                         Description of fields

                                         Del. Date This field shows the production date calculated by the system.

                                         Qty. Shows the quantity.

                                         Order This field shows the number of the order which includes reject orders.
                                         The order number is imported from the ERP system.

                                         Item Shows the item number of the order which includes filler orders.

                                         Last field This field shows the glass type and thickness, as well as the ma-
                                         chines on which the broken lite can be produced.
3.00 / 01-2023




                 D-182                                                             A+W Production Detailed Scheduling
                 Software Reference                                                         Detailed Scheduling of Batches




                                        Tab Rush Order Lites
                                        View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                        Special > tab Rush Order Lites




                                        Fig. D-79     Detailed scheduling for one batch, tab Specials, Tab Rush order lites


                                        This tab shows the rush orders available for this glass type. Rush orders can
                                        be displayed only if the have been entered in dialog Rush orders.

                                           Show rush order lites
                                           Tick the appropriate checkbox in the Organization Dialog to use and dis-
                                           play rush orders. If this checkbox is inactive, the table header contains the
                                           message Rush order lites will not be used!

                                        The symbols in front of the date are:

                                        Icon          Explanation

                                                      The rush order will be produced with this batch in any case.

                                                      The rush order will not be cut with this batch.

                                        Tab. D-13     Explanation of the systems in tab Rush order lites

                                        Select a record on the list and use the context menu to change the attributes.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                   D-183
                 Detailed Scheduling of Batches                                                         Software Reference




                                         Description of fields

                                         Del. Date This field shows the production date calculated by the system.

                                         Qty. Shows the quantity.

                                         Order Shows the number of the order which includes rush orders. -1 means
                                         that the rush order was entered manually, in dialog Enter rush orders.

                                         Item Shows the item number of the order which includes rush orders.

                                         Last field This field shows the glass type and thickness, as well as the ma-
                                         chines on which the broken lite can be produced.

                                         Tab Thickness
                                         View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                         Special > tab Glass Thickness




                                         Fig. D-80     Detailed scheduling for one batch, tab Specials, tab Glass thickness


                                         You can use this dialog to change the optimization (cutting) thickness of lites
                                         to be fit into an IG unit. This will reduce the waste. You can define the lites to
                                         be cut with a thicker glass. This allocation defines the maximum change. Use
                                         tab Glass Thickness to enter the lites that shall be actually cut with a different
                                         thickness. There are the following restrictions for the tab Glass Thickness
                                         •   The thickness can be changed only for lites that are to be fit into an IG unit;
                                             this IG unit must not contain a sub-element with more than one direct sub-
                                             element.
                                         •   Cut element and IG must belong to the same batch.
3.00 / 01-2023




                 D-184                                                              A+W Production Detailed Scheduling
                 Software Reference                                                          Detailed Scheduling of Batches




                                           Change thickness
                                           Tab Glass Thickness is available only if the property Difference in thickness
                                           has been allocated.

                                        The symbols in front of the order are:

                                        Icon          Explanation

                                                      The lite will be cut from thicker glass.

                                                      The lite will not be cut from thicker glass.

                                        Tab. D-14     Explanation of the systems in tab Thickness

                                        Select a record on the list and use the context menu to change the attributes.

                                        Description of fields

                                        Order This field shows the number of the order which contains lites that can
                                        be cut from thicker glass

                                        Item Shows the item number of the order which includes the lites.

                                        Qty. Shows the quantity.

                                        Unnamed field This field shows the current thickness and the cutting table on
                                        which the lite will be cut.

                                        New Thickness Shows the new thickness of the lite to be cut.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-185
                 Detailed Scheduling of Batches                                                        Software Reference




                                         Tab Free Optimization
                                         View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                         Free Optimization




                                         Fig. D-81    Detailed scheduling for one batch, tab Free optimization


                                         This tab shows the optimization types used for the individual glass types. For
                                         glass types optimized in sequence, double-click on the item to change the op-
                                         timization from sequenced optimization to free optimization. An [X] will appear
                                         in front of XOPTS. Only a sequenced optimization can be changed into a free
                                         optimization; this is impossible for manual cutting.
                                         The bottom section of the dialog allows to change the optimization for individ-
                                         ual racks, instead of glass types.

                                         Description of fields

                                         Glass Type This field shows the article number of the glass type. The glass
                                         type is loaded from master data.

                                         Thickness This field shows the lite thickness. The thickness is loaded from
                                         master data.

                                         Optimization This field shows the optimization mode used for detailed
                                         scheduling.

                                         Sqft (B): Shows the optimized surface in sqm.
3.00 / 01-2023




                                         Quantity (B) This field shows the optimized number of lites for this glass
                                         type. * behind the quantity means that fillers are included.



                 D-186                                                             A+W Production Detailed Scheduling
                 Software Reference                                                        Detailed Scheduling of Batches




                                        Bottom section

                                        Rack Shows the number of the rack containing the lites.

                                        Stack Shows the stack containing the lites.

                                        Qty. This field shows the number of lites on the stack.

                                        Width Shows the width of the stack in mm.


                                        Tab Partial Quantities
                                        View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                        Partial Quantities




                                        Fig. D-82     Detailed scheduling for one batch, tab Partial quantities


                                        This tab can be used to remove part of the lites from the optimization. In case
                                        of too much waste for instance, individual lites can be transferred to manual
                                        cutting, or optimized with one of the following batches. The dialog consists of
                                        two sections: The top section shows the glass types to be optimized with this
                                        batch. Select a glass type to view information on the order in the bottom sec-
                                        tion.

                                           Partial quantities
                                           Tab Partial quantities is available only if this has been activated in param-
                                           eter settings.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                               D-187
                 Detailed Scheduling of Batches                                                        Software Reference




                                         Description of the fields in the top section

                                         Glass Type This field shows the glass type/thickness combinations. Exam-
                                         ple: 1306/6.0 means that this glass type's product number is 1306, and its
                                         thickness 6.0 mm. Glass types are defined in master data.

                                         Thickness This field shows the lite thickness. The thickness is defined in
                                         master data.

                                         Sqft (B): Shows the optimized surface in sqm.

                                         Quantity (B): This field shows the number of lites optimized for this glass
                                         type. The following positive figures in the brackets (e.g. 10) show the number
                                         of fillers to be cut. (10) means that 10 fillers will have to be cut. Negative (e.g.
                                         -4) figures show the number of lites that were removed from this batch, and
                                         will have to be cut with a different thickness. (-4) means that four lites were re-
                                         moved from the batch, and have to be cut with a different thickness. Both val-
                                         ues can be combined, of course: (10/-4).

                                         Stockplates This field shows the number of stockplates required for optimi-
                                         zation. Stock sizes are defined in master data.

                                         Waste This field shows the waste of this optimization in %.

                                         Residue Plate This field shows the length of the residue plate.

                                         Description of the fields in the bottom section

                                         Order Shows the number of the order which includes the glass type.

                                         Item Shows the item number of the order which includes the glass type.

                                         Rack Shows the rack number containing the item.

                                         Field without name Shows the lite dimensions.

                                         Qty. Shows the quantity.

                                         Partial Quantity This field shows the partial quantities. If this is 0, no partial
                                         quantities were defined for this item. To enter a partial quantity, double-click on
                                         the order number in the bottom section of the dialog. The input dialog Partial
                                         quantity appears in which you can enter the required quantity.
3.00 / 01-2023




                 D-188                                                             A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Tab Organization
                                        View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                        Organization




                                        Fig. D-83     Detailed scheduling for one batch, tab Organization


                                        This tab gives an overview of the organization settings for this batch used in
                                        detailed scheduling. You can use other settings. Settings should be changed
                                        only with the utmost care.

                                        Description of fields

                                        Processing Sequence The combo box shows the selected processing se-
                                        quence.

                                        Master organization The combo box shows the selected master organiza-
                                        tion.

                                        Organizations This section shows all defined organizations.

                                        Organization Groups This section shows all defined organization groups.

                                        Sort Groups The checkbox is related to field Organization Groups and de-
                                        fines whether the selected group shall be sorted.
                                         The groups will be sorted.
                                         The groups will not be sorted.
                                        The two combo boxes below refer to the checkbox Sort Groups. If this check-
3.00 / 01-2023




                                        box is ticked, select from the top combo box the required group and from the
                                        bottom combo box, the sorting (if applicable).



                 A+W Production Detailed Scheduling                                                              D-189
                 Detailed Scheduling of Batches                                                      Software Reference




                                         Group Formation This combo box shows the Group formation selected for
                                         this organization group.

                                         Sorting within Groups The combo box shows the Sorting within the groups
                                         selected for the organization group.

                                         Racks Section Racks shows the racks that can be used for the batch in ques-
                                         tion. The entries are loaded from dialog Rack settings.

                                         Disable Use this button to disable the rack selected in section Racks. It will
                                         not be available for detailed scheduling, and will be marked ***. To activate the
                                         rack, use again the button disable.

                                         Stacking Mode The radio button defines the rack mode for detailed schedul-
                                         ing. The values are loaded from dialog Rack Settings.

                                         Stacking Mode Groups This section shows the rack mode selected for
                                         groups. The values are loaded from dialog Rack Settings.

                                         Sort Groups The checkbox is related to field Stacking Mode Groups and de-
                                         fines how the selected group shall be sorted.
                                          The groups will be sorted.
                                          The groups will not be sorted.
                                         The two combo boxes below refer to the checkbox Sort Groups. If this check-
                                         box is ticked, select from the top combo box the required group and from the
                                         bottom combo box, the sorting (if applicable).

                                         Max. Number of Groups This field shows the maximum number of groups
                                         that can be put on a rack. The entries are loaded from dialog Rack Settings.

                                         Description of buttons

                                         Save This button is active only if you have changed the settings in tab Orga-
                                         nization. Use the Save button to adopt the changes. Only then will the changes
                                         be adopted.

                                         Repeat If changes have been made, detailed scheduling can be repeated so
                                         that the effects of the changes or the changed rack load become evident. After
                                         that, you can press the [Save] button.
3.00 / 01-2023




                 D-190                                                            A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Tab Organization Options
                                        View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                        Organization Options




                                        Fig. D-84     Detailed scheduling for one batch, tab Organization options


                                        This tab shows the organization applied to this batch.

                                        Description of the fields in section Master Organization

                                        Stack XOPT Together If certain lites are removed from detailed scheduling
                                        to be optimized by XOPT, this field defines how these lites shall be stacked.
                                        The entries are loaded from dialog Master organization.

                                        Fields in section Organization

                                        Left section The left section shows the organization used for this batch. The
                                        entries are loaded from dialog Organization.

                                        Stacking Mode The radio button defines the stacking mode for detailed
                                        scheduling. The values are loaded from dialog Rack Settings.
                                        Field Stacking Mode is related to the field on its right side. The picture in the
                                        right field is based on the property selected in field Stacking Mode. It helps to
                                        visualize the selected property.

                                        Maximum Load of A Racks This field shows the percentage of the A rack
                                        surface that can be loaded.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-191
                 Detailed Scheduling of Batches                                                    Software Reference




                                         No Group Splitting if Occupied by The value in this field defines the point
                                         from which on groups will not be split. The entries are loaded from dialog Or-
                                         ganization.

                                         No Line Item Splitting if Occupied by The entry in this field defines the
                                         point from which on items will not be split. The entries are loaded from dialog
                                         Organization.

                                         Description of buttons

                                         Save This button is active only if you have changed the settings in tab Orga-
                                         nization options. Use the [Save] button to accept the changes. Only then will
                                         the changes be adopted.

                                         Repeat If changes have been made, detailed scheduling can be repeated so
                                         that the effects of the changes or the changed rack load become evident. After
                                         that, you can press the [Save] button.
3.00 / 01-2023




                 D-192                                                           A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Tab Options
                                        View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                        Options




                                        Fig. D-85     Detailed scheduling for one batch, tab Options


                                        This tab contains only optimization options which serve to improve the optimi-
                                        zation results.

                                        Description of fields

                                        Glass Type This field shows the article number of the glass type. The glass
                                        type is loaded from master data.

                                        Thickness This field shows the lite thickness. The thickness is loaded from
                                        master data.

                                        Table Allocation Shows the cutting tables valid for this glass type.

                                        Pair Shows the percentage of pairs in this optimization.

                                        Pair Optimization Ticking this checkbox means that free optimizations will
                                        be automatically run as pair optimizations is possible.

                                        A+W Shape Optimizer If you are working with A+W Shape Optimizer, please
                                        enable this checkbox.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                              D-193
                 Detailed Scheduling of Batches                                                     Software Reference




                                         Runtime Factor The runtime factor defines the number of optimization runs
                                         to be computed by two different methods. Valid entries are 1 to 9. The runtime
                                         factor should always be set to 9. Nine optimization runs each will be calculated
                                         by two different methods; the best result will be selected automatically. If you
                                         enter 9, computing will of course take longer than for an entry of 2. The opti-
                                         mization result will very probably be much better, however.

                                         Cutting Mode The radio button shows the cutting mode used for detailed
                                         scheduling. The entries are loaded from dialog Master Organization.
                                         This field defines the cutting mode for the XOPT(S) optimizations. The radio
                                         button shows the cutting mode used for detailed scheduling. Selection of the
                                         appropriate cutting mode depends on the cutting table and the company's re-
                                         quirements. Generally, cutting mode 1 will produce the best yield while cutting
                                         mode 4 shows the worst results. Higher waste might be compensated by
                                         quicker breakout and stacking (due to the simpler cutting mode). The cutting
                                         mode determines the position of the lites on the subplate between two adja-
                                         cent Y cuts. Possible values:
                                         1: Between two Y cuts, lites of different width and height can lie next to anoth-
                                         er. Hence, W cuts may be made.
                                         2: Between two Y cuts, only lites of different width and the same height can lie
                                         next to another.
                                         3: Between two Y cuts, only lites of the same item can lie next to another.
                                         4: Between two Y cuts, only up to two lites of the same item can lie next to an-
                                         other.
                                         5-7: Special mode for Coopmes tables. This mode is identical to the mode 2-
                                         4. For Z cuts: Z cuts up to the plate edge do not cut any lites.

                                         Trim The fields left trim, right trim, top trim and bottom trim show the trim en-
                                         tered for this glass product. The grey fields refer to the values taken from the
                                         glass product master data. The values in the white fields can be overridden.
                                         This is just a temporary change of trim for the batch on hand.

                                         Max. Subplate This entry shows the maximum width of the subplate. The
                                         greyed field refers to the entry loaded from glass product master data. This en-
                                         try can be changed in the white field. This is just a temporary change of trim
                                         for the lot on hand.

                                         Z Costs This entry defines the costs per Z cut. The greyed field refers to the
                                         entry loaded from glass product master data. This entry can be changed in the
                                         white field. This is just a temporary change of the costs for the lot on hand.
3.00 / 01-2023




                 D-194                                                            A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Tab Stockplate Selection
                                        View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                        Stockplate Selection




                                        Fig. D-86     Detailed scheduling for one batch, tab Stockplate selection


                                        This tab provides an overview of the stockplates used in this batch.

                                        Description of fields

                                        Table Allocation Shows the cutting tables valid for this glass type.

                                        Glass Type This field shows the article number of the glass type. The glass
                                        type is loaded from master data.

                                        Thickness This field shows the lite thickness. The thickness is loaded from
                                        master data.

                                        Width x Height Shows the width and height of the stocksize in mm. This en-
                                        try is loaded from master data.

                                        Quantity Shows the number of existing stocksizes. 9999 means an infinite
                                        number. Double-click on the field to change the number of stocksizes.

                                        Modify Quantity Press this button to open the dialog Number of Stockplates.
                                        In this dialog you can change the number of available stockplates.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                 D-195
                 Detailed Scheduling of Batches                                                       Software Reference




                                         Description of the fields in section Residue Use

                                         Width If a residue plate was left over from a previous optimization that can be
                                         used for this batch, enter the width of this residue plate.

                                         Height If a residue plate was left over from a previous optimization that can
                                         be used for this batch, enter the height of this residue plate.


                                         Change Minimum Number of A Racks
                                         View > Batch View > Select Batch > Context menu Detailed scheduling > tab
                                         Rack Allocation > select Rack Load from the left window > in the right window,
                                         double-click on the Glass Type for which the minimum number of A racks shall
                                         be changed.




                                         Fig. D-87    Change minimum number of A racks


                                         This dialog allows to change the minimum number of A racks required for a
                                         batch.
                                         Override the existing value, and leave the dialog by [Ok].
3.00 / 01-2023




                 D-196                                                           A+W Production Detailed Scheduling
                 Software Reference                                                       Detailed Scheduling of Batches




                                        Sequence of Tables
                                        Master Data > Detailed Scheduling > Tables




                                        Fig. D-88     Sequence of machines


                                        Detailed scheduling allows to allocate a table, independent of the machine al-
                                        location. This requires that the tables are available in a defined checking se-
                                        quence. This sequence can be defined for the tables in master data (only by
                                        means of a text field, without relation of the tables), or by means of this dialog.
                                        This dialog will sort all existing tables by the field XOPT_TISCH::RANG. Use
                                        the buttons [Up] and [Down] to shift the tables and adapt the checking se-
                                        quence. If you quit this dialog via button [OK], the above-mentioned field Rank
                                        will automatically be adapted in the database.
                                        For the internal allocation of tables, all tables will be feasibility-checked for a
                                        certain lite, in the defined sequence. The first table found will be allocated to
                                        the lite.
                                        Internal table allocation will only be used if explicitly set by the user, or if ma-
                                        chinery allocation did not create a table allocation.

                                        Description of fields

                                        Display The view shows all defined cutting tables. Cutting tables are defined
                                        in master data.

                                        Description of buttons

                                        Up Use this button to change the checking sequence of the cutting tables. To
                                        change the checking sequence, select the cutting table to be moved one po-
                                        sition up in the checking sequence. Now press the button [Up] until the cutting
                                        table has reached the required position.

                                        Down Use this button to change the checking sequence of the cutting tables.
                                        To change the checking sequence, select the cutting table to be moved one
                                        position down in the checking sequence. Now press the button [Down] until the
                                        cutting table has reached the required position.
3.00 / 01-2023




                 A+W Production Detailed Scheduling                                                                  D-197
                 Detailed Scheduling of Batches                   Software Reference
3.00 / 01-2023




                 D-198                            A+W Production Detailed Scheduling
Detailed Scheduling            D

                      Section Index




                A+W Production
                 Section Index




                 A                                          Detailed scheduling for batch ...
                 A racks                                    – Tab Filler Orders D-178
                 – Grouping and sorting D-101               – Tab Free optimization D-186
                 – Number ranges D-102                      – Tab Glass thickness D-184
                 – Optimization D-102                       – Tab Nesting D-176
                 – Production sequence D-101                – Tab Options D-193
                 – Standard production organization D-101   – Tab Organization D-189
                 A racks dispatch                           – Tab Organization options D-191
                 – Grouping and sorting D-107               – Tab Partial quantities D-187
                 – Number ranges D-108                      – Tab Rack Allocation D-169
                 – Production sequence D-107                – Tab Rejects D-181
                 – Size categories D-106                    – Tab Residue plates D-180
                 – Standard production organization D-106   – Tab Results D-174
                 A racks spacers                            – Tab Rush Order Lites D-183
                 – Number ranges D-94                       – Tab Special D-176
                 – Optimization D-94                        – Tab Stocksize selection D-195
                 Additional sorting                         Detailed scheduling for batch...
                 – Additional sorting D-151                 – Dialogue D-165
                 – Key D-151                                – Tab Glass types D-166
                 – Tab D-151                                Do not check value
                 – Value D-151                              – Create additional sorting D-152
                 Article number for missing processing      Down
                 – Processing D-162                         – Sequence of machines D-197
                 Ascending                                  – Test sequence D-133
                 – Grouping D-148                           DynOpt settings D-140

                 B                                          E
                 Behavior in detailed scheduling            Editor-Grouping
                 – Lot type D-160                           – Tab D-147
                 Buffer rack D-143                          Editor-Sorting
                                                            – Tab D-150
                                                            End
                 C
                                                            – Filler, Master organization D-136
                 Change minimum number of A racks
                                                            – Rejects, Master organization D-137
                 – Dialogue D-196
                                                            – Residue plate, Master organization D-137
                 Check inversion
                                                            – Test sequence D-133
                 – Rack settings D-143
                 Check number
                 – Harp racks D-156                         F
                 Check quantity                             Filled harp racks
                 – A racks D-154                            – Grouping and sorting D-117
                 – Fixed rack D-157                         – Number ranges D-118
                 Create additional sorting                  – Optimization D-118
                 – Dialogue D-152                           – Production sequence D-117
                 – Do not check value D-152                 – Standard production organization D-117
                 – Sorting D-150                            Filler condition
                 – Value D-152                              – Master organization D-136
                 Creation                                   Flag test
                 – Implicit processing D-164                – Test flag D-11
                                                            Flags D-11
3.00 / 01-2023




                                                            Formula
                 D
                                                            – Grouping D-148
                 Descending
                                                            From/to
                 – Grouping D-148


                 A+W Production Detailed Scheduling                                                D-201
                                                                                                      Section Index




                 – Tab Application, dialog Rack Settings   D-143   – Number D-159
                                                                   – Processing D-162
                 G                                                 – Production sequence D-160
                 Global settings                                   – Reverse sorting D-160
                 – Functional principle D-85                       Lot types
                 Group formation                                   – Tab D-158
                 – Organization groups D-140
                 – Presettings D-146                               M
                 – Rack settings D-142                             Machine type
                 Grouping                                          – Lot type D-159
                 – Ascending D-148                                 Master organization
                 – Descending D-148                                – Dialogue D-134
                 – Formula D-148                                   – End of filler D-136
                 – Lot type D-159                                  – End of rejects D-137
                 – Property D-148                                  – End of residue plate D-137
                 Grouping and sorting                              – Filler condition D-136
                 – A racks D-101                                   – Minimum quantity D-135
                 – A racks dispatch D-107                          – Name D-134
                 – Filled harp racks D-117                         – Production groups D-135
                 – Harp racks, no filling up D-112                 – Pseudo parts D-136
                                                                   – Pseudo series D-135
                 H                                                 – Quick organization D-134
                 Harp racks, no filling up                         – Script D-136
                 – Grouping and sorting D-112                      – Stack XOPT together D-134
                 – Number ranges D-113                             – Start filler D-136
                 – Optimization D-113                              – Start rejects D-137
                 – Production sequence D-112                       – Start residue plate D-137
                 – Standard production organization   D-112        – Tab D-128
                                                                   – Use filler D-136
                                                                   – Use rejects D-137
                 I                                                 – Use residue plates D-136
                 Implicit processing                               – Use rush orders D-137
                 – Creation D-164                                  Max
                 – Lot type D-163                                  – Number of A racks, dialog Rack D-154
                 – Name D-163                                      – Number of groups (tab Application), dialog Rack
                 – Tab D-163                                         Settings D-144
                 – Type D-163                                      – Number of harp racks, dialog Rack D-155
                                                                   Max. number of stacks/rack
                 K                                                 – Racks D-154
                 Key                                               Maximum weight
                 – Additional sorting   D-151                      – A rack D-155
                                                                   – Fixed rack D-157
                 L                                                 – Harp rack D-156
                 L rack                                            Minimum quantity
                 – Dialog Rack D-154                               – Master organization D-135
                 Lot type
                 – Behavior in detailed scheduling D-160           N
                 – Grouping D-159                                  Name
                 – Implicit processing D-163                       – Implicit processing D-163
3.00 / 01-2023




                 – Machine type D-159                              – Lot type D-159
                 – Name D-159                                      – Master organization D-134
                 – Name/Type/Procurement type D-159                – Organization groups D-140


                 D-202                                                        A+W Production Detailed Scheduling
                 Section Index




                 – Processing D-161                                – Organization D-146
                 – Rack settings D-142                             – Processing sequence D-146
                 Name of organization type                         – Sorting on the rack D-146
                 – Organization D-138                              Processing
                 Name/Type/Procurement type                        – Article number for missing processing   D-162
                 – Lot type D-159                                  – Lot type D-162
                 New                                               – Name D-161
                 – Production sequence D-130                       – Procurement type D-161
                 New condition                                     – Tab D-161
                 – Production sequence D-130                       – Type D-161
                 No splitting of..if rack load is over...percent   Processing sequence
                 – Organization D-139                              – Presettings D-146
                 Number                                            Procurement type
                 – Lot type D-159                                  – Processing D-161
                 Number of slots for ...                           Production
                 – Rack D-155                                      – Organization D-138
                 Number ranges                                     Production groups D-135
                 – A racks D-102                                   – Master organization D-135
                 – A racks dispatch D-108                          Production sequence
                 – A racks spacers D-94                            – A racks D-101
                 – Filled harp racks D-118                         – A racks dispatch D-107
                 – Harp racks, no filling up D-113                 – Filled harp racks D-117
                                                                   – Harp racks, no filling up D-112
                 O                                                 – Lot type D-160
                 Optimization                                      – New D-130
                 – A racks D-102                                   – New condition D-130
                 – A racks spacers D-94                            – Settings D-131
                 – Filled harp racks D-118                         – Tab D-130
                 – Harp racks, no filling up D-113                 Property
                 Optimization behavior                             – Grouping D-148
                 – Rack settings D-143                             Pseudo parts
                 Organization                                      – Master organization D-136
                 – Dialogue D-128, D-138                           Pseudo series D-135
                 – Functional principle D-25                       – Master organization D-135
                 – Name of organization type D-138
                 – No splitting of...if rack load is               Q
                   over...percent D-139                            Quantity D-154
                 – Presettings D-146                               – Slot number, dialog Rack D-155
                 – Production D-138                                Quick organization
                 – Stacking mode D-138                             – Master organization D-134
                 – Type D-138
                 Organization groups                               R
                 – Dialogue D-140                                  Rack D-154
                 – Group formation D-140                           – Check number (of A racks) D-154
                 – Name D-140                                      – Check number (of harp racks) D-156
                 – Sorting of groups D-140                         – Check quantity (fixed rack) D-157
                 – Sorting within the groups D-141                 – Dialogue D-153
                                                                   – L rack D-154
                 P                                                 – Max. number of A racks D-154
3.00 / 01-2023




                 Presetting                                        – Max. number of harp racks D-155
                 – Dialogue D-146                                  – Max. number of stacks/rack D-154
                 – Group formation D-146                           – Maximum weight (A rack) D-155


                 A+W Production Detailed Scheduling                                                          D-203
                                                                                                 Section Index




                 – Maximum weight (fixed rack) D-157            Size categories A racks dispatch D-106
                 – Maximum weight (harp rack) D-156             Sorting
                 – Number of slots D-155                        – Create additional sorting D-150
                 – Number of slots for ... D-155                Sorting of groups
                 – Quantity D-154                               – Organization groups D-140
                 – Robot D-154                                  Sorting on the rack
                 – Sortjet D-154, D-156                         – Presettings D-146
                 – Stacking depth (A rack) D-154                Sorting within the groups
                 – Stacking depth (fixed rack) D-156            – Organization groups D-141
                 – Stacking width (A rack) D-154, D-155         – Rack settings D-142
                 – Stacking width (fixed rack) D-156            Sortjet
                 – Start=0 D-155                                – Harp rack D-154, D-156
                 – Two slots/number D-155                       Stack XOPT together
                 Rack mode D-144                                – Master organization D-134
                 Rack settings                                  Stacking depth
                 – Check inversion D-143                        – A rack D-154
                 – Dialogue D-142                               – Rack (fixed rack) D-156
                 – Group formation D-142                        Stacking mode
                 – Max. number of groups (tab                   – Organization D-138
                   Application) D-144                           – Rack settings D-144
                 – Name D-142                                   Stacking mode for groups
                 – Optimization behavior D-143                  – Rack settings D-143
                 – Rack type (tab Application) D-145            Stacking width
                 – Reception rack D-143                         – A rack D-154, D-155
                 – Separate next step (tab Application) D-144   – Fixed rack D-156
                 – Sorting within the groups D-142              Standard production organization
                 – Stacking mode D-144                          – A racks D-101
                 – Stacking mode for groups D-143               – A racks dispatch D-106
                 – Tab Application, from/to D-143               – Harp racks, no filling up D-112
                 Rack type                                      – Short description D-92
                 – Rack settings (tab Application) D-145        Standard production organizations
                 Reception rack                                 – Filled harp racks D-117
                 – Rack settings D-143                          Start
                 Reserve sorting                                – =0, rack D-155
                 – Lot type D-160                               – Filler, Master organization D-136
                 Robot                                          – Rejects, Master organization D-137
                 – Functional principle D-51                    – Residue plate, Master organization D-137
                 – Rack D-154                                   – Test sequence D-132

                 S                                              T
                 Script                                         Test sequence
                 – Master organization D-136                    – Down D-133
                 Sequence of checks                             – End D-133
                 – Functional principle D-81                    – Start D-132
                 Sequence of machines                           – Tab D-132
                 – Dialogue D-197                               – Up D-132
                 – Down D-197                                   Two slots/number
                 – Up D-197                                     – Rack D-155
                 Settings                                       Type
3.00 / 01-2023




                 – Production sequence D-131                    – Implicit processing D-163
                 Short description of the standard production   – Organization D-138
                 organization D-92                              – Processing D-161



                 D-204                                                     A+W Production Detailed Scheduling
                 Section Index




                 U
                 Up
                 – Sequence of machines D-197
                 – Test sequence D-132
                 Use
                 – Filler, Master organization D-136
                 – Rejects, dialog Master Organization   D-137
                 – Residue plates, dialogue Master
                   Organization D-136
                 – Rush orders, dialogue Master
                   Organization D-137

                 V
                 Value
                 – Additional sorting D-151
                 – Create additional sorting D-152
3.00 / 01-2023




                 A+W Production Detailed Scheduling              D-205
                                               Section Index
3.00 / 01-2023




                 D-206   A+W Production Detailed Scheduling

