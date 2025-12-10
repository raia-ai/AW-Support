---
title: "EN CONFIG A+W Enterprise DOP"
category: "configuration"
product: "A+W Enterprise DOP"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W Enterprise DOP"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration   A+W Enterprise DOP                                                                        deutsch        A+W Software GmbH   EN-CONFIG-A+W Enterprise DOP.docx   - -INTERNAL-                                                                     1 Change history   Date               Author             Comments                                         Version 2019-02-05         Initial version/EB Transfer from different documents                1.0     Contents 1.   Legal Bac"
source_file: "EN-CONFIG-A+W Enterprise DOP.pdf"
---


# EN CONFIG A+W Enterprise DOP

         Configuration


A+W Enterprise DOP




                                                                   deutsch




   A+W Software GmbH   EN-CONFIG-A+W Enterprise DOP.docx   - -INTERNAL-
                                                                    1
Change history


Date               Author             Comments                                         Version
2019-02-05         Initial version/EB Transfer from different documents                1.0




Contents
1.   Legal Background and Motivation                                                         4
     1.1. Availability                                                                       6
     1.2. Reference to documentation                                                         6
2.   Construction products regulation: Level 1                                               7
     2.1. Master Data Input and Management                                                   7
     2.2. Defining new Document Types                                                        7
                   Restrictions for handling declarations of performance                     7
     2.3. Allocation of Document Types to Certain Forms                                      8
                   Allocation of declarations of performance to special products / product
           structures                                                                        8
     2.4. Registration of Declarations of Performance                                        9
     2.5. Settings in Article Master Data                                                   10
     2.6. Rules for Product Encoding for the Declaration of Performance                     12
                   Example 1: encoding for float glass                                      12
                   Example 2: encoding as atyp=150                                          13
                   Example 3: encoding for all parts of BOM                                 14
     2.7. Application at Order Entry                                                        15
                   Chang of Document Type in the Order                                      15
                   Registering a Declaration of Performance                                 16
                   Determining the Declaration of Performance for an Order                  16
                   Effects of Order Amendments                                              18
                   Handling of Existing Orders                                              18
                   No further changes can be made simultaneously in the order by the intauf
           service                                                                          19
     2.8. Output on Forms                                                                   19
     2.9. A+W Enterprise 5 Print Service                                                    20
     2.10. Transfer to Production                                                           20
     2.11. System Configuration                                                             21
                   Stored Procedures                                                        21
                   Email reference line                                                     21
                   Direct data import in A+W Production                                     21
     2.12. Data Structures - Tables and Fields                                              22
                   repdokuzu                                                                22
                   xledesc                                                                  22
                   xlesprzu                                                                 23
                   xdokutype                                                                23

A+W Software GmbH               EN-CONFIG-A+W Enterprise DOP.docx                                2
                mpdokutype                                                         23
                artikel (extension)                                                24
                kprodkeylezu (transaction data)                                    24
                kposp (transaction data, extension)                                25
                kaufref (transaction data, extension)                              25
                    printfiles (transaction data)                                  25
                    mplercvd (transaction data)                                    26
                    Kaufdokutype (transaction data)                                26
3.   Extension of the construction products regulation: Level 2.                   28
     3.1. Configuration                                                            28
     3.2. Master data                                                              29
                 New product codes                                                 29
                 Market partner                                                    31
                 Article master data                                               31
                 ID assignment                                                     31
                 Maintenance of technical values                                   32
     3.3. Quotation and Order Entry                                                34
                 Start the calculation program.                                    36
                 Evaluation according to DIN EN 1279                               36
     3.4. Creation of DoP Documents                                                37
                 intauf                                                            37
                 Print Service                                                     37
                 DoP report                                                        37
                 Email text for DoP emails                                         38
     3.5. Data structures                                                          38
     3.6. Tables and fields                                                        38
                 MP                                                                38
                 mailparam                                                         38
     3.7. Further documents regarding construction products regulation             39
4.   Expansion of Construction products regulation to include central components   40
     4.1. Local entry without declaration of performance                           40
     4.2. Handling in the central office                                           40
     4.3. Reworking by the background process INTAUF                               41
     4.4. Distribution of the data in the other companies                          41
     4.5. Manual reworking                                                         42
     4.6. Configuration                                                            42
                 Availability                                                      42
5.   A+W CR DoP form                                                               43
6.   Setting declaration of performance "invalid"                                  44
7.   Environment variables                                                         45




A+W Software GmbH               EN-CONFIG-A+W Enterprise DOP.docx                       3
1. Legal Background and Motivation
As of 1 July 2013, the European Construction Products Regulation prescribes that all
manufacturers and intermediate dealers in the EU issue, manage, and provide declarations of
performance (DoP for short).




Figure 1: Interaction of Declaration of Performance and CE code (direct process)




Figure 2: Interaction of Declaration of Performance and CE code (dealer process)


A declaration of performance must be issued if a construction product belongs to a harmonized
standard, or is consistent with a European Technical Assessment (ETA). Statements and
information on the performance/characteristics of a product can be made only (e.g. in


A+W Software GmbH                      EN-CONFIG-A+W Enterprise DOP.docx                        4
advertisements) if these are stated and specified in the same way in the declaration of
performance.
"By issuing the declaration of performance, the manufacturer takes the responsibility for the
construction product being in compliance with the stated performance." (excerpt from official
gazette)


The application of the Construction Products Regulation requires that a declaration of
performance is issued for every product/every product structure. The declaration of performance
must be provided at the latest upon delivery, per order item, and in electronic form (PDF/DOCX).
If an order includes several identical products it is sufficient to supply the declaration of
performance just once per product. It is also permitted to issue a declaration of performance
which comprises all order items. If requested by the customer, the declaration of performance
must be provided in printed form.
The declaration of performance must be kept for ten years and must be presented upon request
(e.g. customer's or auditor's request).




Fig. 3: Declaration of performance - an example




