---
title: "EN CONFIG A+W iQuote"
category: "configuration"
product: "A+W iQuote"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W iQuote"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration Instructions   A+W iQuote v6                                         english                                 - -INTERNAL- Change history   Date       Author         Remarks                                                        Version 2015-01-14 D. Langsdorf   Release version                                                13.0.0 2015-09-01 D. Langsdorf   SN configuration                                               13.0.1 2015-10-05 D. Langsdorf   Print server configuration"
source_file: "EN-CONFIG-A+W iQuote.pdf"
---


# EN CONFIG A+W iQuote

    Configuration Instructions


A+W iQuote v6




                                    english




                            - -INTERNAL-
Change history


Date       Author         Remarks                                                        Version
2015-01-14 D. Langsdorf   Release version                                                13.0.0
2015-09-01 D. Langsdorf   SN configuration                                               13.0.1
2015-10-05 D. Langsdorf   Print server configuration                                     13.0.2
2015-12-14 D. Langwald    Master data consolidation before introduction of iQuote        13.0.3
2015-12-14 D. Langsdorf   Workflow configuration                                         13.0.4
2016-01-14 D. Langsdorf   Reworking                                                      13.0.5
2016-01-18 D. Langsdorf   Decimals of sizes                                              13.0.6
2016-01-28 D. Langsdorf   Activities Model Mapping                                       13.0.7
2016-01-29 D. Langsdorf   Description of article images                                  13.0.8
2016-02-10 D. Langsdorf   Business Case configuration                                    13.0.9
2016-02-12 D. Langsdorf   Production area and document numbers                           13.0.10
2016-02-19 D. Langsdorf   Print Job documentation adjusted                               13.0.11
2016-03-04 D. Langsdorf   Rounded corners parameter values 2.3                           13.0.12
2016-04-15 D. Langsdorf   Correction of business cases                                   13.0.13
2016-06-23 D. Langsdorf   Macro recording configuration 2.12                             13.0.15
2016-09-30 D. Langsdorf   Workflow Properties built-in                                   13.2.1
2016-10-24 D. Langsdorf   Variants of implementation                                     13.2.2
2016-11-29 D. Langsdorf   Exchange groups not for gas 2.4                                13.2.3
2017-01-05 D. Langsdorf   Product release and sorting                                    13.3.1
2017-01-23 D. Langsdorf   Box sales 4.3 + 2.13                                           13.3.2
2017-02-02 D. Langsdorf   Check in workflow 4.4                                          13.3.3
2017-02-17 D. Langsdorf   Self pick-up 4.5 + 2.14                                        13.3.4
2017-02-27 D. Langsdorf   Commission and customer PO number 2.15                         13.3.5
2017-03-22 D.Langsdorf    Restriction of the processings 2.16 + 4.3                      13.3.6
2017-03-30 D. Langsdorf   History for A+W Business documents 2.17 + 2.18                 13.3.7
2017-04-20 D. Langsdorf   Document attachments in history 2.18                           13.4.1
2017-05-02 D. Langsdorf   Report attachments in history 2.19                             13.4.2
2017-07-03 D. Langsdorf   Save the shopping cart and the configuration2.20               13.4.4
                          Total thickness for insulated glass 2.21 + Show IG structure
2017-08-03 D. Langsdorf                                                                  13.4.5
                          2.22
2017-09-26 D. Langsdorf   Addition of property total thickness IGU 2.21 + 4.3            13.4.7
Date       Author         Remarks                                                         Version
2017-10-13 D. Langsdorf   Color selection for products 2.23 + 4.3                         13.4.8
2018-01-10 D. Langsdorf   Filtering of products and ISO exchange 2.24 + 4.7               13.4.1525
2018-07-20 D. Langsdorf   IG replacement with spacer colors 2.26 + 4.3                    13.4.2201
2018-10-22 D. Langsdorf   AutoCollapsible property Workflow Activities 4.6                13.4.2538
2018-10-22 D. Langsdorf   Multilingual Workflow 4.8                                       13.4.2538
2018-11-21 D. Langsdorf   Processing parameters min/max values 2.3.2                      13.4.2538
2018-11-21 D. Langsdorf   New workflow definitions 4.2                                    13.4.2538
2018-12-10 D. Langsdorf   Dynamic values for workflow 4.9                                 13.4.2538
2019-02-26 D. Langsdorf   Color filter and special colors 2.27 + 4.7                      13.4.2705
2020-05-04 D. Langsdorf   Sorting the processing types with filters 2.16                  13.4.3805
2019-05-04 D. Langsdorf   Printout with Crystal Reports 2.9                               13.4.3805
                          2-phase commit with document creation (breaking change)
2020-06-18 D. Langsdorf                                                                   13.4.3924
                          2.6 + 2.28
2020-08-10 D. Langsdorf   File upload and web links 2.29 + 4.3                            13.4.4104
2020-08-11 D. Langsdorf   Access to internal data structures in the workflow 4.10
2020-09-23 D. Langsdorf   Pattern/coating side and side for single glass 2.30 + 4.3       13.4.4263
2020-11-26 D. Langsdorf   Project selection with products 2.31 + 4.4 + 4.7                13.4.4448
2021-01-05 D. Langsdorf   Creation of processings from the workflow 2.32 + 4.7.1          13.4.4499
2021-02-01 S. Weil        Filter by name (single and IG) 2.25                             13.4.4569
                          Set Bestelltext2 for the 3 entry paths (evaluate entry quote)
2021-03-05 D. Langsdorf                                                                   13.4.4569
                          2.33
                          Extension of mapper workflow added, processing with
2021-03-24 D. Langsdorf                                                                   13.4.4670
                          "ActionMapperAddAction" 4.6
2021-06-22 D. Langsdorf   Customer's own icon for the browser 3.3
2021-07-06 D. Langsdorf   Customer's own texts for the user interface 3.4                 13.4.4899
2021-11-22 D. Langsdorf   Product filter for processings 2.34 + 4.7                       13.4.5228
2022-01-11 D. Langsdorf   Suppress credit limit message 2.35                              13.4.5350
2022-01-21 D. Langsdorf   Model filter in the workflow 4.3 + 2.36                         13.4.5357
2022-03-11 D. Langsdorf   Takeover of the CSS customizing possibilities 6                 13.4.5500
2022-05-10 D. Langsdorf   History with exact status release 2.37                          13.4.5596
2022-11-28 D. Langsdorf   Multi-sites and load distribution 2.38                          13.4.7459
                          Product widget by product groups and article numbers from-
2023-07-10 D. Langsdorf                                                                   13.4.9342
                          to 4.3
Date        Author        Remarks                                                   Version
                          Checkbox widget for GTCs and HTML widget designations 2.39
2023-07-28 D. Langsdorf                                                              13.4.9433
                          and 4.5
2023-10-06 D. Langsdorf   Login page configuration 7                                13.4.10144
2024-01-16 J. Nießner     Login Page Okta
2024-01-29 J. Nießner     Okta login page reworked
Content

1.   System Konfiguration                                           8
     1.1. Infrastruktur Konfiguration                               8
     1.2. Geschäftsfall / Business Case Konfiguration              13
2.   Konfiguration                                                 15
     2.1. Kunden Mitarbeiter freischalten                          15
     2.2. Produkte, Modelle und Bearbeitungen freischalten         15
     2.3. Bearbeitungsparameterwerte Einschränkungen               16
           2.3.1. Bearbeitungsparameter Grenzwerte für Rundecken   16
           2.3.2. Bearbeitungsparameter Min-/Maxwerte              17
     2.4. Definition der ISO Austauschgruppen                      18
     2.5. AV-Bereich Zuordnung für iQuote User                     20
     2.6. Statuszuordnung                                          20
     2.7. Statuspunkte freigeben                                   21
     2.8. AV-Bereich Zuordnung und Dokumentennummern               21
     2.9. Ausdruck und Mailversand mit Crystal Reports             22
     2.10. Anzahl Nachkommastellen für Abmessungen                 23
     2.11. Einrichten eines iQuote Benutzers                       23
     2.12. Konfiguration der Makros                                25
     2.13. Einrichten Lagermaße und Kisten                         26
     2.14. Selbstabholung                                          28
     2.15. Kommission und Kundenbestellnummer                      30
     2.16. Einschränkung der Bearbeitungen im Workflow             30
     2.17. Historienanzeige von A+W Business Dokumenten            34
     2.18. Dokumentenanhänge in der Historienanzeige               35
     2.19. Reportanhänge in der Historienanzeige                   36
     2.20. Speichern des Warenkorbs und der akt. Konfiguration     37
     2.21. Gesamtdicke für Isoliergläser und Produktbezeichnung    39
     2.22. Isolierglas Produktbezeichnung 2 aus Aufbau             41
     2.23. Produktfarben für Artikel                               42
     2.24. Produkt- und ISO-Austauschfilter                        45
     2.25. Filter nach Bezeichnung                                 48
     2.26. Abstandhalterfarben im ISO-Austausch                    49
     2.27. Farbfilter und Sonderfarben                             51
     2.28. Zwei Phasen Commit beim Speichern                       52
     2.29. Datei Upload und Weblink                                53
     2.30. Struktur-/Schichtseite und Verlauf                      54
     2.31. Projekte mit zugehörigen Produkten                      55
     2.32. Bearbeitungen per Workflow einfügen                     58
     2.33. Dokumente Kennzeichen pro Erfassungsweg                 61
     2.34. Produktfilter für Bearbeitungen                         62
     2.35. Kreditlimitprüfung unterdrücken                         63
     2.36. Modellfilter für die Geometrieerfassung                 63
     2.37. Historie mit exakter Statusfreigabe                     66
     2.38. Mehrmandantenfähigkeit und Lastverteilung               67
     2.39. Checkbox-Widget und HTML-Bezeichnung                    72
3.   System Konfiguration                                          76
     3.1. Einbindung in eine Startseite                            76


A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx          5
     3.2. Einrichten der Produktbilder                              77
     3.3. Kundeneigenes Logo für den Browser                        78
     3.4. Kunden Texte für die Oberfläche                           79
4.   Workflow                                                       81
     4.1. Workflow Studio                                           81
     4.2. Workflow Management                                       82
           4.2.1. Konfigurator Erweiterungspunkt ( 0000 )           83
           4.2.2. Mapper Erweiterungspunkt ( 0001 )                 83
           4.2.3. Check In Erweiterungspunkt ( 0002 )               83
           4.2.4. Check Out Erweiterungspunkt ( 0003 )              83
           4.2.5. Dokumentvalidierung Erweiterungspunkt ( 0004 )    83
           4.2.6. Add To Cart Erweiterungspunkt ( 0005 )            84
           4.2.7. Backend Update Erweiterungspunkt ( 0006 )         84
     4.3. Activities Konfigurator                                   85
     4.4. Activities Checkin                                        92
     4.5. Activities Checkout                                       93
     4.6. Activities Model Mapping                                  95
     4.7. Activities Methods                                        97
           4.7.1. Bearbeitungen verändern                          101
     4.8. Mehrsprachiger Workflow                                  103
     4.9. Dynamische Werte für den Workflow                        106
     4.10. Zugriff auf die iQuote Datenstrukturen                  108
5.   Stammdaten Konsolidierung                                     110
     5.1. Genaue Produktbezeichnungen                              110
     5.2. Lochbohrungen für unterschiedliche Durchmesser           110
     5.3. Die richtige Kantenbearbeitungen erfassen                111
     5.4. Verwendung von Farbvarianten                             111
     5.5. ESG immer mit vollständiger Stückliste                   111
6.   CSS Customizing                                               112
     6.1. Allgemeines und Grundlegendes                            112
     6.2. Funktionsweise Custom Theme                              114
     6.3. Übersteuern von Regeln und eigene CSS-Regeln             115
     6.4. Hintergrundfarbe im Hauptmenü                            116
     6.5. Farben Navigationsleiste iQuote                          117
     6.6. Farben Navigationsleiste Konfigurator                    117
     6.7. Lade-Icon ändern                                         118
7.   Login Page Konfiguration                                      119
     7.1. Erstlogin als Administrator                              120
     7.2. Seiten                                                   121
     7.3. Benutzer                                                 123
     7.4. Links                                                    124
     7.5. Einstellungen                                            125
     7.6. Benutzer Selbstregistrierung und Passwort Reset          125
     7.7. Customizing der Login Page                               126
          7.7.1. View Layout für Customizing                       126
          7.7.2. Custom Header und Footer                          127
          7.7.3. Hinzufügen einer View im Menu                     127
          7.7.4. Zugriff auf Kundentexte                           128


A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx            6
         7.7.5. Anpassung der Kundenmails                                      128
8.   Login Page Okta Konfiguration                                             129
     8.1. Okta Plattform Konfiguration                                         129
          8.1.1. Anlegen einer Gruppe und Zuweisung eines Mandaten             131
          8.1.2. Anlegen eines Benutzers und Verbindung mit einem ERP-Kunden   132
          8.1.3. Der Standard Kunde                                            134
     8.2. Konfiguration von “A+W iQuote Login Page Okta”                       135
     8.3. Vorbereitung von iQuote für das Okta Login                           137
     8.4. Customization                                                        138




A+W Software GmbH                 EN-CONFIG-A+W iQuote.docx                          7
1. System configuration
1.1. Infrastructure Configuration
Please start the Web interface of the Infrastructure Services.




Now select the Configuration dialog.




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx   8
On the Configuration dialog, the database connection of the A+W Business COM is entered first.




In the A+W Business User area, the logical Business User must be entered.




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                    9
In its number manager, the purchase orders are collected by iQuote
Under Company logo file name, a deviating company logo can be entered. This file must be in the
Context directory. It is suggested that this is organized in a subdirectory. It should contain all
content for the customer.




