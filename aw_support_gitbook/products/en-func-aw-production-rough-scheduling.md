---
title: "EN FUNC A+W Production Rough Scheduling"
category: "functional_descriptions"
product: "A+W Production"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Production", "Rough Scheduling"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Production - Rough Scheduling                                    english 1. Contents 1.   Contents                                                               3 2.   Notes on this Document                                                 4      2.1. Trademarks                                                        4      2.2. Copyrights                                                        4      2.3. Exclusion of liability"
source_file: "EN-FUNC-A+W Production-Rough Scheduling.pdf"
---


# EN FUNC A+W Production Rough Scheduling

      Functional Description


A+W Production - Rough Scheduling




                               english
1. Contents
1.   Contents                                                               3
2.   Notes on this Document                                                 4
     2.1. Trademarks                                                        4
     2.2. Copyrights                                                        4
     2.3. Exclusion of liability                                            4
3.   Performance Description                                                5
     3.1. Data                                                              5
     3.2. Description                                                       5
     3.3. Requirements                                                      5
     3.4. List of functions                                                 6
     3.5. Limitations                                                       7
     3.6. Notes                                                             9
4.   Contact Address                                                       10




A+W Software GmbH           EN-FUNC-A+W Production-Rough Scheduling.docx        3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The text and illustrations were
compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software
GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or
grossly negligent action.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2016, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation may only be copied whole or in part, stored in an archiving
system or transmitted in any other form in accordance with the license agreement. Transmission
of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or
in any other way, without the written prior approval of A+W Software GmbH.


2.3. Exclusion of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to perform changes to software data, structure and
interfaces as part of program extensions without prior notice. All amendments, extensions,
database queries, reports, analyses, and interface extensions which have been individually
created for our customers and/or machine and software partners as well as all related costs and
expenses are to be borne by the customer (customers, machine and software partners). This also
includes possibly necessary long-term costs and expenses for amending and extending
subsequent program versions. This is necessary to make sure that the commissioned
amendments/extensions which have been made or developed for a version will work flawlessly
and can be used in the successor version.




A+W Software GmbH          EN-FUNC-A+W Production-Rough Scheduling.docx                            4
3. Performance Description
3.1. Data
 Product                 A+W Production
 Article number          220001, 220002
 Module                  Rough Scheduling
 Brief description       Rough Scheduling
                         Creation and management of production batches and
                         buckets as well as definition of views
 Available               Starting with ALCIM 2000


3.2. Description
The rough scheduling serves to feed orders transferred from the commercial ERP system into
detailed planned batches and then into production. It relies on the automatic processes and
calculation of the A+W Production data import (for example, the calculation of geometry data,
broken edges, dimension proposals, costs, and times).
In the rough planning, after successful scheduling (alias data import, Items4Alcim), the people
responsible for work preparation use different views to get an overview of the parts included in
the order/quotation data, their production conditions (e.g. production dates) and dependencies
(e.g. receipt of goods dates for ourchase parts). They then use various strategies to form batches
manually that enable optimal production. The results of the detailed planning, optimization, and
production depend in large measures on the rough planning (batch formation).
Across the entire life cycle of an order and/or quotation in the work preparation and production,
relevant information can be viewed and reported back to the ERP system (e.g. production status,
receipt of goods dates for purchase parts, information about changes).


3.3. Requirements
    •   A+W Production (ALCIM) (article numbers 220001 and 220002)
    •   Set-up and correct master data (e.g. processing sequences, stock dimensions, item master
        data), so that it can be evaluated during scheduling and then calculated and displayed
        correctly.
    •   The scheduling process must flow successfully and correctly.
    •   For the definition and use of views, as well as the efficient application of rough planning
        logic and setting possibilities, an extensive and detailed training by an experienced A+W
        consultant is indispensable.




