---
description: "EN FUNC A+W Residual Stock Manager"
---



# EN FUNC A+W Residual Stock Manager

     Functional Description


A+W Residual Stock Manager




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
     3.6. Notes                                                          7
4.   Contact Address                                                     8




A+W Software GmbH              EN-FUNC-A+W Residual Stock Manager.docx       3
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




A+W Software GmbH             EN-FUNC-A+W Residual Stock Manager.docx                             4
3. Performance Description
3.1. Data
 Product       A+W Realtime Optimizer (220016), A+W Realtime stand-
               alone (220903)
 Module number 220079 / 230079
 Module               A+W Residual Stock Manager
 Brief                Module for reuse of residual plates in upcoming cut batches
 description
 Available            Starting with A+W Production v6


3.2. Description
With the A+W Residual Stock Manager , you can save and process residual plates without
machine assistance. For this purpose there is a web interface that can be opened from anywhere
via a browser The stored residual plates are then automatically available in the A+W Realtime
Optimizer for further processing.


3.3. Requirements
It must be guaranteed that the stock serves supports the interface (MCStockMasterControl) used
by the A+W Realtime Optimizer. This interface already provides communication to third-party
storage systems such as Hegla or Bystronic.


3.4. List of functions
   •   The cutting dialog shows in which manual slot a residual lite is to be stored or from which
       it is to be removed
   •   You can create residual plates manually, defining the glass type, glass thickness, storage
       location/warehouse location, and dimensions of the residual plate
   •   You can change the dimensions of a created residual plate
   •   You can change the storage location of a created residual plate
   •   You can change the glass type and thickness of a created residual plate
   •   In the course of table optimization in the A+W Realtime Optimizer, you can select
       individual residual plates that can be used for the optimization.




A+W Software GmbH           EN-FUNC-A+W Residual Stock Manager.docx                              5
Stored residual plates are displayed in an overview in the A+W Residual Stock Manager and can
be edited in the view, e.g. the sizes of the residuals stored.




The residual plates stored are then used for table optimization in the A+W Realtime Optimizer on
the "Residual plates and stock plates" tab and can be used for the next cutting batch.
Printing of the appropriate labels is also possible from the overview.


3.5. Limitations
It must be heeded that the Stock Service currently only supports the storage and removal of
residual plates. In possible, these functionalities are also possible for stock plates. However, this
requires additional logic that has to be implemented.
You can operate the A+W Residual Stock Manager in connection with a physical residual plate
system such as Hegla ReMaster or Lisec RPS.
Scheduling orders are generated only for end pieces of a stockplate. If Y-residuals should be
scheduled, they must be created manually.




A+W Software GmbH              EN-FUNC-A+W Residual Stock Manager.docx                                  6
3.6. Notes




A+W Software GmbH   EN-FUNC-A+W Residual Stock Manager.docx   7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH          EN-FUNC-A+W Residual Stock Manager.docx   8