It must be specified which back end is operated under iQuote. A+W Business or Cantor




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  10
In the Web settings, it is possible to change the appearance of the Website; for iQuote, please
select the "Web" tab.
Advertising file name: The advertising on the left side of iQuote can be filled with several image
files, they are displayed in alternation, the files must be separated with a semicolon (e.g.
"ads1.jpg;ads2.jpg")
Background file name: The background image can be entered here.
Schema: Under schema, you can search for one of the existing ones or select custom if you have
selected an individual one.
Specify schema: If the schema is not specified, then under "Schema" you set the default. This can
be overwritten by the cookie (by other A+W Websites) or via URL (Web.Web/?theme=black).
If you would like to force Website users to use the pre-set theme, you can specify the schema.




The workflow must be determined; to do this, please select the workflow management




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   11
The appropriate workflow must be set




The expansion point 000-iQuote Configurator is the workflow for the display of the widgets and
controls which queries are displayed.
The expansion point 001-iQuote Assignment handles the assignment/mapping of the data
structures of the front end into the back end. Normally nothing must be done here.
The expansion point 002-iQuote Check In handles the display of the widgets before the
configuration process
The expansion point 003-iQuote Check Out handles the display of the widgets after the
configuration process




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                    12
1.2. Business case configuration
The possible functions in iQuote are controlled via business cases. This can be managed in
the infrastructure configuration. The functions can be switched on or off per business
case.




Please start the Web interface for the infrastructure via Configuration>Business case
functions. You can manage the functions there.
The business cases are listed horizontally, this must be entered in the A+W Business
customer employee management. The business cases are fixed and the default for an
employee is "Access declined". It must be heeded that after a change, the IIS must be
started anew, these settings are cached.




A+W Software GmbH                 EN-CONFIG-A+W iQuote.docx                             13
                            Display quotation and order overviews
 Display overviews
                            Allow printout of an entry confirmation
 Form printing
                            Only Cantor (disable A+W Business)
 Order export
                            Only Cantor (disable A+W Business)
 Request order export
                            Copy quotation to order
 Quotation to order
                            Copy quotation to quotation
 Quotation to quotation
                            Copy order to order
 Order to order
                            Copy order to quotation
 Order to quotation
                            Allows the saving/caching of the shopping cart and the last configuration
 Back up shopping cart
                            Allows the transfer of the shopping cart to ERP (order)
 Direct check-out
                            Allow entry of quotations
 Enter quotations
                            Allow entry of orders
 Enter orders
                            Display prices; otherwise the user does not have any prices
 Display prices
                            Only Cantor (disable A+W Business)
 Price Change
                            Determines to display documents in history that are not entered in iQuote.
 All documents in history




A+W Software GmbH                  EN-CONFIG-A+W iQuote.docx                                             14
2. Configuration
2.1. Enable customer employees
The customer's employee must be enabled for iQuote and the mail address and password/PIN
must be assigned.




The business case must be assigned; through this it is possible to determine which functions are
available in iQuote.


2.2. Enabling products, shapes, and processings
Release
Items, shapes, and processings must be enabled in product management. This also affects the
insulated glass; the exchangeable components are defined by the IGU exchange groups. These
products do not have to be released explicitly. However, then no determination of the sequence
is possible. The customer determines what should be activated here and the workflow created.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                     15
Sorting
In addition to the release of the products for iQuote, the sequence of the products in iQuote can
be determined; for this the entry of the sorting key is necessary. If this is on 1 (default), then the
sorting is always done by product number. However, the sorting key takes precedence and thus it
is possible to get a sensible sorting of the products (e.g. by thickness) even if the product numbers
are not ascending by thickness.


2.3. Processing parameter values Restrictions
2.3.1. Processing parameter limit values for round corners
The iQuote user should only be able to enter defined values for round corners; intermediate
dimensions should be avoided for production-technical reasons. For this, a round corner must be
selected in the product master data and the value with text entered on the Radius field of the
Processing parameters dialog. For the entry of the processing, only a rounding of 5,10,15 is
possible. You must pay attention that the default value matches an entry. Otherwise, there will be
inconsistent display behavior.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                    16
2.3.2. Processing parameters min/max values
In the production master data of A+W Business, it is possible to define the minimum dimension
and the maximum dimension for edge cutouts, area cutouts, notched corners, and corner cut-
offs. For round corners and holds, this is according to the diameter




From the values for warehouse and purchase order, the maximum values will be used in iQuote.
The input of a larger or smaller value is not possible and iQuote will jump back to the maximum or
minimum value.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  17
2.4. Definition of the IGU exchange groups
Definition of the IGU exchange groups serves to guide the user precisely. Thus, for example, it is
no longer possible to exchange a TG for an ornamental glass in the IGU.




Assignment of the products to the exchange groups




Assignment of the exchange groups to each BOM element spacer and glass.Only then is an
exchange possible in iQuote
Warning: Gases cannot be exchanged in iQuote.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                      18
A+W Software GmbH   EN-CONFIG-A+W iQuote.docx   19
2.5. PS area assignment for iQuote user
Assign production area for the user who was determined as Business User in the configuration
management. It is recommended that you create an individual iQuote user here.




The quotations and orders for iQuote are created in this production area.


2.6. Status allocation
Via the Change 24-iQuote status point, it is controlled up to which order status the user can
change a procedure in iQuote. The lock status must be set to this document status. The user
status is assigned in case of change, may not be over the lock status. Otherwise only one change is
possible.




Expansion: 2-phase commit
The order in A+W Business is first created with the status of the status point 502 – deletion
release. Only in the release phase is the status of the status point 1 entry assigned to the
document and the further processing started (commit, ...) An assignment of the status point 502
is thus always required.


A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  20
2.7. Enabling status points
The user can only see the history points that are enabled in the status points for iQuote.
Here at least the points 1,2,4, and 8 should be enabled.




2.8. PS order area assignment and document numbers
Documents that are entered with iQuote receive their document numbers from the number range
of the default production area of the employee who is entered as A+W Business User. The default
assignment can be found on the A+W Business employee dialog.




However, this is only the case if in the assignment workflow, a mapping to the default production
area of the customer consultant of the entering customer was not undertaken. Effective


A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                21
immediately, this mapping is the standard since the pre-defined mapping workflow contains the
appropriate activity


Activity: Customer Consultant Department in Workflow Studio (see also 3.6 Activities Model Mapping)




2.9. Printout and mail sending with Crystal Reports
For the set-up of automatic confirmation mail or any other form printout with Crystal Reports, the
workflow "…Formula\ExchangeService\workflow_print_documents.txt" has to be used. See also
A+W Business Configuration Chapter 10.26.




A+W Software GmbH                                EN-CONFIG-A+W iQuote.docx                            22
2.10.   Number of places after the decimal point for
   dimensions
In the glass area, a dimension in the millimeter range is always entered, only in the area of
furniture glass is there work with 1/10 millimeter precision. In order to satisfy this, iQuote can be
set flexibly.




In the company parameters, on the System tab, the number of places after the decimal point can
be set.




If you enter a 0 here, then no more decimal places can be entered in iQuote. The step change is
displayed to 1,5,10,100 instead of 0.1, 1, 10,100.


2.11.           Setting up an iQuote user
The iQuote user is entered in A+W Business under Master Data -> Partner -> Customers. Please
select a customer and use the functions to reach the employees.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                    23
On the employee dialog, it is possible to configure access under the iQuote group. Activate the
[active] check box and enter the e-mail address as login. Now assign a password and define the
business case under the employee who should work with iQuote. Use the [Unlock] button to
enable a locked login. The locking happens after an incorrect password has been entered three
times.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                    24
2.12.           Configuration of Macros
iQuote can record all familiar macro types (corner, edge, area macros and their parameterizable
types). The macros are released in A+W Business for iQuote like any other processing.
Important is that the SN macro files are reachable via the UNC path for the Commercial Document
Service.




Company -> Company data



In iQuote, a new macro icon appears. The positioning is done as in the corresponding processings
(corner, edge, interior cut-out). In addition, the parameters of the parameterizable macros are
queried. The defaults for the parameters are taken from the CAD file and overwritten by the
stored defaults from A+W Business.




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                 25
2.13.           Setting up stock dimensions and boxes
With the new widget Stock Dimensions, iQuote now supports the sale of boxes and stock
dimensions.
In the stock dimension management Master Data>Products>Product>Stock Dimensions


it is possible to release the stock dimension/box and assign a screen to the stock dimension. This
screen will be displayed in iQuote, but must be present on the IIS. The content path of the widget




in the workflow determines where it appears.
The box is taken over in the order as if it had been recorded in the order entry, including stock
reservation and later removal from stock. The stock on hand is displayed in iQuote with a traffic
light.




With a Stock > minimum stock the stock availability is green, with >0 and < minimum stock it is
yellow and with stock 0 it is red. The stock is only displayed if the box/stock dimension is created
in the stock.
If no image file is stored in the stock dimension, the display is handled with the CAD sketch;
otherwise, the stored image is displayed.

A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                     26
If the box was released incl. the boxes with Ident. no, then these also appear.




The price calculation is done as box price or stock dimension price.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                   27
2.14.           Self pick-up
Self-collection can be defined in the check in/out workflow. Here, a collection is filled in the
workflow, which includes the self-collection dates available for selection. For example, these can
be distinguished according to morning and afternoon collection.




This data is entered as "KeyValue" object in the workflow, whereby the key with the alphanumeric
key must match the route in A+W Business.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                   28
Depending on the self pick-up, the route is then implemented in the order and the order can be
provided at the desired time and date. If the collection is not filled with values, then the selection
of self pick-up is not displayed.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                     29
2.15.            Commission and customer PO number
The commission and customer PO number that are entered during the iQuote configuration are
now also visible in the history overview. The user can use these to limit and filter the documents.




All commissions of a document are displayed separately with "-".
The columns can be moved and hidden.




2.16.            Restriction of the processings in the workflow
The iQuote workflow can now restrict the processings available; this can make sense if for
particular products such as kitchen backsplashes, only particular macro processings may be
applied. Similarly for particular shapes such as the circle, for example, the application of corner
cut-outs is not possible.
Initially, 2 variables must be created and initialized.




These serve to accommodate the selected geometry and the filtering of the processings.
The filters are defined in a sequence activity by deleting and adding the filter collection.
Deleting the filters:




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                      30
Inserting the filters:




The "FilterDescription" must be filled with the A+W Business product group in "Member" and
with a list of processing product numbers separated with commas. If the "Value" is empty, then
all products of this product group are permitted.
The filter object must be assigned the property ProcessingFilter of the ActionValidatorProcessing.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  31
Here in the example, there is a different processing filtering according to selected model. The
property for this in the ValidatorGeometry is




And attach a switch activity to the SelectedGeometry object, now it is possible to define a
different filter by shape number.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                    32
For examples, see the pre-defined iQuote workflow!


Sorting the processing types
The sequence of the filters defines the sequence of the processing types in the processing entry of
A+W iQuote.




Simply shift the filters and the sequence is changed!




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  33
2.17.          History display of A+W Business documents
Via the business cases, it is possible to set the history (overview) using the "All documents in
history" entry (Chapter 2.2.1) so that all of the customer's documents are displayed. That is,
documents that were not entered in iQuote can thus be displayed and their status history called
up.



These documents cannot be edited in iQuote. For each glass item, the SN sketch is created and
displayed in the item view.




This function represents the first step toward the expansion of iQuote into a customer
information system.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  34
2.18.           Document history in the history display
Document header attachments can now be displayed in the history for iQuote. This applies for
quotations and orders. The documents can be downloaded or viewed using the link or the button
in the browser. For display, the appropriate client software is required (PDF viewer, Office, etc.).




In the browser, it is now possible to select whether the file is saved or displayed.




Which attachments are visible for the iQuote user is controlled by the file attachment types
(Master Data > Texts > File attachment types).




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   35
2.19.           Report attachments in the history display
In addition to the document header attachments, form printing generated in A+W Business
(quotation, order confirmation, delivery note, and invoice) can also be enabled for iQuote. The
condition for this is that the form printing was generated with the new Crystal Report Print
Service. Only in this case is forwarding to iQuote possible.
To activate the forwarding, the Handover to iQuote option must be activated per form in the form
management (Master Data>Forms>Form Management). This is only available if the option Form
printing with Crystal Report is activated in the system parameters and the script 20170424a.sql
was executed.




With this option, each printout is saved in the reporting service as a PDF. iQuote then displays
these documents in the history.




These can then be downloaded and displayed with the PDF viewer.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                     36
2.20.    Save the shopping cart and the current
   configuration
iQuote is a Web application with which the browser can be closed at any time. Since the complete
configuration is present in the browser and no document has yet been generated in A+W
Business, everything is gone after closing. In order to prevent this, the configurator service now
saves all data in a storage cache and persists this data in the database every 10 seconds. If the
service is stopped, then the saving is done before the stopping, so that in case of a crash of the
service, there is a maximum data loss of 10 seconds.
The storage of the configuration is activated with the business case option Save Shopping Cart:




If now the user makes another product configuration, stores products in the shopping cart and
does not end this configuration with an order, then this configuration is saved in iQuote and
offers to him for the next configuration. This also works on another device. The user can thus
cancel a session in the middle and continue it later on any end user device.




The user can load the canceled configuration, delete this configuration or display the contents of
the shopping cart. If he does not want to continue the canceled configuration, he can begin a new
configuration. The saved configurations are also retained for him.



A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                    37
A+W Software GmbH   EN-CONFIG-A+W iQuote.docx   38
2.21.   Total thickness for insulated glass and
   product designation
iQuote now allows the entry of insulated glass with specification of the total thickness. The total
thickness of the insulated glass unit is also displayed.




The thickness specification is retained if a glass is exchanged and the thickness specification can
be achieved by changing the spacer. If not, then the thickness specification is deleted.


 Starting with 3-layer insulated glass, the thickness specification is always deleted in case of
exchange of the exchange glass and its thickness since there are various combination possibilities
for the spacers here. The system cannot make an automatic specification here.


The various spacer combinations that belong to a total thickness are displayed in brackets.


Here, iQuote makes the user's life easier since it is also possible to select the spacer combinations
purposefully; this is not possible in the A+W Business order entry.


