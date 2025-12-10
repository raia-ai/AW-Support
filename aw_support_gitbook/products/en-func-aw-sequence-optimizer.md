---
title: "EN FUNC A+W Sequence Optimizer"
category: "functional_descriptions"
product: "A+W Sequence Optimizer"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Sequence Optimizer"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Sequence Optimizer                                   english 1. Content 1.   Content                                                             3 2.   Notes on this Document                                              4      2.1. Trademarks                                                     4      2.2. Copyrights                                                     4      2.3. Exclusion of liability                                         4 3.   Performance"
source_file: "EN-FUNC-A+W Sequence Optimizer.pdf"
---


# EN FUNC A+W Sequence Optimizer

     Functional Description


A+W Sequence Optimizer




                              english
1. Content
1.   Content                                                             3
2.   Notes on this Document                                              4
     2.1. Trademarks                                                     4
     2.2. Copyrights                                                     4
     2.3. Exclusion of liability                                         4
3.   Performance Description                                             5
     3.1. Data                                                           5
     3.2. Description                                                    5
     3.3. Requirements                                                   5
     3.4. List of functions                                              5
     3.5. Limitations                                                    6
     3.6. Notes                                                          6
4.   Contact Address                                                     7




A+W Software GmbH                  EN-FUNC-A+W Sequence Optimizer.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only be
used and copied according to this license. The contents of the documentation are only informative
and are subject to changes without prior notice. The text and illustrations were compiled with the
utmost care. Still, errors cannot be totally excluded. A+W Software GmbH assumes no liability for
errors or imprecise statements unless these can be traced back to intentional or negligent actions.


2.1. Trademarks
All hardware and software names mentioned in this documentation might also be registered
trademarks or other property rights of third parties. The property rights of third parties must be
observed.


2.2. Copyrights
© 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation must be copied, completely or in part, saved, or
transferred only in accordance with our license agreement. Transmission of the documentation is
not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without
the written prior approval of A+W Software GmbH.


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




A+W Software GmbH               EN-FUNC-A+W Sequence Optimizer.docx                               4
3. Performance Description
3.1. Data
 Product                A+W Production
 Module number 220014
 Module                 A+W Sequence Optimizer
 Brief                  Module for optimization of glass types taking into account
 description            various criteria
 Available              Starting with A+W Production v6


3.2. Description
The A+W Sequence Optimizer optimizes the sequence of all glass types within the accurately
scheduled production batches, taking into account the sorting sequences, express sheets, and filler
items as well as all standard shapes and free shapes.
It allows the optimization of individual sheets and provides the PPS solution with the optimization
result per glass type and lot. The loading of sheets onto A racks or harp racks in production sequence
is also taken into account.


3.3. Requirements
The use of A+W Sequence Optimizer requires the following software modules:
    •   A+W Production


3.4. List of functions
The A+W Sequence Optimizer receives its instructions from the detailed scheduling of A+W
Production or from the A+W Realtime Optimizer.
Depending on the instruction, the A+W Sequence Optimizer determines the best possible
compromise between the specified restrictions and the possible glass yield. The instructions allow
a bandwidth from a completely free optimization to an optimization that exactly follows the
sorting specifications per rack.
With its more than 100 strategies, the algorithm, which is very fast even with the use of several
computer cores (multithread CPU), enables you to calculate several variants in a short time. This
way, different strict storage sequences can be played through with different effects on
productivity.
Of course residuals from residual storage are automatically considered here and if necessary all
necessary data for storage or use of any residuals created.




A+W Software GmbH               EN-FUNC-A+W Sequence Optimizer.docx                                 5
In the current version, cross-references between different racks are considered if necessary. This
way, the storage sequence in one place can be coordinated with the sequence in another place.
In addition, it is also possible to limit the number of racks that are available simultaneously. Here,
for example, an optimization intended for 8 racks can be executed so that at any point only a
maximum of 5 racks are used. The next rack will be started in the sequence if one of the ones
already started is completely assigned. This is especially interesting with the use of automatic de-
stacking robots.
The necessary master data and the use of the results for statistics, reports, labels or cutting code
drivers for machine control are described in the environment that the A+W Sequence Optimizer
uses (A+W Production, A+W RealtimeOptimizer).


3.5. Limitations


3.6. Notes




A+W Software GmbH                EN-FUNC-A+W Sequence Optimizer.docx                                   6
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH           EN-FUNC-A+W Sequence Optimizer.docx   7

