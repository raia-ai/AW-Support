---
title: "EN AWBusiness ProductionManager 2.21"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["EN_AWBusiness_ProductionManager_2.21"]
version: "1.0"
last_updated: "2025-12-10"
description: "Production Manager           I                                English                  A+W Business Pro                                                                                                           Introduction                                            Introduction                                        This part of the documentation contains editorial notes.                                          Revision Overview                                        Section         Software"
source_file: "EN_AWBusiness_ProductionManager_2.21.pdf"
---


# EN AWBusiness ProductionManager 2.21

Production Manager           I




                           English




             A+W Business Pro
                                                                                                          Introduction




                                       Introduction
                                       This part of the documentation contains editorial notes.


                                       Revision Overview
                                       Section         Software   Description
                                       Version/Date    version

                                       1.00/07-2013    5.0        Original version

                                       2.00/04/2014    5.4        Revision.

                                       2.10/02-2015    5.5        Revision.

                                       2.20/04-2016    v6         Rejects added.

                                       2.21/01-2017               Product and company names adjusted.



                                       Editorial
                                       The editorial provides information on the following topics:
                                       •   Notes on this document
                                       •   Copyrights
                                       •   Trademarks
                                       •   Contact

                                       Notes on this document
                                       This document is intended for end users of A+W Business Pro.
                                       The documentation and software described are licenses that must only be
                                       used or copied in accordance with the conditions of our license agreement.
                                       The contents of the documentation are only informative and are subject to
                                       changes without prior notice. The text and illustrations were compiled with the
                                       utmost care. Still, errors cannot be totally excluded. A+W Software GmbH can-
                                       not be held liable for errors or inaccuracies, unless they can be attributed to
                                       wilful or grossly negligent action.
                                       This document describes the full scope of the master data.

                                       Copyrights
                                       © 2017, A+W Software GmbH, all rights reserved, including the right of reprint,
                                       the production of copies and of the translation.
                                       The documentation may be copied, completely or in part, saved in an archiving
                                       system, or transferred in any other form only in accordance with our license
2.21 / 01-2017




                                       agreement. Transmission of the documentation is not allowed, either electron-
                                       ically, mechanically, or by recording or in any other way, without A+W Software
                                       GmbH's prior written approval.



                 A+W Business Pro Production Manager                                                               I-3
                 Introduction




                                Trademarks
                                All hardware and software names mentioned in this documentation can also
                                be registered trademarks or other property rights of third parties. Third party
                                copyrights must be observed.

                                Contact
                                A+W Software GmbH

                                Am Pfahlgraben 4-10

                                D-35415 Pohlheim

                                   +49 6404 2051 0

                                   +49 6404 2051 877

                                Zentrale@a-w.com

                                http://www.a-w.com
2.21 / 01-2017




                 I-4                                                  A+W Business Pro Production Manager
                                                                                                                                                       Contents




                                       Contents
                                       Introduction .............................................................................................................. I-3
                                         Revision Overview ................................................................................................ I-3
                                         Editorial ................................................................................................................ I-3

                                       Tutorial                                                                                                                I-7
                                       Overview .................................................................................................................. I-9
                                         Documentation ................................................................................................... I-10
                                           Tutorial Structure ............................................................................................ I-10
                                           Display Conventions ....................................................................................... I-11
                                       Key Notes on the Production Manager .................................................................. I-12
                                         The User Interface .............................................................................................. I-13
                                           Standard Mode ............................................................................................... I-13
                                           Expert Mode .................................................................................................... I-13
                                       Standard Mode ...................................................................................................... I-14
                                         Overview ............................................................................................................ I-15
                                           Starting the Standard Mode ............................................................................ I-16
                                           Batch Creation ................................................................................................ I-17
                                           Detailed Scheduling of a Batch ....................................................................... I-17
                                           Output ............................................................................................................. I-18
                                           Results ............................................................................................................ I-19
                                           Stockplates and Optimization Parameters ...................................................... I-21
                                           Information ...................................................................................................... I-22
                                       Expert Mode .......................................................................................................... I-23
                                         Overview ............................................................................................................ I-24
                                           Start the Expert Mode ..................................................................................... I-25
                                         Order Selection .................................................................................................. I-26
                                           Select the Orders ............................................................................................ I-27
                                           The Order and Item Sections .......................................................................... I-28
                                           Grouping of Data ............................................................................................. I-30
                                             Sorting of data ............................................................................................. I-30
                                           Display the Data Clearly Arranged .................................................................. I-31
                                           Product ............................................................................................................ I-33
                                           Information ...................................................................................................... I-33
                                           Rejects ............................................................................................................ I-34
                                             Enter rejects ................................................................................................ I-34
                                             Create a reject batch ................................................................................... I-35
                                           Working with Rejects ...................................................................................... I-36
                                         Batch Management ............................................................................................ I-38
                                           General ........................................................................................................... I-39
                                           Select Batches Based on Certain Criteria ....................................................... I-42
                                           Detailed View for Batches ............................................................................... I-43
                                           Tab Product and Cutting ................................................................................. I-45
                                         Detailed Scheduling ........................................................................................... I-47
                                           The Process of Detailed Scheduling ............................................................... I-48
                                           Optimization Manager ..................................................................................... I-49
                                           Optimize Batches ............................................................................................ I-51
                                           Temporary Optimization .................................................................................. I-52
                                           Abort Optimization .......................................................................................... I-55
                                         Optimization Overview ....................................................................................... I-56
                                           Optimization Detailed View ............................................................................. I-59
2.21 / 01-2017




                                         Output ................................................................................................................. I-60
                                           Reports and Cutting Codes ............................................................................. I-61
                                           Data Issued ..................................................................................................... I-65



                 A+W Business Pro Production Manager                                                                                                             I-5
                 Contents




                            Master Data ........................................................................................................... I-66
                             Racks ................................................................................................................. I-67
                               Logical Racks and Rack Depth ....................................................................... I-68
                               Rack Mode for A Racks .................................................................................. I-69
                                 Buffer rack ................................................................................................... I-70
                               Rack Groups ................................................................................................... I-73
                               Working with Rack Groups ............................................................................. I-74
                               Criteria ............................................................................................................ I-75
                                 Formula ....................................................................................................... I-76
                               Working with Criteria ....................................................................................... I-77
                               Sorting Key ..................................................................................................... I-78
                               Working with Sorting Keys .............................................................................. I-79
                               Rack Organization .......................................................................................... I-80
                             Grouping and Sorting ......................................................................................... I-82
                               General ........................................................................................................... I-83

                            Software Reference                                                                                                   I-85
                            Overview ................................................................................................................ I-87
                              Rack Organization .............................................................................................. I-88
                              Criteria ................................................................................................................ I-91
                              Logical Racks ..................................................................................................... I-93
                              Rack Groups ...................................................................................................... I-95
                              Sorting Key ......................................................................................................... I-96
                            Standard Mode ...................................................................................................... I-97
                              Wizard ................................................................................................................ I-98
                            Expert Mode ........................................................................................................ I-102
                              Order Selection ................................................................................................ I-103
                              Save View ........................................................................................................ I-107
                              Product ............................................................................................................. I-108
                              Reject Items ..................................................................................................... I-110
                              Enter Rejects .................................................................................................... I-113
                              Create New Batch ............................................................................................ I-114
                              Batch Overview ................................................................................................ I-116
                              Detailed View ................................................................................................... I-118
                              Cutting .............................................................................................................. I-120
                              Edit Cutting ....................................................................................................... I-122
                              Set Batch Status ............................................................................................... I-124
                              Machine Rescheduling ..................................................................................... I-125
                              Optimization Manager ...................................................................................... I-126
                              Abort Optimization ............................................................................................ I-128
                              Temporary Optimization ................................................................................... I-129
                              Optimization Overview ..................................................................................... I-131
                              Optimization Detailed View .............................................................................. I-133
                              Output ............................................................................................................... I-134
                              Printer Settings ................................................................................................. I-137
                              Search Order .................................................................................................... I-139

                            Section Index                                                                                                     I-141
                            Index .................................................................................................................... I-143
2.21 / 01-2017




                 I-6                                                                    A+W Business Pro Production Manager
Production Manager          I

                       Tutorial




             A+W Business Pro
                 Tutorial                                                                                       Overview




                                       Overview
                                       The tutorial for the Production Manager module deals with the basics of the
                                       production solution in A+W Business Pro. This tutorial is based on the under-
                                       standing of the master data and the number manager.

                                           The functions depend on the released modules
                                           Please note that the individual functions are available only if the corre-
                                           sponding modules and interfaces have been installed and released.

                                           If you detect functions in this description which are not available in your ver-
                                           sion, please contact A+W Software GmbH.

                                       Sets of Topics
                                       This tutorial offers the following sets of topics:
                                       •   Key Notes on the Production Manager
                                       •   Standard Mode
                                       •   Expert Mode

                                       Required knowledge
                                       This tutorial is meant for those who prepare orders for production in A+W Busi-
                                       ness Pro. Participants must be familiar with the master data and number man-
                                       ager concept.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                    I-9
                 Overview                                                                                  Tutorial




                            Documentation
                            The following documents are available for the Production Manager module:

                            Hand-out                     Printing the tutorial documents for training

                            PDF                          Complete documentation
                                                         • Tutorial
                                                         • Software Reference
                                                         • Index

                            Online help <F1>             Context-sensitive dialog help for the A+W Business
                                                         software references and tutorials on the basic version


                            Tutorial Structure
                            This tutorial consists of sets of topics with several sessions each. Each ses-
                            sion consists of the following elements:

                            Overview                     Each training session starts with an overview of the
                                                         major topics:
                                                         • Objectives: What shall be conveyed?
                                                         • Benefit: What can this knowledge be used for?
                                                         • Maxims: Which correlations are to be remembered?

                            Concepts                     First, the concepts and terms of the corresponding
                                                         training session will be explained. This is followed by
                                                         examples and operating instructions.

                            Exercises                    For some of the sessions, exercises with certain tasks
                                                         and suggested solutions are available.

                            Cross-references             At the end of each training session there is a section
                                                         with cross references pointing out additional information
                                                         in the software reference and in other sections.
                                                         This shall help you to extend your new-found
                                                         knowledge.


                            Reading instructions
                            The contents of a learning unit are based on the knowledge conveyed in the previous
                            unit. We therefore recommend not to skip any learning units. The contents of a
                            learning unit are based on the knowledge conveyed in the previous unit. We therefore
                            recommend not to skip any learning units.
                            If you are already familiar with a subject you should at least read the summary at the
                            beginning of the session in order to bring the main details to mind.
2.21 / 01-2017




                 I-10                                                A+W Business Pro Production Manager
                 Tutorial                                                                                        Overview




                                       Display Conventions
                                       Certain parts of the sentences are specially marked. The meanings are:

                                       Italics                  mark character strings describing the software
                                                                elements, e.g. the dialog Number manager.

                                       Bold                     marks character strings to be entered via keyboard, e.g.:
                                                                Enter 0.

                                       >                        The so-called breadcrumb trail marks shows how to
                                                                open a dialog, e.g. Production > Production > Transfer
                                                                to production.

                                       []                       Square brackets mark the buttons in the dialog, e. g.
                                                                [OK] to save the dat a.

                                       <>                       Pointed brackets refer to keys or shortcuts on the
                                                                keyboard, e. g. <F1> is used to open the online help
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                   I-11
                 Key Notes on the Production Manager                                                                  Tutorial




                                        Key Notes on the Production
                                        Manager
                                        The task of the production manager is to support your planning and prepara-
                                        tion process for production - from batch creation to printing production papers
                                        and creating machine codes.
                                        The procedure is as follows:


                                         Order               Batch creation   Rack           Optimization   Release
                                         Element selection                    organization


                                        Fig. I-1         Standard process for the production solution


                                        The orders are released for internal capacity planning automatically by means
                                        of a predefined status or manually through the user. In this process, a table is
                                        filled with all necessary data. These data are accessed by the Production Man-
                                        ager.
                                        The process is handled by a single dialog so that the user does not have to
                                        switch between different dialogs.
                                        The module can be found in section Production > Production:




                                        Fig. I-2         The Production Manager in the A+W Business menuA+W Business
2.21 / 01-2017




                 I-12                                                                  A+W Business Pro Production Manager
                 Tutorial                                                      Key Notes on the Production Manager




                                       The User Interface
                                       Production Manager can be operated in two different ways:
                                       •   Standard Mode
                                       •   Expert Mode


                                       Standard Mode
                                       In this mode, the program can be operated by means of a simplified user
                                       prompt, the so-called Wizard.
                                       The Wizard permits to finish the whole process (batch creation, optimizations,
                                       etc.) with just a few entries. The optimization results are displayed at the end
                                       of this process and you can decide whether you are going to accept the batch
                                       and the optimization results.
                                       The standard mode is enabled by pressing the corresponding icon.
                                        “Standard Mode” on page I-13


                                       Expert Mode
                                       In this mode, the user performs the individual steps (job creation, optimiza-
                                       tions, etc.) manually. The user can influence the individual batch creation and
                                       processing steps in detail and quite specifically.
                                       The expert mode is enabled by pressing the corresponding icon.
                                        “Expert Mode” on page I-13
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-13
                 Standard Mode                                                                     Tutorial




                                 Standard Mode
                                 This subject area shows you how to use Production Manager in standard
                                 mode.
                                 This includes the following training sessions:
                                 •   “Starting the Standard Mode” on page I-16
                                 •   “Batch Creation” on page I-17
                                 •   “Detailed Scheduling of a Batch” on page I-17
                                 •   “Output” on page I-18
                                 •   “Results” on page I-19
                                 •   “Stockplates and Optimization Parameters” on page I-21
2.21 / 01-2017




                 I-14                                                 A+W Business Pro Production Manager
                 Tutorial                                                                                Standard Mode




                                       Overview
                                       Objectives

                                       • Becoming acquainted with and understanding the standard mode (Wizard)


                                       Benefit

                                       • Using the Wizard you can complete the whole process with just a few mouse
                                         clicks. This saves time and minimises the risk of errors.


                                       Note

                                       Standard mode             The production manager always opens in standard
                                                                 mode.

                                       Rack Organization         Is preset by the standard organization defined in master
                                                                 data. Another organization can be selected if required.

                                       Rack depth                By changing this entry you can influence the optimization
                                                                 result.

                                       Variant                   The tried variants will be kept. This way you can choose
                                                                 the best variant.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                 I-15
                 Standard Mode                                                                                    Tutorial




                                         Starting the Standard Mode
                                         When the Production Manager is started, it will open in standard mode. You
                                         can switch from export mode to standard mode by pressing the corresponding
                                         icon. In this mode, the program appears as follows:




                 Fig. I-3   Main dialog, standard mode


                                         In standard mode, the program can be operated by means of simplified user
                                         prompts (Wizard).
                                         The Wizard permits to start the whole process (batch creation, optimization,
                                         etc.) with just a few entries. The optimization results are displayed at the end
                                         of this process and you can decide whether you are going to accept (save) the
                                         batch and the optimization results or repeat the optimization with other settings
                                         to achieve a better result.
2.21 / 01-2017




                 I-16                                                          A+W Business Pro Production Manager
                 Tutorial                                                                             Standard Mode




                                       Batch Creation
                                       As a first step, select the number manager (NM). All orders included in this NM
                                       will be compiled in a batch.
                                       The number manager compiles the orders which are going to be processed by
                                       the Production Manager in the same batch.




                                       Fig. I-4     Batch creation


                                       The batch number is automatically assigned by the system and cannot be
                                       changed. Field Status shows the status of the batch. In the above example,
                                       the status is Scheduled in detail, i.e. detailed scheduling has been completed
                                       for this batch. Field Description shows the name of the number manager, the
                                       user, and the batch creation date.
                                       Section Batch content will be filled in only after the batch has been created.
                                       You can see the number of IG units, laminated, toughened, and processed
                                       lites included in the batch.


                                       Detailed Scheduling of a Batch
                                       In the second step, the settings for detailed scheduling and optimization are
                                       made. This is done by selecting a predefined rack organization from a combo
                                       box. You can also define the depth of the rack.
                                       Rack organizations and the rack depth are managed in master data (Master
                                       data > Production > Rack organisa-tion).




                                       Fig. I-5     Detailed scheduling
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-17
                 Standard Mode                                                                             Tutorial




                                 If a Range is set for the rack depth (e.g. 80-120 %), field No. of variants defines
                                 the number of variants which are created by clicking on the icon [Start]. Exam-
                                 ple:
                                 •   Rack depth: 80 - 120 %
                                 •   No. of variants: 5
                                 •   Detailed scheduling with a rack depth of 80, 90, 100, 110, and 120 %.


                                 Output
                                 This is where all output types are set, no matter if the output is to be on paper
                                 or as a file. The combo box offers the following selection:
                                 •   None: There will be no output.
                                 •   All: The following media will be issued:
                                     – Production lists for the batch
                                     – Labels for the batch
                                     – Machine control for the batch
                                     – Standard lists for optimization (spacer bender, IG line)
                                     – Cutting plans for optimization
                                     – Cutting labels for optimization
                                     – Machine control for optimization (cutting table)
                                 •   Selection: This is there the media listed under the item All can be enabled.




                                 Fig. I-6     Saving
