---
title: "EN FUNC A+W Business Form Printing with Crystal Reports"
category: "functional_descriptions"
product: "A+W Business Form Printing with Crystal Reports"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Business Form Printing with Crystal Reports"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Business - Form printing with Crystal Reports                                         english     1. Content     1.   Content                                                                       3     2.   Notes on this Document                                                        4          2.1. Trademarks                                                               4          2.2. Copyrights                                                               4"
source_file: "EN-FUNC-A+W Business Form Printing with Crystal Reports.pdf"
---


# EN FUNC A+W Business Form Printing with Crystal Reports

     Functional Description


A+W Business - Form printing with
Crystal Reports




                                    english
    1. Content
    1.   Content                                                                       3
    2.   Notes on this Document                                                        4
         2.1. Trademarks                                                               4
         2.2. Copyrights                                                               4
         2.3. Exclusion of liability                                                   4
    3.   Performance Description                                                       5
         3.1. Data                                                                     5
         3.2. Description                                                              5
         3.3. Requirements                                                            10
         3.4. List of functions                                                       10
         3.5. Limitations                                                             10
              3.5.1. General                                                          10
              3.5.2. Distributed printing                                             10
         3.6. Notes                                                                   10
    4.   Contact Address                                                              11




A+W Software GmbH       EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx        3
    2. Notes on this Document
    This documentation and the software it describes is only distributed with a license and may only
    be used and copied according to this license. The contents of the documentation are only
    informative and are subject to changes without prior notice. The text and illustrations were
    compiled with the utmost care. However it is not possible to exclude errors completely. A+W
    Software GmbH assumes no liability for errors or imprecise statements unless these can be traced
    back to intentional or negligent actions.


    2.1. Trademarks
    All hardware and software designations mentioned in the documentation can also be registered
    trademarks or other industrial property rights of third parties. The property rights of third parties
    must be observed.


    2.2. Copyrights
    © 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
    copies and of the translation. The documentation may only be copied whole or in part, stored in
    an archiving system or transmitted in any other form in accordance with the license agreement.
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




A+W Software GmbH       EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx                     4
    3. Performance Description
    3.1. Data
     Product                 A+W Business
     Module                  Form printing with Crystal Reports
     Brief description       Form printing with Crystal Reports via AWSOA Reporting
                             Service
     Available               Starting with A+W Business v6


    3.2. Description
    The goal of the development was to shift the process of form printing to a service and to change
    over to the Crystal Reports reporting tool. The advantage of a separate service is the unburdening
    of the individual workstations. The user can continue his work directly after sending the print job
    to the service. The use of Crystal Reports as report generator has the advantage that the designer
    has a much larger selection than with the Gupta Report Builder. A mixed operation with both
    report generators is also possible. Thus, the forms for regular customers can be converted to the
    new platform step by step.
    Furthermore, the output of reports from iQuote is supported. As soon as a form is printed from
    the connected A+W Business, the reporting service creates a PDF document that is available in
    iQuote immediately.




A+W Software GmbH      EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx                    5
    The reporting service must be activated in the A+W Business company master data. After that,
    each form that should be printed via the reporting service is converted in the form management
    according to the documentation.




    Figure 1: Master data with activated reporting service

    The standard reports installed by the setup have to be adjusted depending on customer requests.
    In the form management, the old Gupta Report is distinguished from the new Crystal Report by
    the ending of the file name. It is also specified there which tables are used for the output.
    Appropriate to the settings there, the linked form must also take its data from the set print tables.




    Figure 2: Form management with an order confirmation in the new Crystal Report format




A+W Software GmbH           EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx                6
    As soon as a print is ordered, the reporting service creates an entry in its internal structures and
    then completes the acceptance of the print job right away. The caller (A+W Business) then
    receives the message immediately that the print job was accepted without having to wait for
    completion of the printout. In separate threads whose maximum number can be set, the actual
    processing is then begun.




    Figure 3: Settings for the print service




A+W Software GmbH            EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx                   7
    Each step of this processing is reported back to the caller and can be observed on a tool dialog in
    A+W Business.




    Figure 4: The tool dialog with the status of all print jobs for the user currently logged in

    The user can display or delete already-printed reports with the tool dialog. Only the reports are
    visible that the user currently logged in has printed out. The reports remain in the overview until
    the number of days the respective print job is kept is reached. As soon as that happens, the
    reports in question are deleted by the reporting service. The days kept and the time of the
    deletion process can be defined in the infrastructure settings (see Figure 3).
    The flow of a printout in the service is as follows. As son as the user starts printing in the ERP
    system, the print service is called by a .Net proxy. In the process, all documents to be printed, the
    print mode, the document type, and the form to be used are transferred to the print service.
    Now the print service starts the print procedure and locks the documents, determines invoice and
    delivery note number, takes care of storage transactions, etc. Then the print tables are filled with
    the documents' data. In the process, the print scheme is used, for there the tables and columns
    are stored from which the data required for the print tables must be selected. Directly after filling
    the print tables, the print follow-up runs.
    In the print tables, for the printing, in addition to the print data, a unique ID is stored together
    with a reference to the report to be used. With this information, the Crystal Report Runtime is
    then called in order to create the actual report. Transferred to the report are the above-
    mentioned ID, the output type, the printer to be used or print location, and if necessary, a
    different database connection. Thus, the Crystal Reports Runtime is in a position to create the
    report. Depending on the output type, the printout is either delivered as stream in PDF format or
    sent directly to the printer.




A+W Software GmbH            EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx                   8
                                                                                            XML parameters
                                                   Start of printing
         Messages                                                                           ReportID

                                                                                            Output type
         Stream (report)
                                                                                            Printer

                                                                                            Link for PDF file
                                                   .Net COM proxy
        Client
        (A+W Business / iQuote)




       Spooler                  service
       (.Net)

                                                      Spooler                                           AWSOA
                                                       (.Net)                                          database




         Print              service
                                                           Print lead-up      Filling the print        Print follow-up
         (.Net)
                                                                                   tables

                                                                           Gupta COM object
              Stream (report)




                                                                                Crystal Reports

                                                                                      (.Net)




    Figure 5: Schematic flow of the form printer




A+W Software GmbH           EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx                                  9
    3.3. Requirements
        •   A+W Business (core module)
        •   The update scripts 20170216a.sql and 20170424a.sql must be executed on the main
            database.
        •   A+W infrastructure services


    3.4. List of functions
        •   Seamless integration into the existing A+W Business ERP system
        •   Printout of business documents (e.g. order confirmations, delivery notes, invoices, etc.)
        •   Sending of the generated documents via mail as PDF document without additional third-
            party software
        •   Output of the PDF documents to A+W iQuote
        •   Multi-site support
        •   Multithreading (parallel processing of print jobs)


    3.5. Limitations
             General
    The existing form printing with Gupta Report Builder can use customizing formula that can no
    longer be executed with the new reporting service. The formulas used must be analyzed in detail
    and adjusted according to the documentation in the configuration instructions.


             Distributed printing
    The distributed printing of items on different forms is not supported.




    3.6. Notes




A+W Software GmbH      EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx                  10
    4. Contact Address
    A+W Software GmbH

    Siemensstraße 3

    35463 Fernwald

    Germany

    Tel. +49 641 96620-0



    E-Mail: info@a-w.com

    Internet: http://www.a-w.com/




A+W Software GmbH     EN-FUNC-A+W Business Formulardruck mit Crystal Reports.docx   11

