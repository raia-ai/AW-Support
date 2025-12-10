---
title: "EN CONFIG A+W Production"
category: "configuration"
product: "A+W Production"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W Production"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration   A+W Production                                                                   english       A+W Software GmbH   EN-CONFIG-A+W Production.docx   - -INTERNAL-                                                               1 Change history   Date         Author     Remarks                                               Version 2018-05-11   DLA        Macro resolution, FIX filter                          1.0 2018-06-07   DLA        CrystalReports"
source_file: "EN-CONFIG-A+W Production.pdf"
---


# EN CONFIG A+W Production

        Configuration


A+W Production




                                                              english




  A+W Software GmbH   EN-CONFIG-A+W Production.docx   - -INTERNAL-
                                                              1
Change history


Date         Author     Remarks                                               Version
2018-05-11   DLA        Macro resolution, FIX filter                          1.0
2018-06-07   DLA        CrystalReports                                        1.1
2018-06-11   JMO        O4P                                                   1.2
2018-06-12   JMO        Extension O4P – SPCall                                1.3
2018-07-30   DLA        Configure sketch                                      1.4
2018-08-02   DLA        Reports chapter                                       1.5
2018-06-12   DLA        Release of several instances/furnace bed optis        1.6
2018-08-10   PK         Foil preview in the PT LG_Assembly                    1.7
2018-09-21   DLA        VIEWs + AWPLogoTableEditor                            1.8
2018-09-27   DLA        Release with cancelled items                          1.9
2018-09-27   DLA        AUW functions                                         1.10
2018-10-08   DLA        Existing English texts translated back to German      1.11
2018-10-08   DLA        Document links                                        1.12
2019-02-06   RI         Background printing in booking                        1.13
2019-02-08   DLA        Multi-site                                            1.14
2019-02-19   JMO        Update and new prerequisite label for capacity        1.15
2019-02-22   DLA        Adjustments print booking                             1.16
2019-04-05   DLA        Cancellation of orders                                1.17
2019-05-07   JMO        PrintMode feature added                               1.18
2019-05-08   DLA        Parameter Administrator                               1.19
2019-05-16   RI         Specifying environment for scripts and reports        1.20
2019-05-31   DLA        Archiving                                             1.21
2019-07-29   SFR        Section 6.3.   Opening         the   A+W   Production 1.22
                        Terminal QA with [F1]
2019-08-12   SFR, OSO   Merge IoT configuration instructions into this 1.23
                        document (IoT Smart Trace basic configuration)
2019-08-20   SFR        Restructuring of the subchapter for A+W Production 1.24
                        Terminal, new: PT order - section Automatic
                        Generation of a Batch Number
2019-09-13   SFR        New: Production Terminal IG-Out,              section 1.25
                        incorporating the LoadRackDialog




A+W Software GmbH             EN-CONFIG-A+W Production.docx                             2
Date         Author     Remarks                                                Version
2019-09-16   SFR        New: A+W Realtime Optimizer, section Multiple 1.26
                        User Login
2019-09-20   OSO        Barcoding area added                                   1.27
2019-09-23   SFR, STM   New: Filtering the display of the racks on the dialog 1.28
                        by allowed tables
2019-10-01   SFR        Layout fine-tuning                                     1.29
2019-10-01   RI         Production Terminal IG-In – PMO data                   1.30
2019-10-09   DLA        ReolveMakroProcessing chapter broken down since 1.31
                        in the previous version, the assignment of the titles
                        to the individual chapters was not right.
2019-10-14   OSO        Scanner configuration added under A+W Production 1.32
                        Terminal IG-IN
2019-10-15   OSO        Scanner configuration (optional) added under A+W 1.33
                        Production Terminal IG-ASSEMBLY
2019-10-15   SFR        Replacement of the             figures   with   English 1.34
                        screenshots, formatting
2019-10-17   OSO        Addition of note the quality characteristic for 1.35
                        Vipotron must be entered in apostrophes in the
                        configuration
2019-10-18   OSO        Screenshot replaced for Figure 8-11                    1.36
2019-10-21   SFR        Transfer of PMO data to Production Terminal IG-In 1.37
                        reworked and completed.
2019-10-24   OSO        Addition of the information the lot types must be 1.38
                        specified for the various stations
2019-10-29   SFR        Reworking of the subsections for the Production 1.39
                        Terminal IG-Out and IG-Assembly
2019-11-01   OSO        Addition of the area entry of additional quantities    1.40
2019-11-04   OSO        Addition of parts precise entry of additional 1.41
                        quantities and entry of additional quantities in A+W
                        Business
2019-11-11   SFR        Fine-tuning of Realtime Optimizer section              1.42
2019-11-25   SFR        Formatting of values in Production Terminal, specific 1.43
                        and global
2018-11-26   PK         Reworking of the surplus and additional quantities     1.44
2019-12-09   STM        Part type filter in PT TG-In                           1.45
2019-12-16   STM        Addition to rack feedback                              1.46
2020-01-30   SFR        New section: checking of the rack for existence in 1.47
                        the A+W Rack Manager



A+W Software GmbH            EN-CONFIG-A+W Production.docx                               3
Date         Author   Remarks                                              Version
2020-02-03   OSO      Addition of configuration scanner connection to 1.48
                      Production Terminal (8.1.5)
2020-02-13   OSO      Addition of A+W Production Terminal Processing       1.49
2020-03-19   STM      SP for turning in PT IG-In                           1.50
2020-04-30   PK       Installation after ERP item                          1.51
2020-05-28   OSO      Addition reporting from goods receipt                1.52
2020-06-03   OSO      Addition SN driver call for each lite                1.53
2020-07-21   PK       Automatic archiving                                  1.54
2020-07-24   STM      Display of additional parts in Production Terminal   1.55
2020-09-23   PK       Performance Counter                                  1.56
2020-10-19   PK       Break with incomplete installed message              1.57
2020-11-30   STM      Production Terminal TG-Out with several scanners     1.58
2021-01-28   DLA      Archiving of SKIZZEN                                 1.59
2021-02-23   PK       Expanded archiving                                   1.60
2021-02-23   PK       Archiving via customizing                            1.61
2021-03-24   STM      Addition to the Performance Counter                  1.62
2021-04-27   RI       Production Terminal Tracing                          1.63
2021-07-07   STM      Rack feedback extended workbench                     1.64
2022-05-23   STM      Timestamp of bookings                                1.65
2023-10-02   STM      Messages to the Smart Factory                        1.66
2023-11-09   STM      Remake handling                                      1.67
2024-01-02   EB       Production monitor (document content from mar- 1.68
                      ket solution)
2024-01-03   EB       Chapter A+W Capacity (document content from 1.69
                      market solution)
2024-01-03   EB       Scheduling remakes (document content from mar- 1.70
                      ket solution)
2024-04-03   JMO      O4P worksteps "AfterWorks" and "AfterWorksParal- 1.71
                      lel" added.
2024-04-25   JMO      Late transfer of production-irrelevant data          1.72




A+W Software GmbH         EN-CONFIG-A+W Production.docx                              4
Content

1.   Scheduling                                                         10
     1.1. Orders4Production                                             10
          1.1.1. Set-up                                                 10
          1.1.2. Description of the work step                           11
          1.1.3. ResolveMacroProcessings                                16
     1.2. Cancellation of orders                                        18
     1.3. Later transfer of production-irrelevant data                  18
          1.3.1. Changing order data                                    19
          1.3.2. Change of item data                                    21
2.   Rough Scheduling                                                   25
     2.1. FIX filter                                                    25
          2.1.1. How can a FIX filter be configured?                    25
          2.1.2. How is a FIX filter linked to a display?               25
          2.1.3. How can you see that your FIX filter is active?        25
          2.1.4. FIX filter for the standard displays                   26
          2.1.5. Known Problems                                         26
     2.2. VIEW database for rough scheduling views                      26
     2.3. Additional and surplus quantities                             27
          2.3.1. Commercial surplus                                     27
          2.3.2. Technical surplus                                      28
          2.3.3. Additional quantities                                  28
          2.3.4. Surplus and additional quantities in the database      28
          2.3.5. Additional and surplus quantities in the OrderXML      29
          2.3.6. Reporting of additional and surplus quantities         29
          2.3.7. Entry of additional and surplus quantities             30
          2.3.8. A+W Production precise to the part                     32
          2.3.9. A+W Production multiples                               33
          2.3.10. A+W Business                                          34
3.   Batch release                                                      36
     3.1. Executing the release of several instances                    36
          3.1.1. Synchronization of printing across several instances   37
     3.2. Release of batches with cancelled items                       38
     3.3. Specifying environment for scripts and reports                38
4.   Crystal Reports                                                    40
     4.1. Parameters for control                                        40
     4.2. Report call directly via PPS WebService                       41
     4.3. Generate true to scale sketches                               41
          4.3.1. Display of the step profile                            44
          4.3.2. Generate turned sketches                               45
     4.4. Printing customer logos                                       45
          4.4.1. Adding a logo                                          47
          4.4.2. Editing a logo                                         48
          4.4.3. Deleting a logo                                        48
          4.4.4. Saving a logo                                          48
5.   A+W Capacity                                                       50
     5.1. How to work with A+W Capacity for scheduling                  50


A+W Software GmbH                  EN-CONFIG-A+W Production.docx             5
          5.1.1. Switch position regular order                   50
          5.1.2. Switch position rush order                      51
          5.1.3. Switch position high-priority order             52
     5.2. Collected information                                  53
          5.2.1. Manual reprocessing (red card)                  53
          5.2.2. Processing chains                               53
          5.2.3. Alternative machine                             53
          5.2.4. CAPA_SETTING/MINIMUM_NORMALTRANSITIONS switch   54
6.   Feedback                                                    55
     6.1. Activation                                             56
     6.2. Reporting of batch status                              56
     6.3. Reporting of production status                         57
     6.4. Reporting of intermediate production status            57
     6.5. Report of rack allocations                             58
           6.5.1. Rack feedback with extended workbench          59
     6.6. Reporting of stock lites                               61
     6.7. Reporting from goods receipt                           62
     6.8. A+W Business                                           63
           6.8.1. Configuration                                  63
           6.8.2. FS_POOL                                        64
           6.8.3. Production overview                            65
           6.8.4. Delivered racks                                67
     6.9. A+W Enterprise                                         67
           6.9.1. Configuration                                  67
     6.10. A+W Cantor                                            69
     6.11. A+W Cantor CIM                                        70
           6.11.1. Configuration in A+W Cantor                   72
           6.11.2. Configuration in A+W Production               72
           6.11.3. Result                                        72
7.   A+W Realtime Optimizer                                      75
     7.1. Multiple user login                                    75
8.   A+W Barcoding                                               76
     8.1. Background printing and e-mail dispatch                76
     8.2. 15-digit Gestellpool Europe barcodes                   78
          8.2.1. Configuration in A+W Production                 78
          8.2.2. Configuration in A+W Smart Companion            80
     8.3. Breakage booking with incomplete assembly message      82
     8.4. Consideration of the timestamp of bookings             82
     8.5. Messages from bookings to the Smart Factory            83
          8.5.1. Lite at registration point                      84
          8.5.2. Booking of the processing "packed" or "sent"    84
          8.5.3. Fraction calculations                           84
          8.5.4. Booking of a state of the type "reuse"          84
9.   Remake handling                                             87
     9.1. Mode of Operation / Operation                          87
          9.1.1. Booking of a partial defect                     87
     9.2. Configuration                                          87
          9.2.1. A+W Production parameters                       87


A+W Software GmbH                EN-CONFIG-A+W Production.docx        6
         9.2.2. PDC master data                                                          88
         9.2.3. Parameter Administrator dialog                                           91
    9.3. Operation of the remake handling                                                94
         9.3.1. Remake handling                                                          94
         9.3.2. Display                                                                  94
         9.3.3. Macros – the rough decision                                              97
         9.3.4. Details – the fine-tuning                                                98
         9.3.5. Assignment of real components (starting with AWP5.4)                    100
         9.3.6. Additional buttons                                                      103
    9.4. Direct booking from the Production Terminal                                    104
    9.5. Database content                                                               104
         9.5.1. Pool_Pos                                                                104
         9.5.2. Pool_teile                                                              105
         9.5.3. Pool_bearbeit                                                           106
         9.5.4. Awbar_Bearbeit                                                          108
         9.5.5. Awbar_booking                                                           108
         9.5.6. Awbar_teile                                                             109
10. A+W Production Terminal                                                             110
    10.1. Functions in all A+W Production Terminals                                     110
          10.1.1. Opening the A+W Production Terminal QA with <F1>                      110
          10.1.2. Formatting of all areas, lengths, and thicknesses                     111
          10.1.3. Formatting of individual table columns                                111
          10.1.4. Checking of the rack for existence in the A+W Rack Manager            112
          10.1.5. Configuration scanner connection to A+W Production Terminal           114
          10.1.6. Performance Counter configuration                                     115
          10.1.7. Tracing                                                               118
    10.2. A+W Production Terminal TG-In                                                 118
          10.2.1. Furnace bed optimization                                              118
          10.2.2. Part type filter                                                      120
    10.3. A+W Production Terminal TG-Out                                                122
          10.3.1. Several scanners                                                      122
    10.4. A+W Production Terminal LG-IN                                                 123
          10.4.1. Installation after ERP item                                           123
    10.5. A+W Production Terminal LG-Assembly                                           123
          10.5.1. Foil preview                                                          123
    10.6. A+W Production Terminal Order                                                 125
          10.6.1. Automatic generation of a batch number                                125
    10.7. A+W Production Terminal IG-In                                                 126
          10.7.1. Transfer of PMO data to the Panorama                                  126
          10.7.2. Transfer of PMO data via XML file                                     126
          10.7.3. Sending of information to quality scanner                             127
          10.7.4. Call of an SP for turning on a turning station                        128
          10.7.5. Display of additional parts in the detail list                        128
    10.8. A+W Production Terminal IG-Assembly                                           130
          10.8.1. Quality scanner configuration                                         130
          10.8.2. Display of additional parts in the detail list                        131
    10.9. A+W Production Terminal IG-Out                                                132
          10.9.1. Dialog for calling up racks from a sorting system (AUW_UnloadRacks)   132
    10.10.     A+W Production Terminal Processing                                       136
          10.10.1. Selection of a fine planning rack                                    136


A+W Software GmbH                EN-CONFIG-A+W Production.docx                                7
          10.10.2.   SN driver call for all lites                     137
11. A+W Production Terminal QA                                        138
12. AUW functions                                                     139
    12.1. Database VIEWs                                              139
          12.1.1. AUW_POOL_TEILE                                      139
          12.1.2. AUW_POOL_SZR                                        139
          12.1.3. AUW_AE_INTPOS                                       139
          12.1.4. AUW_AE_INTPOS_BOM                                   140
          12.1.5. AUW_AE_INTPOS_PROC                                  140
          12.1.6. AUW_REGPT_NEXT                                      141
          12.1.7. AUW_CAPA_OVERVIEW                                   141
          12.1.8. AUW_WIP                                             141
    12.2. Functions and procedures                                    141
          12.2.1. AUW_GETTEXT                                         141
          12.2.2. AUW_POOL_NAME                                       142
          12.2.3. AUW_POOL_PAINT                                      142
          12.2.4. AUW_POOL_SUBPART                                    143
          12.2.5. AUW_PRINT_REMAKE                                    144
    12.3. Table AUW_SETTINGS                                          144
13. Multi-site                                                        146
    13.1. Preparation                                                 146
    13.2. Configuration                                               146
    13.3. Starting the applications                                   152
    13.4. Special features                                            153
    13.5. Update                                                      153
14. Archiving                                                         155
    14.1. Manual archiving                                            155
    14.2. Automatic archiving                                         157
    14.3. Expanded automatic archiving                                158
          14.3.1. How "standard method" works                         158
          14.3.2. How "expanded method" works                         159
    14.4. Archiving via customizing                                   159
    14.5. How is archiving done?                                      160
    14.6. Archive databases                                           160
    14.7. Tables used                                                 161
    14.8. Archiving the SKIZZEN table                                 162
15. A+W IoT Smart Trace                                               163
    15.1. Basic configuration                                         163
          15.1.1. Gateway connection settings                         163
          15.1.2. PDC configuration                                   164
    15.2. Sending reports                                             165
16. Other functions                                                   167
    16.1. Parameter Administrator                                     167
    16.2. Document links                                              168
          16.2.1. A+W Production                                      168
          16.2.2. A+W Production Terminal                             169
          16.2.3. Entry in A+W Business                               170


A+W Software GmbH                     EN-CONFIG-A+W Production.docx         8
17. Production Monitor                                           174
    17.1. Overview                                               174
    17.2. Detail view                                            174
    17.3. Backlogs and workload                                  175
          17.3.1. Display                                        175
          17.3.2. Workload                                       177
          17.3.3. Known problems (in A+W Production 5.1/5.2):    178
    17.4. Manual completion notification                         178
          17.4.1. The process                                    178
          17.4.2. Limitations                                    179
          17.4.3. Known Problems                                 180
18. Table of Figures                                             181




A+W Software GmbH                EN-CONFIG-A+W Production.docx         9
1. Scheduling
Currently there are two scheduling variants since a newer version should replace the previous
Items4Alcim (I4A). The newer scheduling variant Orders4Production (O4P) will be discussed
primarily below.


1.1. Orders4Production
In contrast to Items4Alcim, Orders4Production no longer works in item-oriented fashion, but rather
order-based. Furthermore, the scheduling is taken apart into individual work steps. If a work step
has completely processed an order, the next work step comes and processes it.
The sequence of the work steps can be configured. Some basic rules of sequence are checked
programmatically and, in case of non-adherence, cause the stopping of the scheduling. Thus, for
example, the Capa may not be run through before the MA. This also makes sense because the
machines are not previously assigned and therefore, no capacities can be booked.




Figure 1-1 Parameter administrator: specification of the sequences in O4P

In the parameter administrator (Fig. 1.1), you can also see that the sequences for orders,
quotations, reservation, and calculations can be specified individually. This creates additional
flexibility.
Below, the focus is on the set-up of the O4P and the description of the individual possible
WorkSteps.


          Set-up
If an import "Items4Alcim" is already configured, then nothing further has to be configured. The
sequences of the WorkSteps are initially pre-assigned from the standard database or initialized by
a DB script (awupdate_alcim_2_593.xml). The other switches are identical to those from I4A.
Then during use of the import SPs, the SPs may have to be adjusted. See section "1.1.2.16 SPCall."



A+W Software GmbH                     EN-CONFIG-A+W Production.docx                             10
If several set-ups (I4A) were set up, all but for one must be deactivated. O4P works with several
threads, so that the load is already distributed across all cores of a CPU.
If no "Items4Alcim" were configured, then the procedure is exactly the same as for initial set-up.
Activation of the scheduling (O4P) is done with the switch [ORDERS4PRODUCTION_SETTINGS /
ACTIVE] in the parameter administrator.


         Description of the work step
As already explained, the entire scheduling process is divided into individual work steps, which can
be run through in nearly any order. Some work steps can be omitted completely if they are not
necessary in a project or only for particular order types.
There are two work steps that cannot be configured. Thus each scheduling begins internally with a
"WorkStepStart" and each scheduling ends with a work step "WorkStepEnd“.
Behind the work steps is a comma-separated number. This number specifies how often this work
step may be present within the scheduling process. If the number is greater than 1, then two orders
can be processed simultaneously in this step. Thus it is possible that an order can "overtake"
another within the processing chain. However, this possibility does not exist for all work steps and
furthermore, with use of too many WorkSteps and thus too few CPU cores, there can be
performance issue. Here, you must experiment to get the best results. No general statement can
be made since there are too many configurable options and external dependencies.
1.1.2.1. WorkStepStart (internal)
Here the data of the OrderXML structure is taken over into the memory and checked roughly. It is
also checked whether the order is already in the database and the data is then loaded. Similarly, it
is checked whether the order is in the manual NR and with which NR decision the re-import should
take place.
1.1.2.2. AlcimWorks
This work step calculates the edge surcharges, processes the SN file, and generates images for the
sketches.
This work step can be run in parallel, edited, but always only one item of all available orders at a
time.
Before this work step, the steps "MachineryAllocation", "Enumerate" and "CheckUp1" must have
been run through.
1.1.2.3. AfterWorks
Prerequisite
The work step "AlcimWorks" must have been run already.
Description
The work step can perform different tasks.
    a) Set-up edge detection




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                11
      Machines can be selected for the set-up edge selection in the machine allocation.




      If machines are selected here in "Lines", the SP that was configured under "Afterworks SP"
      is called, which should then determine the set-up edge.


   b) Transport edge detection or validation
      If no lines are configured as under a), then the work step takes over the transport edge
      detection if machines were stored in "Transport Systems" according to the machine
      allocation.




A+W Software GmbH               EN-CONFIG-A+W Production.docx                                12
       The results are written in mzo_aufsttellkante.


   c) Takeover of the geometry data from the CADSheetsService
       All production data (incl. cutting) is transmitted to the CADSheetsService.
       This part is always executed by the "AfterWorks" work step.


For the transport edge detection, the machine allocation (MZO.dll) is used. It can only ever make
one calculation at a time. If several threads are configured for the "AfterWorks" work step, all
threads that share this possibility must be executed one after another.
Furthermore, the machine allocation is also used by the machine allocation (MZO.dll). With this
work step, the AfterWorks must also share the use of the machine allocation.
Remedy: => "MachineryAllocation2" or "MachineryAllocationParallel"
           and "AfterWorksParallel"


1.1.2.4. AfterWorksParallel
(available starting with the QR, which follows QR2403)


A+W Software GmbH                 EN-CONFIG-A+W Production.docx                               13
The content of this work step is identical to the "AfterWorksParallel" work step.
However, this, if the transport edge detection was configured, generates several instances of the
machine allocation (MZO.dll) in an individual process ("Albwir.Alcim.MAPipeServer.exe"). This
way, as many processes are generated as the system has CPU kernels. The items of an order are
then distributd evenly to the processes, which means that an individual order can be processed
much faster.
It must be noted that the work step "MachineryAllocationParallel" works with the same principle.
If both work steps are configured, "MachineryAllocationParallel" and "AfterWorksParallel" must
share the instances of the MZO.dll.


Assignment
In this work step, the familiar assignments are made.
This work step can be run in parallel.
AWDesign
This work step is familiar in I4A as CustomizingStep AWDesign. The AWD files are generated here.
This work step can be run in parallel.
Before this work step, the steps "Enumerate", "CheckUp1" and "CheckUp2" must have been run
through.
BasicScript
This work step must be included if a basic script should be executed for customizing purposes.
This work step can be run in parallel.
BomConfigurator
Here, the actions of the parts tree configurator are executed for deleting/adding parts/processings.
During use it must be noted that the order is not yet in the database at this point in time, so that
no formulas with SQL statements will work. (analogous to I4A)
This work step can be run in parallel.
Before the work step, the "CheckUp1" step must have been run through.
Capacity
Execution of the A+W Capacity Planner.
This work step can be run in parallel, edited, but nevertheless always only order at a time.
Before this work step, the steps "Enumerate", "CheckUp1", "Label", and "MachineryAllocation"
must have been run through.
CheckUp1
After loading the OrderXML structure, this modules takes care of the isolation of additional
properties, creation of new items in the master data, synchronization of the data, and verification
of the parts tree.
This work step can be run in parallel.
CheckUp2



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                14
After execution of the BOMConfigurator, it may be necessary to repeat CheckUp1 with the
manipulated parts tree.
This work step can be run in parallel.
Before this work step, the steps "Enumerate", "CheckUp1" and "BOMConfigurator" steps must have
been run through.
Enumerate
Executes the parts numbering, for which there are currently three modes. See also I1A in the
parameter administrator.
This work step can be run in parallel and may exist multiple times.
GrindArea
This work step executes the decoating module.
This work step can be run in parallel.
Before this work step, the "Enumerate", "CheckUp1" and "MachineryAllocation" steps must have
been run through.
Label
The labeling is done here.
This work step can be run in parallel.
Before this work step, the "Enumerate", "CheckUp1" and "CheckUp2" steps must have been run
through.
MachineryAllocation
An elementary component is the machine allocation, which is executed with this work step.
The results are not yet available in the database after execution; instead, they are placed in the
memory.
This work step can be run in parallel, but always only one item of all available orders at a time is
processed.
Before this work step, the "Enumerate" and "CheckUp1" steps must have been run through.
ResolveMacroProcessings
Additional function for resolving a macro processing into individual processings. A detailed
description of this function is in a separate chapter in this document.
This work step can be run in parallel and may exist multiple times.
SNCreation
The module automatically generates SN files for the A+W CAD Designer (shapes) taking the
OrderXML files into consideration.
This work step can be run in parallel and may exist multiple times.
SPCall
In this step, the familiar SPs cu_prt_itemwrt, cu_prt_ordwrt, and cu_mzo_extended are executed.
CAUTION: To be noted here is that the data in this work step is temporarily written with a negative
order number. If you use this order number in the SP, in order to determine an order number range,
for example, the SP must be adjusted after change from I4A to O4P!

A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                15
This work step can be run in parallel.
Before this work step, the "Enumerate" and "CheckUp1" steps must have been run through.
WorkStepEnd (internal)
In the last step, with successful scheduling, the results are written to the database, the PDC
initialization is started, and the report to the ERP is sent.
In case of errors during scheduling, the error message is reported to the ERP and the table
POOL_IMPORT is updated for manual NR




          ResolveMacroProcessings
