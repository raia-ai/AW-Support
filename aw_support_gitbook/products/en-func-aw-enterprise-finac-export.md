---
title: "EN FUNC A+W Enterprise FinAc Export"
category: "functional_descriptions"
product: "A+W Enterprise FinAc Export"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Enterprise FinAc Export"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   Export of master data and document data for processing in financial accounting                                          e n g l is h 1. Contents 1.   Contents                                                                 3 2.   Notes on this Document                                                   4      2.1. Trademarks                                                          4      2.2. Copyrights                                                          4"
source_file: "EN-FUNC-A+W Enterprise FinAc Export.pdf"
---


# EN FUNC A+W Enterprise FinAc Export

      Functional Description


Export of master data and document
data for processing in financial
accounting




                                     e n g l is h
1. Contents
1.   Contents                                                                 3
2.   Notes on this Document                                                   4
     2.1. Trademarks                                                          4
     2.2. Copyrights                                                          4
     2.3. Exclusion of liability                                              4
3.   Performance Description                                                  5
     3.1. Data                                                                5
     3.2. Description                                                         5
     3.3. Requirements                                                        5
     3.4. List of functions                                                   5
     3.5. Restrictions                                                        6
     3.6. Notes                                                               6
4.   Contact Address                                                          7




A+W Software GmbH                  EN-FUNC-A+W Enterprise FinAc Export.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license.. The contents of the documentation are only
informative and are subject to changes without prior notice. The text and illustrations were
compiled with the utmost care. However it is not possible to exclude errors completely. A+W
Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to
wilful or grossly negligent action.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2023, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation may only be copied whole or in part, stored in
an archiving system or transmitted in any other form in accordance with the license agreement.
The documentation may not be transmitted electronically, by recording or in any other form
without the prior written permission of A+W Software GmbH.


2.3. Exclusion of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions which have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions that
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH              EN-FUNC-A+W Enterprise FinAc Export.docx                             4
3. Performance Description
3.1. Data
 Product                A+W Enterprise
 Module number ###(vorl. 200021)###
 Module                 FinAc Export
 Brief                  Provision of master data and document data for processing
 description            in financial accounting
 Available              A+W Enterprise v6
                        + current AWE FinAc Service

3.2. Description
A+W Enterprise offers the opportunity to export master data and document data in customer-
specific format for provision to financial accounting.
The desired data format is specified by the customer.


3.3. Requirements
    •   Check of the software used for the financial accounting. Determination of the existing
        import interface and the import format.
    •   Provision of the interface documentation for the import interface.


3.4. List of functions
    •   Export in any format (XML, ASCII, etc.), depending on the FinAc specified.
        A common format is currently XML. It is used for the transfer to eGecko, for example.
        Possible at the same time is the transfer to a webservice (SOAP service or REST service).
    •   Configuration of the FinAc service
            o   Export directory
            o   FTP transfer
            o   Timer: Daily export/transfer time
    •   Configuration of the required FinAc accounts.
    •   Export of the data as files in a configured directory. FTP transfer is possible.
    •   Export of documents (SA invoices/credit notes, PU invoices/credit notes, also collective
        invoices).
    •   Export of master data (customers/suppliers).


A+W Software GmbH              EN-FUNC-A+W Enterprise FinAc Export.docx                             5
   •   Consistency check, total check of the amounts in the documents.
   •   Rush FinAc transfer data
       Processing of rush transfer data, regardless of the timer setting, via individual script.
   •   E-mail notification if there are problems during data export.
   •   Automatic updating of the open items (totals) based on the exported documents in A+W
       Enterprise after the FinAc export.
   •   The export of stock movement data is possible.
   •   The import of totals is possible.
   •   Detailed documentation for the export interface will be created.
   •   Easy to maintain, easy update of the AWE FinAc Service in ongoing operation in less than
       10 minutes.


3.5. Restrictions
   •   There is no archiving of the export files thus far.


3.6. Notes
   •   The export of the data is done via a Windows service (A+W Enterprise FinAc Service). A
       suitable service must be provided.
   •   The FinAc interface is programmed customer-specifically.
       The customer provides the required information for the import interface of the FinAc.
       Then, in consultation with the customer, the data transfer is specified (data mapping of
       the A+W Enterprise data and the FinAc import interface), insofar as this is possible in
       advance.
   •   An extensive test phase is anticipated:
           o   A test version of the AWE FinAc Service is installed and configured at the client as
               early in the development process as possible, so that test export files can be
               generated.
           o   When importing the test files into the FinAc, it is determined which data is
               missing in the export file or must be adjusted.
           o   After each test, there is another implementation step until the data is present in
               the desired form.
           o   The repeated installation of the AWE FinAc service in the test phase is done in
               little time (< 10 minutes) and without restriction of the workflows on the
               customer system.




A+W Software GmbH             EN-FUNC-A+W Enterprise FinAc Export.docx                              6
4. Contact Address
A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany
Tel. +49 641 96620-0


E-Mail: zentrale@a-w.com
Internet: http://www.a-w.com/




A+W Software GmbH          EN-FUNC-A+W Enterprise FinAc Export.docx   7

