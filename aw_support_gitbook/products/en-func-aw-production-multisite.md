---
title: "EN FUNC A+W Production Multisite"
category: "functional_descriptions"
product: "A+W Production Multisite"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Production Multisite"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Production Multisite                                   english 1. Contents 1.       Contents                                                    3 2.       Notes on this Document                                      4   2.1.   Trademarks                                                  4   2.2.   Copyrights                                                  4   2.3.   Exclusion of liability                                      4 3.       Performance Description"
source_file: "EN-FUNC-A+W Production Multisite.pdf"
---


# EN FUNC A+W Production Multisite

     Functional Description


A+W Production Multisite




                              english
1. Contents
1.       Contents                                                    3
2.       Notes on this Document                                      4
  2.1.   Trademarks                                                  4
  2.2.   Copyrights                                                  4
  2.3.   Exclusion of liability                                      4
3.       Performance Description                                     5
  3.1.   Data                                                        5
  3.2.   Description                                                 5
  3.3.   Prerequisites                                               6
  3.4.   List of functions                                           6
  3.5.   Restrictions                                                6
  3.6.   Notes                                                       7
4.       Contact Address                                             8




A+W Software GmbH            EN-FUNC-A+W Production Multisite.docx       3
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




A+W Software GmbH               EN-FUNC-A+W Production Multisite.docx                                 4
3. Performance Description
3.1. Data
 Product               A+W Production Multisite
 Article number        228001, 228002
 Module                A+W Production Multisite – Basic License
                       A+W Production Multisite – Site License
 Brief                 Enables the hosting of A+W Production in several locations
 description
 Verfügbar             A+W Production v6 – 2021


3.2. Description
A+W Production Multisite offers the opportunity to operate several production locations in one
infrastructure. Depending on the user's login, the application called in A+W Production is
redirected to the correct infrastructure (database, common directories, etc.).
With this solution, the customer saves massively on hardware costs. Since an update affects all
connected locations simultaneously, costs are also saved here. However, this assumes good
planning and organization for the update.




A+W Production Multisite is offered in 2 modules:
A+W Production Multisite – Basic License (228001): offers the infrastructure for operating A+W
Production in a multisite environment. Several production sites can be connected to this
environment.
A+W Production Multisite - Site License (228002): enables common use of the server
infrastructure by different sites.




A+W Software GmbH              EN-FUNC-A+W Production Multisite.docx                              5
3.3. Prerequisites
Since an update in a multisite environment affects several operations simultaneously, such an
update has to be planned precisely. All operations have to exit the use of A+W Production and its
components (A+W Production Terminal, A+W Realtime Optimizer, etc.) for the time of the
update.
For an update, there are various tasks that must be performed manually. There are instructions
for this in the A+W Production configuration instructions.
For A+W Production Multisite, one basic license and a site license for each connected operation
are required per server. Whereby "per server" should not be taken entirely literally; the focus is
sooner on a commonly used infrastructure.
Example: a group consists of 5 separate operations. In the standard installation, therefore, 15
servers are required for the A+W Production operation:
5 x process server
5 x terminal server
5 x database server
With the introduction of A+W Production Multisite, clusters with the individual operations can be
formed.
    a) Cluster north includes the operations 1 – 3 and requires:
       - 3 servers (process server, terminal server, and database server)
       - 1 x A+W Production Multisite – Basic License
       - 3 x A+W Production Multisite – Site License
    b) Cluster south includes operations 4 and 5 and requires:
       - 3 servers (process server, terminal server, and database server)
       - 1 x A+W Production Multisite – Basic License
       - 2 x A+W Production Multisite – Site License
So 9 servers are eliminated (less the Multisite licenses)!


3.4. List of functions
A+W Production Multisite supports most A+W Production modules. Exceptions are listed under
"restrictions."


3.5. Restrictions
    -   A+W Dashboard (AWDesk #452052) – terminated in Phase 1 since May 2021
    -   Some ICE services (A+W Planning DataProvider, A+W Planning Import, Config Tool, …)
        (AWDesk #458026; Backlogitem 26637)
    -   Various scripts (PostIGU2.bas, Cutting2.bas, vorfein.bas, …) are currently only executed
        from %Programfiles%\... . However, since they can be different for the individual
        operations, they have to be shifted to %Serverdir%\... (AWDesk #395142)
    -   TRANS, TEXTE, Designer Dialoge etc. must be copied or created individually for the
        individual operations. Only for the "default site" is this taken over from the Setup
        Launcher (AWDesk #393513)


A+W Software GmbH               EN-FUNC-A+W Production Multisite.docx                                6
   -    Tools relating to the BLOCK file do not work (DEBNET, ViewBlock, CopyBlock,
       ConvertBlock, …) (AWDesk #416753)
   -   AWPort (problems with IP addresses and does not run as service) – however AWPort is
       terminated (Phase 1 since June 2019; Phase 2 starting in November 2021)!
   -   Interface "Delivery Date Check"


3.6. Notes




A+W Software GmbH            EN-FUNC-A+W Production Multisite.docx                           7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH           EN-FUNC-A+W Production Multisite.docx   8