This document describes the function for resolving macro processings into their part processings in
A+W Production (#414206).
Background, a macro processing is a combination of various processings, e.g. a drilling and a cut-
out. What precisely is included in the macro is not visible. The various processings in a macro cannot
be scheduled on different machines. A statistical evaluation is also difficult to perform. This function
was developed so that this is possible.
The O4P scheduling and a SN drawing of the item are the prerequisites for this function. If it is
active, a macro is taken apart into its part processings. For each part processing, a processing based
on our A+W processing type catalog is generated in the BOM. If for the A+W processing types
included, there is no appropriate processing in the master data, the item gets stuck in the manual
re-working and cannot be scheduled.
This function is available again starting with A+W Production Version 6.4 with database version
2.611.
Configuration
In O4P, the new work step ResolveMacroProcessing must be entered for the scheduling of orders
and reservations next to the work step CheckUp2.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                   16
Figure 1-2 Parameter administrator:       Specification   of   the   sequences   in   O4P   -   example   of
ResolveMacroProcessing

In the processing master data, there must be at least one processing for each A+W processing type.
If there are several processings, one must be selected. In order to assign this processing to the A+W
processing type, a SQL editor is required since there is no user dialog yet.
The table AW_BEARBTYPEN has been expanded to include the field STANDARD_ARTNR. The
processing item number belonging to the A+W processing type must be entered in this field. This
processing item must exist in the A+W Production master data.
SELECT aw_bearbtyp, standard_artnr, * FROM aw_bearbtypen ORDER BY 1;
UPDATE aw_bearbtypen SET standard_artnr = ? WHERE aw_bearbtyp = ?;


After a restart of the scheduling, this feature is active.
Caution: if new processings and processing types are created, it must be ensured that these can
also be scheduled in the MA on appropriate machines. New processing types (not A+W processing
types) must also be assigned to a batch type for detailed scheduling.
Result
If a macro is resolved it can be detected in the table POOL_BEARBEIT. There are 2 new fields:
MAKRO_AUFGELOEST and MAKRO_REFERENZ.
If the field is MAKRO_AUFGELOEST > 0, then this is a macro processing that was resolved. Then
there is at least one new part processing with which the field MAKRO_REFERENZ is filled with the
number from MAKRO_AUFGELOEST of the macro processing.
The SEQUENZ of the newly generated part processings corresponds to the SEQUENZ of the macro
processing. Which of the part processings is done first cannot be determined. These part
processings can be traced via the PDC. Reports are made via the macro processings since the part
processings are unknown in the ERP system.
Resolved macro processings are not loaded in the detailed scheduling and can thus not form lots.
Characteristics
Macros can contain cut-outs that cannot be described as A+W standard cut-outs. (Notched
corner(1300), notch(1400), inner cut-out(1405, 1415)). New A+W processing types were defined:
general notched corner (1303), general notch (1403), and general inner cut-out (1418). If a
processing cannot be described by the previous types, the new A+W processing types are stored.
In the parameters for these processing types, the size of the notch and the minimum rounding
radius are returned. These values can be used for machine allocation.
These new A+W processing types cannot be entered via our ERP systems since you cannot generate
an SN drawing using these types.
Display in rough scheduling
In the rough scheduling displays, you don't always want to see processings of resolved macros. You
can achieve this by filtering these processings in the displays. For this, there is a FIX filter
AUW_FIX_NO_RESOLVE_MACRO that is active in our default displays.
These processings can also be filtered on the Production Monitor if the display is controlled via the
VIEW AUW_CAPA_OVERVIEW. For this, there is a new AUW_SETTINGS parameter [CAPA_VIEW /
SHOW_RESOLVED_MACROS], which is used to control the VIEW.



A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                        17
1.2. Cancellation of orders
Orders can be cancelled via the scheduling. For this, the ERP systems write an OrderXML file with a
cancellation flag. This way, it is currently only possible to cancel entire orders, cancellation of
individual items is not possible.
The behavior described here also corresponds to the behavior via a cancellation via the PPS
WebService.
The entire order is cancelled, but the items behave differently depending on their status. The same
for all items is that the cancellation flag is set (AUFTKZ = 1).
If an order is in the POOL, in a pot or in a roughly scheduled batch, then this order is automatically
moved to the cancellation pot (12600). A now-empty batch or pot is resolved.
If the item is roughly scheduled in a batch with a greater status, then nothing further happens with
the order. It is cancelled and the other applications react to this cancellation flag. If a cancelled lite
is read on an A+W Production Terminal, an appropriate message appears there. If the lite was in a
finely scheduled batch when it was cancelled, there will be a warning on the release of the batch,
so that this item can be removed and deleted from the batch if necessary.
If an item was planned in a package optimization, in the manual follow-up, there is a message about
this cancellation. The message can be confirmed, the removal from a package optimization must
be done manually by the user.




1.3. Later transfer of production-irrelevant data

It is now possible to take over changes to certain data from the ERP even after planning.
Generally, this is the following data:
    -   Delivery date
    -   Customer data
    -   Delivery address
    -   Route
    -   File attachment with identifier for production transfer
    -   Order/item texts with identifier for production transfer
    -   Commission data
    -   Customer item


Such a transfer of the data is done in the OrderXML file with the ordering type "ChangeProduce"
or "ChangeOffer".
Meanwhile, the identification of the ordering type is possible down to the item level. The identi-
fier exists once on the order level and once for each item.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                     18
In this context, the ordering type "NoChange" was also introduced. Items marked this way remain
untouched in the import. This helps save time.
Meanwhile, it is also possible to transfer an OrderXML file with mixed ordering types.
Here, however, the rule applies that an order that consists only of "ChangeProduce" or
"NoChange" items is treated completely as a "ChangeProduce" order. Similarly, a "ChangePro-
duce" order that consists only of normal "Produce" and "NoChange" items is treated as a normal
"Produce" order.
On transfer of a complete "NoChange" order, no data is changed. Here it is not important which
identifier the item contains.


         Changing order data
    a) Takeover of the delivery date and route
        Generally, the delivery date is taken over from the OrderXML from the UDX.AW.ORDER-
        INFOS. There is tag delivery there.
        e.g.:
        <Delivery tour="2" description="Tour Nord / Route North" deliveryDay="2023-09-
        30T00:00:00" enrouteDate="2023-09-30T08:00:00" requestedDeliveryDay="2023-09-
        30T00:00:00" calendarWeek="201920" />

        Here, the deliveryDay, enrouteDate, description and tour are read out. The following
        database fields are thus updated:
        deliveryDay => pool_auftrag.lief_term

        enrouteDate => pool_auftrag.fahr_term

        description => pool_auftrag.tour_info

        tour => pool_auftrag.tour

        However, this only happens under the condition that the new delivery date is in the fu-
        ture and should take place later than the original delivery date.
        However, this condition can be cancelled with the switch ITEMS4ALCIM_SPECIAL/
        ALLOW_LATE_POSTPONE_TO_PAST. The switch is in the Parameter Administrator under
        A+W Production > Order Import > Late Takeover of Production-Relevant Data > Allow De-
        livery Date Change in the Past.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 19
Figure 1-3: ALLOW_LATE_POSTPONE_TO_PAST

   b) Takeover of order documents
      Order documents are transferred in the OrderXML_Datei in UDX.AW.ORDERINFOS > Attache-
      ments. These are then compared to the existing documents in pool_dokumente and added
      if necessary.


   c) Takeover of order texts
      Order texts are transferred in the OrderXML file in the UDX.AW.ORDERINFOS > CUSTOMER_RE-
      FERENCES and in ProcessPlanning. These are then compared to the existing documents in
      pool_txt and added if necessary.



   d) Takeover of customer data
      Here a whole series of data is taken over. The data is in the OrderXML under ORDER_HEADER
      > ORDER_INFO > ORDER_PARTIES > BUYER_PARTY

      Customer number:          PARTY_ID     => pool_auftrag.kunde_nr
      Name:                     NAME         => pool_auftrag.kunde_name1
      Name2:                    NAME2        => pool_auftrag.kunde_name2


A+W Software GmbH                  EN-CONFIG-A+W Production.docx                             20
      Name3:                   NAME3           => pool_auftrag.kunde_name3
      PLZ (Postfach):          ZIPBOX          => pool_auftrag.kunde_plz_postfach
      Postfach:                BOXNO           => pool_auftrag.kunde_postfach
      Straße:                  STREET          => pool_auftrag.kunde_strasse
      PLZ:                     ZIP             => pool_auftrag.kunde_plz_ort
      Ort:                     CITY            => pool_auftrag.kunde_ort
      Landeskennung:           COUNTRY         => pool_auftrag.kunde_landeskennung
      Telefon:                 PHONE           => pool_auftrag.kunde_telefon


   e) Takeover of shipping address
      The data for the shipping address is in the OrderXML under ORDER_HEADER > ORDER_INFO >
      ORDER_PARTIES > DELIVERY_PARTY

      Name:                    NAME            => pool_auftrag.lief_name1
      Name2:                   NAME2           => pool_auftrag.lief_name2
      PLZ (Postfach):          ZIPBOX          => pool_auftrag.lief_plz_postfach
      Postfach:                BOXNO           => pool_auftrag.lief_postfach
      Straße:                  STREET          => pool_auftrag.kunde_strasse
      PLZ:                     ZIP             => pool_auftrag.lief_plz_ort
      Ort:                     CITY            => pool_auftrag.lief_ort
      Landeskennung:           COUNTRY         => pool_auftrag.kunde_landeskennung



        Change of item data
   a) Takeover of item documents
      Item documents are transferred in the OrderXML_Datei in UDX.AW > Attachements. These
      are then compared to the existing documents in pool_dokumente and added if necessary.
   b) Takeover of item texts
      Item texts are transferred in the OrderXML file in the UDX.AW > CUSTOMER_REFERENCES and
      in the ADVICEs of the parts and processings. These are then compared to the existing item
      texts in pool_txt and added if necessary.
      Here there is the particularity that texts with a configuring ID (ADVICE > key) can be igno-
      red. E.g. if texts were generated by SPs and never transferred via the OrderXML file.
      This happens in the Parameter Administrator in A+W Production > Order Import > Late
      Transfer of Production-Irrelevant Data > Ignore Changes to Texts




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                               21
Figure 1-4: IGNORE_TEXTCHANGES_IN_LATEORDERCHANGE




   c) Change of commission data
      This data is in the OrderXML file under UDX.AW > Commission.
      The customer order from CustomerLineItemID and the texts from ADVICEs are taken over.
      The takeover of this data can be suppressed with the switch ORDERS4PRODUCTION_SPE-
      CIAL/IGNORE_COMISSION_CHANGES




A+W Software GmbH                EN-CONFIG-A+W Production.docx                             22
Figure 1-5: IGNORE_COMISSION_CHANGES



   d) Change of the item delivery date
      This date (in pool_pos.lief_term) is only changed with appropriate configuration. The
      switch for activation is in the Parameter Administrator under A+W Production > Order Im-
      port > Late Takeover of Production-Irrelevant Data > Adjustment of Item Delivery Date.
      Here, the same order delivery date is written in the item (pool_pos.lief_term).




A+W Software GmbH               EN-CONFIG-A+W Production.docx                               23
Figure 1-6: CHANGE_POS_LIEFTERM




A+W Software GmbH             EN-CONFIG-A+W Production.docx   24
2. Rough Scheduling
2.1. FIX filter
Displaying a normal filter in the A+W Production POOL can be changed and saved for each station
ID. A FIX filter is a filter that is linked directly to a view and cannot be changed.
For example, you might want to define a view only for IG units. Without a FIX filter, you must select
an IG filter for each station; these can be taken away by the customer at any time and then will not
display the IG units.


           How can a FIX filter be configured?
A FIX filter is defined like a normal filter. The type for which view a filter is defined is not important
for a FIX filter.
The AUW standard FIX filters are not linked to any special type (POOL_FILTER.VIEWS is empty). This
has the advantage that nobody sees the filter in the filter list and thus cannot change the behavior.


           How is a FIX filter linked to a display?
Currently, configuration is only possible with a SQL editor.
First the name of the filter to be used must be determined:
SELECT name, * FROM pool_filter;

The value from column name must be used in the view. For this, the main data record of the
affected view must be determined in the database table POOL_SORT with the following SELECT:
SELECT sortiertyp, station, feldname, titel, sprache, def_filter FROM pool_sort WHERE rang
= 0;

As soon as the view has been determined, insert the name of the filter in the def_filter field:
UPDATE pool_sort SET def_filter = '<name of FIX filter from table POOL_FILTER>' WHERE rang
= 0 AND sortiertyp = '<view type>' AND station = '<station>' AND feldname = '<name of
view>' AND sprache = '<language of view>';


           How can you see that your FIX filter is active?
If a view is opened in A+W Production, you can only see starting with Version 5.4 from the displayed
non-changeable filter name in the display that a FIX filter is active.




Figure 2-1 Pool display - selected filters




A+W Software GmbH                        EN-CONFIG-A+W Production.docx                                 25
          FIX filter for the standard displays
The names of the standard FIX filters begin with AUW_FIX_. These may not be changed. With an
update    since      Version       5.3,    they    are     inserted    automatically    with
awupdate_alcim_AUW_FIX_filter.xml (database update tool) and overwritten.


          Known Problems
    •    A FIX filter is active, but not used. In the SQL instruction for the view, the filter is missing:
         since Version 5.4, a FIX filter definition with more than 127 characters is ignored 
         #332610


2.2. VIEW database for rough scheduling views
For the configuration of the rough scheduling views, it is not just possible to load data from tables.
If information is missing, this can be determined via a VIEW database. Thus, for each usable table,
there are 2 VIEWs in the database, which are available for selection during the configuration of the
fields in the rough scheduling and also automatically in the A+W Production Terminal. The name of
the VIEW consists of the table name and an abbreviation "AUW_" or "CUV_" in front of it.
Example for the table POOL_TEILE, there can be the following VIEWs: CUV_POOL_TEILE and
AUW_POOL_TEILE.
The VIEWs with the abbreviation "AUW_" are created by development and may not be edited or
created in the projects. If this should happen, they are overwritten automatically in case of an
update.
In the project, VIEWs with the abbreviation "CUV_" can be created. These are individual for each
customer installation.
Currently there are the following VIEWs in every installation: AUW_POOL_TEILE and
AUW_POOL_SZR. The fields of these VIEWs are described in the database documentation.




Figure 2-2 Field definition of the rough scheduling for fields from a VIEW




A+W Software GmbH                       EN-CONFIG-A+W Production.docx                                  26
An advantage of using a VIEW, you don't have to create a StoredProcedure in order to procure data.
A VIEW works identically under SQLServer and INFORMIX. You can also use this VIEW like tables in
a report.


2.3. Additional and surplus quantities
Additional or surplus quantities are necessary if for various reasons, production would like to start
with a larger quantity than the customer has ordered. This larger quantity can be handled in
different ways.
Caution: The excess quantity dialog in A+W Production must not be used if the location-spanning
PDC is used at the same time, as otherwise new label numbers would be generated which would
not be known in all production locations.


          Commercial surplus
Commercial surplus and shortfall refers to a complete item. There is a minimum and a maximum
quantity. Production of the maximum quantity is the goal. In case of a break, no remakes are done
unless the quantity underruns the defined minimum.
Surpluses can be entered during the order entry or directly in A+W Production using a surplus
editor. A+W Production reports the quantity produced to the ERP system (here, A+W Business)




Figure 2-3 Commercial surplus




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 27
         Technical surplus
Technical surplus refers to element chains in the bill of materials and can even refer to processing
steps. It is not controlled by order entry, but is entered in A+W Production, either automatically by
SPs or by hand in a special surplus editor. However, these quantities are not known to the ERP
system and therefore have no commercial influence.


         Additional quantities
Additional quantities are also only defined in production and can also be set using the surplus
editor. They are required if a couple of units more shall be produced in general, e.g. for test lites.


         Surplus and additional quantities in the database
The tables POOL_POS, POOL_TEILE and POOL_BEARBEIT offer information on surplus. The table
POOL_POS is only filled if the surplus was taken over from the order entry. If the surplus is only
entered in A+W Production, the fields of POOL_POS remain unchanged.
        POOL_POS. MENGE / POOL_TEILE.MENGE
        Maximum quantity, quantity entered + surplus
        POOL_POS. MINDERMENGE / POOL_TEILE.MINDERMENGE
        Quantity by which the maximum quantity can be reduced before remakes are produced.
        This field will not be set for additional quantities.
The next fields are set by barcoding and are adapted based on the booking.
        POOL_TEILE.BDESTUECKOFFEN_ANZ
        Number of the units that have to be produced for a line item = maximum quantity –
        produced quantity – breakage (for which no remakes had to be produced)
        POOL_TEILE.BDEFERTIG
        0 = item has not been completely produced
        1 = minimum quantity (MENGE – MINDERMENGE) reached
        2 = maximum quantity (MENGE – breakage) reached
        POOL_BEARBEIT.FINAL_KZ
        The field controls the completion reports for units. A unit is complete when the last
        processing step prior to packing and shipping was booked. This field is filled by barcode
        initialization.
        0 – any processing step
        1 – last processing on the shop floor
        2 - packing (BEARBEITSTAMM.AW_BEARBTYP = 1800)
        3 - shipping (BEARBEITSTAMM.AW_BEARBTYP = 1810)
        AW_BEARBTYP must be set for packaging and dispatch, it is not possible to initialize the
        field elsewhere!
There are additional fields for the technical surplus.
        POOL_TEILE.MENGE_NACH
        POOL_TEILE.MINDERMENGE_NACH
        POOL_BEARBEIT.MENGE_PROD



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                  28
        POOL_BEARBEIT.MINDERMENGE_PROD


         Additional and surplus quantities in the OrderXML
Information about additional quantities is transferred in the following tag in OrderXML:
<CommercialQuantities surplusQuantity="10" requestedQuantity="100"
shortageQuantity="10" />


         Reporting of additional and surplus quantities
Surplus quantities can only be reported using fileless feedback. No additional configuration is
required; the reports are created automatically as for all barcode bookings.
The reports transfer the quantity and information BDEFERTIG. This happens if the processing step
is reported completed with FINAL_KZ = 1, whereby the reporting status is 700. This information is
also transferred in case of a report of "delivered," status = 800
A+W Business
A+W Business adjusts the quantity starting with BDEFERTIG = 1. A change of the order status has
no effect; the order status can react as usual to the status (in the A+W Business register point) 700
and 800.
If a surplus has been entered in A+W Production, the reported quantity is processed only if a surplus
has been configured for this product in the A+W Business master data. If this is not the case, the
quantity will not be changed in A+W Business.
If the end quantity of the produced units is reported to A+W Business, the quantity is adjusted in
A+W Business accordingly and invoiced.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 29
A+W Enterprise
A global switch in the A+W Enterprise dispatch control enables the reporting of surpluses.


          Entry of additional and surplus quantities
A+W Production Standard
In A+W Production, there are two additional quantity editors: one for the entry of surpluses and
additional quantities per item and one for the entry of technical surpluses. You have to select one
of these in an installation; the function searches for a dialog called MEDIT.




Figure 2-4 Surplus editor

In order to be able to load the editor in the POOL views with [Enter surplus], it has to be activated
with the parameter [POOL_SETTINGS / MENGEX] = 1.
SELECT text, * FROM parameter WHERE bereich = 'POOL_SETTINGS' AND eintrag
= 'MENGEX';
INSERT INTO parameter (bereich, eintrag, text, typ) VALUES
('POOL_SETTINGS', 'MENGEX', '1', 0);
The editor is used for elements in the basic database; it is also included in the basic package. To
change this or for additional information about the editor, please read the documentation
\\jupiter\DOKU_DocuWare\ALCIM2000\Grobplanung\Installation_Configuration\ALCIM_SurplusE
ditor-Eng.docx.
The dialog used can be set for each StationID:


A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 30
Figure 2-5 Parameter Administrator




A+W Software GmbH                    EN-CONFIG-A+W Production.docx   31
          A+W Production precise to the part
The editor for entering surplus quantities can be opened from the order view in A+W Production.
Right mouse-click on the order in question -> Reentry -> Surplus Quantities




Figure 2-6 Opening a surplus editor

In the standard system, quantities can only be changed item by item. Now it is also possible to
change quantities for individual parts of the BOM with restrictions. For this, configuration is
required on the new dialog (AUW_MEDIT_BOM_LEVEL).




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                          32
Figure 2-7 Additional quantity change

A quantity change for a header automatically affects all subparts. If, for example, the additional
quantity 3 is entered for an IG, all subparts also receive at least this additional quantity. A quantity
change is only possible for parts that have subparts and the procurement type Production. For
example, you cannot change the quantity for a float with procurement type Cutting. A quantity
change for the TG above the float, on the other hand, is possible and also causes a quantity change
for the float.
Table cells in the parts list that cannot be edited due to restrictions are displayed grayed out.
Even if the quantities are only changed for individual parts of the position, the entire item receives
new labels.
In contrast to the additional quantity in the case of breakage, the surplus quantity always produces
remakes. If you enter an additional quantity, the following fields are increased:

MENGE and MENGE_NACH in POOL_TEILE.

The surplus quantity also increases the fields:

MINDERMENGE and MINDERMENGE_NACH.



          A+W Production multiples
The surplus editor can also display multiple parts and change their quantities accordingly. If, for
example, there is a tape with quantity 40 below a TG with quantity 10, an additional quantity of 4
is automatically set for the tape when an additional quantity of 1 is entered for the TG.
Restriction: In items that contain showcases or similar constructions, i.e. where the quantities of a
part may be multiples of its upper part, no test lites may be added.


A+W Software GmbH                       EN-CONFIG-A+W Production.docx                                33
Note: In the detailed scheduling, the following SQL should be executed if the user does not produce
showcases or similar constructs:

insert into parameter (bereich, eintrag, nummer, typ, text) values('FEIN_SPECIALS',
'GLASSCABINETS', 0, 0, 0);

Without this SQL, the new logic would not apply if a subpart by the test lites has an amount that is
a multiple of the amount of the upper part.

The MULTIPLIER field in the POOL_TEILE table in the database must exist and be filled by the import
before you can handle multiples correctly.
The following database script extends the Pool_Teile table with the "Multiplier" field

•        awupdate_alcim_2_631.xml


                  A+W Business
Surplus can be entered in master data right for the product or for a combination of product and
customer. If both are defined, the customer is used.
[Master data / Partner / Customer / Exceeds amount]




Figure 2 - 8 Entry of surpluses

[Master data / Products / Product / Products / 2. Production]




A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                 34
Figure 2-9 Entry of default values for deviating quantities



The values for each item can be changed during the order entry.




Figure 2-10 Entry of deviating quantities


The information is saved in the following A+W Business database fields:
- BW_Auftr_POS.PP_MENGE
- BW_Auftr_POS.PP_UEBERMENGE
- BW_Auftr_POS.PP_UNTER-MENGE




A+W Software GmbH                        EN-CONFIG-A+W Production.docx    35
3. Batch release
The release of batches is done via a freely definable release dialog that is coupled to the respective
detailed planning organization.
The execution of the individual actions of the release (generation of machine code, printing of lists,
etc.) can be done directly in the foreground in the user's session or in the background by the service
ProcessManager. Here it is possible to determine the execution of each individual action
individually.
For execution in the foreground, the user must wait until all actions have been executed before he
can continue working. In the background, it is possible to continue working right away, for the
actions are executed asynchronously.
If for the first release all actions were processed successfully, the batch status will be set to 200
released. With another release of a batch, in order, for example, to print a list, the status is no
longer changed.
The actions to be executed are saved in the table PROZESSE. The status of the respective actions,
especially for execution in the background, can be viewed with the ProcessManagerControl help
program. Actions, e.g. flawed ones, can be deleted or restarted with this program.




Figure 3-1 ProcessManagerControl



3.1. Executing the release of several instances
In order to increase the speed of the release process, several instances of the ProcessManager
service can be put into operation. Here it applies, one site per server. If you would like to put a
second service into operation for a site, it must be on another server.
In the configuration, groups of servers are defined on which one ProcessManager apiece runs.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                  36
Figure 3-2 Parameter group

The executing group must be assigned for the respective actions.


          Synchronization of printing across several instances
In this mode it has been possible since 6.4.x that lists are also printed in the correct sequence on a
printer, even if they are executed by different instances.
For this, a group must be declared the leading group, which sends the lists generated to the printer
in the correct sequence.




Figure 3-3 Parameter leading group

The prerequisite is that the actions of the lists run via the mode INTERN.




Figure 3-4 Configuration of report mode INTERNAL

The ProcessManager instances generate a PDF file for each list. This is saved temporarily in an
output directory. All instances must have access to this directory.



A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                 37
Figure 3-5 Parameters PDF output directory

The leading group sends the PDFs generated to the printer in the desired sequence.


3.2. Release of batches with cancelled items
For batch release, it is checked whether cancelled items are included. If they are, you can prohibit
release or inform the user.
The behavior is controlled via the station-dependent rough scheduling switch [POOL_SETTINGS /
SCHEDULE_RELEASE_STORNO]: 1 = warning that cancelled items are included / 2 = message that a
release with cancelled items is not permitted.




Figure 3-6 Parameter [POOL_SETTINGS / SCHEDULE_RELEASE_STORNO]



3.3. Specifying environment for scripts and reports
Starting with version 6.4.3938, the environment for execution of scripts and reports can be
configured.

Reports
Reports can be executed in two ways. A report can either be executed with a VisualBasic script that
calls the Crystal Report Runtime or the ProcessManager calls the Crystal Report Runtime directly.
The parameter [Script name] contains either the name of the script that should execute the report
or is set to the value 'Internal' in order to execute the report directly in the ProcessManager.
Starting with Version 6.4.               3938,   there   is   a    new     parameter      available,
[_RDLG_ReportExecuteInternal].
This parameter overrides the setting of the report if the A+W script 'Report.vb' is specified. The
default setting 'True' causes the execution of all reports in the ProcessManager without use of the
A+W script 'Report.vb'. The value 'False' results in the previous behavior and executes each report
according to its individual setting.


A+W Software GmbH                    EN-CONFIG-A+W Production.docx                               38
In the case that the A+W script 'Report.vb' has been changed by the customer, with the new default
setting, the behavior is changed. The A+W script 'Report.vb' should then be renamed and the script
name adjusted in the parameters so that the renamed script is accessed. Adjustment should not be
made in the A+W scripts.

Scripts
Scripts were previously always executed in an individual process of the Awh.exe.
This behavior constantly caused problems with the call of the application and the procurement of
trace files. Starting with Version 6.4.3938, it is possible to specify with the parameter
[_RDLG_ScriptExecuteInternal] whether all scripts are executed in an individual process (setting:
'False') or should be executed in the process of release (default setting 'True'). In the case of release
in the foreground, this means an execution in the process Alcim; for release in the background in
the process ProcessManagerService. The trace entries are then written to the trace file of the
respective process and the trace level is set in the respective config tool.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                    39
4. Crystal Reports
In A+W Production, papers are printed via Crystal Reports. There are several versions of the Crystal
Reports runtime, which are installed by Setup. It is recommended that you always use the newest
runtime; in case of an update, it is not activated automatically. Currently, it is the version 2013. The
version 2013_v1 is reserved only for test purposes.
The version of the Crystal runtime used by A+W Production is set with the parameter
[ALCIM_SETTINGS / CRYSTALVERSION]. The runtime must be installed so that it can be used.




Figure 4-1 Parameter administrator: specification of the version of the Crystal Report runtime



4.1. Parameters for control
A+W Production checks existing parameters in a report. If particular parameters exist, particular
behaviors are activated.
These parameters do not have to be used in the report, they just have to exist. If not separately
listed, a parameter of the type character string without special settings is sufficient.
showCRParameterDialog
If the user expects a parameter input for the execution of a report, then a dialog developed by A+W
opens for input of parameters. If the parameter showCRParameterDialog exists, the Crystal
Reports input dialog is used. This parameter has no effect when called in an A+W Production
Terminal; there, the A+W input dialog is always used since this is not otherwise technically possible.
Refresh
It happens that a report is output on a screen and stays there for a longer time. Now the content
should be updated without the user's having to do this manually. If there is one of these parameters
with the name Refresh, the report automatically updates at an interval of one minute. If this
parameter is then also used in the report, so that the user must input a number when starting, the
number input corresponds to the interval.
If another interval should be used, the interval can be specified permanently in the parameter's
name, e.g. Refresh30, Refresh180
TREEDRILLDOWNMENU




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                                 40
If the parameter TREEDRILLDOWNMENU exists, then with display of the report on the screen, the
Crystal Reports control element, which reproduces the tree structure of the report, is displayed on
the left side.
PrintMode
When printing from Crystal Reports, there can always be problems if a printer is set for printing.
The various versions of Crystal Reports runtime have different methods that can be used when
selecting a printer. With Crystal Reports Version 2013, there is a new method that we use and that
is recommended by Crystal Reports. Since there are cases where an older method was necessary,
but we do not want to install an old runtime, the switch [REPORT_SETTINGS /
PRINTMODEFEATURE] was introduced. With it, it is possible to address one of the three possible
print methods purposefully.
For this, in the report a parameter field with the name PrintMode of the type number must be
created and the value 1, 2 or 3 entered in the value list.
1 = old method
2 = old method that tries to reformat a report if the aspect ratio is not correct
3 = method from Crystal Reports Runtime 2013
<Parameter does not exist> = current method from set version starting with 2013




Figure 4-2 Crystal Report Designer - Parameter field dialog



4.2. Report call directly via PPS WebService
A report can be called directly in a browser via the PPS WebService. For this, the page
ViewReport.aspx must be called in the PPS WebService with the parameter Report. If the report
requires input parameters, these must also be specified.
Example:
http://<NameServerPPSWebService>/Albwir.Alcim.DataService/ViewReport.asp
x?Report=//<NameServerTransFolder>/trans/Reports/BDE/AUW_OrderList_Statu
s.rpt&Unterteile_anzeigen=1&Auftrag=700053


