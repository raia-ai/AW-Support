---
description: "EN FUNC A+W Clarity Experience Dispatch"
---



# EN FUNC A+W Clarity Experience Dispatch

     Functional Description


A+W Clarity Experience Dispatch




                                  english
1. Content
1.   Content                                                                3
2.   Notes on this Document                                                 4
     2.1. Trademarks                                                        4
     2.2. Copyrights                                                        4
     2.3. Exclusion of liability                                            4
3.   Performance Description                                                5
     3.1. Data                                                              5
     3.2. Description                                                       5
     3.3. Prerequisites                                                     5
     3.4. List of functions                                                 6
     3.5. Restrictions                                                      7
     3.6. Notes                                                             7
4.   Contact Address                                                        8




A+W Software GmbH            EN-FUNC-A+W Clarity Experience Dispatch.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The contents of the documentation are only
informative and are subject to changes without prior notice. The text and illustrations were
compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH
assumes no liability for errors or imprecise statements unless these can be traced back to
intentional or negligent actions.


2.1. Trademarks
All hardware and software names mentioned in this documentation might also be registered
trademarks or other property rights of third parties. The property rights of third parties must be
observed.


2.2. Copyrights
© 2020 A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation may only be copied whole or in part, stored in
an archiving system or transmitted in any other form in accordance with the license agreement.
The documentation may not be transmitted electronically, by recording or in any other form
without the prior written permission of A+W Software GmbH.


2.3. Exclusion of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions that have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions which
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH           EN-FUNC-A+W Clarity Experience Dispatch.docx                             4
3. Performance Description
3.1. Data
 Product               A+W Clarity Experience
 Module number 200040
 Module                Dispatch
 Brief                 A+W Clarity Experience Dispatch is incorporated into the existing A+W
 description           Enterprise 6 software environment for the planning and processing of
                       dispatch workflows.
 Available             A+W Enterprise V6 and current A+W Clarity Experience



3.2. Description
A+W Clarity Experience is a development initiative in order to, based on the existing A+W
Enterprise 6 database infrastructure and functionality, develop a modern and flexible user
interface for customers.
The A+W Clarity Experience includes all newly developed modules that have been developed in an
agile manner in the course of Clarity Experience. With the agile approach, the customer is
incorporated actively into the development process at all times. The application is transformed
step by step so that the reworked areas work seamlessly with the other A+W Enterprise modules.
The A+W Enterprise dispatch control is the first module that has run through the A+W Clarity
Experience process.
The A+W Clarity Experience Dispatch helps users with their daily work in the dispatch
environment and helps them with the planning and organization of goods dispatch.


3.3. Prerequisites
The prerequisite for the use of A+W Clarity Experience Dispatch is the use of A+W Enterprise
Version 6 with current back end package. The operating system requirements are always
documented so they are up-to-date in the A+W release matrix for modules with ICE
communication.
The data provision for A+W Clarity Experience Dispatch is done via the existing A+W Enterprise
modules. The use of A+W Clarity Experience Dispatch builds on the knowledge of the whole A+W
Enterprise product.
A+W Clarity Experience Dispatch access the database and existing functions of A+W Enterprise
directly. All changes are saved immediately in the known and proven A+W Enterprise data
structures.
For use of the rack level in A+W Clarity Experience Dispatch, use of A+W Production and the A+W
Barcode Manager is required since the data is displayed directly from the A+W Production
database (no interface!).


A+W Software GmbH          EN-FUNC-A+W Clarity Experience Dispatch.docx                          5
If routes should be optimized with the A+W Logistics Optimizer, the appropriate programs and
licenses for the A+W Logistics Optimizer are required.