2.21 / 01-2017




                 I-18                                                   A+W Business Pro Production Manager
                 Tutorial                                                                                Standard Mode




                                       Results
                                       The Optimizations section shows the optimization results. The table will pro-
                                       vide data only after the batch has been created and detailed scheduling and
                                       optimization are completed. You can choose in which sequence the glass
                                       types shall be optimized or set individual glass types to manual cutting.




                                       Fig. I-7     Section Optimizations


                                       When you press the [Start] icon, the suggested batch will be roughly sched-
                                       uled before being scheduled in detail. After that, the individual lites will be op-
                                       timized in the sequence displayed.
                                       When all optimizations have been completed you can use the icon [Save] to
                                       save them. The created batches and optimizations will be saved in the data-
                                       base.

                                          Output is initiated
                                          When you press the [Save] icon, all active output will be initiated including
                                          the transfer of data to the appropriate machines.

                                       Description of the fields in section Overall Result
                                       Section Overall result shows the different optimization variants. By modifying
                                       the settings (e.g. rack depth or the glass type to be optimized first) you can cre-
                                       ate different optimization results (different variants). As a next step, you can
                                       choose the best of these variants and save it. This way, the output (papers and
                                       machinery codes) will only be created for the selected variant. This table will
                                       provide data only after the batch has been created and detailed scheduling
                                       and optimization are completed:




                                       Fig. I-8     Overall result


                                       Field Variant shows how many detailed scheduling and optimization cycles
                                       you have gone through. Every click on the [Start] icon creates another variant
                                       which appears in this column. The individual variants will be kept so that you
2.21 / 01-2017




                                       can eventually choose the best variant.
                                       Field Rack organization shows the rack organization which has been used.
                                       This is the rack organization you have selected in section Detailed scheduling


                 A+W Business Pro Production Manager                                                                 I-19
                 Standard Mode                                                                           Tutorial




                                 and optimization (the entry is loaded from master data: Production > Rack or-
                                 ganization).
                                 Field Factor is the factor for the rack depth you have set in section Detailed
                                 scheduling.
                                 If the lites are put onto harp racks, field Harp racks shows the number of harp
                                 racks which are necessary to put away the lites of the batch. If the lites are
                                 loaded onto A racks, field No. of A racks shows the number of A racks re-
                                 quired.
                                 Field Result shows the overall result for this variant in % while field Waste
                                 shows the total waste for this variant in Eu-ros.




                                 Fig. I-9     Section Optimization per Variant


                                 Field Optimization shows the respective optimizations per variant.
                                 Field Glass type shows the glass types included in the batch. The number in
                                 front of that shows the optimization sequence. The next column shows the cut-
                                 ting table on which the glass is cut, followed by the batch number. Field Quan-
                                 tity shows the quantity per glass type; the next field shows the surface in
                                 square metres.
                                 Field Result shows the optimization result for the glass type in question. The
                                 first figure is the result in %. The following brackets show the number of pat-
                                 terns and the number of stockplates the optimization will need, plus the length
                                 of the residue plate. If the Production Manager automatically sets one of the
                                 glass types to Manual cutting, this is due to the fact that the minimum surface
                                 defined for optimization in master data has not been reached.
                                 The last column shows the waste in Euros.
2.21 / 01-2017




                 I-20                                                  A+W Business Pro Production Manager
                 Tutorial                                                                                Standard Mode




                                       Stockplates and Optimization Parameters
                                       There are two more tabs at the right side of the screen which can be expanded
                                       if required:
                                       •   Tab Stockplates
                                       •   Tab Optimization parameters

                                           Tab Stockplates and Optimization Parameters
                                           When detailed scheduling and optimization of a batch have been complet-
                                           ed, the tabs Stockplates and Optimization Parameters are filled.

                                       You can open the tab Stockplates by clicking on it:




                                       Fig. I-10    Tab Stockplates on the right side of the screen


                                       This tab provides all information on the stockplates for the corresponding glass
                                       type. The displayed values are managed in the Stock module.
                                       You can open the tab Optimization parameters by clicking on it:




                                       Fig. I-11    Tab Optimization parameters on the right side of the screen
2.21 / 01-2017




                                       This tab provides all information on the optimization of the corresponding glass
                                       type. The values displayed are loaded from master data (Articles > Articles).


                 A+W Business Pro Production Manager                                                              I-21
                 Standard Mode                                                                              Tutorial




                                 Section General settings offers a selection of the following optimization
                                 modes:
                                 •   XOPT: This optimization variant is random, i.e. the sequence of the lites af-
                                     ter optimization does not matter and the lites of an item do not have to be
                                     kept together. This will result in quite a good yield but all lites on the racks
                                     have to be rearranged prior to IG production.
                                 •   XOPT-S: This is the standard mode for IG production. The sequence of
                                     lites on the racks defined by the rack organization will be kept. Synchro-
                                     nous optimization of the lites is possible to make sure that lite and counter-
                                     pane can be matched on the IG line. The lites of an order item are always
                                     loaded together on the same A rack after optimization, i.e. the item will not
                                     be split.

                                     Tab Stockplates and Optimization Parameters
                                     When detailed scheduling and optimization of a batch have been complet-
                                     ed, the tabs Stockplates and Optimization Parameters are filled.


                                 Information
                                 This section serves to search an order by its number. Thus, open menu Infor-
                                 mation and the entry Search order. Enter the order number, the corresponding
                                 data are displayed.


                                  How to find the orders
                                 1 Open the entry Information in the menu.
                                 2 Press the [Order] button. Search order opens.
                                 3 Enter the desired number in field Order number.
                                 4 Press the [Filter] button.


                                 Additional information
                                  Software Reference, “Search Order” on page I-139
2.21 / 01-2017




                 I-22                                                    A+W Business Pro Production Manager
                 Tutorial                                                                             Expert Mode




                                       Expert Mode
                                       This subject area will convey the use of the Production Manager in expert
                                       mode.
                                       This includes the following training sessions:
                                       •   “Overview” on page I-24
                                       •   “Order Selection” on page I-26
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-23
                 Expert Mode                                                                                  Tutorial




                               Overview
                               Objectives

                               • Getting to know the view
                               • Knowing how data be loaded
                               • Editing the contents of the views neatly.


                               Benefit

                               • In expert mode you will perform the individual steps like creating batches,
                                 optimising them, etc. You can try out different variants to achieve the best possible
                                 result.


                               Note

                               Expert Mode                  You have to switch explicitly to expert mode.
2.21 / 01-2017




                 I-24                                                   A+W Business Pro Production Manager
                 Tutorial                                                                                    Expert Mode




                                          Start the Expert Mode
                                          You can start the expert mode by pressing the corresponding icon. Among oth-
                                          er things it is meant for multi-stepped glass production. You can perform all the
                                          necessary steps like e.g. compiling the individual batches. You can thus com-
                                          pile batches from different orders based on specific processing steps or opti-
                                          mize different batches together. In this mode, the program appears as follows:




                 Fig. I-12   Main dialog, expert mode


                                          Production Manager consists of the main dialog and different tabs. The follow-
                                          ing main tabs are available:
                                          •   Order selection
                                          •   Batch list
                                          •   Optimization manager
                                          •   Optimization overview
                                          •   Output
                                          Apart from the main tabs there are the tabs which will flash up during the runt-
                                          ime. These include e.g. the Detailed view which is accessible from the Batch
                                          view tab. This view will appear to the right of the tab Batch view.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                  I-25
                 Expert Mode                                                                             Tutorial




                               Order Selection
                               The Order selection offers various selection criteria for compiling an order
                               item's BOM elements in one batch. It serves to restrict the number of orders/
                               order items/BOM elements to be used for batch creation. If an order is select-
                               ed, all of its items are selected too. You can select or deselect individual items
                               however. If you select an item in section Items, the corresponding order will be
                               selected too in section Orders.
                               The dialog consist of several sections. The top right section shows a list of the
                               lites to be optimized. Here you can see the size of the batch. The bottom sec-
                               tion offers order and item data for selection.




                               Fig. I-13    Selection criteria


                               Orders can be selected from the Number manager or from the Process. Proc-
                               esses can also be filtered by Production date.


                               Additional information
                                Software Reference, “Order Selection” on page I-103
2.21 / 01-2017




                 I-26                                                A+W Business Pro Production Manager
                 Tutorial                                                                                 Expert Mode




                                       Select the Orders
                                       This unit teaches you how to select orders for the production manager.
                                       This unit includes the following authorizations to act:
                                       •   How to select orders from the number manager
                                       •   How to select orders by means of the process
                                       •   How to find the orders


                                        How to select orders from the number manager
                                       1 Click on the [Filter] icon. The fields for editing can be accessed now.
                                       2 Tick the radio button Number manager.
                                       3 Open the combo box.
                                       4 Choose the required NM.
                                       5 Press the [Search] icon.
                                       6 The data will be loaded.


                                        How to select orders by means of the process
                                       1 Click on the [Filter] icon. The fields for editing can be accessed now.
                                       2 Tick the radio button Process.
                                       3 Open the combo box.
                                       4 Choose the required process.
                                       5 If required, the date fields from and to can be used to restrict the selection.
                                         These fields refer to the selection you have made in field Process. You can
                                         restrict the process to a certain date. This date refers to the production
                                         date. Example: Process Drilling, production date 15/06/2013 to 20/06/
                                         2013. If you have selected the process Dispatch, the defined date repre-
                                         sents the shipping date.
                                       6 Press the [Search] icon.
                                       7 The data will be loaded.


                                       Additional information
                                        Software Reference, “Order Selection” on page I-103
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                               I-27
                 Expert Mode                                                                               Tutorial




                               The Order and Item Sections
                               The data shown in these areas are based on the settings in section Selection
                               criteria. Section Orders offers a list of orders including order number, customer
                               number, etc.
                               The contents of section Items depend on the selection criteria. The two exam-
                               ples below shall help to illustrate this. We will be using the same order which
                               will be displayed with regard to different Processes.
                               If we select the entry IG production, the following data will be displayed:




                               Fig. I-14    Process IG production


                               The order section shows all orders which include items to be arrissed (or
                               drilled). We select order number 20143.
                               In section Items, mark the individual items of the order 20143 that have to be
                               arrissed. Please note that all items of an order will be marked and locked on
                               the selection list when you select and mark an order in section Order.
                               You can now select individual items and include them in a special batch. To do
                               this , first deselect the order in section Orders before selecting the relevant or-
                               der items individually in section Items.
                               Selecting the entry Cutting results in the display of the following data:
2.21 / 01-2017




                 I-28                                                 A+W Business Pro Production Manager
                 Tutorial                                                                            Expert Mode




                                       Fig. I-15    Process Cutting


                                       Section Items now shows all the individual lites to be cut.


                                       Additional information
                                        Software Reference, “Order Selection” on page I-103
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                        I-29
                 Expert Mode                                                                           Tutorial




                               Grouping of Data
                               Sometimes,a vast bulk of data will be displayed. To be able to keep still track
                               of things, you can group the data then sort them in the group. Grouping of data
                               is identical in the sections Orders and Items. To avoid redundant explanations
                               we are going to describe this process in connection with the example of Or-
                               ders.
                               Grouping is made in the table header:




                               Fig. I-16    Grouping of data


                               The [Column selection] icon opens a box containing all the columns that can
                               be used as grouping criteria. The following chart shows a small selection of
                               columns.




                               Fig. I-17    Column selection


                               Sorting of data
                               You can use the arrows at the end of the column for sorting the data of a group
                               in ascending or descending order:
                               sorts the data in ascending order
                               sorts the data in ascending order.
                               If there is no arrow at the bottom of the column there will be no sorting.
                               Grouping is made in the following section:
2.21 / 01-2017




                               Fig. I-18    Grouping of data




                 I-30                                                A+W Business Pro Production Manager
                 Tutorial                                                                              Expert Mode




                                       Display the Data Clearly Arranged
                                       This unit teaches you how you can show the displayed data clearly arranged
                                       through grouping.
                                       This unit includes the following authorizations to act:
                                       •   How to group the orders
                                       •   Adding further groupings
                                       •   How to save a group
                                       •   How to remove the grouping


                                        How to group the orders
                                       1 Click on the [Column selection] icon.
                                       2 A selection dialog appears.
                                       3 Click the left mouse key on the required field (e.g. customer number) and
                                         keep pressing the mouse key.
                                       4 Keep pressing the mouse key and move the field to the required point in
                                         the table header.
                                       5 When you have reached the required point, release the mouse key.




                                           Fig. I-19   Data grouped by customer number


                                        Adding further groupings
                                       1 Click on the [Column selection] icon.
                                       2 A selection dialog appears.
                                       3 Click the left mouse key on the required field (e.g. input date) and keep
                                         pressing the mouse key.
                                       4 Keep pressing the mouse key and move the field to the required point in
                                         the table header.
                                       5 When you have reached the required point, release the mouse key.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-31
                 Expert Mode                                                                         Tutorial




                                  Fig. I-20    Data grouped by customer number and input date


                                How to save a group
                               1 After you have created the group(s) you can save them.
                               2 Press the [Save] icon.
                               3 The dialog Save view appears.
                               4 Enter a descriptive name in field Name of the view.
                               5 Click on [OK].
                               6 The dialog is closed; the name appears on the right side of the table head-
                                 er.


                                How to remove the grouping
                               1 Select the group you want to delete.
                               2 Click on the [X] icon.
                               3 The selected group will be removed.

                                  Deletion of groups
                                  Groups will be deleted without a security query. The group will be deleted
                                  when you press the [X] icon!
2.21 / 01-2017




                 I-32                                              A+W Business Pro Production Manager
                 Tutorial                                                                                Expert Mode




                                       Product
                                       There is one more tab at the right side of the screen which can be expanded
                                       if required:
                                       •   Tab Product
                                       You can open the tab Prooduct by clicking on it:




                                       Fig. I-21    Tab Product on the right side of the screen


                                       This tab shows detailed information regarding the selected item including the
                                       shape parameter an a graphic preview with dimensioning.


                                       Additional information
                                        Software Reference, “Product” on page I-108


                                       Information
                                       The fields in this section are the same as in the identically named sections in
2.21 / 01-2017




                                       Standard mode which is why we are not going to explain them here again.
                                        “Information” on page I-22




                 A+W Business Pro Production Manager                                                             I-33
                 Expert Mode                                                                           Tutorial




                               Rejects
                               If during the production lites with defects occur, these can now be entered for
                               reproduction.
                               Use the mouse to click the [Rejects] button to open tab Reject Items.




                               Fig. I-22    Tab Reject items


                               This tab provides information on existing rejects and shows detailed informa-
                               tion on rejects to be scheduled. To filter the data you can use the grouping
                               types mentioned above.
                               You have the following options:
                               •   Enter rejects
                               •   Delete rejects
                               •   Create a reject batch

                               Enter rejects
                               Use this dialog to enter rejects. Open in tab Reject Items the context menu and
                               the entry Enter Rejects. A dialog with the same name appears.




                               Fig. I-23    Enter rejects
2.21 / 01-2017




                               Enter the order and item number and press the [Find] button to display all BOM
                               parts for entered order and item number.



                 I-34                                               A+W Business Pro Production Manager
                 Tutorial                                                                                 Expert Mode




                                       Select the BOM parts that shall be entered as rejects and enter the requested
                                       quantity in field Quantity.

                                       Create a reject batch
                                       Use this dialog to create a reject batch. In tab Reject Items select the request-
                                       ed order number, open the context menu and the entry Create New Reject
                                       Batch. The Create New Batch dialog opens.




                                       Fig. I-24    Create reject batch


                                       This dialog is described in detail in chapter:
                                        Software Reference, “Create New Batch” on page I-114
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                               I-35
                 Expert Mode                                                                            Tutorial




                               Working with Rejects
                               In this module you will learn how to deal with rejects.
                               This unit includes the following authorizations to act:
                               •   How to enter rejects
                               •   How to delete rejects
                               •   How to create a new reject batch


                                How to enter rejects
                               1 Click on the icon button [Rejects].
                               2 The Reject Items dialog opens.
                               3 Go to field Order and enter the order number.
                               4 Enter the item number in field Item.
                               5 Click the [Find] icon button. The requested data is displayed in the list.
                               6 Use the mouse to select the lite to be reproduced.
                               7 In Field Quantity enter the number of lites to be reproduced.
                               8 Choose the reject reason from the combo box Reason.
                               9 Choose the reject place from the combo box Location.
                               10 Click on the [Save] button to save the data. The dialog is empty.
                               11 Click on button [End] to close the dialog. You are now back in tab Reject
                                  Items.


                                How to delete rejects
                               1 Click on the icon button [Rejects].
                               2 The Reject Items dialog opens.
                               3 Select the item that is to be deleted.
                               4 Open the context menu.
                               5 Select Delete Rejects. There will be a security query. The item will be de-
                                 leted if you confirm this by [Yes].


                                How to create a new reject batch
                               1 Click on the icon button [Rejects].
                               2 The Reject Items dialog opens.
                               3 Select the order number the reject batch shall be created with.
                               4 Open the context menu.
                               5 Choose Create New Rejects Batch. The dialog Create New Batch opens.