4.3. Generate true to scale sketches
True to scale shape sketches are printed in A+W Production on various lists. Especially on
production lists, we have the problem that sketches cannot be seen clearly when the products have


A+W Software GmbH                      EN-CONFIG-A+W Production.docx                            41
steps. Starting with ALCIM2011, this has changed. Here are some examples of a production list with
stepped IGUs:




Figure 4-3 Example of true to scale sketch

To get such sketches, a SN drawing with appropriate BOM must exist for the relevant item. For all
items without SN drawing, the scheduling can automatically create a SN drawing. For this function,
the OrderXML interface and use of the A+W processing catalog are prerequisites. This is switched
on with the switch CREATE_SN_FILE_BY_ORDERXML.




Figure 4-4 Switch [ITEMS4ALCIM_SPECIALS / CREATE_SN_FILE_BY_ORDERXML]

The SN files are defined in the path saved via the switch DATAFILEPATH. If the switch is empty, the
default path $SERVERDIR$\SN is used.




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                            42
Figure 4-5 Switch [POOL_SN / DATAFILEPATH]

For each item with an SN drawing, the optimization uses the BLOCK export of the SN drawing. This
is not desired, and in most cases also not necessary, and most important, functions such as shape
optimization and extended edge decoating are not possible. In order to optimize default shapes
and rectangles despite SN drawing without BLOCK Export, the switch SNCUTASSTANDARDFRM
must be set. Items already imported must be re-imported so that this setting takes effect.




Figure 4-6 Switch [ALCIM_SHAPE / SNCUTASSTANDARDFRM]

The A+W CAD Designer (Shapes) views used for the sketch generation are defined via the switch
SKETCHPRINTINGVIEWS. Use drawing views such as DRAWINGTARGETPRODUCT and
DRAWINGUNICUT instead of the construction views such as TRAGETPRODUCT and UNICUT.




Figure 4-7 Switch [ALCIM_SN / SKETCHPRINTINGVIEWS]

The views configured via this switch can be selected on the dialog for configuration of the sketch
initialization. The sketch initialization during the batch release decides which of the generated JPG
files (saved next to the SN files) in the SKIZZEN table. Our reports load the sketches from the SKIZZEN
table.


A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                   43
Figure 4-8 Sketch configuration dialog

During the archiving process, the ALCIMServer service can delete SN and JPG files. For this, the
switch DELETE_SN_FILES must be switched on.




Figure 4-9 Switch [ALCIM_BDESETTINGS / DELETE_SN_FILES]


          Display of the step profile
Starting with Version 2012, it is possible to display the profile of a unit on the sketch. This
information is displayed automatically on the sketch if activated in the configuration (SN.INI) of
A+W CAD Designer (Shapes): [Picture]ShowProfile = 1




Figure 4-10 Sketch with profile



Switch for additional information in the profile:



A+W Software GmbH                        EN-CONFIG-A+W Production.docx                         44
[Picture]
ShowProfile = 1
ProfileFontSize = 9
ProfileFontType = ARIAL
ProfileWidthInPercent = 20
ProfileHeightInPercent = 20

ShowProfileSurface = 1
ShowProfileDrilling = 1
ShowProfileMitr = 1


         Generate turned sketches
Since Version 5.3 it has been possible to generate an additional turned sketch for the final product.
This additional sketch has KATEGORIE=20 in the SKIZZEN table (other sketches have the value 2).
This function is switched on via the hidden switch [ALCIM_SHAPE / SKETCHPRINTPRODUCTFLIPPED]
(0=off / 1=on).
SELECT text, * FROM parameter                WHERE    bereich='ALCIM_SHAPE'       AND    eintrag    =
'SKETCHPRINTPRODUCTFLIPPED';


INSERT INTO parameter (lastmodstation, lastmodzeit, bereich, eintrag, text, nummer,
modul) VALUES ('__INIT', GetDate(), 'ALCIM_SHAPE', 'SKETCHPRINTPRODUCTFLIPPED', '1',
0, 'AWORKS');


UPDATE parameter SET text='1'               WHERE    bereich='ALCIM_SHAPE'        AND    eintrag    =
'SKETCHPRINTPRODUCTFLIPPED';
If turned sketches are required for cutting, due to texture or coated glass, this can be turned on via
the switch SN_FLIPMODE=3.




Figure 4-11 Switch [ALCIM_SHAPE / SN_FLIPMODE]



4.4. Printing customer logos
The end customer's logos should always be printed on papers, e.g. shipping labels. A possibility
would be to store these logos in the report itself and to display it via a formula depending on
customer number. The disadvantage is that this would have to be done in each report and would
unnecessarily expand a report.
An alternative is the use of the table SKIZZEN_LOGOS, in which the customer logos are saved and
from which the logos can be printed on reports.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                  45
In order to load logos into this table or change them, there is the tool AWPLogoTableEditor. This
tool is in each A+W Production installation in the Tools directory and is started with the EXE.




Figure 4-12 AWPLogoTableEditor

On first start of the application, first the database connection to the A+W Production database must
be configured. The tool does not determine this itself. In the configuration, use the button with the
screwdriver at the top right.




Figure 4-13 AWPLogoTableEditor – configuration of database

You can view the trace information at runtime; switch the Trace display on or off with the Trace
button.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 46
Figure 4-14 AWPLogoTableEditor – Trace display


          Adding a logo
When adding a logo, the logo number, LogoTyp (also a number) and a comment about the logo are
requested.




Figure 4-15 AWPLogoTableEditor – adding a logo

Last, a file selection for selection of an image file opens. Supported formats are BMP, JPG, GIF, and
TIFF. In our reports, we use BMP or JPG images; other formats may work, but were not tested.




Figure 4-16 AWPLogoTableEditor – image file selection




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                47
          Editing a logo
With selection of a logo, there is a button for editing the value in question in the database next to
each value.




Figure 4-17 AWPLogoTableEditor – editing a logo


          Deleting a logo
The selected logo can be deleted from the database with the Delete button.




Figure 4-18 AWPLogoTableEditor – deleting a logo


          Saving a logo
The image of the selected logo can be saved in a file from the database. Here, the original file format
is retained.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                  48
Figure 4-19 AWPLogoTableEditor – saving a logo




A+W Software GmbH                   EN-CONFIG-A+W Production.docx   49
5. A+W Capacity
5.1. How to work with A+W Capacity for scheduling
This chapter will attempt to describe how to work with scheduling in A+W Production starting
with Version 6.x.
The prerequisite is: An order with a delivery date is entered in the ERP system.
The handling time in working days is deducted from this delivery date, then the order receives a
route date (day with time) depending on the route planning.
The shift end of the last processing must either be before this route date or it can be at the same
time.
If a delivery date postponement is possible through the system, then the switch for the activation
also includes a number of days by which the delivery date may be postponed.
Now the scheduling determines all route dates that are possible in this period right at the start.
Note: Only if the switches ITEMS4ALCIM_SETTINGS / ROUTE_DATES_VIA_CAPA = 1 and
ITEMS4ALCIM_POSTPONE_DELIVERDAYS > 0 are set. Otherwise things proceed step by step and
slowly.
In order to be able to understand other ways of working for scheduling, the flexible transition
time (also informally called the "rubber band") must be discussed.
The program itself can essentially build in a flexible transition time between the second-to-last
and last processing. You CANNOT prevent this!
This flexible transition time can also be used below the assembly (IG, LAMI pre-compound) and
before campaign work processes and before processings locked by the program.
(Note: The switch CAPA_SETTINGS / DISABLE_AUTOMATIC_FLEXITRANS prevents the automatic
setting of the flexible transition time below assembly parts such as IG, LAMI pre-compound, as-
sembly, etc.)


Now the following is distinguished depending on the order type and switch setting:


         Switch position regular order
Switch DD postponement           = NO
Switch to rush grid     = NO
•   Route date is known, for the scheduling, only the normal transitions (shifts + max. shifts) are
    drawn from the transition times.
•   Program tries using the transition times and the flexible transition time to schedule without
    postponing the DD.
•   Scheduling is only done in unlocked shifts and on bottleneck machines with free capacity in
    the shift.
•   If this is not possible, then the order lands on the red card.


A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                    50
Switch DD postponement           = YES, x days
Switch use rush grid    = NO
•   Route date is known, for the scheduling, only the normal transitions (shifts + max. shifts) are
    drawn from the transition times.
•   Program tries using the transition times and the flexible transition time to schedule without
    postponing the DD.
•   If this does not succeed, then there is a postponement to the next possible DD if this is also in
    the range specified.
•   Scheduling is only done in unlocked shifts and on bottleneck machines with free capacity in
    the shift.
•   If this is not possible, then the order lands on the red card.


Switch DD postponement           = YES, x days
Switch use rush grid    = YES
•   Route date is known, for the scheduling, only the normal transitions (shifts + max. shifts) and
    RUSH (shifts, max. shifts not relevant) are drawn from the transition times.
•   Program tries using the transition times and the flexible transition time to schedule without
    postponing the DD.
•   If this does not succeed, then there is a postponement to the next possible DD if this is also in
    the range specified.
•   Both a conversion to rush grid, use of the flexible transition time, as well as a DD postpone-
    ment are stored with internal costs.
•   The program now weighs these internal costs and determines the most "cost-effective" way.
•   Essentially, the program tries to place the rush grid at the start of the production chain.
•   Scheduling is only done in unlocked (Version 5.5 to 6.1 also occupies shifts locked for normal
    orders, but this is an error) shifts and on bottleneck machines with free capacity in the shift.
•   If this is not possible, then the order lands on the red card.
•   Recommendation: Do not activate the use of the rush grid for normal orders.


         Switch position rush order
Switch DD postponement           = NO
Switch to rush grid     = irrelevant since already rush order
•   Route date is known, for the scheduling, both the normal and rush transitions are drawn from
    the transition times.
•   Program tries using the transition times and the flexible transition time to schedule without
    postponing the DD.
•   Here too, the program weighs between rush grid and flexible transition time.


A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                    51
•   The specification is to maintain the DD.
•   Scheduling is only done in unlocked shifts and shifts for rush orders and on bottleneck machi-
    nes with free capacity in the shift.
•   If this is not possible, then the order lands on the red card.


Switch DD postponement           = YES, x days
Switch to rush grid     = irrelevant since already rush order
•   Route date is known, for the scheduling, both the normal and rush transitions are drawn from
    the transition times.
•   Program tries using the transition times and the flexible transition time to schedule without
    postponing the DD.
•   Here too, the program weighs between rush grid and flexible transition time.
•   The specification is to maintain the DD.
•   Scheduling is only done in unlocked shifts and shifts for rush orders and on bottleneck machi-
    nes with free capacity in the shift.
•   If the DD cannot be adhered to, then a new DD is determined, whereby this is already known
    to the system, as mentioned above.
•   Now there is another calculation taking into account the "costs" for usage rush grid, flexible
    transition time, and DD postponement.
•   Therefore, it is theoretically possible that not the next but the DD after the next is found, e.g.,
    if the DD postponement is more "cost-effective" than the continuous use of rush transitions.
•   If no DD is determined, then the order lands on the red card.



         Switch position high-priority order
Switch DD postponement           = NO
Switch to rush grid     = irrelevant since already high-priority order
•   High-prioirity order must go in
•   Scheduling attempt with all grids, also minimal
•   Scheduling attempt in shifts that are open for rush orders
•   Scheduling attempt in shifts of bottleneck machines, even if these are already full
•   Scheduling attempt of a processing in a shift, even if the duration is longer than the shift dura-
    tion (error eliminated in Version 6.2)
•   If this still does not manage to find the DD, then there is a second internal scheduling at-
    tempt.
•   The second attempt ignores the campaign dates and can bring the production start forward.
•   If no scheduling is possible, then the order lands on the red card.


A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                  52
Switch DD postponement          = YES, x days
Switch to rush grid     = irrelevant since already high-priority order
•   High-prioirity order must go in
•   Scheduling attempt with all grids, also minimal
•   Scheduling attempt in shifts that are open for rush orders
•   Scheduling attempt in shifts of bottleneck machines, even if these are already full
•   Scheduling attempt of a processing in a shift, even if the duration is longer than the shift dura-
    tion (error eliminated in Version 6.2)
•   If this still does not manage to find the DD, then there is a second internal scheduling at-
    tempt.
•   The second attempt ignores the campaign dates and can bring the production start forward.
•   If no scheduling is possible, then the DD is postponed.


5.2. Collected information
This information came from a document from the market solution area, which was composed by
NG in 2016.


         Manual reprocessing (red card)
If an order is on the red card, then you can force the scheduling.
    •   "Force scheduling"
        Shifts of bottleneck machines will be ignored, even if these are full.
        A processing with a duration that is longer than the shift duration can be scheduled.
    •   "Ignore scheduling"
        Order will be handled like high-priority order, see above.


         Processing chains
    •   All processings that are done together should have activated the processing chain in the
        MA. These include arrissing, grinding, polishing, drilling, etc.
    •   Just not for processings that must be done one after another, that is, e.g., two times
        screen printing, two times sand blasting.


         Alternative machine
    •   If an alternative machine is activated, then record times the time. Can take somewhat
        longer during import.
    •   Ensure that the processing is not brought forward.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                53
        CAPA_SETTING/MINIMUM_NORMALTRANSITIONS switch
   •   Specifies how many normal transitions are permitted between two machines.
   •   Should not be greater than value from "MaxSchichten".
   •   If a value in "MaxSchichten" is greater than this, then higher values will be ignored.




A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                54
6. Feedback
In the past, many files were used to synchronize batch, order, item, and rack status between A+W
Production and the ERP systems. This required a lot of configuration and caused many problems.
To simplify the configuration, fileless reporting has been developed.
Advantage:
    •   Only a few settings are required for reporting of the basic status of an order/item/rack
    •   No files between the systems are required
    •   Direct view of the production database in order to get more detailed information
Process:




Figure 6-1 Reporting process

ALCIMBOOK service saves changes to the batch/order/item or rack status in special report tables:
    •   ERP_RUECKMELDUNG: Reporting of batch and production status
    •   ERP_GEST_MELDUNG: Reporting of rack assignments, linked to production status
        messages
    •   XOPT_RUECKMELDUNG: Reporting of stock lites used during the cutting process
Two important time stamps are included in all three tables:
    •   MELDEZEIT: Time stamp when the report was generated
    •   SENDEZEIT: Time stamp when the report was transferred successfully to the ERP
        WebService
An individual thread in the ALCIMBOOK service calls the ERP WebService with the content of these
tables as parameters. The ERP WebService transfers this information to the ERP system.




A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                   55
6.1. Activation
To switch on fileless reporting in A+W Production, the switch [ALCIM_STATE / ERPFEEDBACK] = 1
must be set:




Figure 6-2- Switch [ALCIM_STATE / ERPFEEDBACK]



6.2. Reporting of batch status
This replaces the old reporting via STSL files. With the parameter Status Registrations, the A+W
Production batch status is defined that should be reported.




Figure 6-3 Parameter Status Registrations

The following status is sent to the ERP system:
    •   100      roughly scheduled
    •   150      scheduled in detail
    •   200      released
    •   300      in production