Inch values are supported, however there is no metric thickness in an imperial database.


This function is not activated by default and must be activated in the validator exchange activity
workflow with the property "ThicknessPresetHide".




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                       39
Restriction: The function conditions that in A+W Business the spacers are assigned per spacer
type in a separate product group. Only this way is it possible to find the correct spacer. Colors
are not currently supported, if these are just in the spacer text, then one product group must be
created per color.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  40
2.22.    Insulated glass product designation 2 as
   structure
Via workflow, it is possible to configure the back end so that the insulated glass description 2
always consists of the structure (glass and spacers). Up to now, this was only the case if there was
an exchange in the BOM. This is useful for customers who do not use the insulated glass
description 2 and always specify the structure of the glass in the formula printing. Until now, this
could not be displayed this way in iQuote.




For set-up, the iQuote workflow for the expansion point 1 must be added.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   41
In the BackendPriceCalculation activity, the BackEndUpdateAction property must be assigned a
new object. In it, the property "ProductDescriptionMode" must be set to
"ProductDescriptionModes.IsolatedGlassDescription2IsBom."


Examples with image, price, and restriction must always be set to "true."
Otherwise, these actions will not be executed!


 New BackEndUpdateAction() With {.Image = true, .Price = true, .Restriction = true, .ProductDescriptionMode =
 ProductDescriptionModes.IsolatedGlassDescription2IsBom }




2.23.               Product colors for items
For the selection of product colors in iQuote, the available colors must be assigned to the product.




A+W Software GmbH                               EN-CONFIG-A+W iQuote.docx                                       42
The RGB color codes must be entered in the colors so that the tiles are displayed in the
appropriate color. If the RGB value can not display the color attractively, you can also assign a
PNG file. It must be stored in the ContentPath of the widget (e.g. content\auw\colors) and the file
name must include the variant number with the suffix .png (e.g. 8001.png). This file is mainly
displayed, the image size should not exceed 80x80 pixels.




Presently, special colors are not displayed.


In the workflow, the "ProductColor" validator can be inserted into the branch. The product
selected in the product validator must go into the color selection as input parameter.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                 43
For example, this can be done conditionally for some product codes.




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx         44
2.24.           Product and ISO exchange filter
In IQuote, it is now possible to use the product filter added in the workflow to filter the available
products. This way, the total number of products can be reduced to a few. This applies both for
the product selection (single glass, items) as well as for the ISO exchange products (glass and
spacers). Therefore it is possible to select the spacers by spacer types or thicknesses, for example.




For setup, there must be an assignment of the filters according to the product validators in the
configuration workflow. For parameterization, the functions are described in Chapter 4.7.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                    45
Important is that the first filter always gets the option ClearFilter = True so that the filter
collection can be deleted.
The values of the filters display only the values that actually occur in the complete selected hit
quantity. The filters always represent an AND link; only the values within a filter are OR linked.
Thus, for example, the selection of the thicknesses 5, 6, 8 mm.


Currently, there are filters available for the following functions:


    -   Thickn.
    -   Product type
    -   Product class


For setup examples, see the standard workflow. The sequences can simply be copied from there
and attached to your own workflow.


The filter methods for exchange glass can be attached by product type, that is, for float, TG, LSG,
and spacers. For exchange filters, the filters can differ per BOM element. This is achieved since the
filters are inserted per product type. See filter definition in the example. With the filter methods
…ByTuple, however, it is also possible to attach a filter purposefully to the 2nd spacer.


The filters with …Collection… allow a free definition of the values to be filtered.




A+W Software GmbH                       EN-CONFIG-A+W iQuote.docx                                    46
A+W Software GmbH   EN-CONFIG-A+W iQuote.docx   47
2.25.            Filter by name
In iQuote, it is now possible to use an added filter in the workflow, which filters the available
products by their names. This way, the total number of products can be reduced further with the
other filters. The filter can be defined both for the product selection (single glass, articles) as well
as for IG exchange products (glass and spacers).




For setup, there must be an assignment of the filters according to the product validators in the
configuration workflow.




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                      48
2.26.          Spacer colors in IG replacement
Defined spacer colors can now be displayed in iQuote during IG replacement. This option
ColorHide of the ValidatorExchange must be deactivated in the workflow; it is activated by
default.




The assignment of the spacer variants must have been made in A+W Business.




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                49
The IG product structure is also displayed with the color in iQuote. If the glazing thickness is
specified or the spacer changed, then the default color of the spacer is always selected again. This
behavior is also implemented in A+W Business.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   50
2.27.           Color filter and special colors
Now filters can be defined for the product colors. These must be inserted in the workflow behind
the product color activity.




Description, code or special can be defined as ColorFiltertype.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                51
If a color is selected that is a special color, then an additional field appears in the color selection in
which the special color number can be entered.




This special code is written like the color into the item.


2.28.            Two phase commit when saving
A+W iQuote will no longer create duplicate orders if an error occurs during a distributed
transaction in the 2nd step. A 2-phase commit was introduced. This means that the
order/quotation is first created in A+W Business. It receives the status of the status point 502 –
deletion release. At this point there are no further checks (credit limit and scheduling), in the 2nd
step the document number is transferred and the shopping cart is saved in iQuote. As a 3rd step
the order is released and gets the status of status point 1 - new order. If only one error occurs in
step 2, an order with deletion release remains in A+W Business. This is deleted by the end-of-day
routine without being archived. Internally, the middleware (Ice) prevented repeated execution of
the memory routine, as this could also lead to duplicates. This change is a breaking change, see
chapter 3.1 of the installation instructions.

       Create order
       Status point 502




      Save cart in iQuote




       Release order status point
       1




A+W Software GmbH                       EN-CONFIG-A+W iQuote.docx                                      52
2.29.          File upload and web link
A+W iQuote can now upload files and associate web links to external web spaces with the
documents. This is done both at the item level and at the document header level. The upload can
be integrated in the workflow both in the check-in/checkout as well as in the configuration
workflow. Checkin/checkout results in an attachment in the header of the document. The one in
the configurator for an attachment at item level. The workflow determines which file types can be
uploaded and also the maximum file size. For web links the size is only limited by the available
web space.
The uploaded files are first saved with a temporary name in the root directory of the A+W
Business file attachments.




As soon as a document is generated, it is moved to the A+W Business document structure and
given the file name specified by the customer.
An antivirus program must check the files in the root directory, otherwise unchecked files from
the web can reach the intranet. iQuote does not check the files, the customer is responsible for
this.
In the attachment types at least one attachment type must be enabled for iQuote. If this is not
done an exception is thrown.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                    53
The "Attachment" activity from the Common Glass area must be integrated into the workflow. For
their parameterization please see in 4.3.




2.30.           Pattern/coating side and side
In the product selection activity of the workflow, it is now possible to enable whether the user can
change the pattern/coating side and side of a glass. In the workflow, 2 properties have to be
activated for this. Default is the old state that this is not possible. For configuration of the
properties, see 4.3 product activity.




The display then looks like this:


A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                   54
2.31.           Projects with associated products
For selection of project in A+W iQuote, the projects have to be created in A+W Business and
assigned to the customer. If an assignment of products to a project has been made, then the
selection of the products can be restricted to these in iQuote.
The workflow activity "Objects" is in the "iQuote InOut" area, but it can only be used sensibly in
the CheckIn; otherwise the customer would first see standard prices and then select a project.
This doesn't make any sense.




The activity has to be added to the CheckIn workflow. The project number is stored in the
Card.Header.ObjectNo. In the configuration workflow, it is therefore possible to access the


A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                      55
project again. The parameterization is documented under 4.4. If a customer has not been
assigned a project, the selection of projects does not appear. The project assignment cannot be
changed after the fact.
In order to display the products that were assigned to the project in A+W Business (expanded
project definition has to be activated in the Business company master data), the iQuote method
"Products for Object" has to be used in the Configurator workflow.




Via a complaint, it can be queried whether there is a project number; if this is the case, the
workflow queries the product numbers. If not, the standard configuration workflow with all
products is established.




From the "ProductsforObjects" (configuration under 4.7), the string comes as list with the
assigned product numbers. It is passed along in the "ProductNummberIn" property of the
"Products" activity and thus defines the selected products.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   56
A+W Software GmbH   EN-CONFIG-A+W iQuote.docx   57
2.32.           Inserting processings per workflow
With the new workflow activities, it is now possible to enter, change, delete, and find processings
in the processing widget from the workflow. This is applicable if due to upstream queries (e.g. a
partial-surface coating) a processing should be applied automatically.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                   58
The methods are under iQuote methods in the Workflowstudio.




   1) Find processing




   2) Delete processing




A+W Software GmbH                 EN-CONFIG-A+W iQuote.docx   59
   3) Insert processing




   4) Change processing




A+W Software GmbH         EN-CONFIG-A+W iQuote.docx   60
2.33.         Documents flag per entry path
      There are three paths for how orders can get into the system:
      1.      Entered through iQuote
      Assignment of a text to WebDocument.SignForConfiguratorCreated in the mapping
      workflow. This text becomes Bestelltext2 in the order entry.




      2. Via EDI
      A customizing is attached for this in customizing point 100




A+W Software GmbH                  EN-CONFIG-A+W iQuote.docx                          61
        A formula in the context “AFTER_IMPORT” takes care of the assignment of the text to

          !********************************************************************************************;
          !***** EDI Import with transferring referenced P.O. number to P.O. text 2 *******;
          !********************************************************************************************;
          ! Used Variables;

          If m_sFormulaContext = 'AFTER_IMPORT';
                    SET fktDoc.m_sBEST_TEXT2 = ‘EDI Imported’;
                    IF SalStrLength(fktDoc.m_sBEST_TEXT2) > 40;
                                SET fktDoc.m_sBEST_TEXT2 = SalStrLeftX(fktDoc.m_sBEST_TEXT2, 40);
                    EndIf;
          EndIf;


        Bestelltext2.

        3. Manual order entry

        Here nothing has to be done, for all other entries are manual.


2.34.             Product filter for processings
In iQuote, it is now possible thanks to a filter added in the workflow to filter and search for the
processing products by name. The name filter is available in all processings.




The activity must be added to the workflow after the processing activity and always applies for
the foregoing.




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                     62
2.35.           Suppress credit limit
The credit limit check can now be suppressed in iQuote; for this, the property CreditlimitCheck
must be set to false in the Configurator workflow (0000 - A+W iQuote). This can be done for
individual customers or for quotations and not for orders.




2.36.           Shape filter for the geometry entry
The shapes to be displayed in the geometry widget can be restricted by using filters. For this, first
a variable must be created to accommodate the filter.




This variable must be assigned to the "ValidatorGeometry" in the "ShapeFilters" property.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                    63
The filter must now be filled with the shapes to be displayed, but first collections must be deleted
in which data from earlier selections is present. First the "SelectedFilters"




Then the "AllFilters"




Now a filter is inserted:

New FilterDescription() With { .Description ="1", .Member = "ShapeNo", .MatchingOperator="=",
.Value = "1" }




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   64
Finally, the SelectedFilters must be set to the AllFilters in order to restrict the selection to the
filters and activate it.




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                       65
2.37.           History with exact status release
In A+W Business, now access to the document history in the system parameters (tab 5.
Parameters) can be restricted with the switch tab "A+W iQuote history only with exact status" to
documents that have precisely the status that was released under Master Data>Order>Status
elements.




The status element is not checked, but rather the status assigned to the status element.




This enables the user to display only the documents in iQuote that correspond to this status
assignment release. If the option is deactivated, then all documents of the customer are displayed
and stati that are not released are shifted to the next lower status that is released in the display.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   66
2.38.            Multi-site capability and load distribution
Essentially, a distinction must be made between multi-site capability and load distribution. Multi-
site capability allows the use of several different sites in different databases with an iQuote IIS. An
internal multi-site capability is only supported if the business user has a site restriction. Only then
is a customer's document created on the respective internal A+W Business site. Since these
internal sites are no longer the standard, they will not be discussed further here. We will examine
only the external multi-sites in different databases.

The configuration of the iQuote web, the Configurator Service, and the Commercial Document
Service must always be done the same way.
In the web configuration, it is decided whether the web front end is installed so it is multi-site
capable. If the active is set to true for the site, then this site must be addressed using an expanded
URL.




Only if this site is also the default site can the expansion of the site in the URL be omitted.

<Server>/Web.Web/<Sitenumber>, z.B. <Server>/Web.Web/1




There are 2 icons; the first is for site 1, the second is to the default site.



A+W Software GmbH                       EN-CONFIG-A+W iQuote.docx                                   67
If in the web configuration active = true is selected, then this must also be done in the
configuration of the configurator and document services.




The load distribution can be activated regardless of the multi-site installation!!!

In the example above, 2 workers were created for the site 1. The following service configuration
results in the service locator. It can be adjusted by calling the configuration dialogs. Each
configuration change should be accompanied by a restart of the IIS.
For a hardware firewall (non-Windows firewall), it must be noted that the port range to be
released must be expanded, the first Configurator Service uses the port 65235, all additional ones
the following 65236,65237, …. Which port is used can be looked up in the Service Locator (Ice
Grid).




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                 68
Then the access to the configurator and document service are distributed and an even load
achieved.

Essentially, one site per A+W Business database must always be created in the infrastructure. The
site creation is done in the infrastructure




The configuration of the database is then taken care of in the configuration of the individual sites.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                    69
The workflow can also be stored specifically across sites for individual sites. This guarantees
maximum flexibility and simplicity.




Which service is responsible for which site and worker does not depend on the name, but on the
properties in the Service Locator.




AW.Multisite:

                 -1 does not mean site-dependent

                 <> -1 site-dependent

AW.Multisite.Worker:

                 The respectiver worker for load distribution



