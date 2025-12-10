---
description: "EN FUNC A+W Furnace Optimizer"
---



# EN FUNC A+W Furnace Optimizer

     Functional Description


A+W Furnace Optimizer




                              english
1. Content
1.   Content                                                             3
2.   Notes on this Document                                              4
     2.1. Trademarks                                                     4
     2.2. Copyrights                                                     4
     2.3. Disclaimer of liability                                        4
3.   Performance Description                                             5
     3.1. Data                                                           5
     3.2. Description                                                    5
     3.3. Prerequisites                                                  5
     3.4. List of Functions                                              6
          3.4.1. PDC                                                     6
          3.4.2. Furnace entrance                                        6
          3.4.3. Furnace exit                                            6
     3.5. Limitations                                                    7
     3.6. Notes                                                          7
4.   Contact Address                                                     8




A+W Software GmbH                   EN-FUNC-A+W Furnace Optimizer.docx       3
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
© 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation may only be copied whole or in part, stored in
an archiving system or transmitted in any other form in accordance with the license agreement.
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




A+W Software GmbH               EN-FUNC-A+W Furnace Optimizer.docx                                    4
3. Performance Description
3.1. Data
Product               A+W Production
Module number 223023
Module                A+W Furnace Optimizer
Brief                 Optimization of furnace beds
description
Available             Starting with A+W Production v6


3.2. Description
For the tempering process of glass lites for TG/TLG, several lites are placed in advance in area
(furnace batch), which are then moved into the furnace together in order to be processed
accordingly there (no conveyor furnace). The furnace optimization tries on the one hand to use
the available space as well as possible; on the other to assist the worker with the quick
assignment of the bed. Thus the primary goal is an increasing of productivity, to be able to temper
as many lites in a time window as possible.
The A+W Furnace Optimizer is integrated into the A+W Production Terminal TG-In and you can
start an optimization from here. For this, you select a glass type and A+W Production Terminal
displays a selection of racks that are in front of the furnace (are in a permanently defined
registration point). These racks must have been loaded in advance via PDC and booked to this
registration point. Here, the user can select one or more racks and start the optimization. In the
process, the optimization heeds the sequence on the racks so that free access is guaranteed.
To assist the user, he is shown the patterns to be assigned at the furnace entry, including the
information about the racks from which he must take the lites.


3.3. Prerequisites
The respective processes for the tempering can be different in a production environment.
Therefore, details about flows and any work resulting from these must be clarified in advance in a
project.
    •   To operate the A+W Furnace Optimizer, the A+W Barcode Manager is required (article
        number 220009), the affected lites must be labeled.
    •   To book the lites, suitable bar code scanners are required.
    •   For processing, both at the furnace entrance as well as at the furnace exit, an A+W
        Production Terminal (article number 220012) is required. Furthermore, the A+W Basic
        Flow Planner Tempering (article number 223003) is required.




A+W Software GmbH                EN-FUNC-A+W Furnace Optimizer.docx                                   5
   •   A second monitor is required if the furnace batch should be displayed on a separate
       monitor. This is possible both at the furnace entrance and exit. The hardware
       requirements should be clarified in advance.


3.4. List of Functions
3.4.1. PDC
       •   Lites are booked on frames via scanner or A+W Production Terminal.
       •   Racks that are ready for the tempering process are booked to a defined registration
           point (the optimization pool).


3.4.2. Furnace entrance
       •   At the furnace entry, a glass type and one or more racks with this glass type are
           selected.
       •   The optimization calculates the optimal furnace bed assignment, taking into account
           the possible unloading sequence of the rack (time stamp of the PDC).
       •   The result is displayed in a table and a graphic display of the furnace bed.
       •   Missing or broken lites can be reported broken or skipped. These lites are displayed
           on the furnace bed in a special color.
       •   An optimization can be canceled. In the process, the lites not yet booked remain in
           the optimization pool and they can be re-used for the next optimization.


3.4.3. Furnace exit
       •   At the furnace exit, the expected batch is displayed. Its target rack is displayed for the
           lite. The furnace batch is displayed as it has been confirmed at the furnace entrance.
       •   Lites that were reported broken at the entrance are missing from the display.
       •   Lites can be reported broken in the furnace batch. The regular processes for breakage
           in A+W Production then apply.




A+W Software GmbH               EN-FUNC-A+W Furnace Optimizer.docx                                      6
3.5. Limitations
•   For shapes, the furnace batch display displays only the circumscribed rectangle.
•   The optimization only refers to racks that are filled by the PDC and exist on a defined
    registration point. With regard to access on the rack, no distinction is made between the
    various rack types (A-rack, L-rack, harp racks). That is, only the time stamp of the PDC plays a
    role for the removal.
•   The assignment of the furnace batches is done primarily from the point of view of an optimal
    assignment of the area. For the respective furnace, there can be very different requirements
    for an assignment based on the furnace properties or the tempering process.
•   For the furnace optimization it applies that - analogous to the cutting optimization - that due
    to the mathematical complexity, an optimal assignment result cannot be guaranteed.
    Instead, the best possible result found is used.
•   It is not possible to add more lites to an optimization via scanner.
•   Missing lites or lites broken during assignment can therefore create gaps in the furnace bed.


3.6. Notes




A+W Software GmbH               EN-FUNC-A+W Furnace Optimizer.docx                                     7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Furnace Optimizer.docx   8