2.21 / 01-2017




                               6 Enter the description for the reject batch in the Description field.
                               7 Select the required organization from the combo box Rack Organization.



                 I-36                                                 A+W Business Pro Production Manager
                 Tutorial                                                                           Expert Mode




                                       8 Enter the factor in field Factor for Rack Depth.
                                       9 If necessary, enable the checkbox Unlimited Rack Depth.
                                       10 Use the checkboxes below to control how to proceed with the batch. Ena-
                                          ble the required checkbox(es).
                                       11 Click on [OK].
                                       12 The selected order number vanishes from the tab Reject Items.


                                       Additional information
                                        Software Reference, “Reject Items” on page I-110
                                        Software Reference, “Enter Rejects” on page I-113
                                        Software Reference, “Create New Batch” on page I-114
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                        I-37
                 Expert Mode                                                                                Tutorial




                               Batch Management
                               Objectives

                               • Learning how to create a batch.
                               • Knowing how data be loaded
                               • Editing the contents of the views neatly.


                               Benefit

                               • Compiling batches in the optimal way will reduce the waste.


                               Note

                               Batch number                The batch number is assigned by the system.

                               Rack Organization           Can be changed after batch creation.

                               Rack depth                  Changing the rack depth will influence the optimization
                                                           result.
2.21 / 01-2017




                 I-38                                                   A+W Business Pro Production Manager
                 Tutorial                                                                                  Expert Mode




                                       General
                                       When a batch is created, all selected elements which have not been sched-
                                       uled otherwise will be included.
                                       Batches are either created by means of the number manager or by process
                                       using the tab Order selection (context menu Create new batch). The following
                                       dialog appears:




                                       Fig. I-25    Create new batch


                                       Description of fields
                                       The program assigns the next higher number as the batch number. Field De-
                                       scription can be used to enter a detailed description of the batch. Now select
                                       the required organization type from the combo box Rack organization. The
                                       combo box lists all rack organizations defined for your site.
                                       The Factor for the rack depth is the factor for the rack depth to be used for this
                                       batch, in percent. The value for the rack depth is defined in master data (Pro-
                                       duction > Logical racks). You can use the factor to temporarily change the en-
                                       try. 100% means that the entry made in master data will be used. 90% means
                                       that only 90% of the depth defined in master data will be used, i.e. less lites
                                       will fit onto the rack. An increase of this value will result in an overload.
                                       Ticking the checkbox Unlimited rack depth will overrule all the entries in master
                                       data.
                                       Use the checkboxes in section Steps after Batch Creation to control how to
                                       proceed with the batch.
                                       Enable the checkbox Detailed Scheduling and the detailed scheduling starts
                                       automatically after batch formation. The checkbox Optimization Manager can
                                       be enabled only if the checkbox Detailed Scheduling is enabled. Then, the tab
                                       Optimization Manager opens after batch formation and detailed scheduling.
                                       But, an optimization will not be generated! The checkbox Total Manual Cutting
                                       can also be enabled after activating the checkbox Detailed Scheduling. Then,
                                       all lites are set to manual cutting after batch formation and detailed scheduling.
                                       The checkbox Output can be enabled only if the checkboxes Detailed Sched-
2.21 / 01-2017




                                       uling and Total Manual Cutting are enabled. Then, the tab Output opens auto-
                                       matically after batch formation, detailed scheduling, and manual cutting.




                 A+W Business Pro Production Manager                                                                I-39
                 Expert Mode                                                                                         Tutorial




                                             The batch has been created ...
                                             When the batch has been created, its status is Roughly scheduled. The creat-
                                             ed batches can be found on tab Batch list.
                                             Roughly scheduled batches can be handled in the following way:
                                             •   You can change the rack organization allocated at batch creation.
                                             •   You can add further elements to the batch.
                                             •   You can remove elements from the batch.
                                             •   You can resolve the batch.
                                             •   You can transfer the batch to detailed scheduling.




                 Fig. I-26     Main dialog, expert mode, batch list


                                             The dialog consist of several sections. The top section shows the selection cri-
                                             teria. The bottom section lists the existing batches.

                                             Information and filter settings




                                             Fig. I-27     Selection criteria for batches
2.21 / 01-2017




                                             Field Batch number can be used to display batches by number. This requires
                                             that you know the number of the batch you want to view. The fields also serve
                                             for limiting the displayed batches in order to keep track of things.


                 I-40                                                                 A+W Business Pro Production Manager
                 Tutorial                                                                                Expert Mode




                                       The Input date fields can be used for displaying the batches by the date on
                                       which they were created.
                                       The Status combo boxes can be used to display the batches by status. The
                                       following statuses are valid:
                                       •   Roughly scheduled: No rack allocation has been made for these batches
                                           yet.
                                       •   Scheduled in detail: These batches have been allocated to racks.
                                       •   Partly optimized: Some of the glass types included in these batches have
                                           already been optimized.
                                       •   Optimized: All glass types of these batches have been optimized already.
                                       •   Partly finished: This field will not be analysed at present.
                                       •   Completed: All elements belonging to these batches are completed.
                                       You can use the field Description to display the batches by name. You have
                                       assigned the name when creating the batch in dialog Create new batch.

                                       Information and filter settings in section Batches
                                       Column Batch number shows the batch number you have selected on tab
                                       Batch list. This is followed by the date on which the batch was created. Column
                                       Description shows the batch description you have entered when creating the
                                       batch. Follows the rack organization you have chosen at batch creation, and
                                       the batch status. The fields IG, LG, TG, and Glass show the quantities of the
                                       corresponding types that are included in the batch.
                                       Entries which appear in light grey in this section have already been transferred
                                       to the optimization manager. If you click on such an entry, a message to that
                                       effect will pop up. You can display the detailed view and the detailed schedul-
                                       ing results for these entries and start the output (machines, reports, etc.).
                                       Sometimes,a vast bulk of data will be displayed. To be able to keep still track
                                       of things, you can group the data then sort them in the group.
                                       The procedure has already been described on tab Order selection which is
                                       why it will not be explained again at this point.
                                        “Grouping of Data” on page I-30


                                       Additional information
                                        Software Reference, “Create New Batch” on page I-114
                                        “Select Batches Based on Certain Criteria” on page I-42
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-41
                 Expert Mode                                                                          Tutorial




                               Select Batches Based on Certain Criteria
                               This unit teaches you how to select batches for production.
                               This unit includes the following authorizations to act:
                               •   How to select the batches by means of the batch number
                               •   How to select the batches by means of the input date
                               •   How to select the batches based on their description


                                How to select the batches by means of the batch number
                               1 Click on the [Filter] icon. The fields for editing can be accessed now.
                               2 Enter the lowest batch number in field from and the highest batch number
                                 in field to. If you enter the same number in both fields, just the one batch
                                 will be shown.
                               3 Click on the [Search] icon.
                               4 The data will be loaded.


                                How to select the batches by means of the input date
                               1 Click on the [Filter] icon. The fields for editing can be accessed now.
                               2 Ener the input date in the fields from to. If you enter the same date in both
                                 fields, only the batches created on that date will be listed.
                               3 Click on the [Search] icon.
                               4 The data will be loaded.


                                How to select the batches by status
                               1 Click on the [Filter] icon. The fields for editing can be accessed now.
                               2 Enter the appropriate criteria in the fields from to.
                               3 Click on the [Search] icon.
                               4 The data will be loaded.


                                How to select the batches based on their description
                               1 Click on the [Filter] icon. The fields for editing can be accessed now.
                               2 Enter the appropriate text in the Description fields.
                               3 Click on the [Search] icon.
                               4 The data will be loaded.


                               Additional information
                                Software Reference, “Create New Batch” on page I-114
2.21 / 01-2017




                 I-42                                                A+W Business Pro Production Manager
                 Tutorial                                                                                  Expert Mode




                                           Detailed View for Batches
                                           The context menu permits to view the batches in detail. The corresponding
                                           batch appears on a separate tab.
                                           In the following example, we are going to open the detailed view for batch
                                           1379. The batch is selected from the batch view for this purpose.
                                           After that you can select the entry Detailed view from the context menu.
                                           The batch and all its elements appear on a separate tab. This dialog is also
                                           split into different sections:




                 Fig. I-28   Detailed view for batch 1379


                                           Information in section Detailed scheduling:




                                           Fig. I-29        Detailed scheduling
2.21 / 01-2017




                                           This section shows the data you have selected or entered for creating the
                                           batch.


                 A+W Business Pro Production Manager                                                                  I-43
                 Expert Mode                                                                                   Tutorial




                               You can see the batch description which can still be changed at this point. You
                               can also change the rack organization by opening the combo box and assign-
                               ing another organization type. The fields Input date and Status cannot be
                               changed. The input date shows when the batch has been created while the
                               Status field marks the current status of the batch. You can still change the fac-
                               tor for the rack depth at this point or assign an unlimited depth to the rack.
                               Information in section Optimization articles:




                               Fig. I-30     Section Optimization articles


                               This section shows the glass type, the quantity to be optimized, the square
                               metres of surface per glass type, and the corresponding amount of square me-
                               tres compared with the total surface of the batch.

                                  Example:

                                  The batch has a total surface of 67.86 sqm to be optimized. Article 104 A+W
                                  Float 4 mm has a surface of 16.35 sqm. These 16.35 sqm represent 24.10 %
                                  of the total surface.

                                  Section Orders and Items show all information relevant for the order, e.g.
                                  order number, customer number, and shipping date.

                                  Section Items shows item-related information on the corresponding orders,
                                  e.g. quantity, shape number, procurement type.


                               Additional information
                                Software Reference, “Detailed View” on page I-118
                                “Description of the fields in section Orders” on page I-104
                                “Description of the fields in section Items” on page I-105
2.21 / 01-2017




                 I-44                                                  A+W Business Pro Production Manager
                 Tutorial                                                                               Expert Mode




                                       Tab Product and Cutting
                                       There are two more tabs at the right side of the screen which can be expanded
                                       if required:
                                       •   Tab Product
                                       •   Tab Cutting

                                       Tab Product
                                       The tab is the same as the identically named fields on tab Order selection
                                       which is why they are not described here again.
                                        “Product” on page I-33

                                       Tab Cutting
                                       You can open the tab Cutting by clicking on it:




                                       Fig. I-31    Tab Cutting on the right side of the screen


                                       It shows detailed information regarding the selected lite including the shape
2.21 / 01-2017




                                       parameter an a graphic preview. The dotted line shows the shape trims.
                                       Use the button [Edit] to open dialog Edit cutting.



                 A+W Business Pro Production Manager                                                             I-45
                 Expert Mode                                                                            Tutorial




                               Fig. I-32    Edit cutting


                               This dialog allows various modifications. You can select e. g. a different shape,
                               the shape parameter as well as the shape trims and change the quantity to be
                               produced. The dotted line shows the shape trims.
                               The modifications will be displayed in section preview.

                                  Edit Cutting Data
                                  Please consider that any modifications made here, will only affect the cut-
                                  ting. They will not be transferred to the order system.

                               Tab Product
                               The tab Product is the same as the identically named tab in the Detailed view
                               for batches which is why it is not described here again.
                                “Tab Product and Cutting” on page I-45


                               Additional information
                                Software Reference, “Edit Cutting” on page I-122
2.21 / 01-2017




                 I-46                                                A+W Business Pro Production Manager
                 Tutorial                                                                                          Expert Mode




                                       Detailed Scheduling
                                       Objectives

                                       • Getting acquainted with and understanding detailed scheduling
                                       • Getting acquainted with and understanding optimization modes
                                       • Circumstances in which the individual modes are used


                                       Benefit

                                       • Only knowing and understanding the different optimization modes will enable you
                                         to adapt detailed scheduling to your production so that it will operate effectively and
                                         in a time-saving manner.


                                       Note

                                       Variant                      The optimization variants you have been trying out will
                                                                    be kept so that you can choose the best ones.

                                       Detailed scheduling          Distribution of the lites of an order to different glass
                                                                    stacks and racks according to defined criteria for
                                                                    grouping and sorting.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                           I-47
                 Expert Mode                                                                        Tutorial




                               The Process of Detailed Scheduling
                               Roughly scheduled batches can be transferred from tab Batch list to detailed
                               scheduling. The task of detailed scheduling is to determine a production se-
                               quence for the elements of these jobs.batches.
                               The production sequence can be determined by criteria like:
                               •   Customer's requirements
                               •   Production restrictions
                               This step also includes the currently assigned rack organization. The batch
                               status changes from Roughly scheduled to Scheduled in detail.
                               Batches which have been scheduled in detail can be treated in the following
                               ways:
                               •   You can repeat detailed scheduling any number of times (e.g. due to
                                   changed rack organization master data).
                               •   The batches can be transferred to the optimization manager.
                               •   You can resolve the batch.
                               •   You can view the rack load.
2.21 / 01-2017




                 I-48                                              A+W Business Pro Production Manager
                 Tutorial                                                                                  Expert Mode




                                         Optimization Manager
                                         Batches which have been scheduled in detail can be transferred to the optimi-
                                         zation manager. When the first optimization for a batch has been run and con-
                                         firmed, the status changes to Partly optimized.
                                         Partly optimized batches can be handled in the following ways:
                                         •   You can edit individual optimizations of the batch.
                                         •   You can treat these batches in just the same was as batches which have
                                             been scheduled in detail (except resolving the batch).




                 Fig. I-33   Optimization manager


                                         This tab serves to optimize the individual glass types for the selected batches.
                                         This dialog is also split into different sections:
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                I-49
                 Expert Mode                                                                            Tutorial




                               Description of fields in section Batches




                               Fig. I-34    Section Batches


                               Column Batch number shows the batch number you have selected on tab
                               Batch list. This is followed by the date on which the batch was created, plus
                               the batch status. Column Description shows the batch description you have
                               entered when creating the batch. Follows the rack organization you have cho-
                               sen at batch creation. The fields IG, LG, TG, and Glass represent the quantities
                               of the corresponding types included in the batch. The factor for the rack depth
                               also represents the factor you have entered at batch creation.

                               Description of fields in section Glass Type




                               Fig. I-35    Section Glass Types


                               This section shows the individual glass types included in the batch. When you
                               expand the entry for the glass type you will be provided with information on the
                               quantity, the surface, and the batch.
                               As several batches can be loaded into the optimization manager, this shows
                               the batches from which the individual glass types have come.

                               Sections Optimizations and Total Result
                               The fields in section Optimizations and Total result are the same as in the iden-
                               tically named sections in Standard mode which is why we are not going to ex-
                               plain them here again.
                                “Results” on page I-19

                               The tabs Stockplates and Optimization Parameters
                               The tabs Stockplates and Optimization parameters on the right edge of the
2.21 / 01-2017




                               screen are the same as the identically-named tabs in section Standard mode
                               which is why they will not be described again at this point.
                                “Stockplates and Optimization Parameters” on page I-21


                 I-50                                                A+W Business Pro Production Manager
                 Tutorial                                                                                    Expert Mode




                                       Optimize Batches
                                       This session shows you how to optimize batches.
                                       This unit includes the following authorizations to act:
                                       •   How to transfer batches to the optimization manager
                                       •   How to set a glass type to manual cutting
                                       •   How to start the optimization
                                       •   How to save the optimization


                                        How to transfer batches to the optimization manager
                                       1 Select the required batch(es) on tab Batch list.
                                       2 Open the context menu.
                                       3 Click on the menu entry Optimization manager.
                                       4 Tab Optimization manager appears and the data are loaded.

                                           Batch transfer
                                           Only batches with the status Scheduled in detail can be transferred to the
                                           optimization manager!


                                        How to set a glass type to manual cutting
                                       1 Select the required glass type(s) in section Optimizations.
                                       2 Open the context menu.
                                       3 Click on the menu entry Manual cutting. The tick in front of the glass type
                                         vanishes and the Result field shows the entry Manual cutting.


                                        How to start the optimization
                                       1 Select the required glass type on tab Optimization manager in section Op-
                                         timizations.
                                       2 Open the context menu.
                                       3 Click on the menu entry Start optimization.
                                       4 After optimization, the section Total result is filled with data.

                                           Ribbon bar
                                           You can also use the ribbon bar (start) to start the optimization. Opening
                                           the context menu can be omitted in this case.


                                        How to save the optimization
                                       1 Open the context menu.
                                       2 Click on the menu entry Save optimization.
2.21 / 01-2017




                                       3 The optimization will be saved.




                 A+W Business Pro Production Manager                                                                I-51
                 Expert Mode                                                                                       Tutorial




                                                Ribbon bar
                                                You can also use the ribbon bar (save) to save the optimization. Opening
                                                the context menu can be omitted in this case.


                                            Temporary Optimization
                                            Every click on the [Start] icon starts a new optimization. This process serves
                                            to optimize batches with different variations. You can e.g. exchange glass
                                            types or change optimization parameters or stockplates. Existing optimiza-
                                            tions are shown as variants in section Total result.
                                            In section Optimizations you can use the context menu to open the detailed
                                            view. It appears on a separate tab.




                 Fig. I-36     Optimization manager, detailed view


                                            This dialog is also split into different sections:
