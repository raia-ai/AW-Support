---
title: "EN FUNC A+W Continuous Cutting"
category: "functional_descriptions"
product: "A+W Continuous Cutting"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Continuous Cutting"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Continuous Cutting                                   english 1. Contents 1.         Contents                                                       3 2.         Notes on this Document                                         4   2.1.     Trademarks                                                     4   2.2.     Copyrights                                                     4   2.3.     Exclusion of liability                                         4 3."
source_file: "EN-FUNC-A+W Continuous Cutting.pdf"
---


# EN FUNC A+W Continuous Cutting

     Functional Description


A+W Continuous Cutting




                              english
1. Contents
1.         Contents                                                       3
2.         Notes on this Document                                         4
  2.1.     Trademarks                                                     4
  2.2.     Copyrights                                                     4
  2.3.     Exclusion of liability                                         4
3.         Performance Description                                        5
  3.1.     Data                                                           5
  3.2.     Description                                                    5
     3.2.1. A+W Continuous Cutting – Office Planner (220085)              5
     3.2.2. A+W Continuous Cutting – Full Office Planner (220086)         6
 3.3.      Prerequisites                                                  6
 3.4.      List of functions                                              6
     3.4.1. Overview of the planned work                                  6
     3.4.2. Planning of the cutting                                       6
     3.4.3. Continuous cutting                                            7
 3.5.      Restrictions                                                   7
 3.6.      Notes                                                          7
4.         Contact Address                                                8




A+W Software GmbH                   EN-FUNC-A+W Continuous Cutting.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The contents of the documentation are only
informative and are subject to changes without prior notice. The text and illustrations were
compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH
cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly
negligent action.


2.1. Trademarks
All hardware and software names mentioned in this documentation can also be registered
trademarks or other property rights of third parties. Third party copyrights must be observed.


2.2. Copyrights
© 2021, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation can be copied, completely or in part, saved in an archiving
system, or transferred in any other form only in accordance with our license agreement. The
documentation may not be transmitted electronically, by recording or in any other form without
the prior written permission of A+W Software GmbH.


2.3. Exclusion of liability
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




A+W Software GmbH                EN-FUNC-A+W Continuous Cutting.docx                                  4
3. Performance Description
3.1. Data
 Product               A+W Continuous Cutting
 Article number        220085, 220086
 Module                A+W Continuous Cutting – Office Planner

                       A+W Continuous Cutting – Full Office Planner
 Brief                 Module for automating cutting
 description
 Available             QR11-2021 for pilot installation


3.2. Description
The A+W Continuous Cutting module allows the automation of cutting by planning the cutting for
the individual tables in the Office version of the A+W Realtime Optimizer in advance.
In the preparation and planning, the operator inspects the upcoming batches and assigns them to
the appropriate cutting tables for processing. Here the sequence of the batches to be processed is
determined and it is decided for each batch how breakage should be handled and what should
happen to residual plates.
These planned batches are then processed by the workers at the respective cutting tables. They
don't have to select any more cuts themselves or make any settings for cutting. The possibility to
optimize the table is also eliminated. The flow on the cutting table is thus automatic according to
the planned sequence.
Depending on the software on hand, the module is divided up into 2 separate modules.


3.2.1.          A+W Continuous Cutting – Office Planner (220085)
This is an expansion of an existing A+W Realtime Optimizer in the office. With this expansion, it is
possible to plan a sequence, which jobs and lots must be cut next on the A+W Realtime Optimizer
on the cutting table.
In the office, a complete A+W Realtime Optimizer (220016) or the A+W Realtime Optimizer (EL)
Breakout Display (220080) and the A+W Realtime Optimizer (EL) - Basic Optimizer (220081) are
required.
On the cutting table, a complete A+W Realtime Optimizer (220016) or the A+W Realtime Optimizer
(EL) Breakout Display (220080), the A+W Realtime Optimizer (EL) - Basic Optimizer (220081) and
the A+W Realtime Optimizer - Advanced Optimizer (220082) is required.




