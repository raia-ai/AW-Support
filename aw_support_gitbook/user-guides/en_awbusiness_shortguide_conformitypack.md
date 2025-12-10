---
description: "EN AWBusiness ShortGuide ConformityPack"
---



# EN AWBusiness ShortGuide ConformityPack

Implementation of the Conformity Pack in
A+W Business




                                       English
    Editorial
    Notes on this document
    This document is intended for end users of A+W Business. This documentation and the software it describes are issued
    only in connection with licences and must be used and copied only accordance with this licence. The contents of the
    documentation are only informative and are subject to changes without prior notice. The text and illustrations were
    compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for
    errors or inaccuracies unless they can be attributed to wilful or grossly negligent action. This document describes the full
    scope of A+W Business in connection with A+W Production.

    A+W Software GmbH cannot be held liable for data errors resulting from the basics of the standard functions provided
    by Microsoft or Unix.


    Copyrights
    © 2013, A+W Software GmbH, all rights reserved, including the right of reprint, production of copies, and translation.
    The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form
    only in accordance with our license agreement. Without the prior, written consent of A+W Software GmbH, the docu-
    mentation must not be passed on to third parties, neither electronically, mechanically, by recording, or in any other way.


    Trademarks
    All hardware and software names mentioned in this documentation can also be registered trademarks, and should be
    considered as such. Third party copyrights have to be obeyed.



    Value+
                                                                                                        +
    The right to use these functions and services is granted only in connection with a valid value contract or based on
    a special, individual agreement. We reserve the right to audit the licences and their utilization.


    Should you have questions regarding this subject please contact a member of the A+W sales team or please refer
    to our homepage http://www.a-w.com/.




                                             A+W Software GmbH  Konrad-Adenauer-Straße 15

                                             35440 Linden  Germany

                                             Tel. +49 6403 970-0  Fax +49 6403 64390

                                             www.a-w.com  zentrale@a-w.com
                                     2013 A+W Software GmbH
Contents

Editorial                                                        2
   Notes on this document                                        2
   Copyrights                                                    2
   Trademarks                                                    2
        +
   Value                                                         2

Contents                                                         3
Legal Background and Motivation                                  4
Master Data Input and Management                                 6
   Management and Registration of Declarations of Performance    6
   The Utilities Module                                          9
   Company Master Data                                           9
   Product Master Data                                          10
   Partner Master Data                                          11
   Management of Forms                                          12
   Management of Rights                                         13

Application in Document Management                              14
Printing of Forms                                               16
Transfer to Production                                          17




                                                                     A+WBusiness – Short Guide Conformity Pack
Legal Background and Motivation
As from 1 July 2013, the European Construction Products Regulation prescribes that all manufacturers and
intermediate dealers in the EU issue, manage, and provide declarations of performance (DoP for short).




Figure 1: Interaction of Declaration of Performance and CE code (direct process)




                                                                                                             A+WBusiness – Short Guide Conformity Pack




Figure 2: Interaction of Declaration of Performance and CE code (dealer process)

A declaration of performance must be issued if a construction product belongs to a harmonized standard,
or is consistent with a European Technical Assessment (ETA). Statements and information on the
performance/characteristics of a product can be made only (e.g. in advertisements) if these are stated and
specified in the same way in the declaration of performance.
"By issuing the declaration of performance, the manufacturer takes the responsibility for the construction
                                                          1
product being in compliance with the stated performance."
The application of the Construction Products Regulation requires that a declaration of performance is
issued for every product/every product structure. The declaration of performance must be provided at the
latest upon delivery, per order item, and in electronic form (PDF/DOCX). If an order includes several
identical products it is sufficient to supply the declaration of performance just once per product. It is also
permitted to issue a declaration of performance which comprises all order items. If requested by the
customer, the declaration of performance must be provided in printed form.
The declaration of performance must be kept for ten years and must be presented upon request (e.g.
customer's or auditor's request).




                                                                                                                 A+WBusiness – Short Guide Conformity Pack




Fig. 3: Declaration of performance - an example




1
    Official gazette of the European Union, issue 04.04.2011 (L 88 / 12), paragraph 4, section 3
Master Data Input and Management
Using the new functions with regard to the declarations of performance according to the Construction
Products Regulations requires the following settings in your system's master data:
        Declaration of performance management: Registration of declarations of performance
        Company master data: tab Parameters - email dispatch, standard DoP
        The Utilities module: Declaration of performance - product structure
        Product master data: tab Attachments
        Partner master data: tab Attachments
        Management of forms: tab Form
        Management of rights: Right to effect manual changes in the documents, per user


