---
title: "EN_UM_AWProduction_1"
source: "EN_UM_AWProduction_1.pdf"
tags: ["A+W Production", "Software Manual", "Glass Manufacturing", "Window Production", "Door Production", "Production Planning", "Scheduling", "Optimization", "Barcode Management", "ERP Integration"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is the official user manual for A+W Production, a comprehensive software solution designed for the glass, windows, and doors manufacturing industry. It provides a detailed guide on using the software for production planning, scheduling, optimization, and control."
long_description: "The A+W Production Manual is an in-depth technical document intended for end-users of the A+W software suite. It covers the full scope of the A+W Production module, a powerful production planning and control system. The manual is structured to guide users from a general overview to specific, advanced functionalities. It begins with an editorial section outlining documentation conventions, copyrights, and notes. A detailed table of contents provides a roadmap to the various modules, including Rough Scheduling, Detailed Scheduling, Capacity Planning, Machinery Allocation, Barcoding, Realtime Optimization, and Production Terminals. The manual features a tutorial section that introduces the basic system and its supplements, explaining core concepts like the process flow from ERP order entry to production planning. It details various user interface 'views' (e.g., order view, bucket view, batch view) and explains how to perform critical tasks like batch creation, scheduling, and optimization. The document also covers supplementary modules for capacity planning, various optimization systems (Realtime, Sequence, Shape, Rack, Furnace), barcode management, and display systems. It serves as a complete reference for configuring, operating, and mastering the A+W Production software to achieve efficient and transparent manufacturing processes."
---

# A+W Production
## Manual
**Software for Glass, Windows & Doors**

English

---

## Editorial

### Revision overview of the documentation
| Date | Change |
| :--- | :--- |
| 10-2024 | Update of complete manual for PDF and HTML5 format. |

### Notes
This document is intended only for end users of A+W Production.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of A+W Production.

### Copyrights
© 2024, A+W Software GmbH all rights reserved, also those for reprinting, the making of copies and translation.

The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

---

### Display conventions
Individual elements of the sentences are displayed in a special form. The meanings are:

| Term | Description |
| :--- | :--- |
| *Italics* | marks character strings describing the software elements, e.g. the *Buckets* dialog. |
| **Bold** | marks character strings to be entered via keyboard, e.g.: Enter **0**. |
| > | shows the way to open a dialog, e.g. Display > Filler orders > Context menu - List > Order overview. |
| [] | square brackets mark the buttons in the dialog, e. g. [OK] to save the data. |
| < > | pointed brackets refer to keys or shortcuts on the keyboard, e. g. <F1> is used to open the online help. |

### Contact
**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Deutschland

**Tel.:** +49 641 96620 0
**E-Mail:** info@a-w.com
**Web:** http://www.a-w.com

---

# Contents

## Overview (A)
- **Tutorial** A-19
- **Overview** A-22
  - Tutorial Structure A-22
  - The product range of A+W Software GmbH A-24
  - A+W Production introduces itself A-25
- **Basic Module A+W Production** A-27
  - Scheduling A-28
    - Scheduling in General A-29
  - Rough Scheduling A-31
    - Rough Scheduling in General A-32
    - The order view (pool) A-32
    - The order list A-34
    - The bucket view A-34
    - The item view A-35
    - The glass type view A-35
    - The detailed view A-36
    - The processing view A-36
    - The filler order view A-37
    - The batch view A-37
  - Batch Creation A-38
    - Batch creation A-38
    - General rules A-39
  - Detailed Scheduling A-40
    - Detailed Scheduling in General A-41
    - The Process of Detailed Scheduling A-41
    - Grouping and Sorting A-43
  - Rack and Stack Logic A-44
    - Modes for A racks A-44
    - Modes for harp racks A-45
  - Optimization Modes A-46
    - Optimization mode XOPTS 6.2 - fixed sequence A-46
    - Optimization mode XOPTS 6.1 - keep customers together A-46
    - Optimization mode XOPTS 5.2 - standard A-47
    - Optimization mode XOPTS 5.1 - IG on harp racks or many A racks A-47
  - Organization Types A-49
    - Organization Type and Batch Type A-49
  - Machinery Allocation A-50
    - Elements of Machinery Allocation A-51
    - Machines and Machinery Allocation A-52
    - Work Processes and Machinery Allocation A-53
    - Allocation of work processes A-54
    - Processing Types and Machinery Allocation A-55
    - Processing Articles and Machinery Allocation A-55
- **Supplements A+W Production** A-56
  - Capacity Planning A-57
    - A+W Capacity Planner A-58
    - Production monitor A-59
    - Campaign editor A-60
    - Shift editor A-61
    - Graphics-oriented rescheduling A-62
  - Optimization systems A-63
    - Realtime Optimizer A-64
    - Cutting table optimizations A-65
    - Cutting table control A-65
    - Master data A-65
    - Sequence Optimizer A-66
    - Shape Optimizer A-67
    - Rack Optimizer A-68
    - DynOpt A-69
    - Furnace Optimizer A-70
  - Barcode Manager A-71
    - General A-72
    - Scanners A-72
  - Display Systems and Control Units A-74
  - Production Terminal A-75
    - Manual Cutting A-75
    - Order A-76
    - Processing A-77
    - IG-In A-78
    - IG-Assembly A-79
    - IG-Out A-80
    - TG-In A-81
    - TG-Out A-82
    - The aim of the Production Terminals A-82
  - Statistics Modules A-83
    - A+W Discovery A-84
    - Production Cockpit A-85
- **Conventions** A-87
  - User Interface A-89
    - Dialogs A-89
    - Buttons A-90
  - Documentation A-94
    - Structure of the manual A-94
  - Online help A-96
    - Help A-96
    - Contents tab A-97
    - Index tab A-98
    - Find tab A-99
    - Help text not found A-99

## Rough Scheduling (C)
- **Tutorial** C-103
- **Overview** C-105
  - Tutorial structure C-105
- **Rough Scheduling** C-107
  - Production Scheduling Process C-108
- **Views** C-111
  - Views in Rough Scheduling C-112
  - Configure views, work with views C-115
    - Create and configure tabs C-115
    - Create and configure columns C-117
    - Create and configure totals row C-119
    - Define new column or totals row C-121
    - Create and configure filters C-124
    - White screen in a view C-127
  - Exercises: Configure views, work with views C-128
- **Orders / Pool** C-129
  - Orders in Rough Scheduling C-130
- **Buckets** C-132
  - Buckets in Rough Scheduling C-133
- **Batches and Batch Strategies** C-138
  - Batches in Rough Scheduling C-139
- **Items** C-145
  - Items in Rough Scheduling C-146
  - Search for document C-148
- **Software Reference** C-149
- **Rough Scheduling** C-152
  - Orders in Rough Scheduling C-153
    - Orders C-154
    - Order Overview C-157
    - Filler Orders C-160
    - Surplus Editor C-163
    - Change of Procurement Type C-165
  - Buckets in Rough Scheduling C-167
    - Buckets C-168
    - Reservation Orders Bucket C-171
    - Purchase Parts Bucket C-175
    - Bucket Creation C-178
    - Edit bucket description C-180
  - Batches in Rough Scheduling C-181
    - Batches C-182
    - Batch creation C-185
    - Create Special Glass Batch C-187
    - Edit Batch Description C-188
    - Release of Batch (Name): AUW – Repetition C-189
  - Items in Rough Scheduling C-192
    - Items C-193
    - Add Order to Items C-196
    - Split Items C-197
    - Field Definition C-199
    - Export/Import Item View C-201
  - Processings in Rough Scheduling C-202
    - Processings C-203
    - Change Default Times C-206
  - Glass types, Details, Barcoding and Lots C-207
    - Glass Types C-208
    - Details C-211
    - Barcoding C-215
    - Lots C-219
  - Overlapping Dialogs C-222
    - Work Plan C-223
    - Properties of (tab) C-226
    - Column Definition C-227
    - (Filter Name) C-228
    - Filter Definition C-229
    - Links to Documents C-231
    - Edge Deletion C-232
  - Overlapping Context Menus C-234
- **Help Cards** C-239
  - Information about the help cards C-241
- **Batches** C-242
  - Batch creation C-243
  - Add batches C-244
  - Combine batches C-245
  - Resolve batches C-246
  - Remove orders from batches C-247
  - Archive or delete batches C-248
- **Views** C-249
  - Add column or total row C-250

## Detailed Scheduling (D)
- **Tutorial** D-253
  - Notes on the Documentation D-256
    - Important Notes D-256
    - Tutorial Structure D-257
  - Detailed Scheduling - Overview D-258
    - The Process of A+W Production D-259
    - Terms of A+W Production D-261
      - Lot Type D-261
      - Lots D-262
      - Application lot D-262
      - Production lot D-262
      - Racks (storage locations) D-262
      - Application rack D-262
      - Production rack D-263
    - Batches D-263
      - Archiving batches D-263
      - Archiving method D-265
    - Element Tree D-268
    - Organization D-269
  - Grouping and Sorting D-270
    - Overview D-271
    - Introduction D-272
    - Grouping D-273
    - Sorting D-274
    - Additional Sorting D-277
    - Special Elements D-278
      - Filler Orders D-278
      - Residue Lites D-279
      - Rejects D-280
      - Rush Orders Lites D-281
    - Demos and Exercises D-282
  - Racks and Stacking Modes D-284
    - Overview D-285
    - Storage Locations D-286
    - Logical Racks D-286
    - Stacking Rules D-287
    - Predefined Stacking Modes for A Racks D-289
      - Glass Mode D-289
      - Unit Mode D-290
      - Production Mode D-292
      - VABGLA mode D-294
    - Robot Racks D-295
    - Modes for Harp Racks D-295
    - Modes for Fixed Racks D-295
    - Standard Settings in the Configuration D-296
    - Rack Settings in Master Data D-297
    - Demos and Exercises D-300
  - Optimization Modes D-303
    - Overview D-304
    - Different Optimization Modes D-305
      - Optimization Mode 6.2 - Fixed Sequence D-305
      - Optimization Mode 6.1 - Keep Customers Together D-306
      - Optimization Mode 5.2 - Standard D-308
      - Optimization Mode 5.1 - IG on Harp Racks or Many A Racks D-310
      - Optimization Mode Free Optimization - Lites on Harp Racks D-311
    - Double Optimization D-312
    - Demos and Exercises D-314
  - Organizations D-316
    - Organization Types D-317
      - General D-318
      - Tree Structure D-318
      - Master organization D-319
      - Reject Organization D-324
    - Sequence of Checks D-324
    - Organization Type and Lot Type D-327
    - Application and Production Organizations D-327
    - Global Settings D-327
    - Demos and Exercises D-329
    - Production Sequence D-330
      - General D-331
      - Grouping Key for Organization Groups D-331
      - No grouping D-331
      - Including Grouping D-332
  - A+W Standard Organizations D-333
    - Rack Organization D-334
      - A Racks AIR D-334
      - IG A racks D-342
      - A Racks Dispatch D-348
      - Harp Racks, no filling up D-353
      - Filled harp racks D-358
    - Demos and Exercises D-363
- **Software Reference** D-365
  - Overview D-367
  - Organizations D-369
    - Master Organization Tab D-369
    - Production Sequence Tab D-371
    - Test Sequence Tab D-372
  - Master Organization D-375
  - Organization D-379
  - Organization Groups D-381
  - Workstation Settings D-383
  - Default Settings D-387
  - Grouping and Sorting D-388
    - Grouping/Sorting Dialog D-388
    - Editor - Grouping Tab D-389
    - Editor - Sorting Tab D-391
    - Additional Sorting Tab D-392
    - Defining an Additional Sorting D-393
  - Racks D-394
    - Racks D-394
    - Lots D-399
    - Lot Types and Processings D-399
      - Lot Types Tab D-399
      - Processings Tab D-401
      - Implicit Processing Tab D-404
  - Detailed Scheduling of Batches D-406
    - Detailed Scheduling for Batch... D-406
    - Glass Types Tab D-407
    - Rack Load Tab D-410
    - Results Tab D-415
    - Specials Tab D-417
      - Nested Shapes Tab D-417
      - Filler Orders Tab D-419
      - Residue Plates Tab D-421
      - Rejects Tab D-422
      - Rush orders tab D-424
      - Thickness Tab D-425
      - Free Optimization Tab D-427
      - Partial Quantities Tab D-428
      - Organization Tab D-430
      - Organization Options Tab D-432
      - Options Tab D-434
      - Stockplate Selection Tab D-436
      - Change minimum number of A racks D-437
      - Sequence of Tables D-438

## Capacity Planning (E)
- **Tutorial** E-441
- **Overview** E-444
  - Tutorial Structure E-445
- **Basic Principles** E-446
  - Date optimization E-447
  - Scheduling E-448
  - Planning and Scheduling E-453
  - Production Monitor E-454
    - Daily adjustments of the work shifts E-456
    - Setting up Production Monitor E-463
  - Export Work Plan E-466
  - Scheduling and Rescheduling E-467
    - Scheduling of Orders E-468
    - Rescheduling E-469
    - Rescheduling Processings E-471
    - Incorrect Scheduling E-473
  - Post-Processing of Scheduled Orders E-474
  - Campaign Planning E-476
    - Definition of the campaigns E-477
    - Campaigns in scheduling E-479
    - Definition and Management of Campaigns E-479
    - Exercises on Campaigns E-485
  - Reservations E-486
    - Reservation of capacities E-487
    - Definition and Management of Reservations E-488
    - Exercises on Reservations E-494
  - Creating Processings E-495
    - Creation of Processings for Scheduling E-496
    - Creation of Processings E-497
  - Master Data of Capacity Planning E-500
  - Shifts E-501
    - Shift plans E-502
    - Definition of non-working days E-504
    - Create a Shift Plan E-507
    - Defining a Shift Rule E-510
    - Creating a Shift Group E-515
    - Exercises E-519
  - Cost Calculation E-520
    - Definition of the cost calculation E-521
    - Definition and Management of Costs E-522
    - Exercises E-524
  - Transition Times E-525
    - Transition times in shifts or hours E-527
    - Definition of transition times E-531
    - Definition and Management of Transition Times E-534
    - Exercises E-537
  - Default Times E-538
    - Definition of the default times E-539
    - Structure of default time formulas E-540
    - Calculation of time surcharges E-543
    - Editor for formula elements E-545
    - Example - default time for the logical machine cutting E-546
    - Time formula objects E-549
    - Definition and Management of Default Time Formulas E-550
    - Testing time formulas E-556
    - Exercises E-562
  - Machinery Groups E-563
    - Definition of the machinery groups E-564
    - Definition and Management of Machinery Groups E-565
    - Exercises E-568
  - Load Distribution E-569
    - Definition of load distribution E-570
    - Definition and Editing of Load Distribution E-571
    - Exercises E-574
- **Software Reference** E-575
  - Overview E-578
  - Scheduling E-579
    - Production Monitor E-580
    - Displayed Machines E-584
    - Settings E-585
    - Please Select an Order/Batch (Filter) E-588
      - Filter - Orders E-588
      - Filter - Batches E-589
      - Filter - Individual Filters E-590
    - Create New Filter E-591
    - Machine (Name) E-592
    - Adjust Shifts for Machine E-594
    - Shift Properties E-595
    - Reservation Display E-597
    - Workplan from Production Monitor E-598
      - Work Plan - Details E-599
      - Work Plan - Overview E-601
    - Scheduling E-602
    - BOM Configuration E-603
    - Action E-604
    - Rescheduling E-605
    - Machine Reallocation E-610
    - Post-Processing Booking E-611
    - Defective Orders E-614
    - Asynchronous Processing E-615
    - Changes to Scheduled Orders E-616
    - Split Items E-617
  - Campaigns and Reservations E-619
    - Campaigns E-620
      - Campaigns - Individual Dates E-621
      - Campaigns - Weekly Dates E-623
      - Expired Reservations E-624
    - Reservations E-626
      - Reservation for Machine E-629
      - Select a Customer E-630
      - Select Project E-631
  - Processings E-632
    - Creation of Processings E-633
    - Add an Existing Condition E-636
  - Time Master Data E-637
    - Default Times E-638
    - Default Time Formula E-640
      - Add Elements E-644
      - Tabelle, Vector (Name) E-645
      - Input Help for Vectors E-646
      - Select Formula E-648
      - Entering a formula element E-649
      - User-defined Table Elements E-651
      - Select Limit E-652
    - Time Formula Test E-653
    - Formula Object Properties E-655
      - Formula (Name) E-657
    - Course of Formula Evaluation E-658
  - Transition Times E-659
  - Master Data for the Shifts E-662
    - Shifts E-663
      - Shift Calendar E-665
      - Shift Plan E-666
      - Shift Rule E-668
      - Shift Group E-670
    - Machine E-672
  - Machines and Costs E-674
    - Cost Calculation E-675
  - Machinery Groups E-677
  - Load Distribution E-679
- **Help Cards** E-681
  - Information regarding Help Cards E-683
  - Capacity Planning E-684
    - Create a Shift Plan E-685
    - Creating shift rules E-686
    - Create a shift group and assign E-687
    - Integrate new machine E-688
    - Move machine E-689
    - Create allowed times E-690
    - Defining cost records E-691
    - Change shift property flexibly E-692
    - Reschedule processing date E-693
    - Reschedule dispatch date E-694

## Formula Editor (F)
- **Tutorial** F-697
- **Formula Editor** F-699
  - Objective of the formula editor F-699
  - parts of the formula editor: Level I F-699
    - Formula F-700
    - Comparison F-701
    - Condition F-701
      - Linking of elementary conditions F-703
    - Quantity F-704
    - Allocation F-705
  - parts of the formula editor: Level II F-705
    - Formula F-705
    - Comparison F-706
    - Condition F-706
    - Quantity F-708
    - Allocation F-708
  - Elements of the formula editor: Step III F-709
    - Quantity F-709
  - Notation Formula.dll F-711
    - Syntax F-711
      - ASSIGNMENT F-711
      - FORMULA F-711
      - CONDITIONS F-711
      - CONDITION (comparison) F-711
      - SET F-712
      - Function F-712
      - ASSIGNMENT F-712
      - FORMULA F-713
      - CONDITIONS F-713
      - CONDITION F-713
      - SET F-714
  - Check results F-715
  - Conditions for Racks F-716
  - Conditions for Organization Groups F-718
    - Group Formation Mode F-721
  - Conditions for Production Sections F-723
  - More Examples F-726
  - List of Dialogs F-729
- **Software Reference** F-731
  - Formula Editor F-733
    - Select conditions F-734
    - Condition editor F-736
      - Condition F-739
      - Condition name F-741
      - Info F-742
      - Invert F-742
      - Transferred quantity F-743
      - Enter value (numeric) F-744
      - Select quantities F-746
      - Quantity editor F-748
      - Quantity name F-752
      - Info F-754
    - Select formulas I F-755
    - Formula editor F-757
    - Select allocation F-760
    - Allocation editor F-760

## Machinery Allocation (G)
- **Tutorial** G-765
- **Overview** G-767
  - Tutorial Structure G-767
- **Basics** G-768
  - Machine Allocation G-770
  - Machines G-771
    - Machines and Machine Allocation G-772
    - Machine Definition and Management G-778
    - Definition and Editing of Machine Restrictions G-782
    - Machines Exercises G-788
  - Logical Machines G-789
    - Machines and Machine Allocation G-790
    - Definition and Management of Logical Machines G-792
    - Logical Machines - Exercises G-796
  - Work Processes G-797
    - Work Processes and Machine Allocation G-798
    - Work Process Definition and Management G-804
    - Work Processes - Exercises G-807
  - Allocation of Work Processes G-808
    - Flexible Adaptation of Work Processes G-809
    - Allocation of Work Processes and Logical Machines G-814
    - Work Process Allocation - Exercises G-818
  - Conditions, Formulas, Restrictions G-819
    - Conditions and Formulas in Connection with Machine Allocation G-820
    - Select a Condition G-821
    - Select a Formula for the Processing Time of a Logical Machine G-822
    - Selection of Conditions - Exercises G-824
  - Processing Types and Processing Articles G-825
    - Processing Types and Machine Allocation G-826
    - Processing Articles and Machinery Allocation G-827
    - Definition and Management of Processing Types G-829
    - Definition and Management of Processing Articles G-832
  - Machine Allocation - Exercises G-836
  - Machine Allocation - Buttons G-837
- **Software Reference** G-839
  - Machinery Allocation G-841
    - MA Editor G-842
    - MA Editor - Machines G-843
    - MA Editor - Logical Machines G-845
    - MA Editor - Work Processes G-847
    - MA Editor - Work Process Allocation G-849
    - MA Editor - Machine Types G-851
      - New Machine G-853
      - Machine G-854
      - Size Restrictions G-859
      - Spacer Restrictions G-860
      - Select a Condition G-861
      - New Logical Machine G-863
      - Logical Machine G-864
      - Formula Selection G-866
      - New Work Process G-867
      - Work Process G-868
      - New Machine Type G-870
      - Machine Type G-871
    - Machine Allocation - Formulas G-873
      - Select Conditions G-874
      - Condition Editor (Graphic Version) G-876
      - New Condition G-878
      - Info (about the new condition) G-878
      - Select quantity G-879
      - Condition Editor (Text Version) G-880
      - Formula Editor G-882
    - Processings in Machine Allocation G-884
      - Processing Types G-885
      - Processing Articles G-887
    - Adjust Columns G-890
      - Column Definition G-891
- **Help Cards** G-893
  - Information about the help cards G-895
  - Machine Allocation (MA) G-896
    - Add new machine G-897
    - Add new machine G-898
    - New machine for Production Terminal G-899

## Barcoding (H)
- **Tutorial** H-903
- **Overview** H-906
  - Tutorial Structure H-907
- **Basic Ideas** H-908
  - Barcoding H-909
    - Purpose of AWP H-909
  - Booking Elements H-910
    - Products H-911
    - Basic information H-912
    - Direct objects H-912
    - Indirect objects H-912
    - Lites or Units H-912
    - Booking types H-913
  - Booking Places H-914
  - Registration Points H-915
  - Error rack H-916
  - Correct booking H-918
  - Managing Registration Points H-919
    - Truck registration point H-921
  - Storage locations H-922
  - Racks H-923
  - Boxes H-924
  - Managing Racks H-925
  - Personnel H-928
    - Employee H-929
    - Managing Employees H-930
  - Status H-932
    - Status values H-933
      - Unit/group H-933
      - Rack H-933
      - Registration Point H-933
      - Action barcode H-934
    - Managing Status Values H-935
  - Data Entry H-937
    - Scanner H-938
    - Scanner Types H-939
      - Online scanners H-939
      - Denso scanners (WLAN) H-939
      - Serial scanners H-940
      - Offline scanners H-940
    - The scanner configurations H-940
  - Barcodes H-941
  - Booking Examples H-942
    - Scanning Sequence H-943
    - Scanning Units H-945
    - Scanning in Dispatch H-947
    - Scanning Registration Points H-949
    - Truck Registration Point H-952
    - Exercises: H-953
      - Exercise 1: Loading an empty and a partly loaded truck H-953
    - Scanning Racks and/or Boxes H-955
    - Scanning the Status H-957
    - Correcting Erroneous Entries H-958
  - Production Terminals H-959
    - Production Terminals H-960
      - Introduction H-961
    - Breakage Management H-963
      - Overview H-964
      - Breakage Handling (Internal) H-965
  - Statistics, Reporting and Monitoring H-967
    - Overview H-968
    - Barcode Reporting H-969
      - Loading the Reports H-969
      - Examples of Standard Barcode Reports H-969
      - Unit list H-970
      - Order overview H-970
      - Order status H-971
      - Loading list H-971
      - Rack load per lite H-972
      - Rack load per item H-973
      - Booking history H-973
  - Monitoring: A+W Dashboard H-974
    - Overview H-975
  - Statistics: A+W Discovery H-977
    - Overview H-978
- **Software Reference** H-981
  - Overview H-983
  - Master Data H-984
    - Barcode options H-985
    - Barcode types H-986
    - Registration point types H-987
    - Registration points H-988
    - Racks H-992
    - Rack filter H-996
    - Status types H-997
    - Stati H-998
    - Employee H-1000
    - Column Assignment H-1002
      - Columns H-1003
    - Post-processing H-1004

## Packing Optimization (I)
- **Tutorial** I-1007
  - The Basic Idea I-1009
  - General I-1010
  - Master Data I-1013
    - Optimization rules (*.RUL file) I-1013
    - Settings (*.VAL file) I-1013
    - Parameter I-1014
  - Views I-1019
    - Packing group view I-1019
      - Restrictions I-1020
    - View Optimization I-1022
    - Views I-1023
      - 3D view I-1023
      - Top View I-1024
      - Detailed view I-1025
      - Side view (edge view) I-1030
    - Modes I-1032
      - Full screen mode I-1032
      - Editing mode I-1033
      - Checking the rack load I-1034
      - Fixed loading sequence I-1035
      - Expert mode I-1036
      - Free edit mode I-1037
      - Invalid placements I-1040
      - Minimal thickness differences I-1040
    - Clip list I-1042
- **Software Reference** I-1067
  - Menus I-1069
  - Rules I-1071
  - Values I-1073
  - Packing groups I-1076
  - Packing group view I-1079
    - Total line I-1080
    - Filter function I-1080
  - Hotkeys I-1080
  - Context menu for tagged entries I-1082
  - PackView I-1085
    - Menu line I-1086
    - Icons I-1090
    - Views I-1093
    - Change rack description I-1094
    - New rack properties I-1095
    - Change box properties I-1097
    - Unit properties I-1099
  - Info line at the bottom of the screen I-1100

## Realtime Optimizer (J)
- **Tutorial** J-1105
- **Basic Ideas** J-1108
  - Features J-1109
  - Using A+W Production J-1110
    - Overview J-1111
  - Import of data J-1112
    - Working with A+W Production J-1113
    - Master data J-1114
    - Use as a stand-alone system J-1114
    - Import optimizations J-1114
- **Input** J-1116
  - Overview J-1117
  - Rejects, rush order lites or filler orders J-1118
  - Manual entry of lites J-1119
  - Manual creation of plans J-1122
  - Charge editor J-1123
- **Optimization** J-1124
  - Overview J-1125
  - Cutting table optimizations J-1126
    - Create table optimizations J-1126
    - Check and process table optimization result J-1128
    - Resolve table optimization J-1129
    - Linking of table optimizations J-1131
  - Create a quick optimization J-1132
  - Linking of batches J-1133
  - Cutting table control J-1134
- **Cutting** J-1135
  - Overview J-1136
  - Selecting batches for cutting J-1137
  - Check optimization and cut J-1140
  - Interrupt and continue work J-1142
  - Cutting overview J-1143
  - Reset cutting status J-1145
- **Interplay with Other Modules** J-1146
  - Overview J-1147
  - A+W Residual Stock Manager J-1147
  - A+W Planning Web J-1147
    - Interface J-1148
    - Master data J-1148
  - A+W Pattern Viewer J-1156
    - Settings J-1156
    - The interface J-1157
    - The menu bar J-1157
    - Information about lite and waste J-1167
    - Display linked batches J-1167
    - Display setting edge J-1168
    - Display symbol for processings, stamp, logo or reference mark J-1168
    - Color selection for order items J-1169
    - Mark the first and last lite J-1169
    - Rejects J-1170
  - A+W PlanEditor J-1171
  - A+W Continuous Cutting J-1172
    - Overview of the planned batches J-1172
    - Grouping J-1175
      - Rush groups J-1176
    - Resetting batches J-1176
    - Cutting J-1176
  - A+W Defect Optimizer J-1178
  - A+W DynOpt Compact J-1179
    - A+W DynOpt Compact Import J-1179
    - A+W DynOpt Compact Optimization J-1179
    - Create A+W DynOpt Compact batch J-1180
- **Software Reference** J-1183
  - Overview J-1186
  - Menus J-1186
  - Icons J-1187
  - Entry J-1188
    - Rush order lites J-1189
    - Enter rush order lites J-1191
    - Shape input J-1193
    - Shape number J-1195
    - Manual creation of plans J-1196
    - Charge editor J-1199
  - Optimization J-1201
    - Select glass for optimization J-1202
    - Table optimization in the Default variant J-1202
    - Table optimization in the Production date variant J-1205
    - Local optimization job [no] J-1207
    - Overview J-1207
    - Optimize J-1210
    - Description of fields in section Optimization Sequence J-1210
    - Description of buttons in section Sequence J-1211
    - Description of fields in Automatic compilation section J-1211
    - Description of fields in section Batch parameters J-1211
    - Description of fields in section Table J-1212
    - Description of fields in section Optimization parameters J-1212
  - Residue plates and stockplates J-1212
    - Parameter J-1216
    - Number of stockplates J-1219
  - Resetting a cutting batch J-1220
  - Pausing glass types J-1222
  - Currently changed settings J-1224
  - Cutting J-1225
    - Select a batch J-1226
    - Batch [number] - batch [number] J-1230
    - Optimization sequence J-1232
    - Batch: Number J-1233
    - Select the Optimizations to be linked J-1237
    - Optimization result J-1238
  - Rejects pool J-1239
    - Add rejects J-1241
    - Search fields J-1242
  - Input of shapes J-1243
  - A+W DynOpt editor J-1244
    - Description of buttons J-1245
  - Settings J-1248
    - Settings J-1249
    - Table optimization J-1251
  - View J-1252
  - Import J-1253
  - Error reports J-1254
  - A+W Residual Stock Manager J-1255
  - A+W Planning Web J-1255
    - Stock J-1255
    - Rack information J-1257
    - Racks J-1259
    - Rack properties J-1261
    - Glass overview J-1263
    - Add/Edit new data record J-1266
- **Help Cards** J-1269
  - Information about the help cards J-1271
  - Input J-1272
    - Enter rush order lites J-1273
    - Enter rejects J-1274
    - Input of charges J-1275
  - Optimization J-1276
    - Selecting batches and glass types J-1277
    - Create table optimization J-1278
    - Selecting stockplates J-1279
    - Using residual lites J-1279
    - Adding filler orders J-1280
    - Resolve table optimization J-1281
    - Create a quick optimization J-1282
    - Linking an optimization J-1283
  - Cutting J-1284
    - Select batches J-1285
    - Cutting batches again J-1287
    - Skip pattern J-1288
    - Do not generate a cutting code J-1289
    - Interrupt cutting J-1290

## Production Terminals (L)
- **Tutorial** L-1293
- **Overview** L-1297
  - Tutorial Structure L-1297
- **Production Terminal Systems** L-1298
  - Goals of the Production Terminal Technique L-1300
  - Operation of the Production Terminals L-1300
- **Overview Production Terminal: IG** L-1301
  - Using Production Terminal IG-In L-1302
    - Module Presentation: Production Terminal IG-In L-1303
      - Detailed annotations on the individual sections L-1304
    - Operating Sequence L-1307
      - Loading a lot L-1309
      - Changing the machine status L-1310
      - Handling of defective lites L-1311
      - Loading another item number L-1312
      - Loading a remake L-1313
    - Additional functions L-1314
      - Creation of lists (reports) L-1314
      - Export of log entries L-1314
      - Choose program language L-1315
  - Using Production Terminal IG-Assembly L-1316
    - Module Presentation: Production Terminal IG-Assembly L-1317
      - Detailed annotations on the individual sections L-1318
    - Operating sequence L-1320
      - Register at the workstation L-1320
      - Changing the machine status L-1321
      - Handling of defective lites L-1321
      - Skipping a unit L-1321
    - Additional functions L-1321
  - Using Production Terminal IG-Out L-1323
    - Module presentation: Production Terminal IG-Out L-1324
      - Detailed annotations on the individual sections L-1325
    - Operating sequence L-1326
      - Register at the workstation L-1326
      - Input of batches L-1326
      - Changing the machine status L-1327
      - Handling of defective lites L-1327
  - Remake management L-1327
    - Procedure L-1328
- **Overview Production Terminal Manual Cutting** L-1331
  - The use of Production Terminal Manual Cutting L-1332
    - Module presentation: Production Terminal Manual Cutting L-1333
      - Detailed annotations on the individual sections L-1334
    - Release a batch L-1335
    - Using the rejects pool L-1337
    - Adding a lite to the rejects pool by hand L-1339
    - Operating sequence L-1340
      - Register at the workstation L-1340
      - Input of charges L-1341
      - Changing the machine status L-1342
      - Handling of defective lites L-1342
    - Additional functions L-1342
- **Overview Production Terminal Georgian Bars** L-1343
  - Using Production Terminal Georgian Bars L-1344
    - Module presentation Production Terminal Georgian Bars L-1345
      - Detailed annotations on the individual sections L-1346
    - Release a batch L-1347
    - Operating sequence L-1349
      - Register at the workstation L-1349
      - Input of charges L-1350
      - Changing the machine status L-1350
    - Additional functions L-1350
- **Overview Production Terminal: Order** L-1351
  - Using Production Terminal Order L-1352
    - Module presentation: Production Terminal Order L-1353
      - Detailed annotations on the individual sections L-1354
    - Operating sequence L-1357
      - Register at the workstation L-1357
      - Input of charges L-1358
      - Changing the machine status L-1358
      - Handling of defective lites L-1359
    - Additional functions L-1359
- **Overview Production Terminal: Processing** L-1360
  - Using Production Terminal Processing L-1361
    - Module Presentation: Production Terminal Processing L-1362
      - Detailed annotations on the individual sections L-1363
    - Operating sequence L-1366
      - Register at the workstation L-1366
      - Input of chargs L-1368
      - Changing the machine status L-1368
      - Handling of defective lites L-1368
    - Additional Functions L-1369
- **Overview Production Terminal: TG** L-1370
  - Using Production Terminal TG-In L-1371
    - Module Presentation: Production Terminal TG-In L-1372
      - Detailed annotations on the individual sections L-1373
      - Moving or turning lites on the furnace bed. L-1374
    - Operating sequence L-1375
      - Register at the workstation L-1375
      - Input of batches L-1377
      - Changing the machine status L-1377
      - Handling of defective lites L-1377
    - Additional functions L-1377
  - Overview: Production Terminal TG-Out L-1378
  - Using Production Terminal TG-Out L-1379
    - Module presentation: Production Terminal TG-Out L-1380
      - Detailed annotations on the individual sections L-1381
    - Operating sequence L-1383
      - Register at the workstation L-1383
      - Input of batches L-1384
      - Changing the machine status L-1384
      - Handling of defective lites L-1384
    - Additional functions L-1384
- **Overview Production Terminal LG** L-1385
  - Using Production Terminal LG-In L-1386
    - Module presentation Production Terminal LG-In L-1387
      - Detailed annotations on the individual sections L-1388
    - Operating Sequence L-1389
      - Register at the workstation L-1389
      - Loading a lot L-1390
      - Input of batches L-1390
      - Changing the machine status L-1391
      - Replacing damaged lites L-1391
    - Additional Functions L-1391
  - Using Production Terminal LG-Assembly L-1392
    - Module Presentation: Production Terminal IG-Assembly L-1393
      - Detailed annotations on the individual sections L-1394
    - Operating sequence L-1395
      - Register at the workstation L-1395
      - Input of batches L-1395
      - Changing the machine status L-1395
      - Handling of defective lites L-1395
    - Additional functions L-1396
- **Overview Production Terminal Edit** L-1397
  - Using Production Terminal Edit L-1398
    - Module presentation: Production Terminal Edit L-1399
      - Detailed annotations on the individual sections L-1400
    - Operating sequence L-1403
      - Register at the workstation L-1403
    - Additional functions L-1405
- **Software Reference** L-1407
  - Module Operation L-1410
    - Software terms L-1410
      - Buttons L-1410
      - Radio button L-1410
      - Combo box L-1410
      - Menu bar/Menu item L-1411
      - Key combinations L-1411
    - Closing the program L-1412
  - General Overview L-1413
    - Overview: Production Terminal IG L-1414
      - Registration L-1415
      - Go to production number L-1416
      - Preview L-1417
      - Batch L-1418
      - Load lot L-1419
      - Booking of rejects L-1421
      - Load remakes L-1423
      - Status L-1425
      - Remake management L-1426
      - Remake management - Edit L-1429
    - Overview: Production Terminal Manual Cutting L-1432
      - Release L-1433
      - Rejects pool L-1435
      - Breakage entry L-1437
    - Overview: Production Terminal Georgian Bars. L-1439
      - Release L-1440
    - Overview: Production Terminal Order L-1442
    - Overview: Production Terminal Proces-sing L-1443
      - Manual entry L-1444
    - Overview: Production Terminal TG L-1445
      - Manual entry L-1446
      - Open processing steps L-1447
    - Overview Production Terminal LG L-1449
      - Load order L-1450
      - Go to production number L-1452
    - Overview Production Terminal Edit L-1453
  - Reports L-1454
    - Parameter input for report L-1455
  - How to Use the Help Function L-1456
  - Log entries for this session L-1457
  - Language selection L-1458
  - About Production Terminal L-1459
- **Help Cards** L-1461
  - Information about the help cards L-1463
  - Terminal IG-IN L-1464
    - Procedure L-1465
    - Produce a lite L-1466
    - Change the machine status L-1467
    - Book damaged lites L-1468
    - Load production number L-1469
    - Book damaged lites L-1470
    - Load production number L-1471
    - Load remakes L-1472

## Index (Z)
(This section is an index and is best utilized in its searchable, digital format within the original help system.)

---

# A+W Production Overview

### Revision overview of the module
| Date | Change |
| :--- | :--- |
| 02-2017 | Screenshots updated. |
| 01-2017 | Product and company names adjusted. |
| 08-2013 | Complete revision of ALCIM documentation and adjustment to A+W Production. |
| 11-2012 | Updates. |
| 03-2003 | Original version. |

This module provides information on the following subjects:
- Tutorial
- Conventions

---

## Tutorial

### Overview

The training on A+W Production is aimed at producers of IG, toughened, and laminated glass as well as processors who want to get an overview of the performance and the processes of A+W Production.

This system overview shall give you a general idea of the performance and the possibilities of A+W Production. All subjects and modules will be treated in closer detail in separate training sessions and tutorials.

A thorough understanding of the system architecture and the modular structure of A+W Production are prerequisite for the handling and operation of the individual areas and the gathering of the necessary knowledge.

#### Sets of Topics
This tutorial offers the following sets of topics:
- A+W Production introduces itself
- Basic Module A+W Production
- Supplements A+W Production

> **Required knowledge**
> Basic knowledge of EDP or Windows are prerequisite for using A+W Production.

### Tutorial Structure
This tutorial consists of sets of topics with several sessions each. Each session consists of the following elements:

- **Overview**: Each training session starts with an overview of the major topics:
    - **Objectives**: What shall be conveyed?
    - **Benefit**: What can this knowledge be used for?
    - **Maxims**: Which correlations are to be remembered?
- **Concepts**: Concepts and terms of the corresponding training session will be explained first. This is followed by examples and operating instructions.
- **Exercises**: There are exercises featuring special tasks for some of the training sessions.
- **Cross-references**: At the end of each training session there is a section with cross references pointing out additional information in the software reference and in other sections. This shall help you to extend your new-found knowledge.

### Reading instructions
The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any learning units.

If you are already familiar with a subject you should at least read the summary at the start of the session in order to bring the main details to mind.

### The product range of A+W Software GmbH
This illustration shows A+W Production as a production planning and control system in interaction with the ERP system as part of the overall business process.

*(Fig. A-1 shows a diagram of the A+W Software GmbH product range, illustrating the integration of different systems.)*
- **Top-level systems**: ERP, PPS, Machine control, Machinery.
- **ERP Solution (A+W Enterprise, A+W Business)**: Manages Sales, Purchasing, Stock, Dispatch, Statistics, eCommerce.
- **PPS (Production Planning System - A+W Production)**: Handles Capacity planning, Production planning (Rough and detailed scheduling), and Cutting optimization.
- **Machine control (Control Units)**: Includes Production Terminal, Realtime Optimizer, Rack Optimizer, DynOpt, Monitoring, Controlling, and Barcoding.
- **Machinery**: Physical machines like Cutting line, IG Line, LAMI Line.
- **CAD construction**: A+W CAD Designer (Bars) (Shapes + Bars) is shown as an integrated component.

### A+W Production introduces itself
Ever-increasing production requirements call for more and more powerful control and scheduling systems. A+W Production is the production planning and control system of A+W Software GmbH. The modular architecture allows tailoring it to your requirements in an optimum way.

A+W Production offers a multitude of state-of-the-art methods and tools for planning, controlling, monitoring, and analyzing your entire production - from order entry up to NC code creation and the booking of barcode data. In addition to these standardized processes the system allows the direct and dynamic intervention into the production process, e.g. in order to add important, urgent orders or to remove bottlenecks. This gives you full control over all production-relevant resources and data at all times - machinery, costs, times, and capacities.

A high degree of quality is achieved by the networking of machinery and other A+W Software GmbH software modules and due to process visualization and control by means of production terminals at the individual workstations.

To handle the modular structure of A+W Production, the software has been divided into two categories:
- **Basic system**
- **Supplements**

The **basic system** consists of the sections:
- Scheduling
- Rough scheduling
- Detailed scheduling
- Machinery allocation

The following **extension modules** are available:
- Capacity planning
- Optimization systems (Realtime, Sequence, Shape, Rack, DynOpt, Furnace Optimizer)
- Barcode Manager
- Display systems and control units (Production Terminal)
- Statistics modules (A+W Discovery, Production Cockpit)

#### The Process Flow with A+W Production
*(Fig. A-2 shows the process flow. It starts with ERP Order Entry and CAD Designer input.)*
1.  **ERP Order Entry**: Orders are created.
2.  **CAD Designer**: Designs are created.
3.  **Order Check**: An automated check is performed. If there is an error, information is sent back to Order Entry and Order Analysis. If OK, it proceeds.
4.  **Order Analysis**: Orders are analyzed.
5.  **Production Planning**: Approved orders go into the "Order Pool". The pool contains multiple orders, each with items (e.g., Glass 1, Glass 2). These are then grouped for production.

---

## Basic Module A+W Production
This section shows you how to use the basic module, which includes:
- Scheduling
- Rough Scheduling
- Detailed Scheduling
- Machinery Allocation

### Scheduling
This section introduces the operation of the scheduling process in A+W Production.

**Objectives**
- Getting to know the operation of the scheduling module
- Knowing the modules, processes, and procedures involved.

**Benefit**
Only if you know and understand the operation will you be able to understand and adapt the following processes.

**Definitions**
- **Items4ALCIM**: Module name of the scheduling service. Is often used as a synonym.

> **Note: Service**
> Scheduling is a Windows service and can be run interactively. Actively, it is controlled by the user while interactively, it is run as a background process. Several scheduling processes can be run simultaneously.

#### Scheduling in General
The scheduling process (Windows service) saves the order data from the ERP system actively in the production database. There are two ways of transferring data:
- **Direct data import**: By accessing an A+W Enterprise database.
- **XML-based standard interface**: e.g. from A+W Business.

*(Fig. A-3 and A-4 illustrate the detailed interactions between A+W Enterprise/Business and A+W Production. They show various web services and windows services (e.g., Production Items4ALCIM, Booking Engine) exchanging data between the Enterprise/Business database and the Production database via an Import Directory or direct calls. Functions like `GetItemProcurementDate`, `SetOrderStatus`, and `CompleteScheduling` are passed between the systems.)*

During the scheduling process, the following steps are performed for every order item:
1.  What? - Master data
2.  Where? - Machinery allocation
3.  How long? - Capacity planning
4.  When? - Capacity planning
5.  SN file creation
6.  Filling of the so-called "pool_" tables
7.  Loading and performing customization
8.  Geometry calculation
9.  Barcode Initialization
10. Report to ERP system (via WebService)

The transferred orders can now be found in the so-called Pool view (first step in the rough scheduling process).

### Rough Scheduling
This subject area introduces the rough scheduling functions in A+W Production.

**Objectives**
- Getting to know the different views

**Benefit**
Understanding the aims and the use of rough scheduling is the basis of efficient batch creation and management.

**Definitions**
- **Rough scheduling**: The process and tools for efficient batch planning and management based on production-relevant factors.
- **Pool**: The view showing all unscheduled products and intermediate products after order scheduling.
- **Bucket**: A collection of pre-grouped products or individual items to get a general idea of quantities before batch creation.
- **Batch**: The result of rough scheduling; a group of rough-scheduled orders and items that can be released for production.
- **Released element**: Elements explicitly scheduled for production (e.g., lites to be cut).
- **Bill of material (BOM)**: A hierarchical list describing all element dependencies and processing steps.
- **Processing**: Work steps to be performed on a glass/product (e.g., Cutting, toughening, shipping).

#### Rough Scheduling in General
Rough scheduling provides an overall view of orders to be produced, allowing them to be grouped into suitable production batches. This is enabled by a quantity-based evaluation of orders and items through several configurable views.

*(A diagram shows the relationships between different views:)*
- **Pool view**: Shows all unscheduled orders/products.
- **Bucket view**: Shows all pre-grouped orders/products.
- **Batch view**: Shows all roughly scheduled orders/products.
- **Other views providing specific focuses**: Detailed view (special properties), Glass type view, Item view (BOM structure), Processing view (processing steps), Filler order view, Barcode view (status), Order list (whole BOM), and Production lot view (results of detailed scheduling).

By means of these views, orders can be flexibly created and changed any time before detailed scheduling begins.

#### The Views of Rough Scheduling

- **The order view (pool)**: Shows all unscheduled orders, allowing for delivery date-, route-, or customer-oriented planning. Unscheduled means they have not been assigned to a batch yet. Tabs can be used to organize the view, and filters can restrict it.
- **The order list**: Presents a clearly arranged image of the BOM structure and can be configured to show production dates for each BOM element.
- **The bucket view**: Lists existing buckets. Products can be grouped into buckets for pre-scheduling to get an idea of quantities.
- **The item view**: Shows order data for selection and is suitable for finding orders within a batch. It displays a structural view of one or more orders.
- **The glass type view**: Shows the individual sub-elements of a product, useful for arranging batches and buckets for cutting. It handles IG and cast resin combinations.
- **The detailed view**: Similar to the Order view but based on any selected quantity.
- **The processing view**: Gives an overview of the elements and their corresponding processing steps.
- **The filler order view**: Similar to the Order view but only shows orders marked as filler orders.
- **The batch view**: Gives an overview of existing batches and their status (roughly scheduled, scheduled in detail, being produced, etc.).

> **Configuration of views**
> The contents, sorting, filters, and adding up functions can be flexibly configured by means of a context menu - system-wide or user-related.

#### Batch Creation
Batches can be created in the Order, Batch, Filler order, Detailed, Processing, and Glass type views.

**Batch creation** criteria examples:
- **By glass type**: Thick, large, or expensive lites are often produced in separate batches.
- **By product type**: In complex productions, different glass types (IG, toughened) are often separated.
- **By processing step**: Steps with long lead times or high costs (e.g., screen printing) can be the basis for batch creation.
- **By production date**: Determined by capacity planning.
- **By order or item**: Allows for flexibility and late-stage changes, especially in complex productions.

**General rules for batches**:
- A batch should be of a suitable size (e.g., ~2 working hours).
- Special products should be mixed with standard batches where possible.
- The best batch creation strategy is the one that works for your specific purposes.

### Detailed Scheduling
This subject area introduces detailed scheduling.

**Objectives**
- Knowing the targets and general conditions of detailed scheduling.
- Knowing about the different optimization modes and organization types.

**Benefit**
Detailed scheduling helps adjust production with regard to sequence and cutting optimization, determining the best production sequence for batch contents.

**Definitions**
- **Groups**: Formed by characteristic properties like customer number or glass type.
- **Sorting**: Done by properties with a consecutive value within a group (e.g., glass thickness).
- **Physical rack**: An A rack, L rack, or fixed rack.
- **Logical rack**: A virtual stack of glass; several can exist on one physical rack.
- **Organization**: Production organization rules and filters for sequence and processes.

#### Detailed Scheduling in General
A product's path through the shop floor involves various processing steps. The available space and time influence detailed scheduling. For example, limited sorting space after cutting must be compensated by the sequence of lites.

*(A diagram illustrates the production flow: Stock sizes of different glass types are fed to a Cutting Table. Lites are then resorted and sent to a LAMI Line, IG Line, or another Cutting Table, before final resorting and shipping.)*

> **Optimization result**
> Optimizing for the lowest possible waste is not always the main target. An optimization that results in unreasonable sorting work before assembly might be counterproductive.

**The Process of Detailed Scheduling**
This is the second step of production scheduling, starting after rough scheduling is finished. Its task is to determine the production sequence for elements in batches to define racks (quantity and allocation). The sequence can be determined by:
- Customer's requirements (e.g., unloading sequence).
- Results of rack and packing optimization (Rack Optimizer).
- Production restrictions.

The process involves:
1.  Loading data from the database.
2.  Allocating elements to available organizations and rack types.
3.  Grouping and sorting within organization groups and on racks.
4.  Putting the lites onto racks.

*(A symbolic triangle diagram shows the trade-off between **Sequence**, **Waste**, and **Flexibility** in detailed scheduling settings.)*

#### Grouping and Sorting
Grouping and sorting allow the allocation of the required production sequence to individual racks. Optimization then calculates the best yield while adhering to this sequence. This is useful for matching lites of an IG or laminated glass unit.

*(A diagram shows lites "Grouped by glass type" (Float 4 mm, Float 6 mm, Float 8 mm) and then "Sorted by size" within each group.)*

#### Rack and Stack Logic
Detailed scheduling offers various criteria for putting lites onto racks. This allows for an efficient rack and stack logic that stays in control of production paths, improving cycle times and avoiding unnecessary resorting.

*(The symbolic triangle diagram of Sequence, Waste, and Flexibility is shown again.)*

A+W Production offers standard organizations for:
- Special A rack organizations
- Special harp rack organizations
- Units (IG, laminated glass)
- Multi-stepped production
- Lot-based production

**Modes for A racks**
A racks can be filled by four different methods:
- **Glass Mode**: One glass type per rack, with each stack having its own rack number.
- **Unit Mode**: Each unit is set onto a logical rack.
- **Production Mode**: Different glass types can be combined on one logical rack with several stacks.
- **VABGLA Mode**: One logical rack per glass type, with one stack each.

**Modes for harp racks**
- **Together**: Lite and counterpane(s) are always put together on a harp rack.
- **Glass**: Lites are always stacked separately.

#### Optimization Modes
A compromise must be found between the best optimization result (low waste) and the best production sequence. The following modes can be set:

- **XOPTS 6.2 - fixed sequence**: Uses a rigid sequence of groups and lites as released for optimization. This prioritizes **Sequence** over Waste and Flexibility.
- **XOPTS 6.1 - keep customers together**: The sequence of lites within groups is fixed (e.g., by size), but groups can be rearranged to improve the result (e.g., grouping by Route/Customer). This balances **Sequence** and **Result**.
- **XOPTS 5.2 - standard**: The standard mode. Grouping/sorting key only includes the group number. Elements within groups have no fixed sequence and can be optimized freely. This prioritizes **Result** over Sequence.
- **XOPTS 5.1 - IG on harp racks or many A racks**: Lites are optimized at random, but units (e.g., IG units) are kept together.
- **XOPT - lites on harp racks**: Standard optimization for lites on harp racks.

#### Organization Types
Organizations are sets of rules for handling production, enabling efficient batch planning. Depending on the company's structure, multiple organizations can be defined (e.g., toughened glass org, IG org).

**Organization Type and Batch Type**
Each element has an element/processing type (e.g., basic glass, cutting) and a supply type (e.g., ordered). These properties determine the batch type. Additionally, each organization has an organization type that defines which elements it can handle, based on filters for similarities and differences (e.g., Shapes vs. Rectangles, Height, Weight).

### Machinery Allocation
This session introduces the subject of machinery allocation.

**Benefit**
Machines represent the physical machinery and are the basis for production control.

**Definitions**
- **Machinery**: Represents the physical machinery.
- **Logical machine**: A technological description of a machine's operating status or part (e.g., a furnace can be logical machine 'Toughening' or 'Annealing').
- **Machine types**: Predefined types like 'Cutting', 'Spacer bender'.
- **Work processes**: Connect processing types (e.g., 'Cutting') with workpiece properties.
- **Processing types/articles**: Describe the technical type of processing in more or less detail.

*(A diagram shows the linking of software elements for Machinery Allocation:)*
- **Machine** (e.g., Cutting table 8) is defined by a **Machine type** (e.g., Cutting), **Properties** (e.g., registration point 180), and **Restrictions** (e.g., min thickness 2mm).
- The machine is linked to a **Logical machine** (e.g., logical cutting table 8), which can have **Formulas** (e.g., Is a shape).
- A **Process** (e.g., IG cutting) is defined by a **Processing type** (e.g., Cutting) or **Processing article** (e.g., Float cutting).
- The **Allocation of work** links the Logical machine and the Process, and A+W Production then issues the machine code.

#### Machines and Machinery Allocation
The `Machines` tab lists all physical machines. Each machine is allocated a machine type (e.g., cutting, CNC centre).

#### Work Processes and Machinery Allocation
A work process is defined by a processing type, article, group, and/or an additional condition. This describes the technical type of processing. For example, `Shape cutting for laminated glass` can be a specific work process.

#### Allocation of work processes
Logical machines are allocated to work processes, defining the priority of machines for each process. This ensures work is performed by the most cost-effective machine. For example, a `Rectangular grinding` work process is prioritized for a simple Rectangular grinder, while a `Shape grinding` process is sent to the more versatile (and expensive) CNC centre.

#### Processing Types and Processing Articles
- **Processing Type**: Describes the general technical type of processing (e.g., Grinding).
- **Processing Article**: Describes a processing type in more detail (e.g., Bevelling, Mitres, Rounded corners for the Grinding type).

---

## Supplements A+W Production
This subject area introduces the extensions and supplementary modules of A+W Production:
- Capacity Planning (A+W Capacity Planner)
- Optimization systems (Realtime, Sequence, Shape, Rack, DynOpt, Furnace Optimizer)
- Barcode Manager
- Display Systems and Control Units (Production Terminal)
- Statistics Modules (A+W Discovery, Production Cockpit)

### Capacity Planning
Capacity planning allows providing customers with quick information regarding possibilities, capacities, and costs.

**Definitions**
- **Transition times**: Required rest time for glass between work processes (e.g., 8 hours for autoclave).
- **Capacity**: Time a machine is available for production.
- **Use of capacity**: Time span for which work has been scheduled.
- **Reservation**: Time reserved for special orders or customers.
- **Campaign**: Time span in a shift where a machine performs only one type of work process.

#### A+W Capacity Planner
This module schedules existing production capacities, balancing them against reserved capacities. It detects bottlenecks early and checks the desired delivery date. All information (delivery date confirmation, costs, etc.) is reported to the ERP system. It uses master data like shift plans, costs, and transition times.

- **Production monitor**: Provides a detailed capacity overview. It uses colors and icons to show backlog, shift status, capacity usage, overloads, work progress, and reservations.
- **Campaign editor**: Used for scheduling selected work processes on defined shifts or days.
- **Shift editor**: Used for defining and configuring shifts, shift rules, and shift groups.
- **Graphics-oriented rescheduling**: Allows reallocating processing steps to alternative machines and shifts.

### Optimization systems
These systems optimize processes and yield at different points in production.

**Definitions**
- **A+W Realtime Optimizer**: Online cutting control station for manipulating batches after optimization.
- **A+W Sequence Optimizer**: Optimizes waste of individual glass types, respecting the sorting sequence.
- **A+W Shape Optimizer**: Nests shapes from different items within a rectangle to save space.
- **A+W Rack Optimizer**: Optimizes the loading of lites onto transport racks based on weight, load, and sequence.
- **A+W DynOpt**: Dynamic optimization and cutting control for systems like HEGLA SortJet, achieving optimum yield while keeping a defined sequence.
- **A+W Furnace Optimizer**: Determines the optimal furnace bed load based on defined conditions.

### Barcode Manager
A+W Barcode Manager allows tracing individual lites and complex units by processing step, becoming a key planning and control instrument on the shop floor.

**Definitions**
- **Units**: Lites/units can be traced everywhere via their labels.
- **Racks**: Labels on racks allow tracking of their contents.
- **Registration points**: Places on the shop floor where lites/units are scanned/registered.

#### General
The system registers the production flow at essential registration points. Breakage registration is essential, and remakes can be created automatically.

#### Scanners
- **Online scanners**: Transfer scanned data directly to the system (no memory).
- **Offline scanners**: Have memory to save data temporarily (e.g., hand-held scanners).

### Display Systems and Control Units
These systems visualize production data and control the production process at individual terminals.

**Definitions**
- **A+W Production Terminals**: Control system for visualizing and controlling work on the shop floor.
- **A+W Production Cockpit**: Online monitoring and controlling system that visualizes up-to-date production data.

#### Production Terminal
Production Terminals are interactive display and control systems that visualize work schedules and allow for interactive intervention. Different types of terminals are available for different workstations:

- **Manual Cutting**: Visualizes the work schedule for the manual cutting table.
- **Order**: Used where large quantities are booked; an ideal tool for order- or batch-based processing.
- **Processing**: Used at automated processing machinery, providing true-to-scale production sketches.
- **IG-In**: Visualizes the work on hand at the IG line entry for a selected batch or rack.
- **IG-Assembly**: Installed at the IG assembly station, visualizing technical and spacer data.
- **IG-Out**: At the IG line exit, visualizes technical and dispatch-related data for each unit.
- **TG-In**: At the furnace entry, shows the furnace bed load, which can be interactively loaded.
- **TG-Out**: At the furnace exit, displays all registered lites based on the clock rate.
- **The aim of the Production Terminals**: To distribute scheduled jobs, book work performed, register deviations, visualize processes, create remakes automatically, provide workers with all relevant information, and enable manual re-optimization.

### Statistics Modules
These modules optically process extensive, heterogeneous data.

**Definitions**
- **OLAP**: Online Analytical Processing, used for analyzing complex business data.
- **A+W Discovery**: Modern, easy-to-use Business Intelligence System. The analysis surface is Microsoft Excel (Version 2010+). It allows evaluating and analyzing sales, complaints, breakage, and machinery times.
- **A+W Production Cockpit**: Online production benchmarking. It shows the actual degree of utilization, machinery status, productivity, and other parameters in real-time.

---

## Conventions

### User Interface
This chapter explains the control elements of the software.

#### Dialogs
The following terms describe software elements in dialogs:

| Term | Description |
| :--- | :--- |
| **Tab** | Splits dialogs into different subjects for clarity. |
| **Button** | A clickable control to perform a function. (e.g., [OK], [Cancel]). |
| **Hot key** | A key combination (e.g., <Alt> + underlined letter) to release a function. |
| **Radio button** | Allows selecting only one option at a time from a group. |
| **Combo box** | A drop-down list showing available options. |
| **Checkbox** | Offers an option that can be enabled or disabled. |
| **Field** | An input area for data. |
| **Header** | The title bar of a window or section. |
| **Menu bar/menu item** | The main menu at the top of a window. |
| **Tool bar** | A bar with icon buttons for quick access to functions. |
| **Open dialog** | A button that opens a new dialog. |
| **Table/column header**| The header row of a data table. |

#### Buttons
This chapter describes general A+W Production buttons.

| Button | Description |
| :--- | :--- |
| **...** | Opens a dialog related to the preceding field. |
| **Cancel** | Closes the dialog without saving changes. |
| **Change** | Edits the tagged record. |
| **Refresh** | Updates the contents of the open dialog. |
| **Barcoding View** | Opens the Barcoding view dialog. |
| **Data import** | Starts the import of data into A+W Production. |
| **Print** | Opens a dialog for printer settings and to release a printout. |
| **Insert** | Inserts a copied record. |
| **Field help (?)** | (Function has yet to be implemented). |
| **Filter** | Defines new filters in the views. |
| **Copy** | Copies the tagged record to a temporary memory for insertion elsewhere. |
| **Batch view** | Opens the Batch view dialog. |
| **Delete** | Deletes the tagged record, sometimes with a security check. |
| **Manual post-processing** | Opens the Manual post-processing dialog. |
| **New** | Enters a new record. |
| **OK** | Confirms entries, saves changes, and closes the dialog. |
| **Help (?)** | Opens the online help for the current context. |
| **Packing group view** | Opens the Packaging group view dialog. |
| **Pool view** | Opens the Pool view dialog. |
| **Close** | Closes the dialog. |
| **Save** | Saves entries in the database. |
| **Find** | Opens the Find dialog to search for records. |
| **Bucket view** | Opens the Bucket view dialog. |
| **Reject** | Rejects entries without saving. No security check. |

### Documentation

#### Structure of the manual
The documentation is split into sections (A-Z). The following table shows the sections that form this document:

| Section | Content |
| :--- | :--- |
| **A Overview** | Shows the structure of the user manual and explains software terms and buttons. |
| **C Rough Scheduling**| Explains settings and execution of Rough Scheduling. |
| **D Detailed Scheduling**| Deals with the necessary settings for production. A complex section. |
| **E Capacity Planning** | Explains how Capacity Planning works, its settings, and procedure. |
| **F Formula Editor** | Explains how to use the formula editor to create conditions for routing products. |
| **G Machinery Allocation**| Explains how machinery allocation works, its settings, and procedure. |
| **H Barcoding** | Gives an idea of Barcoding (BDE) and a basic understanding of the subject. |
| **I Packing Optimization** | Explains how Packaging Optimization works, its settings, and procedure. |
| **J Realtime Optimizer**| Describes how to use A+W Realtime Optimizer to save on stockplates and control cutting tables. |
| **L Production Terminals**| Tells you how to use control stations to optimize and make production processes more transparent. |

#### Online help
The A+W Production online help can be opened in different ways:
- Help menu
- [Help] button
- <F1> key

The online help opens context-sensitively to the dialog you currently have open. If no topic is current, the start page appears.

- **Contents tab**: Shows modules/catalogs as books. You can navigate to a topic.
- **Index tab**: Used to search for main subjects. Enter the first letter of the word.
- **Find tab**: Searches the entire online help for a term. Use this if Contents or Index is unsuccessful.

**Help text not found**
If a help text cannot be called up directly, use the search functions (Contents, Index, Find) in the online help. For some dialogs, there is no help text.