A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   70
The load distribution is done according to the round robin process; this means that with a new
session, the service is always assigned that is the least used. This assignment remains for 12 hours
and is then discarded. A browser once logged in retains its service assignment for 12 hours and
can also profit from the data caches.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                  71
2.39.          Checkbox widget and HTML designation
The new checkbox widget can be inserted several times into a workflow. The designation is also
HTML-capable.




The property "ShowCheckbox" controls whether the widget contains only text or whether it also
gets a checkbox.

The workflow looks as follows in iQuote; the link opens a new page with the GTCs




The "Document validation" workflow is used to forbid the user from completing the PO. There,
the data object is searched for in CartItem and then a message text inserted. The variable
"checkedAGB" is filled with the content of the checkbox (true/false).



The CommonCheckbox is obtained from the CartItemAction via Linq (FirstOrDefault).




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                    72
The property checked is checked and then a message is added




Inserting the message into the Cart.Hints collection, with access to the custom texts:




Thus, this message appears and the PO is not generated; the user must first accept the GTCs.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                 73
HTML designations for all widgets

All widgets can now display the designation as HTML code. This also goes for access to the custom
text in order to make the designation multilingual.

First create the text in the database; quotation marks are to be "escaped" through another
quotation mark. For a link it is important that the link opens in a new window; this is achieved by
the HTML property target="_blank". The HTML code is written 1:1 to the page.
 INSERT INTO [Core_CustomTexts]
 ([Guid],[VersionId],[LockingToken],[Code],[LanguageCode],[Text]) VALUES
 (newid(),1,'00000000-0000-0000-0000-000000000000', N'IGDescription', 'en-GB' ,
 N'<div>Please select the function of your insulating glass. If you need
 information about insulating glass</div><p><a
 href=''https://de.wikipedia.org/wiki/Mehrscheiben-Isolierglas'' target=''_blank''
 title=''Wikipedia Multi-pane insulating glass''>Wikipedia Multi-pane insulating
 glass</a></p>' )


The custom text is to be inserted into the workflow as follows:




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   74
The result looks like this:




A+W Software GmbH             EN-CONFIG-A+W iQuote.docx   75
3. System configuration
3.1. Incorporation into a start page
iQuote can be incorporated into any homepage via an IFrame tag. For example, here this is done
with the page startup.html. The page uses bootstrap CDN for the layout. However, this is not
mandatory.

This page can be called using http://localhost/AWSOA.Web.Web/Startup.html.


 <!DOCTYPE html>

 <head>

    <!-- Latest compiled and minified CSS -->

    <title>Sample Startup Page</title>

    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css">

    <style>

           .row { margin-right: 0; margin-left: 0; }

           #webconfigframe {min-height: 850px; width: 100%; border: 0; }

           iframe {padding-left: 20px; padding-right: 20px;}

    </style>

 </head>



 <body style="overflow:hidden">

    <div class="container-fluid" style="padding:0;overflow:hidden;">

      <div class="clearfix row" id="header" style="width:100%;height:91px;margin-left:20px;margin-right:0;">

             <div class="col-md-12">

                 <h1><span>A+W - Software for Glass and Windows</span></h1>

             </div>

      </div>

      <div class=row>

           <!-- Iframe of the local Web Configurator, you can set the language and the                        -->

           <!-- Url: http://localhost/AWSOA.Web.Web/[de|en|fr]?theme=[uniform|metro|metroblack|default|black] -->

           <!-- --------------------------------------------------------------------------------------------- -->

          <iframe id="webconfigframe" class="embed-responsive-item"
 src="http://localhost/Web.Web/de?theme=uniform"></iframe>

      </div>

    </div>

 </body>




A+W Software GmbH                           EN-CONFIG-A+W iQuote.docx                                          76
3.2. Set-up of the product images
Essentially iQuote does not provide any images for the products. The products are searched for in
the Content directory of the iQuote master directory
(e.g. "C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content").
It is recommended that you create a subdirectory for each customer in which all images/graphics
are stored. For A+W, this is the subfolder auw. This is always updated during an update. The new
customer folder is retained. In this customer folder, you should create subdirectories for the
individual areas; this helps you maintain an overview.
   -   ads
   -   productcategories
   -   productgroups
   -   products
   -   producttypes
       ….
These relative directories "auw\products" must be entered in the workflow for the
activities so that the bitmaps from this directory are used for the products.
The names must be the A+W Business product number with the extension ".png". Only
PNG images are supported. For the size, 140x100 pixels is recommended, for there is no
scaling in the browser.
For glass and IGUs, a SN sketch is displayed in iQuote; for items the image stored in A+W
Business can be displayed instead of the sketch. Thus, for example, a technical sketch for
hardware or a large product image can be presented for an item.




The stored image is displayed in iQuote.




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                  77
3.3. Customer's own icon for the browser
If the customer requires an own logo for iQuote, this can be stored in the relative folder
~/Content/Custom/Images/
as favicon.ico. This icon is primarily used and replaces the A+W favicon.ico from the main folder.
This main folder file must not be overwritten, because it will always be lost during an update.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                  78
3.4. Customer texts for the user interface
A+W iQuote obtains the language-dependent screen texts as a message resource; these cannot
be changed. In the workflow, it is possible to access localized texts from the "Core_CustomTexts"
table with the "Configurator.GetCustomText(code, languageCode)" method. In order to have this
flexibility in the user interface, now a mechanism has been created in order to make this take
preference for the mask texts over the database table. Thus, for example, the name of the
application can be adapted in the browser or the buttons in the header area if the customer so
wishes.

 -- Selection of the texts
 SELECT [Guid],[Code],[LanguageCode],[Text],[Description] FROM [dbo].[Core_CustomTexts]

After the program start, the "Core_CustomTexts" table is filled automatically with blank texts for
the screen translation. This is done in the first language that is entered in the infrastructure
languages.




Texts that should also be localized then have to be entered via database insert/update command
for the language in question. The value that is obtained by default from the message resource and
displayed is in the comment column. It serves as template for the customer's texts. Among other
things, this is very important if there are placeholders {0},{1}... in the text. With these default
records, you always have an overview of which messages there are. The list adjusts itself.
However, nothing is overwritten.


Inserting a text for the browser application names

 INSERT INTO [Core_CustomTexts]
 ([Guid],[VersionId],[LockingToken],[Code],[LanguageCode],[Text],[Description]) VALUES
 (newid(),1,'00000000-0000-0000-0000-000000000000', N'WebConfigurator', 'de-DE' , N'A+W
 Buy', N'')




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                   79
After the restart of the Configurator Service, the application presents itself under the name "A+W
Buy".




Not all texts can be adapted like this, but a lot of buttons and central texts can; using the
Comment column, it's easy to find these.


A trick for seeing all text codes in iQuote is to use a script to fill all blank texts with the content of
the codes; then the iQuote is only displayed with the codes and the changes can be made
efficiently.


 -- Preset all Text with the textcode
 UPDATE [AWSOA].[dbo].[Core_CustomTexts] SET Text=Code where Text= '';

 -- undo the preset
 UPDATE [AWSOA].[dbo].[Core_CustomTexts] SET Text= '' where Text=Code;




A+W Software GmbH                       EN-CONFIG-A+W iQuote.docx                                       80
4. Workflow
The workflow handles the complete control of iQuote. Which widgets (e.g. product selection,
processing entry) will appear under which circumstances is decided with the 3 workflows.
The Studio workflow handles the editing and creation of workflows.
The delivery state includes standard workflows that are updated by A+W and cannot be edited.
However, they can serve as a template for individual workflows.


4.1. Studio workflow
The Studio workflow is in the Config Tools.




On the File->Load menu, it is possible to load a template (Predefined) or a changed workflow
(Custom).




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                 81
Via the menu, it is also possible to save the workflow. It is stored in the database. However, it can
also be exported from the XAML file and then loaded into another installation.


4.2. Workflow management
With the Management workflow, a created workflow is assigned an end point (there where it is
executed).




It is possible to call the Management workflow using the Configuration menu




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                    82
This is where the assignment for the expansion point for the workflows will be made. Crucial for
iQuote are the expansion points 0 to 6.


4.2.1. Configurator expansion point ( 0000 )
In this workflow, the complete layout of the iQuote is determined, which widgets appear with
which values, tiles, and products. How are these grouped and when is the price calculation called
up for a valid configuration. This workflow is executed for each action in iQuote and is always run
through completely. The surface is then eestablished anew and indicates the current status of the
entry incl. of the price


4.2.2. Mapper expansion point ( 0001 )
The mapper workflow supports the implementation of the iQuote data in A+W Business. Here,
values can be changed, such as the production scheduling area or new product processings can be
inserted into the A+W BOM. An example of this is the addition of surcharges or processings. The
workflow is always called when a price calculation is executed or the A+W Business document is
created.


4.2.3. Check-in expansion point ( 0002 )
The check-in workflow enables the querying of global data such as, e.g. an order reference. It is
run through once at the start of the configuration; if it is empty, iQuote begins immediately with
the product configuration.


4.2.4. Check-out expansion point ( 0003 )
The check-out workflow enables the querying of data such as delivery date or additional PO texts.
It is run through once at the end of the configuration, after the customer leaves the shopping cart.


4.2.5. Document validation expansion point ( 0004 )
The document validation workflow enables the validation of the document after leaving the
check-out workflow. Here, the delivery date can be checked, for example. If an error hint is
returned, then the order is not possible and the user remains in the check-out workflow. The hint
is presented to the user.



A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                   83
4.2.6. Add to cart expansion point ( 0005 )
The add to cart workflow is run through when a product should be placed in the shopping cart.
Here too, if a hint is inserted, then the product is not placed in the shopping cart and the user
receives an error message.


4.2.7. Back end update expansion point ( 0006 )
The back end update workflow calls up the price calculation. It enables the determination of the
surrounding rectangle and the error output if this is not possible. That is, if data that was
determined in the back end should be accessed, then this is the correct starting point.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                     84
4.3. Activities configurator
This workflow is a flow chart at the end of which is the call of the price calculation if a valid
production selection has been made. The "ContentPath" properties should always be adapted, for
only this way is a separation of the client and default A+W images guaranteed. For the content
(images), copyright must always be heeded. The following activities are available:


  Product Types
  Selection of the product types by product type number. The images are searched for in the Content directory.
  Parameters            Description                                                        Default
  Category              Display of category (breadcrumb)                                   AWSOA.Core.Messages.Globa
                                                                                           l.WebCategoryProduct
  Configurator          Access to the Configurator service                                 Configurator
  ContentPath           Relative directory for the content of the widget in the Content    e.g. "auw/producttypes"
                        directory
  Description           Description that appears after the widget header
  Display Name          Name of the activity in the Studio workflow
  ItemIn                Incoming item object of iQuote                                     ItemIn
  ItemOut               Output item object of iQuote                                       ItemOut
  Name                  Title of the widget in iQuote
  ProductType           Selected product type as workflow variable
  ProductTypesIn        ERP product type number                                            „1,2,3,40,50“



  Product Groups
  Selection of the product groups by product type number or product groups. The images are searched for in the Image
  directory.
  Parameters            Description                                                        Default
  Category              Display of category (breadcrumb)                                   AWSOA.Core.Messages.Globa
                                                                                           l.WebCategoryProduct
  Configurator          Access to the Configurator service                                 Configurator
  ContentPath           Relative directory for the content of the widget in the Content    e.g. "auw/producttypes"
                        directory
  Description           Description that appears after the widget header
  Display Name          Name of the activity in the Studio workflow
  ItemIn                Incoming item object of iQuote                                     ItemIn
  ItemOut               Output item object of iQuote                                       ItemOut
  Name                  Title of the widget in iQuote
  ProductGroup          Selected product group as workflow variable
  ProductGroupsIn       ERP product group number that should be displayed                  „1013,2234“
  ProductTypesIn        ERP product type number for display of all groups of the types     „1,2,3,40,50“




A+W Software GmbH                          EN-CONFIG-A+W iQuote.docx                                             85
 Tiles
 Freely-definable tile selection. The images are searched for in the Image directory.
 Parameters             Description                                                          Default
 Category               Display of category (breadcrumb)                                     AWSOA.Core.Messages.Globa
                                                                                             l.WebCategoryProduct
 ContentPath            Relative directory for the content of the widget in the Content      e.g. "auw/producttypes"
                        directory
 Description            Description that appears after the widget header
 Display Name           Name of the activity in the Studio workflow
 ItemIn                 Incoming item object of iQuote                                       ItemIn
 ItemOut                Output item object of iQuote                                         ItemOut
 Name                   Title of the widget in iQuote
 TileId                 Selected Id
 TilesIn                Collection with tile objects
 AutoCollapsible        Widget collapses after selecting a value and displays the            False
                        selection in its title



 Geometry
 Entry of the geometry data. All shapes enabled for iQuote appear in this widget. It enables the entry of an additional
 dimension or the width and height of the rectangle
 Parameters                   Description                                                              Default
 Category                     Display of category (breadcrumb)
 ContentPath                  Relative directory for the content of the widget in the Content          unused
                              directory
 Description                  Description that appears after the widget header
 Display Name                 Name of the activity in the Studio workflow
 ItemIn                       Incoming item object of iQuote                                           ItemIn
 ItemOut                      Output item object of iQuote                                             ItemOut
 Name                         Title of the widget in iQuote
 DefaultRectangleWidth        Specified width of the rectangle
 DefaultRectangleHeight       Specified height of the rectangle
 RectangleOnly                Only rectangle entry should be possible                                  False
 ShapeFilters                 Filter to restrict the available shapes and products                     CartItemActionFilter
                                                                                                       Object
 ValidGeometry                Entry of a valid geometry
 SelectedGeometry             Selected geometry (object must be defined as variable)                   GlassShape Object
 WidthOnly                    Only the width is displayed. No shapes.




A+W Software GmbH                           EN-CONFIG-A+W iQuote.docx                                                86
 Product
 Selection of the products that are defined via the properties of the activity
 Parameters                Description                                                       Default
 Category                  Display of category (breadcrumb)
 ContentPath               Relative directory for the content of the widget in the Content   „auw/products“
                           directory
 Description               Description that appears after the widget header
 Display Name              Name of the activity in the Studio workflow
 ItemIn                    Incoming item object of iQuote                                    ItemIn
 ItemOut                   Output item object of iQuote                                      ItemOut
 Name                      Title of the widget in iQuote
 ProductGroupsIn           Enumeration of the product group numbers of the ERP that          „100,101,102“
                           should be displayed (additive to other enumerations)
 ProductId                 Number of the selected product
 ProductNumbersIn          Enumeration of individual ERP product numbers that should         „1004,1005,1006“ or 104-
                           be displayed (additive to other enumerations)                     110,118
 ProductTypesIn            Enumeration of the product type numbers of the ERP that           „1,2,3“
                           should be displayed (additive to other enumerations)
                           Enumeration of individual ERP product groups that should be       „500,562“
                           displayed (additive to other enumerations)
 AutoSelect                The first product will be selected automatically and thus the     False
                           workflow is forwarded and the next widget established.
 ProductTupleId            Main product or BOM product, enables the hardware entry for       0=Main product
                           a door if > 0
 OptionShowPattern         Show the icon for the pattern direction and side (user can        False
                           change this)
 OptionShowCoating         Show the icon for the coating side (user can change this)         False




 Product Colors
 Selection of the color/variants defined for the product.
 Parameters                Description                                                       Default
 Category                  Display of category (breadcrumb)
 ContentPath               Relative directory for the content of the widget in the Content   „auw/colors“
                           directory (presently not used)
 Configurator              Access to the Configurator service                                Configurator
 Description               Description that appears after the widget header
 Display Name              Name of the activity in the Studio workflow
 ItemIn                    Incoming item object of iQuote                                    ItemIn
 ItemOut                   Output item object of iQuote                                      ItemOut




A+W Software GmbH                           EN-CONFIG-A+W iQuote.docx                                             87
 Name                    Title of the widget in iQuote
 ProductNoIn             Number of the product should be displayed for the assigned
                         colors
 AutoSelect              The first color will be selected automatically and thus the     False
                         workflow is forwarded and the next widget established.
 ColorCode               Includes the color code of the selected color



 Exchange
 Entry of the IG exchange products for glass and spacers. The products must be defined as exchange products in A+W
 Business.
 Parameters                  Description                                                 Default
 Category                    Display of category (breadcrumb)
 ContentPath                 Relative directory for the content of the widget in the     „auw/products“
                             Content directory
 Description                 Description that appears after the widget header
 Display Name                Name of the activity in the Studio workflow
 ItemIn                      Incoming item object of iQuote                              ItemIn
 ItemOut                     Output item object of iQuote                                ItemOut
 Name                        Title of the widget in iQuote
 ProductId                   Number of the IG product for which the exchange should
                             be made
 ProductId                   Number of the selected product
 AutoSelect                  The first product is selected automatically                 False
 ThicknessPresetHide         The selection of the total thickness is suppressed; the     True
                             display of the total strength is not affected by this
 ColorHide                   The selection of the spacer colors is suppressed            True
 GasHide                     Not used                                                    False




A+W Software GmbH                          EN-CONFIG-A+W iQuote.docx                                           88
 Processing
 Entry of the processings
 Parameters                 Description                                               Default
 Category                   Display of category (breadcrumb)                          AWSOA.Core.Messages.Global.
                                                                                      WebCategoryProcessing
 ContentPath                Relative directory for the content of the widget in the   „auw/products“
                            Content directory
 Description                Description that appears after the widget header
 Display Name               Name of the activity in the Studio workflow
 ItemIn                     Incoming item object of iQuote                            ItemIn
 ItemOut                    Output item object of iQuote                              ItemOut
 Name                       Title of the widget in iQuote
 CriteriaDrilling           Product group of the drillings (not in use)
 CriteriaEdgeProcessing     Product group of the edge processings (not in use)
 OptionShowDelete           Display of the button for deleting a processing If both   True
                            buttons are not displayed, the list box for the
                            processings disappears
 OptionShowAdd              Display of the button for adding a processing. If both    True
                            buttons are not displayed, the list box for the
                            processings disappears
 ProcessingFilters          Filter to restrict the available processing types and     CartItemActionFilter Object
                            products
 OptionHeadlineSelection    Overwriting the headline of the processing selection      „“
 OptionHeadlineProcessing   Overwriting the headline of the processing steps          „“




A+W Software GmbH                       EN-CONFIG-A+W iQuote.docx                                             89
 Price calculation
 Call of the price calculation of the ERP system. The activity should only be called if the product is capable of price
 calculation. Product and geometry are specified.
 Parameters                      Description                                                    Default
 Category                        Display of category (breadcrumb)
 BackEndUpdateAction             Back end function to be called for the price calculation       Not used
 ContentPath                     Relative directory for the content of the widget in the        Not used
                                 Content directory
 Display Name                    Name of the activity in the Studio workflow
 ItemIn                          Incoming item object of iQuote                                 ItemIn
 ItemOut                         Output item object of iQuote                                   ItemOut
 Header                          Document header data                                           Cart.Header



 StockDimensions
 Entry of the boxes/stock dimensions with query of stock availability
 Parameters                      Description                                                    Default
 Category                        Display of category (breadcrumb)                               AWSOA.Core.Messages.Globa
                                                                                                l.WebCategoryCases
 ContentPath                     Relative directory for the content of the widget in the        „auw/products“
                                 Content directory
 Description                     Description that appears after the widget header
 Display Name                    Name of the activity in the Studio workflow
 ItemIn                          Incoming item object of iQuote                                 ItemIn
 ItemOut                         Output item object of iQuote                                   ItemOut
 Name                            Title of the widget in iQuote
 ProductNoIn                     Product number for selection of the boxes/stock
                                 dimensions
 DimensionId                     Id of the selected box (composed of product, dimension
                                 and content together)




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                                    90
 Attachments
 Upload of documents and input of web links
 Parameters                      Description                                               Default
 AllowedExtensions               Definition of the file types (extensions) that can be     “”
                                 uploaded. The enumeration is marked with ";".
                                 semicolon and must contain the dot in the ending (e.g.
                                 .pdf;.jpg;.png;.docx;.doc)
 Category                        Display of category (breadcrumb)                          AWSOA.Core.Messages.Globa
                                                                                           l.WebCategoryCases
 ContentPath                     Relative directory for the content of the widget in the   “”
                                 Content directory (without meaning)
 Description                     Description that appears after the widget header          “”
 Display Name                    Name of the activity in the Studio workflow               Attachments
 ItemIn                          Incoming item object of iQuote                            ItemIn
 ItemOut                         Output item object of iQuote                              ItemOut
 MaxFileSize                     Maximum file size in byte
 Name                            Title of the widget in iQuote                             “”



 Bars
 Entering bars (not possible for Business in iQuote !!!)
 Parameters                      Description                                               Default




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                        91
4.4. Activities Checkin
Essentially all In/Out activities can also be used in Checkin.


  InOut DeliveryText
  Entry of a delivery note and a reference number (external order number)
  For parameters, see 3.5     For entry of the customer PO number, the InOutDeliveryText can be used. The customer PO
                              number is then displayed subsequently in the header. The PO text can be hidden.



  InOut Objects
  Displays a customer's projects so that he can select these in order to receive special project conditions. This can be a
  different customer than the customer assigned to the login.
  Parameters                   Description                                                     Default
  Category                     Display of category (breadcrumb)                                “”
  Configurator                 Access to the Configurator service                              Configurator
  ContentPath                  Relative directory for the content of the widget in the         „auw/objects“
                               Content directory; the image has to exist as
                               <projectnumber>.PNG. Otherwise, non.png is searched
                               for.
  CustomerNumber               Number of the customer for which the projects should be         Cart.Header.CustomerNo
                               displayed
  Description                  Description that appears after the widget header                „“
  Display Name                 Name of the activity in the Studio workflow                     ActionValidatorInOutObjects
  ItemIn                       Incoming item object of iQuote                                  ItemIn
  ItemOut                      Output item object of iQuote                                    ItemOut
  Name                         Title of the widget in iQuote                                   „“
  ObjectNumber                 The selected project number. This value goes in and out. If     Cart.Header.ObjectNo
                               the project number that goes in <> 0, the widget is
                               restricted to this project number. It is in change mode.
                               Subsequent change of the project is not possible.




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                                 92
4.5. Activities Checkout
The Checkout workflow controls the process of order completion. After the configuration of the
products, delivery addresses and delivery dates as well as order texts and reference numbers
(order number), it allows entry Essentially each checkout activity can also be used in the Checkin
workflow. In some cases, however, it makes more sense to determine the delivery date if the
product to be ordered is known.


  InOut DeliveryDate
  Entry of the delivery date and the delivery time. For determination of the delivery date, the default delivery times of all
  products in the cart are examined and the date with respect to the longest delivery time is the suggested delivery date. If
  a weekday is stored in the customer route in the ERP, delivery is shifted to the next possible route day. This is a non-
  binding delivery request by the customer.
  Parameters                   Description                                                    Default
  Category                     Display of category (breadcrumb)
  ContentPath                  Relative directory for the content of the widget in the        unused
                               Content directory
  Description                  Description that appears after the widget header
  Display Name                 Name of the activity in the Studio workflow
  ItemIn                       Incoming item object of iQuote                                 ItemIn
  ItemOut                      Output item object of iQuote                                   ItemOut
  Name                         Title of the widget in iQuote
  CustomerNoIn                 Number of the customer for whom the route days should          Cart.Header.CustomerNo
                               be determined
  DesiredDeliveryDate          Specification of the delivery date, there is no more           DateTime.MinValue
                               calculation using the delivery time and route day
  DeliveryTimeHide             The delivery time can be switched off with this property       "True" = delivery time will not
                                                                                              be displayed
  DeliveryTimeFrom             Specification of the delivery time from                        new TimeSpan(18,0,0)
  DeliveryTimeUntil            Specification of the delivery time until                       new TimeSpan(8,0,0)
  SelfCollects                 Collection with KeyValue objects for self pick-up              New
  SelfCollectSelected          Selected key value for self pick-up                            „0“




  InOut DeliveryAddress
  Entry of the deviating delivery address. The existing delivery addresses are offered for selection. However, any delivery
  address can also be entered. Any change to an existing delivery address causes the customer number of the delivery
  address to be reset. It is then no longer the default delivery address.
  Parameters                 Description                                                      Default
  Category                   Display of category (breadcrumb)
  ContentPath                Relative directory for the content of the widget in the          unused
                             Content directory
  Description                Description that appears after the widget header


A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                                93
 Display Name              Name of the activity in the Studio workflow
 ItemIn                    Incoming item object of iQuote                                ItemIn
 ItemOut                   Output item object of iQuote                                  ItemOut
 Name                      Title of the widget in iQuote
 SelectionOnly             Selection of delivery addresses possible, no changes or new   False
                           entries.
 CustomerNoIn              Number of the customer for whom the delivery addresses        Cart.Header.CustomerNo
                           from the ERP are displayed



 InOut DeliveryText
 Entry of a delivery note and a reference number (external order number)
 Parameters                Description                                                   Default
 Category                  Display of category (breadcrumb)
 ContentPath               Relative directory for the content of the widget in the       unused
                           Content directory
 Description               Description that appears after the widget header
 Display Name              Name of the activity in the Studio workflow
 ItemIn                    Incoming item object of iQuote                                ItemIn
 ItemOut                   Output item object of iQuote                                  ItemOut
 Name                      Title of the widget in iQuote



 Checkbox
 Display of an HTML text with an optional checkbox
 Parameters                Description                                                   Default
 Category                  Display of category (breadcrumb)
 ContentPath               Relative directory for the content of the widget in the       unused
                           Content directory
 Checked                   Return value that contains the state of the checkbox
 Description               Description that appears after the widget header, can be
                           HTML code
 Display Name              Name of the activity in the Studio workflow
 ItemIn                    Incoming item object of iQuote                                ItemIn
 ItemOut                   Output item object of iQuote                                  ItemOut
 Name                      Title of the widget in iQuote
 ShowCheckbox              Determines whether the checkbox is with or without            True
                           checkbox




A+W Software GmbH                         EN-CONFIG-A+W iQuote.docx                                         94
4.6. Activities Model Mapping
With the mapping activities, the data model between iQuote and Commercial Document Service
can be influenced. Thus, for example, with enforcement of the property
WebDocument.SignForConfiguratorCreated the character string can be set that is transferred in
the Bestelltext2 of the A+W Business. Thus documents can be marked as entered by iQuote and
also searched for this way. The Bestelltext2 can be printed and the customer thus sees that he has
entered the purchase order.
With the following activity, the production area (Department) is set to the default production area
of the customer consultant. The document number is determined by the production area range.


  Customer Consultant Department
  Provides the production area range of the customer consultant (employee who is assigned to the customer in A+W
  Business). This can be transmitted in the property WebDocument.Department and then determines the production area
  in which the document number is assigned.
  Parameters                 Description                                                     Default
  Configurator               Access to the Configurator service                              Configurator
  CustomerNo                 Customer number                                                 WebCart.Header.CustomerNo
  Department                 Return value of the department/production area                  WebDocument.Department
  Display Name               Name of the activity in the Studio workflow
  DocumentType               Enum of the document type                                       WebCart.Header.DocumentTy
                             DocumentType.Order/DocumentType.Quote controls the              pe
                             number range from which the number is taken



  Get Selected Tile By Display Name
  Searches for the activities with the DisplayName and delivers the selected value. Thus in the MapperWorkflow, it is easy
  to search for an activity and its selected value and use it as deciding value for the mapping.
  Parameters                 Description                                                     Default
  CartItem                   The currently configured item                                   WebCart.CurrentItem
  Name                       DisplayName of Activity in Workflow Studio
  TileId                     Return value of the selected tile



  Add/Change Product
  Adds the commercial document data transfer objects to a product object. Here you can choose where the product is
  inserted - as main product or BOM product - the Append property is used for this
  Parameter                  Description                                                     Default
  WebItemDto                 The currently configured item                                   WebCart.CurrentItem
  ProductID                  Product number that should be inserted/changed
  TupleId                    Main product or BOM product, enables the BOM extension          0=Main product
  Append                     Adds the product to the end or as main product                  false

  Add/Change Action



A+W Software GmbH                           EN-CONFIG-A+W iQuote.docx                                               95
 Adds any product or processing to the commercial document data transfer objects, the processing has to be created in
 the workflow. Here, it is possible to select where the product is added with an existing tuple number is changed, if it is
 not found, will be added. Via the property Append it can be determined whether inserted at the end or after the glass.
 Parameter                  Description                                                       Default
 WebItemDto                 The currently configured item                                     WebCart.CurrentItem
 ProductID                  Product number that should be inserted/changed
 WebDataDto                 Product object that is changed or added                           New
                                                                                              WebProcessingEdgeDto()
                                                                                              With { .ProductId=5000,
                                                                                              .Edge1=True }
 Append                     Adds the product to the end or as main product                    false
 WebActionDto               The WebAction is returned in order to enable additional           Return value
                            changes




A+W Software GmbH                           EN-CONFIG-A+W iQuote.docx                                                 96
4.7. Activities Methods
The activities of the type "Methods" do not insert a widget into iQuote; instead, they change the
workflow data. These are the methods for defining filters in the product widgets, for example.


  ProductFilters
  Inserts a product filter to a prior product widget. The product filter determines what the filter can limit. The filter must
  be behind a product activity. The filter values to be described are selected from A+W Business and are available
  automatically for selection.
  Parameter                   Description                                                          Default
  ClearFilter                 Deletes the filter collection; should be set to true for the first   False
                              assignment and then to false for all others
  Configurator                Access to the Configurator service                                   Configurator
  Description                 Description of the filter that is displayed in iQuote; if blank,
                              then the default description is displayed
  Display Name                Name of the activity in the Studio workflow
  ItemIn                      Incoming item object of iQuote                                       ItemIn
  ItemOut                     Initial item object of iQuote; the filter is inserted here           ItemOut
  ProductFilterType           Type of the filter, e.g. by thickness or by product type and         ProductFilterType.Thickness
                              group                                                                /ProductType/ProductGrou
                                                                                                   p/Description



  ProductExchangeFiltersByTuple
  Inserts a product exchange filter for a defined BOM element (e.g. spacer)
  to a foregoing ISO exchange widget. The exchange filter type determines what the filter can limit. The filter must be next
  to an exchange activity. . The filter values to be described are selected from A+W Business and are available
  automatically for selection.
  Parameter                   Description                                                          Default
  ClearFilter                 Deletes the filter collection; should be set to true for the first   False
                              assignment and then to false for all others
  Configurator                Access to the Configurator service                                   Configurator
  Description                 Description of the filter that is displayed in iQuote; if blank,
                              then the default description is displayed
  Display Name                Name of the activity in the Studio workflow
  ExchangeFilterType          Type of the filter, e.g. by thickness or by product type and         ExchangeFilterType.Thickne
                              group                                                                ss/ProductType/ProductGro
                                                                                                   up

  ItemOut                     Initial item object of iQuote; the filter is inserted here           ItemOut

  TupleId                     BOM number of the product (1=first glass, 2=spacer, etc.)




A+W Software GmbH                             EN-CONFIG-A+W iQuote.docx                                                  97
 ProductExchangeFiltersByType
 Inserts a product exchange filter for a defined ERP product type (e.g. float glass or TG)
 into a preceding ISO exchange widget. The exchange filter type determines what the filter can limit. The filter must be
 next to an exchange activity. . The filter values to be described are selected from A+W Business and are available
 automatically for selection.
 Parameter                   Description                                                          Default
 ClearFilter                 Deletes the filter collection; should be set to true for the first   False
                             assignment and then to false for all others
 Configurator                Access to the Configurator service                                   Configurator
 Description                 Description of the filter that is displayed in iQuote; if blank,
                             then the default description is displayed
 Display Name                Name of the activity in the Studio workflow
 ExchangeFilterType          Type of the filter, e.g. by thickness or by product type and         ExchangeFilterType.
                             group
                                                                                                  Thickness
                                                                                                  ProductType
                                                                                                  ProductGroup
 ItemOut                     Initial item object of iQuote; the filter is inserted here           ItemOut


 TypeId                      The A+W Business product group to be selected (e.g. 1 =
                             float glass, 2 = TG, 3 = LSG, 60 = spacer)



 ProductExchangeFiltersCollectionByTuple
 Inserts a product exchange filter for a defined BOM element (e.g. spacer)
 to a foregoing ISO exchange widget. The exchange filter type determines what the filter can limit. The filter must be next
 to an exchange activity. The filter values to be displayed must be transferred to the activity.
 Parameter                   Description                                                          Default
 ClearFilter                 Deletes the filter collection; should be set to true for the first   False
                             assignment and then to false for all others
 Configurator                Access to the Configurator service                                   Configurator
 Description                 Description of the filter that is displayed in iQuote; if blank,
                             then the default description is displayed
 Display Name                Name of the activity in the Studio workflow
 Filters                     Collection with the filters to be displayed                          Filters
 ItemOut                     Initial item object of iQuote; the filter is inserted here           ItemOut

 TupleId                     BOM number of the product (1=first glass, 2=spacer, etc.)




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                                  98
 ProductExchangeFiltersCollectionByType
 Inserts a product exchange filter for a defined ERP product type (e.g. float glass or TG)
 into a preceding ISO exchange widget. The exchange filter type determines what the filter can limit. The filter must be
 next to an exchange activity. The filter values to be displayed must be transferred to the activity.
 Parameter                   Description                                                          Default
 ClearFilter                 Deletes the filter collection; should be set to true for the first   False
                             assignment and then to false for all others
 Configurator                Access to the Configurator service                                   Configurator
 Description                 Description of the filter that is displayed in iQuote; if blank,
                             then the default description is displayed
 Display Name                Name of the activity in the Studio workflow
 Filters                     Collection with the filters to be displayed
 ItemOut                     Initial item object of iQuote; the filter is inserted here           ItemOut


 TypeId                      The A+W Business product group to be selected (e.g. 1 =
                             float glass, 2 = TG, 3 = LSG, 60 = spacer)



 ColorFilters
 Inserts a color filter into a preceding product color widget. The ColorFilter type determines what the filter can restrict.
 The filter must be next to a product color activity.
 Parameter                   Description                                                          Default
 ClearFilter                 Deletes the filter collection; is currently not needed since         False
                             the color filters do not have defined values
 Configurator                Access to the Configurator service                                   Configurator
 Description                 Description of the filter that is displayed in iQuote; if blank,
                             then the default description is displayed
 Display Name                Name of the activity in the Studio workflow
 ItemIn                      Incoming item object of iQuote                                       ItemIn
 ItemOut                     Initial item object of iQuote; the filter is inserted here           ItemOut
 ColorFilterType             Type of the filter, e.g. according to name, color code or            ColorFilterType.
                             special color
                                                                                                  Description
                                                                                                  Code
                                                                                                  Special




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                                  99
 Products for Objects
 Inserts a color filter into a preceding product color widget. The ColorFilter type determines what the filter can restrict.
 The filter must be next to a product color activity.
 Parameter                   Description                                                          Default


 Configurator                Access to the Configurator service                                   Configurator
 CustomerNumber              Number of the customer for which the project products                Cart.Header.CustomerNo
                             should be obtained
 Display Name                Name of the activity in the Studio workflow
 ObjectNumber                The project number for which the products should be                  Cart.Header.ObjectNo
                             obtained.
 ProductsForObject           Returns the product numbers that are assigned to the                 Variable to be defined
                             customer project, e.g. "1004, 1005, 1006"; this value can
                             then be inserted into a "Products" activity as product list.



 ProcessingFilters
 Adds a product processing filter to an existing processing widget. The product filter determines what the filter can limit.
 The filter must be behind a product activity. The filter values to be described are selected from A+W Business and are
 available automatically for selection.
 Parameter                   Description                                                          Default


 ClearFilter                 Deletes the filter collection; should be set to true for the first   False
                             assignment and then to false for all others
 Configurator                Access to the Configurator service                                   Configurator
 Description                 Description of the filter that is displayed in iQuote; if blank,
                             then the default description is displayed
 Display Name                Name of the activity in the Studio workflow
 ItemIn                      Incoming item object of iQuote                                       ItemIn
 ItemOut                     Initial item object of iQuote; the filter is inserted here           ItemOut
 ProcessingFilterType        Type of the filter, e.g. by name                                     ProcessingFilterType.Descri
                                                                                                  ption




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                                 100
4.7.1. Change processings

 Processing Add
 Search the processing activity specified in the SeachName and insert a processing; this new processing is selected in the
 interface. It appears under the processing type specified in ProcessingTyp. This way, a macro can appear under
 edgework. If the SearchName is not specified, the first processing activity is found. With the activity, processings can be
 created from the workflow.
 Parameter                  Description                                                       Default


 Configurator               Access to the Configurator service                                Configurator
 ItemOut                    Initial item object of iQuote; the processing is inserted here    ItemOut
 NewProcessing              The new processing data object                                    CartItemActionData Variable
 ProcessingType             The processing type under which the processing appears            Enum ProcessingType
 ProductNo                  Product number of the processing to be inserted
 SearchName                 Display name of the action validator to be searched for; if
                            empty, the first one is found.




 Processing Update
 Search the processing activity specified in the SeachName and change the processing; this changed processing is selected
 in the interface. It appears under the processing type specified in ProcessingTyp. This way, a macro can appear under
 edgework. If the SearchName is not specified, the first processing activity is found. With the activity, processings can be
 changed from the workflow. If the processing type change, the parameters are lost.
 Parameter                  Description                                                       Default


 Configurator               Access to the Configurator service                                Configurator
 ItemOut                    Initial item object of iQuote; the processing is inserted here    ItemOut
 NewProcessing              The changed processing data object                                CartItemActionData Variable
 ProcessingType             The processing type under which the processing appears            Enum ProcessingType
 ProductNo                  Product number of the changed processing
 SearchName                 Display name of the action validator to be searched for; if
                            empty, the first one is found.




 Processing Delete
 Search the processing activity specified in the SearchName and delete the transferred processing; the first processing is
 then selected. With the activity, processings can be deleted from the workflow.
 Parameter                  Description                                                       Default
 Configurator               Access to the Configurator service                                Configurator
 ItemOut                    Initial item object of iQuote; the processing is inserted here    ItemOut
 Processing                 Processing object that is to be deleted. Can be searched for      CartItemActionData Variable
                            with "Processing Find."




A+W Software GmbH                           EN-CONFIG-A+W iQuote.docx                                               101
 Removed                    True if the processing was deleted; otherwise false
 SearchName                 Display name of the action validator to be searched for; if
                            empty, the first one is found.




 Processing Find
 Search the processing activity specified in the SearchName and in that, search for the processing with the transferred
 product number or by processing type. The processing is returned or an empty object <nothing>. With the activity,
 processings can be found from the workflow, which are then deleted or changed.
 Parameter                  Description                                                      Default


 Configurator               Access to the Configurator service                               Configurator
 ItemOut                    Initial item object of iQuote; the processing is inserted here   ItemOut
 Processing                 Return of the found processing data object. If nothing was       CartItemActionData Variable
                            found, the return is <nothing> null.
 ProcessingType             The processing type that should be searched for. Only the        Enum ProcessingType
                            processing type or product number can be specified.
 ProductNo                  The product number that should be searched for. Only the
                            processing type or product number can be specified.
 SearchName                 Display name of the action validator to be searched for; if
                            empty, the first one is found.




A+W Software GmbH                          EN-CONFIG-A+W iQuote.docx                                              102
4.8. Multilingual Workflow
iQuote is multilingual via the URL; this means that all fixed texts are output in the appropriate
language. In order to activate this, the language abbreviation (e.g. ../en, ../de) must be attached.
However, the workflow is created customer-specifically and thus here there is also the need to
enable this easily. The duplication of the workflow for each language is surely not the correct
solution. The maintenance of the workflows would suffer for this.
The multilingual texts are managed in the table Core_CustomTexts, currently there is no
management program for this. It would make sense to create an Excel table. This could be
translated and then Insert Statements created with the help of the Excel table.
 INSERT INTO [Core_CustomTexts]
 ([Guid],[VersionId],[LockingToken],[Code],[LanguageCode],[Text],[Comment]) VALUES
 (newid(),1,'00000000-0000-0000-0000-000000000000', <Code nvarchar(255)>, <LanguageCode nvarchar(5)>
 ,<Text nvarchar(max)>,<Text nvarchar(max)> )


These must then be executed in the SQL Server Management Studio.
The subsequent editing can also be done there.




The language codes ('LanguageCode' column) correspond to the Core_Languages table




In order to use these texts in the workflow, there are 2 possibilities:
    1. Via function Configurator.GetCustomText(code, languageCode)
        Definition of a global variable for assignment of "Cart.CurrentItem.Culture"




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                 103
      Configurator.CustomMessage("Test", LanguageCode)




      This function can be used for all activities, for the properties Category, Description, and
      Name.
      To establish a collection, the function can also be used in an expression.




   2. Via language code sequence „@@<code>@@“
      To simplify this, in an activity (not in an expression) without function call, there can be a
      text fetching; for this, the message code must have a "@@" in front of it and be attached.


A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                   104
      The function is then expanded internally and the Configurator.CustomMessage("Test", )
      function is called.




A+W Software GmbH                EN-CONFIG-A+W iQuote.docx                              105
4.9. Dynamic values for the workflow
The workflow can now save dynamic values in the DynamicValues properties of the Cart and
CartItem. These values are saved in the database and always re-presented to the workflow in its
ItemIm property. The workflow must ensure that they are transferred to the ItemOut.
The Activities DynamicValuesGet() delivers a value identified by a string. DynamicValuesAdd()
stores it again. If the value is already there, it is overwritten.




                                      Configurator
             ItemIn                    Workflow                     ItemOut
         DynamicValues                                           DynamicValues




This way, the workflow can now store any data in the workflow that it needs for calculations or
comparisons.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  106
 DynamicValuesGet
 Search in the dynamic values for a specified key. If it is present, the value is returned; otherwise an empty string
 Parameter                   Description                                                       Default


 DynamicValues               Collection of the dynamic values                                  itemIn.DynamicValues
 Key                         Key string for the value
 Value                       Delivers the value for the key transferred; if it is not there,
                             then the value is empty



 DynamicValuesAdd
 Inserts a dynamic value with a specified key. If it is present, the value is overwritten
 Parameters                  Description                                                       Default
 DynamicValues               Collection of the dynamic values                                  itemIn.DynamicValues
 Key                         Key string for the value
 Value                       Delivers the value for the key transferred; if it is not there,
                             then the value is empty




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                                                  107
4.10.           Access to the iQuote data structures
The workflow uses the internal data structures of iQuote and transforms this into new widget
data that appears on the interface. An iQuote without workflow is just an empty shell. In this
process we intervene with ready-made widgets, but it may also be necessary to access this data
via Visual Basic (the programming language of the workflow). This article describes the necessary
steps to implement this.
First you have to define where to add your code. Checkin-, checkout-, configuration- or mapping
workflow For this example I decide to use the configuration workflow and want to access the
checkin data "Customer item" or "Commission". The argument given to this workflow is the cart.




This cart has 3 properties for the different workflows. Cart.CheckIn, Cart.Checkout and
Cart.CurrentItem. I need access to Cart.CheckIn. Cart.checkin has a collection of ItemActions,
which is a collection of CartItemActionData. All widget data objects are children of this
collection. To get the widget data for the order, you need the data object of this widget. The
default display name is "DeliveryText Reference".




First I create a variable locally in a sub-workflow of the widget's data type.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                               108
Then the selected ItemRemark object can be assigned to your "myCommonItemRemark" object
variable with this Visual Basic Linq statement:

TryCast(cart.CheckIn.ItemActions.FirstOrDefault(Function(c) c.DisplayName =
"DeliveryText Reference").SelectedData, CommonItemRemark)

For more information about Linq, please google "Visual Basic Linq 101" on the web for help.
You can now access the customer position with myCommonItemRemark.CustomerItem.
The ILSpy software can be used to find out the shape properties.




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                 109
5. Master Data Consolidation
Before the introduction of iQuote, it must be checked whether the current master data for order
entry is designed for the use of iQuote.
Here it must be considered that the end customer who enters a glass via iQuote does not have
the knowledge of a trained employee of the customer and thus also does not know the
customer's internal structures and work instructions and also should not know these.
This means that all special tasks that a person entering an order must perform to enter a product
must be done by iQuote automatically; it not, products will be entered incorrectly via iQuote. If
this is not possible for a product, it may not be enabled for iQuote.
Examples that an end customer cannot perform in iQuote:
•        There is a process that in case of a particularity, the person entering the order creates a
text (e.g. inserts a correct text or simply overwrites the product designation of a processing), this
text is printed everywhere in production and heeded.
•       Under particular circumstances, a dummy article is attached to the item or order that
influences the price.
Most of these things should be resolved with appropriately-maintained master data or through
use of the correct functions. This can mean a consolidation of the master data, which can be
associated with a lot of effort on the customer's part, The result will also be, in addition to the
possible use of iQuote, easier entry.
In order to find out if something must be adjusted, the customer should play through the entry of
the products that are enabled in iQuote and check whether there are any particularities that a
layperson cannot know and thus could make an error.
In this document, individual examples are listed that have occurred at customers.


5.1. Precise product designations
Using the product designation, the end customer should understand what he is selecting. If, for
example, a processing includes cryptic abbreviations that everybody at the company understands,
it is not necessarily the case that the end customer understands these too.


5.2. Hole drillings for different diameters
For a hole drilling processing, you can define in the master data in which diameter range the
processing may fall. This must be maintained if you would like to work with the following
processings, for example:
•       Hole drilling <= 20mm
•       Hole drilling > 20mm
If this restriction is not maintained, then you can use the processing <= 20 mm for a 30 mm hole,
which may mean a cheaper price. The person recording the order can receive a work instruction
in order to select the correct processing, the end customer cannot.



A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   110
Through the restriction it is ensured that the selected diameter fits the processing. However, it is
much more elegant to have just one processing for all diameters. There is no (more) reason to
have several. The price calculation can orient itself according to the diameter entered, it does not
have to orient itself using the processing article.


5.3. Entering the correct edge processing
For the entry of edge processing, there are several scenarios that require the deeper knowledge
of the person entering the order. The person entering the order knows which edge processing he
must apply how, but the end customer does not know this.
•       On a sheet, several edge processing are entered for the same edge quality, e.g. polish
straight edge, polish round edge, polish special edge. You do this, e.g. due to the price calculation,
rounding is more expensive than a straight edge.
•       A shape where all edges should be polished. The straight edges should be ground on a
normal grinding machine (which may only be able to process straight edges), the arches on a CNC
(which can grind everything but is slower and more expensive).
At the latest starting with AWB 5.5, there is no more reason to use several edge processings for
the same edge quality. See on this the A+W Business configuration documentation, chapter on
Shape edge additions.
If this is introduced, it simplifies normal entry and thus has a big added value for the customer
regardless of iQuote.


5.4. Use of color variants
If you enter a surface processing, e.g. for a finish, you should work for the selection of colors with
appropriate color variants and not just write the color code (e.g. RAL) manually next to the
product designation of the processing. Since you do not want to enter variants for all possible
color codes since there would be too many, you can enter a variant for special colors in addition
to the common ones For this variant it is possible to write the appropriate color code in a field
(that appears when this variant is selected). This field is transferred to production and should be
available in iQuote as soon as case #350715 has been implemented.
In addition, for the color variants in the master data, you can also store a color code for the
display, which is then depicted in iQuote in this color.


5.5. TG always with complete BOM
An edge processing must always be present in the BOM of TG, at least a seaming. If this is missing
in the product's BOM, then during order entry an edge processing must always be applied, even in
iQuote. If this is forgotten, a TG without edge processing is created.
If there is already a seaming in the TG's master data, then it is also not possible to enter an
incorrect product. If the customer would like a higher-quality edge processing, this can be entered
easily; iQuote then reduces the lower-value processing (seaming).




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                    111
6. CSS Customizing
If the CSS is changed for a customer, then you must pay attention that it must be reworked with
each new version. Thus, permanent work and costs are required.


6.1. General information and basic principles
There is a setting that is definitely helpful when testing design adjustments: it can be specified that
with each refresh of the website (that is, when you press F5 in the browser) that the .less files are
recompiled. Thus, changes will be effective immediately. However, this is at the expense of the
performance, so it is not intended for productive operation.
For this, in the file C:\Sandpiper1\WebWeb\web.config                     in   the   line   <compilation
targetFramework="4.5"> the entry debug=“true“ must be added.




For the conversion to live operation, it is not necessary to restore the original file. It is sufficient to
change the value from debug=“true“ to debug=“false“.
Generally, the custom theme should always be used for design adjustments. The theme can be
specified in the infrastructure configuration as follows:




A+W Software GmbH                       EN-CONFIG-A+W iQuote.docx                                     112
Alternatively, it is possible to access the custom theme regardless of the preconfigured theme. For
this, the addition ?theme=custom must be made to the iQuote URL, as you can see in the following
screenshot. However, the prerequisite is that in the infrastructure configuration, the value of the
entry Theme is Mandatory is on Off (see marking no. 5 in the screenshot above).




This way, you can also access all other themes:
    •   Uniform
    •   Black
    •   Default
    •   Metro
    •   Metroblack
    •   Custom
Note: The browser notes the last theme loaded. If you want to change from the custom theme back
to the original theme (Uniform), it is not sufficient to leave off the parameter in the iQuote URL
again. Instead, you have to specify the standard theme as URL parameter one time. Alternatively,
you can delete the browser data.



A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                 113
Otherwise, it is frequently helpful to reset the IIS so that changes become effective. For example,
this is the case if you wwant to change icons (bootstrap glyphicons). That's to say: if you wonder
why a change is not effective immediately, it's best to restart the IIS. The A+W iQuote services play
no role here.
Colors can always be specified in the CSS in different ways. You can make wild combinations. Here's
an example:
    •   Hex color: #0070c0
    •   Red-green-blue: rgb(255,99,71)
    •   Red-green-blue-Alpha: rgba(255,0,0,0.5)
    •   Name of the color (only particular ones): darkblue à You can also write transparent!



6.2. How custom theme works
The custom theme is found under the following path:
C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom
Critical here are the two files kendo.custom.less and awsoa-responsive.custom.less.
The file kendo.custom.less forms the design basis. On the website of the Kendo provider, there is
actually a configurator where you can click together such standard themes yourself. There, the
focus is mostly on text colors, colors of titles, background colors, deviating colors if a field has been
marked with the mouse, tec. Then you can download a finished theme. You get a second
kendo.custom.less file whose content is very similar to that of the original file. That's why it's very
easy for you to transfer its content to the actual file.
Custom Theme Builder | Kendo UI for jQuery (telerik.com)
Note: Here you specify basic settings, however the effects are not immediately visible. This is
because the file is sometimes overridden.
The file awsoa-responsive.custom.less imports the file kendo.custom.less. Here, individual settings
can be overridden. It's easy to trace this with the entry @image-folder, which is present in both
files. For the file kendo.custom.less, the value is "Uniform" and for the file awsoa-
responsive.custom.less, the value is "Default".
Intended are always the folders with the same name in the path C:\Program Files
(x86)\A+W\Sandpiper1\WebWeb\Content\kendo. That the entry comes from the awsoa-
responsive.custom.less file is easy to see using the example of the load icon in iQuote. The icon that
is in the Default folder is displayed.
What the file awsoa-responsive.custom.less does otherwise is that it calls a particular template
file. By default, this is C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\awsoa\awsoa-
theme-template-responsive.less. This file is commented and here you can test various changes in
the browser and then build them permanently into the template file after the fact.




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                    114
6.3. Overriding rules and own CSS rules
This point is probably one of the most important ones.
The later a command comes in the .less file, the higher it seems to be prioritized. It is possible to
build your own CSS rules into .less files, which you can design directly in the browser. At least with
the Chrome browser, this works very well:
For this, you have to right-click on the element you'd like to examine and then select Inspect from
the context menu.




Then the selected element is highlighted in color on the left side and on the right side you can see
the associated CSS rules. The rules that are crossed out do not apply because they are overridden,
for example.




The active rules can be edited directly and you can examine the result live in the browser.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   115
An example of where the background color was overridden by precisely this button is at the end
of the included awsoa-responsive.custom.less file.
This way, it is possible to construct your all of your own rules for any element and to execute
them. The full spectrum of CSS rules is available. These include:
    -    Changing the font size and type
    -    Turning and stretching elements
    -    Editing button sizes
    -    Configuring backgrounds/fillings with particular color gradiants
    -    Adding your own new elements (e.g. displaying a new image)


6.4. Background color on the main menu




File:
C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom\awsoa-responsive.custom.less
Value:



A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   116
@carusell-foo1-background


6.5. Colors of iQuote navigation bar




File:
C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom\awsoa-responsive.custom.less
Values:
Background color of the whole bar: @navbar-background-color
Text color in general: @navbar-text-color
Color of the rectangles around the fields: @navbar-border-color
Fill color of the field you have just selected: @navbar-active-background-color
Fill color of the fields if you point to them with the cursor: @navbar-text-hover-color
Text color of the fields if you point to them with the cursor: @navbar-text-hover-color


6.6. Colors of configurator navigation bar




File:
C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom\awsoa-responsive.custom.less
Values:
Text color: @breadcrumb-text-color
Color of the surrounding rectangles: @breadcrumb-border-color
Fill color of the category you have just selected: @breadcrumb-selected-color
Fill color of the categories not selected: @breadcrumb-completed-color




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                            117
6.7. Change load icon
File:
C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom\awsoa-responsive.custom.less
Value:
@image-folder: "default";
To Do:
In the directory C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\kendo
C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\kendo. Then, in the file awsoa-
responsive.custom.less, set the value of @image-folder to the name of the new folder.
Exchange the file loading-image.gif in the new folder.
Alternatively, you can change it directly in the Default folder.




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                           118
7. Login page configuration
The prerequisite for the configuration is the installation of the A+W iQuote login page as
described in the A+W iQuote installation instructions.
The concept behind the login page should be explained first. The login page is a page before A+W
iQuote and that depends on the iQuote. On it, the user logins are managed; users can register
themselves. The user is assigned an iQuote instance.
Registration of the iQuote is done, but no longer with the user's login data, but rather with a one-
time token. The iQuote trusts the login page; a user who has authenticated himself on the login
page is also authenticated in iQuote. The login page and the iQuote have a trust relationship that
is secured with the private key. Only if it is the same in both systems do the systems trust each
other. A user's login data cannot be used to log in into the stand-alone iQuote. The customer
employee login data still works on the stand-alone iQuote, however; it must be deleted.


                                              Token request

         Login page                           Token send                 iQuote

                                              Login + call

                  User credentials are
                  only stored in the local                                Token
                  database
                                                                         storage



             User
          credentials




A+W Software GmbH                            EN-CONFIG-A+W iQuote.docx                           119
7.1. Initial login as administrator
First, there must be a login with the user admin@a-w.com and the password: Adm1n! Then a new
Admin user should be created and the existing Admin user deleted. The new user becomes an
Admin based on their role. There can be several and if the access to the mail address exists, the
password can also be changed.
Attention: if there is no more Admin access, the login page can no longer be administered. Then
the database must be deleted or the admin role assigned to a user via SQL,




A+W Software GmbH                   EN-CONFIG-A+W iQuote.docx                                120
7.2. Pages
For each site, the URL of the iQuote and if necessary the token URL must be entered. These can
differ if there are restrictions between internal and external access. Normally they are the same.
The access from the login page to the iQuote is authorized via a token; for this, however, the
comparison of a private key is required. This private key must be stored here and in the A+W
Business company master data.




Essentially, a default private key is always returned, even if none is entered in A+W Business. This
is a safety feature and prevents uncontrolled access to the system.
CAUTION: a private key must be compared between the login page and A+W Business; otherwise
no connection can be established. Leaving this blank is not an option.
In addition to the private key, the IPv4 or IPv6 of the login page server must be entered here. Only
queries from this computer are permitted.
CAUTION: If permitted IPs are entered, the ipv6 must absolutely be stored ( ":::1" is the local
host). If no IP is entered, then there is also no check; this is a safety feature and should be used if
possible.




The default customer initially serves to map a newly created user to the various customers. This
way, a private customer can also log in and order products. If this feature should not be possible,
this field must be left empty.

A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                    121
A+W iQuote is a B2B configurator; an entry of the default customer number opens the
configurator as B2C. Here, however, there are various requirements for the contract conclusion,
payment methods that can conflict with the country's laws. This must first be clarified.
If the login page has been activated, then the entry of the iQuote password in the customer
employee management is no longer possible. The business case can then be stored in the
customer management.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                122
7.3. User
If a user is created by the administrator, the user receives a mail with the prompt to assign a
password. This mail has a link with a token that is mandatory for the registration.
The customer number defines with which customer the user is logging into A+W Business. If this is
0, then the default customer of the corresponding page is used. If this is also 0, the user can only
log in on the login page, but not change to iQuote.




CAUTION: The mail to the user contains a link with the address (URL) of the login page. This link
address is controlled via the browser's address bar. If the login page is called from an internal
address, the mail contains an internal address link. With it, it is not possible for the user to set his
password, however. Attention must always be paid that the user registration is done from the
public URL. It's best if the computer in the DMZ doesn't have a local address (DNS) and everyone
must always go via the external URL!!!




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                     123
7.4. Links
Via Administration->Links, links to videos (YouTube) and PDF documents can be entered. They
then appear on the login page.
The URL and symbol URL must be specified for PDF links with a relative path, e.g., "Content/...".
There is no access to files from other domains, except for video.




The first entry is displayed automatically.




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                124
7.5. Settings
Via the self-registration, the possibility can be switched off that a customer can register
themselves. If this is deactivated, then only the Administrator can register customers and send
them an invitation mail. In connection with the default customer number, the self-registration
creates a B2C configurator. Here, however, there are various requirements for the contract
conclusion, payment methods that can conflict with the country's laws. This must first be clarified.




Access to the mail server must be configured; this can be checked with the Test Mail button. The
registered Administrator then receives a mail. If an employee should be informed about all
documents, this person can be entered as BCC (blind copy) or as CC.


7.6. User self-registration and password reset
Via the link on the login dialog, a user can register themselves and also reset their password. The
prompt for this comes via mail.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                 125
7.7. Customizing the login page
7.7.1. View layout for customizing
The login page is completely customizable; this affects the CSS part (see iQuote 6) as well as the
HTML part.
The login page always starts with the custom theme if the following files are stored under
Content\custom
~/Content/Custom/custom.css
~/Content/Custom/kendo.custom.less
~/Content/Custom/awsoa-responsive.custom.less

The Custom.css can contain CSS that do not have a direct relationship with Kendo. It can also be
empty, but for recognition, it must be to the folder.
These files can also be obtained from the Custom directory of the iQuote.

For this, custom cshtml pages (ASP.NET Razor Syntax) must be created that are called exactly the
same as the originals.
The view structure is as follows:




The customized page of the main view of the login page is in the Views->Custom->Home
directory.
The menu is implemented in the PartialNavbar.cshtml; here, for example, extensions to the menu
can be entered.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                 126
If a department-specific view is present, then the custom view must have the same name, e.g.
Index.AWB.cshtml.


7.7.2. Custom header and footer
If on the main page only an individual header and footer should be inserted, this can be done
easily with the views
~/Views/Custom/Home/CustomHeader.cshtml
~/Views/Custom/Home/CustomFooter.cshtml
the advantage of this solution is that the "PartialMain.cshtml" view must not be adjusted and thus
the login page can still be updated.
To find these files, the login page must be in the custom theme; on this, see 7.7.1


7.7.3. Adding a view on the menu
If on the menu of the login page a new view should be incorporated, then first a copy of the
PartialNavbar.cshtml must be created in the Custom->Home folder.




The menu can then be extended at any point there.




The Java Script function loadCustom() must only be given the name of the view to be displayed.
The extended menu then looks as follows:




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                 127
7.7.4. Access to customer texts
Access to the texts from the table Core_CustomTexts (see also Chapter 3.4) is via the following
command in a CSHTML view. The character @ introduces C# code.
@HttpContext.Current.GetCustomMessageString(“MYTEXT“)
This is especially important for the creation of individual views on
the login page in order to guarantee multilingual functionality.



7.7.5. Adjustment of the customer mails
For registration and password change, the login page sends mails to the user; these are in a
multilingual default. Of course customers need to adjust these to suit their corporate identity. For
this, the login page offers the opportunity to define these individual texts differently in the
customer texts. These texts are HTML-capable. To create them with SQL, see Chapter 3.4
The following codes are reserved for the mail subject and body and must be entered into the
customer texts:
•        WebLoginSendMailRegisterSubject
•        WebLoginSendMailRegisterBody
•        WebLoginSendMailResetPasswordSubject
•        WebLoginSendMailResetPasswordBody

Here are examples for inserting customer texts:
    INSERT INTO [Core_CustomTexts]
    ([Guid],[VersionId],[LockingToken],[Code],[LanguageCode],[Text],[Description])
    VALUES (newid(),1,'00000000-0000-0000-0000-000000000000',
    N'WebLoginSendMailRegisterSubject', 'de-DE' , N'A+W Registrierung', N'')

    INSERT INTO [Core_CustomTexts]
    ([Guid],[VersionId],[LockingToken],[Code],[LanguageCode],[Text],[Description])
    VALUES (newid(),1,'00000000-0000-0000-0000-000000000000',
    N'WebLoginSendMailRegisterBody', 'de-DE' , N'<html><p>Sie haben sich registriert
    in unserem Konfigurator</p><p>Bitte aktivieren Sie ihr Konto und vergeben sie ein
    Passwort. Klicken bitte <a href="{0}">hier</a></p></html>', N'')

    INSERT INTO [Core_CustomTexts]
    ([Guid],[VersionId],[LockingToken],[Code],[LanguageCode],[Text],[Description])
    VALUES (newid(),1,'00000000-0000-0000-0000-000000000000',
    N'WebLoginSendMailResetPasswordSubject', 'de-DE' , N'A+W Passwort Zurücksetzen',
    N'')

    INSERT INTO [Core_CustomTexts]
    ([Guid],[VersionId],[LockingToken],[Code],[LanguageCode],[Text],[Description])
    VALUES (newid(),1,'00000000-0000-0000-0000-000000000000',
    N'WebLoginSendMailResetPasswordBody', 'de-DE' , N'<html><p>Sie haben ihr Passwort
    vergessen.</p><p>Bitte vergeben Sie ein Neues. Klicken bitte <a
    href="{0}">hier</a></p></html>', N'')

For the mail body texts, a placeholder for the link address with {0} must be provided, otherwise
the mail will not contain a link.


A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                   128
8. Login page Okta configuration
The prerequisite for the configuration is the installation of the "A+W iQuote login page Okta" as
described in the A+W iQuote installation instructions.
The concept behind the login page should be explained first. The login page is a page before A+W
iQuote and that depends on the iQuote. On it, the user logins are managed. The user is assigned
an iQuote instance.
Registration of the iQuote is done, but no longer with the user's login data, but rather with a one-
time token. The iQuote trusts the login page; a user who has authenticated himself on the login
page is also authenticated in iQuote. The login page and the iQuote have a trust relationship that
is secured with the private key. Only if it is the same in both systems do the systems trust each
other. A user's login data cannot be used to log in into the stand-alone iQuote. The stand-alone
iQuote login page is deactivated and thus cannot be reached. A simultaneous operation of both
login systems is not possible.




8.1. Okta platform configuration
Essentially, configuration of the Okta platform can be done in two ways. First manually (not
recommended and therefore not explained here) or through Terraform. Using this tool, it is
possible to use a superior configuration language to bring a cloud or the local infrastructure into
the desired state for execution. First, download the command line tool Terraform by HashiCorp.
The tool must be placed together with the configuration file
(C:\SANDPIPER1\WebLoginOkta\okta.tf) in a secure place (e.g., "C:\Okta"). This is necessary since
after executing the tool, a state screen for the Okta configuration is created. This may not be lost!
This enables you to use a changed okta.tf file to import an update of the configuration. For the
initial configuration, a command line is started with windows + r. Type in "cmd" and confirm with
"ok" as depicted in the figure.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                  129
In the command line, you navigate to the folder "C:\Okta" with the following command.

    cd C:\Okta



First a token must be generated that allows Terraform to make changes to the Okta tenant. A new
token is created for this in the Okta admin panel on the left menu under "Security->API".




This token must be entered in the "okta.tf" file under the "api_token" element. For the
"org_name" and "base_url", see the Okta admin panel.




provider "okta" {
    org_name = "dev-97365395"
    base_url = "okta.com"
    api_token = "<TOKEN>"
}



A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                             130
In addition, the URL that points to the "A+W Web Login Okta" must be entered with https:// as
follows.
variable "WebLoginUrl" {
  type = string
  default = "<WEB_LOGIN_HTTPS_URL>"
}
After these changes have been made, Okta can be configured with Terraform. This is done in the
same folder via the command line using the following commands:


 terraform init
 terraform plan
 terraform apply



8.1.1. Creating a group and assigning a client
A client is represented in Okta by a group. For this, first you must create a new group and then
assign it to the "iQuote" application. Ideally, the group has the same name as the client. On the
menu on the left side, select "Directory" and then the "Group" menu element. See the following
figure.




Then you open the group and assign the "iQuote" application on the "Applications" tab.
Configuration of the client is done with a click on the pen.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                 131
For this, the URL of the iQuote instance must be entered. Important here is that the iQuote is
hosted via a SSL encryption (HTTPS).




8.1.2. Creating a user and connecting with an ERP customer
On the Okta admin panel, select the "Directory->People" element with the left menu.




Here, the screen must be filled out with the user data. Important is that for the "Groups" element,
the group is entered that corresponds to the desired client.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                   132
To complete the user configuration, you must create an assignment to an ERP customer. To do
this, select the user just created.




After the user has been selected, click on the pen in the "iQuote" area on the "Applications" tab.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  133
You can enter the ERPCustomer on the screen that opens. Here, either the default customer or a
specific one can be selected.




8.1.3. The default customer
The default customer initially serves to map a newly created user to the various customers. This
way, a private customer can also log in and order products. If this feature should not be possible,
this field must be left empty.
A+W iQuote is a B2B configurator; an entry of the default customer number opens the
configurator as B2C. Here, however, there are various requirements for the contract conclusion,
payment methods that can conflict with the country's laws. This must first be clarified.
If the login page has been activated, then the entry of the iQuote password in the customer
employee management is no longer possible. The business case can then be stored in the
customer management.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                 134
8.2. Configuration of "A+W iQuote Okta login page"
To switch the new login page live, the "A+W iQuote Okta Login Page" of the Okta tennant must be
made known. This is done with the configuration file
"C:\SANDPIPER1\WebLoginOkta\appsettings.json". The "Okta" rubric must be configured in this
file.
   "Okta": {
      "OktaDomain": "https://<OKTA_TENENT_HERE>.okta.com",
      "ClientId": "<CLIENT_ID_HERE>",
      "ClientSecret": "<SECRET_HERE>",
      "AuthorizationServerId": "default",
      "UseRedirectModel": "true"
   },
For "OktaDomain", see the Okta admin panel as depicted in the figure. Important is that https://
is placed in front of the Okta domain.




For the "ClientId" and "Clientsecret", use the left menu to navigate to the "Application" "iQuote".
Here, the values can be viewed as in the figure and entered.




To apply the configuration, the "Web.Login.Okta" page in the IIS manager must be restarted.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                  135
In the "Clients" area, the private key for the client in question must be stored. For the clientID, see
the A+W Infrastructure WEb.
  "Clients": {
    "default": {
      "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
    },
    "1": {
      "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
    },
    "2": {
      "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
    }
  }


This private key must be stored here and in the A+W Business company master data.
CAUTION: a private key must be compared between the login page and A+W Business; otherwise
no connection can be established. Leaving this blank is not an option.
In addition to the private key, the IPv4 or IPv6 of the login page server must be entered here. Only
queries from this computer are permitted.
CAUTION: If permitted IPs are entered, the ipv6 must absolutely be stored ( ":::1" is the local
host). If no IP is entered, then there is also no check; this is a safety feature and should be used if
possible.




A+W Software GmbH                      EN-CONFIG-A+W iQuote.docx                                    136
8.3. Preparation of iQuote for the Okta login
In the Infrastructure Web, the logout detour to the login page must be configured.




Under the element "Log out redirect URL", the web address of the login page must be entered.
Important here is that the extension of the URL includes "/Account/SignOut".


NOTE: The "Okta" rubric point can be ignored initially since it does not contain any function.
To apply the configuration, the "Web.Web" page in the IIS manager must be restarted.




A+W Software GmbH                     EN-CONFIG-A+W iQuote.docx                                  137
8.4. Customization
As "deployment model", "A+W iQuote Login Okta" relies on the Okta redirect model. See here to
learn more about this. This means that the entire customization happens via Okta itself; see also
Style the sign-in page | Okta Developer.




A+W Software GmbH                    EN-CONFIG-A+W iQuote.docx                                138