A+W Software GmbH          EN-FUNC-A+W Production-Rough Scheduling.docx                              5
3.4. List of functions
1) Views and information
   •   There are 12 pre-defined views: orders, buckets, batches, filler orders, packaging, purchase
       parts, reservation orders, glass types, items, processings, order overview, details
           o   Each of these views can be expanded using view concept and to include
               information (for example filters, columns, colors).
           o   The scope of the expansion possibilities differs for each of the views mentioned
               here.
           o   For a detailed description of the displays, as well as the possibilities for
               adjustment/management, please see the A+W Production Rough Scheduling
               manual.
   •   Using the view concept, it is possible to display specific information from the A+W
       Production database and incorporate it in a view.
   •   It is possible to define individual views.
   •   It is possible to export and import already-created views. This can be helpful in the course
       of a back-up concept (for restoring views) or with several production locations (identical
       set-up and configuration).
   •   Expansions of/adjustments to views can be saved globally (for all users) or user-specifically
       (only for this user).
   •   Free SQL queries to the A+W Production database are possible.
   •   There is an order search that also offers specific information about what the current status
       of the order/quotation is. Using this, it is possible to conclude with which views you can
       view the appropriate details.
   •   Purchase parts and reservation orders are displayed using different identifiers in specially-
       designed displays.
           o   After successful receipt of goods reporting, purchased parts are removed
               automatically from the purchase display. The information is then visible in the
               order views.
           o   After successful release (from the ERP system), reservation orders are transformed
               into normal orders. The information is then visible in the order views.
   •   With use of the A+W Production Capacity Planner (article number 220006 and 220007),
       data that is determined/calculated in the course of scheduling (costs, default times,
       machines, production dates) is displayed in the rough scheduling views.
   •   With the Late, non-production-relevant changes function, data from the ERP system can be
       transferred to A+W Production, even if the order/batch status is already advanced (e.g.
       optimized or in production). The relevant information is then updated and visible in the
       rough scheduling views.
           o   Non-production-relevant information includes: e-mail address, telephone number,
               shifting of the delivery date into the future, route, delivery address, commission,
               customer item, file attachments.



A+W Software GmbH          EN-FUNC-A+W Production-Rough Scheduling.docx                           6
           o   Individual non-production-relevant information mentioned here can, depending on
               the customer company, be production-relevant. A definition and adjustment of
               permissible work methods and processes by the A+W Professional Service is
               therefore recommended.


2) Batch formation/bucket formation
   •   For a detailed description of the possibility for creating and managing batches and buckets,
       please see the A+W Production Rough Scheduling manual.
   •   It is possible to form batches and/or buckets.
   •   It is possible to add orders, items, and parts to an existing batch and/or bucket
       (depending on the status).
   •   It is possible to remove orders, items, and parts from an existing batch and/or bucket.
       These can then be viewed again in the basic views.
   •   Orders, items, and parts can be packed from an existing batch or bucket into another
       batch or bucket (depending on the status).
   •   It is possible to divide batches and/or buckets (depending on the status).
   •   Batches and/or buckets can be suspended (depending on the status). The orders,
       quotations, items, and/or parts can then be viewed again in the basic views.
   •   Several batches and/or buckets can be merged to one another.
   •   In the process of planning and work preparation, the batch status is increased automatically
       (e.g. in the course of detailed scheduling and optimization).
             o The new status information with respect to the orders/quotations included in the
                 batches is reported to the ERP system.
   •   It is possible to reset the batch status manually (for example, detailed scheduling > rough
       scheduling)
             o The new status information with respect to the orders/quotations included in the
                 batches is reported to the ERP system.
   •   After the planning step Release to production, the batch can be increased both by the
       system (status booking in the course of plant data collection via scanner and/or A+W
       Production Terminal - article numbers 220010, 220011, 220012) as well as manually (for
       example, ready for dispatch or delivered).
             o The new status information with respect to the orders/quotations included in the
                 batches is reported to the ERP system.

3) Post-processing/reworking
   •   It is possible to use the context menu to manually post-process rush lites, filler lites,
       shapes, muntins, and individual processings (e.g. edge deletions or area deletions).
       o   For a detailed description of the post-processing possibilities, please see the A+W
           Production Rough Scheduling manual.


3.5. Limitations
1) Displays


