---
title: "EN CONFIG A+W Enterprise BMECat Import"
category: "configuration"
product: "A+W Enterprise BMECat Import"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W Enterprise BMECat Import"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration Instructions   A+W Enterprise BMECat Import                                                                           english        A+W Software GmbH                                          - -INTERNAL-                        EN-CONFIG-A+W Enterprise BMECat Import.docx    1 Change history             Date          Author                 Remarks                                  Version           2019-02-06    Original version       Transfer from Dokuware document"
source_file: "EN-CONFIG-A+W Enterprise BMECat Import.pdf"
---


# EN CONFIG A+W Enterprise BMECat Import

         Configuration Instructions


A+W Enterprise BMECat Import




                                                                      english




   A+W Software GmbH                                          - -INTERNAL-
                       EN-CONFIG-A+W Enterprise BMECat Import.docx    1
Change history


          Date          Author                 Remarks                                  Version
          2019-02-06    Original version       Transfer from Dokuware document          1.0
          2019-03-04    SVH                    Supplier color assignment
          2020-12-11    SVH                    Operation - general information
          2022-06-21    SVH                    Troubleshooting
                                               [AW-134493] - Troubleshooting –
          2023-01-26    SVH                    doubled mandatory ID records, missing
                                               article prices (net_customer)
                                               [AW-145523] – Troubleshooting –
          2023-05-16    SVH
                                               missing standard supplier
                                               Redesign of/addition to the
          2023-11-30    SVH
                                               documentation
          2025-07-01    IS                     General reworking/new Import dialog




Content

1.   General Information                                                                      4
     1.1. Initial development                                                                 4
2.   Installation                                                                              5
     2.1. Additional components                                                                5
          2.1.1. Microsoft Visual J# Redistributable Package version 2.0 in the Setup          5
     2.2. Licensing                                                                            5
          2.2.1. License Client                                                                6
     2.3. Version compatibility                                                                6
          2.3.1. BMECat Import 2011 (3.6)                                                      6
          2.3.2. BMECat Import 5.5                                                             7
     2.4. DB update                                                                            7
3.   Configuration                                                                             8
     3.1. Master data replication                                                              8
     3.2. Supported imports (suppliers)                                                        8
     3.3. Config tool / config file                                                            9
     3.4. Master data                                                                          9
          3.4.1. Supplier                                                                      9
          3.4.2. Sample articles                                                              10
          3.4.3. Price list                                                                   10
     3.5. Special configurations in A+W Enterprise                                            10
          3.5.1. Compatibility settings                                                       11
     3.6. A+W Enterprise environment variables                                                12
4.   Tables                                                                                   13

A+W Software GmbH            EN-CONFIG-A+W Enterprise BMECat Import.docx                           2
5.   Operation                                                                         14
     5.1. General                                                                      14
     5.2. Login dialog                                                                 14
     5.3. Import dialog                                                                14
          5.3.1. Language                                                              14
          5.3.2. Start                                                                 14
          5.3.3. Import Settings                                                       14
          5.3.4. Supplier Settings                                                     15
          5.3.5. Data Source                                                           15
          5.3.6. Article Table                                                         15