CAUTION: The behavior of batch status 300 has been improved in Version 6.0 (#318353). As soon
as the first process is booked for a lite, the batch status is set to 300 and the batch status in table
FEIN_LOS is also updated. In addition, an entry is generated in table ERP_RUECKMELDUNG in order
to trigger the fileless reporting in the ERP system. Before Version 6.0,
the status and the reporting of the status 300 did not work right!
CAUTION: If the batch status is set manually via the dialog, only a report
for status 300 is written to the ERP system! Any higher status was not
reported! This was corrected with two hot fixes in AWP5.4 (#341677).




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                                56
6.3. Reporting of production status
This replaces the old reporting via STSD and STSB files. Only the stati "produced", "packed", and
"sent" are reported.
The reporting is triggered if the processing on a lite is booked in the PDC system. For each item, the
status is sent with the precise booked quantity depending on POOL_BEARBEIT.FINAL_KZ.
 Reporting     Description       Condition                        Condition
 status                          POOL_BEARBEIT.FINAL_KZ           BEARBEITSTAMM.AW_BEARBTY
                                                                  P
 700           Produced          1                                Processing before processing
                                                                  with AW_BEARBTYP = 1800
 800           Packed            2                                1800
 900           Sent              3                                1810
A correct configuration of the column assignment in the PDC system is required.
For breakage reporting, 3 entries in ERP_RUECKMELDUNG are triggered. For each status
(700,800,900) an entry with the correct quantity of lites.


6.4. Reporting of intermediate production status
Intermediate production stati are stati between the production start and the final processing before
packing:
Roughly scheduled, released, in production, cutting, seaming, drilling, tempering, packing, delivery
xxx = batch status
xxx = intermediate production status
xxx = production status
Normally such stati are displayed in special views in the ERP system via the PPS WebService. For
particular reasons, this information is not sufficient (e.g. in order to update the time management
in A+W Business)
In order to switch on the intermediate production status, the switch [ALCIM_STATE /
ERP_DETAILED_FEEDBACK] = 1 must be set.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                 57
Figure 6-4 Switch [ALCIM_STATE / ERP_DETAILED_FEEDBACK]

In the master data for the registration points, a “tool for order entry“ must be assigned and the
"processing report" activated:




Figure 6-5 Master data registration point for processing reporting

The value from “tool for order entry“ is sent via ERP_RUECKMELDUNG as "machine" to the ERP
system (ERP_RUECKMELDUNG.MASCH). The status of the intermediate product is always 300
(ERP_RUECKMELDUNG.STATUS).
CAUTION: This function has been available since A+W Production Release 6.0 in combination with
A+W Business!
CAUTION: Watch out if you are working with "clean-up registration points" in order to book
processings that were done but not booked. Example: the user has cut the glass but not booked it
into the system. In the column assignment, the cutting processing is assigned to the registration
point 16 (installed). If the IG is now produced on the A+W Production Terminal IG-In and IG-
Assembly, the processing cutting is booked as completed. BUT: the registration point 16 is not
configured for reporting (which is also not possible since various processings are assigned to the
registration point, but only one “tool for order entry“!). This will cause different quantities in A+W
Business and A+W Production!


6.5. Report of rack allocations
This replaces the old reporting via STSG files. To switch on rack feedbacks, the switches
[ALCIM_BDESETTINGS / FEEDBACKEMPTYRACKS] = 1 and [ALCIM_SETTINGS / RACK_FEEDBACK] = 1
must be set:




Figure 6-6 Switch rack feedbacks

It is also necessary to switch on the rack feedback for particular registration points in the master
data...




A+W Software GmbH                       EN-CONFIG-A+W Production.docx                              58
Figure 6-7 Master data Registration point for rack feedback

... in order to ensure that the rack assignment is sent to the ERP system. In our standard system,
this switch is set to registration point 2910 (dispatch).
The reporting is written to the table ERP_GEST_MELDUNG with the following status:
 Status     Description            Condition
 0          Rack is back         If a rack with status "delivered" loses its status due to some
            “OnSide”             booking as with a "begin" booking to registration point dispatch
 900        Rack assignment      If a rack is booked to a registration point with switched-on rack
                                 feedback
 950        Delivered            If status "delivered" is booked to a rack
            "Off-premises"       If a rack is booked to a registration point that is linked to the status
                                 "delivered" (like 11-Off-Premises)
                                 If the delivery address is changed for a delivered rack via A+W
                                 Production Terminal
CAUTION: there is no rack feedback, only when booking a lite to a rack (regardless of which
registration point) or booking of a processing!
CAUTION: status 900 for rack feedback has a different meaning than status 900 for "production
reporting"


          Rack feedback with extended workbench
With another switch, starting with booking version 13.04.5452, a restriction of the "packed"
message (status 900) and the sent message (status 950) is possible:




If the switch is set, there is a rack feedback with status 900 (or 950) only if there are lites with
already-booked packed processing on the rack (or packed processing).


A+W Software GmbH                      EN-CONFIG-A+W Production.docx                                  59
For the rack assignment, only the packed (or sent) lites are taken into consideration.
This switch is helpful if you are working with the extended workbench (EWB). Racks for the EWB
are booked to the registration point dispatch and delivered; however, there may be no feedback
for these racks. The lites on the racks of the EWB have the processing pack EWB (AW processing
type 1805) or send EWB (if this processing exists), but not pack or send. Thus with set switch, there
is no feedback for racks of the EWB.
If there are processings pack EWB and send EWB on the header part too, it has to be prevented
that during booking in dispatch (or to delivered) both processings pack EWB and pack (or send EWB
and send) are booked simultaneously. This is achieved by including the processing types pack EWB
and pack (here 1804 and 1800) and send EWB and send (here 1805 and 1810) in the list of
processing types for which only the first open processing in the sequence is booked. If a rack is
booked in dispatch, then with the first booking only the processing pack EWB is booked; with the
next booking in dispatch, the processing pack:




Starting with booking service version 13.04.8826 and ERP webservice 13.04.6030, a feedback for
racks of the EWB is also possible. For this, a processing type send EWB has to be configured:




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 60
Using the booked processings of the lites on the rack it is decided whether a feedback for the EWB
should occur. For the EWB, a function AWCapacitySetRackInfoForPart() is called in the ERP
webservice. The tuple numbers of all lites on the rack are also transferred to this function.
The processing type pack EWB is recognized on the AW processing type 1805 or on the configured
processing type pack EWB.


6.6. Reporting of stock lites
This replaces the old PRODDAZ/PRODDUZ file reporting. The reporting must be switched on in
XOPTON.CFG:
       [Cutting] WriteXoptRueckmeldung
               0 = no feedback information for ERP
               1 = feedback information for ERP if the pattern is shown by XTV.
               2 = feedback information for ERP if the pattern is confirmed by XTV.
               3 = feedback information for ERP if the transfer of the cutting code has been started
               for the pattern. You may use this mode if no XTV is installed.
Reporting is also possible for a cutting table without A+W Production Realtime Optimizer. Reporting
is done during the first booking of a processing to a part of a batch and is done for all tables
configured in the batch. So that this works, the detailed planning must fill the table
XOPT_USED_JUMBO, switch [FEIN_SPECIALS / USEDJUMBO]. In the ALCIMBOOK switches
[ALCIMBOOK / TABLEIDSXOPTFEEDBACK] the IDs of the cutting tables without A+W Production
Realtime Optimizer must be configured for reporting in a comma-separated list.




A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                 61
Figure 6-8 Switch [ALCIMBOOK / TABLEIDSXOPTFEEDBACK]

CAUTION: if the fileless reporting for stock lites is activated as described above, the reporting via
files must be switched off in XOPTON.CFG. Otherwise, both reporting types will work, which causes
doubled stock lite removals!
       [FeedBackFile] FeedBackFileType=0
              0 = No feedback file will be created


6.7. Reporting from goods receipt
In A+W Production under master data – configuration in the Parameter Administrator under A+W
Production – PDC booking service under processing type for goods receipt, the value 9090 must
be set; otherwise there is no reporting by the booking service to A+W Business.




Figure 5-9 Processing type for goods reporting




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                               62
6.8. A+W Business
Using the fileless feedback it is possible to display the production progress of an order directly from
A+W Production in A+W Business. The data for the new production overview come directly from
A+W Production (online). The status for an Item / Order or Rack is updated by the result of the
fileless feedback.




Figure 6-9 A+W Business Feedback Process

The ERP WebService fills the tables FS_POOL and FS_POOL_KOPF. The interface service (AIS or the
new Exchange Service) processes both tables and writes the result in the A+W Business database,
e.g.: BA_GESTELLE_AUFTR = rack content and customer.
ATTENTION: some feedback takes several minutes to be processed. So you have to be a bit patient
until the result arrives in the system. You can see in the field FS_POOL.STATUS whether or not the
feedback has been processed by the AIS:
 FS_POOL.STATUS         Description
 0                      Not processed
 1                      Successfully processed
 2                      Error
 3                      Locked
ATTENTION: the fileless feedback is strictly necessary for the surplus function!


         Configuration
To activate the fileless feedback, you have to set up some master data:




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                   63
Figure 6-10 A+W Business Configuration Feedback

100-300 = batch status
400-500 = intermediate production status
700-900 = production status


          FS_POOL
All feedback is stored in the table FS_POOL. The content depends on the type of feedback.
Rack feedback:
 Column          Content
 ID              File number. All entries with the same ID coming from the same feedback.
 SEQUENZ_NR Sequence inside one feedback. Record with sequence=0 determines the
            customer who will get this rack (first lite from the rack)
 DATENSATZ       -   Booking mode: 1= rack entry, 2 = nothing, 3 = rack load / rack-content, 4 =
                     rack exit, 5 = change of rack content


A+W Software GmbH                  EN-CONFIG-A+W Production.docx                              64
                 -    Rack name
                 -    Timestamp of booking
                 -    Order number
                 -    Item
                 -    Quantity
                 -    Barcode
                 -    Accessories
 STATUS          0 = not processed
                 1 = successfully processed
                 2 = error
                 3 = locked


          Production overview




Figure 6-11 A+W Business Open production overview

Old                                                                  view:




Figure 6-12 A+W Business Old production overview




A+W Software GmbH                    EN-CONFIG-A+W Production.docx     65
New                view                (based                 on               a    report):




Figure 6-13 A+W Business Production overview based on a report

Configuration of report in the master data [Master data / Company / Company Data] use Folder
[13. Production]:




Figure 6-14 A+W Business Configuration Production overview based on a report

Classic view:




Figure 6-15 A+W Business classic product overview




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                       66
          Delivered racks




Figure 6-16 A+W Business view delivered racks



6.9. A+W Enterprise
The fileless feedback is only available with A+W Enterprise <-> A+W Production. It is not possible to
work with the fileless feedback with ALCIB/PMS.




Figure 6-17 A+W Enterprise feedback process


          Configuration
PMXTVRLOESCHOPT
In A+W Enterprise the information is required how long an optimization job may be valid, or when
it is possible that a new job is be created with the same number. For this, activate the ALCIB
parameter PMXTVRLOESCHOPT and assign a value indicating the number of days. If the parameter
is not set, a default value of 30 days is applied. Read more information to ALCIB in Chapter 4.2 of



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 67
\\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity\Installation_Configuration\TU_090
327_IstConfigListAlcibAlcimOrderXML_129902.doc.
AWC_ALCIM_ANBINDUNG
This parameter has to be activated. Without this the complete function (communication with
AWCapacity, OrderXML) will not work. Since ALCIB2011, no CommonBase is supported anymore,
so the following parameter must be set:
-   AWC_ALCIB_SERVER_NAME
-   AWC_PORT_RPC_DIENST
-   AWC_PORT_CONTROL_SERVER (you will find the ports in: /etc/services).
AWC_FIXIERT_AB
Specifies the ALCIM status from which on an order item is to be regarded as fixed in production,
and hence cannot be edited anymore. Will lead to ALCIB status 300. Standard value 552.
AWC_FREIGEGEBEN_AB
Specifies the ALCIM status from which on an order item is to be regarded as released, and hence
cannot be edited anymore. Will lead to ALCIB status 302, which cannot be reset anymore. Standard
value 554.
AWC_BUCHE_KPOSPROD
If this flag is activated, the table KPOSPROD will be filled after each processing feedback.
AWC_GESTZU_BUCHEN
If this flag is activated the table GESTZU will be filled after each rack feedback.
AWC_IGNORIERE_GESTELLMELDUNG
Is the parameter set to ON, no rack feedback will be transferred into ALCIB table BCBOCK. The ALCIB
parameters GESTELL_BDE, MODUL_STAPELLOGIK and AWC_GESTZU_BUCHEN are ignored. This is
needed if ACLIM can’t guarantee that the feedback of racks isn’t numeric. ALCIB can’t work with
alphanumeric racks.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                              68
6.10.            A+W Cantor




Figure 6-18 A+W Cantor feedback process

For the feedback, a directory has to be defined, in which the XML file of A+W Production is stored.




Figure 6-19 A+W Cantor configuration feedback directory

In addition to the configuration of the directory, a system maintenance queue has to be set up.
System queue 50 can import various formats. Parameter 4 is important for XML response. The
following options are available here:

  Value   Description
  1       A+W Pool STSY ASC
  2       A+W Pool FEIN ASC
  3       A+W Pool STSY ASC (Kunde)
  4       Rack feedback from A+W Production




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                              69
Figure 6-20 A+W Cantor configuration system queue



6.11.            A+W Cantor CIM
The following master data has to be set up in A+W Cantor CIM:
Part Additions
In the master data of terminal group configuration, the part additions 3 and 36 have to be entered.




Figure 6-21 A+W Cantor configuration part additions

Part addition 3 saves all rack information for a fitting field. If there are several lites in this field, the
rack information is separated by commas. Part addition 36 saves the rack information for a glass
field. Which part addition is shown depends on the data procurement of the terminal group.
Terminal group
Both part additions have to be entered in the terminal group:




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                       70
Figure 6-22 A+W Cantor configuration terminal group

Therefore, these two variables are available in the Designer:




Figure 6-23 A+W Cantor rack group designer

Result
If the worker now scans a barcode, the rack information is shown on the terminal group.




Figure 6-24 A+W Cantor rack group result

         The data of the feedback is saved in the respective CIM scheme in the table
         CPB_TEILZUSATZ.



A+W Software GmbH                    EN-CONFIG-A+W Production.docx                        71
                  Configuration in A+W Cantor
PRODCONF
    PRODCONF      Description                                                      Possible values
    599           Releases the system action for the feedback file of A+W          0.1
                  Production.
CANTOR.INI

    Section              Entry            Value   Description
    DIRECTORIES          AlcimImport              Here it is specified in which directory the feedback file
                                                  of A+W Production is imported.


                  Configuration in A+W Production
Rack feedbacks will only be created for out-of-house booking in A+W Production. To activate the
file-less feedback in A+W Production you set the following parameter:
•      [ALCIMBOOK / CANTOR_RACKFEEDBACK] = 1
•     [ALCIMBOOK / CANTOR_FEEDBACKPATH] = $SERVERDIR$\EXPORT\ (Standard)
•     [Data import (Item4Alcim) / CREATE SN FILES ] = 0




Figure 6-25 A+W Production parameter for A+W Cantor rack feedback


                  Result
A file will be created with the name RACK<timestamp>.XML in the following format:
     Attribute                     Data type      Length        Description           A+W source

     <?xml version=”1.0” encoding=”UTF-8”>

     <RACK_RESPONSE>                                            Root level

     <RACK>                                                     Rack element

     RACK_ID                       Char           255           Rack ID



A+W Software GmbH                      EN-CONFIG-A+W Production.docx                                     72
  Attribute                      Data type     Length    Description              A+W source

  <SLOT>                                                 Slot element

  SLOT_ID                        Int                     Slot ID

  <GLASS id=”1”>                                         Glass element
                                                         The attribute ID is optional: if several lites are found in
                                                         one location.
                                                         First pane in slot ID=1, second pane in slot ID=2 etc.

  GLASS_BARCODE                  Int                     Optional: If several
                                                         lites are found in one
                                                         location.

  ORDERER_ORDER_NO               Int                     Order number        of   CANTOR:
                                                         purchaser.               AUFPOS.AufNr              (transl.
                                                                                  orderitem.order#)
                                                                                  OrderXML: Textid 6009

  ORDERER_REFERENCE_ITEM_        Int                     Reference      item      CANTOR:
  NO                                                     number of purchaser.     AUFPOS.RefPosNr        (transl.
                                                                                  orderitem.referenceitem#)
                                                                                  OrderXML: Textid 6010

  ORDERER_FIELD_NO               Int                     Field number        of   CANTOR:
                                                         purchaser.               AUFART.LfdNr            (transl.
                                                                                  orderarticle.sequence#)
                                                                                  OrderXML: Textid 6004

  ORDERER_PIECE_NO               Int                     Quantity of purchaser    CANTOR:
                                                                                  AUFPOS.Stck               (transl.
                                                                                  orderitem.pieces)
                                                                                  OrderXML: UDX.AW -> Amount

  </GLASS>

  </SLOT>

  </RACK>

  </RACK_RESPONSE>
RACK_ID: the rack name from the field AWBAR_GESTELLE.GESTELLNAME.
The following information is created for each lite:
SLOT_ID: For slot carts (rack with AWBAR_GESTELLE.TYP_KZ = 1), the slot number is filled from the
field AWBAR_TEILE.FACHNR. If there are no slot carts, then SLOT_ID is filled with the sequence of
the lites according to booking, beginning with 1.
ORDERER_ORDER_NO: The values for the order and item number of a lite are read from the
database field POOL_TXT.TEXT. The order number is taken from the data record with
POOL_TXT.TEXT_TYP = 6009. If no data record exists for 6009, no feedback is written for this lite. If
there are several data records 6009, feedback is written for each data record.
The value for the order and the position of the lite are determined from the field POOL_TXT.TEXT
with TEXT_TYP = 6009. If a data record for the position does not exist in table POOL_TXT with

A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                     73
TEXT_TYP = 6009, a feedback file will not be created for this lite. If several data records exist with
TEXT_TYP = 6009, the POOL_TXT.TEXT is determined for any one of these data records and written
into the element ORDERER_ORDER_NO.
ORDERER_REFERENCE_ITEM_NO: Same               behavior    as   switch   ORDERER_ORDER_NO,         but
POOL_TXT.TEXT_TYP = 6010 is used.
ORDERER_FIELD_NO: Sam behavior as switch ORDERER_ORDER_NO, but POOL_TXT.TEXT_TYP =
6004 is used.
ORDERER_PIECE_NO: The total from POOL_POS.MENGE of all data records that belong to the same
commercial item (POOL_POS.AE_INTPOS) of the lite.
Caution: Feedback is only generated fro lites where data records from POOL_TXT.TEXT_TYP 6004,
6009 and 6010 exist. The file is initially created with the extension TMP and renamed XML when it
is written completely. The file name contains a time stamp. Errors that occur when writing the file
are logged in the trace of the booking service.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                  74
7. A+W Realtime Optimizer
7.1. Multiple user login
In the A+W Realtime Optimizer, one or more users can be logged into the 'PDC' for evaluation for
each configured cutting table. When closing the A+W Realtime Optimizer, all users must be logged
out so that the A+W Realtime Optimizer can be closed. Registration is done via the main menu bar
Settings > Tables > Login on a separate dialog. It can be configured that at least one user must be
logged in to start the cutting process.
In order to activate the PDC user login in A+W Realtime Optimizer, the following requirements must
be met:
    •   The PDC must be active.
    •   Open the Parameter Administrator in A+W Production via the menu Master Data >
        Configuration.
    •   In A+W Production Terminal both the parameters "Person for 'Logged off'" and the
        "Registration point for 'Logged off'" must be set in section 'Bookings'.




6-1 Configuration in A+W Production for multiple user login in A+W Realtime Optimizer

    •   The     "Albwir.Alcim.GlobalForms.dll",    "Albwir.Alcim.Designer.dll"   and     the
        "DataBaseReader.dll" must be available in the program directory of the A+W Realtime
        Optimizer.
    •   In the xopton.cfg under %AppData%\Roaming\A+W\TECHSOFT\Xopton in the section
        [BDE], the following switches have to be configured:
             o   Mode > 0
             o   BdeUserSignIn=Y
             o   BdeUserSignInMandatory=N / Y
                 N: No user must be logged in to start the cutting                        process.
                 Y: At least one user must be logged in to start the cutting process.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                             75
8. A+W Barcoding
8.1. Background printing and e-mail dispatch
The booking service can be used to print reports and send e-mails.

The ProcessManagerService participates in the process, the one that controls the report generation
and sends e-mails. The CrystalReport runtime is required in order to create the reports. The booking
service decides using the configuration whether a report should be created and sent and write the
order into the table PROZESSE. ProcessManagerService evaluates the table PROZESSE and creates
the reports and sends them.

The configuration and conditions that trigger the background printing are specified in the
parameter administrator:

In the section 'A+W Production -> General -> Mail Settings' the connection data of the mail server
used by the ProcessManagerService to send mails is stored.




Figure 8-1 Connection data of the e-mail server

The section 'A+W Production -> Barcoding Booking Service -> General->Print of Report' defines the
conditions that must be met for a mail to be sent and the parameters of the mail stored.




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                             76
Figure 8-2 Configuration of the booking service for e-mail dispatch and background printing

The following mail parameters must be specified:

    •    Report
         The file path to the CrystalReport file that will be attached as PDF attachment to the e-mail
    •    Recipient
         Address to which the generated e-mail should be sent
    •    Object Type
         The 'Object Type' must be specified. It determines which object (lite, rack or registration
         point) is to be observed for changes in its properties.
    •    Station                                                                                group
         The station group specifies which instance of the ProcessManagerService executes the
         background printing and sending of the e-mail. The instances offered are specified in the
         section 'A+W Production-> Release Dialog-> Group of Executing PCs'.

The following parameters are optional:

    •    Printer
         If a printer is specified, in addition to the e-mail, the report will also be output on this printer
    •    Mail subject
    •    File                    path                    for                  mail                  content
         Path to a TXT file whose content will be copied into the e-mail



A+W Software GmbH                      EN-CONFIG-A+W Production.docx                                      77
    •   Additional                                                                             fields
        Field content of the booking record that can currently be evaluated by the booking service
        can be transferred to CrystalReport. The 'Additional fields' parameter specifies which fields
        from the table AWBAR_BOOKING should also be transferred to the report.

Conditions that can be specified in order to generate a mail:

If one of the parameters is configured, then only an e-mail is generated if the booking is of the
corresponding parameter type.

    •   Stati
    •   Status Type
    •   Registration point
    •   Registration point type

Report definition

The report used must absolutely have a string transfer parameters with the name "Barcode". In
this, the bar code of the defined object type from booking is transferred.




Figure 8-3 Parameter configuration in Crystal Reports



8.2. 15-digit Gestellpool Europe barcodes
          Configuration in A+W Production
In order to be able to use 15-digit Gestellpool Europe barcodes in A+W Production, various
adjustments must be made in the database.
The following DB update scripts must be present in C:\Program Files (x86)\A+W\Techsoft\sql\XML:



A+W Software GmbH                     EN-CONFIG-A+W Production.docx                               78
    •   awupdate_alcim_2_626.xml
    •   awupdate_alcim_2_627.xml
    •   awupdate_alcim_2_628.xml
    •   awupdate_alcim_2_629.xml
    •   awupdate_alcim_2_630.xml
    •   awupdate_alcim_#389903_-1_-1.xml
The standard scripts with the numbers 2_626 to 2_630 cause the enlargement of all database fields
that contain the rack barcode. The customer-specific script with the number #389901_-1_-1
enables the processing of alphanumeric barcodes. Instead of the master data for barcodes
(BC_Types), a new table is created here, in which it is also possible to recognize racks with a regular
expression. This means that a rack does not always have to be precisely 9 characters long and begin
with a 3.
Attention!
With this solution, the master data dialog for racks and the one for barcode types do not work
anymore. Production Terminals, label printing, etc. were not considered in this solution.
After the DB update has been done, the following insert must be executed:
insert into awbar_barcodetypen (nummer,typ,name,laenge,pruefziffer,codetyp,[status],regex,
praefix,ersetzungsmuster) values (1,3,'GESTELL',15,0,0,0,1,'([0-9]{15})$','');
Then the table awbar_barcodetypen looks as in Abbildung 7-1




Figure 8-4 DB table awbar_barcodetypen




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                   79
          Configuration in A+W Smart Companion
In order to be able to process 15-digit Gestellpool Europe barcodes in the AWSOA database, a Regex
adjustment must be made in the configuration of the infrastructure Web under A+W Production -
> CIMScannerSettings in the Barcode Classification.
Please download the current configuration.




Figure 8-5 CIM Server Settings

Open the downloaded configuration with Notepad++.




Figure 8-6 Regex configuration

The entry for the "Regular Expression" for "Rack Barcode (Gestellpool Europe)" must be adjusted
as follows:
"RegularExpression": "([0-9]{15})$",
"Substitution": "$1",
"Description": "Rack Barcode (Gestellpool Europe_long)"




A+W Software GmbH                 EN-CONFIG-A+W Production.docx                                80
Figure 8-7 Regex adapted

After the entry has been adjusted, please save it. Now upload the configuration file within the
infrastructure web under A+W Production -> CIMScannerSettings in the Barcode Classification.




Figure 8-8 Uploading the new configuration
After uploading the configuration, you can see the change under the Barcode Classification 4.




Figure 8-9 New configuration
The configuration is saved automatically by the uploading.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                             81
8.3. Breakage booking with incomplete assembly
   message
If a unit (IG, LAMI or cast resin) is reported broken whose assembly has not been booked, then no
remakes are generated for the subparts of the unit. The subparts are missing in the breakage
pool. To prevent this, it is now possible instead of the breakage booking to book a configurable
state to the unit. The break is initially not booked; instead, the unit appears in the remake hand-
ling. The breakage booking is not made if at least one subpart (glass item) has not been assemb-
led. Missing non-glass items (frames or foils) will not be taken into account. The booking in the
remake handling is only made if the breakage reason is of a type that inserts records into the
breakage pool. If an assembled IG is booked as broken, which contains a non-assembled LAMI,
then the LAMI is booked in the remake handling. The IG with its other subparts will be booked as
broken.

In the remake handling, you can filter by the state for non-assembled lites. In the detail list, the
part is displayed with its subparts. The option for re-use is not available since the part is already
physically broken. Any subpart can be assigned a still-available label number. Then the break can
be booked after the fact, the subparts appear in the breakage pool.

The new behavior is activated by the switch STATUSBARCODENOTASSEMBLED in the parameters
for the booking service. Here the state barcode for non-assembled lites is specified. This state
may not be a breakage reason, the state type also has to be AWBAR_ZUSTANDTYP.BRUCH-
FLAG_TYP = 0. Here the state should be configured, which causes a booking in the remake hand-
ling.

An update of the booking service is not sufficient. The display and bookings of the remake hand-
ling have also been changed. There is no additional switch for the remake handling. Since labels
have to be assigned, the existing switch for the dialog mode (expert mode) has to be set to 1.


8.4. Consideration of the timestamp of bookings
By default, location bookings or state bookings are not executed if for the registration point, the
rack or the lite a different booking with a newer timestamp has already been made. Now the boo-
king timestamp can be ignored with a switch. The bookings are then made regardless of their ti-
mestamp.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                   82
8.5. Messages from bookings to the Smart Factory
Bookings to the Smart Factory can be reported from A+W Production Booking.
The messages are activated with a switch in the parameters for the booking service:




If the switch is set, the following types of bookings will be reported:




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                     83
          Lite at registration point
If the registration point of a lite changes, this is reported. The message includes the label of the
lite, the number of the registration point, and the time stamp of the booking. Here it doesn't mat-
ter due to which type of booking the registration point changes. This can be a booking lite at re-
gistration point or rack at registration point or a status booking due to which the registration
point of a lite changes. No restriction to particular registration points is provided. The Smart Fac-
tory will only react for particular registration points, for example, for an IG line. This can be confi-
gured accordingly in the master data for the Smart Factory.


          Booking of the processing "packed" or "sent"
If for the last lite of an order and a production item the processing "packed" or "sent" it booked,
then a message is issued. The message includes the order number, item number, and time stamp
of the booking. Furthermore, the report includes the type of booking, that is, "packed" or "sent".
This message can be used in the Smart Factory to initiate an archiving.


          Fraction calculations
For a breakage booking, the label of the lite, the number of the registration point, and the time
stamp of the booking are also reported. The reported registration point is the late one before the
breakage recording point 19.


          Booking of a state of the type "reuse"
Booking of a state of the type "reuse" ("prolonging") on a lite is reported. The message includes
the label of the lite, the number of the registration point, and the time stamp of the booking. If
the lite is installed and is at the registration point "installed" (16), the last registration point be-
fore 16 is reported.
This state is booked for a lite that can be reused after a break, which should be fed back into the
automatic process of the Smart Factory. "Reuse" can be booked directly to a lite or via the remake
handling.
The booking service detects the state of this type on the field AWBAR_ZUSTANDTYP.FUNKTION-
TYP = 3.
Set-up of a state type "reuse":
In the master data for the state types, a new state type for "reuse" ("prolonging") must be crea-
ted if it does not already exist. The state type for representation (re-use) can be used as a temp-
late. Decisive is that the "function" is set to the value 3. If the 3 cannot be selected, the table
TEXTE must be updated.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                        84
In the master data for the states, a state must be created that is assigned to the state type
"reuse".
Set-up of the remake handling for the booking of "reuse":
In the parameters for remake handling, a state for the booking of "reuse" can be specified.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                               85
If for an IG from the remake handling "direct remake" is selected, then for the sub-parts of the IG,
the original procurement type (cutting), reuse or prolonging can be selected. In case of reuse or
prolonging, a registration point and a rack can also be specified.




A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                  86
9. Remake handling
This document describes how "partial defect" works and all the individual steps that are required
to start up this function. Some of these steps are already set in the default database between the
A+W Production Terminals. These are listed here only for better understanding and troubleshoo-
ting, or they are supposed to serve as help in case of an update from an older version.
Previously, the concept of partial defect was also called "rough scheduling remake" or "OP
remake".
The partial defect should essentially fulfill two requirements:
    a)      The possibility to report only parts of an assembled product as broken (partial defect)
    b)      Via an editor, to decide what should be done with the individual parts of the remake
            (via a new item in the pool (OP remake) or immediate reproduction, etc.)


9.1. Mode of Operation / Operation
         Booking of a partial defect
The booking of a partial defect can be done via an A+W Production Terminal or a scanner. Here a
status booking of the type 40=partial defect must be made. The booked component is thus
booked to the registration point 40=defectpool and can then be processed further in the remake
handling.


9.2. Configuration
         A+W Production parameters
In A+W Production, under "Master Data, Configuration, Parameters, PDC Booking Service, Activa-
tion Rough Planning Remakes=1" the OP remake is activated (or "Enable Rough Scheduling
Remake").
In the parameter table, the entry is under Bereich=ALCIMBOOK und Eintrag = NACHLAUFPOS


Under "Master Data/Configuration/Parameters/A+W Production/General/Parameter Record PPS
Remake Dialog" you can set which parameter set you want to use (Default = AUW_PPSREMAKE).
In the parameter table, the entry is under Bereich=ALCIM_SETTINGS and Eintrag = PARAMETERSE-
TREMAKEDIALOG:




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                87
          PDC master data
Registration point types
Type 80: Defect Location
All registration points are assigned to this registration point type that are regarded as causing de-
fect location. This is not always the registration point at which the defect was booked (optional).




Type 40: Defect Pool
This registration point type is only introduced so that you can distinguish the defect pool from the
"normal" registration points. Only thus is it ensured that it is not displayed incorrectly for registra-
tion point filters in the A+W Production Terminal.




Registration Points
RPNO 5: Production
Is the default outgoing registration point for lites that can be reused.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                   88
Type 40: Defect Pool
Lites that are on this registration point are displayed in the remake handling. Reports can also be
set to this registration point. The evaluation via the registration point is simpler and performance
is better (index!) than via status types.




RPNO 81/82: Defect Location 1-2




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 89
Status Types
Type 40: Partial Defect
This controls that all partial defects are booked to the registration point "Defect Pool". Thus the
editor for the remake handling can be executed with better performance.




Type 60: Re-Use
This function ensures that the procurement types of the AV remakes are set correctly.
If the function "02-ReUse" is not present, the current texts must be loaded into the database (or:
INSERT INTO texts (modul, idnum, idtext, sprache, format, status) VALUES 'ASWTZUSTANDFKT-
TYP', 2, '2', 'Wiederverwendung', 'GER', 0, 0)).




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                     90
Stati
Status 40: Partial Defect
At least the status 40-Partial Defect of type 40-Partial Defect is required. Naturally additional stati
of the same type can also be created. This status is booked by the break recorder in order to book
the part into the remake handling.




State 50: Re Use




          Parameter Administrator dialog




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                   91
Parameters for the main dialog (misc)
Surface              AUW_PPSRemakeDialog_Main

Selected Tables      AWBAR_TEILE:AWBAR_ZUSTAND:AWBAR_ZU-             Tables from which data can be selected for the
                     STANDTYP:POOL_TEILE:AWBAR_STEL-                 main dialog
                     LEN:POOL_POS:AWBAR_PERSON

FROM Clause          AWBAR_TEILE, AWBAR_ZUSTAND, AWBAR_ZU-           Dto.; but these entries are relevant for internal Sel-
                     STANDTYP, POOL_TEILE, AWBAR_STELLEN,            ect!
                     POOL_POS, AWBAR_PERSON

Fixed SQL-Filter     awbar_teile.zustandnr=awbar_zustand.zu-         Here, it will be joined into awbar_stellen via
                     standnr and awbar_zustandtyp.typ=awbar_zu-      awbar_teile.esnralt to display the name of the re-
                     stand.typ and                                   gistration point where the reject happens

                     awbar_teile.auftnr=pool_teile.auftnr and
                     awbar_teile.pos=pool_teile.pos and
                     awbar_teile.u_pos=pool_teile.u_pos and aw-
                     bar_teile.teilenr_min=pool_teile.teile_nr and

                     awbar_teile.auftnr=pool_pos.auftnr and
                     awbar_teile.pos=pool_pos.pos and

                     awbar_teile.esnralt=awbar_stellen.esnr and

                     awbar_teile.esnr=awbar_zustandtyp.esnr and

                     awbar_teile.personnr = awbar_person.personnr
                     and

                     awbar_teile.esnr <> 0




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                            92
Automatic Update          False                                            Defines whether the dialog will be updated auto-
                                                                           matically

Update Frequency          180                                              Interval in seconds to update the dialog

Edit Dialog               AUW_PPSRemakeDialog_Edit

Rebook Dialog             AUW_PPSRemakeDialog_BookStateDialog

Status type for broken    40                                               Status bookings of this status type are moved to
parts                                                                      remake handling

Status barcode for        500000010
„Rejects“

Status barcode for        500000060                                        Parts that can be reused are booked with this sta-
„Reuse“                                                                    tus

Waiting time for book- 10                                                  Time in seconds that the booking service waits until
ing confirmation                                                           the booking was processed in awbar_booking. In
                                                                           case it takes longer a message appears.

Dialog Mode               0                                                0 = safe mode (only assembled parts are displayed)
                                                                           1 = expert mode (complete BOM is displayed)


Parameters for processing dialog:
Selected tables               AWBAR_TEILE:                                 Tables from which data for the processing dialog
                              AWBAR_BEARBEIT:                              can be used
                              BEARBEITSTAMM

FROM Clause                   AWBAR_TEILE,                                 Dto.
                              AWBAR_BEARBEIT,
                              BEARBEITSTAMM

Fixed SQL-Filter              awbar_teile.etikettnr=awbar_bearbeit.eti-    According to this, only processings are displayed
                              kettnr and bearbeitstamm.artnr=awbar_bear-   that were already reported. Only these can be
                              beit.art_nr and awbar_bearbeit.fertig=1      repeated

Types for Registration        200,300,600,…..                              This limits the registration points that can be used
Point                                                                      for parts (normally the registration points in the
                                                                           production area)

Types for Reject Regis-       80                                           This limits the registration points for the defect lo-
tration Point                                                              cation. Defect location = registration points at
                                                                           which the break should have happened

Status Types for Reject       4                                            Reasons for defect that are communicated with the
Reasons                                                                    part on the dialog after the processing

Filter on Part Types          10                                           If you do not want to see the films or frames, you
                                                                           can suppress these part types here. By default, the
                                                                           LSG films (ttype=10) are suppressed
                                                                           WARNING: If the frames are suppressed here, they
                                                                           are also not considered for a remake item (excep-
                                                                           tion: the IG is previously assembled with the
                                                                           frame). If the frame is not considered, there will be
                                                                           no bending data in the new item since the frame
                                                                           has the procurement type "ignore"!




A+W Software GmbH                          EN-CONFIG-A+W Production.docx                                             93
9.3. Operation of the remake handling
          Remake handling
Remake handling is on the Options menu element in A+W Production:




          Display
In the top list, the dialog for remake handling displays all lites that are in the remake handling.
These are all lites that have a state type that can be configured in the parameters. Several state
types can be configured.




Display in the detail list:
The detail list is filled if a lite is selectd in the top list. The display and the possible actions depend
on several switches.
With a switch, particular part types can be excluded from display in the detail list. For example,
spacers or foils can be excluded from the display.




Depending on which part is selected, the detail list is filled differently.
IG with installed lites:


A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                      94
For an IG with installed lites, the IG and the installed parts are displayed in the detail list. All ac-
tions "reuse" "scheduling remake" and "direct remake" are possible.




Purchased IG:
For a purchased IG, only the IG is displayed, all three actions are also possible.
Non-produced IG:
For an IG to be produced without installed lites, the behavior depends on two switches.




If the "Display planned lites" switch is set, the IG and the parts planned for installation according
to the detailed scheduling are displayed. Here it plays no role how the switch is set for expert
mode. Prerequisite for the display of the planned parts is that none of these parts is already in-
stalled in another IG. This switch makes sense in an installation with DynOpt, where installation is
always done after detailed scheduling. All actions "reuse" "scheduling remake" and "direct
remake" are allowed.
If both switches "display planned lites" and "expert mode: are not set, only the IG will be dis-
played. Only the "reuse" action is allowed.
If the "expert mode" switch is set, the IG and its subelements will be displayed. For the subele-
ments, no fields from the AWBAR tables will be displayed; the labels are not assigned.




Subelement of an IG or TG:
If the "expert mode" switch is set, the subelement from the remake handling, the counterlites,
and the header part will be displayed. The label is only displayed for the lite from the remake
handling. All actions "reuse" "scheduling remake" and "direct remake" are possible.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                        95
If the "expert mode" switch is not set, only the subelement from the remake handling will be dis-
played. The action "scheduling remake" is not allowed.




    1) In the upper part of the screen, there is a menu bar (as in the A+W Production Terminal).
       It will be possible to attach lists here in the future.
    2) In the top data grid (Overview), there is information about the parts that were booked
       with a partial defect (status type 40) and all parts that are at the registration point 40 (de-
       fect pool).
       Blue dots in the "PP" (=purchased parts) column mark the parts that are themselves
       purchased parts or in whose BOMs there are purchased parts.
    3) If in the upper grid you select a lite, the associated BOM parts for it are displayed (details).
       Associated parts are the parts that will be installed on the selected part according to the
       PDC (according to awbar_teile.eingebaut_in). Thus, if the frame is not installed on the IG
       via the A+W Production Terminal IG Assembly, it can also be displayed and edited here.
       Expansion starting with AWP5.4: essentially the entire BOM is displayed below a part.
       Thus a decision can also be made for the associated components about how to proceed
       with them.
       Expansion starting with AWP6.3 (#376221): if the components are assembled first and
       then reported broken, the system knows which BOM parts are affected. The expansion
       from AWP5.3 leads to the fact that labels must be assigned to parts not yet assembled.


A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                   96
        The assigned labels must be removed manually from production. Errors that can happen
        during manual assignment can end in a big mix-up in production. Especially in DynOpt en-
        vironments this can result in production stop.
        For security reasons, a switch was implemented in the parameter, that allows to choose
        between 2 modes:
        switch „Dialog Mode“ (section=@PROPERTY_LOGICAL, entry=_PPSR_EXPERTMODE)
        0 = limited mode (only installed subparts are displayed)
        1 = expert mode (complete BOM is always displayed)
         see chapter Configuration

    4) With the "Rebook" button, it is possible to assign the lites in the upper data grid to
       another break reason (status). Furthermore, it is possible to provide individual lites with
       an info text. The text is saved in the table awbar_teile.infotext.




       For easier operation, it is possible to rebook or edit several selected lites simultaneously.
    5) The filter here serves to filter individual stati in the remake handling. Thus, e.g. you can
       limit the display to the reason for defect "scratches"
    6) The buttons F7, F8, F9 are macros for making a rough decision about the treatment of the
       broken lite. Details about this will be provided later


         Macros – the rough decision