A+W Software GmbH         EN-FUNC-A+W Production-Rough Scheduling.docx                             7
   •   Colored highlights (e.g. colored columns for different information) is only possible via
       customizing. If you would like/require colored highlights, please contact A+W Support.
   •   By default, quotations and orders are not separated in different displays. For a distinction
       (e.g. for quotation optimization), additional information must be filtered (e.g. display of the
       order ID in an additional column).
   •   Quotations and orders cannot be optimized together.
       o The system does not prevent the joint planning of quotations and orders in batches and
           buckets. This may cause an error at the start of the optimization.
       o An additional information column with the quotation/order ID should therefore always
           be configured in the scheduling views in order to prevent joint scheduling (and then
           joint optimization).
   •   For the display of information, it can be relevant to define components/items in the master
       data as so-called release parts (e.g. Master data > Item > Item). This defines whether the
       parts are visible explicitly in the views or whether they are included implicitly in products
       and can be planned implicitly (e.g. film for LSG or spacer for IGU.)
       o The only display that can also display non-released parts is the Processing display. All
           other displays can generally only display released parts. An adjustment/change is not
           possible.
       o In older program versions (ALCIM) - in the so-called compact mode - all parts/items are
           defined as released parts.
   •   There are no standard displays that provide an overview of all items of an order if these
       have been scheduled in different batches and/or buckets.
       o It is recommended that you use additional reports (e.g. Crystal Reports) or create
           individual displays in order to keep a comprehensive overview of all order data in
           various batches.

2) Batch creation/bucket creation and management
   •   In practice, there are various strategies for optimal batch formation; these depend heavily
       on the company in question, the machines, and the products to be produced. Therefore,
       there is no automatic batch formation and management.
   •   There is no reference between different batches and/or buckets. If parts from orders are
       included in different batches and/or buckets, the user is obligated to manage the data.
       o It is recommended that you use additional reports (e.g. Crystal Reports) or create
           individual displays in order to keep a comprehensive overview of all order data in
           various batches.
   •   Orders/quotations included in buckets cannot be optimized or released to production. It is
       necessary to form a batch for this.
   •   With use of the A+W Production Capacity Planner (article number 220006 and 220007),
       determined processing and/or assembly dates are not considered in the batch formation.
       Thus on the batch formation as production date dialog, the current date is always
       selected/pre-populated, not the earliest product start date determined by the capacity
       planning for all parts of a batch.
       o   Here it is recommended that you insert the earliest product start date for all parts
           determined by the capacity planning as additional column in the rough scheduling
           views and then confirm the dates in the batch formation manually.

3) Post-processing/reworking




A+W Software GmbH         EN-FUNC-A+W Production-Rough Scheduling.docx                              8
   •   Manually post-processed glass, processings, muntins, and/or shapes are not considered
       by the A+W Production Capacity Planning (if used, article number 220006 and 220007)
       since this processing runs in the background during scheduling. Appropriate data (e.g.
       costs or processing durations) can therefore not be displayed in the rough scheduling
       views.


3.6. Notes
Set-up of new displays
   •   The set-up is normally done in the course of a customer project or update. For this, a
       detailed conversation is initiated, in which the customer (e.g. Production Manager and
       employees who handle work preparation) and the A+W consultant analyze the basic
       conditions and real requirements together. Then there is an attempt to map this in the
       displays.
   •   In a new project, a database with a set of defined and described displays can be made
       available to the customer. This guarantees that a) production is quick and easy using the
       default views defined and b) these displays continue to function in the course of update
       and patches.
   •   The batch formation has significant effects on the detailed scheduling and yield results and
       can therefore result in significant added costs. Therefore, it is recommended that you
       familiarize yourself intensively with the possibilities and displays of the A+W Production
       Rough Scheduling. Furthermore, it is recommended that in case of changes in the item
       master data area, you always contact A+W Support.
   •   In practice, there are various strategies for optimal batch formation; these depend heavily
       on the company in question, the machines, and the products to be produced. Therefore,
       there is no automatic batch formation and management.
   •   The A+W standard database, which we offers customers in the course of a new project and
       we recommend that they use, includes a pre-defined set of displays and master data. These
       were set up by experienced A+W consultants based on many years' experience.

Additional notes and detailed information
   • For detailed descriptions of exact operation methods and workflows in the course of rough
        scheduling, please see the A+W Production Rough Scheduling manual and the help.
   • For detailed questions before you have purchased product(s), please contact A+W Sales or,
        in the course of cooperation, A+W Support.




A+W Software GmbH         EN-FUNC-A+W Production-Rough Scheduling.docx                           9
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH       EN-FUNC-A+W Production-Rough Scheduling.docx   10

