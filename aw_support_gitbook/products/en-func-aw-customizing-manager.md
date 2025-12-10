---
description: "EN FUNC A+W Customizing Manager"
---



# EN FUNC A+W Customizing Manager

     Functional Description


A+W Customizing Manager




                              english
1. Content
1.       Content                                                    3
2.       Notes on this Document                                     4
  2.1.   Trademarks                                                 4
  2.2.   Copyrights                                                 4
  2.3.   Exclusion of liability                                     4
3.       Performance Description                                    5
  3.1.   Data                                                       5
  3.2.   Description                                                5
  3.3.   Requirements                                               5
  3.4.   List of functions                                          5
  3.5.   Restrictions                                               6
  3.6.   Notes                                                      6
4.       Contact Address                                            7




A+W Software GmbH            EN-FUNC-A+W Customizing Manager.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The contents of the documentation are only
informative and are subject to changes without prior notice. The text and illustrations were
compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH
cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly
negligent action.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2020, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation may only be copied, in whole or in part, saved in an archiving
system, or transferred in any other form only in accordance with our license agreement.
Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by
recording or in any other way, without the written prior approval of A+W Software GmbH.


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




A+W Software GmbH               EN-FUNC-A+W Customizing Manager.docx                                  4
3. Performance Description
3.1. Data
 Product               A+W Customizing Manager

 Article Number        264201, 264202
 Module                A+W Customizing Manager
 Brief                 Tool for copying user-defined objects (reports, scripts, saved
 description           procedures, etc.) to several locations at the same time
 Available             November 2020


3.2. Description
With the A+W Customizing Manager you can save objects in the database in order to distribute
them easily to several systems/locations. It enables you to trace changes and versions and to
ensure that you are executing the same customer-specific objects on all systems.
The A+W Customizing Manager can connect to databases for A+W Enterprise, A+W Business and
A+W Production. This enables the distribution of database objects (stored procedures, views, and
functions).


3.3. Requirements
This tool requires:
    •   Installation on a Windows server
    •   Database users for login. The database users require appropriate privileges in order to
        delete and create stored procedures, views, and functions
    •   In order to define a "Listener" for the DRDA protocol on Informix
    •   IBM DB2 driver package in Windows
    •   An Informix database


3.4. List of functions
    •   Version tracing for objects
    •   Assignment of objects to locations
    •   Checking of which version is used in a location
    •   Distribution of several objects of the same category to several or individual locations at
        once
    •   Informs the user to which location and in which environment the object was distributed
        or not.
Type of the objects:


A+W Software GmbH              EN-FUNC-A+W Customizing Manager.docx                                  5
    •   Scripts (.bas, SELO, .cfg and others)
    •   Crystal Reports
    •   Stored procedures
    •   Views
    •   Functions
Environments for
    •   A+W Business
    •   A+W Enterprise
    •   A+W Production
Enables the configuration of categories:
    •   Database connection
    •   Report path
    •   Script path
    •   It is possible to add user-defined categories.

For each location and every environment.


3.5. Restrictions
A+W Customizing Manager requires an Informix database. The required database licenses must
be acquired separately.
The A+W Customizing Manager can only establish one connection to Informix database(s).
User-defined categories are only possible for file-based objects, not for database objects.
Access for one user.


3.6. Notes




A+W Software GmbH              EN-FUNC-A+W Customizing Manager.docx                           6
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH           EN-FUNC-A+W Customizing Manager.docx   7