6.   Functions                                                                         16
     6.1. Process overview                                                             16
     6.2. Quantity Unit                                                                17
     6.3. Article prefix / determination of the A+W Enterprise article number          17
           6.3.1. Dorma                                                                17
           6.3.2. Pauli                                                                18
           6.3.3. KL-Megla                                                             18
     6.4. Determination of the A+W Enterprise color number (FarbOffset)                19
           6.4.1. Dorma                                                                19
           6.4.2. Pauli                                                                19
           6.4.3. KL-Megla                                                             19
           6.4.4. WWS                                                                  19
           6.4.5. SWS                                                                  20
           6.4.6. Provitris/Gral                                                       20
           6.4.7. General                                                              20
     6.5. Article names                                                                21
     6.6. Size restrictions                                                            21
     6.7. Compulsory dimensions                                                        21
     6.8. Prices                                                                       21
     6.9. Loading and saving an article in AWE (AlcibArticle.BmeCatStoreArticle())     22
     6.10. Gral master data import (AWDesk #409001)                                    23
     6.11. Assignment: article - suppliers                                             23
7.   Troubleshooting                                                                   24
     7.1. KL-Megla master data import                                                  24
     7.2. Logging                                                                      24
     7.3. No IBM Informix directory                                                    25
     7.4. No supplier found                                                            25
     7.5. Missing switches/configuration                                               26
     7.6. Incorrect format in the import file                                          26
     7.7. Exception when establishing the DB connection                                26
     7.8. Error during import of the article data                                      27
           7.8.1. Multiple suppliers have articles in the same article number range.   27
     7.9. Exception / NULLReference in article update                                  27
     7.10. Missing article prices                                                      28




A+W Software GmbH          EN-CONFIG-A+W Enterprise BMECat Import.docx                      3
1. General Information
The BMECat master data import is an application for the import of supplier article master data
from suppliers into the AWE customer system. Among other things, the import of articles from
the suppliers Dorma, Schlechtendahl, and KL-Megla is already implemented.
Up to Version ALCIB 2008, the BMECat master data import required the CommonBase in order to
read out configuration data.
Starting with Version 3.5 (ALCIB 2009), no more CommonBase is required.
Starting with Version 3.6 (ALCIB 2011), the BMECat master data import was converted to the new
dimensioning tables artvermass, artvermassspr, artpreiseig. During DB access, the settings from
CLIENT_LOCALE and DB_LOCALE are considered.
This document was created within the framework AWDesk #206297 with Version 2009.


1.1. Initial development
The master data transfer was developed with AWDesk #103253.
For this, there are documents under \\jupiter\Doku_DocuWare\AWEnterprise\B2B_DORMA.




A+W Software GmbH          EN-CONFIG-A+W Enterprise BMECat Import.docx                           4
2. Installation
Installation is done using the Setup Launcher. For detailed information, please see the installation
document.
In versions <=5.5, the configuration of the DB connection must be stored by hand in the config file
(status as of 07/08/2014). Starting with Version 6, there is a complete config tool available.


2.1. Additional components
The BMECat master data import requires the Microsoft Visual J# Redistributable Package Version
2.0 (must be downloaded and installed if necessary).
If this installation is missing, you will receive the following error message:




        2.1.1.      Microsoft Visual J# Redistributable Package version
            2.0 in the Setup
Starting with Version 5.4, the package is installed by the SetupLauncher during setup installation.
See also AWDesk #219225


2.2. Licensing
In order to be able to use the BMECat import, a LicenseClient must be installed on the computer
on which the import is installed. This happens completely normally via the SetupLauncher. For the
configuration of the LicenseClient, you must know what server's name is on which the
LicenseServer is installed.
If you also install the LicenseMonitor, you can use the monitor to see which licenses are currently
present.
For the master data import, a license of the following type is needed:
Application: AWB2B (900)
Edition: Standard



A+W Software GmbH            EN-CONFIG-A+W Enterprise BMECat Import.docx                              5
Version: 2012
"BusinessArea" and "Modules" are different depending on the supplier. For the Dorma import,
you need "BusinessArea: Dorma" and "Module 2: Dorma master data [...]" (see also screenshot)
If a license is not yet present, you must request it (the person who is responsible for creating
licenses changes from time to time, please ask Frank Agel).
A particular file must probably be installed on the license server.




        2.2.1.          License Client
In the config tool of the License Client (machine), which is installed on the same computer as the
BMECat import, the IP of a License Server is stored. On the next dialog, you must also specify the
correct site for which the License Client should query the licenses. (See also AWDesk #424092)
Using the License Monitor, you can check for which sites which licenses exist.


2.3. Version compatibility
With ALCIB 2009 (4.4), the setup "ALCIB 2009 BMECat Import" (3.5) must be executed.
With ALCIB 20011 (4.5), the setup "ALCIB 2011 BMECat Import" (3.6) must be executed.


        2.3.1.          BMECat Import 2011 (3.6)
The BMECat Import 2011 is not compatible with an AWE database 2009 (or older), since with
Version 2011 the conversion to the table artvermass was made.


A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                              6
        2.3.2.         BMECat Import 5.5
The BMECat Import 5.5 is not compatible with an AWE database 2011 (or older) since with
Version 5.5 in the table lieffarbzu the field "fabnr" was renamed "farbnr".


2.4. DB update
The content of the tables aldfuectrl and aldfuetyp is delivered automatically to the customer
during installation.
In order to be able to perform the configuration, the tables aldfuetyp and aldfuectrl must be up-
to-date. In the versions ALCIB 2009 and ALCIB 2011, therefore, the entries must be added by
hand.
CAUTION:
Very important: In aldfuectrl, idtyp for id=24 must be checked. idtyp must be 3! Perform update if
necessary: "update aldfuectrl set idtyp=3 where id=24“ (#255047)




A+W Software GmbH          EN-CONFIG-A+W Enterprise BMECat Import.docx                              7
3. Configuration
3.1. Master data replication
If the BMECat import is used in connection with a master data replication, it must be checked in
advance whether all components (articles, colors, market partners, prices) will be replicated or
whether restrictions must be heeded here.
       The customer 11 uses the import and article replication. Unfortunately, the color numbers in the
       companies connected by the replication do not match, so that colors may not be replicated
       automatically, but rather must be adjusted manually at the sites.
       See AWDesk #318773




3.2. Supported imports (suppliers)
The import of the following master data is supported:
       No.   Name                 EDI type in         Developed      Starting     License
                                  AWE                 with           with
                                  configuration       AWDesk         AWE
                                                                     Version
       1     Dorma                106                                < 3.6        Application:
                                                                     (2011)       AWB2B (900)
                                                                                  BusinessArea:
                                                                                  Dorma
                                                                                  Modules: ?
       2     Schlechtendahl       107                                < 3.6        Application:
                                                                     (2011)       AWB2B (900)
                                                                                  BusinessArea:
                                                                                  Schlechtendahl
                                                                                  Modules: ?
       3     KL-Megla             108                                < 3.6        Application:
                                                                     (2011)       AWB2B (900)
                                                                                  BusinessArea: KL-
                                                                                  Megla
                                                                                  Modules: ?
       4     Pauli                111                 #297517        3.6          Application:
                                                                     (2011)       AWB2B (900)
                                                                                  BusinessArea:
                                                                                  Pauli
                                                                                  Modules: 8


A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                                   8
       5      Provitris (Dorma    112                #297424        3.6         Application:
              branch)                                               (2011)      AWB2B (900)
              (#409001 – now                                                    BusinessArea:
              Gral)                                                             Provitris
                                                                                Modules: 9
       6      SWS                 113                #296013        3.6         Application:
                                                                    (2011)      AWB2B (900)
                                                                                BusinessArea: SWS
                                                                                Modules: 10
       7      Willach             114
                                  Note: the
                                  supplier Willach
                                  can be
                                  configured on
                                  the AWE side,
                                  in the BMECat,
                                  however, the
                                  import is not
                                  implemented
                                  for want of
                                  request. (Status
                                  as of
                                  07/14/2025)




3.3. Config tool / config file
Starting with Version 5.5, the BMECat import has a config tool.
(AWDesk #323739)
Starting with Version 6.0, the DB settings are maintained via the config tool and when starting the
BMECat import, are taken over completely into the login dialog.
During the update of the BMECat, the settings maintained via the config tool are retained.


3.4. Master data
If in the other documentation, the simplified talk is of "mpfduectrl", this refers to the "System >
Data Transfer > Document Transfer > Configuration" dialog.


        3.4.1.          Supplier
In the A+W Enterprise market partner master data, one supplier per interface must be created.
Which supplier is used for which interface is defined via the default supplier of the sample article
(mpdfuectrl ID 15).


A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                                9
        3.4.2.            Sample articles
In the A+W Enterprise article master data, one sample article per interface must be created.
Important data that must be maintained:
    -   Article type = part
    -   Art. type = 830 – hardware part
    -   Misc. article = no
    -   Color/size variant: Colors/variables
    -   Sale item = yes
    -   Procurement = stock and/or PO
    -   Default supplier - appropriate supplier from the A+W market partner master data
    -   Pricing method 31 PCd color articles"
This sample article is stored on the Configuration dialog "System > Data Transfer > Document
Transfer > Configuration" per supplier (=dfuetyp => see section "Supported imports (suppliers)")
in the ID 15.


        3.4.3.            Price list
Within the import, supplier-specific prices are supplied. These are inserted into the A+W
Enterprise price master data. For this, it is required that a price list (PLCD) be created and then
assigned to the respective supplier/interface via the configuration (System > Data Transfer >
Document Transfer > Configuration ID 26 dialog). The prices are not saved in supplier-specific
prices, but rather in the general color-dependent prices.


3.5. Special configurations in A+W Enterprise
On the dialog System > Data Transfer > Transaction Transfer > Configuration, all settings are
stored that were previously stored in the CommonBase.
For the article master data import, partner type "supplier" and market partner "" (empty) must be
selected.
In the field "Type of the EDI", the master data type is specified (see also section "Supported
imports (suppliers)":
        1. Dorma (EDI type 106)
        2. Schlechtendahl (EDI type 107)
        3. KL-Megla (EDI type 108)
        4. Pauli (EDI type 111)
        5. Provitris/Gral (EDI type 112) -> Dorma-Ableger (AWDesk #409001)
        6. SWS (EDI type 113)




A+W Software GmbH             EN-CONFIG-A+W Enterprise BMECat Import.docx                             10
All control types must then be specified for the desired EDI type. If a setting is missing, the import
reports this at the start and the import cannot be executed.
         aldfuectrl ID        Data type              Description
         14                   num.                   color offset
         15                   num.                   default product number / sample article
         18                   num.                   import short product description
                                                     Only effective for article update, not for new
                                                     articles
         19                   num.                   import long product description
                                                     Only effective for article update, not for new
                                                     articles
         20                   num.                   import pictures (currently not implemented)
         24                   alphanum. (case        prefix imported products
                              255047)
         26                   num.                   price list (PLCD) / Preisliste (PLKZ)
         27                   alphanum.              picture path (currently not implemented)




        3.5.1.           Compatibility settings
Some switches that were previously configurable in the CommonBase were stored in this BMECat
version in the program code. The existing configuration settings are not evaluated and therefore
do not need to be set.



A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                             11
        aldfuectrl ID         Data type         Description            Fixed value
        13                    alphanum.         catalog type           "FIT"
        16                    alphanum.         division               "GLAS"
        17                    alphanum.         file type BMECat       "BMECAT"
        21                    alphanum.         keyword picture        "PICTURES"
                                                transmission
        22                    alphanum.         language of product    "de"
                                                master data (country
                                                code)




3.6. A+W Enterprise environment variables
The alenv variable ARTIKELBILD_PFAD can be assigned.




A+W Software GmbH        EN-CONFIG-A+W Enterprise BMECat Import.docx                 12
4. Tables
The following tables are manipulated by the import:
artikel
musskenn
defformel
artpiczu
arttxtzu
strukt
infoart
modparam
pposzu
pstrukt
artvarzu
prsvek
nsteuer
artvermass
artvermassspr
artpreiseig
artbezfremd
xxfarbe
xsprbez
artliefzu
artfarbzu
lieffarbzu
pkzfarb
artrepsteuer




A+W Software GmbH         EN-CONFIG-A+W Enterprise BMECat Import.docx   13
5. Operation
5.1. General
In order to be able to execute the BMECat import, in principle, no exclusive access to the
database is required. The article master data can also be used by other users during the import.
However, there is an interruption of the entire import as soon as a user has entered item master
data during the import, which is within the number range of the article to be imported (see also
chapter on article prefix).
In simpler terms: when starting the import, you have to ensure that the article master data (also
the extended data such as colors and prices) of the supplier to be imported will not be entered for
the duration of the import in A+W Enterprise.


5.2. Login dialog
For each call of the BMECat import, the data is taken over from the configuration (see "EN-INST-
A+W Enterprise BMECat Import").


5.3. Import dialog
        5.3.1.           Language
In which language the dialog opens is defined by the Windows language. If a language is not
supported, Entglish is selected.


        5.3.2.           Start
At the start of the BMECat import, a series of checks are executed. If one of these checks fails, this
is depicted highlighted in red on the top part of the dialog (see section "Troubleshooting").


        5.3.3.           Import Settings
In the "Import settings" dialog area, the supplier of the import file can be selected. All suppliers
that are stored correctly in A+W Enterprise on the "System > Data Transfer > Document Transfer >
Configuration" dialog are available for selection.
Settings on the right side are:
"Delete Variants & Deactivate Articles“: Color variants that are no longer included in the
interface file for an article are removed from the article-color assignment (table "artfarbzu") and
from the prices (table "pkzfarb"). If an existing article is not completely included in the interface
file, then the article is discontinued. Included variants are kept. Since this behavior corresponds to
the earlier behavior, this option is active by default.
Caution: This can cause problems in the stock and in existing documents.


A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                            14
If the option is not selected, then the variants (table artfarbzu, pkzfarb) that do not occur in the
file are not deleted. Articles that are not completely included in the file remain active (still: 0).
"Global Commit": If this option is selected, the import of an entire file is executed in a big
transaction. This means that all or no articles are imported. If the option is not selected, each
article including all variants and prices will be scheduled in a single transaction. This can cause a
file to be imported in part.


5.3.4. Supplier Settings
In the "Supplier Settings" section, the configured values of the supplier selected in "Import
Settings" are displayed. These include the Muster-Artikel (Sample Article), the Preisliste (Price
List), of the article Prefix, the Farb-Offset (Color Offset), takeover of the Langbezeichnung (Import
Long Description) and takeover of the Kurzbezeichnung (Import short Description). These values
serve instead of the control and cannot be changed on this dialog.



5.3.5. Data Source
In the "Data Source" section, you can use the "Choose file" button to select the interface file to be
read in. The default directory for this can be defined in the config tool.


5.3.6. Article Table
With the "Read file" button, the file selected in the "Data source" section is read in and the result
displayed in the table.
The initial feasibility checks are done here. If this is a file-global error, on first occurrence, this is
highlighted in red in the top dialog area, and further importing is canceled. If it is a variant-specific
error, the corresponding line is marked with the status "error". The error is described in more
detail in the "Error" column.
If an error occurs, the import of the file is not possible.
see also section „Troubleshooting“


With the "Import to database" button, the data from the "Article table" is processed and saved in
the A+W Enterprise database. The "Status" column provides information about the progress of
the processing.
The Status colum can contain the following values:
Error – The article/variant contains an error. Please check the "Error" column
Processing – The article/variant is being processed now
New – This article/variant is new
Update – This article/variant was changed




A+W Software GmbH            EN-CONFIG-A+W Enterprise BMECat Import.docx                                15
6. Functions
6.1. Process overview
With the "Read file" button, the file selected in section "Data Source" is read in and the result
displayed in the table "Article Table".
If the reading in proceeds without errors, you can start the import by clicking the "Import to
database" button.
During the import, the progress is displayed in the Status column.
With the "Cancel Import" button, you can stop the "Import to database". How things will proceed
with the articles already imported is decided with the "Global Commit" option from the section
"Import Settings".
If the import was executed successfully, this is displayed in green on the upper edge.




In the specified log file, you can check which status an imported article has the whether there was
a price change. For more details about the log, see section "Troubleshooting > Logging"




If an error occurs during the import, you can use the "Global Commit" option from the section
"Import Settings" to decide what to do with already imported data.




A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                             16
6.2. Quantity Unit
In the interface, the quantity unit "MTR" is sent for meters. During import into A+W Enterprise,
this is taken over as quantity unit 3 - "mm", however. The weight must be converted accordingly.
There is no conversion of the dimension restrictions (min_length and max_length). Similarly, there
is no conversion of the price since in A+W Enterprise, for GME = mm, the price is expected as per
meter.


6.3. Article prefix / determination of the A+W
   Enterprise article number
AWDesk #255047
How a supplier article number becomes an A+W Enterprise article number depends on the
supplier.
It is hard-coded in the source code at which place in the imported element <SUPPLIER_AID> the
ColorID begins.
In the first step, it is checked whether the customer article number from the transfer file
(<SUPPLIER_AID>) includes the color code. The color code is then separated from the customer
article number.
It is hard-coded in the source code at which place in the imported element <SUPPLIER_AID>
(customer article number) the ColorID begins.
If the external article number is shorter than the maximum AWE article number length (8 places)
minus the prefix length, then the places between prefix and external article number are filled with
zeroes.


        6.3.1.          Dorma
For Dorma, this is the 7th place; that means, the first 6 places are interpreted as article number.
During the scheduling of Dorma files, 6 characters are cut off from the front of the Dorma article
number and the 2-digit prefix from the configuration (mpdfuectrl ID 24) is attached to the front. It
must be heeded that with the "Dorma" interface, the prefix is specified with a maximum of 2
digits and numerically; otherwise, parts of the Dorma article number are lost.


1.Example:
Dorma article number: 876543, Prefix 08
=> A+W Enterprise article number = 08 + 123456.Substring(6 - (8 -2)) = 8123456, that is, all 6
digits of the Dorma article number are used


2.Example:
Dorma article number: 123456, Prefix 088




A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                           17
=> AWE article number = 088 + 123456.Substring(6 - (8 -3)) = 088 + 123456.Substring(1) =
8823456, now the FIRST! of the 6 places of the Dorma article number are ignored and overwritten
by the prefix.
By contrast, for
Dorma article number: 123456, prefix 88 (without leading 0)
=> AWE article number = 88 + 123456.Substring(6 - (8 -3)) = 88 + 123456.Substring(1) =
88123456, now the FIRST! of the 6 digits of the Dorma article number are taken over.



        6.3.2.           Pauli
For Pauli, all places are interpreted as article number.
The A+W Enterprise article number is determined depending on the maximum length of the
article number in A+W Enterprise (hard-coded 8) and the length of the article prefix.
During the scheduling of Pauli files, the prefix from the configuration (mpdfuectrl ID 24) followed
by "000000" is used as start value for the article creation. The last article is then <Prefix>999999.
It must be heeded that with the "Pauli" interface, the prefix is specified with a maximum of 2
digits and numerically.
Example:
Pauli article number 54321, prefix 110
=> A+W Enterprise article number = 110 + 54321.Substring = 11054321


PF [AW-98452].
During the import of the manufacturers Pauli and Sohn, a new article number was created during
each import. This behavior has been corrected. Starting now, the article number is searched for
using the field "artbez2" in the table "artikel". If nothing is found here, a new article is created.
This field will not be filled for long, so that when updating (if the field was not yet filled), this
behavior can still happen. If the field is filled, the article is updated and no new article is created.


        6.3.3.           KL-Megla
For KL-Megla, this is the 6th place; that means, the first 5 places are interpreted as article
number.
KL-Megla article number: 54321, Prefix 087
=> A+W Enterprise article number = 087 + 54321.Substring(5 - (8 -3)) = 8754321, that is, all 5
digits of the KL-Megla article number are used.
See AWDesk #255047.




A+W Software GmbH            EN-CONFIG-A+W Enterprise BMECat Import.docx                              18
6.4. Determination of the A+W Enterprise color
   number (FarbOffset)
AWDesk #297424 // AWDesk #274960
The original logic for determination of a new A+W Enterprise color number, is based on the fact
that there is initially an attempt to take over the supplier color number as A+W Enterprise color
number. This logic has proven unsustainable, after gradually other hardware manufacturers were
integrated, some of whom transfer 5-digit color numbers or alphanumeric IDs.
The determination of the supplier color ID of an article depends on the supplier. If different
suppliers are imported, each supplier should be assigned its own color number range
(ColoreOffset - (mpdfuectrl ID 14)), so that colors are not overwritten. Attention must be paid that
the color numbers in A+W Enterprise can be a maximum of 4 digits.
Hard-coded is a limit of 999, so that an offset of 4000 produces a number range of 4000 – 4999,
for example. This should be considered when assigning the offset for different suppliers.
The supplier color number is saved as reference in lieffarbzu.


        6.4.1.           Dorma
The ColorOffset (mpdfuectrl ID 14) must absolutely be 4-digit. The A+W Enterprise color number
is formed from <ColorOffset> + color number from the interface.
If the ColorOffset is not 4-digit, the supplier is not made available for the scheduling.
Hard-coded is a limit of 999, so that an offset of 4000 produces a number range of 4000 – 4999,
for example.


        6.4.2.           Pauli
Starting from the ColorOffset, the next free number is assigned. If the offset is zero, the color
number 1 is the beginning.


        6.4.3.           KL-Megla
For KL-Megla, the ColorID is transferred in a <Feature>-Element (the ColorID is also an attachment
in the <SUPPLIER_AID> element.
The ColorOffset (mpdfuectrl ID 14) must absolutely be 4-digit. The A+W Enterprise color number
is formed from <ColorOffset> + color number from the interface.
If the ColorOffset is not 4-digit, the supplier is not made available for the scheduling.
Hard-coded is a limit of 999, so that an offset of 4000 produces a number range of 4000 – 4999,
for example.


        6.4.4.           WWS
The ColorOffset (mpdfuectrl ID 14) must absolutely be 4-digit. The A+W Enterprise color number
is formed from <ColorOffset> + color number from the interface.


A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                             19
If the ColorOffset is not 4-digit, the supplier is not made available for the scheduling.
Hard-coded is a limit of 999, so that an offset of 4000 produces a number range of 4000 – 4999,
for example.


        6.4.5.            SWS
Starting from the ColorOffset, the next free number is assigned. If the offset is zero, the color
number 1 is the beginning.


        6.4.6.            Provitris/Gral
Starting from the ColorOffset, the next free number is assigned. If the offset is zero, the color
number 1 is the beginning.



        6.4.7.            General
The colors of all articles to be imported are collected in a hash table.
During the update/insert for an article, first all entries in pkzfarb for article, price list (defined via
mpdfuectrl) and artfarbzu are deleted.
Then the A+W Enterprise ColorID is determined:
•   first it is checked in lieffarbzu whether for the supplier and the current supplier ColorID
    (lifarbnr) a record exists; if so, the associated AWE ColorID is taken over
•   if there is no AWE ColorID, a new AWE ColorID must be found
-   first it is checked whether the supplier ColorID exists as AWE ColorID in xxfarbe; if it does not
    exist, it will be taken over one-for-one as AWE ColorID
-   if the ID in xxfarbe already exists, the offset (configuration mpdfuectrl ID 14) is added to the
    supplier ColorID and it is checked whether the resulting number exists in xxfarbe; if it does
    not exist, it is used
-   if the ID already exists in xxfarbe, the offset (configuration mpdfuectrl ID 14) is used as basis
    and incremented until a number is reached that does not yet exist in xxfarbe (here, there is
    the limit offset + 999 for the color number)
For a newly determined AWE ColorID, an insert is made in xxfarbe and lieffarbzu for the current
color.
Then the entries in artfarbzu and pkzfarb are updated.


Supplier color assignment dialog
During the import of a new supplier master data file, it is checked using the corresponding table
lieffarbzu whether or not the colors of an item to be imported are already created in AWE as AWE
colors.
If it is detected that a supplier color is not yet created as AWE color, it is created during the
import.


A+W Software GmbH             EN-CONFIG-A+W Enterprise BMECat Import.docx                                20
In the ideal case, the table lieffarbzu is not manipulated by a user, but rather by the import logic.
The dialog then delivers the overview of all created supplier colors to the user.
It can also happen that a color is needed for an order for a supplier that is not yet created in
lieffarbzu because after the last supplier master data import from the supplier, new colors were
made available.
Then the new supplier color can be created manually via the dialog in order to enter the order.


6.5. Article names
Within the configuration, it can be specified whether the short description (short description,
mpdfuectrl ID 18) and/or the long description (long description, mpffuectrl ID 19) should be taken
over. Here, the "short description" in A+W Enterprise corresponds to the article main description
and the "long description" depending on length to the long description 1 to 3
If a new article (not variant) is imported, both descriptions are always imported, regardless of the
configuration.
If an existing article is imported (update), then only the configured description is
imported/overwritten.


6.6. Size restrictions
If in the interface a "min_length" and "max_length" are sent, then these values are entered in the
dimension restriction maximum width and minimum width.
Caution: If variants with different dimension restrictions are sent to the interface, the last variant
wins. There are no variant-specific dimension restrictions in A+W Enterprise.


6.7. Compulsory dimensions
If in the interface a "min_length" and "max_length" are sent, then a record in the compulsory
dimensions with the name "width" and the local language is generated from alsysinfo. If
"min_length" and "max_length" are identical, the identifier "Entry" is set to "No". If the limit
dimensions are different, the identifier is set to "Yes" and the minimum value is entered as
default value.
Caution: If variants with different dimension restrictions are sent to the interface, the last variant
wins. There are no variant-specific compulsory dimensions in A+W Enterprise.




6.8. Prices
Within the interface, one price is sent per variant A price <= 0 causes an error even during the
import of the data ("Read file") and the file cannot be imported.




A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                             21
If a correct price is sent, then this price is entered both in the article color assignment (Master
data - Article - F4 - Color/sizes, table artfarbzu) asd well as in the color-dependent prices (Master
data - Prices - PCd prices - Colorted articles, table pkzfarb). The entry is made in both places since
in A+W Enterprise it is possible to define where the price calculation determines the prices.
If a variant is imported for correction (update), it is first checked whether the price in the
interface file differs from the price in the article-color assignment and then, whether it differs in
PCd prices - Colored articles. The display in the import log primarily shows the deviation in the
PCd prices. If there is no deviation present in the article-color assignment, then this is displayed.




6.9. Loading and saving an article                                                   in       AWE
   (AlcibArticle.BmeCatStoreArticle())
For the suppliers Dorma, KLMegla, and Provitris/Gral, the AWE article that must be loaded is
determined directly from the supplier article number.
For the suppliers Pauli and WSS, the AWE article is determined via the detour of the table
artfarbzu (for this, first the supplier number from the sample article must be selected) since the
AWE article number cannot be derived directly from the supplier article number.
If no AWE article can be found, the sample article is loaded.




A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                              22
6.10.           Gral master data import (AWDesk #409001)
Provitris was sold to "Gral Systeme GmbH“, for this reason the query of the manufacturer name in
the article file and all naming in the BMECat import and in the configuration in the AWE Backend
was adjusted accordingly.


6.11.           Assignment: article - suppliers
The assignment of articles to suppliers (artliefzu) now has the manufacturer number of the basic
article for all manufacturers (without color marking). Previously, the first color variant was
entered in this field.
The assignment of articles to suppliers (artliefzu) now has no more price since it almost always
refers to a color variant. Previously, the price of the first color variant was entered here.
See PF [AW-98452].




A+W Software GmbH          EN-CONFIG-A+W Enterprise BMECat Import.docx                             23
7. Troubleshooting
Starting in July 2025
Error messages are displayed on the top part of the import dialog. Here, some messages and their
cause are documented. The text of the message can differ in detail (especially during translation).


7.1. KL-Megla master data import
During import of the master data (price list 2014), somebody noticed that approx. 700 articles
(which allegedly belong to the standard program) are not present in the list. As a result, these
articles are ignored during import.
See AWDesk #318773


7.2. Logging
The A+W uniform tracing can be set as usual via the config tool.


In addition, an import log is written in an Excel file. On the first worksheet "Article", this includes
the most important information such as status (updated/new/delete), article and color numbers.




On the second worksheet "New Colors", the colors are listed that were created anew in the color
keys.




The name of the file is displayed in the upper status line of the import dialog as a link.

A+W Software GmbH            EN-CONFIG-A+W Enterprise BMECat Import.docx                             24
7.3. No IBM Informix directory




When starting the BMECat, it is checked whether INFORMIXDIR is set in the setnet32 settings. If
not, a corresponding warning appears. The import works with missing INFORMIXDIR, but special
error messages cannot be output and cause a "NullReferenceException" in the further course of
things.




7.4. No supplier found
Problem:
After the start of the BMECat, the message "No suppliers were found in the database" appears
right away and the drop-down menu for the supplier is empty.


Solution:
For none of the supported suppliers (see section "Supported imports (suppliers)") was a
Configuration stored on the System > Data Transfer > Document Transfer > Configuration dialog.


Problem
"The ID of standard supplier for the article <Sample Article> was not given. …”




Solution:




A+W Software GmbH          EN-CONFIG-A+W Enterprise BMECat Import.docx                         25
In the sample article, no (or a no longer extant) standard supplier is stored. The master data of the
sample article must be adjusted.


7.5. Missing switches/configuration
If a switch/configuration evaluated during master data import is not stored in the configuration
("System > Data Transfer > Document Transfer > Configuration" dialog; table mpdfuectrl), a
corresponding message (with the note that the switch must first be created) is output to the
screen and the master data import cannot be started.


7.6. Incorrect format in the import file
If in the XML file an incorrect format is transferred (e.g., incorrect decimal separator for prices,
not supported currency abbreviation), then the error message "There is an error in XML
document(<line+1>,<column>)" is output, followed by a more precise description of the error.
The import is cancelled with the occurrence of the first format error.




For technical reasons, the transfer of an incorrect currency cannot be output record-specifically as
error (as for incorrect quantity unit, for example); instead, on first occurrence it leads to a format
error.




Attention: The treatment of the price ("PRICE_AMOUNT") is different than the treatment of the
net weight (NetWeight). The net weight is transferred in an "FVALUE" in the "FEATURE". This is
initially an object without specific data type, that's why here (status as of 06/21/2022) both a
comma and a dot are permitted as decimal separator.
See also AWDesk #387865.
openTRANS BMECat interface description in Share Point „A+W Software GmbH\A+W Clarity R&D -
Dokumente\Interfaces\openTRANS\BMECat“




7.7. Exception when establishing the DB connection
When installing a BMECat 2011 with a SetupLauncher Version 5, the AW.IBM.Data.Informix.dll is
not replaced by the IBM.Data.Informix.dll in the installation directory. Therefore, the error
message "Closing exception database type: Informix" appears (The assembly
IBM.Data.Informix.dll must then be copied by hand into the installation directory.)
Furthermore, under some circumstances, the <runtime> entry in the machine.config is missing
(see document \\hausi\bug\A+W_Allgemein\Entwicklung\ALCIB\Develop\ICLIT09B.docx).
See AWDesk #388129

A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                                26
It is conceivable that other BMECat import setup/SetupLauncher combinations can cause such
problems.
During the installation with the appropriate SetupLauncher 2011, the problems probably will not
occur.




7.8. Error during import of the article data
        7.8.1.   Multiple suppliers have articles in the same article
            number range.




In the number range defined by "article prefix", there are articles that have a different default
supplier than suppliers defined via the sample article.
SELECT COUNT(ARTNR) FROM ARTIKEL WHERE ARTNR >= @MIN AND ARTNR <= @MAX AND STILL
= 0 AND STDLINR != @LINR"




7.9. Exception / NULLReference in article update
During import, the following error message appears:




"NullReferenceException: the object reference has not been specified for an object instance."
Cause is the setnet32 setting "use my settings," in which an incorrect "INFORMIXDIR" is stored.
"use my settings" must be deactivated and "INFORMIXDIR" must be checked.
When starting the BMECat, it is already checked whether "INFORMIXDIR" is set, and if not, a
corresponding warning is output.




A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                             27
7.10.           Missing article prices
It must be checked whether in the import file the price in the attribute "net_customer" is
transferred. If "net_list" is used instead, the file must be adjusted. "net_list" must be replaced
with "net_customer". Only this way will the prices be found during import.
Element <ARTICLE_PRICE>:
correct: <ARTICLE_PRICE price_type="net_customer">
incorrect: <ARTICLE_PRICE price_type="net_list">
See also PF [AW-134493], [AW-133248], [AW-133490], [AW-146372], [AW-156201]




A+W Software GmbH           EN-CONFIG-A+W Enterprise BMECat Import.docx                              28