Below, we are going to describe these settings in detail.


Management and Registration of Declarations of Performance
To be able to attach a declaration of performance to a document (or a specific order) or to assign a
declaration of performance to a product or a business partner by default, the declaration of performance
has to be registered in the system first.


This registration can be made centrally in Master Data > Products > General > Declaration of Performance,
Management.




                                                                                                            A+WBusiness – Short Guide Conformity Pack




Fig. 4: Dialogue "Declaration of performance management"
Number
Number of the declaration of performance (alpha-numerical)

Name
Name of the declaration of performance. This should be unique and descriptive.

Language
Language in which the declaration of performance is issued. The combination of number, name, and
language of the declaration of performance allows keeping and registering a DoP with a certain number in
different languages.

Link
<Reference_Path>\dop; path for saving the declarations of performance. It is defined in Company master
data > tab Documents.

[Add], [Remove]
These buttons are used for adding a language version of the DoP, or removing it from the list.


How to register a declaration of performance
1.   Go to Master data > Products > General > Declaration of performance management.
2.   Go to Menu > Start > New to register a new declaration of performance.
3.   Enter the number and name.
     You can choose these entries at random. Every DoP number must exist only once however.
4.   Select the language of the DoP. Alternatively, you can allocate different languages (documents) to a
     DoP with a unique number.
5.   Click on the [File] icon next to the field Link to open the directory.
6.   Choose the required template.
7.   Go to Menu > Start > Save to save the data.
     The DoP is now available in product management and can be assigned as required.


Alternatively you can register a DoP in product master data (as a default for a certain product) or in
company master data (as a default for a business partner). These declarations of performance will be
automatically loaded and dispatched if no specific, individual DoP is assigned to a product structure or
document.
                                                                                                            A+WBusiness – Short Guide Conformity Pack
Fig. 5: Registering a declaration of performance


New / Remove (left side of dialogue)
Create a new record (new, blank dialogue) for entering a new declaration of performance or delete the
remove the existing record/entries.

New (right side of dialogue)
Save the new record.




      Registering a Declaration of Performance
To assign a declaration of performance to a document (e.g. a specific order) or to assign a declaration of
performance to a product by default, the declaration of performance must be registered in the system first.
A+W Business offers a new table for this purpose in which all defined combinations of product structure
(ID) and declaration of performance are saved. Default product structures defined in master data will be
                                                                                                              A+WBusiness – Short Guide Conformity Pack




taken into account as well as alternative product structures which e.g. result from a sheet being exchanged
at item entry.
Technical information: Product structure table (BW_PRODUKT_AUFBAU_LENR)
The Utilities Module
Module Utilities > System > Declaration of Performance, Product Structure




Fig. 6: Declaration of performance, product structure



This dialogue serves to define the distinctive features to be analysed in product structures. Every defined
product type/product group combination is treated as an individual feature.
Should this distinction be insufficient you can also define that the corresponding article number shall be
used as well.




Company Master Data
Master Data > Company > Company data > tab Parameter




Fig. 7: Company data - tab Parameter


Dispatching declarations of performance
                                                                                                               A+WBusiness – Short Guide Conformity Pack




This setting serves to activate the dispatch of declarations of performance for this business partner.
In management of forms you can also define whether the declaration of performance shall be dispatched
upon printing.
Standard Declaration of Performance
This field serves to define the DoP to be dispatched by default to the business partner if an order item has
not been assigned any specific, separate DoP. The declarations of performance are saved in the standard
directory for file attachments in <Reference_Path>\dop. This directory is defined in Company data > tab
Documents.
The [File] button can be used for registering a declaration of performance for this product/product
structure. Use the [Zoom] icon to display the list of declarations of performance already registered in the
system and saved in <Reference_Path>\dop.



Product Master Data
Master Data > Products > Products> tab Attachments




Fig. 8: DoP allocation/registration in article master data


In product master data you can assign a declaration of performance which shall be dispatched by default for
this product/product structure. In the actual order, this DoP can be amended for the individual items, e.g.
after a sheet has been exchanged.


Number
Number of the specific declaration of performance assigned to this product/structure by default. The
combination of product structure (product structure ID) and DoP number is saved in the system.
                                                                                                              A+WBusiness – Short Guide Conformity Pack