2.21 / 01-2017




                 I-52                                                               A+W Business Pro Production Manager
                 Tutorial                                                                               Expert Mode




                                       Description of the fields in section Rack




                                       Fig. I-37    Section Rack


                                       This is where all relevant information on the racks is displayed. Column Batch
                                       number shows the batch number you have selected on tab Optimization man-
                                       ager. This is followed by the rack number and the rack type on which the lites
                                       are loaded, plus the logical rack.

                                       Description of fields in section Batches




                                       Fig. I-38    Section Batches


                                       Column Batch number shows the batch number you have selected on tab Op-
                                       timization manager plus the date on which the batch was created.

                                       Description of the fields in section Stocksizes




                                       Fig. I-39    Section Stocksizes


                                       Column Quantity shows the required number of stockplates. Fields Height and
                                       Width represent the sizes of the stockplates used. Field Surface shows the
                                       surface in square metres while field Priority represents the corresponding pri-
                                       ority.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                             I-53
                 Expert Mode                                                                             Tutorial




                               Description of the fields in section Pattern




                               Fig. I-40    Section Patterns


                               Column Patterns lists the individual patterns. Click on a pattern to display its
                               image in section Cutting plan. Field Opti group shows the optimization group.
                               Field Quantity shows the quantity with reference to the pattern. Fields Height
                               and Width represent the sizes of the stockplates used.

                               Description of the fields in section Cutting Plan




                               Fig. I-41    Section Cutting Plan


                               This section shows a sketch of the cutting plan created by the optimization.
                               The sketch represents the stockplate to be cut and provides all essential infor-
                               mation on the optimization, the article, and the individual lites.
                               The first number is the rack number (e.g. 7968). This is followed by the lite size
                               (e.g. 1200x800). The order number and corresponding item are shown below.


                               Additional information
                                “Stockplates and Optimization Parameters” on page I-21
2.21 / 01-2017




                 I-54                                                A+W Business Pro Production Manager
                 Tutorial                                                                                     Expert Mode




                                           Abort Optimization
                                           Here it is possible to stop a running optimization by clicking on [Abort].




                 Fig. I-42   Abort optimization


                                           Additional information
                                            Software Reference, “Abort Optimization” on page I-128
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                    I-55
                 Expert Mode                                                                                          Tutorial




                                            Optimization Overview
                                            The optimization overview provides a comprehensive view of the optimiza-
                                            tions that have been run.




                 Fig. I-43     Optimization overview


                                            This tab shows the optimizations which have been run for the individual glass
                                            types. Various selection criteria can be used to keep the contents of this list at
                                            bay. You can view the details of a selected glass type (detailed view) and start
                                            the output (machine output, reports).
                                            This dialog is also split into different sections:

                                            Description of fields in section Selection Criteria




                                            Fig. I-44     Section Selection Criteria
2.21 / 01-2017




                                            This is where you can select the data to be displayed. The combo boxes in
                                            field Optimization give access to specific optimizations. Field Input date can


                 I-56                                                                  A+W Business Pro Production Manager
                 Tutorial                                                                                       Expert Mode




                                          be used to display the optimizations run on certain days while the combo box-
                                          es permit to view specific Batch numbers.
                                          The optimization section is found below. This is where the data are displayed
                                          based on the above selection criteria.

                                          Description of fields in section Optimizations




                 Fig. I-45   Executed optimizations


                                          Sometimes,a vast bulk of data will be displayed. To be able to keep still track
                                          of things, you can group the data then sort them in the group.
                                          The procedure has already been described on tab Order selection which is
                                          why it will not be explained again at this point.
                                           “Grouping of Data” on page I-30
                                          Field Optimization shows the optimization number. This is followed by the op-
                                          timization mode. The following entries are possible:
                                          •   XOPT: This optimization variant is random, i.e. the sequence of the lites af-
                                              ter optimization does not matter and the lites of an item do not have to be
                                              kept together. This will result in quite a good yield but all lites on the racks
                                              have to be rearranged prior to IG production.
                                          •   XOPT-S: This is the standard mode for IG production. The sequence of
                                              lites on the racks defined by the rack organization will be kept. Synchro-
                                              nous optimization of the lites is possible to make sure that lite and counter-
                                              pane can be matched on the IG line. The lites of an order item are always
                                              loaded together on the same A rack after optimization, i.e. the item will not
                                              be split.
                                          Field Glass type shows the glass types included in the optimization. The next
                                          column shows the cutting table on which the glass is cut, followed by the batch
                                          number. Field Status shows the status of the optimization in question. The fol-
                                          lowing statuses are valid:
                                          •   Optimized: The optimization has been run
                                          •   Released: The cutting code for the optimization was issued
                                          •   Partly completed. Cutting has commenced
                                          •   Completed: All stockplates of the optimization have been cut
2.21 / 01-2017




                                          •   Withdrawn: All stockplates of this optimization were withdrawn from stock.
                                          Field Quantity shows the quantity per glass type; the next field shows the sur-
                                          face in square metres.


                 A+W Business Pro Production Manager                                                                     I-57
                 Expert Mode                                                                          Tutorial




                               Field Result provides the optimization result for the corresponding glass type
                               in %.


                               Additional information
                                Software Reference, “Optimization Overview” on page I-131
2.21 / 01-2017




                 I-58                                               A+W Business Pro Production Manager
                 Tutorial                                                                                     Expert Mode




                                           Optimization Detailed View
                                           In section Optimization overview you can use the context menu to open the
                                           detailed view. It appears on a separate tab.




                 Fig. I-46   Optimization overview, detailed view


                                              Identical sections and fields
                                              This dialog is the same as dialog Temporary optimization and is explained
                                              at the following point.

                                               “Temporary Optimization” on page I-52


                                           Additional information
                                            Software Reference, “Optimization Detailed View” on page I-133
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                 I-59
                 Expert Mode                                                                                Tutorial




                               Output
                               Objectives

                               • Knowing the different views of the tab.
                               • Knowing about the output of the different media.


                               Benefit

                               • The optimization manager knows which output is required for the individual
                                 batches. Nothing will be omitted.


                               Note

                               Entries shaded in grey     There will be no output for entries shaded in grey.

                               Printer                    Printing can be done on the standard printers or on other
                                                          printers.

                               Paper and cutting code     Tab Output serves to print all necessary / selected
                                                          production papers and start the data transfer to the
                                                          machines.
2.21 / 01-2017




                 I-60                                                 A+W Business Pro Production Manager
                 Tutorial                                                                                      Expert Mode




                                       Reports and Cutting Codes
                                       All output, no matter if on paper or in the shape of a file, is started from this tab.
                                       The dialog is accessible directly (tab Output), from the tab Batch list, and from
                                       the tab Optimization overview.
                                       From the Batch list you can access the output only for batches with the status
                                       Scheduled in detail, Optimized, or Released. For batches the status of which
                                       is roughly scheduled, output cannot be started because detailed scheduling is
                                       missing.
                                       Output is accessible for all optimizations from the Optimization overview.




                 Fig. I-47   Output


                                       This dialog is also split into different sections:
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                    I-61
                 Expert Mode                                                                                        Tutorial




                                             Description of fields in section Batches
                                             The title of this section is determined by the list from which it is accessed.
                                             When accessed from the Batch list, this section is called Batches and when
                                             accessed from the Optimization overview, it is named Optimizations.




                 Fig. I-48     Output, accessed from the batch list


                                             Column Batch number shows the batch number you have selected on tab
                                             Batch list. This is followed by the date on which the batch was created, plus
                                             the corresponding user. Column Description shows the batch description you
                                             have entered when creating the batch. Follows the rack organization you have
                                             chosen at batch creation. The fields IG, LG, TG, and Glass show the quantities
                                             of the corresponding types that are included in the batch. Valid texts are:

                                             .
                                             Symbol       Explanation

                                                          Output is incorrect e.g. because the batch has not been
                                                          completely optimized.

                                                          The output is correct.


                                             Tab. I-1      Explanation of symbols

                                             Description of fields in section Optimizations




                 Fig. I-49     Output, accessed from the optimization overview


                                             Column Optimization shows the optimization number. This is followed by the
                                             date on which the optimization was created. Column Glass type show the op-
                                             timized glass type and column Mode, the corresponding optimization mode.
                                             Column Cutting table defines the cutting table on which this glass type will be
                                             cut. The next columns refer to the batch number, the status, the quantity opti-
                                             mized, the corresponding surface, and the result.
2.21 / 01-2017




                 I-62                                                               A+W Business Pro Production Manager
                 Tutorial                                                                                       Expert Mode




                                          Description of fields in section Reports




                 Fig. I-50   Section Reports


                                          The column Name defines the report. The following reports are possible:
                                          •    Production lists (IG, laminated glass, etc.)
                                          •    Manual cutting lists
                                          •    Spacer lists
                                          •    Muntin lists
                                          •    Processing lists
                                          •    Rack lists
                                          •    Labels
                                          The next column is called Printer. The combo box gives access to all installed
                                          printers and allows selecting the requested one. The column is preset by the
                                          printer set in master data. Column Copies can be edited as well. Click on the
                                          column to open the field for changing the number of copies. You can change
                                          the preset value. Column Settings offers context menus depending on the re-
                                          port type.
                                          As for Labels, you can control the behaviour in connection with printing serial
                                          labels:




                                          Field Series from defines the minimum quantity for a series. The radio buttons
                                          can be used to define whether a label shall be printed per item or per label. In
                                          connection with the version One label per unit you can use the following field
                                          to define the number of units for which a label shall be printed.
                                          As for lists, you can use the context menu for allocating one printer for all lists.
                                          The same applies to labels. You can also set the number of copies to be print-
                                          ed in general.
2.21 / 01-2017




                                          The icon in the Message column shows the current status.
                                          Entries shaded in grey will not be printed because no output is possible at this
                                          point. Example: Production lists for laminated glass cannot be printed for IG.


                 A+W Business Pro Production Manager                                                                     I-63
                 Expert Mode                                                                                      Tutorial




                 Fig. I-51     Section Machines


                                           This is where the machine code is issued. The program automatically lists all
                                           machines involved in production, no matter if these are benders or whole lines.
                                           Field Machine shows the machine name. Field Output defines the directory in
                                           which the machine code is saved. The next field allows saving the code in an-
                                           other directory.


                                           Additional information
                                            Software Reference, “Output” on page I-134
2.21 / 01-2017




                 I-64                                                           A+W Business Pro Production Manager
                 Tutorial                                                                               Expert Mode




                                       Data Issued
                                       This unit teaches how a list is printed and how a cutting code is generated.
                                       This unit includes the following authorizations to act:
                                       •   How to print a list
                                       •   This is how you generate the cutting code for a machine


                                        How to print a list
                                       1 Select the optimization for which the list must be printed in the Optimiza-
                                         tions section.
                                       2 Select the required list in the Reports section
                                       3 Press the [Start] icon.
                                       4 The output will be started.


                                        This is how you generate the cutting code for a machine
                                       1 Select the optimization for which the cutting code must be generated in the
                                         Optimizations section.
                                       2 Select the machine for which the code must be generated in the Machine
                                         section.
                                       3 Press the [Start] icon.
                                       4 The output of machine control begins.


                                       Additional information
                                        Software Reference, “Output” on page I-134
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-65
                 Master Data                                                                     Tutorial




                               Master Data
                               This subject area introduces the production manager's master data and how
                               to use them.
                               This includes the following training sessions:
                               •   “Racks” on page I-67
                               •   “Criteria” on page I-75
                               •   “Grouping and Sorting” on page I-82
2.21 / 01-2017




                 I-66                                               A+W Business Pro Production Manager
                 Tutorial                                                                                       Master Data




                                       Racks
                                       Objectives

                                       • Knowing and understanding racks
                                       • Knowing and understanding stacking modes
                                       • Understanding the effects of the rack modes


                                       Benefit

                                       • Once you have understood the functions of the stacking modes you can organize
                                         your production accordingly. A well-organized production will save time, space,
                                         and money.


                                       Definitions

                                       Physical rack                Rack (A rack, L rack, fixed rack)

                                       Logical rack                 A logical rack consists of one or more stacks of glass
                                                                    and defines how these stacks belong together (e.g. to
                                                                    turn them into IG or laminated glass units). This depends
                                                                    on the selected stacking mode. A logical rack is just an
                                                                    area on a physical rack with a certain number, onto
                                                                    which glass stacks can be put that belong together.

                                       Rack depth                   The rack depth defines the maximum stack depth
                                                                    (maximum load) of the rack. The bigger the entry here,
                                                                    the more lites can be loaded in front of each other.


                                       Note

                                       What can be put on a rack? Generally, only parts of a batch can be put onto a stack
                                                                  or on a harp rack.

                                       Different glass types on a   The program generally separates different glass types
                                       stack                        and allocates them to different stacks.

                                       Stacking mode                Different glass types can be combined on a logical rack.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                    I-67
                 Master Data                                                                                    Tutorial




                               Logical Racks and Rack Depth
                               A logical rack consists of one or more stacks of glass and defines how these
                               stacks belong together (e.g. to turn them into IG or laminated glass units).
                               A logical rack is just a numbered section on a physical rack onto which match-
                               ing stacks of glass are loaded. lites are loaded onto the logical racks in the pro-
                               duction sequence defined for the individual racks.
                               Physical racks are created from the logical racks. For A racks and L racks, this
                               is done by taking into account the rack depth plus the number of rack sides
                               (1 or 2 for L or A racks).




                                                                                                        Rack depth




                                                                             Logical rack 1001    Logical rack 1002
                                      Rack, side view
                                                                                      Rack, top view
                               Rack depth               Rack depth


                               Fig. I-52      Logical Racks and Rack Depth


                               The rack depth defines the maximum stack depth (maximum load) of the rack.
                               The bigger the entry here, the more lites can be loaded in front of each other.
                               A new stack will be started when the rack depth and thus the maximum load
                               has been reached.
2.21 / 01-2017




                 I-68                                                 A+W Business Pro Production Manager
                 Tutorial                                                                                                 Master Data




                                       Rack Mode for A Racks
                                       Production Manager uses a rack mode in which different glass types can be
                                       combined in several stocks on a logical rack. Different product combinations
                                       to be produced can be loaded.


                                                    Float 4                                                  Rack depth
                                           Grp. 3                              Float 6

                                                                                Float 6
                                                    Float 4
                                                                                                           Thermal

                                                                                Float 6




                                                                                                  Grp. 4
                                                     Float 4


                                                                                                           Thermal
                                                                  Logical rack 1001
                                                                        Top view


                                       Fig. I-53               Rack mode for A racks


                                       •            Each glass type is set onto a different stack.
                                       •            Different glass types are put onto a logical (or physical) rack together.
                                       •            When a stack has reached the maximum, the whole rack number is con-
                                                    sidered to be "full".
                                       •            Groups belonging together must be defined and kept together.
                                       •            You will need less physical racks.
                                       •            You will need additional auxiliary and control mechanisms like e.g. produc-
                                                    tion papers or monitoring systems in order to keep track of things.

                                                    Separation of glass types
                                                    The program always separates the glass types. This applies to the stacking
                                                    of glass types and to optimization.

                                       Stacking of split groups
                                       When a stack has reached the maximum load, the last group will be split. The
                                       lites of this group which exceed the maximum load (rack depth) and the corre-
                                       sponding lites of the appropriate group on the other rack are moved to a new
                                       rack together - with a new rack number. (Group 3 is over the limit which is why
                                       the last lite of group 3 and the last lite of group 4 will go to a new rack: 1002).
                                       New glass types and new groups can be put onto this rack. Rack 1001 is con-
                                       sidered to be full while rack 1002 can take more groups until the maximum
                                       load is reached.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                            I-69
                 Master Data                                                                                                                Tutorial




                                                                                                                             Rack depth
                  Grp. 3




                                                          Float 6

                                                          Float 6
                           Float 4


                                                          Float 6
                           Float 4




                                                                                                                                   Grp. 4
                                                                                                         Grp. 3
                                                                                    Thermal                       Float 4               Thermal
                                      Logical rack 1001                                                               Logical rack 1002
                                              Top view                                                                         Top view




                 Fig. I-54           Stacking of split groups


                                                      Buffer rack
                                                      There is a special rack for each of the three sections IG, laminated glass and
                                                      glass which collects all those BOM elements which are not put onto a regular
                                                      rack. These three racks are A racks with an unlimited rack depth and fixed rack
                                                      numbers: 9991 (glass), 9992 (laminated glass), and 9993 (IG).

                                                             Clashing numbers
                                                             When racks are allocated for rack organization, the program checks if the
                                                             rack numbers used (from-to) clash with other rack numbers or with the
                                                             fixed rack numbers 9991, 9992, and 9993. Clashing numbers are invalid! If
                                                             this occurs, the program will inform you accordingly. The conflicts must now
                                                             be solved.
2.21 / 01-2017




                 I-70                                                                          A+W Business Pro Production Manager
                 Tutorial                                                                                   Master Data




                                       Rack definition and management
                                       The entries are loaded from master data (Production > Rack organization).
                                       This is where the rack types can be defined and managed:
                                       Master data > Production > Logical racks




                                       Fig. I-55     Logical Racks


                                       The dialog consist of several sections. The top left section shows the fields
                                       rack name and type. The type is the detailed scheduling type. The following
                                       types are available:
                                       •   IG
                                       •   LG
                                       •   Glass (individual lites as complete lites to be shipped, or processed lites)

                                           Detailed scheduling type and racks
                                           This allocation also makes sure that the lites are loaded onto the appropri-
                                           ate racks. This means that if you choose the detailed scheduling type LG
                                           for example, the lites will be automatically loaded onto racks meant for lam-
                                           inated glass. No additional filter (criterion) is required. Within the rack or-
                                           ganization for LG racks (allocation) you can use criteria to distinguish e.g.
                                           shapes and rectangles and distribute them to different rack numbers.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                 I-71
                 Master Data                                                                             Tutorial




                               The section below refers to the Grouping and Sorting of the groups. You can
                               assign existing groupings here and define whether groups shall be sorted.
                                “Sorting Key” on page I-78
                               The data concerning the physical racks are shown below this. First comes the
                               name of the physical rack, and from the combo box Type you can choose the
                               appropriate type (A rack, harp rack, L rack). Field Depth can be filled in only
                               for A or L racks. For those, the rack depth is entered here. Field No. of slots
                               can only be filled in for harp racks. In this case, the number of slots is entered
                               here. Field lites per slot is only used for harp racks and defines the number of
                               lites which can be put into a slot.
                               The fields Rack no. from to define the range of numbers for the corresponding
                               rack.


                               Additional information
                                Software Reference, “Logical Racks” on page I-93