A+W Software GmbH                     EN-CONFIG-A+W Enterprise DOP.docx                         5
1.1. Availability
This functionality is available starting from ALCIB version 2011, in some cases also with ALCIB
version 2009. (s.a. #274142)


1.2. Reference to documentation
Performance Description
The performance description of the module is linked via the intranet (PM > Documentation)
AWE SLT
Extra module.
Description is missing here




A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                                6
2. Construction products regulation: Level 1
2.1. Master Data Input and Management
Using the new functions with regard to the declarations of performance according to the
Construction Products Regulations requires the certain settings in your system's master data
which will be described below. We would like to describe these for you in brief below.


2.2. Defining new Document Types
The menu in section System keys has been completed by the item Document types. This menu
allows entering different document types and the corresponding output type. Foe declaration(s)
of performance, the document type Declaration of performance has been fixed which is firmly
linked with Document type 1.


The output type defines whether or not a business partner shall receive a declaration of
performance. You can select the output type "by email" or "none". If you choose the output type
"none, the declaration of performance is deemed to be generally irrelevant. The checkbox [VF]
can be used to control its application to the document in general.




Fig. 4: Definition and management of document types


When the document types have been defined (but at least the declaration of performance) the
data can be changed for individual business partners in Partner master data. The sub-menu
Text/Print > Document types can be used to adapt existing data which have been saved in the
code. This way, business partners who ship their goods to non-EU countries can be excluded from
the declaration of performance rule.



          Restrictions for handling declarations of performance
    •    Declarations of performance are firmly linked with document type 1.

A+W Software GmbH                    EN-CONFIG-A+W Enterprise DOP.docx                            7
    •    File names must not include special characters like „äöüÄÖÜß“, “|“, „%“ etc.
    •    The actual printing of declarations of performance cannot be done. Instead, declarations
         of performance can be emailed and issued in pdf format as provided by legislation.
    •    The archiving of declarations of performance or other document attachments in A+W
         Enterprise is not scheduled. We recommend saving these documents on a central server
         system or integrating an external archiving system.




2.3. Allocation of Document Types to Certain Forms
In dialogue Document types, transaction types can be selected for which a certain document type
shall be issued (see figure 3, right dialogue section). In System > Print management > Forms >
Document type allocation, the actual forms can be allocated to the transaction types. If no forms
have been defined there, documents cannot be printed or dispatched. At this point you can also
determine the email addresses for document dispatch: To the business partner in question, to the
user who has triggered the document issue, or both.




Fig. 5: Allocation of forms and recipients to document types




           Allocation of declarations of performance to special products
        / product structures
The allocation of declarations of performance to article types or individual articles is controlled by
the product code. You can define certain rules for the product code structure. For more
information please see Rules for Product Encoding for the Declaration of Performance.




A+W Software GmbH                      EN-CONFIG-A+W Enterprise DOP.docx                             8
2.4. Registration of Declarations of Performance
To assign a declaration of performance to a document (e.g. a specific order) or to assign a
declaration of performance to an article type or a product by default, the declaration of
performance must be registered in the system first.


Declarations of performance can be registered by product / product structure in Product code >
Technical values > Declarations of performance. First, enter the alpha-numerical name of the
declaration of performance plus a short description.


Now use <Ctrl+K> or the button [New file] to add the appropriate DoP in different languages. The
documents will be saved by the local computer on the defined server in <DATEI_REF_PFAD>\dop.
If the document was added in different languages at once, the languages have to be allocated
later.


Technical information: The data are saved in database table xledesc. This way, these data can be
used later in all search dialogues.




Fig. 6: Registration of specific declarations of performance


If the documents have already been saved on the server in <DATEI_REF_PFAD>\dop, they can be
assigned by [F9] or using the button [New file] in field File.




A+W Software GmbH                       EN-CONFIG-A+W Enterprise DOP.docx                          9
Fig. 7: Assigning specific declarations of performance by [F9]




2.5. Settings in Article Master Data
Assigning a declaration of performance to a specific article requires the appropriate settings in
article master data. Two new fields for articles have been added to article master data for this
purpose. One field defines the relevance of the DoP (1 = relevant, 0 = irrelevant) while the second
field is meant for the number of the declaration of performance (DoP no.). These fields can be
found on tab Technical values.


The DoP number can be entered by hand right in the field "Declaration of performance" or you
can select an existing number using the search logic.




A+W Software GmbH                       EN-CONFIG-A+W Enterprise DOP.docx                        10
Fig. 8: Settings in article master data


For manual entries, the system checks whether the defined DoP number already exists. If this DoP
number is unknown, the user will be asked whether it shall be assigned. If not, the number will be
deleted. If this is required, the described dialogue for registering a new declaration of
performance will appear.




Fig. 9: Assigning a specific declaration of performance in article master data




A+W Software GmbH                         EN-CONFIG-A+W Enterprise DOP.docx                    11
An existing DoP can only be assigned by a user who has got the right KYLE=‘r‘ while a new DoP can
only be assigned by users with the right KYLE=‘w‘.


When you leave article master data, a product code will be determined for DoP-relevant products
based on the master BOM and on the defined encoding rules (see below) which will be saved in
the database together with the corresponding DoP number.
Technical information: DB table kprodkeylezu.


As an alternative for assigning a DoP to a specific article you can also assign a product code. The
advantage of this is that the assignment is made for all products / article types matching this
product code. This option is described below.




2.6. Rules for Product Encoding for the Declaration of
   Performance
A declaration of performance reflects the technical features and the performance characteristics
of a product structure. To make the management and assignation easier you can define rules as to
how the products shall be represented in a declaration of performance. To this end you can
define individual codes for products and their bills of material.


The basic idea is that only certain characteristics and elements of the product BOM are relevant
for the allocation of a declaration of performance (which is not the case for a spacer as part of an
IG unit for instance). It is therefore possible to automatically allocate the same declaration of
performance to different products with similar bills of material. The code can be defined for
article types (in general) or for individual articles with certain BOM elements (specific). Decisive
for the product code is always the item article or its article type.
The following dialogue is accessible from the menu ALCIB > Master data > Products > Technical
values > Product encoding.



         Example 1: encoding for float glass
All float glass types shall be represented by the same DoP (e.g. LE-FLOAT-STD). Please make the
following settings:

    •   Analysis type = Article type
    •   Number = 100
    •   Encoded as = A type
    •   All other fields remain blank

All products of the article type = 100 (FLOAT fixed size) will get the product code "|100-
<Ass.Pos>". The appropriate declaration of performance can now be assigned to this product
code.

A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                   12
Fig. 10: Rule for product encoding for the declaration of performance




           Example 2: encoding as atyp=150
If encoding as "Article number" is chosen for article type 150 (toughened glass), every toughened
glass article will get the product code "|<Article number>-<Assembly position>" (e.g. "|350005-1"
or "|350006-1").


If a different declaration of performance is required for a special toughened glass processing, this
processing can be defined in "Detailed information" either as the article type, A+W processing
type, or as an article number, and the appropriate encoding type for this processing can be
defined. For example, a coating with ArtNo. 198160 can become part of the product code as
article number. In this case, product code "|350005-1|198160-0|" is generated for toughened
glass with this coating.




A+W Software GmbH                      EN-CONFIG-A+W Enterprise DOP.docx                          13
Fig. 11: Product code definition - encoding as article number




           Example 3: encoding for all parts of BOM
If you select General information > All glass types, all elements of the BOM with article type 100
to 170 will be included in the code. For IG articles, the airspace can be included in the code as well
as other BOM elements which are decisive for determining the technical values. In Detailed
information you can also enter specific glass types if not all glass types are important for assigning
the declaration of performance.




A+W Software GmbH                      EN-CONFIG-A+W Enterprise DOP.docx                           14
Fig. 12: Detailed information for product encoding


If a product encoding rule is changed, the product code will be determined based on the new rule
for all new orders and new items in existing orders. This means that due to the new rule for the
product code(s), no declaration(s) of performance can be found for the existing structures so that
they have to be reassigned.


Technical information: ENV switches existing in versions ALCIB2009 or ALCIB2011 for product
encoding, ISO_PRODKEY_CODE, VSG_PRODKEY_CODE, ESG_PRODKEY_CODE and
FLOAT_PRODKEY_CODE will be automatically adopted for these product areas when the data are
entered for the first time.




2.7. Application at Order Entry
           Chang of Document Type in the Order
When a new order is entered and partner data are loaded from master data, information on the
relevant document types will be gathered as well. Data are loaded first from the code section
which may then be replaced by possibly existing partner data. The data entered for the current
partner (output type and allocated form) have priority over the general data in the code section.
In the info menu (<Shift+F4>) of the order, you can use Document types to view the data ->
settings and change them if necessary. These changes will only apply to the order in question, and
will have top priority.




A+W Software GmbH                      EN-CONFIG-A+W Enterprise DOP.docx                        15
Fig. 13: Replacing the document type in the order


If the declaration of performance is set to Output = "none" in the order, no declaration of
performance will be determined for this order.



           Registering a Declaration of Performance
Only registered declarations of performance will be accepted in the documents. Registrations can
only be made by users with the right KYLE=‘w‘.



           Determining the Declaration of Performance for an Order
When all sizes for the item have been entered, a code will be created based on the sizes and the
bill of material which is then used to search for a DoP number in the allocation table
(kprodkeylezu). This is only done for products which have been marked as DoP-relevant in article
master data, provided that the DoP assignment has not been switched off in document type
output. If a DoP is found, the DoP code appears at order entry in Consignment. The defined DoP
number can be displayed in the item on tab Properties.




A+W Software GmbH                      EN-CONFIG-A+W Enterprise DOP.docx                       16
Fig. 14: Identification of the assigned declaration of performance in the order


If no declaration of performance is found, a declaration of performance number can be entered
by hand in field DoP number. The program now checks whether this declaration of performance
has been registered yet. If this is the case, the manual entry will be adopted. If the DoP has not
been registered so far, the system allows registering the new DoP number (and thus, the
declaration of performance).


The user has to have the appropriate rights for registering a declaration of performance in the
order.




Fig. 15: Registering a declaration of performance in the order



A+W Software GmbH                       EN-CONFIG-A+W Enterprise DOP.docx                         17
You can use the search logic "Selo" [F9] in field DoP number to view the already registered
declarations of performance and select the appropriate one for the item/order <Ctrl+K>.




Fig. 16: Applying the search logic "Selo" in field DoP number

You can use <Ctrl+R> to adopt the relevant DoP number directly from article master data.
Alternatively, you can use <Ctrl+L> to try and allocate a DoP based on the product code and the
defined sizes (refresh).



           Effects of Order Amendments
The system and the functions with regard to the new Construction Products Regulation have been
integrated and are so flexible that you will always be able to adjust them to the customer's
requirements and the situation on hand. You can e.g. change the originally assigned DoP for an
order. These additional or manual order amendments will however result in restrictions and will
have certain effects on the further system behavior:

• Deleting existing files (DoP) and assigning new ones can cause errors in the following processes
  and in following transactions because the files are not allocated to the current transaction and
  will only be analyzed when printed.
• If the bill of materials is changed, a product is exchanged, or a relevant size is changed (e.g.
  airspace in IG), the product code will be recalculated, and the relevant DoP will be determined.
• If a document includes several items with an identical product code and the DoP is changed or
  a new DoP is assigned, it will be adopted for all items with the same product code straight away.
• If a DoP is assigned to a new BOM structure in the order, this DoP will apply to this structure as
  soon as the order is saved.
• For EDI orders, the background process intauf will determine the DoP. Internal EDI will not
  transfer the DoP number; the DoP number will be determined at the receiving site by intauf.




           Handling of Existing Orders
If an existing order is loaded for correction, the program checks if all DoP-relevant items actually
have a DoP. If not, the program tries to find it. The same applies to new orders created with a
reference to old orders. Please note that a DoP will be determined only for those items which
have not been assigned a DoP so far.




A+W Software GmbH                       EN-CONFIG-A+W Enterprise DOP.docx                          18
If an existing document has already been assigned a DoP which had been valid at the time the
document was created, and the product structure (which was entered in the same document)
was assigned another DoP later, the program will not automatically check the allocation for the
existing document.
Menu item Document amendment can be used for checking and assigning the DoP to existing
documents by hand.




Fig. 17: Checking the DoP assignment in menu Document Amendment


<Ctrl+F10> can be used for importing documents before a defined delivery date, the items of
which have no DoP assigned so far. You will see the order/document numbers which include at
least one DoP-relevant item without DoP assignment. The code Free is set for these orders.


[F3] can be used for transferring all listed orders to the background process intauf which will
redetermine the DoP for all items. This applies also to those items which have already been
assigned a valid declaration of performance. You can also enter existing orders which shall get
new declarations of performance or for the items of which the declarations of performance shall
be updated.



        No further changes can be made simultaneously in the order
      by the intauf service
When declarations of performance are checked and/or changed by the background service intauf,
this service will not be available for other/parallel changes during that time.




2.8. Output on Forms
When printing forms, at email dispatch and when printing preliminary delivery notes and delivery
notes in dispatch, the program checks whether declarations of performance and/or other
documents have to be dispatched. It also checks if the form to be printed is allocated to one or
more document types. If this is the case, the document types found will be compared with the
document data. The program will process the declarations of performance and those documents
the document types of which have a matching form vector and are set to output type "by email".




A+W Software GmbH                  EN-CONFIG-A+W Enterprise DOP.docx                              19
You can dispatch up to two emails per document, one to the business partner and one to the
employee. If the recipient is the business partner, the email address is loaded from partner
master data (mp.email). If the recipient is the employee, the email address will be loaded from
employee master data (mitarb.email).


The DoP documents are determined based on the language defined in master data. If there is no
document matching the language code of the order, the program will use the document which is
available in the national language. If no document is found for a DoP number, the configured
replacement document will be used.


If there are items which have been defined as DoP-relevant but have not been assigned a DoP
number, the replacement document will be loaded and dispatched automatically. Maximally one
replacement document will be used per email.


Please note that the preliminary delivery note is a form which processes the data via kauf.vorgang
= 5. If you want to dispatch a declaration of performance together with the preliminary delivery
note (shipping), you have to set the corresponding form vector to "OC" first.


To make sure that declarations of performance are sent just once to the customer, A+W
Enterprise will internally record the DoP numbers sent on a certain date, and the corresponding
email addresses (technical information: table mplercvd). Once a DoP number is listed there for a
business partner, it will not be dispatched again. The same applies to repeated printing.
If there is an error during email dispatch, the corresponding system entries will be deleted so that
the data can be sent again.


2.9. A+W Enterprise 5 Print Service
Electronic dispatch of the declarations of performance and other documents is exclusively done
by the A+W Enterprise 5 Print Service. This Windows service must be installed on a server with a
Windows Server operating system.
Crystal Reports forms are not required if only DoP documents are to be dispatched.



     Further information on system implementation and configuration
Further details are available from AWDesk case 274142 and the attached documentation (e.g.
system specification).




2.10.           Transfer to Production
The declaration of performance number is transferred via Order.xml to the production planning
system A+W Production where it can be used for reports and production papers. The DoP is kept
in A+W Production as a text record for the item, with text type 6100.

A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                                20
If the declaration of performance number shall be transferred via direct data import, it has to be
transferred as a text record to the item. This requires the adaptation and extension of your
system.


In case of questions or if the data transfer does not work as specified please contact a member of
the A+W support team.




2.11.           System Configuration
The variable MODUL_DOP (ON/OFF) activates the logic.
The basic path for file references is entered in the environment variable DATEI_REF_PFAD. This
path must be accessible in UNIX/Linux as well as in Windows. The DoP documents are saved in the
directory DATEI_REF_PFAD\dop.


In the environment variable DOP_ERSATZDOKUMENT you can enter a file name for a document
which shall be dispatched if no matching declaration of performance can be found in the system.
The file must be saved in the same directory as all other DoP documents.



                Stored Procedures

                Email reference line
The email reference is determined by the SP rpdokumailsubject. This stored procedure is not
supplied by default by development but has to be implemented on site. This SP has the following
parameters:

    •   integer auftrnr,
    •   smallint vorgang,
    •   smallint subnr,
    •   smallint formart,
    •   integer mailmanr (akt.manr)




                Direct data import in A+W Production
For configuring/extending the direct data import please run one of the SPs cupmawppauftxt,
cupmawpppmptxt or cupmawppspectxt. The text type 6100 must be used. In ALCIB versions 2011
and 2009, the declaration of performance number with the codes aufnr, posnr and setid=10 is
found in field charval4 in table kposprvfld.



A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                               21
For details on the Text SPs please refer to the document
\\Jupiter\DOKU_DocuWare\ALCIM2000\Import\DirekterDatenimport\User_Manuals\TU_030218
_DirekterImport_58749.doc chapter 2.9.1.




2.12.           Data Structures - Tables and Fields
                repdokuzu
 Field name                       Data type                        Description
 Dokuart                          Smallint                         Document type from
                                                                   xdokutype
 Formart                          Smallint                         Form type from rep
 Empfaenger                       Smallint                         Recipient
                                                                   0 – market partner
                                                                   1 – employee
                                                                   2 – market partner +
                                                                   employee


Replication:
The table can be replicated by means of the existing key replication functions.



                xledesc
 Field name                       Data type                        Description
 Lenr                             char(40)                         Declaration of performance
                                                                   number
 Lebez                            Char(200)                        Short explanation, detailed
                                                                   description
 Manr                             Long                             Number of the employee who
                                                                   has created this DoP


 edat                             Date                             Input date


Replication:
The table can be replicated by means of the existing key replication functions.




A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                               22
                xlesprzu
 Field name                       Data type                        Description
 Lenr                             char(40)                         Declaration of performance
                                                                   number
 File                             Char(200)                        File name
 Manr                             Long                             Number of the employee who
                                                                   has allocated this file to the
                                                                   DoP
 sprkz                            Smallint                         Document language


Replication:
The table can be replicated by means of the existing key replication functions.



                xdokutype
 Field name                       Data type                        Description
 Dokuart                          Smallint                         Document type
 Dokubez                          Char(20)                         Name
 Dokutyp                          Smallint                         Document type:
                                                                   miscellaneous (0) or DoP (1)
 Form                             Smallint                         Form vector
 Output type                      Smallint                         Output type (for DoP, preset
                                                                   as email) - email or none
 Document flag                    Smallint                         To be added to the document
 Prodflag                         Smallint                         reserved


Replication:
The table can be replicated by means of the existing key replication functions.



                mpdokutype
 Field name                       Data type                        Description
 Mpnr                             Long                             Market partner number
 kuliflag                         Smallint                         Market partner type
 Dokuart                          Smallint                         Document type


A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                                23
 Dokubez                           Char(20)                          Description
 Dokutyp                           Smallint                          Document type:
                                                                     miscellaneous (0) or DoP (1)
 Form                              Smallint                          Form vector
 Ausgabeart                        Smallint                          Output type (for DoP, preset
                                                                     as email) - email or none
 Vorgangsflag                      Smallint                          To be added to the document
 Prodflag                          Smallint                          reserved


Replication:
This table is integrated in partner replication by a new environment variable, RP_MPDOKUTYPE. If
the environment variable is not set, the table is replicated by the key mpdokutype.mpnr =
mp.mpnr and mpdokutype.kuliflag = mp.kuliflag. If the variable is set, there will be no replication.
All fields except mpnr and kuliflag are valid local fields.
Partner replication does not check the feasibility of master data at present. This is why the
existence of the transferred mpdokutype.dokuart in xdokutype will not be checked.


                artikel (extension)
 Field name                        Data type                         Description
 Lenr                              Char(40)                          Declaration of performance
                                                                     number
 lerelvant                         Smallint                          Defines if the article is DoP-
                                                                     relevant.


Replication:
Both fields can be defined as local fields. When replication is finished the program checks if the
reference artikel.lenr = xledesc.lenr exists. If not, a warning is recorded in the log, and an
appropriate email is dispatched. This is no actual error however. The replication is still considered
to be successful; the article will be saved.



                kprodkeylezu (transaction data)
 Field name                        Data type                         Description
 hashcodekey                       Char(32)                          MD5 encoded product code
 prodkey                           Char(2000)                        Product code
 Lenr                              Char(40)                          Declaration of performance
                                                                     number.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                   24
 prodkeyId                         Long                              Internal administration
                                                                     number, number from
                                                                     internal number area
 manr                              Long                              Employee who has made the
                                                                     allocation
 edat                              Date                              Date of entry



                kposp (transaction data, extension)
 Field name                        Data type                         Description
 Lenr                              Char(40)                          Declaration of performance
                                                                     number
 Prodkeyid                         Long                              Refers to table kpordkelezu
 lerelvant                         Smallint                          Defines if the article is DoP-
                                                                     relevant.



                kaufref (transaction data, extension)
 Field name                        Data type                         Description
 sprkz                             Smallint                          Document language
 dokuart                           Smallint                          Document type
 prodflag                          Smallint                          reserved


EDI:
This table will only be transferred in connection with P.O. transfer. There will be no transfer in
connection with P.O. creation and internal linking of orders.


                printfiles (transaction data)
 Field name                        Data type                         Description
 Pid                               Integer                           Unique print ID
 Seqnr                             Smallint                          Sequence number
 Statusflag                        Smallint                          Processing status of the file
 Mpnr                              Integer                           Market partner number
 Kuliflag                          Smallint                          Market partner type
 Filename                          char(200)                         File name
 Dokuart                           Smallint                          Document type


A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                   25
Dokutype                 Smallint                   Document type
                                                    0 = miscellaneous
                                                    1 = declarations of
                                                    performance
Receiver                 Smallint                   Recipient
                                                    0 – market partner
                                                    1 – employee
                                                    2 – market partner +
                                                    employee
char_key                 char(40)                   External code. Here: DoP
                                                    number.
long_key                 Integer                    External code.
                                                    This field will not be analyzed
                                                    at present



             mplercvd (transaction data)
Field name               Data type                  Description
Mpnr                     Integer                    Market partner number
Kuliflag                 Smallint                   Market partner type
Lenr                     char(40)                   Declaration of performance
                                                    number
Sendedatum               Date                       Date of email dispatch
Formart                  Smallint                   Form type used to dispatch
                                                    this declaration of
                                                    performance
Email                    char(80)                   Email address to which this
                                                    declaration of performance
                                                    has been sent



             Kaufdokutype (transaction data)
Field name               Data type                  Description
auftrnr                  Long                       Document number
                                                    (kauf.auftrnr)
aufnr                    Long                       Internal document number
                                                    (kauf.aufnr)



A+W Software GmbH       EN-CONFIG-A+W Enterprise DOP.docx                         26
Vorgang             Short                       Document type
                                                (kauf.vorgang)
Subnr               Short                       Sub-number (kauf.subnr)
Dokuart             Smallint                    Document type
Dokubez             Char(20)                    Description
Dokutyp             Smallint                    Document type:
                                                miscellaneous (0) or DoP (1)
Formular            Smallint                    Form vector
Ausgabeart          Smallint                    Output type (for DoP, preset
                                                as email) - email or none
Prodflag            Smallint                    reserved




A+W Software GmbH   EN-CONFIG-A+W Enterprise DOP.docx                          27
3. Extension of the construction products
  regulation: Level 2.
3.1. Configuration
Environment variable MODUL_DOP_2 (ON/OFF) is used to enable the logic for the second
configuration level for the BauPVO and the link to a calculation program that supports the A+W
SLT interface. If this variable is set, MODUL_DOP, i.e. the first configuration level is active too.
DOP_CALCULATOR (OFF, 1, 2) serves to define the calculation program for technical values.
Presently, there are two programs, A+W SLT (=1) and SommerGlobal (=2), that can be configured.
The environment variables DOP_CALCULATOR_MODE and DOP_CALCULATOR_PATH define how
the calculation program is to be addressed plus its storage place. DOP_CALCULATOR_MODE
(0/OFF, 1) defines whether the calculation program is installed locally (=0) or in the network (=1).
If it is installed in the network, DOP_CALCULATOR_PATH must be used to defined the path - in
UNC notation – in which the executable program can be found. In this case, make sure that the
Firebird driver from SommerGlobal is installed under Program Files (x86)\Sommer Informatik
GmbH\FBTreiber. The program checks this. If this driver was not installed, no calculator call is
possible and the start button is grayed out.
Although the program Sommerglobal was installed correctly, sometimes the "Ext. Calculation"
button is not active. This is because the localization of the installation folder is no longer possible
with newer versions. That's why with DOP-CALCULATOR_MODE 0 (no network installation) the
path to the program can be specified with the variable DOP_CALCULATOR_PATH. If this is not the
case, the registry will be searched for the following keys:
    •   HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall\Som
        merGlobal\
        oder
        HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows\CurrentVersion
        \Uninstall\SommerGlobal\
    •   HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Uninstall\Sommer
        Global\
        order
        HKEY_CURRENT_USER\Software\ Wow6432Node
        \Microsoft\Windows\CurrentVersion\Uninstall\SommerGlobal\
The string value InstallLocation is then expected here.


In DOP_MPNR, the "miscellaneous“ business partner is defined which is used for business partner
/ article allocation. This partner has to be entered in partner master data as a "miscellaneous"
business partner.
The DoP numbers created by the system consist of the text from DOP_PRAEFIX and of a number
from a defined number range.
The languages for which the DoP documents shall be created are defined in DOP_SPRACHEN,
separated by commas. These documents are created by the Print Service. Their file names consist
of the content of DOP_DOK_PRAEFIX, the DoP number, and the language code.


A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                    28
The variables DOP_MAILTEXT and CR_MAILSIZE are used to configure the Print Service. For details
please refer to the text.
With the variable DOP_RESTRICT_LEVEL, you control the behavior of any incorrect data for the
transfer to Sommer Global.


changeuser


3.2. Master data
         New product codes
Section Keys > Products > Technical values offers two new dialogues.
Product usage (menu item i)
This is where the usage is maintained in all languages to be printed on the declarations of
performance.
Parameter description (menu item j)
This is where the possible declared performances are maintained, in all languages. Field "No."
shows a selection of possible performances in the defined sequence. The reference is initially
taken from the defined description but can be changed into the reference which is to be printed
on the document. You can also enter a measure for the performance if this shall be printed. Even
the defined standard will be used in the document for the corresponding performance. The
program does not check whether the standard for the individual performance is the same in all
languages.
This order corresponds to the xledesk.output vector and is binding as of the A+W Enterprise of
2019-12-05.
    1. Fire resistance (feuerw)
    2. Fire behavior (brandvh)
    3. Fire exposure (brandbea)
    4. Bullet resistance (dschussh)
    5. Explosion resistance (sprwirkh)
    6. Burglar resistance (ebruchh)
    7. Pendulum impact resistance (pschlagw)
    8. Thermal resistance (tempbest1)
    9. Load resistance (lastw/ lastw2/ lastw3)
    10. Airborne sound insulation (rwwert)
    11. Color reproduction index (farbwieder )
    12. Thermal properties (Ug value) (ugminvalue )
    13. Light transmission factor (trminwert)
    14. Radiation transmission factor (strahltrans )


A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                              29
    15. Solar energy transmission factor (sgwert)
    16. Exterior light transmission factor (pvawert)
    17. Interior light transmission factor (pviwert)
    18. Radiation reflection factor (strahlref )
    19. Radiation absorption factor (strahlabsorp)
    20. Total energy transmission acc. to EN 410 (gminwert)
    21. Secondary inward thermal emission acc. to EN 410 (gsekwert)
    22. Shading coefficient acc. to EN 410 (shkoef )
    23. Thermal radiation factor acc. to EN 13363-2 (warmstr)
    24. Convection factor acc. to EN 13363-2 (konvekt)
    25. Ventilation factor acc. to EN 13363-2 (beluft)
    26. Total energy transmission acc. to EN 13363-2 (gneuwert)
    27. Second. inward thermal emission acc. to (EN 13363-2) (gneuwert)
    28. Direct internal radiation reflection (strahlrefi)
    29. Type (prodtypbez)
    30. Purpose (zweck)
    31. Harmonized product standard (pnorm)
    32. Notified body (notifstelle)
    33. Emissivity of layers in single glasses (strahlrefi)
    34. Direct internal radiation reflection (emissiv)
    35. Load resistance / bending strength (biegefest)
The two values (33) and (34) are determined via A+W SLT and passed on to A+W Enterprise via
the corresponding interface. Thus the values in A+W Enterprise can be filled automatically.
In order to use this logic, it is necessary to install the new back end with environment, the new
front end and an updated (>Version 7.2139) A+W SLT.
Bending strength in AWE (master data)
Master data key
In ..->Product key>Technical values->Groups->Bending strength you can define the bending
strength for different types of glass.
Product encoding of sand blasting
With the change according to the new DIN EN1279-5, A+W Enterprise has been extended as
follows:
Since the bending strength also depends on the article "sand blasting," for all encryptions, Sand
blasting must also be in the list with details.
Unfortunately, in the table, it was also possible to toggle AW processing types for "type of
evaluation." In the document entry, however, there was no evaluation for AW processing types.
Therefore, the coding should be done for the atype= 587. The dialog for product encryption



A+W Software GmbH                  EN-CONFIG-A+W Enterprise DOP.docx                                30
(xprodkeyart.mfo) was adjusted with alcib build 13.04.6030 so that only artnr/atyp are available
for selection. (s.a. #447754)



          Market partner
A market partner of the type "Miscellaneous" should be defined, to which the article data can
refer. This defined number should also be entered in the ENV switch DOP_MPNR.
Maximum email size
The maximum size of the emails a business partner can be receive can be entered on tab "Print"
for customers and suppliers. If no entry is made for a partner, the environment variable
CR_MAILSIZE will be analyzed in which a system-wide default can be entered. If this environment
variable has not been set, 10 Mbytes will be used as a general default.
The Print Service will analyze this entry when sending emails; awmail will not do this.
If an email has more than one file attachment, the program now checks whether the maximum
email size is exceeded. If this is the case, the file attachments will be distributed to several emails
so that the maximum size can be kept.

          Article master data

          ID assignment
All relevant articles (glass, spacers, gas) in "Partner details" have to be allocated to the article
numbers (SommerID) of the calculation program. This is made by the entry for the partner
Miscellaneous – XXX and SommerID for the article in field "ext. article". If there is no allocation,
the technical performance will not be determined.




Since the article "Air" is not kept in A+W Enterprise, the following logic will be used for the
transfer: The ID for air is entered in connection with the spacer article in "additional description";
it will be transferred if no gas is found in the BOM.
Since in A+W Enterprise the coated glass types are only marked with a flag, you enter the glass ID
of the glass itself in "Ext.Artikel" and additional ID of the coating in detail view as "additional
designation."
Bending strength in article master data
For all single glasses (article types 100 to 160), a bending strength group can be assigned to an
article in the "Technical values" tab, which is subsequently included in the evaluation.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                    31
         Maintenance of technical values
There are various technical values which are not determined by the calculation program based on
the structure but have to be entered by hand for the product. If the product has been marked as
"relevant" for the declaration of performance (tab "Techn.values"), a dialog for data maintenance
can be started via menu "Product code->Extended techn.values" or <CtrlF8>, or by pressing <F5>
in field "Declaration of performance".
If no declaration of performance has been entered, the program will create a new number. It
consists of the contents of the ENV switch DOP_PRAEFIX + a unique number which is determined
in the „lenummer“ number range.
Field contents in the dialog
All fields of the declaration of performance "header" have to be filled in because this information
will be printed on the document. The "Assessment system" is preset by 3 (assessment by
SommerGlobal) and field "Notified authority" shows the entries of Sommer Informatik. These
fields cannot be changed.




Section "Declared performances" lists the possible performances for printing the declaration of
performance. All fields which can be determined by A+W SLT interface and the external
calculation program are marked by "*". All other fields can be maintained here manually. If the
performance shall be printed in the document, it has to be ticked in the checkbox as well. At least
one performance has to be selected in order to issue a declaration of performance.




A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                               32
Field "Load resistance" is preset by the glass thickness. For IG units, the load resistance of up to
three individual sheets will be shown. The load resistance field can be modified. The program will
not check whether the new entry matches the master data value.
All fields marked by (*) can be maintained by hand of course. If the calculation through the
calculation program is started later on however, manually changed data will be changed.
Determination of the technical performances is started by the "ext. calculation" button or by
<Start/F3>.


New DoP number
A new DoP number will be assigned if an article did not have a DoP number before but has been
marked as relevant.
Manually defined DoP numbers are still valid as long as they already exist in the system. Selection
by Selo is also possible.
If a new DoP is entered or selected by Selo, the extended technical data cannot be changed.
If the dialogue is started without a number, the program will want to know whether the data of
an existing product shall be adopted. If this is the case, enter the reference article. All declared
performances are adopted, and the load resistance is amended. The user can change the values
afterwards or use the calculation program to determine them. The data can be changed until the
article is saved.
Changing existing data
Automatic amendment: If the product code of an article or article type is changed in Product code
-> Technical values, the program realizes this and immediately informs the user when the article is
loaded. A new product code is created for the article, and a new DoP number is assigned. If the
files for the old DoP number have already been assigned, these will be adopted too. This file
allocation will however be kept only until the extended technical values are loaded because it
cannot be checked whether the entered or determined data match the file contents.

A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                33
IMPORTANT! If a declaration of performance number for a product already exists, the fields in the
dialogue cannot be changed any more. If recalculation for an existing DoP is started via the
calculation program (<F3>), the program will want to know whether a new DoP number shall be
assigned because the old number will be invalidated; the new DoP number will become valid for
this structure after saving. When the new number is assigned, the data can be changed until the
article is saved.
Calculation of technical performances
Determining the values for IG requires an airspace which is not mandatory in master data
however; calculation is therefore started with the default AIR=12 should the airspace be missing
(table musskenn). Determination of the product codes also starts with the default airspace. The
data of the structure or of the article itself will be passed on to the A+W SLT interface and the
calculation program. It is essential for IG that all elements of the article type= glass (100 to 170),
spacer (210,211), and gas have an ID assigned. As the master data for IG products do not include
an article for "air", the ID for air should be entered in connection with the spacer! For laminated
glass articles, even the film layers have to have an ID. If the laminated unit only has an ID for glass
and none for the film layer, the "incorrect" structure will be rejected by the calculation program.
If no allocation is found in the BOM elements, the main article's ID will be transferred.
The declaration of performance will be saved together with all declared performances in the
database table xledesc (this table has been extended).
Dimensioned products
Extended technical performances cannot be determined for dimensioned products in article
master data because the fixed BOM is not available at that point.


3.3. Quotation and Order Entry
The program behavior for determining the DoP number has not been changed. If a DoP is found
for the current product structure, it will be adopted including all saved, declared performances. It
will be adopted including all saved, declared performances. These can be viewed for completely
entered items in "Product details -> Technical values->Declaration of performance" in the item
menu or by <CtrlT>. The left half of the first view shows the technical values determined by
AWE5. The right side shows the header of the existing declaration of performance.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                  34
All declared technical values are listed in "Declared performances". If the DoP already exists, the
data cannot be changed. If the user still starts the calculation of values (CTRL+A/START), the
program will want to know whether the new DoP shall be created and issues a warning saying
that the old DoP will be rendered invalid. All fields marked (*) will be changed.




Old, existing data can be restored by means of <Ctrl+R> or the "Reset" button. When the DoP is
issued for the first time (there has been no DoP for this structure before), the new number will
not be adopted after the reset, and the dialogue closes automatically.


A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                                 35
If there is no DoP for the current structure as yet, a DoP can be assigned manually. Only an
existing DoP number will be accepted however. You can also select and assign a DoP by <F9>. Or
you can start the Declaration of performance dialogue from the menu. A new number will be
assigned (see p.1.3.2). If a DoP record already exists for the main article with the standard
structure (for IG e.g. for another airspace or after replacement of a sheet), the program will want
to know if this shall be used as a template. If there are no records in master data, the program will
want to know if another product shall be used as a template. All values will be adopted for the
new DoP. If the user is authorized to create a DoP (KYLE) and a calculation program is configured,
the program also asks whether the declared technical values shall be determined.
In a new DoP, all values can be changed. This is not the case for existing DoPs.
The function "Declaration of performance" <Ctrl+L> has been revised. Since new DoPs cannot be
assigned freely, files cannot be allocated at this point either. You can view the file allocation
however.
Please note!
In all fields of the declared performances from "Temperature resistance" onwards (except
"Radiation absorption level"), the value "NPD" or a number can be entered. The contents of the
entries in the other fields will not be checked. The input format will be checked.
The technical performances determined on the basis of the calculation program are kept separate
from the technical values which are always calculated anew by A+W Enterprise. The declared
values are reference values only. The calculated values can differ from those. If the calculated
values are poorer it is advisable to check the master data. You should also check the data to be
adopted for the spacer text. This may require an amendment of the spacer formula. (Text
management->Text creation).



          Start the calculation program.
The external calculation program is started interactively whenever a new DoP is created for a
structure. If it is started specifically by <Start/F3>, the user can use the active right (MPLE) to start
the external module in the foreground. The start method will be checked. This can only be done
however to check the calculated data. Amended values or exchanged elements will NOT BE
ADOPTED.


          Evaluation according to DIN EN 1279
If the data are prepared for a new declaration of performance, the bending strength for single and
multi-sheet glass is determined in accordance with the specifications of DIN EN 1279-5.


For single glasses, the value is drawn according to the defined group.For single glasses, the value
is drawn according to the defined group. In the case of multiple glasses, the bending strength is
determined by the data of the individual glass elements. For IG elements the values of the
individual lites are separated by "-" and for LAMI (max. 2 lites) by "/".


The bending strength is only assigned via the glass article. There is no change of groups via added
processing. If there is an A+W processing "sandblasting" in the BOM, the bending strength of



A+W Software GmbH                  EN-CONFIG-A+W Enterprise DOP.docx                                  36
single glass is automatically corrected (multiplied by 0.6). With multiple lites the user gets a hint
and the value should be adjusted manually.


The original assignment of the data for load resistance (glass thickness) remains unchanged.


3.4. Creation of DoP Documents
           intauf
If a new DoP number is created in an order, the corresponding master data will be automatically
created in the tables xledesc (header) and xlesprzu (DoP files). For every language defined in
DOP_SPRACHEN, a record is created in xlesprzu, albeit with an empty xlesprzu.datei field. The file
name is entered in the field by the Print Service afterwards.
Field xledesc.status is initialized with a value of 0. This field will be set to 1 when the print job for
the DoP documents is created for the Print Service. This shall make sure that the DoP documents
are issued just once. In case of an error in the Print Service, this field will be reset to 0 so that the
DoP documents can be issued at the next opportunity.
If the processed is edited by the background process intauf, creation of the DoP files will be
started for all new DoP numbers.

           Print Service
The Print Service creates the DoP documents, copies them to DOP, and enters them in table
xlesprzu. A new output type is defined for this purpose (printtransfer.outputflag = 11). If an error
occurs while the DoP documents are issued, the status of the DoP master data will be reset to 0 as
described above. This way, a new print job can be created for this DoP number by intauf.

           DoP report
A report template in Crystal Report format has been created for the DoP documents which can be
amended for every customer.
In ALCIB, the report has to be set up in System > Print management > Forms > Manage. Special
settings are described in the table below.


 Field                                                Contents
 Formularart                                          195
 Repart                                               Crystal
 Reptyp                                               List
 Anzeige                                              0 = no display
 Aktiv                                                Yes
 Anz.Param.                                           2
 Vorgang                                              195
 Parameter 1                                          char / "lenr“ / enter "Yes"


A+W Software GmbH                  EN-CONFIG-A+W Enterprise DOP.docx                                   37
 Parameter 2                                        nums / "sprkz“ / enter "Yes“


The DoP report is created and installed by the ALCIB service team.

            Email text for DoP emails
DoP documents are dispatched as described in the document on the first configuration level of
BauPVO. SP2 includes a supplement: It is now possible to enter a statistical HTML file which
appears as email text in the email body.
The file name is determined by the stored procedure rpdokumailtext.
This SP has the following parameters:
    -   integer auftrnr,
    -   smallint vorgang,
    -   smallint subnr,
    -   smallint formart,
    -   integer mailmanr (akt.manr)
The return value of the SP is a char value of 256 characters; it must include a file name including
the path. If the SP fails to determine a file name or if the SP has not been installed, the
environment variable DOP_MAILTEXT will be analyzed which can be defined by a default setting.
The Print Service has to have ample access rights for these files. We therefore recommend to save
the files used on the server on which the Print Service is run.
The HMTL files cannot handle graphics at present.


3.5. Data structures

3.6. Tables and fields
            MP
 Field name                       Data type                          Description
 mailsize                         Smallint                           Max. email size for these
                                                                     partners



            mailparam
 Field name                       Data type                          Description
 mailsize                         Smallint                           Max. email size for these
                                                                     email recipients




A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                                38
3.7. Further documents                        regarding           construction
   products regulation
\\jupiter\Doku_DocuWare\ALCIB-
PMS\!General\Marketing_Documents\A+W_Gesamtlösung_zur_Bauproduktenverordnung.pptx


\\hausi\AWDCaseDoc\382\382708\DE-Installationsanleitung_AW_SLT.docx
\\hausi\AWDCaseDoc\382\382708\DE-Installationsanleitung_AW_SLT_Network_Driver.docx
\\jupiter\Doku_DocuWare\AWSLT\!General\A+W SLT - Übersicht.docx




A+W Software GmbH            EN-CONFIG-A+W Enterprise DOP.docx                       39
4. Expansion of Construction products
  regulation to include central components
A company is selected as the central registration point (CRP) for all declarations of performance
for all products and this is entered in the appropriate environment switch in ALL companies. By
activating this switch, the functionality described below is also activated.


4.1. Local entry without declaration of performance
In all companies, the search for a declaration of performance is conducted on the basis of the
BOM. If for the appropriate structure there is no declaration of performance present but the
product is service-relevant, the user is informed of this. If the entry was made in the central office
and the person making the entry has appropriate rights, then there is a query whether the
declaration of performance should be generated. The additional procedure is as it was previously.
In all other companies (not the central office) there is only a message about the missing
declaration of performance. In addition, the responsible employee in the central office is
informed automatically via e-mail with specification of the order n umber and company number.
The transaction can be saved. The items that are declaration of performance-relevant but have no
declaration of performance contain a unique numeric declaration of performance identifier for
the company that is temporary, which is initially saved in the table field kposp.prokeyid. If the
order is obtained for correction before the company-spanning final declaration of performance
has been reported, then the BOMs of such items as well as SZR for IG can only be changed with
the appropriate warning. Under some circumstances, the change may not make sense since the
access to the data from the central office is made directly to the database in the local companies
and you cannot see in the central office that the transaction is presently being edited locally by a
user. The declaration of performance determined from the central office then applies for the old
structure and it not found for the changed structure. If the relevant changes should nevertheless
be made (glass exchange or SZR), we recommend deleting the item and entering it anew with the
appropriate changes.


4.2. Handling in the central office
As soon as the responsible employee is informed of the required declaration of performance, he
can obtain the data from the appropriate local company. For this, the employee starts one of the
following transaction entries anew (order/quotation/priceless entry) and specifies in the header
any customer and any date. This data is not evaluated and is only necessary in order to reach the
item dialog.
In Version AWE5.4 there is no separate access for the entry of the declarations of performance for
third-party companies.
In AWE6 there is an extra access in the area Master data -> Keys -> Products -> Technical values ->
Entry of declaration of performance. The easier data selection can be developed, however this is
not part of this development.
In the empty item field of the 1st item with Ctrl+N , you get one after another the following
queries: company number (H1), transaction type (order/quotation)(V), order number (ANR).
When all 3 entries have been made and are valid, the declaration of performance-relevant items


A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                 40
of the ANR transaction are obtained without declaration of performance from the Company H1. If
the order is currently in processing by the background process intauf at the company H1, then the
access is declined and the creation of the declaration of performance must be done at a later
point in time. Per BOM number and SZR, only 1 item is obtained. No information about shapes,
muntins or steps is obtained because these are not relevant to the declaration of performance. In
the transaction header, the order number, company, and customer from the third-party
transaction are shown. First it is checked whether for this structure there is a declaration of
performance present, if, for example, one was applied for recently by another company (H2). If
this is the case, then this declaration of performance is taken over immediately and the data is
transmitted directly to the company H1 (tables xledesc and kpordkeylezu are filled). If in the
central office no declaration of performance is present for this structure, the declaration of
performance can be generated anew for each item. The new declaration of performance is then
saved in the central office and in parallel also in the company H1. After the last item has received
its declaration of performance, the transaction A1 in company H1 is automatically placed before
the background process intauf (intaufart -41). If not all structures from the third-party transaction
have received a declaration of performance, you can nevertheless end entry of declarations of
performance with <END> or <F12>.Here the question is raised whether the third-party transaction
should nevertheless be taken over into the original company for further processing. In this case,
not all items in company H1 receive a newly-created declaration of performance. During the
entire entry of the declarations of performance for a third-party order, the technical data can be
changed. When the third-party transaction is exited, then all newly-entered declarations of
performance for the appropriate structures are permanently defined in the central office; the
associated values can thus no longer be changed.
In the central offices, in addition, the table xlesprzu is prepared for the newly-entered
declarations of performance with all defined languages and the task is forwarded to the print
service for the file creation.
Insofar as the data was obtained from the third-party company for the transaction entry, the
entry switches into the separate entry mode, which prevents the saving of the transaction data of
the item (kpos/iposp/aufstrukt, etc.) in the central offices. You can only obtain and edit 1 third-
party transaction per batch. In order to obtain a third-party transaction, all items of the previous
transaction must be deleted.


4.3. Reworking by the background process INTAUF
When the background process INTAUF receives a task from the central office for completion of
the declaration of performance, then all items in the corresponding order are checked again and
the declarations of performance sent by the central office are used. If the assignment was
successful and the clear company-wide declaration of performance was taken over into the
transaction, then the temporarily-assigned numeric ID is set to 0 once again. After that, the order
item can also be changed again.


4.4. Distribution of the data in the other companies
After the generation of a declaration of performance for one thus-unknown structure, the
structure counts as recognized and the data is available immediately both in the central office as
well as in the commissioning company. So that the data is also made known to all other
companies (and also for the case that the access to the third-party database was not successful



A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                                41
during writing back of the data), a key replication must be configured for the appropriate tables.
(xledesc, kprodkeylezu, xlesprzu).


4.5. Manual reworking
On the menu element "Transaction change" from the empty dialog, you can use Ctrl + F10 using
the stored ADHOC-SQL No.84 to obtain all orders from a particular delivery date for which at least
one item is present with a declaration of performance-relevant item but without valid declaration
of performance. These can be placed manually in front of the background process. However here
there is no check whether for this structure a declaration of performance was already transferred
from the central office.


4.6. Configuration
DOP_ZENTRALE = company number where declaration of performance for all sites is entered.
DOP_ZENTRALE_MANR = employee who is informed via e-mail that a declaration of performance
is required.
CHECK_DOP_ANGEBOT : if declaration of performance should also be tested for quotations.
MeldID 82 is responsible for the mail information about required declaration of performance and
can also be configured for special groups.
Deliver altab/alfield from AWE6 (xledesc, xlesprzu, kprodkeylezu)
Heed documentation about key replication.
\\jupiter\DOKU_DocuWare\ALCIB-PMS\DFUE\Replikation\Schluessel_Replikation_DE.doc


Check DB access cross via central-local DB.
select * from alcib_<hauptmandant>@<informixserver>:alcibversion.


hauptmandant and informixserver are on-site in the table xhaus.


KAUF/mfo/kauf.neu.mfo
Current fx_texte/errmsg.


         Availability
Central management of the declaration of performance is used starting with A+W Enterprise
Version 5.4.




A+W Software GmbH                EN-CONFIG-A+W Enterprise DOP.docx                               42
5. A+W CR DoP form
With adjustment of the technical values and changing of the DIN requirements, the DoP forms
should also be checked before start-up of the new functions. The data procurement in the course
of the A+W CR form for the DoP must then be adjusted accordingly. Only after that are the new
fields on the CR DoP visible.




A+W Software GmbH               EN-CONFIG-A+W Enterprise DOP.docx                            43
6. Setting declaration of performance
  "invalid"

If it is necessary to set a declaration of performance invalid due to changed values, this can be
done as follows:
With the menu element Keys -> Products -> Technical Values -> Declaration of Performance
(documents), you start the familiar dialog for document assignment. If it is known which
declaration of performance should be deactivated, then you enter it in the "number" field or
select it using the search function (F9). The description of the purpose, etc. are loaded into the
dialog. In addition, the keys (product structure keys) of the declaration of performance are
retrieved. If this key is not unique, then a "*" is displayed in the field.
On the lower part of the dialog, the new "Invalid" button is now displayed. Use this button or the
key combination SHIFT+F9 to load the data for the declaration of performance into a separate
dialog. On this dialog, you can mark individual declarations of performance for deactivation. With
<START> or the "Invalid" button, the marked data is then deactivated irrevocably. This happens by
changing the coded product key, so that starting from the time in the document entry for this
structure, the declaration of performance will no longer be found.
If several declarations of performance become invalid, because the technical properties of a glass
have changed, for example, you can find these by pressing the "Invalid" button in an empty
"Number" field or pressing CTRL+F9. Then there is an inquiry for an article number that can occur
in the encoding. If you enter 350005 in the field, for example, then all declarations of
performance are listed where the article 350005 exists either as header or as BOM element in the
key. The prerequisite for this is the encryption of the product for the declaration of performance
via article numbers.
The deactivation is also logged in the table "leablaufprot". Here, the product key and old key
coding are also noted.
The declaration of performance is therefore not deletec, just "deactivated". This is necessary so
that the old declaration of performance still applies for the existing documents. For newly entered
documents, no declaration of performance will be found through the encoding until a new one is
stored. If a document with reference is entered and it is determined that the existing declaration
of performance no longer applies and there is no new one, this will be deleted from the item. If an
old document is loaded for correction and it is determined that a new declaration of performance
has been stored, then the user is asked whether this should also be retrieved. Whether or not the
question is asked can be configured with the environment variables "CHECK_DOP_CURRENT". The
old declaration of performance is retained by default.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise DOP.docx                                  44
7. Environment variables
CHECK_DOP_CURRENT (client reference: no)
Activates the question whether a current declaration of performance should be changed in case
of order change.




A+W Software GmbH              EN-CONFIG-A+W Enterprise DOP.docx                            45
A+W Software GmbH   EN-CONFIG-A+W Enterprise DOP.docx   46