In order to make operation easier, it is possible to use macros to make a rough decision about
how the subparts should be treated. The following macros are possible:



                             Reuse: This macro is used if the complete part can still be reused. That
is, the part is assigned the procurement type "reuse" and disappears from the defect pool. In the
database, however, it remains on the registration point "defectpool" (if nothing else is specified)
and it is assigned the status "Reuse" (at which point it disappears from the defect pool).



                           AV remake: With this macro, a completely new production item is crea-
ted in the order pool for this part with the original procurement types. The old production item is




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                  97
reduced in quantity accordingly so that the total quantity of the order item is correct again. This
production item can now be steered into production using rough and detailed planning.



                           Direct remake: This macro creates a "normal" break. That is, the indivi-
dual parts are treated as for a direct defect booking and must be reproduced manually (e.g. wit-
hout planning).


         Details – the fine-tuning
Using the macros, only a rough decision is made. More precise settings for each individual part
can be made with a double-click on the part or by selecting it and then clicking the "Edit" button
(F3):




Procurement Type: here you can change the procurement type of the selected parts. You can
only ever select
 between the original procurement type and "Reuse". If you select the procurement type "Reuse,"
then the drop-down box becomes "Registration-Point" and the input field becomes "Rack".
Procurement types for participating parts (that is, parts that are not booked directly as defects
but for which label numbers were assigned), the procurement type depends on the planning sta-
tus. If the planning status is < planned in detail, the part retains its original procurement type. For
planning status >= planned in detail, the procurement type is automatically "Reuse" since the part
has to be produced in its original batch anyway.


A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                     98
Registration Point: If the part can be reused, you select the location where you store the part un-
til its reuse here. This information can be displayed on the A+W Production Terminal.

Rack: Here, in addition to the registration point, a rack can be specified on which you store the
reusable part. This information is displayed, e.g. for the remaking of the entire IG on the A+W
Production Terminal IG-In instead of the logical rack number (here: rack 17):




Defect-Reason: If the part in question cannot be reused and you select the procurement type
"Production," then you can select the real defect reason here. This can then be used for statistical
evaluations.

Defect-Location: In addition to the defect reason, you can specify a defect location here. This can
be selected regardless of the registration point at which the break occurred.

Processes: Especially for processings such as screen printing, coating, etc., it can be that you do
not want to reproduce the entire lite. That is, it is sufficient to repeat individual processings:




On the "Processes" dialog, all processings are displayed that were already booked on the lite in
question. By placing a checkmark in the "Repeat" column, precisely these processings are reset in
the PDC table so that you can rebook them.



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                     99
Re-Schedule: By placing the checkmark next to "Re-Schedule", a new production item is genera-
ted in the order pool (see above)


           Assignment of real components (starting with AWP5.4)
This function is only available in "Expert Mode" (see configuration chapter).
If a subpart of an unplanned or planned product is broken, you would like to:
        a) Reschedule the corresponding BOM components (counterlites, spacer, hea-
           der parts)
        b) Be able to reschedule the individual components in the capacity planning
        c) Be able to produce the product in a new batch

If a BOM element is booked into remake management, previously you could only manage the
BOM element itself and the installed parts below it. Reason: the individual components have eit-
her no clear relationship to one another (as long as they have not been planned in detail) or only a
loose planning relationship. Nevertheless, each BOM part can be identified by a barcode, any
time. Since the counterlites can, in theory, have any (and also different) production status/stati,
the system cannot determine automatically which components must be broken out of the original
order in order to pack them in a split-off item that can be planned. But a split item is necessary to
assign via rescheduling new production dates to the individual parts.

To solve this problem, starting in AWP5.4 in case of a break of a subpart, the complete BOM is dis-
played in the remake handling. The still-unknown and not yet clearly identified components are
displayed without barcode. If the employee in this situation generates an OP remake directly, the
behavior remains as previously. That is, a new item is generated in which only the partial defect
can be planned anew and the production is done in the original.

Example:


                                        An order consists of 4 insulated glass lites. Nothing has
                                        been planned; the components still have no clear relati-
                                        onship to one another. The label No. 13 is booked in inco-
                                        ming goods as a partial defect and via the remake hand-
                                        ling as OP remake. Thus in the original item the label No.
                                        13 is marked as "defect" and a new item is created.




                                        In this item, only the part with the label number 13
                                        can be re-planned! Both parts with the "virtual" la-
                                        bel numbers 05 and 26 have the procurement type
                                        "11-Production in the original" and are thus ignored
                                        by the planning.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                100
If now in the above-mentioned situation the counterlite is an expensive (purchased) TG
that should be coated before assembly, you have to be able to stop the original coating of
the part and reschedule the production dates for the coating and the assembly with a
transfer. For this, in the new item you must assign "real" label numbers from the original
item:




Thus a new item that can be planned completely is created and the quantities are reduced ac-
cordingly in the original item:




The assignment of the real component is undertaken on the new "Edit" dialog (starting
with AWP5.4):




A+W Software GmbH                 EN-CONFIG-A+W Production.docx                                101
In order to make the assignment of the label numbers easier for the employee, this dialog
offers only the theoretically-possible label numbers with specification of batch (if present,
with current parts status), current location (registration point and rack), and the time of
the last booking.
On the new data grid, the user can inform himself about the status of the possible parts.
Depending on the production status, he now selects the "real" label number. After that
(or beforehand), he must ensure that precisely this label number is taken from produc-
tion. In addition, he can assign a new registration point to the selected label number.
Here the lite is "parked" until it is required again for production.
The procurement type of the individual parts of the new item depends on the planning
status of the original item. If the parts of the original item were still in the pool or only
roughly planned, the parts of the remake get the original procurement type so that they
can be planned anew and produced. If, however, the parts were already planned in detail
or they were in a still-higher status (released or in production), they get the procurement
type "10 Reuse from defect". The reason for this is that the parts are already in an opti-
mized batch from which they can no longer be removed. That is, the lite will be cut
anyway; the frame bent since it is in a bending file.
Parts of the remake that must be produced anew in the BOM because the subparts were
broken (e.g. TG from float, LSG, IG, etc.) get the procurement type of the original part.
TIP: Since 11/28/2014 (alcimbooking and defect.dll Build 1542) it is possible to assemble
an IG from 2 parts from the remake handling. That is, if lite 1 and lite 2 of an item are in
the remake handling, it is recommended for the processing of lite 1 to select the label for
lite 2, which is also in the remake handling. This reduces the number of remake items.

A+W Software GmbH                EN-CONFIG-A+W Production.docx                            102
         Additional buttons



                         Update refreshes the screen. In the parameters, it is also possible to set
a time after which the screen is refreshed automatically (see above).



                      Edit opens the "Edit Defects" menu on which the fine settings for the sel-
ected component can be made.



                         Back resets the last setting



                         All back resets all settings that you have made to the part.



                         Save makes the actual booking according to the settings made. That is,
as long as you have not yet pressed this button, nothing happens in the database and you can
undo your actions.


A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                103
                         Close exits this dialog


9.4. Direct booking from the Production Terminal
In the Production Terminal IG-Out, there are now 2 possibilities for defect handling:
     a) The employee selects a defect reason as previously and another employee decides in the
        remake handling what should happen with the individual parts
     b) If the employee selects a defect reason of the type partial defect, the remake handling o-
        pens directly with the current lite and the employee can then decide directly how the in-
        dividual parts should be treated. (for configuration, see below)


9.5. Database content
This section provides special fields or behaviors in the database that can help with research.


           Pool_Pos
QTY_ORDER
        Database description : Original order quantity
        Original: remains unchanged
        AV remake: must go to the new item = order quantity (now it is only 1)