2.21 / 01-2017




                 I-72                                                 A+W Business Pro Production Manager
                 Tutorial                                                                                 Master Data




                                       Rack Groups
                                       Rack groups serve for processing racks in front of the IG line or laminating
                                       compound by turns. They are essential if a rack-wide production sequence is
                                       required. Racks which have not been allocated to any rack group can be used
                                       for production at random.
                                       Example:
                                       lites (from one rack group) smaller than 2500 x 1400 are put onto harp racks.
                                       All other lites are loaded onto A racks. The desired production sequence is: by
                                       order (order A, order B, order C).
                                       lites from orders A, B, and C are put onto harp racks as well as onto A racks.
                                       If this is the case, both racks have to be accessible at the same time for IG
                                       production. When producing IG units for order A, lites may have to taken from
                                       the harp rack sometimes and sometimes from the A rack, depending on the
                                       size of the lites. This method is only possible if a Rack group is used for Rack
                                       organization.
                                       The rack group is assigned a sorting key. This key sorts the lites on the racks
                                       that belong to this group.
                                       The corresponding settings are made in dialog Rack groups.
                                       Master data > Production > Logical rack groups




                                       Fig. I-56    Rack Groups
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-73
                 Master Data                                                                      Tutorial




                               Working with Rack Groups
                               This unit teaches you how to handle rack groups.
                               This unit includes the following authorizations to act:
                               •   How to define a new rack group
                               •   How to change an existing rack group
                               •   How to delete a rack group


                                How to define a new rack group
                               1 Click on the icon [New].
                               2 Enter the desired name in the Name field.
                               3 Choose the corresponding sorting from combo box Sorting key.
                               4 Click on the [Save] icon.


                                How to change an existing rack group
                               1 Go to section Rack groups and select the group you want to change.
                               2 Make the required changes. You can change the name as well as the sort-
                                 ing key.
                               3 Click on the [Save] icon.


                                How to delete a rack group
                               1 Go to section Rack groups and select the group to be deleted.
                               2 Click on the [Delete] icon.
                               3 There will be a security query. Click on [Yes].
                               4 The entry will be deleted.


                               Additional information
                                Software Reference, “Rack Groups” on page I-95
2.21 / 01-2017




                 I-74                                                A+W Business Pro Production Manager
                 Tutorial                                                                                  Master Data




                                        Criteria
                                        Criteria serve for checking whether a certain BOM element can be allocated
                                        to a logical rack. Criteria are computing rules using formulas to define whether
                                        an element meets the specified conditions of the logical rack.
                                        It may be required to allocate lites to a new subsequent rack based on a cer-
                                        tain criterion. This is done by means of the checkbox Change rack at. No ad-
                                        ditional lites will be loaded onto the partly loaded rack in this case.
                                        Master data > Production > Criteria
                                        The corresponding dialog looks as follows:




                 Fig. I-57   Criteria


                                        The dialog consist of several sections. The top section shows the details of the
                                        selected criterion.
2.21 / 01-2017




                                        Fig. I-58    Section Criterion




                 A+W Business Pro Production Manager                                                               I-75
                 Master Data                                                                           Tutorial




                               Field Name shows the name of the criterion. The name can be assigned at
                               random. Field Description contains a more detailed description which can also
                               be selected at random. Section Formula shows the formula of which the crite-
                               rion consists.
                               Example:
                               •   Large lites on rack 1000
                               •   Shapes on rack 2000
                               Since the allocation criteria are not mutually exclusive, e.g. large shapes, tab
                               Test sequence (Master data > Production > Rack organization) can be used to
                               define priorities for the criteria.

                               Formula
                               The term Formula stands for a (mathematical) function based on the proper-
                               ties of the BOM elements which has a certain value (variable). The variables
                               which can be used in formulas have English names and are shown in the na-
                               tional language, e.g. Width.


                               Additional information
                                Software Reference, “Criteria” on page I-91
2.21 / 01-2017




                 I-76                                                A+W Business Pro Production Manager
                 Tutorial                                                                                  Master Data




                                       Working with Criteria
                                       This unit teaches you how to handle criteria.
                                       This unit includes the following authorizations to act:
                                       •   How to define a new criterion
                                       •   How to change an existing criterion
                                       •   How to delete a criterion


                                        How to define a new criterion
                                       1 Click on the icon [New].
                                       2 Enter the desired name in field Name, e.g. Series.
                                       3 Field description can be used to enter an additional description, e.g. Quan-
                                         tity > 15.
                                       4 The Formula field is used for assigning the criteria to the formula in the tree
                                         structure on the right. Example: If you double-click on the entry Quantity,
                                         the entry appears in section Formula. Now move the cursor right behind the
                                         entry and enter >15.


                                        How to change an existing criterion
                                       1 Go to section Selection and choose the entry you want to change.
                                       2 Make the required changes in section Criterion.
                                       3 Press the [Save] button


                                        How to delete a criterion
                                       1 Go to section Selection and enter the formula to be deleted.
                                       2 Click on the [Delete] icon.
                                       3 There will be a security query. Click on [Yes].
                                       4 The entry will be deleted.


                                       Additional information
                                        Software Reference, “Criteria” on page I-91
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                               I-77
                 Master Data                                                                            Tutorial




                               Sorting Key
                               So-called sorting keys help to sort a large number of elements. A sorting key
                               can be a single field, e.g Order number or Customer number or can consist of
                               several, linked fields. In the rack organization, a sorting key is allocated to a
                               rack group. This key sorts the elements of a group. The appropriate settings
                               are made in dialog Sorting key.
                               Master data > Production > Sorting key




                               Fig. I-59    Sorting key


                               The dialog is split into different sections. The top section shows the name of
                               the sorting key. Section Sorting key shows the name and a preview. The fields
                               Formula and Sorting in section Details are combo boxes which can be expand-
                               ed. Combo box Formula contains all entries made in dialog Criterion (Master
                               data > Production > Criteria). Combo box Sorting defines whether the entries
                               are sorted in ascending or descending order. The sorting keys also serve for
                               Grouping and Sorting within the groups on the logical racks.


                               Additional information
                                Software Reference, “Sorting Key” on page I-96
2.21 / 01-2017




                 I-78                                                A+W Business Pro Production Manager
                 Tutorial                                                                                Master Data




                                       Working with Sorting Keys
                                       This unit teaches you how to handle sorting keys.
                                       This unit includes the following authorizations to act:
                                       •   How to define a new sorting key
                                       •   How to change an existing rack group
                                       •   How to delete a sorting key


                                        How to define a new sorting key
                                       1 Click on the icon [New].
                                       2 In field Name, enter the name of your choice, e.g. Order.
                                       3 Choose the required entry from the combo box Formula.
                                       4 Choose the required sorting from combo box Sorting.
                                       5 Click on the [Save] icon.


                                        How to change an existing rack group
                                       1 Go to section Sorting key and choose the entry to be changed.
                                       2 Change the fields Formula and Sor-ting as required.
                                       3 Click on the [Save] icon.


                                        How to delete a sorting key
                                       1 Go to section Sorting key and choose the entry to be deleted.
                                       2 Click on the [Delete] icon.
                                       3 There will be a security query. Click on [Yes].
                                       4 The entry will be deleted.


                                       Additional information
                                        Software Reference, “Sorting Key” on page I-96
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-79
                 Master Data                                                                              Tutorial




                               Rack Organization
                               Tailored to the individual production, different rack organizations can be de-
                               fined in the program.
                               One of these rack organizations can be selected as the standard organization.
                               When a batch is created, this rack organization will be assigned to the batch
                               by default. This assignment can be changed prior to detailed scheduling.
                               The rack organization mainly describes the following aspects of production:

                               The products to be produced (what):
                               In the first step, the rack organization is used to classify the different product
                               types collected in a batch (IG, laminated glass, toughened glass, processed
                               glass) by the following three types:
                               •   IG
                               •   Laminated glass
                               •   Glass (including toughened glass).
                               This classification results in lot types.

                               Racks onto which the lites or intermediate products are to be load-
                               ed (where):
                               The second step defines the logical rack onto which the lites of the (interme-
                               diate) product are to be loaded. The criterion of each logical rack will be deter-
                               mined based on the properties of the (intermediate) product to be sorted and
                               if the criterion is relevant for a logical rack, the (intermediate) product will be
                               allocated to this logical rack. If none of the rack organization criteria applies to
                               the (intermediate) product, this (intermediate) product is passed on to the au-
                               tomatically created buffer rack.

                               Chronological and organizational production process (how):
                               The Rack organization dialog lists all rack organizations defined for your com-
                               pany.
                               The sequence of lines from top to bottom represents the chronological se-
                               quence in which the logical racks will be processed in front of the IG line (type
                               IG) or before the laminating pre-compound (type laminated glass). This means
                               that the lites will be taken from these racks in order to produce the correspond-
                               ing unit.
                               lites allocated to a logical rack are actually loaded onto so-called physical
                               racks (harp racks, A racks, L racks). These physical racks have natural restric-
                               tions, e.g. the number of slots or the rack depth. To take this into account, the
                               elements assigned to a logical rack because of a certain criterion will be dis-
                               tributed to physical racks.
                               The criterion for A racks is the rack depth which is taken into account for de-
                               termining the sorting sequence (breakout sequence) of the lites. The rack
                               depth defines how many physical racks will be needed for distributing the lites
2.21 / 01-2017




                               of the batch onto these racks.




                 I-80                                                  A+W Business Pro Production Manager
                 Tutorial                                                                          Master Data




                                          The corresponding dialog looks as follows:
                                          Master data > Production > Rack organization




                 Fig. I-60   Rack Organization


                                          Additional information
                                           Software Reference, “Rack Organization” on page I-88
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                     I-81
                 Master Data                                                                                    Tutorial




                               Grouping and Sorting
                               Objectives

                               • Knowing and understanding grouping
                               • Knowing and understanding sorting
                               • Understanding the effects of grouping and sorting.


                               Benefit

                               • Grouping and sorting serves to organize the stacking of the individual lites in the
                                 required sequence. Without grouping and sorting, the lites would have to be
                                 resorted prior to every production step.


                               Definitions

                               Grouping                     is done by different, unique values for a property, e. g. by
                                                            customer number, glass thickness.

                               Sorting                      is based on properties which assume a progressive
                                                            value within the defined group (e.g. size).


                               Note

                               Creation                     Grouping or sorting is created by random combinations
                                                            of properties and formulas.
2.21 / 01-2017




                 I-82                                                   A+W Business Pro Production Manager
                 Tutorial                                                                                 Master Data




                                       General
                                       The groups and sorting allows allocating the required production sequence to
                                       the individual racks.
                                       Production Manager allows defining grouping criteria and deciding whether
                                       grouping shall be done in a certain sequence (sorted groups) or whether the
                                       contents of the groups shall be sorted (sorting within the group). Every logical
                                       rack can have its own grouping and sorting.
                                       Optimization calculates the optimum yield taking into account the grouping
                                       and sorting. Once it has been set up, the defined sequence can be used for
                                       matching lites of an IG and laminated glass unit.

                                                          Grouped by glass type




                                         Sorted by size

                                       Fig. I-61     Grouping and Sorting


                                       The illustration above shows lites grouped by thickness. Within each group
                                       (perhaps one rack per thickness), lites are sorted by height.
                                       Grouping and sorting depend on how your production is organized and being
                                       run. They are defined by a random combination of properties and formulas.
                                       Grouping is done by different values which are characteristic for a property,
                                       e.g. by Customer number, glass thickness/colour, type of shape. Groups can
                                       be formed by various criteria; the groups do not have to be sorted internally.
                                       The appropriate settings are made in dialog Sorting key.


                                       Additional information
                                        “Sorting Key” on page I-78
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-83
                 Master Data                                Tutorial
2.21 / 01-2017




                 I-84          A+W Business Pro Production Manager
Production Manager              I

                Software Reference




             A+W Business Pro
                 Software Reference                                                                        Overview




                                       Overview
                                       Open the menu Master data > Production
                                       All data required for the correct operation of the production manager are en-
                                       tered and managed in module Master data (section Production).
                                       Master data are arranged in the following menus:
                                       •   Rack organization:
                                           This menu item is used to define the rack organization.
                                            “Rack Organization” on page I-88
                                       •   Criteria:
                                           This menu item is used to define the criteria.
                                            “Criteria” on page I-91
                                       •   Logical racks:
                                           This menu item serves to define the logical racks.
                                            “Logical Racks” on page I-93
                                       •   Rack groups:
                                           This menu item is used to define the rack groups.
                                            “Rack Groups” on page I-95
                                       •   Sorting key:
                                           This menu item serves to define the sorting keys.
                                            “Sorting Key” on page I-96

                                           Dialog buttons
                                           The standard buttons and menus are described in detail in section Over-
                                           view and in the tutorials. We are therefore not going to describe them in
                                           connection with the dialogs.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-87
                 Overview                                                              Software Reference




                            Rack Organization
                            Master Data > Production > Rack Organization




                            Fig. I-62    Rack Organization


                            This dialog is used to define the rack organization or to change existing organ-
                            izations.

                            Description of the fields in section Selection

                            Name Enter the name of the rack organization or change the name of an ex-
                            isting rack organization.

                            Standard This checkbox defines whether the rack organization shall be used
                            as the standard organization. Only one rack organization can be used as a
                            standard at a time.
                             The rack organization is not the standard organization.
                             This rack organization is the standard organization.
2.21 / 01-2017




                 I-88                                            A+W Business Pro Production Manager
                 Software Reference                                                                          Overview




                                       Description of the fields in section Rack Organization

                                       Name This field shows the name of the rack organization.

                                       Standard This checkbox defines whether the rack organization shall be used
                                       as the standard organization. Valid options:
                                       • Yes: This rack organization is the standard organization.
                                       • No: This rack organization is no standard organization.

                                       Description of the fields in section Details

                                       Type This field shows the detailed scheduling type. Valid options:
                                       • IG
                                       • LG
                                       • Glass

                                       Formula This field shows the formula for the rack organization. The entries
                                       are based on the criteria (Master data > Production > Cri-teria). The arrow keys
                                       at the end of the field can be used to access all defined criteria and allocate
                                       them.

                                       Rack (logical) This field shows the logical rack. The entries are based on the
                                       logical racks (Master data > Production > Logical racks). The arrow keys at the
                                       end of the field can be used to access all defined logical racks and allocate
                                       them.

                                       Rack group This field shows the rack group. The entries are based on the
                                       rack groups (Master data > Production > Rack groups). The arrow keys at the
                                       end of the field can be used to access all defined rack groups and allocate
                                       them.

                                       Production sequence If the rack organization includes more than one de-
                                       tailed scheduling type, you have to define the production sequence. The se-
                                       quence is marked by numbers. 1 means that this detailed scheduling type will
                                       be produced first, followed by 2, etc. To change the numbers, click on the field
                                       and enter the required number.

                                       Sequence of checks This field defines the sequence in which the logical
                                       racks are going to be checked.

                                       Rack no. (from) This field shows the start of the rack number range for the
                                       rack in question. The entries are based on the logical racks (Master data >
                                       Production > Logical racks).
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-89
                 Overview                                                              Software Reference




                            Rack no. (to) This field shows the end of the rack number range for the rack
                            in question. The entries are based on the logical racks (Master data > Produc-
                            tion > Logical racks).

                            Rack no. (current) This field shows the current rack number.

                            Rack (physical) This field shows the name of the physical rack. The entries
                            are based on the logical racks (Master data > Production > Logical racks).

                            Rack depth This field shows the depth of the physical rack if the rack is an A
                            or L rack. The entries are based on the logical racks (Master data > Production
                            > Logical racks).

                            Number of slots If the rack is a harp rack, this field shows the number of slots
                            this rack offers. The entries are based on the logical racks (Master data > Pro-
                            duction > Logical racks).

                            Number of lites per slot If the rack is a harp rack, this field shows how many
                            lites can be put into a slot. The entries are based on the logical racks (Master
                            data > Production > Logical racks).


                            Additional information
                             Tutorial, “Racks” on page I-67
