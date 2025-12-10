---
title: "EN FUNC A+W Generation of Partial Delivery"
category: "functional_descriptions"
product: "A+W Generation of Partial Delivery"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Generation of Partial Delivery"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Business (PRO) - Generation of Partial Delivery                                      english 1. Contents 1.   Contents                                                                 3 2.   Notes on this Document                                                   4      2.1. Trademarks                                                          4      2.2. Copyrights                                                          4      2.3. Exclusion of liability"
source_file: "EN-FUNC-A+W Generation of Partial Delivery.pdf"
---


# EN FUNC A+W Generation of Partial Delivery

      Functional Description


A+W Business (PRO) -
Generation of Partial Delivery




                                 english
1. Contents
1.   Contents                                                                 3
2.   Notes on this Document                                                   4
     2.1. Trademarks                                                          4
     2.2. Copyrights                                                          4
     2.3. Exclusion of liability                                              4
3.   Performance Description                                                  5
     3.1. Data                                                                5
     3.2. Description                                                         5
     3.3. Requirements                                                        6
     3.4. List of functions                                                   6
     3.5. Limitations                                                         6
     3.6. Notes                                                               7
4.   Contact Address                                                          8




A+W Software GmbH           EN-FUNC-A+W Generation of Partial Delivery.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The greatest care was used in
compiling the texts and figures. However it is not possible to exclude errors completely. A+W
Software GmbH assumes no liability for errors or imprecise statements unless these can be traced
back to intentional or negligent actions.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2016, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation may only be copied whole or in part, stored in an archiving
system or transmitted in any other form in accordance with the license agreement. Without the
prior written permission of A+W Software GmbH, the documentation may not be transmitted
electronically, by recording or in any other form.


2.3. Exclusion of liability
A+W Software GmbH assumes no liability for data errors that rely on basic principles of the
standard functions made available by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All adjustments, expansions, database
queries, reports, analyses, and interface expansions that were created individually for our
customers and/or machines and software partners as well as all costs and efforts associated with
these were borne by the client (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary in order to ensure that the adjustments/expansions commissioned that
were undertaken/developed for a version will also work perfectly and be used in the subsequent
version.




A+W Software GmbH          EN-FUNC-A+W Generation of Partial Delivery.docx                          4
3. Performance Description
3.1. Data
 Product                   A+W Business (Pro)
 Module number             210017 (230017)
 Module                    A+W Generation of Partial Delivery
 Brief description         With this module partial deliveries can be created
                           automatically
 Available                 Starting with A+W Business (Pro) v5.5 / v6.0


3.2. Description
The A+W Business module "Generation of Partial Delivery' is a module for the easy creation of
partial deliveries both on the basis of items reported ready as well as per rack.
Items reported ready:
Production items are reported ready by the reporting from the production software
    •   With A+W Production via the fileless reporting to A+W Business
    •   In A+W Business Pro through the reporting ready of an item
Purchased items are reported ready through
    •   The entry of goods receipt
    •   Or alternatively via an appropriate registration point in A+W Production
Stock items
    •   behave like production items
Service items
    •   cannot be partial deliveries and are reallocated pro rata in the partial delivery.
Alternatively, the available quantities can also be entered manually in the "Production overview"
module.
Rack order assignments:
Order items are assigned to a rack either via barcoding scannings (scanner) in production or via
the rack management, where you can specify the rack assignment. The "Generation of Partial
Delivery" module creates easy and quick partial deliveries for such order-rack assignments. The
partial delivery is generated on the basis of the quantity of the order item that exists on the
selected rack.




A+W Software GmbH          EN-FUNC-A+W Generation of Partial Delivery.docx                          5
3.3. Requirements
    •   A+W Business (core module)
    •   Ready reports from A+W Production:
        -   Fileless feedback (ERP Webservice)
    •   Configuration of the registration points for
        -   "Produced" for produced parts and
        -   "Goods receipt" for ordered parts
    •   PDC in production
        -   A+W Business Scanner software (individual license)
    •   A+W Business Pro
        -   Configuration of the A+W Business Capacity Planning (machines, production areas,
            etc.)


3.4. List of functions
    •   Generation of partial deliveries on the basis of quantities reported ready
    •   Editing of the partial quantities to be delivered
    •   Generation of partial deliveries based on order items per rack
Features:
       Color marking of the orders in the number manager (complete/not complete)
       Progress indicator (ready, partially delivered, ready for partial delivery) in pieces and
        percentage.
       Manual "completion report" of an order (for example, in case of missing reports)
       Direct printing of the partial delivery note
       Several partial deliveries can be generated for an order.
       Selection possibilities by customer, delivery date, and status (per rack)
       Overwriting of order header data (per rack)
            o   Delivery date
            o   Route
            o   Truck
            o   Driver


3.5. Limitations
Service items cannot be partial deliveries, however they are copied for the creation of the partial
delivery, that is, they are reallocated pro rata.


A+W Software GmbH           EN-FUNC-A+W Generation of Partial Delivery.docx                           6
Only the quantities reported ready can be partially delivered. A correction of the quantities ready
must be made in the previous modules (production or goods receipt) or manually in the
"Production overview" module.
Different orders on a rack will not be combined into a partial delivery. The restriction is that one
order produces one partial delivery. The complete rack is always delivered in part.


3.6. Notes
The module triggers an upstream system that was integrated in the program to create document
copies. Thus the program is independent and can be maintained better because it is not a
component of a module with many modes.




A+W Software GmbH          EN-FUNC-A+W Generation of Partial Delivery.docx                             7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH       EN-FUNC-A+W Generation of Partial Delivery.docx   8