Quantity
        Database description: number of units. The reduced quantity only is given here if split in
        production item. Sum of field Quantity of all production items yields MENGE_AUFTRAG.
        See also ART_NR_PRODUKT. In case of surplus, this is the max. quantity to be supplied.
        Original: reducing by 1 makes no sense. What should be in there if the item consists of
        just one piece and 2 pieces are broken. Then remake items are generated, with which
        quantity? The quantities could even be negative.
        Application of STM: only if the header part should be produced in the remake, then it re-
        ceives the quantity 1 and the quantity of the original item is reduced. However, this could
        create confusion and make the contents of the database harder to understand.
        Better: the remake item is always filled with 0; the original item contains the original
        quantity. That is, in the pool_pos, the commercial quantity is always represented. It does
        not change; it remains unchanged regardless of how many remakes should be produced
        (handled with #321974)
        AV remake: is always initialized with 0
Remake
        Database description:
        Original: = 0
        AV remake: =1; identifies the AV remake

A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                  104
           Pool_teile
Quantity
        Database description: maximum quantity to be produced before all processings. Can devi-
        ate with production-technical surplus from POOL_POS.MENGE. For cut parts, always cor-
        responds to the cut quantity.
        Original:
        07/21/2014, see #324738: the quantity in Tabelle Pool_teile must be reduced since other-
        wise the detailed scheduling produces too many parts.
        07/22/2014, the quantity may only be reduced if the status of the parts <= roughly plan-
        ned and labels were assigned! Otherwise, the quantity remains unchanged.
         08/04/2014 STM: must be handled with #324738. Here, the fields created in pool_teile
        must also be filled (reference to the original item)
         08/20/2014 PK: CAUTION: If you book an IG as AV remake even though it is still in the
        pool, it will not work! An IG can only be reported broken if it was produced and thus has
        at least a status > "released". Such a test is thus irrelevant!
         08/15/014 STM (#321974):In the original item, the value is only reduced by 1 if the
        remake item has been completed through assignment of labels and the batch status is less
        than fine-planned. In each case, the field has the same value for all parts of an item.
        AV remake: is always initialized with the quantity 1.
 Original item quantity=5   Status <= roughly scheduled         >= scheduled in detail




 Labels were assigned
 (mode: Interpane)




 Labels were not assigned
 (mode: Normal)




Order quantity


A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                 105
       Database description: original order quantity
       Original: remains unchanged
       AV remake: must go to the new item = be order quantity (now is only 1)
Bdestückoffen_Anz
       Database description: number of not yet produced pieces of this part, is filled by PDC.
       Original: unclear for non-booked parts (spacers), false for parts that can be reused
       AV remake: unclear for non-booked parts (spacers), false for parts that can be reused
Menge_Nach
       Database description: maximum quantity after all processings, corresponds for header
       parts to the max. delivery quantity (that is, this is the quantity ordered less the surplus)
       Original: will be reduced by 1 (11/18/2012 STM # 333374): "When generating a remake
       item, the field POOL_TEILE.MENGE_NACH in the original item is used for the broken lite
       and all parts below it are reduced by the quantity 1, since these parts will be produced in
       the remake item. If the remake position on the remake management dialog is assigned
       sheets from the original item, then the MENGE_NACH field in the original item for these
       parts is also reduced by 1."
       AV remake: must be on the new item = 1
Prodmenge
       Database description: quantity already produced
       Original: will not be filled (not ever)
       AV remake: will not be filled (not ever)
Breakvorgaengerpos
       Database description:
       Original: = 0
       AV remake: includes the item number from which this item arose
Breakorigpos
       Database description:
       Original: = 0
       AV remake: includes the item number from the original item. If an AV remake is genera-
       ted several times from a lite, the very first item number is listed here.


        Pool_bearbeit
Menge_prod
       Database description: the quantity that should be produced in this production step (custo-
       mer quantity plus processing-dependent surplus)
       Original: must be reduced by 1
        07/22/2014 PK: must be reduced by 1 if the part is initialized in the remake with 1



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 106
         08/15/2014 STM (#321974): if the field is initialized in the remake item with 1, then the
        field for the part in the original item is reduced by 1.
        AV remake: will be initialized with 1
        07/22/2014 will be initialized with 0 for the procurement types 10 (reuse from break) and
        11 (production in the original); otherwise always with 1
        08/15/2014 STM (#321974): In the remake item, the field is initialized with 1 if the procu-
        rement type of the part matches the procurement type in the original item; otherwise
        with 0.
        11/11/2014 STM (#332816): If a remake item is assigned labels from the original item,
        then the POOL_BEARBEIT.MENGE_PROD field in the original item for these parts is re-
        duced by 1 and that of the remake item is initialized with 1. Previously, the run status of
        the original item was considered during the initialization.
 Original item quantity=5      Status <= roughly scheduled        >= scheduled in detail




 Labels were assigned
 (Mode: Interpane)




 Labels were not assigned
 (Mode: Normal)




Quantity
        Database description: processing quantity per part. Determine quantity from KANTEN-
        MATRIX during filling from item set. (PK: since 5.3, has always been initialized with 1)
        Original: remains unchanged
        AV remake: will be initialized with 1
Menge_gut
        Database description: the number of the total intact lites after this processing
        Original: will be reduced by one if the part was previously reported good



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                  107
      AV renmake: if the lite was previously reported good and can be reused, then menge_gut
      will be initialized with 1; otherwise with 0
Menge_bruch
      Database description: the number of broken lites in this step
      Original: counts the number of broken lites
      AV remake: will be initialized with 0
Menge_gefertigt
      Database description: the actual edited quantity of lites (PK: =menge_bruch+menge_gut)
      Original: remains unchanged
      AV remake: will be initialized with 1 if the procurement type 10-reuse is from break and
      the lite was previously finished. Otherwise menge_fertig will be initialized with 0
Menge_verfuegbar
      Database description: PK: zdisplays the number of parts that can be produced in this work
      process because the previous processes and products are finished.
      Original: is reduced for the part reported broken
      AV remake: is only initialized with 1 for cutting, frame (that is, the lowest parts in the
      BOM); otherwise with 0


        Awbar_Bearbeit
Menge_Soll
      Database description: processing target quantity (PK: always in pieces lites)
      Original: label number will be renamed (-001)
      AV remake: will be initialized with 1
Menge_Ist
      Database description: processing actual quantity (PK: always in units lites)
      Original: label number will be renamed (-001)
      AV remake: will be initialized with 0


        Awbar_booking
Defect mode
      0: Does as specified in the master data for the defect status.
      1: Make no remakes.
      2: Make a remake without defect pool.
      3: Make a remake with defect pool.
      4: Make an AV remake. This booking record then generates the complete remake item for
      all parts.



A+W Software GmbH                 EN-CONFIG-A+W Production.docx                                    108
In addition, individual bits can be set:
        16: Installed subparts are not automatically reported broken. This is required if individual
        booking records are written for the subparts.
        32/36: Make no PDC initialization when generating a remake item. This is required if the
        first booking record generates the remake item (with BREAKAGE MODE = 36) and before
        PDC initialization the start labels are set in POOL_TEILE for the remake item with the follo-
        wing booking records. The record in AWBAR_INITDATA is written by the remake dialog
        after making all bookings for the remake item.
        52: = 4 + 16 + 32 there are also such combined values
        256: Installed lites may be booked regardless of whether or not this is allowed. Thus boo-
        king records are processed in any case for installed lites.
        257:     ??
Errorregpt
       Includes the registration point that was specified as defect location in the remake hand-
       ling
Bruch_text
        Includes the text that you entered in the remake handling for a broken lite. Later, this text
        lands in awbar_teile.infotext.


          Awbar_teile
Status and status name
    After a break of a subpart, in the remake handling all components are assigned a label num-
    ber and an AV remake is generated. Confusingly, the IG then gets the status "60-Reuse" in
    awbar_teile. However, the procurement type in the pool_teile is correctly "0-Production".




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                               109
10. A+W Production Terminal
If settings are changed in the master data, a subsequent restart of the A+W ALCIM Booking Engine
booking service and the corresponding A+W Production Terminal is required.


10.1.           Functions in all A+W Production Terminals
                Opening the A+W Production Terminal QA with <F1>
It is possible to open the A+W Production Terminal QA module from the A+W Production Terminal.
Instead of opening the batch window with <F1>, A+W Production Terminal QA is then started by
pressing <F1>.
For the activation, the following steps are required:
    •   Open the Parameter Administrator with <Ctrl>+<F9> from the appropriate A+W Production
        Terminal
    •   If necessary, copy the station and the AUW default screen




Figure 10-1 Parameter Administrator with parameter "Use dialog QA"


A+W Software GmbH                    EN-CONFIG-A+W Production.docx                          110
    •   Set the parameter Use QA Dialog to True with the drop-down list entry under the Dialogs
        sections
    •   Confirm with a click on [Apply]


                 Formatting of all areas, lengths, and thicknesses
For the values length, area, and depth, which are used in the A+W Production Terminals, a global
formatting can be stored for each. For this, for all columns that are configured using the same
setting, the appropriate variable must be stored:
    •   For all areas: ALXF_ToolTV_AREA
    •   For all lengths: ALXF_ToolTV_DIMENSION
    •   For all thicknesses: ALXF_ToolTV_THICKNESS
If now for such columns, analogous to the specific formatting described under 8.1.3, you now enter
the variables listed above, these columns can be configured as follows with the help of global
parameters:
    •   Open the Parameter Administrator with <Ctrl>+<F9> from the appropriate A+W Production
        Terminal
    •   Select the header part A+W Production Terminal
    •   Configuration of the 3 parameters Indirect Area, Indirect Length and Indirect Thickness in
        order to format all appropriate values




Figure 10-2 Global formatting

    •   Confirm with a click on [Apply]


                 Formatting of individual table columns
If data is displayed in a table in an A+W Production Terminal, the columns can be configured
individually. The formatting of the values displayed can also be configured. The following steps are
required for the change:
    •   Open the Designer with <Ctrl>+<F12> from the appropriate A+W Production Terminal
    •   Select the data table

A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                111
    •    In the right table under Draft > Columns next to (Collection), click on the three dots




    •    On the new Selected Columns window, select the appropriate column




Figure 10-3 Formatting of data columns

    •    Under Format, click again on the three dots
    •    Select the desired format on the Format of the column values window
    •    Click [OK] twice to confirm, save the dialog in the database, and then close the Designer


             Checking of the rack for existence in the A+W Rack
        Manager
If the A+W Rack Manager is used, it is possible to activate that all rack numbers entered into the
A+W Production Terminal are checked to see whether these have already been created in the A+W
Rack Manager. If a rack entered is not in the A+W Rack Manager, a warning is displayed and the
user is asked to use a different rack. If a rack is created in the A+W Rack Manager but not in A+W
Production, this rack is created automatically in A+W Production.
The prerequisite is that all bookings are made at the same time. How this is activated is also
described in this subchapter.
For the activation, the following steps are required:
    •    Open the Parameter Administrator via A+W Production. To do this, select the Master Data
         > Configuration menu.
    •    Navigate to Parameter > A+W Production > General > ALCIM BOOK and set the
         synchronous/asynchronous booking parameter to the value 1 (see Abbildung 8-4)




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                              112
Figure 10-4 Configuration of synchronous booking

    •   Navigate to Parameter > A+W Production > Barcoding Booking Services > General and set
        the Temporary rack parameter to the value 1 (see Abbildung 8-5)
    •   Restart the A+W ALCIM Booking Engine booking service and the corresponding A+W
        Production Terminal




Figure 10-5 Configuration of the rack comparison with the A+W Rack Manager




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                        113
           Configuration scanner connection to A+W Production
     Terminal
The configuration of a scanner depends on the type of installation of the A+W Production
Terminal. If the A+W Production Terminal should be operated on a terminal server (recom-
mended), it is necessary that a "header character" be sent before the actual barcode. This is then
entered as "start bit" in the parameter configuration.
Log into A+W Production Terminal and open the Paramater Administrator (CTRL+F9). Under sta-
tions, select the affected station and make the following settings under keyboard scanner on the
right side:
 Enabled                                          Please set to "True"
 Start Bits                                       Please enter "S"
 Stop Bits                                        \r (already present)
 Scanner recognition                              Remains empty
 Language for the keyboard                        Standard




Figure 10-6 - Keyboard scanner parameters


In case of a local installation, the scanner can be connected directly to the A+W Production
Terminal via "VID/PID". Please make the following settings:
 Enabled                                          Please set to "True"
 Start Bits                                       Delete start bit (if present)
 Stop Bits                                        \r (already present)
 Scanner recognition                              Select icon with the 3 dots and scan a barcode
 Language for the keyboard                        Standard




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                              114
Figure 10-7 - Scanner ID



The detailed configuration of the various scanners used by A+W is described in separate
documents.
These are found in: \\jupiter\TECHSOFT_BDE\Scanner-Tools\SCANNER



                 Performance Counter configuration
With the Performance Counter (lite counter), you can display on the Production Terminals how
many lites, how much area, and how many linear meters were produced at a registration point in
a particular time. This way, you can see what was produced in a "real" shift.
All 3 values are added up until the status at the registration point changes or a separate "Delete"
button is pressed. The data is always updated when you press the "Produce" button or after an
adjustable time (so that data is also counted that is recorded with a scanner.) The display remains
empty as long as no "ON" status on the registration point is selected.
The values displayed are calculated from the following fields:




A+W Software GmbH                  EN-CONFIG-A+W Production.docx                               115
Linear meters = 2 x height + 2 x width; that is, the edge matrix is not taken into account since you
cannot know from the registration point which edges are relevant for this.
Area= value from pool_teile.flaeche_modell




Since this functionality is not integrated in the standard, it has to be configured separately:
Timer for refreshing after a specified time:
        Parameter: area = @PROPERTY_SYSTEM; Eintrag = RefreshTimeAmountControls
        The time is specified in minutes and should not be selected too small in order to prevent
        an unnecessary load on the database
Button for resetting the values:
        Button, action: ResetUnitCounter
Field for the number of lites:
        Output field; action = SUM_PIECES
Field for the total of linear meters:
        Output field; action = SUM_LINEARMETERS
Field for the total of the area:
        Output field; action = SUM_AREA


This function is available in all Production Terminals except the Production Terminal "Edit" and
the "Supply" terminals.
Restriction: the data is only displayed in the Metric system. That is, the imperial measurement
system is not supported!
Attention: since the period for the cumulation of the values from the status booking on the ma-
chine is defined (that is, last status booking "machine on" to now), the values can also be dis-
played correctly after a terminal restart. Here, however, the production terminal has to be set so
that an ending or restarting of the program does not reset this machine status. For this, you deac-
tivate the automatic booking of the status when starting and ending the Production Terminal by
selecting the status '-1' in the parameters 'ToolTVOrderStateBegin' and 'ToolTVOrderStateEnd'.
Expansion as of Production Terminal 13.04.8314: In the parameters, a list of statuses can be spe-
cified optionally; these reset the lite counter. These statuses apply globally for all Production Ter-
minals. Only if one of these statuses is booked is the counter reset. Thus it is possible to book a
break or maintenance during a shift without resetting the counter.




A+W Software GmbH                       EN-CONFIG-A+W Production.docx                              116
A+W Software GmbH   EN-CONFIG-A+W Production.docx   117
                Tracing
The Production Terminal can save its trace data in two different ways. The behavior is specified
via a switch that you find in the ParameterAdministrator. Stationen => Trace Ziel. The following
settings can be applied:
PPSWebService:
Previously, all data was transmitted to the PPSWebservice. The PPSWebservice writes all data to
the associated trace file. The consequence is that the trace data from different Production Termi-
nals is in one file.
LocalDisc:
The new settings saves the data, just as you are used to doing from the other products. Each Pro-
duction Terminal writes the data to an individual file that is on the local hard disk. The trace level
and time period for which the data is kept is still set in the Konig tool of the PPSWebservice.
Both:
Trace data is sent both to the PPSWebservice and saved locally.




10.2.           A+W Production Terminal TG-In
                Furnace bed optimization
In A+W Production Terminal TG-In, racks located at a registration point in front of the furnace can
be selected for optimization. For this purpose, a dialog opens showing all available racks. The dialog
contains two lists. A list shows all groups of lites that can be optimized together. A criterion for this
can be the type of glass or the thickness. This list only allows simple selection. A second list shows
all the racks containing lites from the selected group. The list of racks allows multiple selection.
Here, the racks whose lites are to be optimized are selected. Optimization takes place when the
dialog is closed. The optimization takes into account the stacking sequence on the racks. The lites
that were last booked on the rack are first placed on the furnace bed.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                  118
Figure 10-8 Furnace bed

In the list of the TG-In all lites of the optimization are displayed, usually several furnace beds. For
the lites belonging to the next furnace bed, a column in the list is filled with the name of the furnace
bed. All lites of the next furnace bed are displayed in the furnace bed display. Lites that are missing
or broken can be entered with the Cancel button and marked in color on the display. The furnace
bed then has a gap at the corresponding point. There are two ways of producing the furnace bed.
Either the entire furnace bed is produced with Produce or each individual selected lite of the
furnace bed must be confirmed beforehand with a button. Only the confirmed lites are then booked
during production.
If an optimized furnace bed is displayed, it is not possible to add further lites to the furnace bed by
scanning.
Optimization is only possible if a "XOPT furnace" license for furnace bed optimization is available. If
the Production Terminal TG-In has the button for optimization, a license check is performed. If no
license is available, a corresponding message appears.
There is a new button in the Designer with the action OPTIMIZE. By default, this can be done under
"File/Optimization" or with the hotkey <Ctrl>+<O>. This button opens the dialog for selecting the
racks. The DesignerForm for this dialog is stored in the parameters of the TG-In
(AUW_Racks_For_Optimization). The registration point on which the available racks are located is
configured in the parameters in the TOOLTVTGINREGPOINTOPTIMIZATIONIN switch (default: 1313,
1323, etc.). The dialog contains two lists with the actions GROUPLIST and RACKLIST. The GROUPLIST
contains an action column with the action Group, after which the group is grouped.
The optimization is performed on the server on which the PPS web service is running. The setup for
furnace optimization must have been carried out there. The optimization takes place in a
temporarily created subdirectory of %appdata%\A+W\Techsoft\XOPT\OfenOpti for the user of the
PPS web service. The result of the optimization is saved as a save file in the directory
C:\inetpub\wwwroot\Albwir.Alcim.DataService\Reports and transferred to the Production
Terminal.
If the button with the action PRODUCEUNIT is available, the lites on the furnace bed must be
confirmed individually.

Further switches for the optimization must currently still be inserted by hand into the database:

    a) Orientation of the lites on the furnace bed

        insert into parameter (bereich, eintrag, nummer, typ, text) values ('FEIN_ZUSATZOPTI’,
        'SHEETORIENTATION', 0, 0, 1);

        Where: text=


A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                  119
                0: no specification
                1: longEdgeItemParallelToLongEdgeOven
                2: longEdgeItemParallelToShortEdgeOven

    b)    Distance of lites to edge

         insert into parameter (area,entry,number,type,text) values(‚FEIN_ZUSATZOPTI‘                 ,
         ‚EDGETOP‘, 0, 0, 100);
         insert into parameter (area,entry,number,type,text) values(‚FEIN_ZUSATZOPTI‘                 ,
         ‚EDGEBOTTOM‘, 0, 0, 100);
         insert into parameter (are,entry,number,type,text) values(‚FEIN_ZUSATZOPTI‘                  ,
         ‚EDGELEFT‘, 0, 0, 100);
         insert into parameter (area,entry,number,type,text) values(‚FEIN_ZUSATZOPTI‘                 ,
         ‚EDGERIGHT‘, 0, 0, 100);
         Where "text" defines the distance in mm to the border

Additional settings are planned in case 441310.

Note: Both on the data grid of the furnace entrance as well as on the furnace bed display, it is
recommended that you display the name of the source rack. Only then does the user know from
which rack he must take the lites.


                Part type filter
Programming case #454705
The A+W Production Terminal TG-In parameters now provide a switch for a list of part types:




If no part types are specified here or -1 (not defined) is selected here, the link between
AWBAR_TEILE and POOL_TEILE via AWBAR_TEILE.TEILENR_MIN = POOL_TEILE.TEILE_NR is made to
fill the data grid.
If part types are configured, now there is filtering according to the part types. The link for the data
grid      is   made     via    AWBAR_TEILE.TEILENR_MIN           <=    POOL_TEILE.TEILE_NR          and
AWBAR_TEILE.TEILENR_MAX >= POOL_TEILE.TEILE_NR. If several records are found, then the
record with the largest part number is used for the display.

Example:
 Label                     Part number              Part Type                 Name
 000004711                 1000000                  6                         TGH - Processed
 000004711                 1000001                  6                         Tempered glass
 000004711                 1000002                  1                         Float



A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                120
If no part types are configured, then in the data grid, "TG processed" is displayed in the data grid as
name from POOL_TEILE.
If the part type 6 is configured, "TGH" is displayed.
If the part types 1 and 6 are configured, "Float" is displayed.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                  121
10.3.            A+W Production Terminal TG-Out
                 Several scanners
In Production Terminal TG-Out, several users can simultaneously book the lites of an oven bed
onto different racks. Each user books with a scanner on the previously scanned rack.
Up to five different scanners can be configured in the parameters of the TG-Out. An ID must be
specified for each scanner. The scanner is to be configured in such a way that the scanned bar-
code gets this ID as prefix. All IDs used must have the same length, the length must also be confi-
gured.




Before a booking, the person and rack have to be scanned for the scanner. On the main screen
and in the external furnace bed, there are output fields for the person (action Person1, Person2,
etc.) and for the rack name (action Rack1, Rack2, etc.). The scanned person and rack will be dis-
played for every scanner.




On the main screen and in the external furnace bed, for each scanner, the last scanned barcode of
a lite or of status can be displayed in an output field with the action LastBarcode1, LastBarcode2,
etc.


If the barcode of a lite is scanned, it is booked to the frame. The output fields are stored with the
appropriate color for the packing group.




In the list, the rack is displayed for all lites in this packing group.




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                              122
By scanning an allowed break reason and a lite, a break is booked.




10.4.           A+W Production Terminal LG-IN
                Installation after ERP item
Programming case #458450
Previously, a LAMI could only be assembled from components of the same production item. If,
however, a commercial item is split into several production items, e.g. due to the capacity plan-
ning, the working method at LAMI intake is a bit complicated.
On the Production Terminals LG-In and LG-Assembly, it is therefore now optionally possible to as-
semble parts from different production items. Here, it is only checked whether the item numbers
from the ERP system match. On the Production Terminal LG-In, it is possible to scan lites from dif-
ferent production items until a LAMI is complete. When filling the display via the dialogs for loa-
ding a lot or an order, parts with the same production items are still displayed and produced. On
the Production Terminal LG-Assembly, the plausibility check for the lites at the intake can be rest-
ricted so that lites from different production items are accepted and can be assembled.
The behavior on both Production Terminals LG has to be activated with the USEERPITEM switch.


10.5.           A+W Production Terminal LG-Assembly
                Foil preview
Programming case #399150
It is now possible to configure the Foil preview in the Designer of the A+W Production Terminal LG-
Assembly. This offers less detail than the original view, but a better overview of the foils that will
be needed in the future.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 123
For the configuration, the following steps are required:
You can reach the foil preview most quickly with the following steps:
    •   You replace the "PREVIEWLIST" action of the lower data grid with "FOILPREVIEWLIST"




        Figure 10-9 Action for the foil preview

    •   Delete the following columns from the data grid:
        ProdNr, Los, Etikett, Alarm(Storno)
    •   Change the sources for the following columns:
        Width from pool_teile.breite,
        Height from pool_teile.hoehe,
        Job from pool_teile.lauf
    •   Insert a total column for the number of foils:
        Anzahl = count(pool_teile.artbez1)
CAUTION: no fields from awbar_teile can be used in this data grid!
To display the number of foils, there must also be a column containing the SQL command "COUNT",
as it is grouped by label number and foil:
e.g. Anzahl = COUNT(POOL_TEILE.ARTBEZ1)
CAUTION: if you want to display data for the LSG from Pool_teile (e.g. the item designation), then
you must first select the field from pool_teile and then rename the SQL output "ppol_teile2.xxxx":




Figure 10-10 SQL expression for the foil preview




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                          124
10.6.            A+W Production Terminal Order
                 Automatic generation of a batch number
In A+W Production Terminal Order, a batch number can be generated automatically. If the last
booking at the respective registration point is longer ago than the configured duration in minutes,
a new batch number is generated.
For the activation, the following steps are required:
    •   Open the Parameter Administrator with <Ctrl>+<F9>
    •   If necessary, copying of an AUW default screen
    •   Setting of the switch "Automatic batch generation" to the desired time interval in minutes
        under the "Bookings" section
    •   Confirm with a click on [Apply]




Figure 10-11 Parameter Administrator with parameter "Automatic Batch Creation"

The default value of this switch is 0, then no automatic batch number is generated.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                             125
10.7.            A+W Production Terminal IG-In
                 Transfer of PMO data to the Panorama
When loading an IG lot from a packaging optimization run, A+W Production Terminal IG-In can read
the PMO data from the database and transfer it to the Panorama. The data is only transmitted if a
complete lot is loaded. If only some of the racks are selected that are in a lot, no PMO data is
transmitted to the panorama.
For the activation, the following steps are required:
    •   Open the Parameter Administrator with <Ctrl>+<F9>
    •   If necessary, copying of an AUW default screen
    •   Setting of the switch "Results of the PMO" to true under the section 'Machine allocation'
    •   Confirm with a click on [Apply]




Figure 10-12 Configuration for provision of PMO data


                 Transfer of PMO data via XML file
A+W Production Terminal IG-In can make data from the packaging optimization available to other
machines via XML file. Here, an XML file is generated for each rack. The XML files are copied to a
configured directory and are available there for possible machine activation.
The prerequisite for this is the activation of the switch "Results of the PMO" from section 8.5.1.
Furthermore,        the     program       Alcim2XML.exe     must      be    in    the    directory
ProgramFiles(x86)\A+W\Techsoft\PackOpt. This program must be copied manually into the
directory since it is not part of the setup.
For the activation, the following steps are required:
    •   Open the Parameter Administrator with <Ctrl>+<F9>
    •   If necessary, copying of an AUW default screen
    •   Setting of the parameter "Directory for PMO data" to the desired target directory under
        the section 'Machine Assignment'
    •   Confirm with a click on [Apply]



A+W Software GmbH                     EN-CONFIG-A+W Production.docx                           126
Figure 10-13 Configuration for transfer of PMO data via XML file


                 Sending of information to quality scanner
A+W Production Terminal IG-In can make available information about the lite to be scanned to a
quality scanner on the IG line.
For the configuration, the following steps are required:
    •   Open the Parameter Administrator with <Ctrl>+<F9>
    •   If necessary, copying of an AUW default screen
    •   Selection of the quality scanner type to be activated with the parameter "Quality Scanner
        type" under the section 'Machine Assignment'




Figure 10-14 Parameters for quality scanner



A+W Software GmbH                     EN-CONFIG-A+W Production.docx                          127
    •   For the parameter "Quality scanner directory"enter the path to the directory here in which
        the feedback from the quality scanner is entered.
        The feedback is only written if the affected lite is produced (trigger). After production, the
        entry is deleted.
    •   For the parameter "Quality scanner recipe" you can set how precisely the quality scanner
        should work. Depending on the manufacturer, there are different options:
            o   Viprotron offers the quality levels A, B, C, D, E, F. In the configuration, the
                respective quality level must be entered with apostrophes.
            o   SoftSolution can be configured at will: here you can link any database fields of a
                lite to one another. The results from this link have to be configured in the
                Softsolution database.
    •   Confirm with a click on [Apply]
Optionally, it can be configured in A+W Production Terminal IG-Assembly that the result of the
quality scanner is displayed. (see section 8.6.1)


                Call of an SP for turning on a turning station
In the parameters, the name of an SP can be specified, which is called for each IG subpart (not for
frames) before the lite is transferred to the panorama.




The SP expects as parameters: AUFTNR, POS, U_POS, TEILE_NR, ETIKETTNR. If this SP is present, it
is called. With a return value of 1, the lite is turned. For each lite, in the panorama the property
"ToolTV.SpecialAction" is set to 1 if the lite should be turned. The prerequisite is the use of a spe-
cial panorama that can evaluate this property.


                Display of additional parts in the detail list
In the detail list of the Production Terminal IG-In and IG-Assembly, you can now also optionally
display the parts from which an IG subpart is constructed. If, for example, a produced LAMI is in-
stalled in an IG, its subparts are displayed in the list below the LAMI. For the additional tiles, the
information configured in the designer from the database is displayed. Fields from the AWBAR or
FEIN tables (for example, label or rack number) remain empty for these parts.



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                  128
A+W Software GmbH   EN-CONFIG-A+W Production.docx   129
10.8.           A+W Production Terminal IG-Assembly
                Quality scanner configuration
Optionally, it can be set in A+W Production Terminal IG-Assembly that the result of the quality scan
is displayed. The prerequisite is that 8.5.3 must be configured.
For the configuration, the following steps are required:
    •   Open the Parameter Administrator with <Ctrl>+<F9>
    •   If necessary, copying of an AUW default screen
    •   Selection of the quality scanner type to be activated with the parameter Quality Scanner
        type under the section Machine Assignment
    •   The parameters to be configured are in the machine assignment section




Figure 10-15 Parameters for quality scanner

    •   Quality scanner directory: please enter the directory path here. The files for the scanner
        communication will be written to this directory. This directory will be analyzed by the
        quality scanner.
    •   Quality scanner breakage reason: please enter the breakage reason here that should be
        used when reporting a defective lite from the scanner to the booking.
    •   Quality scanner type: Select the quality scanner type to be activated from the selection
        menu here.
    •   Quality scanner lite switching: switching with the result of the quality scan.
        o   TRUE: The result of the quality scan will be considered. If then a lite is found to be good
            by the quality scanner, it is produced automatically in the IG-Assembly. The operator
            only      has       to     intervene      in     case     of     a        defective     lite.
            If the result of the quality scan should be considered, the parameter Confirm individual
            subparts when producing in the Bookings section must also be set to true.




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                  130
Figure 10-16 Parameters for individual lite booking

         o   FALSE: The result of the quality scan will be ignored. Switching of lites is treated
             normally, the operator must press [Produce] so that - depending on the configuration
             - the lite or unit is switched.
    •    Confirm with a click on [Apply]


                 Display of additional parts in the detail list
See 8.6.5.




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                         131
10.9.            A+W Production Terminal IG-Out
             Dialog for calling up racks from a sorting system
          (AUW_UnloadRacks)
In A+W Production Terminal IG-Out, a second screen can be incorporated, one that displays from
which logical A-racks lites are already present in the sorting system and what the respective target
and actual quantity is. The user can use this screen to select a rack and request the transport out
of the sorting system.
For the configuration, the following steps are required:
    •    Open the Parameter Administrator with <Ctrl>+<F9>
    •    If necessary, copying of the station and the AUW default screen
    •    Set the parameter Dialog for Retrievable Racks to "AUW_UnloadRacks"




Figure 10-17 Parameter Administrator with dialog selection for racks that can be called up

    •    Check and adjust the lot types for this station in the Bookings section. If, for example,
         individual lites should be displayed on this dialog, the parameter Lot types for this station
         must be set to 100; for IG units to 700.




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                              132
Figure 10-18 Select lot types

    •    The racks displayed can be filtered by cutting tables. For this, the tables must be created in
         the Registration Points area under the parameter List to Filter Cutting Tables. For this, click
         [...] and create a new entry per table that can be filtered, whereby the filter is the
         registration point number. For the entry All tables, leave the filter empty.




Figure 10-19 Parameter Administrator for the filter possibility by cutting tables




A+W Software GmbH                        EN-CONFIG-A+W Production.docx                              133
Figure 10-20 Configuration of tables for filter selection

    •    For the parameter Selected filter for cutting tables, enter the list item to which the combo
         box should be set at the start of the dialog. Here, 0 = first list entry, 1 = second list entry,
         etc.
    •    Confirm with a click on [Apply]
    •    Change to the Designer with <Ctrl>+<F12>
    •    Adding a button with the action "LOADRACKS." The labeling of the button is then set
         automatically. A shortcut button can be added to the button, for example, <F2>. For this,
         select the appropriate button in the Behavior section. It makes sense to add this shortcut
         button to the button labeling. Under Layout set the anchor according to the other buttons.




A+W Software GmbH                        EN-CONFIG-A+W Production.docx                               134
Figure 10-21 Designer with new action button [Racks that can be called up]

    •   Save change in the database with [File] > Save (Database) and exit the Designer
If the new button is not visible in full-screen mode, the anchors are probably not set correctly. To
do this, go into the Designer again and adjust the anchor. It can be helpful to take a look at the
anchors of already-existing buttons.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                             135
10.10.            A+W Production Terminal Processing
                  Selection of a fine planning rack
In A+W Production Terminal Processing it is possible to use the dialog for loading a lot to select a
fine planning rack and place it on the display. Now it is also possible with an open dialog to select
the rack by scanning any lite on the rack.




Figure 10-22 selection of a fine planning rack

The dialog for loading a lot now also contains an input field with the action BARCODE. As an
alternative to scanning, you can enter the barcode of the lite here and confirm it with ENTER. The
dialog must include the input fields with the actions JOBINPUT and FEINBOCKINPUT. These fields
will be filled when scanning a lite.




Figure 10-23 Dialog for loading a lot



A+W Software GmbH                       EN-CONFIG-A+W Production.docx                            136
                 SN driver call for all lites
On the Production Terminal Processing, it is possible to call up the drivers for all lites in the list
with a button. Here, the call is made just once for all lites in the list that belong to one part. Only if
there is a part change is there a new call. Now the driver for each lite in the list can be called opti-
onally.
This can be done in the A+W Parameter Administrator under Parameter – A+W Production Termi-
nal Processing – “Assigned Station” – SN – driver call for each lite.




Figure 10-24 SN driver call




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                    137
11. A+W Production Terminal QA
Several screens can be configured in A+W Production Terminal QA. The content of each screen is
configured in an XML file. The XML files must be in the installation directory C:\Program Files
(x86)\A+W\Production\A+W ProductionTerminal QA in addition to the application (exe file).
The visual arrangement of the window and notice texts are configured in the XML file. Only the
following data are saved in AWSOA database Quality_TrackingData:
   •   InputCategory
       <local:QATerminalData x:Key="BaseData" DataType="DataIsoOut"/>
   •   InputData
       <TextBox x:Name="textBox" Grid.Column="1" Grid.Row="4"          Text="{local:ModelString
       Id=Charge No}"/>
The setup already contains two XML files, which can be used as an example.




A+W Software GmbH                 EN-CONFIG-A+W Production.docx                            138
12. AUW functions
AUW functions are SPs, VIEWs, tables, reports, screens that standardize customizing. They
distinguish themselves in that these functions begin with the abbreviation AUW_. A change of these
functions is not permissible since they are overwritten with an update.


12.1.             Database VIEWs
In the A+W Production database, there are standard VIEWs that can be used on the CrystalReports
papers in order to determine data more easily.


                  AUW_POOL_TEILE
The VIEW AUW_POOL_TEILE displays the BOM of an item vertically and horizontally.
This VIEW can be incorporated into the rough scheduling displays and into the leading screens.
auftnr            pos                teile_nr           teile_nr1 teile_nr2 teile_nr3
700052            1                  0                  1000000             2000000              3000000
700052            1                  1000000            1010000
700052            1                  1010000
700052            1                  2000000
700052            1                  3000000

Currently, this VIEW supports a maximum of 8 horizontal parts for the following fields from table
POOL_TEILE: ARTNR, ARTBEZ1, DICKE, TTYP, BESCHAFFUNGSART
Before this VIEW was created, the VIEW AUW_BOM already existed. However, this could not be
integrated into the POOL views. For reasons of backward compatibility, the VIEW AUW_BOM still
exists; it refers internally to the VIEW AUW_POOL_TEILE.


                  AUW_POOL_SZR
The VIEW AUW_POOL_SZR is an expansion for the table POOL_SZR. It determines whether an edge
of a lite has an individual sealing depth or cutback. For each edge, the values for sealing depth and
cutback are displayed. This VIEW works with the shape data record 1000
(POOL_MODELL.BEARB_NR = 1000) of a frame part and with the thickness of the frame
(POOL_SZR.RAHMENSTAERKE).
This VIEW can be incorporated into the rough scheduling displays and into the leading screens.
auftnr   pos       teile_nr kantenindividuell versiegeltiefe1    versiegeltiefe2        versiegeltiefe3
         versiegeltiefe4    rueckschnitt1     rueckschnitt2      rueckschnitt3          rueckschnitt4
700113 1          2000000 1          3000       13000   23000    33000     10000        20000    30000     40000
700113 2          2000000 0          4000       4000    4000     4000      11000        11000    11000     11000


                  AUW_AE_INTPOS
This VIEW AUW_AE_INTPOS displays information of a production item (table POOL_POS) adds up
for the item of the order entry (POOL_POS.AE_INTPOS).



A+W Software GmbH                        EN-CONFIG-A+W Production.docx                                             139
auftnr   ae_intpos          kommission1                  tour    mindermenge       menge   count_pos
700055   1        Triple IG with muntins                         2      0                  1       1
700055   2        Triple IG with muntins                         2      0                  150     3
700055   3        IG with different sealing types        2       0                 10      1
700055   4        IG with different gases                        2      0                  20      1
700055   5        IG with different gases                        2      0                  15      1
700055   6        IG with different gases                        2      0                  25      2
700055   7        IG with different gases                        2      0                  3       1

COUNT_POS          Number of production items in A+W Production
Current fields of POOL_POS:
kommission1, kommisson2, kd_pos, tour, SUM(mindermenge), SUM(menge)


                  AUW_AE_INTPOS_BOM
The VIEW AUW_AE_INTPOS_BOM works like the VIEW AUW_AE_INTPOS, but on the part level
(table POOL_TEILE).
auftnr   ae_intpos          teile_nr            ttyp     beschaffungsart   menge   count_pos
700055   1                  0                   7        0                 1       1
700055   1                  1000000             1        1                 1       1
700055   1                  2000000             12       9                 1       1
700055   1                  2010000             13       9                 1       1
700055   1                  3000000             1        1                 1       1
700055   1                  4000000             12       0                 1       1
700055   1                  5000000             1        1                 1       1

Current fields of POOL_TEILE:
teile_nr, oberteil_nr, ttyp, otyp, beschaffungsart, artnr, artbez1, artbez2, glasart, glasart_bez,
warengrp, breite, hoehe, dicke, modell_nr, bestell_flag, ausgangsnr, struktur_typ, struktur_pos,
beschicht_typ, beschicht_pos, stufen_flag, SUM(prodmenge), SUM(minermenge), SUM(menge)


                  AUW_AE_INTPOS_PROC
The VIEW AUW_AE_INTPOS_PROC works like the VIEW AUW_AE_INTPOS, but only the processing
level (table POOL_ BEARBEIT).
auftnr   ae_intpos        teile_nr     bearb_nr artnr    typ     menge_prod        menge_gut      count_pos
700055   2        0                    0        999970   1600    150               1              3
700055   2        0                    2        999996   1810    150               0              3
700055   2        0                    1        999995   1800    150               0              3
700055   2        1000000              0        999910   1700    150               0              3
700055   2        2000000              0        999975   1620    150               0              3
700055   2        2010000              0        999976   1640    150               0              3
700055   2        3000000              0        999910   1700    150               0              3
700055   2        4000000              0        999975   1620    150               0              3
700055   2        5000000              0        999910   1700    150               0              3

Current fields of POOL_BEARBEIT:
teile_nr, bearb_nr, sequenz, artnr, typ, text1, text2, bearbeit_name, kantenmatrix, mass_zuschlag,
final_kz, schicht, bestell_kz, mzo_id_phys, mzo_id_es, mzo_technologie1, mzo_maschin_txt,
dauer,       kosten,     SUM(menge_prod),            SUM(menge_gefertigt),      SUM(menge_gut),
SUM(menge_bruch), SUM(menge_prodnl), SUM(menge_verfuegbar)




A+W Software GmbH                         EN-CONFIG-A+W Production.docx                                  140
                 AUW_REGPT_NEXT
The VIEW AUW_REGPT_NEXT displays the current, the next, and registration point after that for a
processing (AWBAR_BEARBEIT).
auftnr   pos     teile_nr bearb_nr esnr    teile_nr2    bearb_nr2   esnr2    teile_nr3    bearb_nr3    esnr3
700052   2       0                0        1610      0       1       2910     0        2        11
700052   2       0                1        2910      0       2       11       -1       -1       -1
700052   2       0                2        11        -1      -1      -1       -1       -1       -1
700052   2       1000000          0        110       0       0       1610     0        1        2910
700052   2       2000000          0        1710      0       0       1610     0        1        2910
700052   2       3000000          0        210       0       0       1610     0        1        2910


                 AUW_CAPA_OVERVIEW
The VIEW AUW_CAPA_OVERVIEW displays all processings (table POOL_BEARBEIT). Here,
processings of a machine of the same AW type are grouped on one part (e.g. 3 processings, drillings
on a part for the same machine displays this VIEW in a data record).
The display of the VIEW can also be influenced by the AUW_SETTINGS switch:
         [CAPA_VIEW / SHOW_OFFERS] – for displaying offers
         [CAPA_VIEW / SHOW_RESOLVED_MACROS] – for displaying resolved macros
AUW_CAPA_TODO
The VIEW AUW_CAPA_TODO displays information similar to the VIEW AUW_CAPA_OVERVIEW.
Here, all completely produced processings are already filtered


                 AUW_WIP
This VIEW AUW_WIP is the basis of our WIP (Work in Process) list AUW_WIP.RPT. For all parts in production
(not installed, not broken, and is booked), the current costs up to and including the last booked processing
(processing before NEXTES, with a lower POOL_BEARBEIT.SEQUENZ) are added up.
         POOL_TEILE.MATERIALKOSTEN + POOL_BEARBEIT.MATERIALKOSTEN + POOL_BEARBEIT.KOSTEN +
         POOL_BEARBEIT.KOSTEN_PERSONAL + POOL_BEARBEIT.KOSTEN_SONSTIGE
AUW_WIP_AWB
The VIEW AUW_WIP_AWB is called by the VIEW AUW_WIP and makes data from table
AWBAR_BEARBEIT unambiguous for the list. Per part, there can be several data with the same
NEXTES. With the same NEXTES, the data record with the lowest BEARB_NR is determined.


12.2.            Functions and procedures
Functions and procedures can be used, e.g. for reports or in the planning displays.


                 AUW_GETTEXT
This function determines a particular text from the table POOL_TXT.TEXT. It is called with the
following parameters:
@spAuftNr                Order number


A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                    141
@spPos         Item number
@spUPos                Sub item
@spTeileNr             Part number
@spTextTyp             Text type (POOL_TXT.TEXT_TYP)
@spTextNr              Text number (POOL_TXT.TEXT_NR)
@spFROM                 Place from which the text should begin; 0 = from the first place
@spFOR         Length of the text, 0 = complete text


                AUW_POOL_NAME
This function determines the name of a transferred ID and is called with the following parameters:
@spCode                ID
@spControl             Control code, can have the following values:
        auwRegpoint = Name of the registration point
        auwLotType = Batch type of the detailed scheduling; batches used are marked with a *
        auwStaff = Name of the person from the PDC system
        auwProdTermFix = Text of the status from POOL_BEARBEIT.PROD_TERM_FIX
        auwMAReal = MZO_REALMASCHINE.TEXT of ID_REAL = @spCode
        auwMAPhys = MZO_PHYSMASCHINE.TEXT of ID_PHYS = @spCode


Example (for determination of the name of the next registration point):
      AUW_POOL_NAME (AWBAR_TEILE.NEXTES,'AUWREGPOINT')


                AUW_POOL_PAINT
This function is used in the rough scheduling displays in order to mark the fields with a color. The
return value is the color code plus a specific text.
@spNumber1             First number
@spNumber2             Second number, is not required for all functions
@spControl             Control code:
        auwBatchStatus = @spNumber1 = batch status (e.g. POOL_LAUF.STATUS)
        auwPMOStatus = @spNumber1 = PMO status
        auwLotType = @spNumber1 = Batch type (e.g. FEIN_TEILE.TYP), if @spNumber2 = 0 then only the
        color code is returned
        auwTargetActual = Target/actual (@spNumber1/@spNumber2) for barcoding display
        auwOrderMark = @spNumber1 = ID (e.g. POOL_AUFTRAG.AUFTKZ), @spNumber2 = return value,
        if 0 is the return value, a symbol
        auwElementNo = @spNumber1 = Part number (e.g. POOL_TEILE.TEILE_NR), different color for part
        0 and other part numbers




A+W Software GmbH                    EN-CONFIG-A+W Production.docx                              142
        auwComplaint = @spNumber1 =Original order number, @spNumber2 =current order number; if
        different, return value is a colored *
        auwBreakage = @spNumber1 = 1 (breakage), 2 (cancellation), 3 (quantities PDC breakage)
        auwNumber = @spNumber1 = 1 – x; each number returns a different color code (currently 1-7);
        @spNumber2 = 0 only color code
        auwRemakeOrder = @spNumber1 = POOL_BESTELLTEILE.NACHBESTOFFEN, @spNumber2 =
        POOL_BESTELLTEILE.NACHBESTTODO
        All other control codes = color; color code is returned if @spNumber1 <> 0; @spNumber2 = 0 only
        color code as text (can be combined with other fields in the display). Use the following control codes
        or a fixed RGB value (e.g. '38,8,92'):
                auwRed = 255,0,0^
                auwLime = 0,255,0^
                auwDarkcyan = 0,176,199^
                auwGold = 200,190,40^
                auwGray = 200,200,200^
                auwLightGray = 230,230,230^
                auwDarkGray = 160,160,160^
                auwBlue = 0,128,255^
                auwGreen = 0,128,0^
                auwTomato = 255,99,71^
                auwPink = 252,15,192^
                auwPurple = 128,32,128^
                auwViolet = 238,130,238^
                auwBrown = 165,42,42^
                auwOrange = 255,165,0^
                auwDarkOrange = 255,140,0^




                AUW_POOL_SUBPART
This function for rough scheduling views for determination of the item description of a sub part
with a color code. (TTYP <= 9, no spacers, foils, …). For determination of the color code, the function
AUW_POOL_PAINT is used internally:
        Red      Sub part is not released
        Green    Sub part is released
        Blue     Sub part is taken from stock
        Gold     Sub part is ordered but item is not complete


The function has the following parameter:


A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                      143
@spAuftNr                 Order number
@spPos           Item
@spUPos                   Sub item
@spTeileNr                Part number
@spCounterSubPart         Counter of the sub parts that should be analyzed. Non glass articles are not
counted!


                AUW_PRINT_REMAKE
This SP delivers a character string with script and printer name. With this result, A+W Production
Terminal can control the output of different reports on different printers.
This function is used in a special breakage dialog in A+W Production Terminal in order to send a
cutting report to a cutting printer, a frame report to a frame printer, etc. for re-production.
The SP checks the item type and the procurement type of a specific part. If something is not defined,
a standard script and printer are used.
Syntax:
{SCRIPT:ScriptName;PRINTER:PrinterName}{SCRIPT:ScriptName;PRINTER:PrinterName}{SCRIPT:Scr
iptName;PRINTER:PrinterName}
ScriptName= name of the script or report as defined in A+W Production Terminal (not the physical
name of the report!)
PrinterName = Name of the printer as in the printer implementation in A+W Production Terminal
It is possible to call up several reports per part (e.g. frame with muntin). If only one script (report)
should be called up where the printer is not required, the syntax is: {SCRIPT:ScriptName} or just
{ScriptName}
How is this SP configured on the A+W Production Terminal breakage dialog:
auw_print_remake(awbar_teile.auftnr,                                          awbar_teile.pos,
awbar_teile.u_pos, awbar_teile.teile_nr)


12.3.           Table AUW_SETTINGS
This table includes settings for AUW functions. This table can also be used for customizing. If this is
done, these parameters must be identified with CU_ in the name.
[REPORT / MINRESTBLATT]
Minimal width of residual lites that should not be counted as trash. This switch is used for the AUW
waste statistics. The value is set in 1/1000 mm, default value: 1200000.
[CAPA_VIEW / SHOW_OFFERS]
The switch controls whether quotation data is display in the VIEWs AUW_CAPA_OVERVIEW and
AUW_CAPA_TODO.
         0 = Quotations are filtered
         1 = Quotations are displayed
[CAPA_VIEW / SHOW_RESOLVED_MACROS]



A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                 144
This switch controls the display of resolved macros (MAKRO_AUFGELOEST > 0) in the VIEWs
AUW_CAPA_OVERVIEW and AUW_CAPA_TODO.
     0 = resolved macros are filtered
     1 = resolved macros are displayed




A+W Software GmbH                EN-CONFIG-A+W Production.docx                     145
13. Multi-site
The multi-site function in A+W Production refers to the installation of several A+W Production
environments on a server. On this server, these A+W Production environments are still separated.
Each environment has its own database, its own configuration, and also its own services. All A+W
Production environment use the same A+W Production version and the user has the opportunity
at the start of A+W Production to choose among the configured sites.
If the A+W software is updated on the server, all configured sites are affected.


                                                            Process Server
                                                        BookingService Site 1
                                                        BookingService Site 2
             Database Server
                                                        PPS WebService Site 1
               AWSOA DB                                 PPS WebService Site 2
              AWP DB Site 1                                     …
              AWP DB Site 2




                                                           Terminal Server
               File Server
                                                           AWP Application
          TRANS Share Site 1
          TRANS Share Site 2



Figure 13-1 Multisite infrastructure

When multi-site should be started up, a single site must be installed first. From it, you can change
to MultiSite. Here it must be noted that once you have changed, there is no way back.


13.1.             Preparation
The following must be available before the configuration:
    •    One A+W Production database per site with different names since the name is also the
         name of the ODBC connection.
    •    A release of a TRANS directory on a file server per site
    •    A Windows domain user for the execution of the services per site
    •    One AWSOA environment


13.2.             Configuration
The configuration of the sites is done via the infrastructure in the AWSOA environment. The sites
are created under master data.


A+W Software GmbH                      EN-CONFIG-A+W Production.docx                            146
Figure 13-2 Infrastructure configuration sites

Each site has a number. This should be identical to the site number of the connected ERP site. One
of the defined sites must be marked as default site.
After the sites were created, Windows users must be assigned to the sites. If a Windows user is
assigned to several sites, then at the start of A+W Production, he can select with which site he
would like to connect. Each service user may only be assigned to one site.




Figure 13-3 Infrastructure site assignment




A+W Software GmbH                       EN-CONFIG-A+W Production.docx                         147
For the configuration, Windows users or groups from the left list are assigned to the sites in the
right list using drag & drop.


In the next step, various settings must be made for the individual sites. These are settings that the
A+W Production config tool takes over for the SingleSite, which can no longer be used for MultiSite.
These settings are made in the AWSOA infrastructure under Configuration.




Figure 13:4 Infrastructure configuration

The switches defined here for A+W Production must be configured for each previously-created site.
The site can be changed via the combobox in the upper right area.




Figure 13-5 Infrastructure A+W Production configuration

In the basic settings, the TRANS drive and the user for the Windows services are defined. These
settings are unique per site. The connected drive for the TRANS directory can be identical for all
sites (default is P:). There is a new connection with each start of A+W Production.




Figure 13-6 Infrastructure A+W Production configuration basic settings

The database connection to the A+W Production database in question for the site must be
configured. Unfortunately, there is no function for testing the connection in order to check whether
the settings are correct.


A+W Software GmbH                          EN-CONFIG-A+W Production.docx                         148
Figure 13-7 Infrastructure A+W Production configuration database connection

For the configuration of the URL to the PPS WebService, the site number must also be specified:
http://<ProcessServer>/PPSWebService-C<Client Number>/Albwir.Alcim.DataService.asmx




Figure 13-8 Infrastructure A+W Production configuration PPS WebService URL

The settings for the Service Monitor do not have to be made; the A+W Production MultiSite CONFIG
tool does this. They can be viewed and changed if necessary.




Figure 13-9 Infrastructure A+W Production configuration Service Monitor

If the configuration is complete, the A+W Production MultiSite config tool can be started. On first
start, it asks whether you really want to change to MultiSite. If you confirm this, a flag is set in the
registry. Resetting this manually does not make the server a SingleSite server again. Once it is set,
there is no going back. However, there is nothing that speaks against using the MultiSite function
in an installation with just one site.
    [HKLM\SOFTWARE\WOW6432Node\Albat+Wirsam\Techsoft]MultiClient = 1 (DWORD)
The CONFIG Tool replaces the A+W Production CONFIG Tool; effective immediately, this can no
longer be started. On the first dialog, you have the opportunity to make the trace settings for the
A+W Production modules. For the configuration of the MultiSite, it must be started as
administrator, which can be achieved with the appropriate button on the first dialog.



A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                 149
Figure 13-10 A+W Production MultiSite CONFIG Tool

The CONFIG tool first generates an ODBC connection for each site. On the dialog, all services
required for A+W Production are listed, one per site. With this dialog, you can decide which services
should be installed here if services must be installed on different servers, e.g. for the purpose of
load balancing.
These services are created automatically. The services from the SingleSite are still present, but
deactivated.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                150
Figure 13-11 A+W Production MultiSite CONFIG tool services

In the next step, the CONFIG tool creates one PPS WebService instance per site if the tool is running
on the server to which the WebService address is pointing.




Figure 13-12 A+W Production MultiSite CONFIG tool services

The MultiSite CONFIG tool must run on the process and terminal server.



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                151
Figure 13-13 Services according to A+W Production MultiSite CONFIG tool

The configuration is thus complete, the applications can be started.


13.3.            Starting the applications
If a Windows user is assigned to several sites, a dialog for selecting the site appears at the start of
A+W Production and A+W Realtime Optimizer. So that this works, the AWSOA environment must
be accessible. If this should be running on the process server, the applications will not start should
this server not be accessible, e.g. due to maintenance work. This was different in the SingleSite.
When starting, the TRANS drive is connected to the configured drive, e.g. P. The connected drive is
still required for various older features (e.g. in the area of drivers), which cannot be worked around
with the UNC path of the TRANS drive.




Figure 13-14 A+W Production site selection

A+W Realtime Optimizer can change sites, but in the productive system there must be one
Windows user per site for each A+W Realtime Optimizer. This is due to the direct coupling to a
cutting table. This cannot simply be changed. The basic settings (XOPTON.CFG) are also unique per
Windows user and cannot be changed.


A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                 152
A+W Production Terminal has no appropriate function for changing the site. Here, the correct PPS
WebService must be used; this is configured as usual. When starting A+W Production Terminal,
hold down the <SHIFT> key to reach the PPSWebService selection dialog. Enter the appropriate PPS
WebService there:
http://<ProcessServer>/PPSWebService-C<Client Number>/Albwir.Alcim.DataService.asmx




Figure 13-15 A+W Production Terminal selection of PPSWebService

In order to call up the CapaView from the planning domains, the site number must be specified in
the address:
http://<Server for AWSOA Planning>/Planning.Web/<Client Number>/Capaview
The same applies for the scanner solutions from the AWSOA CIM domains:
http://<Server for AWSOA CIM>/CIM.Web/<Client Number>/SmartTerminalBooking
http:// <Server for AWSOA CIM>//CIM.Web/<Client Number>/barcodereading


13.4.           Special features
So that the sites have their own environments, all settings that do not come from the database are
on the TRANS release of the site. Dependent applications, e.g. A+W CAD Designer (Shapes) must be
configured so that these use their configurations from the TRANS release. This means with direct
use of these dependent applications, these use the configuration of the last started A+W Production
site. Since generally one user is assigned to just one site, there should be no problems. If this is not
the case, this must be noted.
Configurations that cannot be shifted to the TRANS directory must be created in the MultiSite so
that there are no overlaps. In A+W Production this affects the machine drivers that are called with
batch release. Especially cutting code drivers, but also old bender and sealer drivers and new ones
with special configurations. Some of the configuration of these drivers is in the programs directory.
Thus it must be heeded that the configurations, directories for the drivers are unique across sites.


13.5.           Update
In case of an update of the A+W applications in the MultiSite, additional steps must be performed
per site, which happen automatically with SingleSite.
To perform these steps, it is recommended that you dial in on the ProcessServer under each of the
services users since these are assigned only one site, and to perform the steps there.
Databases
The A+W Production database must be updated manually. This happens manually with the
DBUpdateTool. In the Multisite, make sure to update all databases of all sites (also archive
databases!).
Designer screens



A+W Software GmbH                    EN-CONFIG-A+W Production.docx                                  153
The updating of the designer screens (release dialog, A+W Production Terminal screens, etc.) is
done in the SingleSite automatically by the SetupLauncher. In the MultiSite, this must be done
manually since the SetupLauncher does not recognize the sites.
Execute the DesignerFormsUpdater.EXE in a DOS box under each Windows services user on the
ProcessServer.
C:\Program Files (x86)\A+W\Techsoft\Tools\DesignerUpdater\DesignerFormsUpdater.EXE

TEXTE table
The updating of the TEXTE table is done in the SingleSite via the A+W Production CONFIG Tool. In
the future, this should be done by the A+W Production MultiSite CONFIG Tool; until this works, we
must take advantage of a trick.
    1. On the ProcessServer, stop all services and end all applications
    2. Temporarily set the MultiClient switch to 0 in the registry
    3. Under each Windows services user, start the A+W Production CONFIG Tool and there,
       execute only the update of the TEXTE table
    4. Set the MultiClient switch back to 1
TRANS release
The "Shared Folder" diskset updates the data to the TRANS release. In the process, the
SetupLauncher takes the directory that was configured for it; it does not recognize the configuration
of the MultiSite.
The current solution for updating all TRANS releases would be to uninstall the "Shared Folder"
diskset again (this should not delete any data) and reinstall it, while setting the next TRANS release
in the SetupLauncher. Repeat this until you have done all sites.
Alternatively, the data from the updated TRANS release can be copied to the other releases. For
this, however, you have to know exactly what is updated and what is not. If you simply copy the
whole directory, the configuration will destroy the site.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 154
14. Archiving
14.1.            Manual archiving
Batches that are no longer needed in the production system can be archived. For this, the batch to
be archived must be set to "archivable" in A+W Production via the batch display (batch status 2000).




Figure 14-1 Archiving a batch in A+W Production

As soon as the archiving has access to this batch, the status is set to "in archiving" (batch status
2001). The status 2001 marks the batches for further processing (archive or delete). With the
parameter "DELETIONDELAY", you can define a delay in days between the transfer of the status
2000 and 2001. The delay refers to the database field "pool_lauf.lastmodzeit".
Archiving is done via the ALCIMServer that is installed on the ProcessServer. There are 2 ways to do
this. With the first one, the batches are simply deleted; with the second, the batches are shifted to
archive databases. The procedure is controlled with the switch [ALCIM_ARCHIV / NOARCHIV]: 0 =
archive databases; 1 = delete.




Figure 14-2 Archiving or deleting configuration batches

If batches should be archived in archive databases, then the appropriate databases and an ODBC
data source must exist. One database per year and one additional database that is used for
problems are required. By default, this database has the name ALCIMQRT and the annual databases
have the year at the end of their names (e.g. ALCIMQRY2019). The ODBC data source must be set
up on the ProcessServer on which the ALCIMServer service is running.


A+W Software GmbH                      EN-CONFIG-A+W Production.docx                             155
The ODBC connect string for the archive database must be configured in A+W Production
([ALCIM_ARCHIV / DATABASE]), here the syntax is different for INFORMIX and SQLServer. For
SQLServer, the database user and password must be stored here for the person who has the right
to delete data from the production database and write it in an archive database. This information
is stored under INFORMIX directly in the IDBC data source.
Informix:         DSN=<ODBC data source>; DATABASE=<archive database without year>;
SQLServer:        DSN=<ODBC data source>; DATABASE=<archive database without year>;
                  UID=<user>; PWD=<password>;




Figure 14-3 Configuration of DSN for archive database

In addition to the data in the database, files can also be deleted during archiving. These can be file
with batch reference ([ALCIM_BDESETTINGS / DELETE_FILE_WITHSCHEDULE]), e.g. optimization
results, or files with order references([ALCIM_BDESETTINGS / DELETE_FILE_WITHORDER]),
ORDERXML files. It is also possible to set whether SN files that are assigned to the items should be
deleted ([ALCIM_BDESETTINGS / DELETE_SN_FILES]).




Figure 14-4 Configuration deletion of files during archiving




A+W Software GmbH                       EN-CONFIG-A+W Production.docx                             156
14.2.           Automatic archiving
Since July 2020 (#45912), there are additional archiving modes that can be activated with the pa-
rameter ([ALCIMSVR] / [BATCH_ARCHIVING_MODE]).
0 = previous behavior, status must be set manually to 2000
1 = batches with the status 700 (produced) or higher are archived
1 = batches with the status 800 (packed) or higher are archived
3 = batches with the status 900 (delivered) or higher are archived
The batch statuses 700 – 900 are set automatically by AlcimBooking based on pool_bearbeit.fi-
nal_kz:
All header parts in the batch with pool_bearbeit.Final_KZ = 1 -> 700 produced-> pool_teile.bdefer-
tig > 0
All header parts in the batch with pool_bearbeit.Final_KZ = 2 -> 800 packed -> pool_teile.bde_ver-
packt > 0
All header parts in the batch with pool_bearbeit.Final_KZ = 3 -> 900 delivered ->
pool_teile.bde_versendet > 0
CAUTION: If one of the new Archivierunsmod1 (1, 2 or 3) is used, it is necessary that the delay of
the archiving be set to at least one day in order to prevent immediate archiving (e.g. in order to
book breaks after the fact). For security reasons, therefore, always use one day delay as soon as
BATCH_ARCHIVING_MODE > 0 and DELETIONDELAY < 1.


Booking discipline
The automatic archiving is based on PDC bookings and therefore depends on the booking discip-
line. As soon as a header part in a batch does not reach the appropriate status, the batch status
cannot be set and thus the automatic archiving is initiated. Therefore, attention has to be paid
that especially the header parts are booked completely.
AlcimBooking takes are of forgotten bookings for subparts as well as it can automatically. This is
controlled via the fields "bdefertig“, "bde_verpackt" and "bde_versendet“ in the table
"pool_teile." Each of these fields can assume the following values:
0 = not yet complete
1 = PO quantity was reached
2 = PO quantity plus the surplus (=maximum quantity) was reached
If you are working without surplus, the value changes directly from 0 to 2 as soon as all lites are in
the appropriate condition (available, packed or sent).
As soon as all header parts are booked packed (that is, all processing on the header parts with
pool_bearbeit.Final_KZ = 2 were booked), pool_teile.bde_verpackt is 1 or 2 and AlcimBooking en-
sures that this value is also inherited by all subparts. This achieves the following:
    a) Forgotten bookings on subparts are "corrected"
    b) Batches that only include subparts or subparts whose header parts are in other batches
       can nevertheless receive a status for automatic archiving



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 157
Essentially it applies that: a complete archiving of a batch can only be done when dependent bat-
ches (which contain common order items) are also in this status. Since you can never assume
100% booking reliability, you can support customers with helpful views or reports.


14.3.           Expanded automatic archiving
A new configuration switch "Archiving method" has been introduced in order to switch between
the old archiving method (which is set and used by default) and the new "expanded" method,
which is less restrictive and allows the archiving and releasing of more batches.




0 = Standard archiving method
1 = expanded checking of the batches. Here additional flags of the orders are considered in a
batch in order to check whether an order can be archived. This method is less restrictive than the
standard method.
The parameter "BATCH_ARCHIVING_MODE" tells the AlcimServer starting with which status a
batch should be regarded as "ready for archiving". The value of "Automatic batch archiving" can
be 1=Status 700 (produced), 2=Status 800 (packed), 3=Status 900 (delivered) or 0=Status 2000
(set manually as archivable).


         How "standard method" works
Example for batch 1000, whose status is set to 900
and the configuration parameter "archivable status" is set to 3 (status 900, delivered).




If AlcimServer processes the batch 1000 [column A] with a status equal to or greater than "archi-
vable status" (900 in the example), it checks all orders of the batch 1000 [column D] and then
checks in which other batches contained [column F] and whether they all have a status equal to or
greater than "archivable status".

In this example, the order 2000001 cannot be archived because there is another batch 1002 that
also contains this order and this batch only has the status 700. Since this is less than "archivable
status," batch 1000 cannot be archived.




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                158
                How "expanded method" works
The new method was invented in order to be able to archive more batches.

The new method enables the archiving of orders that can be regarded as completed, even if they
are included in another batch with a status less than "archivable status" but with a status equal to
or greater than 700 (= produced).

Example: batch 1000 has the status 900 and the parameter "archivable status" is set to 3 (900, de-
livered).




If the status of the batch is 700 or larger and smaller than "archivable status," then other data re-
cords from pool_teile and pool_auftrag also have to be analyzed.

Part of an order 2000001 [column D], which is included in the batch 1001 [batch F] does not have
to be analyzed since the status [column G] of this batch is equal than or greater to "archivable sta-
tus".

But another part of the order 2000001 [column D] that is included in the batch 1002 [column F]
has to be analyzed because the status [column G] of this batch is 700 or greater and less than "ar-
chivable status".

The condition that this part of the order 2000001 [column D] counts as archivable is that all
pool_teile data records for the specified batch and given order have set at least one of bdefertig |
bde_verpack | bde_versendet flags [columns K,L,M] to a value not equal to zero or that the auftkz
value of the pool_auftrag has to be greater than zero (canceled).

As you can see in comparison to the standard method, the new method considers the order
2000001 [column D] as archivable and thus the batch 1000 can be archived.


14.4.           Archiving via customizing
With customizing, orders can be marked in the database as archivable. The booking service checks
the status of all batches that are at least released once a day at 12:00 AM. Here the batch status is
increased if this is possible. If, for example, a batch contains an archivable order that is not dis-



A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                 159
patched and a dispatched order, the batch status is set to dispatched (900). The check by the boo-
king service is only done if the automatic archiving is configured by the AlcimServer. Thus, the
batch is archived, even if not all orders are booked accordingly.
The archiving of orders can be identified via a customizing in that you enter a value > 0 in the
pool_auftrag.force.


14.5.            How is archiving done?
By default, archiving is done year by year, one archive database per year. The year in question and
the associated archive database is determined with the following stored procedures. If these are
changed, the default behavior can be changed, but this is not recommended.
    •   cu_alcsv_arcord (archiving of the orders)
    •   cu_alcsv_arcsched (archiving of the batches)
    •   cu_alcsv_arcopt (archiving of the PMO data)
An order is only archived if all items of this order are completely planned in archivable batches. If
this is not the case, the batch remains with the status "in archiving" (2001) until the condition is
fulfilled and the batch can be archived completely.
In addition to the manual possibilities for archiving a batch, there is also the archiving pot 12600.
Cancelled orders are shifted to it and archived automatically by the ALCIMServer service.
The archiving of batches marked for archiving starts X days after marking. The time in days can be
configured with the switch [ALCIM_SETTINGS / DELETIONDELAY]. If the switch is set to the value 0,
the archiving begins immediately. The day of marking comes with the time stamp
POOL_LAUF.LASTMODZEIT.




Figure 14-5 Configuration of deletion delay



14.6.            Archive databases
Archive databases have the same data structure as the production database. On first access by the
ALCIMServer service, it adds the field XXXARCTIME to each table.
For an update of the structure of the production database, the structure of all archive databases
must also be updated accordingly.



A+W Software GmbH                      EN-CONFIG-A+W Production.docx                               160
To generate a new, empty archive database, the data structure of the production database must
be backed up. A new archive database is created and this data structured loaded. The data structure
may not include any TRIGGERs; functions, stored procedures, and VIEWs are not required. Required
are the indexes of the tables.
After the structure is loaded, a data record with the version of the data structure must be entered
in the PARAMETER table. This data record can be unloaded from the production database and
loaded into the archive database or you can add it directly to the archive database with INSERT:
INFORMIX: INSERT INTO parameter (lastmodstation, lastmodzeit, bereich, eintrag, nummer,
typ, text) VALUES ('INIT', TODAY,'DATENBANK','ALCIM',0,1,'<DB Version>');

SQLServer: INSERT INTO parameter (lastmodstation, lastmodzeit, bereich, eintrag, nummer,
typ, text) VALUES ('INIT', CURRENT_TIMESTAMP,'DATENBANK','ALCIM',0,1,'<DB Version>');

INFORMIX (Windows)
To be executed on the database server in the DOX boxes of the environment. It may be necessary
to adjust the commands to the environment in question.
Load data from production database:
DBSCHEMA -d alcimdb C:\Temp\dbschema.sql
ECHO unload to 'c:\Temp\parameter.uld' select * from "alcimdb".parameter WHERE
eintrag = "ALCIM" AND bereich = "DATENBANK" | dbaccess alcimdb
Generate archive database:
ECHO create database alcimqry2019 in alcimqry with buffered log | dbaccess
DBACCESS alcimqry2019 C:\Temp\dbschema.sql


ECHO load from 'c:\Temp\parameter.uld' insert into "alcimdb".parameter | dbaccess
alcimqry2019
LOMOSET -isvalcimqry -dbnalcimqry2019
SQLServer
With the SQLServer Managment Studio, the structure can be created with the script wizard in a SQL
file (Select database  Tasks  Generate Scripts…). Select all tables and activate the option that
indexes should be taken along.
Then execute script generated on a generated archive database and then transfer the version to
the parameter table.
USE alcimqry2019
INSERT INTO parameter SELECT * FROM alcimdb..parameter WHERE bereich='DATENBANK' AND
eintrag='ALCIM'


14.7.           Tables used
The ALCIMServer service analyzes the tables to be archived dynamically. Thus it is possible to create
customer-specific tables and also to have them processed by the archiving. Of course these tables
also have to exist in the archive databases.
For the analysis of the tables, the ALCIMServer service proceeds in the following steps:




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                161
Order tables
The table is an order table if the following is fulfilled:
    •   Table includes an AUFTNR column
    •   Exceptions are tables ...
             •   … AWBAR_CHARGE, ERP_RUECKMELDUNG, AWINFO_TEMP_ORDER
             •   ... whose names begin with BDESTAT_
Batch tables
The table is a batch table if the following is fulfilled:
    •   Table contains a LAUF, JOB or JOBID column
    •   Table includes no AUFTNR column
    •   Exceptions are tables ...
             •   …    XOPT_STATISTIK,           XOPT_STATISTIK_JUMBO,        CU_IP_STATISTIK_KOPF,
                 CU_IP_STATISTIK_PROD
             •   ... whose names begin with BDESTAT_
PMO tables
The table is a PMO table if the following is fulfilled:
    •   Table includes an OPTI_ID column
    •   Table name begins with PMO_
    •   Exception is the table PMO_ITEMS


14.8.            Archiving the SKIZZEN table
The SKIZZEN table contains images of the individual lites. Data from this table is archived if the time
stamp of the data records is older than a configured number of days. This is controlled via the
configuration file LABELPRINT.INI. Also controlled via this configuration is that you should not
delete the image files. These exist in addition to the SN drawings and are copied into the SKIZZEN
table with the batch release. The JPG files are deleted by the archiving on the ALCIMServer. If the
SKIZZEN of a batch are deleted although lists with sketches should be printed again, these can be
copied again into the SKIZZEN table by repeating the sketch generation in the batch release.
        [ALCIM_Skizzen]
        CleanRecordsAfterDays=5
        DoNotDeleteAlcimSNDrawFiles=Yes
        DoNotDeleteAlcimSNDrawFilesAtAll=Yes
The switches ACCESS_DSN and CompactDatabase have no more significance; they come from
the times when sketches were saved in an individual Access database.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                162
15. A+W IoT Smart Trace
15.1.            Basic configuration
                 Gateway connection settings
So that data and documents can be sent via the gateway service to external systems such as
Actiware, connection points are configured under A+W Infrastructure Web.
For this, start the web interface of the Infrastructure Services using the following URL:
http://servername/infrastructure.web
or open via the A+W folder on the desktop. Now select the configuration dialog.




Figure 15-1 Infrastructure Web start page

Now enter the gateway connection settings under the Gateway point:




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                         163
Figure 15-2 Configuration of the gateway connection settings

In the current version of the Actiware modules, NO encrypted connection is possible; the switch
must remain in the default value OFF. Similarly, neither user nor password is evaluated.


                 PDC configuration
So that PDC data is sent to the gateway service, the master data in A+W Production must be
adjusted as follows:
Via Master Data > Configuration, you can reach the Parameter Administrator. Search here in the
barcoding booking service for "gateway" and set the switch Barcoding Statistics > External
Barcoding Statistics to 1.




Figure 15-3 Activating the PDC data transfer to the gateway service

Setting this value causes the booking data to be written to the awbar_gateway_data table. It can
then be forwarded by the gateway service to external services.




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                         164
15.2.           Sending reports
This function was previously realized for the A+W Production Terminal screens Order and xxx-Out.
If reports are printed in the production environment, for example from an A+W Production
Terminal, it is possible to send these to external systems. For this, the following settings must be
made:
    •   Press [Ctrl] + [F12]
    •   Insert an output field with the action REGPOINTOUT. For example, this field can be placed
        behind the SNLive view. This field is required so that the registration point number can be
        included with the report.




A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                165
    •   Open     the    script   processing    with    the    "Script   and     Reports"    rubric




    •   Set the "Archive report" switch to [True]




    •   Confirm with OK
This configuration must be done per screen and then applies automatically to all reports.




A+W Software GmbH                  EN-CONFIG-A+W Production.docx                              166
16. Other functions
This section describes functions that cannot be assigned clearly to any other section.


16.1.            Parameter Administrator
In A+W Production, the Parameter Administrator serves to make general and station-dependent
settings in A+W Production. The Parameter Administrator can be reached in A+W Production via
the menu Master Data  Configuration. From dialogs with Designer technology (A+W Production
Terminal, release dialog, etc.), the Parameter Administrator can be reached with the key
combination <CTRL><F9>.
When creating a new station in A+W Production, station parameters in the "General" area must
always be present. In other areas, these are only necessary if the corresponding functions are used.
For this reason, you can only enter new stations in this area. A station in A+W Production has a
length of 2 digits or letters.




Figure 16-1 Parameter Administrator: Creating a new station

In other areas, you can only select a station that already exists under "General" from a list when
creating a new station.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                             167
Figure 16-2 Parameter Administrator: Transferring a new station

The same behavior occurs if in an area you mark a station and want to copy it. Then in the "General"
area you have the opportunity to enter a new station and in other areas the selection of a station
already present in "General".


16.2.            Document links
It is possible to attach external documents (e.g. a PDF) to an order or individual items of an order.
These documents can be displayed and printed using various functions in A+W Production.


                 A+W Production
Document links are stored in A+W Production in the database table POOL_DOKUMENTE.
Documents that are assigned the item 0 apply for the entire order.
From the POOL views, document links can be managed with the [Belonging documents] context
menu. Existing document links can be opened, deleted, created anew or edited.




Figure 16-3 Management of document links

With batch release, there is a function for printing the document links of a batch.


A+W Software GmbH                     EN-CONFIG-A+W Production.docx                              168
Figure 16-4 Print document links on release

By default, this prints all documents of an item for all end products found in the batch. If an item is
split into several batches, the documents are only printed in the batch where the end product is
located. Order-related documents are not printed.
Printing is controlled by the script DocumentLink.vb. Customer-specific adjustments incur costs;
for this, a copy of the file with the customer abbreviation must be created.
Caution: Opening is only possible if there is a link to the Doculink from the A+W Production station
(ideally always use the UNC path) and the file format can be started by an application linked in
Windows.


                 A+W Production Terminal
In A+W Production Terminal, the link is displayed in the element "Linkeddocuments":




Figure 16-5 Document links in A+W Production Terminal

This element is available on all screens. The links displayed can be filtered for each screen using a
parameter via the type The link.




Figure 16-6 Switch filter document links in A+W Production Terminal

Caution: Opening is only possible if the WebService can establish a link to the Doculink (ideally
always use the UNC path) and the file format can be started by an application linked in Windows to
the A+W Production Terminal Client.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                169
                 Entry in A+W Business
In the document entry, item entry, and in the product, customer, supplier, and partner master data,
there is a storage possibility for any file attachments, e.g. Word files, Excel files, JPEGs, and e-mails.
These are simply saved in the corresponding field via the usual Windows drag & drop function. Here
it is also possible to copy elements from Outlook, Outlook Express, and Windows Live Mail directly
via drag & drop. Supported are mails, contacts, attachments, and calendar entries.




Figure 16-7 File attachment in A+W Business

A+W Business copies the files into a directory stored in the company master data (Master Data >
Company Data > 4. Documents):




Figure 16-8 Configuration directory for file attachment in A+W Business

The directory stored there is completed with the document type, document number and (if
applicable) item number or master data type, and is saved. Only the relative path is saved in the
database.




Figure 16-9 Directory for file attachment in A+W Business

Click on such an attached file in A+W Business to start the corresponding application, and to open
the document linked to the file type.
All file attachments can be grouped by type now. This helps to control which file attachments will
be taken over for the transfer to production (OrderXML), copying quotations into orders, and PO
transfer (e.g. product information) and which shall not (e.g. calculation information).




A+W Software GmbH                      EN-CONFIG-A+W Production.docx                                 170
Figure 16-10 Types for file attachment in A+W Business

For the setup, the required attachment types have to be defined in text master data (Master Data
> Text > File Attachment Types) before they are activated in the settings dialogs for transfer to
production (Production > Production > Production Transfer > Function Settings), Copy documents
(Documents > Quote > Quote NM > Copy Documents), and PO transfer (Documents > Order > P.O.
transfer).




Figure 16-11 Configuration transfer file attachment from A+W Business

By default, all attachments are initialized with type A (all) and will always be transferred (exception:
PO transfer).
File attachments in the document order entry
Essentially, an attachment can only be assigned to a document if the document has already received
a valid document number.
In item entry, an attachment is visualized with an appropriate icon.




A+W Software GmbH                     EN-CONFIG-A+W Production.docx                                 171
Figure 16-12 File attachment in item entry in A+W Business

In the document view, the document links can also be displayed on an individual tab. This is possible
even for archived documents.




Figure 16-13 File attachment in document view in A+W Business

When importing orders via EDI interface (Documents > Order > Import), document attachments
can also be imported. These are pre-populated with the document link type A.
When you copy documents, only the file reference will be copied, not the file itself. When you enter
series at item entry, the annexed file will not be kept.
During the saving of items as macros, existing document links are also saved.
An overview of the attachments to the product is found on the item info dialog on tab 3.
Attachments, from which they can be opened with a double-click. Thus, this data can be accessed
quickly at any time in the document entry.




Affected database tables
File attachments in A+W Business databases are saved in the following tables:
KA_ATT_TYPE                       File attachment types
BA_MAKRO_ATT_POS                  File attachments for macros
BW_ANFR_ATT_KOPF                  Inquiry file attachment header
BW_ANFR_ATT_POS                   Inquiry file attachment items


A+W Software GmbH                     EN-CONFIG-A+W Production.docx                              172
BW_ANGEB_ATT_KOPF    Quotation file attachment header
BW_ANGEB_ATT_POS     Quotation file attachment items
BW_AUFTR_ATT_KOPF    Order file attachment header
BW_AUFTR_ATT_POS     Order file attachment items
BW_GUTSCH_ATT_KOPF   Credit note file attachment header
BW_GUTSCH_ATT_POS    Credit note file attachment items
BW_BEST_ATT_KOPF     Purchase order file attachment header
BW_BEST_ATT_POS      Purchase order file attachment items
BA_PRODUKTE_ATTACH   File attachment for products
KU_ATTACH            File attachment for customers
LI_ATTACH            File attachment for suppliers
PA_ATTACH            File attachment for partners
FS_ATT_KOPF          File attachment on header level from external interface
FS_ATT_POS           File attachment on item level from external interface




A+W Software GmbH       EN-CONFIG-A+W Production.docx                          173
17. Production Monitor
17.1.            Overview




Figure 17-1 Production Monitor



17.2.            Detail view

With the         icon (upper left corner of the Production Monitor), you can switch to a detailed
view for a day. Here, the various planning states of the orders are depicted with different colors:


 In the pool

 Rough and detailed
 scheduling
 Released




A+W Software GmbH                   EN-CONFIG-A+W Production.docx                                174
The tooltip in this display indicates the precise data:




Figure 17-2 Tooltip display in Production Monitor



17.3.                Backlogs and workload
                     Display
Backlogs are displayed when you move the mouse over a traffic light display:




Figure 17-3 Display of backlogs

Here, all lites are regarded that must still be produced in the period Today-30 days - until today
(incl. - changed starting with 5.3; see below)(and are not yet finished).
If only values (that is, no times) will be displayed for the backlogs (see figure),



then no specified times are stored for this machine.
The data displayed (status A+W Production 5.1) will be determined with the following SQL (SQL
Server):
SELECT
SUM((pt.menge_nach - pt.mindermenge_nach) * pb.dauer) AS backorderAmount,
SUM(pb.dauer * (CASE pb.menge WHEN 0 THEN pt.menge
                              ELSE pb.menge_gut / pb.menge END)) AS backorderAmountDone,
SUM((pt.menge_nach - pt.mindermenge_nach)) AS backorderCount,
SUM(CASE pb.menge WHEN 0 THEN pt.menge
                   ELSE pb.menge_gut / pb.menge END) AS backorderCountDone

FROM pool_bearbeit pb, pool_teile pt, pool_pos pp

WHERE pb.auftnr = pt.auftnr
 AND pb.pos = pt.pos
 AND pb.u_pos = pt.u_pos
 AND pb.teile_nr = pt.teile_nr
 AND pb.prod_term >= convert(date, dateadd(d,-30,getdate()))
 AND pb.prod_term < cast(getdate() as date)
 AND pb.auftnr = pp.auftnr



A+W Software GmbH                             EN-CONFIG-A+W Production.docx                     175
 AND pb.pos = pp.pos
 AND pb.u_pos = pp.u_pos
 AND pp.auftkz = 0
 AND pb.mzo_id_phys = 110



Starting with Version 5.3, the new fields from pool_bearbeit are used:
SELECT
SUM((pt.menge_nach - pt.mindermenge_nach) * pb.dauer) AS backorderAmount,
SUM(pb.dauer * (CASE pb.menge WHEN 0 THEN pt.menge
                              ELSE pb.menge_gut / pb.menge END)) AS backorderAmountDone,
SUM((pt.menge_nach - pt.mindermenge_nach)) AS backorderCount,
SUM(CASE pb.menge WHEN 0 THEN pt.menge
                   ELSE pb.menge_gut / pb.menge END) AS backorderCountDone

FROM pool_bearbeit pb, pool_teile pt, pool_pos pp

WHERE pb.auftnr = pt.auftnr
 AND pb.pos = pt.pos
 AND pb.u_pos = pt.u_pos
 AND pb.teile_nr = pt.teile_nr
 AND pb.prod_term >= convert(date, dateadd(d,-30,getdate()))
 AND pb.prod_term < cast(getdate() as date)
 AND pb.auftnr = pp.auftnr
 AND pb.pos = pp.pos
 AND pb.u_pos = pp.u_pos
 AND pp.auftkz = 0
 AND pb.mzo_id_phys = 110



You can reach the backlog display by clicking the right mouse button on the traffic light symbol ...




... and selecting "Display backlog".
In the following display, 2 filters should be set:



"Max backlogs (-30)":
cast(pool_bearbeit.prod_term as date) >= convert(date, dateadd(d,?,getdate()))
With StandardParameter -30
filters the backlogs to a maximum of 30 days in the past. Without this filter, all backlogs are drawn
from the database.
"Only production orders":
POOL_POS.AUFTKZ<>90 and POOL_AUFTRAG.AUFTKZ<>90
filters out the quotation orders.
This display also displays the backlogs starting 30 days in the past, however WITHOUT today

The weight should be calculated in the work plan from pool_teile.flaeche * pool_teile.dicke / 1000
* 2,5 * pool_bearbeit.menge_prod. Then the data will match the figures from the Production Mo-
nitor. For insulated glass, this does not hold true, but there a display in weight makes no sense.
Pool_teile.flaeche is important in this formula since this way, shapes are also taken into account.




A+W Software GmbH                              EN-CONFIG-A+W Production.docx                     176
Pool_bearbeit.menge_prod is important since with it, cancellations are displayed correctly (in
case of cancellation, reduces in contrast to pool_teile.menge)


                      Workload
You can display the workload of a shift by moving the mouse over a shift in the Production Moni-
tor:




Figure 17-4 Utilization of a shift

The data for this is gathered with the following SQL:
SELECT
pb.prod_term AS prod_term,
 pb.schicht AS schicht,
 pb.mzo_id_phys AS mzo_id_phys,
pb.mzo_technologie1 AS mzo_technologie1,
COUNT(*) AS rcount,
SUM(pb.dauer * pt.menge) AS wload,
SUM(pb.dauer * (CASE pb.menge WHEN 0 THEN pb.menge
                                  ELSE pb.menge_gut / pb.menge END)) AS wloaddone,
SUM(CASE pb.menge WHEN 0 THEN pb.menge
                       ELSE pb.menge_gut / pb.menge END) AS wdone,
SUM(pt.menge) AS squantity,
MAX(pb.sequenz) AS maxSequenz ,
 pt.status AS pt_status

FROM pool_teile pt, pool_bearbeit pb, pool_pos pp

WHERE pb.prod_term >= CAST('2013-10-23' as date) AND
pb.prod_term <= CAST('2013-10-23' as date) AND
pb.mzo_id_phys IN (2910) AND

pt.auftnr = pb.auftnr AND
pt.pos = pb.pos AND
pt.u_pos = pb.u_pos AND
pt.teile_nr = pb.teile_nr AND

pt.auftnr = pp.auftnr AND
pt.pos = pp.pos AND
pt.u_pos = pp.u_pos AND

pp.auftkz = 0

GROUP BY pb.prod_term, pb.schicht, pb.mzo_id_phys, pb.mzo_technologie1, pt.status



Starting with Version 5.3, the new fields from pool_bearbeit are also used:
SELECT
pb.prod_term AS prod_term,
pb.schicht AS schicht,
pb.mzo_id_phys AS mzo_id_phys,
pb.mzo_technologie1 AS mzo_technologie1,
COUNT(*) AS rcount,
SUM(pb.dauer * (CASE pb.menge_prod WHEN 0 THEN pt.menge



A+W Software GmbH                             EN-CONFIG-A+W Production.docx                      177
                                       ELSE pb.menge_prod END)) AS wload,
SUM(pb.dauer * (CASE WHEN pb.menge = 0 THEN pb.menge
                       WHEN pb.menge_prod = 0 THEN (pb.menge_gut / pb.menge)
                       WHEN pb.menge_gut > pb.menge_prod THEN (pb.menge_prod / pb.menge)
                       ELSE (pb.menge_gut / pb.menge) END)) AS wloaddone,
SUM(CASE WHEN pb.menge = 0 THEN pb.menge
           WHEN pb.menge_prod = 0 THEN (pb.menge_gut / pb.menge)
           WHEN pb.menge_gut > pb.menge_prod THEN (pb.menge_prod / pb.menge)
           ELSE (pb.menge_gut / pb.menge) END) AS wdone,
SUM(CASE pb.menge_prod WHEN 0 THEN pt.menge ELSE pb.menge_prod END) AS squantity,
MAX(pb.sequenz) AS maxSequenz ,
pt.status AS pt_status
FROM pool_teile pt, pool_bearbeit pb, pool_pos pp
WHERE pb.prod_term >= @start_prod_term
 AND pb.prod_term <= @end_prod_term
 AND pb.mzo_id_phys IN (110,120,130)
 AND pt.auftnr = pb.auftnr
 AND pt.pos = pb.pos
 AND pt.u_pos = pb.u_pos
 AND pt.teile_nr = pb.teile_nr
 AND pt.auftnr = pp.auftnr
 AND pt.pos = pp.pos
 AND pt.u_pos = pp.u_pos
 AND pp.auftkz = 0
GROUP BY pb.prod_term, pb.schicht, pb.mzo_id_phys, pb.mzo_technologie1, pt.status




                   Known problems (in A+W Production 5.1/5.2):
    -    Tooltip of the backlogs takes today into account, the display does not  #286367 (elimi-
         nated in 5.3 or with Hotfix „0_A+W Production 5_1976.zip“)
    -    Tooltip for the backlogs and work plan do not consider PDC cancellations (that is, still oc-
         cupy the capacity)  #286365 (eliminated in 5.3 or with Hotfix „0_A+W Production
         5_2113.zip“)
    -    No PDC tables should be used in the workplan. Here, please use only the pool tables since
         otherwise there will be undesired effects:a) the "figures" will not be correct
         b) for quotation orders, no data will be displayed (since not PDC-initialized)