2.21 / 01-2017




                 I-90                                             A+W Business Pro Production Manager
                 Software Reference                                                                          Overview




                                       Criteria
                                       Master Data > Production > Criteria




                                       Fig. I-63    Criteria


                                       This dialog is used to define the criteria for the racks to change them.

                                       Description of the fields in section Selection

                                       Name Enter the name of the criterion or change the name of an existing cri-
                                       terion.

                                       Sorting key The combo box lists all sorting keys defined for your company.
                                       Expand the box and choose the required sorting key. The entry is loaded from
                                       master data (Production > Sorting key).
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-91
                 Overview                                                            Software Reference




                            Description of the fields in section Rack Groups

                            Name This field shows the name of the rack group. The entry is loaded from
                            master data (Production > Rack groups).

                            Sorting key This field shows the name of the sorting key. The entry is loaded
                            from master data (Production > Sorting key).

                            Sorting key preview This field shows the formula which defines the sorting
                            key. The entry is loaded from master data (Production > Sorting key).


                            Additional information
                             Tutorial, “Criteria” on page I-75
2.21 / 01-2017




                 I-92                                             A+W Business Pro Production Manager
                 Software Reference                                                                         Overview




                                       Logical Racks
                                       Master Data > Production > Logical Racks




                                       Fig. I-64    Logical racks


                                       Use this dialog to define the logical racks which exist in your company, or
                                       change existing racks.

                                       Description of the fields in section Logical Racks

                                       Name Enter the name of the logical rack.

                                       Type Choose the required type from the combo box. Valid options:
                                       • IG
                                       • LG
                                       • Glass
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                             I-93
                 Overview                                                             Software Reference




                            Description of the fields in section Grouping/Sorting

                            Grouping The combo box lists all groups defined for your company. Select
                            the required group. The entry is loaded from master data (Production > Rack
                            groups).

                            Sorting within groups The combo box lists all sortings defined for your com-
                            pany. Choose the required sorting. The entry is loaded from master data (Pro-
                            duction > Sorting key).

                            Sort groups This checkbox defines whether the groups shall be sorted. The
                             The groups will not be sorted.
                             The groups will be sorted.


                            Additional information
                             Tutorial, “Logical Racks and Rack Depth” on page I-68
2.21 / 01-2017




                 I-94                                             A+W Business Pro Production Manager
                 Software Reference                                                                           Overview




                                       Rack Groups
                                       Master Data > Production > Rack Groups




                                       Fig. I-65    Rack Groups


                                       This dialog can be used to collect certain racks in a rack group. This means
                                       that for laminated glass production, racks belonging to the same group will be
                                       alternately accessed before proceeding to the next rack (or the first rack of the
                                       next group).

                                       Description of fields

                                       Name Enter the name of the rack group.

                                       Sorting key The combo box lists all sorting keys defined for your company.
                                       Expand the box and choose the required sorting key. The entry is loaded from
                                       master data (Production > Sorting key).

                                       Sorting key preview This field shows the formula which defines the sorting
                                       key. The entry is loaded from master data (Production > Sorting key).


                                       Additional information
                                        Tutorial, “Rack Groups” on page I-73
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                               I-95
                 Overview                                                                Software Reference




                            Sorting Key
                            Master Data > Production > Sorting Key




                            Fig. I-66    Sorting key


                            This is where you can define a sorting key to sort a number of elements. This
                            key sorts the lites on the racks that belong to this group.

                            Description of the fields in section Logical Racks

                            Name Enter the name of the sorting key.

                            Formula Select the required formula from the combo box. First, click on the
                            field to activate it. Another click will open the combo box. The entries are
                            based on the criteria (Production > Cri-teria).

                            Sorting Select the required sorting from the combo box. First, click on the
                            field to activate it. Another click will open the combo box. The following options
                            are available:
                            • Ascending: Sorting will be done in ascending order.
                            • Descending: Sorting will be done in descending order.


                            Additional information
2.21 / 01-2017




                             Tutorial, “Sorting Key” on page I-78




                 I-96                                                A+W Business Pro Production Manager
                 Software Reference                                                                 Standard Mode




                                       Standard Mode
                                       This section offers the data you will need to operate the Production Manager
                                       in standard mode.
                                       You will find the following entries:
                                       •   “Order Selection” on page I-103
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-97
                 Standard Mode                                                               Software Reference




                                 Wizard
                                 Production Manager > Standard Mode




                                 Fig. I-67    Standard mode


                                 In standard mode, the program can be operated by means of simplified user
                                 prompts (Wizard).
                                 The Wizard permits to start the whole process (batch creation, optimization,
                                 etc.) with just a few entries. The optimization results are displayed at the end
                                 of this process and you can decide whether you are going to accept (save) the
                                 batch and the optimization results or repeat the optimization with other settings
                                 to achieve a better result.
2.21 / 01-2017




                 I-98                                                  A+W Business Pro Production Manager
                 Software Reference                                                                        Standard Mode




                                       Description of the fields in the section Batch creation

                                       Number manager Use the combo box to access the corresponding data.
                                       The combo box offers all entries you have made in the number manager sec-
                                       tion.

                                       Batch After you made the selection in the number manager, this field shows
                                       the batch number.

                                       Status This field shows the batch status.

                                       Name This field shows the name of the number manager, the user, and the
                                       batch creation date.

                                       Batch content This field will be filled after batch creation. You can see the
                                       number of IG units, laminated, toughened, and processed lites included in the
                                       batch.

                                       Description of the fields in section Detailed Scheduling and Opti-
                                       mization

                                       Rack organization The combo box lists all rack organizations defined for
                                       your company. Select the required organization type. The entries are loaded
                                       from master data (Production > Rack organization).

                                       Factor for the rack depth This entry is the factor for the rack depth (in per-
                                       cent) to be used for this batch. The entry for the rack depth is loaded from mas-
                                       ter data (Production > Logical racks). You can use the factor to temporarily
                                       change the entry. 100% means that the entry made in master data will be
                                       used. 90% means that only 90% of the depth defined in master data will be
                                       used, i.e. less lites will fit onto the rack. An increase of this value will result in
                                       an overload.

                                       Unlimited rack depth This checkbox defines whether the depth of this rack
                                       is unlimited.
                                        The rack has the depth defined in master data, taking into account the field
                                       Factor for the rack depth.
                                        The depth of the rack is unlimited. The value entered in master data will be
                                       changed.

                                       No. of variants This field is related to the field Factor for rack depth. If a
                                       Range is set for the rack depth (e.g. 80-120 %), this field defines the number
                                       of variants which are created by clicking on the icon [Start]. Example:
                                       • Rack depth: 80 - 120 %
                                       • No. of variants: 5
                                       • Detailed scheduling with a rack depth of 80, 90, 100, 110, and 120 %.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                   I-99
                 Standard Mode                                                             Software Reference




                                 Description of the fields in the section Save

                                 Output This is where all output types are set, no matter if the output is to be
                                 on paper or as a file. The combo box offers the following selection:
                                 • None: There will be no output.
                                 • All: The following media will be issued:
                                    – Production lists for the batch
                                    – Labels for the batch
                                    – Machine control for the batch
                                    – Standard lists for optimization (spacer bender, IG line)
                                    – Cutting plans for optimization
                                    – Cutting labels for optimization
                                    – Machine control for optimization (cutting table)
                                 • Selection: This is there the media listed under the item All can be enabled.

                                 Description of fields in section optimizations

                                 Glass type This field shows the glass types included in the batch. The
                                 number in front of that shows the optimization sequence.

                                 Cutting table Here, you see the table on which the glass shall be cut.

                                 Jobs This field shows the batch number.

                                 Quantity This column shows the number of lites to be optimised.

                                 Size This column shows the total surface of the article to be optimised.

                                 Result This field shows the optimization result for the glass type in question.
                                 The first figure is the result in %. The following brackets show the number of
                                 patterns and the number of stockplates the optimization will need, plus the
                                 length of the residue plate.

                                 Waste This field shows the total waste of the glass type in the currency set
                                 for A+W Business Pro.

                                    Contents of section Optimizations
                                    The table will provide data only after the batch has been created and de-
                                    tailed scheduling and optimization are completed:

                                 Description of the fields in section Overall Result

                                 Variant This field shows the different optimization variants.
2.21 / 01-2017




                 I-100                                                A+W Business Pro Production Manager
                 Software Reference                                                                  Standard Mode




                                       Rack organization This is where the rack organization that you have chosen
                                       at batch creation is shown.

                                       Number of harp racks Here you see the number of harp racks which are
                                       necessary to put away the lites of the batch.

                                       Number of A racks Here you see the number of A racks which are neces-
                                       sary to put away the lites of the batch.

                                       Result This field shows the total waste of the glass type in the currency set
                                       for .

                                       Waste This field shows the total waste of the glass type in the currency set
                                       for A+W Business Pro.


                                       Additional information
                                        Tutorial, “Standard Mode” on page I-14
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                          I-101
                 Expert Mode                                                            Software Reference




                               Expert Mode
                               This section offers the data you will need to operate the Production Manager
                               in expert mode.
                               You will find the following entries:
                               •   “Order Selection” on page I-103
                               •   “Reject Items” on page I-110
                               •   “Create New Batch” on page I-114
                               •   “Cutting” on page I-120
                               •   “Optimization Manager” on page I-126
                               •   “Output” on page I-134
2.21 / 01-2017




                 I-102                                                A+W Business Pro Production Manager
                 Software Reference                                                                         Expert Mode




                                       Order Selection
                                       Production Manager > tab Order Selection




                                       Fig. I-68    Order selection in expert mode


                                       Use this dialog to create production batches and optimizations. Various selec-
                                       tion criteria are available for this purpose. The dialog consists of different sec-
                                       tions. In section Selection criteria, you can use the Number manager or the
                                       Process to select the required data.

                                       Description of fields in section Selection Criteria

                                       Number manager After ticking the radio button you can access the corre-
                                       sponding data in the combo box. The combo box offers all entries you have
                                       made in the number manager section.

                                       Work Process After ticking the radio button you can access the correspond-
                                       ing data in the combo box. The combo box contains all work processes from
                                       the orders, transferred to the A+W Business Pro capacity planning.

                                       Date from - to These fields refer to the selection you have made in field Proc-
                                       ess. You can restrict the process to a certain date. This date refers to the pro-
                                       duction date. Example: Process Drilling, production date 15/06/2013 to 20/06/
                                       2013. If you have selected the process Dispatch, the defined date represents
                                       the shipping date.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                               I-103
                 Expert Mode                                                            Software Reference




                               Description of the fields in section optimization Articles

                               Product
                                This column shows the product number. The entries are loaded from master
                               data (Products > Article).

                               Product name 1 This column shows the product name. The entries are load-
                               ed from master data (Products > Article).

                               Quantity This column shows the number of lites to be optimised.

                               Size This column shows the total surface of the article to be optimised.

                               m²% This column shows the surface of the article in relation to the total sur-
                               face of the batch. Example:




                               The batch has a total surface of 67.86 sqm to be optimised. Article 104 A+W
                               Float 4 mm has a surface of 16.35 sqm. These 16.35 sqm represent 24.10 %
                               of the total surface.

                               Description of the fields in section Orders

                               Order number This column shows the order number.

                               Customer number This column shows the customer number.

                               Status This column shows the order status.

                               Input date This columns shows the input date of the order.

                               Order area This column shows the order area. The entries are loaded from
                               Master data (order areas).

                               Consultant This column shows the consultant. The entries are loaded from
                               Employee Master Data. If an employee has been firmly assigned to a custom-
                               er, this is the consultant.

                               Salesman This column shows the salesman. The entries are loaded from
                               Master data.

                               P.O. date If the item needs to be purchased, the P.O. date will be shown here.
2.21 / 01-2017




                               Shipping date This field shows the scheduled shipping date.




                 I-104                                              A+W Business Pro Production Manager
                 Software Reference                                                                         Expert Mode




                                       Requested date This field shows the delivery date requested by the custom-
                                       er.

                                       Delivery date This field shows the delivery date.

                                       Route This field shows the route number. The entries are loaded from master
                                       data (Dispatch > Routes).

                                       Priority This field shows the priority of this order. Valid options are:
                                       • Normal
                                       • Urgent
                                       • Addition
                                       • On call

                                       Customer data The next fields provide information on the customer such as
                                       street address, post code, city, phone number, etc.

                                       Description of the fields in section Items

                                       Order number This column shows the order number.

                                       Item number This column shows the item number.

                                       BOM item This column shows the BOM item. Example: BOM item 0 is the
                                       finished product. BOM item 1 is the article right below. If there is yet another
                                       article below that (intermediate product), it will be item 1.1. If there is another
                                       article next to this one, this will be item 1.2.

                                       Input date This columns shows the input date of the order.

                                       Product This column shows the product number. The entries are loaded from
                                       master data (Products > Article).

                                       Product name 1+2 This column shows the product name. The entries are
                                       loaded from master data (Products > Article).

                                       Short info This column provides quick information on the article. The entries
                                       are loaded from Master data (Article).

                                       Quantity This column tells you how many units have been ordered.

                                       Width This column shows the width of the BOM part.

                                       Height This column shows the height of the BOM part.

                                       Size This column shows the total surface of the article.

                                       Lin.m. This column shows the linear metres around the edges.
2.21 / 01-2017




                                       Shape number This column shows the shape number.




                 A+W Business Pro Production Manager                                                                I-105
                 Expert Mode                                                              Software Reference




                               Product type This column shows the product type. The entry is loaded from
                               master data (Products > General > Product types).

                               Product class This column shows the product class. The entry is loaded
                               from master data (Products > General > Product types).

                               Procurement type This column shows the procurement type. Valid options
                               are:
                               • 0: Production
                               • 1: Cutting
                               • 2: Stock withdrawal
                               • 3: Processing
                               • 7: Glass supplied by customer
                               • 9: P.O.
                               • 102: Stock addition through production
                               • 109: P.O.(complete)

                               Glass This column shows the lites included in this item.

                               Spacer This column shows the width of the spacer.

                               Gas filling This column shows the gas filling. The entry is loaded from mas-
                               ter data (Products > Article > Article).

                               Step This column shows whether a stepped part is below that BOM part in the
                               BOM. The entry is loaded from master data. Valid options:
                               • Yes: A stepped unit exists.
                               • No: A stepped unit does not exist

                               Muntins This column shows whether muntins are below the BOM part in the
                               BOM. Valid options:
                               • Yes: Muntins exist
                               • No: Muntins do not exist

                               Interlayers This column shows the film layer to be used. The entry is loaded
                               from master data (Products > Article > Article).

                               Main elements This column shows the main element. The entry is loaded
                               from master data (Products > Article > Article).

                               Main element type This column shows the main element type. The entry is
                               loaded from master data (Products > Article > Article).


                               Additional information
                                Tutorial, “Order Selection” on page I-26
2.21 / 01-2017




                 I-106                                                A+W Business Pro Production Manager
                 Software Reference                                                                        Expert Mode




                                       Save View
                                       Production Manager > tab Order Selection > Group Orders > icon [Save]




                                       Fig. I-69    Save view


                                       This dialog allows saving the grouping, the sequence and the number of fields
                                       in the list for the view in question. The advantage is that you can define several
                                       groupings with different criteria.

                                       Name of view Enter the name of the view by which this grouping shall be
                                       saved.


                                       Additional information
                                        Tutorial, “Grouping of Data” on page I-30
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                               I-107
                 Expert Mode                                                                Software Reference




                               Product
                               Production Manager > tab Order Selection > tab Product




                               Fig. I-70    Tab Product on the right side of the screen


                               This tab shows detailed information regarding the selected lite including the
                               shape parameter an a graphic preview.

                               Description of fields

                               Quantity This field shows the quantity.

                               Width This field shows the width of the lite.

                               Height This field shows the lite height.

                               Shape number If the lite is a shape, the shape number appears in this field.

                               SN file If the lite is a free shape, the respective SN file appears in this field.
2.21 / 01-2017




                               Shape parameter If the lite is a shape, the respective parameters (height,
                               height 1, etc.) appear in this field.


                 I-108                                                A+W Business Pro Production Manager
                 Software Reference                                                                  Expert Mode




                                       Preview The section shows a preview of the lite including dimensioning.


                                       Additional information
                                        Tutorial, “Product” on page I-33
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                        I-109
                 Expert Mode                                                                 Software Reference




                               Reject Items
                               Production Manager > tab Reject Items




                               Fig. I-71    Tab Reject items


                               This tab appears, after you press the icon button [Rejects]. You can enter re-
                               jects or create reject batches with existing reject lites.

                               Description of fields

                               Order number This column shows the order number.

                               Item number This column shows the item number.

                               Sub-item number This column shows the sub-item number

                               BOM item This column shows the BOM item. Example: BOM item 0 is the
                               finished product. BOM item 1 is the article right below. If there is yet another
                               article below that (intermediate product), it will be item 1.1. If there is another
                               article next to this one, this will be item 1.2.

                               Batch This column shows the batch number.

                               Product This column shows the product number. The entries are loaded from
                               master data (Products > Article).

                               Product name 1+2 This column shows the product name. The entries are
                               loaded from master data (Products > Article).

                               Short info This column provides quick information on the article. The entries
                               are loaded from Master data (Article).

                               Quantity This column tells you how many units have been ordered.

                               Width This column shows the width of the BOM part.

                               Height This column shows the height of the BOM part.

                               Size This column shows the total surface of the article.