3.4. List of functions
A+W Clarity Experience Dispatch assists the role of the Dispatcher and Picker in the dispatch
environment. The appropriate dialogs are tailored to the respective role.
The Dispatcher has a complete overview of all goods to be sent. His task is to plan the deliveries
and compose the routes.
The Picker prepares the goods to be delivered based on the Dispatcher's planning. He always has
current information from production (completion messages and rack allocation). He checks
whether the goods on the rack are complete and then releases the rack for dispatch.
List of functions
    -   The central calendar starts with the current month, positioned on the current day. All
        days with planned routes are "highlighted." Navigation on the calendar is done analogous
        to calendar navigation in the MS Office products.
    -   After selecting a calendar day, an overview of all routes for the selected day is displayed
        clearly with the most important information.
    -   After selection of a route, the orders with their KPIs and summary KPIs are visualized
        clearly for the entire route so they are easy to understand
        (quantity, weight, area, number of delivery addresses, etc.).
    -   Using selected symbols, various order types (rush order, top priority order, replacement
        order, etc.) are identified.
    -   A configurable attention symbol ( ) indicates orders to which special attention must be
        paid. For this, particular limit values can be defined flexibly (e.g. special shape, weight,
        dimensions, etc.).
    -   The Dispatcher can shift individual orders, items or parts of them.
        He can also shift several orders or several items at the same time. In case of a shift, a
        reason for the shift must be specified.
        Each change and shift is logged.
    -   On the timeline, the Dispatcher all (partially) shifted orders, all order components, and
        their status are displayed clearly.
    -   On the item and/or rack level, the Picker checks to make sure the goods are complete and
        releases them finally for dispatch. A+W Clarity Experience Dispatch helps with dialogs are
        that are specially optimized for these activities.
    -   The Picker always has information about whether the order is already complete, how
        many units are planned, produced, and packed.
    -   The current data (from the A+W Production PDC (production progress, last registration
        point, rack allocation, etc.) are available to the Picker online in the barcode view.
    -   The Picker can "report after the fact" parts that were not reported (missing quantity
        check).
    -   The system supports role-based handling of missing parts.
        The Picker can report parts as "missing" or reset the "missing status."


A+W Software GmbH           EN-FUNC-A+W Clarity Experience Dispatch.docx                               6
        The Dispatcher sees the parts marked as missing on a special dialog and can shift them
        directly to another route with later delivery. If the completion of a route is required when
        the Dispatcher is not present, then the Picker can shift the missing parts to a special
        clarification route, from which the Dispatcher can later update the planning.
    -   The private fields of the order in A+W Clarity Experience Dispatch are available to support
        special customer-specific requirements.
    -   The system offers a clear possibility for printing loading lists and the selected (advance)
        delivery notes with visual identification of what has already been printed. For printing, the
        proven reports of A+W Enterprise dispatch control are available (Crystal Reports® and/or
        Repgo).
    -   The familiar, proven list printing from A+W Enterprise is available with and without
        parameter entry.
    -   There is an easy search function available for searching. With it, you can search the orders
        according to different criteria (order, customer, delivery address, consignment, etc.) and
        periods of time. As result, all hits are displayed; in particular, the various routes and data
        for partial deliveries. By selecting the desired data record, you can go directly to the
        corresponding order in A+W Clarity Experience Dispatch.
    -   An integration of the A+W Logistics Optimizer enables the optimization of routes and
        support for delivery with the A+W Smart Delivery app.
Additional interface features
    -   The software can be scaled to fit any needs.
    -   For better clarity, there are a multitude of filter and sorting functions available.
    -   Colored status symbols help maintain clarity on all levels.
    -   Numerous tooltips help you with operation.
    -   In many places, colored progress bars also enable an assessment of the current situation
        in dispatch and production at first glance.


3.5. Restrictions
Not all A+W Enterprise dispatch control functionalities are currently available in A+W Clarity
Experience Dispatch. The module includes the functions listed above and will be enhanced
according to priorities in close cooperation with our customers.


3.6. Notes
The simultaneous use of the A+W Clarity Experience Dispatch and the Dispatch control module in
A+W Enterprise is possible. The deliveries per route/day to be processed by the user are locked
program-internally in order to prevent a simultaneous processing and mutual interference or
overwriting.
Please note that the A+W Clarity Experience Dispatch product is in constant development and
therefore, functionalities will be improved constantly and new functionalities added.




A+W Software GmbH            EN-FUNC-A+W Clarity Experience Dispatch.docx                           7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH        EN-FUNC-A+W Clarity Experience Dispatch.docx   8