17.4.              Manual completion notification
Backlogs cannot be reported completed directly from the workplan.


                   The process
For this, you select a machine/shift from which the lites should be reported completed:




Figure 17-5 Display in the Production Monitor


A+W Software GmbH                          EN-CONFIG-A+W Production.docx                          178
Then you open the workplan (double-click or right mouse-click). Here, you then mark the or-
ders/processings that should be reported completed and select the "Report completed" option on
the context menu:




Figure 17-6 Batch overview

After that, another confirmation message appears:




Figure 17-7 Program message

and here we go. That is, all lites from the selection (with their components that you have sear-
ched for) and are booked to the planned esnr_soll.


                Limitations
    -   The lites will be booked normally. That is, also in awbar_teile, they are suddenly on a re-
        gistration point where they never were before
    -   In awbar_teile, you cannot detect that this is a manual booking (except that no person is
        specified; in awbar_booking, the station is "DEBKMO"). That is, the statistics are "mucked


A+W Software GmbH                  EN-CONFIG-A+W Production.docx                                   179
       up" and you must take this into account. Therefore, should only be used only in case of
       emergency and if you are sure that the lites are truly complete.
   -   the subparts are not "married". That is, you do not see which subparts are installed in a
       header part. The defect management then does not work with such parts!
   -   in the MZO and in the column assignments, the same registration points must be used.
       That is, if the MZO calculate an ESNR-target 1610 and the ESNR 1612 is responsible in the
       column assignment for the processing booking, the lites are booked to the 1610, but they
       do not disappear from the backlog list!


               Known Problems