2.21 / 01-2017




                 I-110                                                A+W Business Pro Production Manager
                 Software Reference                                                                   Expert Mode




                                       Lin.m. This column shows the linear metres around the edges.

                                       Shape number This column shows the shape number.

                                       Product type This column shows the product type. The entry is loaded from
                                       master data (Products > General > Product types).

                                       Product class This column shows the product class. The entry is loaded
                                       from master data (Products > General > Product types).

                                       Procurement type This column shows the procurement type. Valid options
                                       are:
                                       • 0: Production
                                       • 1: Cutting
                                       • 2: Stock withdrawal
                                       • 3: Processing
                                       • 7: Glass supplied by customer
                                       • 9: P.O.
                                       • 102: Stock addition through production
                                       • 109: P.O.(complete)

                                       Glass This column shows the lites included in this item.

                                       Spacer This column shows the width of the spacer.

                                       Gas filling This column shows the gas filling. The entry is loaded from mas-
                                       ter data (Products > Article > Article).

                                       Step This column shows whether a stepped part is below that BOM part in the
                                       BOM. The entry is loaded from master data. Valid options:
                                       • Yes: A stepped unit exists.
                                       • No: A stepped unit does not exist

                                       Muntins This column shows whether muntins are below the BOM part in the
                                       BOM. Valid options:
                                       • Yes: Muntins exist
                                       • No: Muntins do not exist

                                       Interlayers This column shows the film layer to be used. The entry is loaded
                                       from master data (Products > Article > Article).

                                       Main elements This column shows the main element. The entry is loaded
                                       from master data (Products > Article > Article).

                                       Main element type This column shows the main element type. The entry is
                                       loaded from master data (Products > Article > Article).
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                          I-111
                 Expert Mode                                                          Software Reference




                               Processings This column shows the processing for the corresponding item.

                               Production date This column shows the production date for the correspond-
                               ing item.

                               Machine This column shows the machine for the corresponding item.


                               Additional information
                                Tutorial, “Product” on page I-33
2.21 / 01-2017




                 I-112                                              A+W Business Pro Production Manager
                 Software Reference                                                                      Expert Mode




                                       Enter Rejects
                                       Production Manager > tab Reject Items > Context menu > Enter Rejects




                                       Fig. I-72    Enter rejects


                                       In this dialog, you have the opportunity to enter rejects manually.

                                       Description of fields

                                       Order Enter the order number the reject lites belong to.

                                       Item Enter the item number.

                                       Quantity Enter the quantity, i.e. the number of lites to be reproduced.

                                       Reason Select the reject reason from the combo box.

                                       Location Select the reject place from the combo box.

                                       Sub-item number This column shows the sub-item number
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                             I-113
                 Expert Mode                                                                  Software Reference




                               Create New Batch
                               Production Manager > tab Order Selection > Select order > Open context
                               menu > Create New Batch
                               Production Manager > tab Reject Items > Select order > Open context menu
                               > Create New Reject Batch




                               Fig. I-73     Create new batch


                               This dialog is used for creating new batches. The dialog is accessed by the
                               context menu, entry Create new batch.

                               Description of fields

                               Batch number This field shows the batch number. The batch number is as-
                               signed by the system in ascending order. You cannot change the batch
                               number.

                               Name Enter the name of the batch. By default, this field shows the selection
                               criterion (e.g. cutting) and the user. The data are loaded from master data. You
                               can change the entries.

                               Rack organization The combo box lists all rack organizations defined for
                               your company. Select the required organization type. The entries are loaded
                               from master data (Production > Rack organization).

                               Factor for the rack depth This entry is the factor for the rack depth (in per-
                               cent) to be used for this batch. The entry for the rack depth is loaded from mas-
                               ter data (Production > Logical racks). You can use the factor to temporarily
                               change the entry. 100% means that the entry made in master data will be
                               used. 90% means that only 90% of the depth defined in master data will be
                               used, i.e. less lites will fit onto the rack. An increase of this value will result in
                               an overload.
2.21 / 01-2017




                 I-114                                                 A+W Business Pro Production Manager
                 Software Reference                                                                      Expert Mode




                                       Unlimited rack depth This checkbox defines whether the depth of this rack
                                       is unlimited.
                                        The rack has the depth defined in master data, taking into account the field
                                       Factor for the rack depth.
                                        The depth of the rack is unlimited. The value entered in master data will be
                                       changed.

                                       Description of check boxes

                                       Detailed scheduling If you enable this check box, detailed scheduling takes
                                       place automatically after batch formation.

                                       Optimization manager This check box can only be used in connection with
                                       the check box Detailed scheduling. Then, the tab Optimization Manager opens
                                       after batch formation and detailed scheduling. But, an optimization will not be
                                       generated!

                                       Total manual cutting This check box can only be used in connection with the
                                       check box Detailed scheduling. Then, all lites are set to manual cutting after
                                       batch formation and detailed scheduling..

                                       Output The check box is enabled after activating the check boxes Detailed
                                       Scheduling and Total Manual Cutting.


                                       Additional information
                                        Tutorial, “Batch Management” on page I-38
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-115
                 Expert Mode                                                                         Software Reference




                                          Batch Overview
                                          Production Manager > tab Batch List




                 Fig. I-74   Batch list


                                          This dialog shows you all saved created batches. The dialog consists of two
                                          sections. The top section shows the selection criteria. The bottom section lists
                                          the existing batches.

                                          Description of fields in section Selection Criteria

                                          Batch number Fields from to can be used to display batches by number.
                                          The fields also serve for limiting the displayed batches in order to keep track
                                          of things.

                                          Creation date This field can be used for displaying the batches by the date
                                          on which they were created.
2.21 / 01-2017




                 I-116                                                          A+W Business Pro Production Manager
                 Software Reference                                                                      Expert Mode




                                       Status This combo box can be used to display the batches by status. The fol-
                                       lowing statuses are valid:
                                       •   Roughly scheduled: No rack allocation has been made for these batches
                                           yet.
                                       •   Scheduled in detail: These batches have been allocated to racks.
                                       •   Partly optimised: Some of the glass types included in these batches have
                                           already been optimised.
                                       •   Optimised: All glass types of these batches have been optimised already.
                                       •   Released: The production papers have been printed and the machine code
                                           has been created for the optimization of this batch.
                                       •   Partly completed: Some parts of the batch have been produced but yet not
                                           all.
                                       •   Completed: All parts of the batch have been produced.

                                       Name You can use this field to display the batches by name. You have as-
                                       signed the name when creating the batch in dialog Create new batch.

                                       Description of fields in section Batches

                                       Batch number This column shows the batch number.

                                       Creation date This field shows the date when the batch has been created.

                                       Status This field shows the status of the batch.

                                       Description This field shows the description you entered at batch creation.

                                       Rack organization This is where the rack organization that you have chosen
                                       at batch creation is shown.

                                       IG This field shows the quantity of IG included in the batch.

                                       LG This field shows the quantity of LAMI included in the batch.

                                       Toughened glass This field shows the quantity of TG included in the batch.

                                       Glass (single and processed) This field shows the single and processed
                                       glass included in the batch.

                                       Factor for the rack depth This is where the factor that you have chosen at
                                       batch creation is shown.


                                       Additional information
                                        Tutorial, “Batch Management” on page I-38
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-117
                 Expert Mode                                                                         Software Reference




                                           Detailed View
                                           Production Manager > tab Batch List > Select batch > Open context menu >
                                           Detailed View




                 Fig. I-75   Detailed view for a batch


                                           This dialog allows viewing a selected batch in detail. This dialog is accessed
                                           by the context menu, entry Detailed view, and consists of several sections.

                                           Description of the fields in section Detailed Scheduling

                                           Name Shows the batch name. You have assigned the name when creating
                                           the batch in dialog Create new batch. If required, you can change the name at
                                           this point.

                                           Rack organization Shows the rack organization. This is the rack organiza-
                                           tion you have selected in dialog Create new batch when creating the batch.
                                           You can only change the rack organization for batches in status Roughly
                                           scheduled.

                                           Creation date Shows the date on which the batch was created.
2.21 / 01-2017




                 I-118                                                          A+W Business Pro Production Manager
                 Software Reference                                                                      Expert Mode




                                       Status Show the batch status.

                                       Factor for the rack depth Shows the factor (in percent) for the rack depth to
                                       be used for this batch. You can only change the value for batches either in sta-
                                       tus Roughly scheduled or Detailed scheduled.

                                       Unlimited rack depth This checkbox defines whether the depth of this rack
                                       is unlimited. You can only change the value for batches either in status Rough-
                                       ly scheduled or Detailed scheduled.
                                        The rack has the depth defined in master data, taking into account the field
                                       Factor for the rack depth.
                                        The depth of the rack is unlimited. The value entered in master data will be
                                       changed.

                                       Description of the fields in section optimization Articles

                                       Product This column shows the product number. The entries are loaded from
                                       master data (Products > Article).

                                       Product name 1 This column shows the product name. The entries are load-
                                       ed from master data (Products > Article).

                                       Quantity This column shows the number of lites to be optimised.

                                       Surface This column shows the total surface of the article to be optimised.

                                       Surface % This column shows the surface of the article in relation to the total
                                       surface of the batch. Example:




                                       The batch has a total surface of 67.86 sqm to be optimised. Article 104 A+W
                                       Float 4 mm has a surface of 16.35 sqm. These 16.35 sqm represent 24.10 %
                                       of the total surface.

                                          Fields in sections Orders and Items
                                          The fields in sections Orders and Items are the same as the identically
                                          named fields on tab Order selection which is why they are not described
                                          here again.


                                       Additional information
                                        Tutorial, “Detailed View for Batches” on page I-43
2.21 / 01-2017




                                        “Description of the fields in section Orders” on page I-104
                                        “Description of the fields in section Items” on page I-105




                 A+W Business Pro Production Manager                                                             I-119
                 Expert Mode                                                                Software Reference




                               Cutting
                               Production Manager > tab Details > tab Cutting




                               Fig. I-76    Tab Cutting on the right side of the screen


                               This tab shows detailed information regarding the selected lite including the
                               shape parameter an a graphic preview.

                               Description of fields

                               Quantity This field shows the quantity.

                               Width
                                This field shows the width of the lite.

                               Height This field shows the lite height.

                               Shape number If the lite is a shape, the shape number appears in this field.
2.21 / 01-2017




                               SN file If the lite is a free shape, the respective SN file appears in this field.




                 I-120                                                A+W Business Pro Production Manager
                 Software Reference                                                                      Expert Mode




                                       Shape parameter If the lite is a shape, the respective parameters (height,
                                       height 1, etc.) appear in this field.

                                       Shape trims If the lite is a shape, the parameters (height, height 1, etc.) ap-
                                       pear in this section.

                                       Preview The section shows a preview of the lite including dimensioning.

                                       Process Use this button to open dialog Edit cutting.


                                       Additional information
                                        Software Reference, “Edit Cutting” on page I-122
                                        Tutorial, “Tab Cutting” on page I-45
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-121
                 Expert Mode                                                                Software Reference




                               Edit Cutting
                               Production Manager > tab Details > tab Cutting > Button [Edit]




                               Fig. I-77    Edit cutting


                               This dialog shows a detailed cutting information regarding the selected lite in-
                               cluding the shape parameter and a graphic preview.

                               Description of fields

                               Quantity This field shows the quantity.

                               Width This field shows the width of the lite.

                               Height This field shows the lite height.

                               SN file If the lite is a free shape, the respective SN file appears in this field.

                               Shape parameter If the lite is a shape, the respective parameters (height,
                               height 1, etc.) appear in this field.
2.21 / 01-2017




                               Shape trims In case of shapes this section shows the respective trims for left,
                               right, top, and bottom.


                 I-122                                                A+W Business Pro Production Manager
                 Software Reference                                                                  Expert Mode




                                       Preview The section shows a preview of the lite including dimensioning. The
                                       dotted line shows the shape trims.


                                       Additional information
                                        Tutorial, “Tab Cutting” on page I-45
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                        I-123
                 Expert Mode                                                          Software Reference




                               Set Batch Status
                               Production Manager > tab Batch List > Select order > Open context menu >
                               Set Batch Status




                               Fig. I-78   Set batch status


                               This dialog serves to change the status of a batch.

                               Description of fields

                               New batch status Use the combo box to set the batch status to Completed.

                                  Change batch status manually
                                  For batches that consist e.g. only of purchased glass you can change the
                                  batch status manually.
2.21 / 01-2017




                 I-124                                             A+W Business Pro Production Manager
                 Software Reference                                                                         Expert Mode




                                         Machine Rescheduling
                                         Production Manager > tab Batch List > Select batch > Open context menu >
                                         Machine Rescheduling




                 Fig. I-79   Machine rescheduling


                                         Use this dialog to re-schedule products to other machines. The dialog consists
                                         of two sections::
                                         •   Current machine allocation
                                         •   Alternative machines
                                         The section Current machine allocation shows a tree structure with the follow-
                                         ing levels:
                                         •   Machine
                                         •   Work process
                                         •   Product
                                         The section Alternativ machines offers the corresponding alternatives. This
                                         section serves e.g. for texts Following texts are possible:
                                         •   Please select a Product for machine rescheduling: In this case you chose
                                             the wrong level.
                                         •   According to the batch status a machine rescheduling is not possible: In
                                             this case the batch has already a status in which rescheduling is not pos-
                                             sible anymore.
                                         •   No alternatives available for rescheduling: It is not possible to reschedule
                                             the product, since no alternatives are available.

                                         Description of buttons
2.21 / 01-2017




                                         Rescheduling Press this button to reschedule the product to the selected
                                         machine.

                                         Close Press this button to close the dialog.
                 A+W Business Pro Production Manager                                                               I-125
                 Expert Mode                                                                        Software Reference




                                         Optimization Manager
                                         Production manager > tab Optimization manager




                 Fig. I-80   Optimization manager


                                         This dialog displays the batches that were transferred to the optimization man-
                                         ager. The dialog consists of four sections. The batches are displayed at the up-
                                         per left. Adjacent to the right are all glass types of all batches that were
                                         transferred to the optimization manager. The batches in which the glass type
                                         is present is displayed if a glass type is opened. The respective optimizations
                                         and the overall result are displayed in the lower section.

                                         Description of fields in section Batches

                                         Batch number This column shows the batch number you have selected on
                                         tab Batch list.

                                         Creation date This field shows the date when the batch has been created.

                                         Status Show the batch status.
2.21 / 01-2017




                                         Description This field shows the batch description.




                 I-126                                                        A+W Business Pro Production Manager
                 Software Reference                                                                            Expert Mode




                                       Rack organization This is where the rack organization that you have chosen
                                       at batch creation is shown.

                                       IG This field shows the quantity of IG included in the batch.

                                       LG This field shows the quantity of LAMI included in the batch.

                                       TG This field shows the quantity of TG included in the batch.

                                       Glass (single and processed) This field shows the single and processed
                                       glass included in the batch.

                                       Factor for the rack depth This is where the factor that you have chosen at
                                       batch creation is shown.

                                       Description of fields in section Glass type
                                       This section shows all glass types included in the batch. When you expand the
                                       entry for the glass type you will be provided with information on the quantity,
                                       the surface, and the batch.

                                          Fields in section Optimizations and total result
                                          The fields in section optimizations and Total result are the same as in the
                                          identically named sections in Standard mode which is why we are not going
                                          to explain them here again.


                                       Additional information
                                        Tutorial, “Optimization Manager” on page I-49
                                        “Description of fields in section optimizations” on page I-100
                                        “Description of the fields in section Overall Result” on page I-100
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                 I-127
                 Expert Mode                                                                          Software Reference




                                             Abort Optimization
                                             Production Manager > tab Optimization Manager > Execute > Optimizations >
                                             [Cancel]




                 Fig. I-81   Optimizations


                                             This dialog shows the optimizations regarding the corresponding batches. To
                                             abort the optimization click on button [Cancel].


                                             Additional information
                                              Tutorial, “Abort Optimization” on page I-55
2.21 / 01-2017




                 I-128                                                              A+W Business Pro Production Manager
                 Software Reference                                                                      Expert Mode




                                          Temporary Optimization
                                          Production Manager > tab Optimization manager > Details




                 Fig. I-82   Temporary optimization


                                          This dialog shows the detailed view for an optimization variant. It will be
                                          opened from the Optimization Manager via the context menu, Detailed View
                                          entry and consists of several sections

                                          Description of the fields in section Rack

                                          Batch number The batch number that you selected on the Optimization
                                          manager tab is displayed here.

                                          Rack The rack number on which the lite was placed is shown here.

                                          Rack type The rack type on which the lite was placed is shown here. Possible
                                          values are:
                                          • A Rack
                                          • Harp rack
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-129
                 Expert Mode                                                            Software Reference




                               Log. rack This is were the logical rack is displayed.

                               Quantity This is were the number of lites on the rack is displayed.

                               Description of fields in section Batches

                               Batch number This is were the batch numbers of the batches are displayed
                               that are involved in the optimization.

                               Creation date This field shows the date when the batch has been created.

                               Name This field shows the batch description.

                               Description of the fields in section Stocksizes

                               Quantity This column shows the number of stock sizes of this size that were
                               used for the optimization.

                               Width This column shows the width of the stock size.

                               Height This column shows the height of the stock size.

                               Surface This column shows the surface of the stock size in square meters.

                               Priority This column shows the priority of the stock size.

                               Description of the fields in section Pattern

                               Pattern This column shows the individual patterns.

                               Optimization group This column shows the optimization groups.

                               Quantity This column shows how often this pattern must be cut.

                               Width This column shows the width of the pattern.

                               Height This column shows the height of the pattern.


                               Additional information
                                Tutorial, “Temporary Optimization” on page I-52