A+W Software GmbH               EN-FUNC-A+W Continuous Cutting.docx                                   5
3.2.2.          A+W Continuous Cutting – Full Office Planner (220086)
This is a special A+W Realtime Optimizer version for the office, which allows the use of all functions
that are required to plan and prepare orders and lots that should be cut next on the A+W Realtime
Optimizers on the cutting table. Thus, this module includes both table optimization and the planner
for continuous cutting.
On the cutting table, a complete A+W Realtime Optimizer (220016) or the A+W Realtime Optimizer
(EL) Breakout Display (220080), the A+W Realtime Optimizer (EL) - Basic Optimizer (220081) and
the A+W Realtime Optimizer - Advanced Optimizer (220082) is required.


3.3. Prerequisites
    •   A+W Production (core module)
    •   A+W Realtime Optimizer (for the planning and continuous cutting, see above for details)


3.4. List of functions
The basic function of A+W Continuous Cutting consists functionally of 3 parts:
    •   Overview of the planned lots (in the office)
    •   Planning of the cutting (in the office)
    •   Continuous cutting (on the cutting table)


3.4.1.          Overview of the planned work
In the overview, you can see the planned lots for each cutting table and get an overview of how
much work there still is for the individual tables.


3.4.2.          Planning of the cutting
In the planning view, all lots optimized in A+W Production and released for cutting and their
properties are displayed. Here, you can now select which lots should be cut on the cutting table
for which they were optimized. Here, the sequence can be specified and various settings made.
For lots already planned, it is possible to make changes, assuming that the cutting has not yet
begun.
    •   Filter: For a better overview, filters can be applied in order to filter the lots displayed by
        glass types, for example.
    •   Production date: if a time span is specified here, only lots are displayed whose production
        date is in this time span.
    •   Reoptimization: specifies the mode for the reoptimization and the quantity of broken lites
        starting from which this should be triggered.
    •   Rush optimization: specifies whether a rush optimization should be executed for the lot if
        a particular quantity of broken lites has been reached.
    •   Residual plate management: specifies whether and in which mode the residual plate
        should be linked.


A+W Software GmbH                EN-FUNC-A+W Continuous Cutting.docx                                6
    •   Process residual plate: allows the processing of the residual plate starting with a particular
        length.
    •   Group: several batches can be combined into a group. Batches of the same group will be
        sent together to the cutting table in cutting in the A+W Realtime Optimizer. If cutting has
        begun for a group in cutting, no batch in this group may be changed. A batch must be
        assigned to a group in order to be released for cutting.
    •   Rush group: batches that belong to the rush group are handled preferentially.
    •   Sequence: for batches and groups whose cutting has not yet begun, the sequence in which
        they are processed can be changed at will.
    •   Reset: already planned batches and settings can be reset so that they are not cut
        automatically.


3.4.3.          Continuous cutting
If the A+W Realtime Optimizer on the cutting table is running in "continuous cutting" mode, an
overview of the batches planned for this table is displayed before the start of cutting. Here it is
possible to reset a batch if necessary. If you continue with the cutting, the first group will be loaded
into cutting and the cutting started. If there is a rush group, it is loaded first and the subsequent
group is attached. When the last batch of the current group has almost been cut, the next group is
loaded into cutting automatically. This way, all planned batches are gradually processed
automatically according to the settings made in planning.


3.5. Restrictions
A batch can only be planned for the table that was assigned to it in A+W Production. If a batch
should nevertheless be cut on another cutting table, this can be achieved with the table
optimization in the Office version of the A+W Realtime Optimizer.


3.6. Notes
An Office version of A+W Continuous Cutting is required for planning continuous cutting.




A+W Software GmbH                EN-FUNC-A+W Continuous Cutting.docx                                  7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Continuous Cutting.docx   8