The [File] button can be used to register a declaration of performance for this product/product structure.
Use the [Zoom] icon to display a list of declarations of performance already registered in the system and
saved in the defined directory in <Reference_Path>\dop.

Declaration of performance required
This setting defines whether a DoP is required for the product in question (a spacer will not require a
separate DoP for example). The code and the assigned DoP will be adopted for the order item. If no DoP is
assigned, the standard DoP defined in company master data will be used.



     Registering a Declaration of Performance
To assign a declaration of performance to a document (e.g. a specific order) or to assign a declaration of
performance to a product by default, the declaration of performance must be registered in the system first.




Partner Master Data
Master data > Partners > Customer > Customer > tab Attachments




Fig. 9: Partner master data (example customer)

Dispatching declarations of performance
                                                                                                                A+WBusiness – Short Guide Conformity Pack




This setting is used for activating the dispatch of declarations of performance for the partner (customer) in
question.
Management of Forms
Master Data > Forms > Form Management > tab Form




Fig. 10: Form Management


Email dispatch
This setting defines the print point at which the DoP shall be emailed.




                                                                          A+WBusiness – Short Guide Conformity Pack
Management of Rights
Master Data > Products > General > Declaration of Performance, Management




Fig. 11: Partner master data (example customer)



This dialogue serves to define the user rights with regard to the management of declarations of
performance. You can e.g. define whether a user shall be entitled to manually assign a declaration of
performance at item entry.


                                                                                                        A+WBusiness – Short Guide Conformity Pack
Application in Document Management
When a new item is entered, the declaration of
performance number for the item is initially
loaded from product master data.


When an item is changed (e.g. glass exchange),
the product structure of the current item will be
checked/re-determined. This product structure
is searched in the product structure table, and
the product structure ID plus the corresponding
DoP number are adopted for the item. If the
structure cannot be determined, the declaration
of performance number will be removed from
the item.


This is followed by an input check at item entry.
The program checks whether the flag for
determining the declaration of performance has
been set in product master data for the product
in question and if so, whether a declaration of
performance exists in the item. If the code has
been set but no declaration of performance has
been assigned, a message to that effect will be
issued. This permits to assign a DoP by hand at a
later stage. This message can also be disabled on
user level.



                                                    Fig. 12: Process of determining the DoP at document entry

The item is saved now. If the declaration of performance number for the current item has been changed by
hand, it will be saved for the item. If the product structure of the item has been changed (e.g. glass
exchange), the new product structure - along with the assigned declaration of performance number - is
saved in the product structure table. If the product structure has already been entered in this table, the
assigned declaration of performance number will be replaced.
                                                                                                                A+WBusiness – Short Guide Conformity Pack
Module Documents > Order > Order > tab Items




Fig. 13: Assigning a declaration of performance to an item


Declaration of Performance
Number of the assigned declaration of performance


DoP search
Starts the search dialogue for the manual search for a registered declaration of performance




                                                                                               A+WBusiness – Short Guide Conformity Pack
Printing of Forms
When the form is printed, the system first checks in which language the form (order confirmation, delivery
note, etc.) shall be printed. In customer master data, the standard language assigned to the customer is
checked. If no language settings for the declaration of performance are found for the item (neither in the
forms nor in customer master data), the standard DoP will be loaded from company master data.


After the declaration of performance has been dispatched, an internal note is made in customer data
(technical info: table DR_KUNDEN_LENR). This makes sure that this DoP will not be dispatched again next
time the customer orders the same product structure. As an additional information, the printing date and
the shipping information (type of printout and document number) are also saved in the table. When
printing is repeated, this table will be checked; emailing of this declaration of performance will be
suppressed.




                                                                                                             A+WBusiness – Short Guide Conformity Pack
Transfer to Production
The transfer to the production planning system A+W Production must include the DoP number as a text
record in the Order.xml. Enter the appropriate standard text with a special text code and allocate it in
product data.


Module Master data > Text > Text




Fig. 14: Example: Standard text for transfer to production


The link to the declaration of performance can also be transferred to A+W Production via Order.xml. Enable
the Code for file attachments to be transferred > A All for this purpose

                                                                                                             A+WBusiness – Short Guide Conformity Pack
Module Production > Production > Transfer to Production > Menu Functions > Settings > tab
Text/Attachments.




Fig. 15: Transferring text and attachments to production




                                                                                            A+WBusiness – Short Guide Conformity Pack