For the booking, broken lites are also written to awbar_booking, which causes error messages in
the PDC post-processing  286361: is solved with Hotfix 0_A+W Production 5_1791.zip.




A+W Software GmbH                 EN-CONFIG-A+W Production.docx                                180
18. Table of Figures
Figure 1-1 Parameter administrator: specification of the sequences in O4P .................................. 10
Figure 1-2 Parameter administrator: Specification of the sequences in O4P - example of
     ResolveMacroProcessing ......................................................................................................... 17
Figure 1-3: ALLOW_LATE_POSTPONE_TO_PAST ............................................................................. 20
Figure 1-4: IGNORE_TEXTCHANGES_IN_LATEORDERCHANGE ........................................................ 22
Figure 1-5: IGNORE_COMISSION_CHANGES .................................................................................... 23
Figure 1-6: CHANGE_POS_LIEFTERM ............................................................................................... 24
Figure 2-1 Pool display - selected filters .......................................................................................... 25
Figure 2-2 Field definition of the rough scheduling for fields from a VIEW..................................... 26
Figure 3-1 ProcessManagerControl.................................................................................................. 36
Figure 3-2 Parameter group ............................................................................................................. 37
Figure 3-3 Parameter leading group ................................................................................................ 37
Figure 3-4 Configuration of report mode INTERNAL ........................................................................ 37
Figure 3-5 Parameters PDF output directory ................................................................................... 38
Figure 3-6 Parameter [POOL_SETTINGS / SCHEDULE_RELEASE_STORNO]...................................... 38
Figure 4-1 Parameter administrator: specification of the version of the Crystal Report runtime .. 40
Figure 4-2 Crystal Report Designer - Parameter field dialog ........................................................... 41
Figure 4-3 Example of true to scale sketch ...................................................................................... 42
Figure 4-4 Switch [ITEMS4ALCIM_SPECIALS / CREATE_SN_FILE_BY_ORDERXML] .......................... 42
Figure 4-5 Switch [POOL_SN / DATAFILEPATH] ............................................................................... 43
Figure 4-6 Switch [ALCIM_SHAPE / SNCUTASSTANDARDFRM] ....................................................... 43
Figure 4-7 Switch [ALCIM_SN / SKETCHPRINTINGVIEWS] ............................................................... 43
Figure 4-8 Sketch configuration dialog ............................................................................................ 44
Figure 4-9 Switch [ALCIM_BDESETTINGS / DELETE_SN_FILES] ........................................................ 44
Figure 4-10 Sketch with profile ........................................................................................................ 44
Figure 4-11 Switch [ALCIM_SHAPE / SN_FLIPMODE]....................................................................... 45
Figure 4-12 AWPLogoTableEditor .................................................................................................... 46
Figure 4-13 AWPLogoTableEditor – configuration of database ....................................................... 46
Figure 4-14 AWPLogoTableEditor – Trace display ........................................................................... 47
Figure 4-15 AWPLogoTableEditor – adding a logo ........................................................................... 47
Figure 4-16 AWPLogoTableEditor – image file selection ................................................................. 47
Figure 4-17 AWPLogoTableEditor – editing a logo........................................................................... 48
Figure 4-18 AWPLogoTableEditor – deleting a logo......................................................................... 48
Figure 4-19 AWPLogoTableEditor – saving a logo............................................................................ 49
Figure 6-1 Reporting process ........................................................................................................... 55
Figure 6-2- Switch [ALCIM_STATE / ERPFEEDBACK] ........................................................................ 56
Figure 6-3 Parameter Status Registrations ...................................................................................... 56
Figure 6-4 Switch [ALCIM_STATE / ERP_DETAILED_FEEDBACK] ...................................................... 58
Figure 6-5 Master data registration point for processing reporting ................................................ 58
Figure 6-6 Switch rack feedbacks ..................................................................................................... 58
Figure 6-7 Master data Registration point for rack feedback .......................................................... 59
Figure 6-8 Switch [ALCIMBOOK / TABLEIDSXOPTFEEDBACK] .......................................................... 62
Figure 6-9 A+W Business Feedback Process .................................................................................... 63
Figure 6-10 A+W Business Configuration Feedback ........................................................................ 64
Figure 6-11 A+W Business Open production overview .................................................................... 65
Figure 6-12 A+W Business Old production overview ....................................................................... 65
Figure 6-13 A+W Business Production overview based on a report ................................................ 66


A+W Software GmbH                                EN-CONFIG-A+W Production.docx                                                       181
Figure 6-14 A+W Business Configuration Production overview based on a report ......................... 66
Figure 6-15 A+W Business classic product overview ....................................................................... 66
Figure 6-16 A+W Business view delivered racks .............................................................................. 67
Figure 6-17 A+W Enterprise feedback process ................................................................................ 67
Figure 6-18 A+W Cantor feedback process ...................................................................................... 69
Figure 6-19 A+W Cantor configuration feedback directory ............................................................. 69
Figure 6-20 A+W Cantor configuration system queue ..................................................................... 70
Figure 6-21 A+W Cantor configuration part additions ..................................................................... 70
Figure 6-22 A+W Cantor configuration terminal group ................................................................... 71
Figure 6-23 A+W Cantor rack group designer .................................................................................. 71
Figure 6-24 A+W Cantor rack group result....................................................................................... 71
Figure 6-25 A+W Production parameter for A+W Cantor rack feedback ........................................ 72
Figure 8-1 Connection data of the e-mail server ............................................................................. 76
Figure 8-2 Configuration of the booking service for e-mail dispatch and background printing ...... 77
Figure 8-3 Parameter configuration in Crystal Reports ................................................................... 78
Figure 8-4 DB table awbar_barcodetypen ....................................................................................... 79
Figure 8-5 CIM Server Settings ......................................................................................................... 80
Figure 8-6 Regex configuration ........................................................................................................ 80
Figure 8-7 Regex adapted ................................................................................................................ 81
Figure 8-8 Uploading the new configuration ................................................................................... 81
Figure 8-9 New configuration........................................................................................................... 81
Figure 10-1 Parameter Administrator with parameter "Use dialog QA" ....................................... 110
Figure 10-2 Global formatting ........................................................................................................ 111
Figure 10-3 Formatting of data columns ........................................................................................ 112
Figure 10-4 Configuration of synchronous booking ....................................................................... 113
Figure 10-5 Configuration of the rack comparison with the A+W Rack Manager ......................... 113
Figure 10-6 - Keyboard scanner parameters ................................................................................. 114
Figure 10-7 - Scanner ID ................................................................................................................. 115
Figure 10-8 Furnace bed ................................................................................................................ 119
Figure 10-9 Action for the foil preview .......................................................................................... 124
Figure 10-10 SQL expression for the foil preview .......................................................................... 124
Figure 10-11 Parameter Administrator with parameter "Automatic Batch Creation" .................. 125
Figure 10-12 Configuration for provision of PMO data................................................................. 126
Figure 10-13 Configuration for transfer of PMO data via XML file ............................................... 127
Figure 10-14 Parameters for quality scanner................................................................................. 127
Figure 10-15 Parameters for quality scanner................................................................................. 130
Figure 10-16 Parameters for individual lite booking...................................................................... 131
Figure 10-17 Parameter Administrator with dialog selection for racks that can be called up ...... 132
Figure 10-18 Select lot types .......................................................................................................... 133
Figure 10-19 Parameter Administrator for the filter possibility by cutting tables......................... 133
Figure 10-20 Configuration of tables for filter selection ................................................................ 134
Figure 10-21 Designer with new action button [Racks that can be called up] .............................. 135
Figure 10-22 selection of a fine planning rack ............................................................................... 136
Figure 10-23 Dialog for loading a lot ............................................................................................ 136
Figure 10-24 SN driver call ............................................................................................................ 137
Figure 13-1 Multisite infrastructure ............................................................................................... 146
Figure 13-2 Infrastructure configuration sites ............................................................................... 147
Figure 13-3 Infrastructure site assignment .................................................................................... 147
Figure 13:4 Infrastructure configuration........................................................................................ 148
Figure 13-5 Infrastructure A+W Production configuration ............................................................ 148
Figure 13-6 Infrastructure A+W Production configuration basic settings ..................................... 148

A+W Software GmbH                                 EN-CONFIG-A+W Production.docx                                                         182
Figure 13-7 Infrastructure A+W Production configuration database connection ......................... 149
Figure 13-8 Infrastructure A+W Production configuration PPS WebService URL .......................... 149
Figure 13-9 Infrastructure A+W Production configuration Service Monitor ................................. 149
Figure 13-10 A+W Production MultiSite CONFIG Tool ................................................................... 150
Figure 13-11 A+W Production MultiSite CONFIG tool services...................................................... 151
Figure 13-12 A+W Production MultiSite CONFIG tool services...................................................... 151
Figure 13-13 Services according to A+W Production MultiSite CONFIG tool ................................ 152
Figure 13-14 A+W Production site selection .................................................................................. 152
Figure 13-15 A+W Production Terminal selection of PPSWebService ........................................... 153
Figure 14-1 Archiving a batch in A+W Production ......................................................................... 155
Figure 14-2 Archiving or deleting configuration batches ............................................................... 155
Figure 14-3 Configuration of DSN for archive database ................................................................ 156
Figure 14-4 Configuration deletion of files during archiving ......................................................... 156
Figure 14-5 Configuration of deletion delay .................................................................................. 160
Figure 15-1 Infrastructure Web start page .................................................................................... 163
Figure 15-2 Configuration of the gateway connection settings ..................................................... 164
Figure 15-3 Activating the PDC data transfer to the gateway service ........................................... 164
Figure 16-1 Parameter Administrator: Creating a new station...................................................... 167
Figure 16-2 Parameter Administrator: Transferring a new station ............................................... 168
Figure 16-3 Management of document links ................................................................................. 168
Figure 16-4 Print document links on release ................................................................................. 169
Figure 16-5 Document links in A+W Production Terminal ............................................................. 169
Figure 16-6 Switch filter document links in A+W Production Terminal ......................................... 169
Figure 16-7 File attachment in A+W Business ................................................................................ 170
Figure 16-8 Configuration directory for file attachment in A+W Business .................................... 170
Figure 16-9 Directory for file attachment in A+W Business ........................................................... 170
Figure 16-10 Types for file attachment in A+W Business .............................................................. 171
Figure 16-11 Configuration transfer file attachment from A+W Business .................................... 171
Figure 16-12 File attachment in item entry in A+W Business ........................................................ 172
Figure 16-13 File attachment in document view in A+W Business ............................................... 172
Figure 17-1 Production Monitor .................................................................................................... 174
Figure 17-2 Tooltip display in Production Monitor ........................................................................ 175
Figure 17-3 Display of backlogs ...................................................................................................... 175
Figure 17-4 Utilization of a shift ..................................................................................................... 177
Figure 17-5 Display in the Production Monitor.............................................................................. 178
Figure 17-6 Batch overview............................................................................................................ 179
Figure 17-7 Program message ........................................................................................................ 179




A+W Software GmbH                                 EN-CONFIG-A+W Production.docx                                                       183