2.21 / 01-2017




                 I-130                                               A+W Business Pro Production Manager
                 Software Reference                                                                           Expert Mode




                                          Optimization Overview
                                          Production Manager > tab Optimization Overview




                 Fig. I-83   optimization overview


                                          This dialog shows the optimizations which have been run for the individual
                                          glass types. Various selection criteria can be used to keep the contents of this
                                          list at bay. You can view the details of a selected glass type (detailed view) and
                                          start the output (machine output, reports). In addition, you can cancel optimi-
                                          zations, debit stockplates and re-process patterns.

                                          Description of fields in section Selection Criteria

                                          Optimization The from to fields can be used to display optimizations by
                                          number. The fields also serve for limiting the displayed optimizations in order
                                          to keep track of things.

                                          Creation date This field can be used for displaying the optimizations by the
                                          date on which they were created. The fields also serve for limiting the dis-
                                          played optimizations in order to keep track of things.
2.21 / 01-2017




                                          Batch number The from to fields can be used to display optimizations that
                                          are assigned to one or more optimizations.



                 A+W Business Pro Production Manager                                                                  I-131
                 Expert Mode                                                             Software Reference




                               Description of the fields in section optimization

                               Optimization This column shows the optimization number.

                               Optimization mode This field shows the the optimization mode used. Possi-
                               ble values are:
                               • XOPT
                               • XOPTS

                               Creation date This field shows when the optimization was created.

                               Glass type This field shows the glass type that was optimized.

                               Cutting table Here, you see the table on which the glass shall be cut.

                               Batches This field shows the batch numbers that have lites in the optimiza-
                               tion.

                               Status The status is displayed in this field.

                               Quantity This column shows the total surface of the article to be optimized.

                               Surface This column shows the total surface of the article to be optimised.

                               Result This field shows the optimization result for the glass type in question.


                               Additional information
                                Tutorial, “Optimization Overview” on page I-56
2.21 / 01-2017




                 I-132                                                A+W Business Pro Production Manager
                 Software Reference                                                                          Expert Mode




                                           Optimization Detailed View
                                           Production Manager > Optimization Overview Tab > Detailed View




                 Fig. I-84   Optimization detailed view


                                           This dialog shows the detailed view for an optimization. It will be opened from
                                           the Optimization Overview via the context menu, Detailed View entry and con-
                                           sists of several sections
                                           The content of this dialog is identical to the content of the Temporary Optimi-
                                           zation dialog, which is why it will not be explained again at this point.
                                            “Temporary Optimization” on page I-129


                                           Additional information
                                            Tutorial, “Temporary Optimization” on page I-52
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                I-133
                 Expert Mode                                                                  Software Reference




                               Output
                               Production Manager > tab Output




                               Fig. I-85     Output


                               All output, no matter if on paper or in the shape of a file, is started from this tab.
                               The dialog is accessible directly (tab Output), from the tab Batch list, and from
                               the tab Optimization overview.

                               Description of fields in the Batches section (from the batch over-
                               view)

                               Batch number This column shows the batch number you have selected on
                               tab Batch list.

                               Creation date This field shows the date when the batch has been created.

                               User This field shows who created the batch.

                               Description This field shows the batch description.

                               Rack organization This is where the rack organization that you have chosen
                               at batch creation is shown.
2.21 / 01-2017




                 I-134                                                 A+W Business Pro Production Manager
                 Software Reference                                                                          Expert Mode




                                       Status Show the batch status.

                                       IG This field shows the quantity of IG included in the batch.

                                       LG This field shows the quantity of LAMI included in the batch.

                                       Toughened glass This field shows the quantity of TG included in the batch.

                                       Glass This shows the individual lites and the processed lites included in the
                                       batch.

                                       Message This is where the message text is shown. The following texts are
                                       possible:

                                       .
                                       Symbol      Explanation

                                                   Output is incorrect e.g. because the batch has not been
                                                   completely optimised.

                                                   The output is correct.



                                       Description of fields in the Optimization section (from optimiza-
                                       tions)

                                       Optimization This column shows the optimization number.

                                       Creation date This field shows when the optimization was created.

                                       Glass type This field shows the glass type that was optimized.

                                       Mode This field shows the the optimization mode used.

                                       Cutting table Here, you see the table on which the glass shall be cut.

                                       Batches This field shows the batch numbers.

                                       Status The status is displayed in this field.

                                       Quantity This column shows the total surface of the article to be optimized.

                                       Surface This column shows the total surface of the optimized articles.

                                       Result This field shows the optimization result for the glass type in question.

                                       Description of fields in section Reports

                                       Name This column shows the name of the report, e.g. production list, rack list,
                                       etc.
2.21 / 01-2017




                                       Printer This field shows the printer that provides the print out.

                                       Copies This field shows how many copies were issued.


                 A+W Business Pro Production Manager                                                               I-135
                 Expert Mode                                                            Software Reference




                               Settings The column offers context menus depending on the report type.

                               Message The icon displayed in this columns provides information about the
                               status of the output.

                               Description of fields in the section Machine

                               Machine This column shows the machine for which the machine code will be
                               issued.

                               Output This field shows the the directory in which the machine code is saved.


                               Additional information
                                Tutorial, “Output” on page I-60
2.21 / 01-2017




                 I-136                                             A+W Business Pro Production Manager
                 Software Reference                                                                         Expert Mode




                                       Printer Settings
                                       Production Manager > tab Output > Print Settings




                                       Fig. I-86    Printer settings


                                       This dialog is used to establish the settings for the following output:
                                       •   Labels
                                       •   Cutting Plan
                                       •   Printer

                                       Description of fields in the section Labels

                                       Series starting with This field defines the minimum quantity for a series. The
                                       radio buttons can be used to define whether a label shall be printed per item
                                       or per label. In connection with the version One label per unit, you can use the
                                       following field to define the number of units for which a label shall be printed.

                                       Description of the fields in section Cutting Plan

                                       Print all All cutting plans are printed if you activate this radio button.

                                       Print last page Only the last page of the cutting plan will be printed if this ra-
                                       dio button is activated.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                I-137
                 Expert Mode                                                          Software Reference




                               Description of fields in the section Printer

                               Reports Use the combo box to select the printer on which the reports must
                               be printed.

                               Labels Use the combo box to select the printer on which the labels must be
                               printed.

                               Copies This is where you can set the number of copies that must be printed
                               as a default.

                               Description of buttons

                               Save The global print settings can be saved through this button. They are
                               now always available and must not be re-established for each print.
2.21 / 01-2017




                 I-138                                            A+W Business Pro Production Manager
                 Software Reference                                                                        Expert Mode




                                       Search Order
                                       Information > Order




                                       Fig. I-87    Search order


                                       This dialog allows to search orders. There are several search criteria for this
                                       purpose. The dialog consists of different sections. In section Selection criteria,
                                       you can use the Order number manager, the Number manager or the Custom-
                                       er to select the required data.

                                       Description of fields in section Selection Criteria

                                       Order number After the radio button is activated, you can enter the order
                                       number in the field behind.

                                       Number manager After ticking the radio button you can access the corre-
                                       sponding data in the combo box. The combo box offers all entries you have
                                       made in the number manager section.

                                       Customer After ticking the radio button you can access the corresponding
                                       data in the combo box. The combo box contains all customers for which orders
2.21 / 01-2017




                                       exist in the capacity planning of A+W Business Pro.




                 A+W Business Pro Production Manager                                                              I-139
                 Expert Mode                                                                   Software Reference




                               The order and Item sections
                               The sections Orders and Items are the same as the identically named fields
                               on tab Order selection which is why they are not described here again.
                                “Description of the fields in section Orders” on page I-104
                                “Description of the fields in section Items” on page I-105


                               Additional information
                                Tutorial, “Order Selection” on page I-26
2.21 / 01-2017




                 I-140                                                 A+W Business Pro Production Manager
Production Manager              I

                     Section Index




             A+W Business Pro
                 Section Index                                                                Index




                 Index
                 A                                          – Product I-119
                 Abort optimization   I-128                 – Product description 1 I-119
                                                            – Quantity I-119
                                                            – Rack organization I-118
                 B
                                                            – Status I-119
                 Batch
                                                            – Surface I-119
                 – Batch overview I-116
                                                            – Surface % I-119
                 Batch creation
                                                            Detailed view for batches I-118
                 – Overview I-38, I-47, I-60
                                                            Display conventions I-11
                 Batch overview I-116
                                                            Documentation
                 – Batch number I-116, I-117
                                                            – Types I-10
                 – Creation date I-116, I-117
                 – Description I-117
                 – Factor for rack depth I-117              E
                 – Glass (single and processed)     I-117   Edit cutting
                 – IG I-117                                 – Height I-122
                 – LAMI I-117                               – Quantity I-122
                 – Rack organization I-117                  – SN file I-122
                 – Status I-117                             – Width I-122
                 – TG I-117                                 Enter rejects
                 Batches                                    – Item I-113
                 – Detailed view I-118                      – Order I-113
                 – Machine load transfer I-125              – Place I-113
                                                            – Quantity I-113
                                                            – Reason I-113
                 C
                                                            Expert mode
                 Criteria I-91
                                                            – Overview I-24, I-67
                 Criterion
                 – Grouping I-94
                 – Groups sorted I-94                       F
                 – Name I-91                                Find order
                 – Sorting key I-91                         – Customer I-139
                 – Sorting within the groups I-94           – Number manager I-139
                 – Type I-93                                – Order number I-139
                 Cutting
                 – Button edit I-121                        G
                 – Height I-120                             Grouping
                 – Preview I-121, I-123                     – Save view    I-107, I-114
                 – Quantity I-120
                 – Shape number I-120
                                                            L
                 – Shape parameter I-121, I-122
                                                            Logical rack
                 – Shape trims I-121, I-122
                                                            – Name I-93
                 – SN file I-120
                 – Width I-120
                                                            M
                                                            Machine load transfer I-125
                 D
                                                            Master data
                 Detailed view batch
2.21 / 01-2017




                                                            – General I-97, I-102
                 – Creation date I-118
                                                            Module
                 – Description I-118
                                                            – Function I-9
                 – Factor for rack depth I-119


                 A+W Business Pro Production Manager                                          I-143
                 Section Index                                                                       Index




                 N                                         – Glass (items) I-106
                 Name of view I-107                        – Header part type (items) I-106
                 New batch                                 – Header parts (items) I-106
                 – Batch number I-114                      – Height (items) I-105
                 – Bezeichnung I-114                       – Item number (items) I-105
                 – Detailed scheduling I-115               – Muntins (items) I-106
                 – Factor for rack depth I-114             – Number manager I-103
                 – Optimization manager I-115              – Offset (items) I-106
                 – Output I-115                            – Order number I-104
                 – Rack organization I-114                 – Order number (items) I-105
                 – Total manual cutting I-115              – Priority I-105
                 – Unlimited rack depth I-115              – Procurement type (items) I-106
                                                           – Product I-104
                                                           – Product (items) I-105
                 O
                                                           – Product description 1 I-104
                 Optimization detailed view I-129, I-133
                                                           – Product description 1/2 (items) I-105
                 Optimization manager
                                                           – Product group (items) I-106
                 – Batch description I-126
                                                           – Product type (items) I-106
                 – Batch number I-126
                                                           – Purchase date I-104
                 – Creation date I-126
                                                           – Quantity I-104
                 – Factor for rack depth I-127
                                                           – Quantity (items) I-105
                 – Glass (single and processed) I-127
                                                           – Representative I-104
                 – IG I-127
                                                           – Route I-105
                 – LAMI I-127
                                                           – Serial meter (items) I-105
                 – Rack organization I-127
                                                           – Shape number (items) I-105
                 – Status I-126
                                                           – Shipping date I-104
                 – TG I-127
                                                           – Short description (items) I-105
                 optimization manager I-126
                                                           – Status I-104
                 Optimization overview I-131
                                                           – Surface I-104
                 – Batch number I-131
                                                           – Surface (items) I-105
                 – Batches I-132
                                                           – Surface in relation I-104
                 – Creation date I-131, I-132
                                                           – Width (items) I-105
                 – Cutting table I-132
                                                           – Work process I-103, I-104
                 – Glass type I-132
                                                           Output
                 – Optimization I-131, I-132
                                                           – Batch description I-134
                 – Optimization mode I-132
                                                           – Batch number I-134
                 – Quantity I-132
                                                           – Batches I-135
                 – Result I-132
                                                           – Creation date I-134
                 – Status I-132
                                                           – Creation date (optimization) I-135
                 – Surface I-132
                                                           – Cutting table I-135
                 Order selection
                                                           – Glass I-135
                 – AIR (items) I-106
                                                           – Glass type I-135
                 – BOM item (items) I-105
                                                           – IG I-135
                 – Consultant I-104
                                                           – LAMI I-135
                 – Customer data I-105
                                                           – Machine I-136
                 – Customer number I-104
                                                           – Message I-135, I-136
                 – Date from/to I-103
                                                           – Mode I-135
                 – Delivery date I-105
                                                           – Name of report I-135
                 – Desired date I-105
                                                           – Optimization number I-135
                 – Entry date I-104
2.21 / 01-2017




                                                           – Printer I-135
                 – Entry date (items) I-105
                                                           – Quantity I-135
                 – Foils (items) I-106
                                                           – Rack organization I-134
                 – Gas filling (items) I-106
                                                           – Result (optimizations) I-135


                 A+W Business Pro Production Manager                                                 I-144
                 Index                                                                Section Index




                 – Settings I-136                  Rejects
                 – Status I-135                    – AIR (items) I-111
                 – Surface (optimizations) I-135   – Batch I-110
                 – TG I-135                        – BOM item I-110
                 – User I-134                      – Foils (items) I-111
                 Overview                          – Gas filling (items) I-111
                 – Expert mode I-24, I-67          – Header part type (items) I-111
                                                   – Header parts (items) I-111
                 P                                 – Height (items) I-110
                 Printer settings I-137            – Item number I-110
                 – Copies I-138                    – Muntins (items) I-111
                 – Print all I-137                 – Offset (items) I-111
                 – Print last page I-137           – Order number I-110
                 – Printer for labels I-138        – Processings I-112
                 – Printer for reports I-138       – Procurement type (items) I-111
                 – Series from I-137               – Product (items) I-110
                 Product                           – Product description 1/2 (items) I-110
                 – Height I-108                    – Product group (items) I-111
                 – Preview I-109                   – Product type (items) I-111
                 – Quantity I-108                  – Production date I-112
                 – Shape number I-108              – Quantity (items) I-110
                 – Shape parameter I-108           – Serial meter (items) I-111
                 – SN file I-108                   – Shape number (items) I-111
                 – Width I-108                     – Sheets (items) I-111
                                                   – Short description (items) I-110
                                                   – Sqft. (items) I-110
                 R                                 – Sub-item number I-110, I-113
                 Rack group                        – Width (items) I-110
                 – Name I-95
                 – Sorting key I-95
                 – Sorting key preview I-95        S
                 Rack Organization I-88            Save view I-107, I-114
                 Rack organization                 – Name I-107
                 – Check sequence I-89             Set batch status I-124
                 – Default I-89                    – New I-124
                 – Default (selection) I-88        Sorting key
                 – Formula I-89                    – Formula I-96
                 – Logical rack I-89               – Name I-96
                 – Name I-89                       – Sorting I-96
                 – Name (selection) I-88           Standard mode
                 – Number of lites per slot I-90   – Batch number I-99
                 – Number of slots I-90            – Batches (optimizations) I-100
                 – Physical rack I-90              – Cutting table (optimizations) I-100
                 – Production sequence I-89        – Desription I-99
                 – Rack depth I-90                 – Factor for rack depth I-99
                 – Rack group I-89                 – Glass type (optimization) I-100
                 – Rack no. current I-90           – Number manager I-99
                 – Rack no. from I-89              – Number of A racks (total result) I-101
                 – Rack no. to I-90                – Number of harp racks (total result) I-101
                 – Type I-89                       – Number of variants I-99
2.21 / 01-2017




                 Racks                             – Outputs I-100
                 – Logical rack I-93, I-95         – Quantity (optimizations) I-100
                 – Sorting key I-96                – Rack organization I-99



                 I-145                                      A+W Business Pro Production Manager
                 Section Index                                Index




                 – Rack organization (total result)   I-101
                 – Result I-101
                 – Result (optimizations) I-100
                 – Status I-99
                 – Surface (optimizations) I-100
                 – Unlimited rack depth I-99
                 – Variant (total result) I-100
                 – Waste (total result) I-101

                 T
                 Temporary optimization
                 – Batch number I-129, I-130
                 – Creation date I-130
                 – Description I-130
                 – Height (shape) I-130
                 – Height (stock sizes) I-130
                 – Log. rack I-130
                 – Optimization group I-130
                 – Priority I-130
                 – Quantity I-130
                 – Quantity (shape) I-130
                 – Quantity (stock sizes) I-130
                 – Rack I-129
                 – Rack type I-129
                 – Shape I-130
                 – Surface I-130
                 – Widht (shape) I-130
                 – Width (stock sizes) I-130
2.21 / 01-2017




                 A+W Business Pro Production Manager          I-146

